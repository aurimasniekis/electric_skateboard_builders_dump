# Need HELP! Motor rotates too slow

### Replies: 17 Views: 957

## \#1 Posted by: charlie17 Posted at: 2017-08-04T15:09:20.151Z Reads: 64

```
Hi,

I just start to build my electric state board, but I have a problem that the motor rotates too slow. I adjusted my motor configuration and setting hundreds of times still doesn't work. Really need some help there.

This is the setting of my board.
I get a Turnigy G160 Brushless Outrunner 245kv (160 Glow) from HobbyKing.
Two ZIPPY Compact 5000mAh 3s 40c Lipo Pack in series.
I also get an Enertion motor controller as my VESC.
<img src="/uploads/db1493/original/3X/3/8/38ad9bf951252e05b31f7df509738d4f400d36ab.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/2/6/26c18ef929430e8150b9fc4b6de3f0a4f0cd6a55.JPG" width="666" height="500">
This is mine motor configuration on BLDC tool.
<img src="/uploads/db1493/original/3X/8/a/8a907f6d6f2bb2647191e6e8bfa0f93216238fc7.jpg" width="690" height="375">
How can I get my motor work with the same components? Do I have to purchase more LiPo Battery to make it work?

Thanks
```

---
## \#2 Posted by: evoheyax Posted at: 2017-08-04T15:17:10.839Z Reads: 59

```
first off, set your motor amps to 120. You never set motor amps less than battery amps. Guarantee for bad performance.
```

---
## \#3 Posted by: Jinra Posted at: 2017-08-04T15:25:20.982Z Reads: 58

```
Please don't set your motor amps to 120... 

Did you run detection?
```

---
## \#4 Posted by: evoheyax Posted at: 2017-08-04T15:38:15.178Z Reads: 58

```
[quote="Jinra, post:3, topic:29688"]
Please don't set your motor amps to 120...
[/quote]

Have you tried it? Even if you don't want to set it so high, It should be higher.
```

---
## \#5 Posted by: Jinra Posted at: 2017-08-04T15:39:13.509Z Reads: 59

```
Look at the motor, it's a small stator single. They're going to burn out their motor at that setting.

I had a 5065 single running at just 60A motor and it was burning hot after a 1.5 mile incline.
```

---
## \#6 Posted by: charlie17 Posted at: 2017-08-04T16:25:52.395Z Reads: 55

```
I run the detection, but it says detection failed.
```

---
## \#7 Posted by: Alanhunt123 Posted at: 2017-08-04T16:28:04.314Z Reads: 54

```
Increasing the motor amp will only increase low end torque when duty cycle is low... Once he hits ~37% duty cycle, battery max would kick in (if he sets motor max to 120a). I've found battery max to be a much better way to control how much power the motors actually see.

Are you trying to do a motor detection, or have you already done that? If you are doing a motor detection, try taking the belt off.

I have tested VESC with lower voltage (5S) on a 245kv 6364 SK3, and the motor barely turned when I had the belt installed. Running on 8S the motor really showed some decent power. I've never had luck with VESC at low voltage like 6S, I suppose a higher kv might work better.
```

---
## \#8 Posted by: Jinra Posted at: 2017-08-04T16:28:11.667Z Reads: 51

```
Post screen shots. Try using a higher eRPM or current during detection (up to 1200 erpm or 6A current)
```

---
## \#9 Posted by: Sander Posted at: 2017-08-04T17:23:14.074Z Reads: 40

```
Isnt the Voltage wrong?
Input Min = 13
Input Max = 13
```

---
## \#10 Posted by: Jinra Posted at: 2017-08-04T17:24:32.826Z Reads: 40

```
no that's his battery cutoffs, which shouldn't be interfering with it unless he's perhaps using 3S.

@charlie17 you did make sure your batteries are in series and not parallel ya?
```

---
## \#11 Posted by: Sander Posted at: 2017-08-04T17:24:52.010Z Reads: 39

```
@charlie17 your input voltage is wrong!
Change the battery cutoff start to 25.2V
and battery cutoff end to 20.4V
```

---
## \#12 Posted by: Sander Posted at: 2017-08-04T17:25:36.005Z Reads: 39

```
He is using two 3s, and I am sure he is using it in series, 13 volt will not move the motor fast, 20V will move it much faster.

"Two ZIPPY Compact 5000mAh 3s 40c Lipo Pack in series."
```

---
## \#13 Posted by: Jinra Posted at: 2017-08-04T17:26:38.432Z Reads: 37

```
Well i mean the title of the post is "motor rotates too slow" so he could be using 3s on accident.

Correct cutoffs are not important for setup or detection, just needs to be lower than current working voltage.
```

---
## \#14 Posted by: Sander Posted at: 2017-08-04T17:27:46.569Z Reads: 37

```
well I ran my motors on 13 volts, they did not move fast, he is limiting the max voltage to 13.
```

---
## \#15 Posted by: Jinra Posted at: 2017-08-04T17:29:33.716Z Reads: 37

```
[quote="Sander, post:14, topic:29688"]
they did not move fast
[/quote]

That's the point, his problem is that they're moving slow. If he put his batteries in parallel on accident, it would explain that since it'd be below the cutoffs.
```

---
## \#16 Posted by: Sander Posted at: 2017-08-04T17:30:29.412Z Reads: 39

```
No I am talking about he has his Battery Cutoff start to 13V!
If he change it to 25.2V it moves much faster.
```

---
## \#17 Posted by: Jinra Posted at: 2017-08-04T17:32:33.230Z Reads: 38

```
No.. it doesn't. Cutoff is the voltage floor for which the power gets reduced. He could set it to 0v and it wouldn't make any difference as long as he's actually using 6s.

Once you get "battery cutoff start" power is reduced a bit. Once you hit "battery cutoff end" power is reduced almost completely.

That value is not max input voltage, max input voltage is above that and is correctly set to 57v
```

---
