# 1 week of riding later - Have some questions

### Replies: 17 Views: 910

## \#1 Posted by: paul775 Posted at: 2016-08-20T08:23:32.639Z Reads: 156

```
First some general deck information:

* Chaka's VESC
* 190kv SK3 6364 Motor
* 9S (3x3s) Series 5000mAh 30C
* Winning Remote
* TB Motor Mount

> **Question 1: I throttle up and then right away thumb off throttle/remote I get a bump/jolt**

When I throttle up and then let go of it I get a weird bump. I would like to find out why I get this bump because at high speeds this may lead my board to a wobble and then crash. 
My guesses are VESC Current Settings, VESC PPM Settings, or Winning Remote Tuning.

_I also messed up a bearing on one of my wheels so I bought more bearings to fix that. That could be it. I will know on Sunday and test it again to rule it out._

<img src="/uploads/db1493/original/2X/c/cc053681f0708828d29b1670b2871e3b399e5f6d.png" width="690" height="229">

> **Question 2: Belt can not go fully on top of big pulley**

My 12mm belt isn't completely on the Drive Wheel Pulley. The board runs completely fine and have done at least 2 miles every day for the past 5 days. Since my mount finally does not move at all and everything is fine I will not mess with it but for clarification how bad is it this?

_Left side is the normal riding setup. Right side is for comparison._
<img src="/uploads/db1493/original/2X/e/e72e07fed7507833edf6243800398389499d2b37.png" width="590" height="394">

> **Question 3: LiPo question**

For LiPo's, is it safe to keep the 3 x 3s batteries in series plugged in but not plugged into the VESC (At least 2 hours)? That can be my on/off switch. They will be capped off so no metal will touch unless I take the caps off.

<img src="/uploads/db1493/original/2X/9/95100f89e97e111dea3f3c452ced30ae90239971.png" width="590" height="380">
```

---
## \#2 Posted by: makevoid Posted at: 2016-08-20T08:33:21.136Z Reads: 142

```
1. Post your PPM settings, you may need to re-tune min ppm and/or increase deadband. Check that when you let go your finger the value returns to 50% (neutral position) correctly

2. Ideally you want to adjust it so it stays 99% on top of the pulley, otherwise you will shoorten the life of your belt, fine adjusting and locking/threadlocking your mount can be tricky but when you get it right it should stay in place basically forever, then you need to care just about belt tension. If you're light / don't brake too hard the belt will not wear fast too so the current situation may be right for you.

3. Totally fine
```

---
## \#3 Posted by: i2oadsweepei2 Posted at: 2016-08-20T09:29:11.793Z Reads: 131

```
My belt was like that too and still overhangs by a hair. I might be crazy but when I flipped the wheels around so the sidewall with the rings was facing outward and more of the belt sat on the pulley. If that is a @torqueboards pulley then he has spacers I believe. Though mine is fine without them. Over 200kms and I'm about to add another 16km or so this morning.
```

---
## \#4 Posted by: paul775 Posted at: 2016-08-20T09:51:38.224Z Reads: 123

```
Thanks for the reply. I will post ppm picture and will try to adjust the belt tomorrow. Heading to sleep now
```

---
## \#5 Posted by: paul775 Posted at: 2016-08-20T09:53:31.296Z Reads: 116

```
That's funny haha. I will try to flip it if my loctite will allow it tomorrow.
```

---
## \#6 Posted by: popopopop Posted at: 2016-08-20T10:51:00.910Z Reads: 109

```
I have TB's mount. Your clearance looks fine from the before pic, even if you had 1-2 mm more of overhang. Are you sure your wheel pulley is straight and doesn't wobble? Take off your belt and spin your wheel to check. This was the issue that caused my belt to look like the left side. Flipping it to the shallower side of the wheel helped the alignment, but I think only because I started it on a fresh wheel.
```

---
## \#7 Posted by: Chris1 Posted at: 2016-08-20T16:15:41.887Z Reads: 93

