# FAULT_CODE_ABS_OVER_CURRENT fault happens mostly when going over any bump

### Replies: 21 Views: 551

## \#1 Posted by: tylerkend Posted at: 2018-07-12T22:54:56.713Z Reads: 157

```
I built a newish esk8 and it seems to stall for a few seconds if I go over even the smallest bump and sometimes at random. On some rides its fine and only stops once or twice but other times it will stop every few seconds making it impossible to ride. I have about 20km on it so far.

I have tried setting the motor max and batt max lower and increasing the absolute max but it doesn't make a difference. The voltage during the faults seems to be incorrect because my battery was at about 40v but the fault reported it as ~31v

Specs: 
10s4p Samsung 25R battery pack
190kv torque boards motor
FOCBOX
82mm wheels
16t/36t

FOCBOX settings

![Capture|690x407](upload://3BBSFgiR4g0mvWgfK3BwGSFjxoC.PNG)
![Capture1|690x407](upload://bqR4Jkwyjx8APXvZzS9enEqrKmx.PNG)

Here is the faults:
> The following faults were registered since start:
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 134.6
> Voltage          : 31.95
> Duty             : 0.61
> RPM              : 66.1
> Tacho            : 11582
> Cycles running   : 5976
> TIM duty         : 4010
> TIM val samp     : 1898
> TIM current samp : 5165
> TIM top          : 6534
> Comm step        : 6
> Temperature      : 25.11
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 136.2
> Voltage          : 32.49
> Duty             : 0.49
> RPM              : 1018.6
> Tacho            : 14980
> Cycles running   : 12639
> TIM duty         : 3890
> TIM val samp     : 1797
> TIM current samp : 5805
> TIM top          : 8017
> Comm step        : 2
> Temperature      : 25.37
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 130.5
> Voltage          : 31.87
> Duty             : 0.61
> RPM              : 301.2
> Tacho            : 17822
> Cycles running   : 8706
> TIM duty         : 4011
> TIM val samp     : 1899
> TIM current samp : 5162
> TIM top          : 6527
> Comm step        : 6
> Temperature      : 25.57
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 135.3
> Voltage          : 31.25
> Duty             : 0.58
> RPM              : 109.5
> Tacho            : 21202
> Cycles running   : 7000
> TIM duty         : 3979
> TIM val samp     : 1872
> TIM current samp : 5328
> TIM top          : 6912
> Comm step        : 2
> Temperature      : 25.70
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 134.6
> Voltage          : 32.69
> Duty             : 0.46
> RPM              : 14.8
> Tacho            : 34218
> Cycles running   : 4464
> TIM duty         : 3862
> TIM val samp     : 1773
> TIM current samp : 5952
> TIM top          : 8358
> Comm step        : 4
> Temperature      : 26.26
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 137.3
> Voltage          : 31.93
> Duty             : 0.56
> RPM              : 10.8
> Tacho            : 43024
> Cycles running   : 5463
> TIM duty         : 3963
> TIM val samp     : 1858
> TIM current samp : 5417
> TIM top          : 7118
> Comm step        : 2
> Temperature      : 26.95
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 137.7
> Voltage          : 30.48
> Duty             : 0.58
> RPM              : 120.1
> Tacho            : 51802
> Cycles running   : 83770
> TIM duty         : 3987
> TIM val samp     : 1879
> TIM current samp : 5288
> TIM top          : 6818
> Comm step        : 2
> Temperature      : 28.13
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 34.9
> Current filtered : 130.0
> Voltage          : 35.66
> Duty             : 0.75
> RPM              : 72.5
> Tacho            : 56634
> Cycles running   : 5598
> TIM duty         : 4094
> TIM val samp     : 2044
> TIM current samp : 4790
> TIM top          : 5492
> Comm step        : 4
> Temperature      : 28.63
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 133.4
> Voltage          : 32.10
> Duty             : 0.53
> RPM              : 512.7
> Tacho            : 63772
> Cycles running   : 28521
> TIM duty         : 3942
> TIM val samp     : 1841
> TIM current samp : 5530
> TIM top          : 7378
> Comm step        : 2
> Temperature      : 28.86
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 138.0
> Voltage          : 30.59
> Duty             : 0.59
> RPM              : 529.1
> Tacho            : 69922
> Cycles running   : 2652
> TIM duty         : 3991
> TIM val samp     : 1882
> TIM current samp : 5268
> TIM top          : 6773
> Comm step        : 2
> Temperature      : 29.07
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 134.6
> Voltage          : 32.36
> Duty             : 0.46
> RPM              : 5.0
> Tacho            : 83308
> Cycles running   : 30138
> TIM duty         : 3860
> TIM val samp     : 1771
> TIM current samp : 5964
> TIM top          : 8386
> Comm step        : 2
> Temperature      : 28.91
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 131.2
> Voltage          : 32.70
> Duty             : 0.50
> RPM              : 0.1
> Tacho            : 87450
> Cycles running   : 16334
> TIM duty         : 3910
> TIM val samp     : 1813
> TIM current samp : 5700
> TIM top          : 7773
> Comm step        : 4
> Temperature      : 28.84
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 132.3
> Voltage          : 32.21
> Duty             : 0.57
> RPM              : 1034.2
> Tacho            : 90224
> Cycles running   : 6665
> TIM duty         : 3978
> TIM val samp     : 1871
> TIM current samp : 5337
> TIM top          : 6932
> Comm step        : 2
> Temperature      : 28.78
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 136.6
> Current filtered : 130.6
> Voltage          : 39.89
> Duty             : 0.20
> RPM              : -0.0
> Tacho            : 94361
> Cycles running   : 0
> TIM duty         : 840
> TIM val samp     : 1995
> TIM current samp : 4095
> TIM top          : 4200
> Comm step        : -1
> Temperature      : 28.86
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 0.4
> Current filtered : 133.6
> Voltage          : 40.20
> Duty             : -0.00
> RPM              : 1117.7
> Tacho            : 122334
> Cycles running   : 26070
> TIM duty         : -263
> TIM val samp     : 131
> TIM current samp : 26505
> TIM top          : 52747
> Comm step        : 6
> Temperature      : 30.04
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 132.9
> Current filtered : 130.2
> Voltage          : 39.89
> Duty             : 0.19
> RPM              : 1.6
> Tacho            : 125973
> Cycles running   : 0
> TIM duty         : 780
> TIM val samp     : 1995
> TIM current samp : 4095
> TIM top          : 4200
> Comm step        : -1
> Temperature      : 30.33
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 132.1
> Voltage          : 32.10
> Duty             : 0.60
> RPM              : 60.4
> Tacho            : 125980
> Cycles running   : 1052
> TIM duty         : 4001
> TIM val samp     : 1891
> TIM current samp : 5211
> TIM top          : 6640
> Comm step        : 6
> Temperature      : 30.39
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 130.7
> Voltage          : 32.36
> Duty             : 0.49
> RPM              : 288.1
> Tacho            : 130440
> Cycles running   : 5537
> TIM duty         : 3895
> TIM val samp     : 1801
> TIM current samp : 5777
> TIM top          : 7953
> Comm step        : 2
> Temperature      : 31.32
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 131.2
> Voltage          : 32.25
> Duty             : 0.56
> RPM              : 87.1
> Tacho            : 313108
> Cycles running   : 2956
> TIM duty         : 3968
> TIM val samp     : 1863
> TIM current samp : 5390
> TIM top          : 7054
> Comm step        : 6
> Temperature      : 37.25
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 130.7
> Voltage          : 31.96
> Duty             : 0.56
> RPM              : 73.4
> Tacho            : 323712
> Cycles running   : 41463
> TIM duty         : 3968
> TIM val samp     : 1863
> TIM current samp : 5387
> TIM top          : 7048
> Comm step        : 6
> Temperature      : 36.39
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 119.1
> Current filtered : 131.0
> Voltage          : 39.96
> Duty             : -0.00
> RPM              : 2689.1
> Tacho            : 335749
> Cycles running   : 67253
> TIM duty         : -263
> TIM val samp     : 131
> TIM current samp : 26505
> TIM top          : 52747
> Comm step        : -1
> Temperature      : 37.34
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 156.0
> Current filtered : 131.6
> Voltage          : 39.80
> Duty             : 0.00
> RPM              : 768.8
> Tacho            : 351287
> Cycles running   : 0
> TIM duty         : 0
> TIM val samp     : 247
> TIM current samp : 2347
> TIM top          : 4200
> Comm step        : -1
> Temperature      : 37.80
> 
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
> Current          : 139.7
> Current filtered : 130.2
> Voltage          : 39.62
> Duty             : 0.00
> RPM              : 483.7
> Tacho            : 365831
> Cycles running   : 0
> TIM duty         : 0
> TIM val samp     : 183
> TIM current samp : 2283
> TIM top          : 4200
> Comm step        : -1
> Temperature      : 38.09

Does anyone have any troubleshooting ideas or can see anything wrong with my setup.
I have looked through a bunch of threads here but I cant seem to find anything that relates to this.
EDIT: It happens at any speed including slower than a walking speed.
```

