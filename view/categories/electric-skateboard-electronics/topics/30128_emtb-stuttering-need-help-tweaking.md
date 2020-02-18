# eMTB stuttering, need help tweaking

### Replies: 35 Views: 1078

## \#1 Posted by: bmcm Posted at: 2017-08-09T00:19:23.157Z Reads: 81

```
Hello All,

* MBS 200mm tires with 72T drive pulley
* Turnigy SK3 190kv 6364 motor with 20T pulley
* 9mm HTD5 belt
* 10S3P LG MJ1 (10A) battery back + basic 40A BMS
* Ollin VESC with Ackomaniac firmware (4.28) - also happened with stock Ollin/VESC FW 4.12
* Nunchuck (wired)

[https://youtu.be/zcbOHjKYmw8](https://youtu.be/zcbOHjKYmw8)

As you can see in the video, the motor stutters a lot during startup and when moving. The video and sound should hopefully be more descriptive than words. You can also see the watts-up meter, which shows < 10A draw - doesn't seem to be hitting the max amp threshold. 

Doesn't happen when there's no weight on the board, only when I'm on it (150lbs).

I can't tell if it's mechanical (belts and pulleys slipping, etc), or electronic/wiring (power delivery, etc), or software (VESC settings, etc). 

Does anything stick out for anyone?

<img src="/uploads/db1493/original/3X/9/1/91b74c2da9509ee1f9f8aaafe3e586f4fdda1754.png" width="690" height="277"><img src="/uploads/db1493/original/3X/8/a/8a21c78712bd492f185583f41dc8e0ceae493baf.png" width="690" height="217"><img src="/uploads/db1493/original/3X/8/c/8c30b48b9805af44b317f3c05b889819f7b8c51c.png" width="690" height="197"><img src="/uploads/db1493/original/3X/5/0/50bd09e077ab1026d66f6aceef6d13e62f572395.png" width="690" height="380">

Thanks in advance!

@chaka ideas?
```

---
## \#2 Posted by: JLabs Posted at: 2017-08-09T00:21:32.554Z Reads: 71

```
All motors without sensors will stutter on startup. There may be some settings you can tweak to help but I am no expert.. @Jinra do you have any advice?
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-08-09T00:22:34.294Z Reads: 71

```
Yea that’s a normal problem, not much you can do to change that than maybe up the startup boost to .30.
```

---
## \#4 Posted by: bmcm Posted at: 2017-08-09T00:25:17.920Z Reads: 71

```
Thanks for the quick feedback. I can try adjusting the startup boost and see.

What about during riding (not coasting, but keeping speed)? Almost sounds like slippage. Would an idler to keep tension help?
```

---
## \#5 Posted by: racidon Posted at: 2017-08-09T00:26:10.117Z Reads: 70

```
Have you tried FOC?
```

---
## \#6 Posted by: bmcm Posted at: 2017-08-09T00:30:55.856Z Reads: 71

```
@racidon I did, but couldn't get it setup correctly. After applying all the parameters and rebooting, the nunchuck doesn't spin the motor at all, or produce any sort of life. And I can't detect hall sensors (detection moves motor a few degrees forward and back, but then errors).
```

---
## \#7 Posted by: bmcm Posted at: 2017-08-09T00:33:58.227Z Reads: 65

```
BTW, with a 20T and 72T pulley, I'm supposed to get between 7 and 8 teeth of contact, which according to the several online calculators, should be plenty. Unfortunately my 2 pulleys are about 3-5mm from each other :sweat:
```

---
## \#8 Posted by: Jinra Posted at: 2017-08-09T00:35:45.550Z Reads: 64

```
You'll need sensors for smooth start up, I'll check out the video when i get home
```

---
## \#9 Posted by: bmcm Posted at: 2017-08-09T00:39:21.953Z Reads: 63

```
@GrecoMan's suggestion of increasing the startup boost (I just made it 0.060, not 0.3) absolutely helped. But I'm getting awful jerking while moving.


@Jinra darn ... already invested in more unsensored SK3's for making this one a dual-motor, plus another one for another board.
```

---
## \#10 Posted by: GrecoMan Posted at: 2017-08-09T00:41:36.866Z Reads: 61

```
I think for satellite it’s recommended that you stay below .50 startup boost.  But having dual motors should help your problem a lot.  It can also be solved with a simple push before you start riding
```

---
## \#11 Posted by: bmcm Posted at: 2017-08-09T00:42:15.390Z Reads: 56

```
@GrecoMan I hope you mean 0.050, not 0.5?
```

---
## \#12 Posted by: GrecoMan Posted at: 2017-08-09T00:42:38.964Z Reads: 55

```
Haha yes, .050
```

---
## \#13 Posted by: GrecoMan Posted at: 2017-08-09T00:50:53.940Z Reads: 53

```
also @bmcm a wider belt will help with more torque transfer.  12mm or 15mm are the best
```

---
## \#14 Posted by: bmcm Posted at: 2017-08-09T00:53:43.610Z Reads: 51

```
@GrecoMan yep, agreed. At the time I bought the drivetrain, SDP-SI did not have options for anything wider than 9mm for my ratio, specifically the larger drive pulley at 72 teeth. If I go wider I might have to 3d print my own out of nylon (not impossible since I have a Prusa MK2 3d printer).
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-08-09T00:56:09.392Z Reads: 49

```
with dual motors it should be fine, ive seen a lot of other people (I think ive seen @jinra use 9mm belts on a dual drive) use 9mm on dual with no problems
```

---
## \#16 Posted by: Jinra Posted at: 2017-08-09T01:00:48.085Z Reads: 50

