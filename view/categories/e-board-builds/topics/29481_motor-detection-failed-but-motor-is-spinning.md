# Motor Detection Failed, but motor is spinning

### Replies: 26 Views: 1489

## \#1 Posted by: milesperhour Posted at: 2017-08-02T19:40:56.393Z Reads: 126

```
**Hi everyone**,

This is my first time posting on this forum, but I've been reading posts for a while. I'm setting up the VESC for the first time and I keep getting the error "Bad detection result received" when I try to detect the motor. When I hit "start detection" the motor spins up to 24,000 ERPM stops accelerating and then jumps up to 45,000 ERPM momentarily before cutting off.
<img src="/uploads/db1493/original/3X/c/3/c35f08bc0d84819113a715b4bd2e39bcd2ec705b.PNG" width="690" height="299">
 

The motor spins fine using the arrow keys, however I cant get it to detect. I have tried varying the Current and Min ERPM to no avail (300-1200 ERPM & 1-6A current). The motor always spins fine but wont detect. I have also tried varying the Battery cutoff voltages and changing to a much shorter USB cable. There are currently no faults when I check the terminal

Here are my current settings
<img src="/uploads/db1493/original/3X/4/8/48f058b0d84aa31df20c50c98102a15aee14f81e.PNG" width="690" height="304">
<img src="/uploads/db1493/original/3X/1/d/1d0540e3e63bbfd8c00107728b8eb42fdf069964.PNG" width="690" height="298">

I am using a TORQUEBOARDS VESC 4.12
Turnigy SK3 5055 430Kv motor (max 70A)
4X2S 8000maH batteries in series (8S, 29.6V 30C continuous)

I'm not sure if the high kV of my motor is causing the problem? If you have any suggestions I would really appreciate it.

Thanks

-milesperhour
```

---
## \#2 Posted by: ikjahaa Posted at: 2017-08-02T19:51:41.833Z Reads: 103

```
just spitballing here, are your batteries fully charged ?
```

---
## \#3 Posted by: sl33py Posted at: 2017-08-02T19:53:34.100Z Reads: 104

```
you've done most of what i'd do.  I'd double check you have the belt/wheel disconnected if it might be part of the issue.  I had one not detect when  my belt was too tight, removed belt and detected fine.
```

---
## \#4 Posted by: ikjahaa Posted at: 2017-08-02T19:59:26.404Z Reads: 103

```
Also, might  here might be some usefull information ... [http://www.electric-skateboard.builders/t/vesc-motor-detection-failing/6640?u=ikjahaa](http://www.electric-skateboard.builders/t/vesc-motor-detection-failing/6640?u=ikjahaa)
```

---
## \#5 Posted by: Jinra Posted at: 2017-08-02T20:01:03.195Z Reads: 102

```
Detection current is a bit low, try 6A

EDIT: nevermind i see you've done that
```

---
## \#6 Posted by: milesperhour Posted at: 2017-08-02T20:03:50.466Z Reads: 98

```
No my batteries are at ~50%. Ill try charging them
```

---
## \#7 Posted by: milesperhour Posted at: 2017-08-02T20:04:43.038Z Reads: 94

```
There's nothing on my motor shaft. It's completely free
```

---
## \#10 Posted by: Jinra Posted at: 2017-08-02T20:08:08.966Z Reads: 91

```
ah it's your max erpm limit. Your hitting almost 90k erpm during detection but your limit is set to 60k. You need a new motor...
```

---
## \#11 Posted by: Sander Posted at: 2017-08-02T20:09:07.533Z Reads: 89

```
Why does he need a new one if he is almost hitting 90k erpm? Can it fry the VESC?
```

---
## \#12 Posted by: milesperhour Posted at: 2017-08-02T20:10:27.861Z Reads: 89

```
Can't I limit the max ERPM from the BLDC ? I have it set to 60,000 right now.
```

---
## \#13 Posted by: Jinra Posted at: 2017-08-02T20:10:33.827Z Reads: 88