---
## \#2 Posted by: Lionpuncher Posted at: 2018-07-12T23:02:39.520Z Reads: 125

```
Doing a small search on this forum reveals to me you might have something funky going on with your vesc. Do a quick search you'll likely find the answer.
```

---
## \#3 Posted by: Sebike Posted at: 2018-07-12T23:05:34.873Z Reads: 128

```
My guess would be a loose connection somewhere creating a short amp spike. Check if your bullet connectors have a tight connection etcetera..
```

---
## \#4 Posted by: tylerkend Posted at: 2018-07-12T23:17:44.884Z Reads: 123

```
I have made sure the bullet connectors, sensor connector and the input power cables are all connected well.
```

---
## \#5 Posted by: tylerkend Posted at: 2018-07-12T23:20:06.629Z Reads: 126

```
I have tried searching it but nothing seems to relate to my exact problem.
```

---
## \#6 Posted by: RedEagle Posted at: 2018-07-12T23:21:00.498Z Reads: 125

```
This happens when components are not soldered on correctly. Check your caps and shunts. Sometimes problems only come to light under close scrutiny, like two bridged legs or small solder balls etc.

EDIT: This could also be caused by long battery wires(ripple current). For every additional 30cm of battery wire going to the vesc, caps should be added.
```

---
## \#7 Posted by: tylerkend Posted at: 2018-07-12T23:35:49.121Z Reads: 125

