# Motor is consistently cutting out after 10 minutes / 1 mile

### Replies: 28 Views: 370

## \#1 Posted by: fromualdez Posted at: 2019-07-16T22:47:37.148Z Reads: 92

```
Hey all, 

After 10 minutes of riding (or after 1 mile), my motor starts to cut out (both power and breaking). If I give it a second, it'll start to run in 5 second spurts, with delays in-between growing larger and larger. I've ridden it about 5 times (after tinkering each time), and it happens every time.

I've used the current VESC tool to program the VESC through the simple setup and I'm sure all of me entries are correct.

Also, I was planning to run a dual setup, but every time I run a detection on the second VESC, it immediately disconnects. I don't know if this is related, but I'm just throwing it out there. 

Please help.
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-07-16T22:59:14.177Z Reads: 89

```
What version vesc do you have? If it's a 4.12, a common issue is a temperature sensor with the wrong value, so the vesc thinks it's hotter than it is, causing thermal protection to kick in. Check your realtime monitoring with the vesc on the bench, and you may see a mosfet temperature around 80C, where it should be in the 20s-30s.
```

---
## \#3 Posted by: Soflo Posted at: 2019-07-17T00:25:03.169Z Reads: 78

```
What battery are you running?
```

---
## \#4 Posted by: trampa Posted at: 2019-07-17T01:29:43.726Z Reads: 77

```
More details help to understand the issue. VESC or Clone? Which model? Motor model? Temp sensor in motor?

Your issue is very likely motor temperature related. If you loose acceleration and brakes, it's very likely a wrong temp reading.
```

---
## \#5 Posted by: fromualdez Posted at: 2019-07-17T04:41:30.387Z Reads: 67

```
Hey all, I have a new issue. After troubleshooting both vescs and motors, I got them to work for awhile... but when I started it the last time, it turned on then all the lights went out. The battery indicator, the power button, the VESCs, everything. After a bit, it turned on again (lights that is), but now the motors wont work. 

The VESCs (BLDC ESC 4.12) and motor (MBoards 6374 180KV) are all from MBoards and recently bought. I purchased my battery (10S5P 18650 Lithium Battery Pack 36V, 10Ah, 360Wh).

Here are some pictures below. 