```
While he can raise the limit the drv is known to fry at over 60k. I wouldn't risk it personally, even for detection.
```

---
## \#14 Posted by: Hummie Posted at: 2017-08-02T20:11:20.893Z Reads: 89

```
I thought the max erpm being at 60,000 despite having a higher kv would keep his motor from going too fast to damage the vesc and all would be good.  ?

for me when it wont detect it's either a short in the motor or magnets or rotor is imbalanced.  does it spin smoothly or with any wobble?
```

---
## \#15 Posted by: Jinra Posted at: 2017-08-02T20:15:18.212Z Reads: 84

```
Detection is likely different, even with the normal limit i believe the vesc just shuts off or errors out when it hits
```

---
## \#16 Posted by: milesperhour Posted at: 2017-08-02T20:19:58.048Z Reads: 79

```
@Hummmie the motor spins very smoothly. I'm pretty sure I'm not shorting the motor leads as I soldered them and used heat shrink. There is no exposed wire.

@Jinra Could I detect the motor using less cells (6s) and then use those setting with the full 8s setup?
```

---
## \#17 Posted by: Jinra Posted at: 2017-08-02T20:25:16.099Z Reads: 74

```
you need a new motor, you'll blow out the vesc for sure when you use it
```

---
## \#18 Posted by: Hummie Posted at: 2017-08-02T20:28:14.427Z Reads: 74

```
are you saying that because it's so high kv?  wont the erpm limit keep him under the limit and all will be well?  maybe if he just uses fewer cells for the test if it's a test specific thing?
```

---
## \#19 Posted by: Jinra Posted at: 2017-08-02T20:29:33.212Z Reads: 77

```
I can't say for sure since i haven't tried it personally, but i believe the vesc turns off if it hits the limit. Besides that, it's a very inefficient setup with huge losses.
```

---
## \#20 Posted by: Hummie Posted at: 2017-08-02T20:35:28.604Z Reads: 74

```
so hitting the limit would cause a shutdown as apposed to holding the motor to a max erpm that it could run at?  oo.  but why do you say his set-up is inefficient?
```

---
## \#21 Posted by: milesperhour Posted at: 2017-08-02T20:36:45.155Z Reads: 75

```
I believe I can use soft limits on the controller side though. I chose such a high rpm combination because I wanted very high torque for climbing hills. From my calculations I should be able to do a 25% grade hill at 20 mph
```

---
## \#22 Posted by: Jinra Posted at: 2017-08-02T20:38:16.774Z Reads: 70

```
you usually want lower kv motors for more torque not higher
```

---
## \#23 Posted by: milesperhour Posted at: 2017-08-02T21:42:36.227Z Reads: 67

```
I tried taking out one of my batteries so I would have 6s but I have the same problem. The motor spiked up to 21000 ERPM and then cut out
<img src="/uploads/db1493/original/3X/3/f/3fab4ebc936e69a93b065412b6dc00b263fbacb8.png" width="690" height="297">
```

---
## \#24 Posted by: milesperhour Posted at: 2017-08-02T21:43:30.845Z Reads: 63

```
@jinra shouldnt this work since I am way under the ERPM max of 60,000
```

---
## \#25 Posted by: Jinra Posted at: 2017-08-02T21:44:43.881Z Reads: 62

```
6S will probably still hit the limit. If you really want to do detection on that motor, you can raise the limit to 100k temporarily.
```

---
## \#26 Posted by: milesperhour Posted at: 2017-08-02T21:45:54.313Z Reads: 59

```
I will try that, but the real time is only reading 21,000. nowhere near 60k.
```

---
## \#27 Posted by: Jinra Posted at: 2017-08-02T21:47:25.244Z Reads: 60

```
Detection makes the motor spin at varying eRPM's
```

---
## \#28 Posted by: milesperhour Posted at: 2017-08-03T20:53:02.540Z Reads: 56

```
Thanks for the help everyone. I got the motor to detect by upping the current to 7A. All the tutorials said to set current between 1 and 6A but it wouldn't work for me until I increased it.
```

---
