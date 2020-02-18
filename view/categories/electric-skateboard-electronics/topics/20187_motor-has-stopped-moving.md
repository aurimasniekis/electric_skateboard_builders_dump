# Motor has stopped moving

### Replies: 30 Views: 1538

## \#1 Posted by: Koto Posted at: 2017-04-03T08:08:06.098Z Reads: 126

```
okay, so i was going for my 3rd ride, when my esk8 randomly started cutting out. after observing this i stopped riding and walked home. My batteries were very low, but i recharged them and they seem fine because everything turns on when i plug in. another culprit may be the motor, for i hadn't fastened down the motor pulley enough and it scraped a bit on the outside. suspect 3 - by this time the motor had completely cut out. The vesc may be to blame. i realised as i turned on the Vesc, there was a red light that flashed three times, and as i pressed the controller no white light came on. when i turned the vesc off, a red light flashed once. Also, i tried doing "start detection" on the BLDC tool, and it came up with  "Bad Detection Results recieved" .Thanks for reading, Is there a way to fix? 

Thanks, _xXKOTOXx_
```

---
## \#2 Posted by: Hummie Posted at: 2017-04-03T08:17:25.739Z Reads: 120

```
put the vesc on the pc and do the bldc ...motor test
```

---
## \#3 Posted by: Koto Posted at: 2017-04-03T08:19:12.662Z Reads: 118

```
@Hummie did the "start detection" and it comes up with "bad detection"
```

---
## \#4 Posted by: Hummie Posted at: 2017-04-03T08:21:17.797Z Reads: 112

```
then I bet your vesc is probably fine and the motor is not.
```

---
## \#5 Posted by: laurnts Posted at: 2017-04-03T08:21:54.241Z Reads: 109

```
Seems not vesc problem, but either battery or motor. I think its battery issue. If you use lipo and drained them completely, although its charging will never last a minute to ride.
```

---
## \#6 Posted by: Hummie Posted at: 2017-04-03T08:22:09.158Z Reads: 105

```
check your motor leads and make sure they are well insulated and not touching.  look inside if you can and see.
```

---
## \#7 Posted by: Koto Posted at: 2017-04-03T08:22:11.152Z Reads: 102

```
@Hummie Thoughts? what do you think i should do.
```

---
## \#8 Posted by: Hummie Posted at: 2017-04-03T08:23:45.264Z Reads: 100

```
are your batteries up to voltage ? maybe you can fail the test with low batteries.  

its hard to tell if a motor is shorted.  a multimeter is rarely accurate enough.  you can get an inductance meter for like 12bucks and they're really accurate.
```

---
## \#9 Posted by: Koto Posted at: 2017-04-03T08:24:05.384Z Reads: 98

```
what do you think the red flashing means
```

---
## \#10 Posted by: Hummie Posted at: 2017-04-03T08:24:45.989Z Reads: 89

```
i think it's in the bldc program.  and then the terminal tab and literally type faults.  I think
```

---
## \#11 Posted by: flatsp0t Posted at: 2017-04-03T08:25:04.223Z Reads: 85

```
Well first things first:

Can you go to the Terminal tab after you got a failed detection and type faults there.
```

---
## \#12 Posted by: Koto Posted at: 2017-04-03T08:25:09.367Z Reads: 81

```
ill send a video
```

---
## \#13 Posted by: Koto Posted at: 2017-04-03T08:26:39.695Z Reads: 88

```
How @flatsp0t
```

---
## \#14 Posted by: flatsp0t Posted at: 2017-04-03T08:28:52.674Z Reads: 118

```
Do a motor detection again, let it fail.
then go to the Terminal tab, type faults in the text box and click send.
<img src="/uploads/db1493/original/3X/b/4/b4c145c65b93ae9f042fca329f6e4e83ce60af0a.png" width="650" height="500">
```

---
## \#15 Posted by: Koto Posted at: 2017-04-03T08:29:56.868Z Reads: 118

