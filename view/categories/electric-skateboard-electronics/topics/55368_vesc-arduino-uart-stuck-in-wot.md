# VESC Arduino UART Stuck in WOT

### Replies: 4 Views: 507

## \#1 Posted by: ZFreaky Posted at: 2018-05-14T02:36:53.400Z Reads: 78

```
Hey guys,

I've got an issue where my VESC stays in Wide Open Throttle if left at WOT for more than a second with the nunchuck set command. It appears that the UART connection locks up as the rpm read stays at one place but the BLDC tool shows it fluctuating. If I swing the throttle back and forth it sometimes breaks out of the lock, but the minimum time it stays in the lock is unacceptable. Now apparently if I limit the rpm in the BLDC tool to before the battery can't push the motor any faster, the issues stops, so it appears to only happen when the motor can't spin to the software rpm limit, could be the VESC breaking itself out of the lock. The throttle indicator in the nunchuck setup screen also locks up, but the mega I'm using as the commanding UART is still responsive, no idea what's causing it, any help would be appreciated.

    #include <SPI.h>
    //Using the nRF34 library from https://github.com/TMRh20/RF24
    #include <nRF24L01.h>
    #include "RF24.h"
    #include "printf.h"

    //Library for VESC UART
    //#define DEBUG 
    #include "Config.h"
    #include "VescUart.h"
    #include "datatypes.h"
    #include "local_datatypes.h"

    RF24 radio(7,8);

    //Define variables for remote
    struct remotePackage remPack;
    bool recOK = true;
    uint32_t lastTimeReceived = 0;

    uint32_t t1 = 0;
    uint32_t t2 = 0;

    struct bldcMeasure VescMeasuredValues;

    byte counter = 1;

    const uint64_t pipes[2] = { 0xABCDABCD71LL, 0x544d52687CLL };
    int8_t persXJoy = 0;

    void setup() {
      // put your setup code here, to run once:
        SERIALIO.begin(115200);
      
      //SEtup debug port
      DEBUGSERIAL.begin(115200);
      //SetDebugSerialPort(&DEBUGSERIAL);
      
      SetSerialPort(&SERIALIO);
      radio.begin();
      radio.setAutoAck(1);                    // Ensure autoACK is enabled
      radio.enableAckPayload();               // Allow optional ack payloads
      radio.enableDynamicPayloads();
      radio.setChannel(0x68);
      radio.setRetries(0,15);                 // Smallest time between retries, max no. of retries
      radio.setPALevel(RF24_PA_MAX);              // Here we are sending 1-byte payloads to test the call-response speed
      radio.openWritingPipe(pipes[0]);        // Both radios listen on the same pipes by default, and switch when writing
      radio.openReadingPipe(1,pipes[1]);
      radio.startListening();   

      remPack.valXJoy     = 512; //middle Position
      remPack.valYJoy     = 512;
      remPack.valLowerButton  = 0;
      remPack.valLowerButton  = 0;
      //Serial.println("setup done");
      //VescUartGetValue(VescMeasuredValues);
    }

    void loop() {
      // put your main code here, to run repeatedly:
    //  Serial.println((millis() - t2));
    //  if ((millis() - t2) > 10) {
    //    VescUartGetValue(VescMeasuredValues);
    //    t2 = millis();
    //    Serial.println("read");
    //  }
      VescUartGetValue(VescMeasuredValues);
      //radio.writeAckPayload(pipes[0], &VescMeasuredValues, sizeof(VescMeasuredValues));
      
      //byte pipeNo;
      //Get data from TX                                    // Dump the payloads until we've gotten everything
      while ( radio.available(pipes[1])) {
        radio.read(&remPack, sizeof(remPack));
        radio.writeAckPayload(pipes[0], &VescMeasuredValues, sizeof(VescMeasuredValues));
        recOK = true;
        //Serial.println("catch");
      }

      VescUartSetNunchukValues(remPack);
      uint32_t now = millis();

      if (recOK == true)
      {
        lastTimeReceived = millis();


        recOK = false;
      }
      //Check if package were received within timeout
      else if ((now - lastTimeReceived) > 500)
      {
        remPack.valXJoy = 128; //middle Position
        remPack.valYJoy = 128;
        remPack.valUpperButton = false;
        remPack.valLowerButton = false;

      }
      Serial.println(remPack.valYJoy);
      
    }
```

---
## \#2 Posted by: aethyr Posted at: 2018-05-15T18:00:15.013Z Reads: 31

```
Its been a while since I've done arduino coding, but I seem to recall that debug logging could eat up a lot of cpu/bandwidth on the serial port. You might also try introducing a delay() in the main loop() - its possible you're spamming the UART channel with too many read requests a second?

I also know nothing about how this arduino and nunchuck is integrated with the vesc? What is the arduino used for here? Just as an interface between the vesc and nunchuck?
```

---
## \#3 Posted by: ZFreaky Posted at: 2018-05-15T18:23:08.430Z Reads: 31

```
I tried a vector of the delay method with this:

> //  if ((millis() - t2) > 10) {
//    VescUartGetValue(VescMeasuredValues);
//    t2 = millis();
//    Serial.println("read");
//  }

It's similar to delay() but works as a flag instead of a cpu seize since I want to set the control values as quickly as possible, however for some reason the read function refuses to work if it's not continuously called.

The arduino is working as an interface between the nunchuck radio and vesc, future plans involve peripherals that I don't wanna code the vesc for.

I did more experimenting and found that if I put in a duty cycle limit to 90% instead of the stock 95%, it won't lock up. I don't believe it's a UART hogging issue, because it only locks up once it reaches 95% duty cycle, not anywhere else throughout the input arc with the same sample and input rate so something in the vesc is failing when it's trying to get passed that duty cycle. I admit I haven't tried this with other control methods such as PPM, I2C or analogue, so it might be exclusive to the UART control. Idk, I'm hoping the duty cycle limiting will work.
```

---
## \#4 Posted by: iscle Posted at: 2018-05-16T18:30:03.505Z Reads: 20

```
Hi! 

I'm not sure which Arduino board are you using, but if it's NOT an Arduino Nano, Uno or Pro Mini (an Arduino Mega 2560 or STM32F103C8 board will work, because both have more than one Serial (currently using Serial1) and enought memory for the sketch), you can try my new library which I'm using in my electric longboard running the latest VESC firmware. Right now I have only tested the setChuckValues functions.

This is the library: https://github.com/Iscle/VESC_Arduino_Library
This is the sketch I'm using: https://gist.github.com/Iscle/ba6b96ae57336c7717b587f61384a9c2

It might be a little confusing now, as I haven't got time to clean everything up and comment the code, but if you know a bit of C or C++ I'm sure you will be able to adapt my sketch to your likings!
```

---
