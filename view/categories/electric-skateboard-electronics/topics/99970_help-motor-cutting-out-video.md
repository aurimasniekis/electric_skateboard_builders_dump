# HELP-Motor Cutting Out (Video)

### Replies: 38 Views: 257

## \#1 Posted by: esk8snith Posted at: 2019-08-08T23:07:02.508Z Reads: 45

```
During the middle of my ride today, my motor started cutting out. I just built the board and was testing it and this happened, so I lowered the Batt Max and messed around with a couple other settings and it was fine until like 20 min into the ride when this starts happening:

**VIDEO**: https://streamable.com/q1mwc

I am using a Maytech Dual VESC. These are the current settings that I have: 
* **Motor Type** : BLDC Unsensored, Split PPM
* **Motor Max** : 80 A
* **Motor Min** : -35 A
* **Batt max** : 15 A
* **Batt min** : -12 A

Settings from Skatemetric Foosted guide/

Battery: 10s3p Samsung 25R which can do 60A (bypassed BMS for discharge). 
Motors: Dual 6354 200kV

It only happens a few minutes into riding. I initially thought that the VESC could be overheating so I reduced the current limits for the battery. 

Help pls, I wanna ride and not die lol

Thanks!
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-08-09T00:15:33.908Z Reads: 38

```
@esk8snith  That looks like a wire connection issue to me. I'd open it up, unplug and replug all the connections check any and all of your solder joints, redo the motor/sensor detection, recheck all your other settings (PPM 
 values, voltage cutoff, everything) and try again.
```

---
## \#3 Posted by: esk8snith Posted at: 2019-08-09T00:40:45.193Z Reads: 36

```
i just taped all my motor bullet connectors to make sure that they weren’t touching each other. I was also noticing cutoffs when my voltage dropped below 31v while accelerating. 

i’m gonna try it out not and see but do you know what else it could be since it doesn’t happen at the beginning of rides and only happens at low battery.

If my VESC voltage cutoff is 31v and my battery sags while accelerating is my vesc just gonna cut out?
```

---
## \#4 Posted by: Santino Posted at: 2019-08-09T00:49:35.494Z Reads: 37

```
Its looks like a poor connection for me too, do you use a loop key? Maybe when you are using the board, the connector get slightly loose...So una vesc get more current than the other. Also if you experience too much voltage sag, it could be the batteries quality (maybe fake cells?)...An my last point of view, 80amp motor max with a 10s3p, isn't that too much?
```

---
## \#5 Posted by: esk8snith Posted at: 2019-08-09T01:15:25.786Z Reads: 35

```
All connections are solid now for sure, only one of the motor cuts out too for some reason.
```

---
## \#6 Posted by: esk8snith Posted at: 2019-08-09T01:15:54.602Z Reads: 35

```
And i use an Antispark that’s built into the VESC
```

---
## \#7 Posted by: MysticalDork Posted at: 2019-08-09T01:26:21.933Z Reads: 35

```
[quote="esk8snith, post:3, topic:99970"]
If my VESC voltage cutoff is 31v and my battery sags while accelerating is my vesc just gonna cut out?
[/quote]

No it won't cut out completely, but it will reduce power output to protect your batteries. Are your batteries fully (or at least mostly) charged during your testing? and how far apart are your cutoff start and cutoff end voltages from eachother?
```

---
## \#8 Posted by: esk8snith Posted at: 2019-08-09T01:27:09.888Z Reads: 29

```
i’m at 31 and 28 for cutoffs. currently it’s not it’s at 20% but it’s also been happening at around 40-45% battery
```

---
## \#9 Posted by: esk8snith Posted at: 2019-08-09T01:27:39.082Z Reads: 26

```
it’s not just cutting out my motor is locking up for a second and then the belt is slipping
```

---
## \#10 Posted by: MysticalDork Posted at: 2019-08-09T01:28:23.565Z Reads: 28

```
Are there any differences in settings between your two vescs/halves? Have you tried checking faults in the vesc tool console?
```

---
## \#11 Posted by: Santino Posted at: 2019-08-09T01:51:24.677Z Reads: 30

```
You have a pack constant discharge of 60A....Pushing 2 motors at 80A it is too much for the battery set up. Therefore after a few minutes of drive (if you drive hard it gets worse), your batteries are draining with too much stress, so the closer you reach the safety cut off, the ESC will activate the cut off. If you are willing to test 30A motor max and 30A battery max, linear, many it is just that. In that case the solution will be increasing cells in series and parallel. Imagine you are creating a voltage sag at 32V goes down 4V when you push the throttle, that would be 28V, a good reason for a ESC to cut off...When the battery recovers a little bit, it pushing some ups again...but you are playing under the red line the hole time...
```

---
## \#12 Posted by: MysticalDork Posted at: 2019-08-09T01:57:24.788Z Reads: 28

```
Motor amps are NOT the same as battery amps. It's totally possible to draw 30 amps from the battery and feed 80 to the motor.
```

---
## \#13 Posted by: Santino Posted at: 2019-08-09T01:57:37.711Z Reads: 28

```
You may also check your cut of time and amps, I use 10amps so it won't create a sudden stop if a fault happens...
```

---
## \#14 Posted by: Waiboard Posted at: 2019-08-09T01:58:59.334Z Reads: 27

```
I am having a similar problem, my configuration is two Flipsky 6354 190KV / VESC 4.20 dual plus / 10s4p engines with BMS 100A for loading and unloading.