```
Fault            : FAULT_CODE_DRV8302
Current          : -0.8
Current filtered : 0.0
Voltage          : 31.41
Duty             : 0.02
RPM              : 0.0
Tacho            : 1
Cycles running   : 4
TIM duty         : 866
TIM val samp     : 441
TIM current samp : 23107
TIM top          : 45331
Comm step        : 2
Temperature      : 29.18

Fault            : FAULT_CODE_DRV8302
Current          : 0.5
Current filtered : -0.1
Voltage          : 31.42
Duty             : 0.02
RPM              : 1.0
Tacho            : 2
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 3
Temperature      : 29.15

Fault            : FAULT_CODE_DRV8302
Current          : 0.3
Current filtered : -0.2
Voltage          : 31.41
Duty             : 0.03
RPM              : 1.4
Tacho            : 3
Cycles running   : 4
TIM duty         : 1160
TIM val samp     : 609
TIM current samp : 21453
TIM top          : 41687
Comm step        : 4
Temperature      : 29.18

Fault            : FAULT_CODE_DRV8302
Current          : -0.5
Current filtered : -0.4
Voltage          : 31.42
Duty             : 0.02
RPM              : 3.0
Tacho            : 6
Cycles running   : 4
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 1
Temperature      : 29.20

Fault            : FAULT_CODE_DRV8302
Current          : -0.0
Current filtered : 0.3
Voltage          : 31.41
Duty             : 0.02
RPM              : 1.9
Tacho            : 7
Cycles running   : 3
TIM duty         : 834
TIM val samp     : 442
TIM current samp : 23299
TIM top          : 45714
Comm step        : 2
Temperature      : 29.20

Fault            : FAULT_CODE_DRV8302
Current          : 0.4
Current filtered : -1.0
Voltage          : 31.42
Duty             : 0.02
RPM              : 2.0
Tacho            : 9
Cycles running   : 3
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 4
Temperature      : 29.12

Fault            : FAULT_CODE_DRV8302
Current          : 0.1
Current filtered : -0.5
Voltage          : 31.42
Duty             : 0.02
RPM              : 1.9
Tacho            : 10
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 5
Temperature      : 29.25

Fault            : FAULT_CODE_DRV8302
Current          : 1.0
Current filtered : -0.3
Voltage          : 31.42
Duty             : 0.00
RPM              : 0.1
Tacho            : 11
Cycles running   : 1
TIM duty         : 263
TIM val samp     : 10
TIM current samp : 26384
TIM top          : 52747
Comm step        : 6
Temperature      : 29.25

Fault            : FAULT_CODE_DRV8302
Current          : 0.6
Current filtered : 0.5
Voltage          : 31.45
Duty             : 0.01
RPM              : 0.1
Tacho            : 12
Cycles running   : 1
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 1
Temperature      : 29.49

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : 0.5
Voltage          : 31.39
Duty             : 0.02
RPM              : 1.1
Tacho            : 13
Cycles running   : 2
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 2
Temperature      : 29.44

Fault            : FAULT_CODE_DRV8302
Current          : 0.3
Current filtered : -0.2
Voltage          : 31.39
Duty             : 0.36
RPM              : 0.0
Tacho            : 14
Cycles running   : 1
TIM duty         : 3705
TIM val samp     : 755
TIM current samp : 5903
TIM top          : 10296
Comm step        : 3
Temperature      : 30.47

Fault            : FAULT_CODE_DRV8302
Current          : -0.1
Current filtered : 0.1
Voltage          : 31.39
Duty             : 0.60
RPM              : 300.3
Tacho            : 16
Cycles running   : 378
TIM duty         : 3999
TIM val samp     : 1999
TIM current samp : 5332
TIM top          : 6666
Comm step        : 5
Temperature      : 30.41

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : 0.1
Voltage          : 31.45
Duty             : 0.36
RPM              : 1.0
Tacho            : 17
Cycles running   : 2
TIM duty         : 3702
TIM val samp     : 1846
TIM current samp : 7010
TIM top          : 10329
Comm step        : 6
Temperature      : 30.47

Fault            : FAULT_CODE_DRV8302
Current          : -1.4
Current filtered : 0.4
Voltage          : 31.41
Duty             : 0.02
RPM              : 0.0
Tacho            : 21
Cycles running   : 2
TIM duty         : 903
TIM val samp     : 10
TIM current samp : 26384
TIM top          : 52747
Comm step        : 4
Temperature      : 30.76

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : -0.3
Voltage          : 31.44
Duty             : 0.01
RPM              : 0.0
Tacho            : 22
Cycles running   : 1
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 5
Temperature      : 30.76

Fault            : FAULT_CODE_DRV8302
Current          : -0.5
Current filtered : 0.7
Voltage          : 31.38
Duty             : 0.03
RPM              : 1.4
Tacho            : 23
Cycles running   : 5
TIM duty         : 1160
TIM val samp     : 609
TIM current samp : 21453
TIM top          : 41687
Comm step        : 6
Temperature      : 30.70
```