```
Thanks for the response!
I am not sure how to check the components on the FOCBOX as it is all screwed together. I might try opening it up and look and my battery wires are 10 gauge and about 50cm for the wiring between the cells and about 40cm straight from the negative and positive terminal to the FOCBOX. How big of capacitors should i consider adding?
```

---
## \#8 Posted by: RedEagle Posted at: 2018-07-12T23:44:45.259Z Reads: 117

```
63v 1000 uF
```

---
## \#9 Posted by: tylerkend Posted at: 2018-07-12T23:50:01.982Z Reads: 116

```
will a 50v 2200uF capacitor work cause my batteries are at 42v and they are the only ones i have on hand.
```

---
## \#10 Posted by: RedEagle Posted at: 2018-07-12T23:53:10.043Z Reads: 118

```
That'll work fine.
```

---
## \#11 Posted by: lrdesigns Posted at: 2018-07-13T02:25:44.998Z Reads: 103

```
I was going to say that maybe the capacitor legs had broken from vibration.
```

---
## \#12 Posted by: PartyPoison Posted at: 2018-07-13T02:42:45.128Z Reads: 103

```
I had this problem before,  when i test my settings, all are good/working but when i enclosed it in the board, it didnt work, and have same faults, i did was, i re-routed my wires, made it short and secure ( make sure wires doesn't move)  and all is working!
```

---
## \#13 Posted by: tylerkend Posted at: 2018-07-13T03:45:11.760Z Reads: 103