My current configuration is recommended by Flipsky:

    Current Max Motor: 30A
    Current Max Brake Motor: -25A
    Absolute Maximum Current: 130A
    Slow ABS Current Limit: True
    Battery Current Max: 30A
    Battery Current Max Regen: -25A

But I still get cuts on my board.
I don't understand how to calculate these values?
```

---
## \#15 Posted by: Santino Posted at: 2019-08-09T01:59:34.361Z Reads: 25

```
I think there is a limit to push volts from a battery...motor and bat amps...also motor get stator saturation at a certain point....so I disagree with you
```

---
## \#16 Posted by: Santino Posted at: 2019-08-09T02:03:05.230Z Reads: 25

```
Unless there is something wrong with the ESC, I would check all of the connections, at all leves.....I had a similar issue not long ago, my anti spark was getting just a little bit loose...one of my motors pushed ok, the other one not much...fix it , everything runs great now...
```

---
## \#17 Posted by: MysticalDork Posted at: 2019-08-09T02:06:16.170Z Reads: 25

```
Yes, you are correct that there is a limit on the voltage from the battery. But the motor has a lower impedence at low speed due to lack of back-EMF - more current can flow. The vesc acts like a stepdown converter, converting high voltage at low current, to lower voltage at higher current. 

Test it yourself: get a meter that can measure AC and DC current. Put it on your battery wire and then on one of your motor phase wires. Under load at low speed, the phase current can and usually will be higher than the battery current.
```

---
## \#18 Posted by: Waiboard Posted at: 2019-08-09T02:07:11.959Z Reads: 25

```
I'm going to check the connections, but beyond that do you know how those values are calculated?
For example why put) Current Max Motor: 30A / Current Max Brake Motor: -25A Battery Current Max: 30A / Battery Current Max Regen: -25A), and not set other different values?
```

---
## \#19 Posted by: Santino Posted at: 2019-08-09T02:12:39.524Z Reads: 22

```
I've done that many times....Agree with you too...But 10s3p...thats only 60amps continues...If he is pushing to hard, voltage sag will be created by battery stress...A complete cut of and coming back from the dead could be read at the ESC like a regenerative energy = stopping....So I just think it is a mix of the way you ride, your set ups, climate, etc.... If things get warm...everything is possible...Also they should check if they have the latest firmware downloaded...
```

---
## \#20 Posted by: Santino Posted at: 2019-08-09T02:12:59.728Z Reads: 23

```
https://calc.3dservisas.eu/?TdDBDoIwEATQf-nZmCIF1OtqPEmakMhdONTEShOOxn93Z2jE29tJd1p4m7sEczTPx_QyGx1aHcptrZ6lUxeW9Igpgaxd4hOmXbZfzc5Cmbq8mP72kkfqKC5BrCorEmFN_oqGILlpCGfV3pI3rDs4Sm6KfHbDzE-wI9f7ozDG4bGf-ZENfLnCFdnjOH7DiNsO1ny-
```

---
## \#21 Posted by: MysticalDork Posted at: 2019-08-09T02:16:43.859Z Reads: 21

```
[quote="esk8snith, post:1, topic:99970"]
* **Batt max** : 15 A
* **Batt min** : -12 A
[/quote]

 That's the draw per motor from the battery. Total of thirty amps. 80 **motor amps**, fifteen **battery amps.**