---
## \#16 Posted by: Koto Posted at: 2017-04-03T08:32:59.509Z Reads: 99

```
@flatsp0t know what it means?
```

---
## \#17 Posted by: flatsp0t Posted at: 2017-04-03T08:35:20.489Z Reads: 103

```
Well, that is not that good.
Seems like a fried DRV.
This could be caused by either a short, or a setup/configuratin problem.

May i ask where you got the VESC from and When?
```

---
## \#18 Posted by: Koto Posted at: 2017-04-03T08:36:01.914Z Reads: 102

```
recently bought, diyelectricskateboards
```

---
## \#19 Posted by: flatsp0t Posted at: 2017-04-03T08:41:16.008Z Reads: 105

```
Well, then it is not the Firmware bug i thought of, so i would try to examine the reason and check for shorts.
if there are none, it is most likely a configuration issue.

Anyways, you need to get your Vesc repaired. Maybe ask @torqueboards if he is willing to help you wit this, if not and you are in the US/Can you can ask @JohnnyMeduse to repair it, he is the uncrowned king of dead(and ofc. repaired) DRVs.
```

---
## \#20 Posted by: Koto Posted at: 2017-04-03T08:42:17.666Z Reads: 105

```
@flatsp0t sorry - im a noob. what is a drv
```

---
## \#21 Posted by: flatsp0t Posted at: 2017-04-03T08:45:04.599Z Reads: 100

```
It is the Mosfet(the things tht switch power to the motor pases) driver chip. This is the most common failure on VESCs, as the chip is a bit prone to failure.
```

---
## \#22 Posted by: Koto Posted at: 2017-04-03T08:46:59.257Z Reads: 100

```
thanks. ill try fix it
```

---
## \#23 Posted by: Parafodas Posted at: 2017-04-03T09:40:07.424Z Reads: 102

```
@JohnnyMeduse is super super Nice insane guy like all ppl see ave oh foi tube
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2017-04-03T12:50:10.483Z Reads: 92

```
HI @Koto,

hummm.... with these kind of results, I can only come to the sad conclusion that your vesc might be damage. But you should also take a closer look at your motor before trying another vesc, Look like it might be the root cause of your problem. 

May I suggest to contact @torqueboards at first, to see want types of warranty he can was with your VESC. And after if you still need some repair to be done, I will more than happy to help you. I you feel that you can do it by yourself go for it... (i can also give you some advise if needed)

Regards 
JF
```

---
## \#25 Posted by: Koto Posted at: 2017-04-04T06:56:33.115Z Reads: 80

```
Thank you very much @JohnnyMeduse ! I'm talking to torqueboards about it. Don't have a warranty - so not looking good. I hooked up 3 triple a batteries to the motor to see if it would do anything. It made a weird sound and then shook a little bit. Do you think its okay?
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2017-04-04T14:27:29.798Z Reads: 71

```
[quote="Koto, post:25, topic:20187"]
It made a weird sound and then shook a little bit.
[/quote]


You can check with a multi-meter the Resistance R48-R49-R50-R51 just to be sure they are at 100ohms, and also take a peek at the shunt just to make sure they are properly solder in place.

But looking at the manipulation you did it, the conclusion is mostly to be a Burn drv chip.
```

---
## \#27 Posted by: Koto Posted at: 2017-04-05T23:23:08.168Z Reads: 65

```
so im kind of a noob, and dont know the terminology, but im assume you mean to look at the solder points. and i dont know what or how to use a multimeter
```

---
## \#28 Posted by: Koto Posted at: 2017-04-05T23:25:24.047Z Reads: 65

```
My talk with torqueboards is not looking good. I dont have a warranty, so I dont think i can get a replacement.
```

---
## \#29 Posted by: frameto Posted at: 2017-10-09T21:29:01.435Z Reads: 50

