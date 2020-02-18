# After VESC Firmware update, motors not detected?

### Replies: 23 Views: 1981

## \#1 Posted by: herojeanpierre Posted at: 2017-12-02T18:58:02.041Z Reads: 136

```
Hello all! 

I am a little concerned since after using the vesc tool to update my VESC firmware, I am no longer able to control the motors. I followed the [firmware update instructions](http://vesc-project.com/node/179) to the tee.

(Hardware is 48, and I updated it to firmware 3.34)

I am pretty sure VESC isn't bricked because

1. The remote throttle input can be read from the on the screen.
2. When I spin the motors with my hands, the realtime data shows a change in current.
3. It reads the firmware update and doesn't throw any errors.

The things that isn't working is that it can't detect the motors. Like when I try to calibrate the BLDC parameters it just can't detect a motor. I am using Maytech 230kv sensored motor, running sensorless. Not only that but when I use my remote after unplugging the vesc, it does nothing. 

Has this ever happened to anyone? Any ideas? I made sure my battery voltage cutoff is correct as well.
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2017-12-02T19:10:10.215Z Reads: 122

```
Post your settings

Go to terminal and type in "faults"
```

---
## \#3 Posted by: herojeanpierre Posted at: 2017-12-02T19:11:48.850Z Reads: 121

```
The following faults were registered since start:

Fault            : FAULT_CODE_OVER_TEMP_FET
Current          : -0.3
Current filtered : 0.0
Voltage          : 45.23
Duty             : 0.001
RPM              : 6.6
Tacho            : 3
Cycles running   : 0
TIM duty         : 3
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 3
Temperature      : 330.57

Why the hell does it say its 330 degrees when it's not. Wow. Maybe that's the problem, incorrect sensor reading?
```

---
## \#4 Posted by: ARetardedPillow Posted at: 2017-12-02T19:13:10.425Z Reads: 109

```
I havent seen that before, are you running 12s? And check to see if youve blown the mosfet

Hmm bad sensors??
```

---
## \#5 Posted by: herojeanpierre Posted at: 2017-12-02T19:13:47.167Z Reads: 108

```
Yes 12S, how do I check to see if I've blown a mosfet?
```

---
## \#6 Posted by: ARetardedPillow Posted at: 2017-12-02T19:16:44.652Z Reads: 103

```
Id say the easiest way is to look at the actual thing closely and see lol

Check for burn marks and stuff
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-12-02T19:17:19.883Z Reads: 101

```
yea just check and see if any of the FET’s look burned at all, post a pic here when you get a chance too
```

---
## \#8 Posted by: herojeanpierre Posted at: 2017-12-02T19:21:08.533Z Reads: 100

```
All of the FETS look perfect. 

<img src="/uploads/db1493/original/3X/7/6/76601075ef6f7db86d12c1adbfbe25638500f3be.png" width="640" height="480">
<img src="/uploads/db1493/original/3X/8/c/8c0707ef4380ff9c5930ee34527c794aa574d7cb.png" width="375" height="500">
```

---
## \#9 Posted by: herojeanpierre Posted at: 2017-12-02T19:21:45.594Z Reads: 99

```
Thanks for helping me out btw, I really appreciate it.
```

---
## \#10 Posted by: ARetardedPillow Posted at: 2017-12-02T19:24:02.426Z Reads: 101

```
Hmm look really really closely at the pins like reeaaaaly closely, and tb vesc?

If theres nothing wrong then I think the temp sensors are bad, try reflashing your vesc to ackmaniac's
```

---
## \#11 Posted by: herojeanpierre Posted at: 2017-12-02T19:27:43.848Z Reads: 102

```
The mosfets are looking perfect... I actually rode the board for about 15 miles perfectly before updating the firm.

Sorry I am not to familiar with the term "flashing" or ackmaniacs fw. How do I flash my vesc to ackmaniacs?
```