```
Yea just got home and saw the video. You will either need sensors to help with the startup or kick start to get going. VESC has no idea the position of the rotor can so it can't give you a smooth startup. You can try .1 startup boost to see if it's any better. It may work better with dual motors, albeit unreliably.
```

---
## \#17 Posted by: bmcm Posted at: 2017-08-09T01:03:22.013Z Reads: 49

```
Thanks, @Jinra.

Any advice, though, on fixing the jerking that happens when moving?   It's apparent after 40s into the video.
```

---
## \#18 Posted by: Jinra Posted at: 2017-08-09T01:04:25.740Z Reads: 49

```
Is it that loud thudding sound? What is that? Does the jerking happen with you off the board?

@bmcm given that you're running a MTB you should leave absolute max at the default 130 value. Also your battery min is way too high. Don't regen above rated current of your cells.
```

---
## \#19 Posted by: bmcm Posted at: 2017-08-09T01:04:30.409Z Reads: 47

```
Yeah, more and more I'm tempted to just bite the bullet and commit to dual motors. I just didn't feel like spending another $250-300 (vesc, pulleys, belt, motor mount) but I might have to.
```

---
## \#20 Posted by: bmcm Posted at: 2017-08-09T01:06:06.013Z Reads: 44

```
@Jinra Yep, that's it. It happens when moving. Not sure - possibly the belt.  I think it only happens when I'm on it.
```

---
## \#21 Posted by: GrecoMan Posted at: 2017-08-09T01:06:19.414Z Reads: 42

```
Dual motors wont fix what sounds like an electrical problem in one motor.  It will feel exactly the same with dual motors.  Have you taken it outside yet?
```

---
## \#22 Posted by: Jinra Posted at: 2017-08-09T01:06:48.126Z Reads: 43

```
give it a kick start, then throttle to see if the thudding sound is still happening.
```

---
## \#23 Posted by: GrecoMan Posted at: 2017-08-09T01:06:58.572Z Reads: 44

```
Oh than I would recommend a tensioner if its a problem with the belt
```

---
## \#24 Posted by: bmcm Posted at: 2017-08-09T01:10:16.944Z Reads: 44

```
Strange. When set to FOC the nunchuk doesn't produce any input (the progress bar Display stays 50%) whereas when set to BLDC the nunchuk works fine.
```

---
## \#25 Posted by: Jinra Posted at: 2017-08-09T01:11:40.353Z Reads: 43

```
You gotta run detection for FOC if you want to use it. Also be careful applying throttle to non-moving motors. Large current on a stalled motor will kill it and /or the VESC.
```

---
## \#26 Posted by: bmcm Posted at: 2017-08-09T01:17:42.493Z Reads: 45

```
@Jinra I did run detection for FOC. 

And thanks, yeah. I'm careful about that. I've learned my lesson with other motors in other projects. 

<img src="/uploads/db1493/original/3X/a/9/a98415c8d78bc71cfc44091ce241020c54117a88.png" width="690" height="413">

@edit I cannot get the hall sensor detection to ever work, though. Is that required for FOC setup to be complete?
```

---
## \#27 Posted by: Jinra Posted at: 2017-08-09T01:18:39.993Z Reads: 45

```
Hm, not sure then. I have zero experience with using a nunchuck based control mode
```

---
## \#28 Posted by: GrecoMan Posted at: 2017-08-09T01:21:04.872Z Reads: 44

```
Yup same here, I cant help you.  Ive only ever used the GT2B :grin:
```

---
## \#29 Posted by: GrecoMan Posted at: 2017-08-09T01:23:24.588Z Reads: 44

```
Not meaning to hijack the thread with this random question, but without looking at my profile, how old would you guys guess I am? @Jinra @bmcm
```

---
## \#30 Posted by: bmcm Posted at: 2017-08-09T01:27:36.290Z Reads: 41

```
Haha, I know your true age, but you're right in that you come across older. So if that's what you're going for, good job :-) And thanks for the help.
```

---
## \#31 Posted by: GrecoMan Posted at: 2017-08-09T01:29:50.190Z Reads: 41

```
Haha darn! Ive gotten mixed results with people not taking me seriously because I'm so much younger than most everyone on here.  That said, I'm no supergenius, just your average highschool freshman with hopes of being an electrical engineer one day.
```

---
## \#32 Posted by: bmcm Posted at: 2017-08-09T01:32:45.357Z Reads: 41

```
Looks like my drive pulley is also badly out of alignment with the wheel. I had a suspicion, but looking at the belt moving the way it is, it's definitely wrong. Probably contributing to the issue I'm getting while moving.

https://youtu.be/jSqpxEMuRJo
```

---
## \#33 Posted by: GrecoMan Posted at: 2017-08-09T01:36:41.304Z Reads: 39

```
MY EYES!!!   All though ive just been blinded by that horrible sight, that should not be the main cause of your problem.  It definetly contributes to your start up problem because It puts a crazy amount of stress on the belt which makes it incredibly hard for the motor to spin, I discovered this well tensioning my belt the other day.  So please for the love of god get that straightened out and report back
```

---
## \#34 Posted by: Jinra Posted at: 2017-08-09T01:48:42.267Z Reads: 37

```
Yea you should definitely fix that before running it on the belt again, it can be a pain to get just right.

@GrecoMan uhh, 17?
```

---
## \#35 Posted by: GrecoMan Posted at: 2017-08-09T01:50:17.619Z Reads: 38

```
Haha @Jinra I'm only 13, the goal is to make people realise that just because I'm younger than them doesn't mean I'm not trustworthy.
```

---
