# Read Data Send By a Nano Remote With Arduino

### Replies: 5 Views: 422

## \#1 Posted by: SpartanFrench Posted at: 2018-05-07T13:48:59.064Z Reads: 64

```
Hi guys,

Do you know if there is a way to **read data send by a nano remote** with an **arduino**.

My goal is to **detect** when I push the **throttle** and when I pull the **brake** with an arduino.
I am making a rear light on my Helmet with RGB strip and want them to blink hard when I brake.

Thank you guys.
```

---
## \#2 Posted by: skelstar Posted at: 2018-05-07T21:16:49.781Z Reads: 53

```
If you have a VESC then you could put the "Application" mode (?) into PPM-UART and then hook the Arduino up to the UART port pins and use [this](https://github.com/RollingGecko/VescUartControl) library, or [this](https://github.com/bastianraschke/ESP8266VESC) library (esp if you're using ESp32/ESp8266). You can then read current/speed values and have the arduino work out what the controller is doing.

It's not technically reading the remote, it's reading what the controller's behaviour is.

Clear as mud? :)
```

---
## \#3 Posted by: wafflejock Posted at: 2018-05-08T00:11:23.812Z Reads: 41

```
Yeah only way to read the remote signals would be to know what protocol and frequency they're using exactly (which channel and what base band).

You could possibly reverse engineer it easiest way is probably to just disassemble and look at what chipset it's using but creating a generic receiver might be difficult (HackRF is basically a generic receiver but not cost effective really more just for fun at that point).

You can have multiple receivers with say an nrf on both and one nrf transmitter then both receivers can capture the transmitted signal, but again it depends on being able to tune in and decode whatever the data stream is from the nano.  Alternatively like @skelstar was saying you can probably use a pair of esp8266 to transmit from the VESC and receive in the helmet for the lighting control.
```

---
## \#4 Posted by: skelstar Posted at: 2018-05-08T00:43:42.904Z Reads: 28

```
I have 100s of hours mucking around with a pair of ESP32s and getting them to talk to each other. Best bet is probably Bluetooth (ESP32 has built-in Bluetooth), but the Bluetooth stack is hard work.

I tried ESPNow (wifi-based, think it might be websocket) but abandoned that too. Also tried painlessMesh (google it... there is a github repo out there).

If speed is an issue then just buy a couple of nRF24L01 modules (stupid cheap) and just deal with the 7 wires that you have to solder tot he ESps at both ends (yuck).
```

---
## \#5 Posted by: PI3RR3 Posted at: 2018-07-20T23:28:01.271Z Reads: 14

```
Wire the receiver's data pin to a PWM pin, and also VCC and GND to your arduino, then use pulseIn function.
In my case, I have values around 1800 when I push the throttle (2000 if speed switch of the remote is pushed), 1500 when released and 1100 when braking.

If anyone knows how to replace the nano remote/receiver with an Arduino, I am interested.

    const int receiver1 = 11;
    unsigned long ch1;

    void setup ()
    {
      Serial.begin(9600);
      pinMode(receiver1, INPUT);
    }

    void loop()
    {
      ch1 = pulseIn(receiver1, LOW);
      Serial.print("Ch1 = ");
      Serial.println(ch1);

      delay(20);
    }
```

---
