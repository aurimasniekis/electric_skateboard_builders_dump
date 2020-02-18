# Logging/monitoring the vesc

### Replies: 12 Views: 643

## \#1 Posted by: spork Posted at: 2018-04-22T19:30:23.623Z Reads: 121

```
I'm currently running two VESC's in parallel (one to each rear wheel of my mountain board).  Both controlled by a Y'd PPM signal.  I want to log and/or monitor telemetry from at least one vesc using an arduino - while still controlling the vesc via ppm.

I see a lot of threads on the vesc UART, but I haven't found one that walks you through the setup procedure, pinnouts, baud rate, etc.  I think I've found the answer to most of the questions, but one thing I haven't yet found is the correct configuration of the vesc for monitoring/logging via the UART while still  controlling the vesc via ppm.  

I assume I need to go to the "App configuration" tab of the BLDC tool and select "PPM AND UART".  Can someone confirm?

Also, if someone knows of a document or tutorial that can walk me through the setup and configuration to do this it would be most appreciated.
```

---
## \#2 Posted by: Acido Posted at: 2018-04-22T19:32:27.217Z Reads: 119

```
I think you are looking for a bt module
```

---
## \#3 Posted by: spork Posted at: 2018-04-22T19:45:04.325Z Reads: 113

```
Why do you suggest I'm looking for a bluetooth module?  I'm just trying to communicate with an Arduino.
```

---
## \#4 Posted by: Ebisane9 Posted at: 2018-04-22T20:23:25.075Z Reads: 102

```
>  I’m just trying to communicate with an Arduino

...via the UART... in order to get telemetry...https://buildkitboards.com/products/vesc-bluetooth-adapter

BT module does exactly (barring the arduino) what you described and it is plug and play. @jlabs has one on his site linked above

Edit: wording
```

---
## \#5 Posted by: spork Posted at: 2018-04-22T20:47:47.300Z Reads: 89

```
Thanks!  It looks like your link has a link back to this forum that describes the BLDC setup.  I'll give it a try.
```

---
## \#6 Posted by: Ebisane9 Posted at: 2018-04-22T20:49:49.653Z Reads: 86

```
No problemo!
```

---
## \#7 Posted by: oyta Posted at: 2018-04-22T21:10:48.673Z Reads: 79

```
If your need is logging, and you don’t have to use Arduino, you can also check out www.metr.at 

Nice app(s), but you need the metr bt dongle. With this you can log, change settings, set up modes, set up TCP bridge do you don’t have to use an USB cable to connect with the VESC Tool. And more. Not sure how it is when not using CAN though..
```

---
## \#8 Posted by: spork Posted at: 2018-04-22T21:13:19.696Z Reads: 75

```
It looks like that's another app to get the data to a smartphone - right?  I really don't want a smartphone in the mix.  Just want to stream data to an arduino.  And I'm not looking to control the vesc; just read it.
```

---
## \#9 Posted by: banjaxxed Posted at: 2018-04-23T21:15:57.024Z Reads: 61

```
The app can run in your phone in your pocket, it keeps a connection with the bt module and stores  the logs

Presumably ackmaniacs free app does the same thing for android phones
```

---
## \#10 Posted by: spork Posted at: 2018-04-23T21:53:02.323Z Reads: 51

```
I'm planning to make a small LCD dashboard that mounts to my remote control.  I just want it to stream battery voltage, speed, etc.  I really want to avoid a phone.
```

---
## \#11 Posted by: Slak Posted at: 2018-04-24T12:12:57.938Z Reads: 40

```
No BT module needed for what you want to do. All you need is the RollingGecko library to read from the VESC and that's it !

Here's a link : 
https://github.com/RollingGecko/VescUartControl
```

---
## \#12 Posted by: TSG_AU Posted at: 2018-04-24T13:31:39.386Z Reads: 30

```
Just remember to switch to the VESC6 branch if you're running v3.x firmware on your VESC. Also if you use CAN to connect the VESCs together you might be able to log from both of the VESCs. I haven't tried that yet however, and have questions of my own
```

---