---
## \#12 Posted by: GrecoMan Posted at: 2017-12-02T19:30:32.890Z Reads: 103

```
flashing = updating
1. Click on this @Ackmaniac
2. Under his most popular topics, find the one that says something about extended BLDC tool (should be one of the first ones)
3. Scroll to the bottom of his first post in the thread and download the files.
4. Unzip the files, install the program
5. Read his directions in that thread on how to flash FW
```

---
## \#13 Posted by: herojeanpierre Posted at: 2017-12-02T19:32:29.293Z Reads: 101

```
Okay I'll try this and tell you how it works. Thanks
```

---
## \#14 Posted by: ARetardedPillow Posted at: 2017-12-02T19:38:29.357Z Reads: 101

```
Here check out this link
http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116
```

---
## \#15 Posted by: herojeanpierre Posted at: 2017-12-02T20:57:15.957Z Reads: 95

```
I followed all the steps, installed the FW, and everything. But I still get 

The following faults were registered since start:

Fault            : FAULT_CODE_OVER_TEMP_FET
Current          : -0.3
Current filtered : 0.1
Voltage          : 45.15
Duty             : 0.001
RPM              : 6.7
Tacho            : 3
Cycles running   : 0
TIM duty         : 3
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 2
Temperature      : 377.04
 
So I guess it must be the temp sensors... I wish I could turn the temp settings off. Unless you have any other suggestions I think we figured out my problem. I did buy these ESC's off a friend who got them repaired.

Thanks guys
```

---
## \#16 Posted by: Sander Posted at: 2017-12-02T21:37:44.954Z Reads: 92

```
I thought you should do motor detection with fully charged battery? As I can see the voltage is 45.15 not ~50.4V?
```

---
## \#17 Posted by: chaka Posted at: 2017-12-02T22:58:32.485Z Reads: 85

```
Overtemp fault indicates to me that you uploaded the incorrect firmware. You may have fried the PCB if you tried running a motor test.
```

---
## \#18 Posted by: scepterr Posted at: 2017-12-02T23:04:13.877Z Reads: 84

```
Is that typical? Wrong fw blows temp resistor?
```

---
## \#19 Posted by: chaka Posted at: 2017-12-02T23:07:16.184Z Reads: 82

```
No but it will cause an incorrect temp measurement.
```

---
## \#20 Posted by: herojeanpierre Posted at: 2017-12-03T02:04:01.015Z Reads: 86

```
It was the correct firmware from the start. I made sure of it. Plus, the motor was never detected so nothing could've been fried.
```

---
## \#21 Posted by: Mobutusan Posted at: 2018-01-01T23:37:32.062Z Reads: 72

```
Did you ever figure this out? I tried @Ackmaniac's latest 3.1 firmware with a Torqueboards VESC, and I got the same "Over Temp" error, and could not even get the motors to spin during detection. I switched back to the 2.54 fw and BLDC tool from his original thread and everything works fine now.
```

---
## \#22 Posted by: Ackmaniac Posted at: 2018-01-01T23:45:54.218Z Reads: 73

```
I guess you are installing the wrong firmware for your hardware. If you have the 4.12 hardware you have to choose this file.

<img src="/uploads/db1493/original/3X/c/0/c08e3447b1566f37bf994c0d9b362329eccd6dec.png" width="690" height="337">

It also could be because of wrong readings from the motor temp sensor. But you can check that when you have a look at the realtime data.
```

---
## \#23 Posted by: Mobutusan Posted at: 2018-01-02T00:03:24.378Z Reads: 68

```
Ah, yes. Derp. That makes sense. I'll try it again with the proper hardware selected this time. I'm still kind of a VESC noob, and was trying your latest software way too late last night, er, this morning and missed that. I figured it had to be something simple that I was missing since it worked on your old fw. 

Thanks for the prompt response and all your hard work on this project. Really great stuff, especially with the app. I'll definitely be sending a donation your way soon. 👍
```

---