```
with the added capacitor I am still getting the same faults.
I also opened the FOCBOX and both the capacitors were attached and all of the rest of the components looked fine.
Any other ideas?

    The following faults were registered since start:

    Fault            : FAULT_CODE_ABS_OVER_CURRENT
    Current          : 82.4
    Current filtered : 137.3
    Voltage          : 36.64
    Duty             : 0.30
    RPM              : 1212.6
    Tacho            : 73264
    Cycles running   : 11092
    TIM duty         : 3567
    TIM val samp     : 1685
    TIM current samp : 7687
    TIM top          : 12004
    Comm step        : 4
    Temperature      : 31.29

    Fault            : FAULT_CODE_ABS_OVER_CURRENT
    Current          : 101.5
    Current filtered : 133.6
    Voltage          : 36.34
    Duty             : 0.23
    RPM              : 882.5
    Tacho            : 76105
    Cycles running   : 763
    TIM duty         : 3340
    TIM val samp     : 1477
    TIM current samp : 8877
    TIM top          : 14800
    Comm step        : 1
    Temperature      : 31.21

    Fault            : FAULT_CODE_ABS_OVER_CURRENT
    Current          : 120.2
    Current filtered : 132.5
    Voltage          : 38.79
    Duty             : 0.00
    RPM              : 378.6
    Tacho            : 115613
    Cycles running   : 750
    TIM duty         : 263
    TIM val samp     : 131
    TIM current samp : 26505
    TIM top          : 52747
    Comm step        : 5
    Temperature      : 33.02

    Fault            : FAULT_CODE_ABS_OVER_CURRENT
    Current          : 156.0
    Current filtered : 131.3
    Voltage          : 33.50
    Duty             : 0.60
    RPM              : 656.9
    Tacho            : 116550
    Cycles running   : 13024
    TIM duty         : 4003
    TIM val samp     : 1892
    TIM current samp : 5204
    TIM top          : 6624
    Comm step        : 2
    Temperature      : 32.10

    Fault            : FAULT_CODE_ABS_OVER_CURRENT
    Current          : 156.0
    Current filtered : 131.8
    Voltage          : 34.27
    Duty             : 0.33
    RPM              : 591.1
    Tacho            : 118649
    Cycles running   : 2274
    TIM duty         : 3648
    TIM val samp     : 1590
    TIM current samp : 7092
    TIM top          : 11004
    Comm step        : 5
    Temperature      : 32.07

    Fault            : FAULT_CODE_ABS_OVER_CURRENT
    Current          : 156.0
    Current filtered : 132.8
    Voltage          : 33.67
    Duty             : 0.46
    RPM              : 556.9
    Tacho            : 119376
    Cycles running   : 5037
    TIM duty         : 3861
    TIM val samp     : 1771
    TIM current samp : 5960
    TIM top          : 8378
    Comm step        : 2
    Temperature      : 31.93
```

---
## \#14 Posted by: Eboosted Posted at: 2018-07-13T05:23:38.968Z Reads: 94

```
Open your Focbox one if the caps legs is broken
```

---
## \#15 Posted by: tylerkend Posted at: 2018-07-14T21:25:55.055Z Reads: 81

```
I checked and the capacitor legs are still attached
```

---
## \#16 Posted by: RedEagle Posted at: 2018-07-14T22:54:59.128Z Reads: 82

```
Can you upload your vesc settings?
```

---
## \#17 Posted by: tylerkend Posted at: 2018-07-15T17:25:24.163Z Reads: 79

```
I posted the motor and BLDC settings in the original post. Do you want screenshots of other setting pages?
I have updated the FOCBOX firmware from 2.18 to 3.37 or 3.38 and switched the motor to foc mode and it seems to work now but i did not get to do any extensive testing yet.
```

---
## \#18 Posted by: DeathCookies Posted at: 2018-07-15T17:52:32.999Z Reads: 80

```
If it still doesnt work properly attach some pictures of the vesc PCB. That way we can See if it looks faulty or not
```

---
## \#19 Posted by: RedEagle Posted at: 2018-07-16T17:51:04.190Z Reads: 76

```
I was getting shutdowns at some point when I passed over tram rails. My solution was slowing down at 15 km/h.
```

---
## \#20 Posted by: TarzanHBK Posted at: 2018-07-17T13:59:53.328Z Reads: 68

```
sounds like something is loose somewhere, could be a whole lot of things - might even be the motor shorting under impacts. Check all connections and components, if nothing helps, try a new vesc
```

---
## \#22 Posted by: RedEagle Posted at: 2018-08-01T00:46:26.622Z Reads: 53

```
https://www.electric-skateboard.builders/t/ever-get-an-over-current-fault-check-your-motor-for-shorts/35286
```

---
