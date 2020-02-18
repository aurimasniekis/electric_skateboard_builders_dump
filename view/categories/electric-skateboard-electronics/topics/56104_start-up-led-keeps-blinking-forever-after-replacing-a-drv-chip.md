# Start up led keeps blinking forever after replacing a DRV chip

### Replies: 16 Views: 349

## \#1 Posted by: Mike_Lemon Posted at: 2018-05-20T18:05:12.828Z Reads: 54

```
Hello all, 

I've got two vescs connected to a battery one of them wen bad so I replaced it's MCU(flashed it with th 2.18V firmware) and replaced the DRV chip now when I hook it to a 6S battery it just keeps the startup blinking for ever no matter the battery voltage setting and won't spin the motor unlike the other vesc  which works properly 

Any idea for what's the problem? 

Also note the CAN bus IC is removed to prevent any other possible issues.

Thanks for helping.
```

---
## \#2 Posted by: danielz Posted at: 2018-05-20T20:21:05.564Z Reads: 43

```
checked your fets with a multimeter?
```

---
## \#3 Posted by: Mike_Lemon Posted at: 2018-05-20T20:23:44.846Z Reads: 42

```
How? check what?
```

---
## \#4 Posted by: danielz Posted at: 2018-05-20T20:47:56.024Z Reads: 37

```
https://www.electric-skateboard.builders/t/vesc-troubleshooting/51502/6

video of me checking mine on this thread
```

---
## \#5 Posted by: Deodand Posted at: 2018-05-20T20:51:46.445Z Reads: 36

```
If the normal LED never quits blinking, it means your vesc is never recieving commands. The LED will go solid when the motor is active. I'm assuming you've connected it over usb and run motor calibration? Does the led go solid when you send a command from the vesc tool? If it works from vesc tool it could be a problem with the servo-input pin not soldered correctly on the mcu or missing passives for the filter circuit on the ppm input pin.
```

---
## \#6 Posted by: Mike_Lemon Posted at: 2018-05-20T20:57:18.440Z Reads: 34

```
Can't see or understand a thing of what is ging on there, How do I check wether the FET is good or not? where to probe? what to expect

[quote="Deodand, post:5, topic:56104, full:true"]
If the normal LED never quits blinking, it means your vesc is never recieving commands. The LED will go solid when the motor is active. I’m assuming you’ve connected it over usb and run motor calibration? Does the led go solid when you send a command from the vesc tool? If it works from vesc tool it could be a problem with the servo-input pin not soldered correctly on the mcu or missing passives for the filter circuit on the ppm input pin.
[/quote]

No I'm telling you nothing other than the motor battery and usb is connected. it can connect to the PC via BLDC and read settings and stuff but will refuse to run the motor with the arrow keys and the same led that makes the blinking thing at power keeps doing that over and over sometimes after power up it won't even blink after some time.
```

---
## \#7 Posted by: Deodand Posted at: 2018-05-20T20:58:48.295Z Reads: 26

```
What color LED is blinking? Red?
```

---
## \#8 Posted by: Mike_Lemon Posted at: 2018-05-20T20:59:43.976Z Reads: 27

```
Yeah that one.
```

---
## \#9 Posted by: Deodand Posted at: 2018-05-20T21:02:01.879Z Reads: 26

```
This means your motor driver is in a fault state. Something is causing it to lock in this mode. You'll need to look at what fault is being triggered in the data tab to try and target the cause.
```

---
## \#10 Posted by: danielz Posted at: 2018-05-20T21:03:02.116Z Reads: 25

```
You can see in the video where each probe is, one on the power input. You need to check the resistances are all the same for all six. One of mine had failed it was doing all kinds of weird things including corrupting its firmware. It also said drv fault, but the drv was fine. Might not be your problem, but only takes a few seconds to rule out.
```

---
## \#11 Posted by: Deodand Posted at: 2018-05-20T21:04:13.186Z Reads: 23

```
Just look at what fault is getting thrown before going to the trouble of probing fets. If its a drv fault then check the fets
```

---
## \#12 Posted by: Mike_Lemon Posted at: 2018-05-20T21:05:52.856Z Reads: 22

```
Well when I type "faults" in the BLDC terminal if says there are no faults.
```

---
## \#13 Posted by: Mike_Lemon Posted at: 2018-05-20T21:06:46.961Z Reads: 23

```
Probing all the FETs Drain to source indicates that all resistances are at around 40.9kOhM+- 2kOhm
```

---
## \#14 Posted by: Deodand Posted at: 2018-05-20T21:10:23.220Z Reads: 22

```
So red led is blinking and faults terminal command says no faults? Strange. Is there any data in the realtime data tab?
```

---
## \#15 Posted by: Mike_Lemon Posted at: 2018-05-20T21:20:16.166Z Reads: 22

```
Actually now I tryed probing the Voltage regulator and a taltalum  blew up in my face gonna have to order the parts to replace it now will check on it later.
```

---
## \#16 Posted by: Mike_Lemon Posted at: 2018-05-20T21:41:11.139Z Reads: 17

```
Fixed it by replacing the cap and the VR but I'm afraid the MCU didn't make it :frowning: nothing to replace it with yet.
```

---