Battery amps =/= motor amps.
```

---
## \#22 Posted by: Santino Posted at: 2019-08-09T02:18:33.092Z Reads: 20

```
Your pack min voltage is 30v...you are going to low...the chart will help you to translate that to your reading...if you battery push 60amp max thats equals to 30A to each motor...It does not matter ir you motors are rated at 80A (also do not trust the vendor on that info)...Best is to run the latest VescTool firmware...it is a great help when it comes to setting and true values...
```

---
## \#23 Posted by: esk8snith Posted at: 2019-08-09T02:20:09.716Z Reads: 21

```
@MysticalDork is correct, my motor curr limit can be anything, but vesc won’t accept more than 15A from vattery
```

---
## \#24 Posted by: Santino Posted at: 2019-08-09T02:22:28.484Z Reads: 21

```
Yes thats right, sorry for that mystique...
```

---
## \#25 Posted by: Waiboard Posted at: 2019-08-09T02:24:55.687Z Reads: 20

```
I don't understand what this calculator is for?
My question is how do I know what values to put on the VESC Tool?
I have a Samsung 25r 10s4p battery with constant BMS 100A for charging and discharging.
```

---
## \#26 Posted by: laurnts Posted at: 2019-08-09T02:26:55.485Z Reads: 20

```
Your motor kv seems to be quite high, with possibility that the motor its self doesnt sustain high amp output. I had this type of motor that constantly cutting out due to over current. If you plug the vesc and do real time data and logging, youll see vesc continuously report over current. One way to go around this is to throttle gently and not punching it from 0 to 100 in a blip.
```

---
## \#27 Posted by: Santino Posted at: 2019-08-09T02:30:07.521Z Reads: 20

```
If you experience cut off maybe it is created by the BMS, when you are low it start the balancing creating and emergency cut of...Many of us bypass the discharge... To add the values at the vesc tool just check the vesc-tool project web page and go to documents...Also everything it is on the forum...
```

---
## \#29 Posted by: MysticalDork Posted at: 2019-08-09T02:38:04.314Z Reads: 18

```
Nope, you're doing it again. His **battery max** will be 80A/2=40A. The motor max can be higher, up to the rating of the motors themselves. Usually I set mine to 60 or 80 each.
```

---
## \#30 Posted by: Santino Posted at: 2019-08-09T02:42:49.005Z Reads: 19

```
I am out...too late and tired...sorry if I confuse any of you guys...Thank you MysticalDork...sorry again...
```

---
## \#31 Posted by: MysticalDork Posted at: 2019-08-09T03:00:49.769Z Reads: 18

```
No worries, it's easy to get twisted around with all the different numbers flying around.
```

---
## \#32 Posted by: sayekim Posted at: 2019-08-09T06:41:38.728Z Reads: 18

```
Can you show us a picture of how your bms is bypassed?

I made a foolish mistake once and thought I had bypassed it but it wasn’t really. 
This made my bms cut off power when hitting upper and lower limits of the bms cut offs. 

It doesn’t seem to be the case for you though since you mention it only happens to one side. 

Perhaps check the cut off values in the VESC tool to see if they have the same cut off values.
```

---
## \#33 Posted by: MysticalDork Posted at: 2019-08-09T06:59:50.172Z Reads: 18

```
I second this: Weird things can happen when setting up two vescs and you can end up with funny settings. 

I'd also suggest plugging in the offending vesc and checking for any fault or error codes. Don't power off the vesc between when the cutout happens and when you plug into the computer - the error codes are in volatile memory and will disappear if power is lost even for a second.
```

---
## \#34 Posted by: Darkie02 Posted at: 2019-08-09T07:16:32.464Z Reads: 17

```
I would 

It looks like a min voltage cut off or overloaded over temp

Check battery cut off on both vesc 
Check each each p group voltage and pack voltage
Check vesc temp
Check nothing could be shorting eg phase wires 
Plug vesc in to pc befor turning off and look at the fault code
```

---
## \#35 Posted by: esk8snith Posted at: 2019-08-09T21:32:57.034Z Reads: 17

```
The following faults were registered since start:

Fault            : FAULT_CODE_DRV
Current          : 20.5
Current filtered : -3.7
Voltage          : 16.96
Duty             : 0.688
RPM              : 18496.2
Tacho            : 17940
Cycles running   : 73186
TIM duty         : 4061
TIM val samp     : 2030
TIM current samp : 4983
TIM top          : 5905
Comm step        : 4
Temperature      : 32.77
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : -71.2
Current filtered : -130.4
Voltage          : 29.19
Duty             : 0.862
RPM              : 224.6
Tacho            : 192620
Cycles running   : 154478
TIM duty         : 4189
TIM val samp     : 2072
TIM current samp : 4502
TIM top          : 4859
Comm step        : 6
Temperature      : 44.06
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : -70.5
Current filtered : -144.9
Voltage          : 23.17
Duty             : 0.671
RPM              : 11402.5
Tacho            : 240644
Cycles running   : 79167
TIM duty         : 4050
TIM val samp     : 2025
TIM current samp : 5043
TIM top          : 6037
Comm step        : 4
Temperature      : 40.23
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : -75.0
Current filtered : -146.0
Voltage          : 23.32
Duty             : 0.681
RPM              : 11655.3
Tacho            : 245804
Cycles running   : 5949
TIM duty         : 4057
TIM val samp     : 2028
TIM current samp : 5008
TIM top          : 5960
Comm step        : 4
Temperature      : 40.38
 
Fault            : FAULT_CODE_DRV
Current          : -4.3
Current filtered : -54.3
Voltage          : 17.96
Duty             : 0.612
RPM              : 12791.5
Tacho            : 265455
Cycles running   : 70762
TIM duty         : 4009
TIM val samp     : 2004
TIM current samp : 5282
TIM top          : 6556
Comm step        : 5
Temperature      : 40.90
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : -80.7
Current filtered : -146.8
Voltage          : 23.15
Duty             : 0.690
RPM              : 11602.1
Tacho            : 269852
Cycles running   : 115
TIM duty         : 4062
TIM val samp     : 2031
TIM current samp : 4973
TIM top          : 5884
Comm step        : 4
Temperature      : 40.77
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : -74.1
Current filtered : -143.0
Voltage          : 23.77
Duty             : 0.684
RPM              : 10370.9
Tacho            : 273392
Cycles running   : 6000
TIM duty         : 4058
TIM val samp     : 2029
TIM current samp : 4995
TIM top          : 5933
Comm step        : 4
Temperature      : 40.56
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : -75.8
Current filtered : -145.3
Voltage          : 21.82
Duty             : 0.666
RPM              : 9176.8
Tacho            : 276446
Cycles running   : 1480
TIM duty         : 4047
TIM val samp     : 2023
TIM current samp : 5063
TIM top          : 6079
Comm step        : 4
Temperature      : 40.56
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : -73.4
Current filtered : -145.6
Voltage          : 23.06
Duty             : 0.677
RPM              : 9692.7
Tacho            : 279752
Cycles running   : 20406
TIM duty         : 4054
TIM val samp     : 2027
TIM current samp : 5020
TIM top          : 5986
Comm step        : 4
Temperature      : 40.44
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : -89.9
Current filtered : -138.5
Voltage          : 18.97
Duty             : 0.656
RPM              : 4502.8
Tacho            : 287990
Cycles running   : 63064
TIM duty         : 4041
TIM val samp     : 2020
TIM current samp : 5099
TIM top          : 6157
Comm step        : 4
Temperature      : 40.80
```

---
## \#36 Posted by: esk8snith Posted at: 2019-08-09T21:35:21.597Z Reads: 17

```
Just had a NASTY fall bit a rough patch of road and I'm almost sure that one of the motors completely locked up, throwing me off the board at around 15 mph. I came home, cleaned up my wounds and plugged in my VESC to my computer to find the faults above.

This time, I was running CANBUS, Arkmaniac firmware, Motor 50,-40 and Batt 12,-6 (just to make sure it wasn't cutting out)
```

---
## \#37 Posted by: MysticalDork Posted at: 2019-08-09T21:45:23.786Z Reads: 16

```
You've got DRV errors, which means you've blown your DRV chip, which means it's time to either replace/have someone else replace the DRV chip, or get a new vesc.
```

---
## \#38 Posted by: esk8snith Posted at: 2019-08-09T21:48:31.745Z Reads: 17

```
Was the lockup caused by the DRV error or the ABS over current error? @MysticalDork
```

---
## \#39 Posted by: MysticalDork Posted at: 2019-08-09T21:50:30.896Z Reads: 16

```
Most likely the fried DRV is the cause of the overcurrent faults and the lockups. The next question is, what's the cause of the fried DRV? The most common causes are disconnected or shorting phase wires while riding. Just once is enough to fry the chip. @esk8snith
```

---