```
<img src="/uploads/db1493/original/2X/3/3b5af6ab5e861b12a2927ea2cac14c494cb41594.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/d/d0fb9f3a174957385691b98bd18e370a0756f313.jpeg" width="375" height="500">
I found that the TB wheel pulley sits too far into the hub of the drive wheel.  You need to make a spacer out of a large washer and put that behind the pulley.  I used the one that came with the wheel pulley on the inside then my drilled washer on the outside.  You will also need 6 6mx55 bolts, the 6mx50's that come with the kit are a hair too short.
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-20T16:20:42.426Z Reads: 92

```
Are you film throttling and then letting go completely? or just returning it to neutral? If you let it go, the momentum from the throttle snapping back could be triggering the pwm signal to brake. You can fix this by increasing the dead band.
```

---
## \#9 Posted by: paul775 Posted at: 2016-08-20T19:44:33.404Z Reads: 85

```
I am fully throttling and then letting go completely. Since it's the Winning Remote, if I fully let go I presume it should go to neutral as well.

I have increased the Dead Band from **0.15 to 0.25**. 

I have to test it again on my flat street which I'll do Sunday since I have work right now. I only notice the bump when I'm at high speeds (like 10mph and then fully throttling to 15mph and letting go, right then I get a bump).

<img src="/uploads/db1493/original/2X/1/1d84e70801fc4ba2539a152e03d24a527a2c7357.png" width="690" height="350">

<img src="/uploads/db1493/original/2X/e/e3e2ac8acfc588015e90f4bea254a366e5deed8c.png" width="690" height="244">

Here's a quick video I made yesterday before this thread. I was trying to go 20mph+ but that bump at 12 second scared me haha.

https://youtu.be/bAiKPRjEh7c
```

---
## \#10 Posted by: Jinra Posted at: 2016-08-20T19:56:07.707Z Reads: 76

```
It could just be the resistance is slowing the board down since you're no longer supplying current to the motors.
```

---
## \#11 Posted by: makevoid Posted at: 2016-08-20T20:14:11.516Z Reads: 72

```
I can hear a little brake, I don't think it's just motor resistance. I still suspect that the thottle goes to 40% or something when you release it and it breaks a bit. This thing doesn't happen if instead of letting go the throttle you accompany it to 50% (neutral position) right? 
Also we can't see the Display bar because the screenshot is cut, Ideally you want 99-100% when you're full throttle and 49-50% when neutral. If you look at that screen and accelerate then release the throttle, does the pulsewidth display bar goes to 50% or it goes for a split-second to 40%? Also I think deadband setting is pretty high, it shouldn't be a problem of that beeing too low.
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-20T20:15:20.804Z Reads: 68

```
I didn't watch it with sound, but I suspect he may just have to rebind to reset neutral throttle on the remote.
```

---
## \#13 Posted by: paul775 Posted at: 2016-08-20T20:54:19.309Z Reads: 65

```
Okay I will later connect the remote and check where neutral is.
```

---
## \#14 Posted by: treenutter Posted at: 2016-08-20T20:55:06.593Z Reads: 63

```
[quote="paul775, post:1, topic:7973"]
Question 1: I throttle up and then right away thumb off throttle/remote I get a bump/jolt
[/quote]

@paul775  when I experienced this it was because the deadband of Ppm wasn't high enough for the remote, so letting the throttle return to center triggered a moment of braking. Try adjusting your PPM mix and max, and increase deadband.
```

---
## \#15 Posted by: makevoid Posted at: 2016-08-20T21:25:39.308Z Reads: 57

```
I think 0.25 it's pretty high, I usually use 0.1 max, I don't think that's the case
```

---
## \#16 Posted by: sl33py Posted at: 2016-08-20T22:01:38.784Z Reads: 59

```
[quote="paul775, post:1, topic:7973"]
Left side is the normal riding setup. Right side is for comparison.
[/quote]
Your pulley looks pretty far from the motor mount.  That distance may give some leverage to moving the belt.  I would work on alignment to try and keep the belt fully on the gerar. 

[quote="Chris1, post:7, topic:7973"]
I found that the TB wheel pulley sits too far into the hub
[/quote]

Look at @Chris1's setup.  See how his motor gear is flipped to keep it close/flush w/ motor mount?  Is yours like that or do you have it reversed?  That may be part of an alignment issue.  I'd also move the motor mount as close to the gear as possible (with it lining up).  And the last spacer suggestion to move the wheel gear out a hair likely would help.

GL!
```

---
## \#17 Posted by: paul775 Posted at: 2016-08-20T22:57:17.338Z Reads: 50

```
Okay I will mess around with the pulley/belt, then fix my bearings, then will change my Deadband back to 0.15 and check how close Neutral is to 50% and I'll report back! Thanks guys!
```

---