![20190716_213757|281x500](upload://qx1hAq1Q8MRCrBJdj36Iahj7hwm.jpeg) ![20190716_213830|690x388](upload://rwrKGQz0UKpPF9iQxnz0zF7prqb.jpeg) ![20190716_213838|690x388](upload://dadPAeVgxzm2Vtkqws1TuFki8i7.jpeg)
```

---
## \#6 Posted by: fromualdez Posted at: 2019-07-17T04:44:02.935Z Reads: 58

```
I posted again below as a new problem has arisen. As a result, I never got far enough to check my vesc on the bench. Thanks for the reply.
```

---
## \#7 Posted by: MysticalDork Posted at: 2019-07-17T07:10:41.393Z Reads: 53

```
Sounds like the shutting off issue is battery related.  Where did you get the battery from? What cells? What BMS, and is it bypassed or not?
```

---
## \#8 Posted by: fromualdez Posted at: 2019-07-17T12:40:15.915Z Reads: 44

```
I got it from diyeboard.com. Here are the states: 10S5P 18650 Lithium Battery Pack 36V, 10Ah, 360Wh. It states that the bms was built in. As for bypassed, I'm not sure what you mean. I'm currently using an anti spark switch? Thanks for responding.
```

---
## \#9 Posted by: fromualdez Posted at: 2019-07-17T12:43:40.099Z Reads: 44

```
Hi, I have a new issue which I wrote about below. Not sure if you get notifications when I respond. When I last turned it on, the lights flickered, then went out. The motors ran for a quick second, then nothing. For a while, the board wouldn't turn on at all. About 5 minutes later it started up again, but now the motors won't spin. Super disappointed and worried that I broke something...
```

---
## \#10 Posted by: MysticalDork Posted at: 2019-07-17T19:36:50.611Z Reads: 30

```
All right, try bypassing the anti spark switch and see if that changes things. Just unplug it, and connect the vescs straight to your battery.
```

---
## \#11 Posted by: fromualdez Posted at: 2019-07-17T20:35:56.315Z Reads: 30

```
Hi, I unconnected it from the anti spark switch. Same thing happens. Everything powers up but the motors still don't run. I do notice, however, that Everytime I hit the throttle, three red LED lights blink on the VESC. I imagine thats something important? Thanks again!
```

---
## \#12 Posted by: MysticalDork Posted at: 2019-07-17T20:38:18.504Z Reads: 28

```
Try plugging the vescs into your computer and checking the error logs?
```

---
## \#13 Posted by: fromualdez Posted at: 2019-07-17T20:57:43.030Z Reads: 29

```
I'm sorry, but I'm not entirely confident I know how to do that. But this is what I see: 

![Capture|690x367](upload://eDnF0EdnfpP2FMPXiAqolXiAANs.jpeg) 
![Capture|690x371](upload://asRQ6eAHhKlPzwDnejXM6rIPEKA.jpeg)
```

---
## \#14 Posted by: RedEagle Posted at: 2019-07-17T21:02:36.247Z Reads: 25

```
3 blinking red leds means you have a fault code. Try replicating the issue and check for a fault code. Don't disconnect the battery as this will wipe the memory and you will get nothing.
```

---
## \#15 Posted by: MysticalDork Posted at: 2019-07-17T21:05:44.589Z Reads: 26

```
In the vesc terminal, type "faults". Do this while the vesc is still plugged in and powered by the battery. Disconnecting the battery between when you get three flashing lights and when you plug in the computer and read the faults will wipe the memory and you won't get any fault codes.
```

---
## \#16 Posted by: fromualdez Posted at: 2019-07-17T21:19:37.638Z Reads: 24

```
Sigh? Is my VESC done for? "FAULT_CODE_DRV"
```

---
## \#17 Posted by: fromualdez Posted at: 2019-07-17T21:20:15.716Z Reads: 25

```
Thanks so much, as I responded down below, I got this error code: FAULT_CODE_DRV. No good, right?
```

---
## \#18 Posted by: fromualdez Posted at: 2019-07-17T21:23:30.407Z Reads: 23

```
Here's the whole thing... How'd I mess up?

Fault            : FAULT_CODE_DRV
Current          : -0.6
Current filtered : 0.0
Voltage          : 41.67
Duty             : 0.000
RPM              : -0.0
Tacho            : 3
Cycles running   : 2
TIM duty         : 1
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 8400
Comm step        : 0
Temperature      : 25.93
```

---
## \#19 Posted by: RedEagle Posted at: 2019-07-17T21:36:09.117Z Reads: 21

```
Yes, you'd have to get your drv replaced. it could be a number of things, like:
- bad motor detection
- bad/loose connectors
- bad solder job
- shorted phase wires
- bad settings
- bad battery
- bad caps
- switched setup without doing a proper reconfiguration 

to name a few.
```

---
## \#20 Posted by: MysticalDork Posted at: 2019-07-17T21:42:56.033Z Reads: 21

```
I think you've got multiple problems with your build, not just a DRV - That wouldn't explain your lights going out. That  was likely caused by any of the following: Bad BMS, bad battery connection to antispark, bad antispark, bad antispark connection to the rest of the electrical system.

My guess is your initial question of the motor cutting out after a short range was a thermal issue, or maybe a voltage setting? What are your battery cutoff start and battery cutoff end values set at?
```

---
## \#21 Posted by: fromualdez Posted at: 2019-07-17T21:49:24.040Z Reads: 22

```
Do you have any suggestion as to how to proceed and safeguard against this from happening again? Is there a way for me to figure out what happened and what some of the culprits might be?
```

---
## \#22 Posted by: fromualdez Posted at: 2019-07-17T21:50:40.688Z Reads: 22

```
Sigh, do you know how I might be able to isolate the problem? Should I just scrap what I have? I'm not entirely sure what to do..?
```

---
## \#23 Posted by: MysticalDork Posted at: 2019-07-17T21:51:24.620Z Reads: 20

```
Do you have a multimeter?
```

---
## \#24 Posted by: RedEagle Posted at: 2019-07-17T21:52:05.893Z Reads: 21

```
As mentioned earlier, we need your settings and setup before we can make a guess and take it from there.
```

---
## \#25 Posted by: fromualdez Posted at: 2019-07-17T21:53:50.090Z Reads: 22

```
Ok, I'm sorry, I'm really new. Can you tell me what I need to post? Really sorry.
```

---
## \#26 Posted by: fromualdez Posted at: 2019-07-17T21:54:05.495Z Reads: 21

```
No, but I can get one...
```

---
## \#27 Posted by: MysticalDork Posted at: 2019-07-17T21:55:57.665Z Reads: 20

```
Get one. Doesn't have to be a $200 fluke, but a multimeter is an absolute no-exceptions **must-have** for anyone building electric vehicles.
```

---
## \#28 Posted by: RedEagle Posted at: 2019-07-17T22:08:23.695Z Reads: 19

```
Your parts list and the vesc settings. Motor and remote settings specifically.
```

---
