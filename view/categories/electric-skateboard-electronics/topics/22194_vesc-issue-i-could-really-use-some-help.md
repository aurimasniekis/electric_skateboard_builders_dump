# VESC issue, I could really use some help!

### Replies: 10 Views: 570

## \#1 Posted by: EpicLavalamp Posted at: 2017-05-02T06:50:53.953Z Reads: 63

```
Hey everyone, I just put my first build together and I had it working for only a moment.. So basically my problem I believe is the DRV or the motor...

My build:
-Turnigy Aerodrive SK3 - 6374-192kv Brushless Outrunner Motor
-2 Turnigy 5000mAh 5S 30C Lipo Packs in series
-VESC 4.12 from Miami Electric Boards

I'm using firmware 2.18. When I first hooked everything up it worked like a dream. Motor detected, controller operated it, could go forward and brake etc. This was before the wires were secure so I hiked them up for a test run, and then when I was actually ready to hop on and test it I got nothing..

Hooked it back up to the computer and couldn't get the motor to spin once so ever. Not with the transmitter, the computer, nor the motor detection. After running the motor detection and looking to the terminal for faults I get this:


Fault            : FAULT_CODE_DRV8302
Current          : -1.2
Current filtered : 0.4
Voltage          : 41.35
Duty             : 0.01
RPM              : 0.3
Tacho            : 3
Cycles running   : 3
TIM duty         : 689
TIM val samp     : 356
TIM current samp : 24112
TIM top          : 47511
Comm step        : 3
Temperature      : 25.42

Fault            : FAULT_CODE_DRV8302
Current          : -0.3
Current filtered : 0.6
Voltage          : 41.35
Duty             : 0.02
RPM              : 0.3
Tacho            : 4
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 4
Temperature      : 25.49

Fault            : FAULT_CODE_DRV8302
Current          : 0.9
Current filtered : -0.4
Voltage          : 41.29
Duty             : 0.02
RPM              : 1.2
Tacho            : 5
Cycles running   : 4
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 5
Temperature      : 25.52

What should I do here? Can I fix this? Please, I was so excited to have this thing working and right on the brink it seems to have failed...
```

---
## \#2 Posted by: Eboosted Posted at: 2017-05-02T07:03:00.690Z Reads: 51

```
Can you post your VESC settings?
```

---
## \#3 Posted by: EpicLavalamp Posted at: 2017-05-02T07:05:38.269Z Reads: 56

```
Definitely! <img src="/uploads/db1493/original/3X/6/4/64214dc1fb9d55840656636ef173881ef6036221.PNG" width="690" height="355"><img src="/uploads/db1493/original/3X/4/1/41ec4905fcc1cd982c60329a58f46dff323c7368.PNG" width="690" height="357">
```

---
## \#4 Posted by: Eboosted Posted at: 2017-05-02T07:11:02.121Z Reads: 56

```
According to this screen you are not connected to the VESC, if you just disconnected after reading the values and get a failed motor detection then you need to change the DRV chip. 

Is your VESC flashing a blinking red light constantly?
```

---
## \#5 Posted by: EpicLavalamp Posted at: 2017-05-02T07:17:24.252Z Reads: 54

```
I was not connected to it at the time of the screen cap, correct. The VESC does flash a blinking red light in sets of 3's 6 times while trying to detect the motor. After it shows the "Bad detection results received" status in the bottom right the red blinking light stops. It will also blink a red light 6 times when I try to operate the motor via transmitter or computer arrow key commands.
```

---
## \#6 Posted by: Eboosted Posted at: 2017-05-02T07:19:04.110Z Reads: 54

```
If you didn't even riden it contact the vesc supplier
```

---
## \#7 Posted by: EpicLavalamp Posted at: 2017-05-02T07:21:02.919Z Reads: 57

```
I was thinking of doing that. It was such a disappointment to not even try it out! But, in your opinion, do you think these issues point to a faulty DRV?
```

---
## \#8 Posted by: makevoid Posted at: 2017-05-02T07:27:59.483Z Reads: 53

```
is there a burn mark on the drv chip? maybe post a picture of the board without heatshrink and a screenshot of the advanced tab
```

---
## \#9 Posted by: EpicLavalamp Posted at: 2017-05-02T07:56:53.297Z Reads: 49

```
So I took the heatshrink off and oddly enough the DRV looks like it's in perfect condition! However, there seems to be some sort of capacitor near by that has melted? Check it out:
<img src="/uploads/db1493/original/3X/c/d/cdf08d321adb7a3e289917dd82f56311584d2132.jpg" width="690" height="388">

Also here are my advanced settings:
<img src="/uploads/db1493/original/3X/7/f/7f5d221849562cda4c7682f1ded1409718de482b.PNG" width="690" height="356">
```

---
## \#10 Posted by: Norco Posted at: 2017-05-02T09:17:11.503Z Reads: 41

```
Phase wires touching could have fried it?
```

---
