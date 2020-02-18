# Vesc not working - Error ABS_OVER_CURRENT

### Replies: 16 Views: 1092

## \#1 Posted by: Enrico Posted at: 2017-04-12T12:36:03.285Z Reads: 156

```
Hey guys,
Yesterday I went to go re-program my braking and before touching any settings, there was a blinking red/pink light. 

When I went to detect motor again, active sampling had an error code: ABS_OVER_CURRENT. Upon rebooting the vesc and trying the detection again the motor just clicks.

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : -144.0
Current filtered : -137.0
Voltage          : 20.80
Duty             : 0.65
RPM              : 300.6
Tacho            : 2
Cycles running   : 71
TIM duty         : 4038
TIM val samp     : 2112
TIM current samp : 5208
TIM top          : 6192
Comm step        : 3
Temperature      : 31.42


I've checked all 3 phase wires and they're all perfectly fine. 

Any help would be appreciated guys.

Motor: 
5065 BLDC outrunner motor
3-8s
80A
1600w
270kv

Battery: 
24V 60A
(18650 cells)

The vesc I'm using is one with a heatsink.
```

---
## \#2 Posted by: Montiey Posted at: 2017-04-12T14:31:32.605Z Reads: 136

```
140 amps?
Geeze, what setup are you running? I'm lucky if my SK3 will brake at 60A, but still.
If those numbers don't match your motor then you know the problem (the motor).
```

---
## \#3 Posted by: Enrico Posted at: 2017-04-12T15:37:19.818Z Reads: 132

```
How do I adjust? Two days ago everything was perfectly fine
```

---
## \#4 Posted by: Montiey Posted at: 2017-04-12T17:15:06.057Z Reads: 127

```
What motor, what batteries? 140 isn't normal for a single drive, but only your motor's specs can tell for sure.

You might want to check "SLOW ABSOLUTE MAX" in BLCD tool, too. That introduces a mean-filtering delay to the abs_current value which can keep this from happening. But still, 140 amps is alot. Perhaps you have another motor to test with?
```

---
## \#5 Posted by: Guacamoleface Posted at: 2017-04-12T17:48:43.114Z Reads: 116

```
Post your settings or screenshots of the BLDC settings :)
```

---
## \#6 Posted by: Enrico Posted at: 2017-04-12T18:25:59.384Z Reads: 112

```
I tried a different motor, 320Kv but still the same result
```

---
## \#7 Posted by: Enrico Posted at: 2017-04-12T18:28:15.247Z Reads: 111

```
Here are the settings: <img src="/uploads/db1493/original/3X/8/2/82eefd4293e4683a65514bcdc014c457b52e00cc.png" width="690" height="422"><img src="/uploads/db1493/original/3X/b/4/b4d5c9e55c0cb65f30fe90aba02e35c4aae25815.png" width="690" height="422"><img src="/uploads/db1493/original/3X/8/2/820406dfb9f72094eccef12752c90a0073336c29.png" width="690" height="408">
```

---
## \#8 Posted by: Enrico Posted at: 2017-04-12T18:30:14.884Z Reads: 101

```
I have no idea why it's 144 A
```

---
## \#9 Posted by: Enrico Posted at: 2017-04-12T18:37:40.953Z Reads: 103

```
Motor:
5065 BLDC outrunner motor
3-8s
80A
1600w
270kv

Battery: 
Custom welded 18650 cells (24x)
24V at 60A
```

---
## \#10 Posted by: themegak Posted at: 2017-04-12T18:49:35.329Z Reads: 103

```
try 

40 amp batt max and motor max. where did you get your vesc ?
```

---
## \#11 Posted by: Enrico Posted at: 2017-04-12T18:52:45.765Z Reads: 104

```
Came in contact with the guys at Arc Boards EV (from kickstarter).

They had a surplus of Vescs for their boards so I managed to get them to sell me one.
```

---
## \#12 Posted by: themegak Posted at: 2017-04-12T18:57:42.178Z Reads: 104

```
depending on what version of the vesc hardware that was used (yes, all vescs are not equal) the amperage max will vary.  Try lowering both of the motor max and batt max vaules until you stop getting that error.  More times than not, the error you are getting is indicative of too much power being used / requested.  Vescs can be delicate which is why their is such a big difference in price for some vescs over others.  I found 22 to 25 amp max batt will usually result in way less errors/issues on older vesc hardware.
```

---
## \#13 Posted by: Montiey Posted at: 2017-04-12T22:15:32.690Z Reads: 97

```
Try setting ABS MAX to 150 or something (just for a test or two) and see if the motor will run at all. If not then it'd seem like your problem isn't with older hardware or overpowered motors.
```

---
## \#14 Posted by: Shogu12 Posted at: 2017-04-13T00:09:00.906Z Reads: 90

```
I had to replace the drv chip on a Vesc when it had that issue.
```

---
## \#15 Posted by: Enrico Posted at: 2017-04-13T19:33:27.337Z Reads: 82

```
I'm guessing you've got some mad soldering skills then ;)? 

Where'd you get the chip?
```

---
## \#16 Posted by: Shogu12 Posted at: 2017-04-13T21:12:23.782Z Reads: 78

```
It's actually  not that hard you just need the right  tools. I got the chip from mouser.
```

---