```
I have a similar problem on the two vesc of my dual setup.
I also bought the vesc to diyelectricskateboard in june :

 first vesc faults :

The following faults were registered since start:

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : -0.7
Voltage          : 46.45
Duty             : 0.02
RPM              : 0.1
Tacho            : 5
Cycles running   : 3
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 4
Temperature      : 26.51

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : -0.0
Voltage          : 46.39
Duty             : -0.02
RPM              : -0.3
Tacho            : 6
Cycles running   : 2
TIM duty         : -792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 1
Temperature      : 26.97

Fault            : FAULT_CODE_DRV8302
Current          : -0.6
Current filtered : 0.2
Voltage          : 46.48
Duty             : -0.02
RPM              : -2.3
Tacho            : 4
Cycles running   : 4
TIM duty         : -898
TIM val samp     : 449
TIM current samp : 22908
TIM top          : 44919
Comm step        : 3
Temperature      : 27.10

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : -0.1
Voltage          : 46.35
Duty             : 0.02
RPM              : 0.0
Tacho            : 3
Cycles running   : 3
TIM duty         : 954
TIM val samp     : 498
TIM current samp : 22615
TIM top          : 44233
Comm step        : 6
Temperature      : 30.25

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : 0.5
Voltage          : 46.35
Duty             : 0.02
RPM              : 0.0
Tacho            : 5
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 2
Temperature      : 30.31

Fault            : FAULT_CODE_DRV8302
Current          : 0.3
Current filtered : -0.1
Voltage          : 46.38
Duty             : 0.02
RPM              : 1.9
Tacho            : 6
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 3
Temperature      : 30.39

Fault            : FAULT_CODE_DRV8302
Current          : 0.3
Current filtered : -0.0
Voltage          : 46.33
Duty             : 0.00
RPM              : 1.0
Tacho            : 7
Cycles running   : 1
TIM duty         : 263
TIM val samp     : 10
TIM current samp : 26384
TIM top          : 52747
Comm step        : 4
Temperature      : 30.41

Fault            : FAULT_CODE_DRV8302
Current          : -1.0
Current filtered : -0.1
Voltage          : 46.41
Duty             : 0.00
RPM              : 1.0
Tacho            : 8
Cycles running   : 1
TIM duty         : 263
TIM val samp     : 10
TIM current samp : 26384
TIM top          : 52747
Comm step        : 5
Temperature      : 30.41

Fault            : FAULT_CODE_DRV8302
Current          : 0.1
Current filtered : 0.1
Voltage          : 46.38
Duty             : 0.02
RPM              : 1.7
Tacho            : 9
Cycles running   : 3
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 6
Temperature      : 30.41

Fault            : FAULT_CODE_DRV8302
Current          : 0.4
Current filtered : -0.5
Voltage          : 46.35
Duty             : 0.02
RPM              : 0.2
Tacho            : 10
Cycles running   : 4
TIM duty         : 1053
TIM val samp     : 541
TIM current samp : 22046
TIM top          : 43010
Comm step        : 1
Temperature      : 30.49

Fault            : FAULT_CODE_DRV8302
Current          : 0.3
Current filtered : 0.4
Voltage          : 46.35
Duty             : 0.02
RPM              : 0.2
Tacho            : 11
Cycles running   : 2
TIM duty         : 792
TIM val samp     : 451
TIM current samp : 23572
TIM top          : 46242
Comm step        : 2
Temperature      : 30.52

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : -0.1
Voltage          : 46.36
Duty             : 0.02
RPM              : 1.1
Tacho            : 12
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 3
Temperature      : 30.52

Fault            : FAULT_CODE_DRV8302
Current          : -1.0
Current filtered : -0.0
Voltage          : 46.33
Duty             : 0.01
RPM              : 0.0
Tacho            : 13
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 4
Temperature      : 31.29

Fault            : FAULT_CODE_DRV8302
Current          : 0.0
Current filtered : -0.3
Voltage          : 46.32
Duty             : 0.02
RPM              : 2.0
Tacho            : 15
Cycles running   : 2
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 6
Temperature      : 31.26

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : 0.3
Voltage          : 46.32
Duty             : 0.02
RPM              : 1.9
Tacho            : 16
Cycles running   : 2
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 1
Temperature      : 31.32

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : -0.2
Voltage          : 46.32
Duty             : 0.02
RPM              : 0.0
Tacho            : 19
Cycles running   : 3
TIM duty         : 955
TIM val samp     : 499
TIM current samp : 22615
TIM top          : 44233
Comm step        : 4
Temperature      : 31.56

Fault            : FAULT_CODE_DRV8302
Current          : -0.0
Current filtered : -0.3
Voltage          : 46.32
Duty             : 0.02
RPM              : 1.0
Tacho            : 20
Cycles running   : 2
TIM duty         : 792
TIM val samp     : 451
TIM current samp : 23572
TIM top          : 46242
Comm step        : 5
Temperature      : 31.59

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : 0.5
Voltage          : 46.33
Duty             : 0.02
RPM              : 1.4
Tacho            : 21
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 6
Temperature      : 31.59

Fault            : FAULT_CODE_DRV8302
Current          : 0.4
Current filtered : -0.4
Voltage          : 46.32
Duty             : -0.02
RPM              : -0.1
Tacho            : 20
Cycles running   : 4
TIM duty         : -898
TIM val samp     : 462
TIM current samp : 22921
TIM top          : 44919
Comm step        : 1
Temperature      : 31.61

Fault            : FAULT_CODE_DRV8302
Current          : 1.3
Current filtered : -0.1
Voltage          : 46.27
Duty             : 0.02
RPM              : 0.0
Tacho            : 20
Cycles running   : 4
TIM duty         : 955
TIM val samp     : 499
TIM current samp : 22610
TIM top          : 44222
Comm step        : 3
Temperature      : 31.99

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : -0.3
Voltage          : 46.26
Duty             : 0.02
RPM              : 0.0
Tacho            : 21
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 4
Temperature      : 31.96

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : -0.2
Voltage          : 46.29
Duty             : 0.02
RPM              : 1.0
Tacho            : 22
Cycles running   : 4
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 5
Temperature      : 31.99


Second vesc faults :

The following faults were registered since start:

Fault            : FAULT_CODE_DRV8302
Current          : 0.5
Current filtered : -0.0
Voltage          : 46.48
Duty             : 0.01
RPM              : 4.2
Tacho            : 10
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 4
Temperature      : 28.91

Fault            : FAULT_CODE_DRV8302
Current          : 0.1
Current filtered : -0.1
Voltage          : 46.50
Duty             : 0.01
RPM              : 2.0
Tacho            : 11
Cycles running   : 1
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 5
Temperature      : 28.89

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : 0.0
Voltage          : 46.44
Duty             : 0.01
RPM              : 1.9
Tacho            : 12
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 6
Temperature      : 28.97

Fault            : FAULT_CODE_DRV8302
Current          : -0.5
Current filtered : 0.1
Voltage          : 46.44
Duty             : 0.01
RPM              : 20.4
Tacho            : 22
Cycles running   : 1
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 6
Temperature      : 30.36

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : 0.2
Voltage          : 46.45
Duty             : 0.02
RPM              : 1.2
Tacho            : 23
Cycles running   : 2
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 1
Temperature      : 30.55

Fault            : FAULT_CODE_DRV8302
Current          : -0.0
Current filtered : 0.2
Voltage          : 46.48
Duty             : 0.02
RPM              : 1.2
Tacho            : 24
Cycles running   : 2
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 2
Temperature      : 30.55

Fault            : FAULT_CODE_DRV8302
Current          : 0.7
Current filtered : 0.1
Voltage          : 46.47
Duty             : 0.01
RPM              : 1.6
Tacho            : 25
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 3
Temperature      : 30.57

Fault            : FAULT_CODE_DRV8302
Current          : -0.5
Current filtered : 0.2
Voltage          : 46.33
Duty             : 0.01
RPM              : 8.6
Tacho            : 32
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 6
Temperature      : 33.16

Fault            : FAULT_CODE_DRV8302
Current          : -0.0
Current filtered : 0.0
Voltage          : 46.36
Duty             : 0.02
RPM              : 3.0
Tacho            : 34
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 2
Temperature      : 33.21

Fault            : FAULT_CODE_DRV8302
Current          : -0.0
Current filtered : 0.1
Voltage          : 46.33
Duty             : 0.01
RPM              : 1.9
Tacho            : 35
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 3
Temperature      : 33.16
```

---
## \#30 Posted by: ARetardedPillow Posted at: 2017-10-10T01:26:52.670Z Reads: 40

```
Okay, more people need to be informed about this, if the vesc flashes red 3 times, that means youve fried your drv chip and you either need to replace that chip or just get a new vesc completely, fried vesc is still useful though. And another thing, if your vesc flashes red 4 times, that means you have a fault and your eskate needs to be inspected and checked of problems.
```

---
