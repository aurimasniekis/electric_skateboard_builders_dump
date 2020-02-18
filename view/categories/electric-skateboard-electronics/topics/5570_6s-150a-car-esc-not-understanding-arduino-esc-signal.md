# 6S 150A Car ESC not understanding arduino ESC signal

### Replies: 7 Views: 990

## \#1 Posted by: michaeld33 Posted at: 2016-07-04T22:04:45.082Z Reads: 121

```
I have a remote with a RF transmitter, connected to an Arduino with a receiver, using the code below, and when the Arduino is connected to the ESC, the ESC doesn't understand the signal it is receiving. The ESC does work since I can use my quadcopter controller with it, but it doesn't work with the code I am using. I have attached the code below:

/* 
Analog Signal Receiver
Receiving an Analog Signal over VirtualWire 
Developed by Michael Delaney
*/

#include <VirtualWire.h>
#include <Servo.h>

const int transmit_pin = 12;
const int receive_pin = 2;
const int transmit_en_pin = 3;
int ledPin = 13;

int potData;



Servo esc;

// RF Transmission container
char potMsg[4]; 

void setup() {
  Serial.begin(9600);
  
  // sets the digital pin as output
  pinMode(ledPin, OUTPUT);  
  esc.attach(9); 
  //ESC.setMinimumPulse(800);
  //ESC.setMaximumPulse(2000);   
    
    // VirtualWire 
    // Initialise the IO and ISR
    // Required for DR3100
    vw_set_tx_pin(transmit_pin);
    vw_set_rx_pin(receive_pin);
    vw_set_ptt_pin(transmit_en_pin);
    vw_set_ptt_inverted(true); 
    // Bits per sec
    vw_setup(2000);     
    
    // Start the receiver PLL running
    vw_rx_start();       

} // END void setup

void loop(){
    uint8_t buf[VW_MAX_MESSAGE_LEN];
    uint8_t buflen = VW_MAX_MESSAGE_LEN;
    
    // Non-blocking
    if (vw_get_message(buf, &buflen)) 
    {
    int i;
        // Turn on a light to show received good message 
        digitalWrite(13, true); 
    
        // Message with a good checksum received, dump it. 
        for (i = 0; i < buflen; i++)
    {            
          // Fill Sensor1CharMsg Char array with corresponding 
          // chars from buffer.   
          potMsg[i] = char(buf[i]);
    }
        
        // Null terminate the char array
        // This needs to be done otherwise problems will occur
        // when the incoming messages has less digits than the
        // one before. 
        potMsg[buflen] = '\0';
        
        // Convert Sensor1CharMsg Char array to integer
        potData = atoi(potMsg);
        potData=map(potData,0,1023,0,179);
        esc.write(potData);
        
        
        // DEBUG 
        Serial.print("Sensor 1: ");
        Serial.println(potData);
        
        // END DEBUG
                
        // Turn off light to and await next message 
        digitalWrite(13, false);
    }
}
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-07-05T00:02:58.790Z Reads: 88

```
Figured it out, the signal was getting muted by the ESC, working on building a circuit to fix the problem
```

---
## \#3 Posted by: brandon Posted at: 2016-10-13T13:49:12.243Z Reads: 53

```
Did you ever come up with a solution? I'm betting I'm dealing with the exact same problem though I haven't broken out the oscope to check, since I have the exact same results with the same esc.
```

---
## \#4 Posted by: michaeld33 Posted at: 2016-10-14T13:11:30.699Z Reads: 48

```
Yes and no, it was receiving the correct signal, but there were library compatibility issues so I ended up not being able to use it. If you want to do it, I would recommend using bluetooth. A friend of mine did and his board works fine.
```

---
## \#5 Posted by: brandon Posted at: 2016-10-14T21:38:24.144Z Reads: 41

```
I got it working :)
```

---
## \#6 Posted by: Maxid Posted at: 2016-10-14T21:49:44.260Z Reads: 39

```
Could you tell us what you did to get it working? A topic with instructions would be great.
```

---
## \#7 Posted by: brandon Posted at: 2016-10-14T21:58:32.350Z Reads: 38

```
I intend to create a very exhaustive article on interfacing with speed controllers as soon as I get everything working well.

I think my issue was calibrating the esc as the manual is in very broken English. After calibration though, it seems to work without any problem. I did ~10 miles today until I melted my pulleys.
```

---
