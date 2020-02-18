# Arduino-Vesc Uart communication problem

### Replies: 4 Views: 1377

## \#1 Posted by: goldenHusky Posted at: 2017-03-11T21:25:53.809Z Reads: 160

```
Hi,

has anybody experience with an Arduino Mega + the runningpenguin library for Uart communication for the Vesc ?

https://github.com/RunningPenguin/VescUartControl

I always get „Failed to get data from VESC1!“ when reading values from the Vesc.

Setup: 
• Arduino Mega
• 2x Vesc with FW 2.18
• Arduino IDE 1.8.1

Uart is set in the app tab and also the baudrate is set to 256 800 in bldc tool, as written in the description of the library.
The strange thing is, that the Vesc1.UartSetCurrent(); function works, so the communication parameter must be correct. Furthermore I receive data from the Vesc when using RollingGeckos Library (which is the original library where the penguin lib is forked from), but I need independent control of 2 vesc via uart for a project..

I would really appreciate it, if someone could give me a hint or have a quick look at the libraries code.. I'm not a software pro :sweat:
Thank you!
```

---
## \#2 Posted by: Pedrodemio Posted at: 2017-03-13T12:58:39.544Z Reads: 131

```
Are booth VESCs connected via can? It are you splitting the ex/tx lines to the two VESCs?
```

---
## \#3 Posted by: goldenHusky Posted at: 2017-03-13T19:41:19.142Z Reads: 116

```
Hi,

they aren't connected via CAN. Each Vesc has an individual uart connection to an Arduino Mega, so Vesc1 goes to Serial1 (Rx1 and Tx1) and Vesc2 to Serial2( Rx2 and Tx2). I think it's a software problem..
```

---
## \#4 Posted by: Pedrodemio Posted at: 2017-03-14T14:40:23.310Z Reads: 104

```
I see, I've never tried this way

I think you need to modify the library for it to work, if you try to use to instances of it, they would share all variables and the data will be a mess, with information from both VESCs
```

---
