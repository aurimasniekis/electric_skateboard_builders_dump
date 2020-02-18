# Drive System Bottlenecks &amp; 4100W Single Motor

### Replies: 43 Views: 885

## \#1 Posted by: kuphjr Posted at: 2018-07-12T22:03:38.697Z Reads: 187

```
So @torqueboards recently released their [4100 6390 motor](collections/electric-skateboard-motors/products/electric-skateboard-motor-6380-170kv) and it got me thinking.  Is there any real benefit to these motors compared to their 6374 motor other than the 20kv difference?  Since the focox can only handle 60A continuous (and from what I have read burst current is pretty much irrelevant in a sealed enclosure), the bottleneck is the speed controller and not the motor, right? The maximum power a focbox could deliver at 12s is ~2800W so any motor more powerful than 3000 watts should be irrelevant.

Can anyone with a 4000+ watt motor answer any of these questions?

Also, it would seem that if you have a 3p battery that can produce 60A continuous, there is no increase in the amount of continuous power that can be generated between a dual motor versus a single motor drive system, right?  I know logically this would be the case, but I want to know if people have different experiences in real application.
```

---
## \#2 Posted by: wafflejock Posted at: 2018-07-12T22:10:25.636Z Reads: 178

```
12S x 4.2 = 50.4V × 60A max (pretty sure this is the limit on vesc components) is at 3000W so fully charged you could in theory put that much power through the system.  Regarding discharge on a single battery through multiple escs/motors you do basically get one half the output for each each/motor but you will generally have less loss from heat both in splitting the power.  Would expect higher efficiency but no real world experience.
```

---
## \#3 Posted by: kuphjr Posted at: 2018-07-12T22:24:20.654Z Reads: 171

```
Yeah I used ~3.7 volts for the wattage calculation in my first post, but the main point I was making is that there is theoretically absolutely no difference between the 4100 and 3100 watt motors while using a focbox if you correct for the 20kv difference by using a different gear ratio.  I guess the only slight difference would be the 6380 motor might be able to dissipate heat slightly better due to the increased surface area, but I bet the real world difference is imperceptible.
```

---
## \#4 Posted by: Holyman92 Posted at: 2018-07-12T22:41:32.103Z Reads: 160

```
[quote="kuphjr, post:1, topic:61698"]
So @torqueboards recently released their [4100 6390 motor ](collections/electric-skateboard-motors/products/electric-skateboard-motor-6380-170kv)
[/quote]

6380* and I had this same thought... we would need an 8000w system to take advantage of these motors full potential... @Kug3lis wheres tht ESC at lol
```

---
## \#5 Posted by: Battosaii Posted at: 2018-07-12T22:42:17.931Z Reads: 152

```
Larger stator has more physical leverage making more torque. Watts doesn't seem to mean much.
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-07-12T22:43:25.400Z Reads: 153

```
I was able to utilize my 4kW motors even with 4.5kW using simple FocBoxes and our case ;)
```

---
## \#7 Posted by: Holyman92 Posted at: 2018-07-12T22:44:06.161Z Reads: 151

```
I want a vesc 6... and really? You're able to keep them that cool...
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-07-12T22:45:06.717Z Reads: 150

```
I never reached more than 50ºC at 26ºC outside :)
```

---
## \#9 Posted by: Holyman92 Posted at: 2018-07-12T22:45:53.972Z Reads: 143

```
Very nice... I can't wait to get ur case installed... I just got my caps but I'm having a bit of trouble sadly
```

---
## \#10 Posted by: strattos Posted at: 2018-07-12T22:48:59.012Z Reads: 143

```
Spot on the money the larger motor will have better cooling. Personally a single 6374 is more than enough power for my skinny ass. Tho I'm sure I woulda gone for the 68xx if torqueboards was selling them when I was ordering parts.
```

---
## \#11 Posted by: Kug3lis Posted at: 2018-07-12T22:49:29.392Z Reads: 138

```
I dont know if you will be able to reach same performance on 4.12 with dual case but I am using it with Finned so it dissipates much better ;)
```

---
## \#12 Posted by: Holyman92 Posted at: 2018-07-12T22:52:02.312Z Reads: 136

```
I plan to have air vents cut on my enclosure that force air in from the front and have to blow across the case to escape in the back, should help keep the batteries a little cooler too since they are gonna be in the enclosure as well
```

---
## \#13 Posted by: kuphjr Posted at: 2018-07-12T22:56:10.238Z Reads: 135

```
Yes, but couldn’t you just use a different gear ratio to account for the difference?
```

---
## \#14 Posted by: kuphjr Posted at: 2018-07-12T22:57:48.860Z Reads: 134

```
I have heard that in real world performance the thermals are nearly identical to the focbox in other threads.
```

---
## \#15 Posted by: kuphjr Posted at: 2018-07-12T22:58:29.399Z Reads: 136

```
I heard about your cases in another thread too! I am definitely going to pick one up sometime.
```

---
## \#16 Posted by: Holyman92 Posted at: 2018-07-12T23:00:39.493Z Reads: 136

```
![1531436357677342242694|375x500](upload://8tvlbKYCdxWjnEtn7hCgUyJ0W87.jpg)
![1531436423355472547138|375x500](upload://nvMhMPRO9bHKH7YSYuJ8dLbseNi.jpg)
```

---
## \#17 Posted by: PatRocks Posted at: 2018-07-12T23:32:59.753Z Reads: 126

```
@Kug3lis 's dual case is pretty freaking rad. The highest temperature I have seen since installing it is 45 C, and that was on a 20 to 22% Hill test (hill street, San Diego). Once I let off, the temp just plummets. Great design, highly recommend it.
Edit: careful with the installation, it's critical that the fets are in contact with the thermal pads. I had this wrong initially 😅
```

---
## \#18 Posted by: Holyman92 Posted at: 2018-07-12T23:38:25.133Z Reads: 127

```
I like it, but the link for the caps in his post are wrong... those are still too long lol... they are shorter and will fit, but the wires will get cut... so here's my work around in the 2nd pic

![1531438611465513106721|374x500](upload://jIPEo3ykiTv24KJd9ElPkWjlP8G.jpg)

![1531438684517551823596|375x500](upload://jeUSu6xMhPur2LucVeqAxxBZ9jS.jpg)
```

---
## \#19 Posted by: PatRocks Posted at: 2018-07-12T23:39:30.610Z Reads: 126

```
Oh my bad I was talking about the dual focbox case
```

---
## \#20 Posted by: kuphjr Posted at: 2018-07-16T18:25:47.135Z Reads: 101

```
Can anyone comment on the traction difference between dual and single motors for hard acceleration and breaking? Does it really matter? How much do you notice the uneven drive from the back wheels?

Also, has anyone ever had issues with belts breaking while using a 3000-4000 watt single motor setup?
```

---
## \#21 Posted by: sodniwe Posted at: 2018-07-16T18:44:42.374Z Reads: 98

```
I run the 6380 on a single wheel setup with a 12S 3P battery at 60 amps.  The amount of torque the board has is insane.  I think another motor is always best for braking and going up hills but otherwise the board works well.  I’m gonna try a 20mm belt and better remote to help control the torque a bit better.  Otherwise I’m switching to a dual drive setup
```

---
## \#22 Posted by: kuphjr Posted at: 2018-07-16T18:50:45.240Z Reads: 97

```
I understand the benefit of dual motors for breaking because 2 VESCs can dissipate more energy than 1 and there is more breaking surface area in contact with the ground (and redundancy if a belt breaks), but you should arguably have the same performance up hills with a dual motor because the battery is the bottleneck in power output, not the motors.  Unless you find your back wheel slipping when you go up hills, in which case a dual motor setup will give you more grip.
```

---
## \#23 Posted by: sodniwe Posted at: 2018-07-16T18:52:46.115Z Reads: 94

```
Yes - I also definitely experience slippage on VERY steep hills but think dual drive might also have issues
```

---
## \#24 Posted by: kuphjr Posted at: 2018-07-16T18:53:58.490Z Reads: 92

```
Just to clarify, is it slippage between the wheel and the ground or between the belt and the motor pulley?
```

---
## \#25 Posted by: sodniwe Posted at: 2018-07-16T18:55:43.402Z Reads: 92

```
I get both on very steep hills sometimes.  I think running 20mm belts would be best on a one wheel setup but doesn’t help with wheel traction
```

---
## \#26 Posted by: kuphjr Posted at: 2018-07-16T18:55:47.046Z Reads: 90

```
I've been riding my dual drive for awhile and so far I can honestly say I prefer my single drive because of how much better it is on battery and how much less friction there is while gliding.

The reason I am asking questions is because I just want to see if there are any drawbacks to very large single motor drives. I don't want to spend $135 on a 4100 W single motor to find out that all it does is cause slippage.
```

---
## \#27 Posted by: sodniwe Posted at: 2018-07-16T18:58:14.602Z Reads: 87

```
Gotcha - my torque is so high I just shredded a belt and can’t ride it till the new one comes in.  I think is partially cause my nano remote is terrible / too sensitive and I’m still dialing in my vesc settings with the new motor.  I’m planning on building a nano remote to help solve the issue.  I would def recommend a 20mm belt for this or any single drive (haven’t tested 20mm yet though)
```

---
## \#28 Posted by: kuphjr Posted at: 2018-07-16T19:01:05.831Z Reads: 87

```
Yeah, I am sure 107mm 74A ABEC11 Flywheels should eliminate any wheel slippage and I am using @marcmt88 motor mounts with idler pulleys which should really minimize any belt slip. Are you using idler pulleys?

Also do you have any pictures of your build? Also, I have 2 6355 3100W 260kv motors on @marcmt88 motor mounts all mounted to a TB 218mm hanger. If you want to work out a deal and trade your 6380 motor please let me know!
```

---
## \#29 Posted by: kuphjr Posted at: 2018-07-16T19:02:03.963Z Reads: 83

```
It uses 12mm belts with idler pulleys and I have never had one break in 4 months of riding.
```

---
## \#30 Posted by: sodniwe Posted at: 2018-07-16T19:05:19.738Z Reads: 82

```
I’m not running idler pulleys but have been thinking about it.  Would bigger wheels give better street traction?   I don’t have pictures on me but can record a video or throw up pictures tonight
```

---
## \#31 Posted by: kuphjr Posted at: 2018-07-16T19:07:50.542Z Reads: 83

```
Size does contribute to traction a little, but I think the softness of the wheels matters a lot more.  74A wheels are really soft and grippy compared to 78A and ABEC11 urethane is much better quality than generic wheels (at least according to what I have read on this forum).
```

---
## \#32 Posted by: Colson003 Posted at: 2018-07-16T19:28:58.532Z Reads: 74

```
Gearing is also something to consider. If it’s geared for torque you’re more likely to lose traction and peel out. If it’s geared for speed you’re less likely to lose traction, but at the expense of more heat.
```

---
## \#33 Posted by: FredrikHems Posted at: 2018-07-16T19:45:18.428Z Reads: 69

```
Torque steering and wheel slippage are the main reason I prefer dual. 4kw is more than enough for almost every one, but it doesnt matter how much power your motor has, If you cant put it down to the ground. Also the torque steering on powerful single can be pretty annoying If you are accelerating/braking hard.
```

---
## \#34 Posted by: wafflejock Posted at: 2018-07-16T20:19:13.508Z Reads: 63

```
Don't think I ever have issues with accelerating hard but I suppose I may just be steering unconsciously but definitely have noticed the braking tugs to one side if I'm hitting them hard.  Typically I just try to avoid braking hard, but in an emergency can catch you off guard.
```

---
## \#35 Posted by: skatardude10 Posted at: 2018-07-16T20:28:20.712Z Reads: 63

```
Do you have the Nano X from enertion?

If so, you need to calibrate your remote when you turn it on. Before you power on your board / ESCs, turn on your remote and pull full throttle and full brake. Then you can power on your board and it will behave normally. I used to have the same issue with my Nano X until I learned about this.... Crazy high torque and braking until I got up to full speed. Now I just do full acceleration and braking on the remote before powering on my board and it works normally.
```

---
## \#36 Posted by: kuphjr Posted at: 2018-07-16T22:34:06.300Z Reads: 52

```
I’m trying to develop a board for a small scale production to sell at my university and I fount think I can really justify the increase in price, but I really appreciate all the feedback!
```

---
## \#37 Posted by: sodniwe Posted at: 2018-07-17T00:35:49.696Z Reads: 47

```
skatedude10, I'm in love with you.  I don't have the Nano X from enertion but I have the nano remote from torqueboards.  I just did a short ride and i think that did that trick.  I had been turning down the throttle curve 100% and reducing the power of the board to try and compensate for this issue.  I need to give it some more testing but looks like that solved the issue!  I had read that before somewhere but it only talked about the nano x and thought it didn't apply to me :slight_smile:
```

---
## \#38 Posted by: Brdchris Posted at: 2018-07-17T01:13:51.779Z Reads: 42

```
Total newbie here, but I don’t think motor amps equal battery amps. Something with the inductance of the motor. So yea, theoretically two motors could better utilize battery and esc current
```

---
## \#39 Posted by: kuphjr Posted at: 2018-07-17T01:34:49.615Z Reads: 38

```
I'm not entirely sure that would be correct, but I certainly don't know everything there is to know about BLDC motors.

Just in theory, seeing as energy cannot be created or destroyed, the energy drawn from the battery should equal the energy used for acceleration minus whatever losses there are due to heat and friction regardless of how many motors and ESCs there are. The only way I could see a dual motor & esc setup being slightly more efficient is because everything would stay cooler, but I bet this increased efficiently would be far outweighed by the additional belt and motor friction of a dual drive vs a single drive.
```

---
## \#40 Posted by: Brdchris Posted at: 2018-07-17T01:40:32.197Z Reads: 34

```
No, you are wrong. Apparent and reactive and real power are all very different. Switching from dc to ac’ish can be a real doozy.
```

---
## \#41 Posted by: kuphjr Posted at: 2018-07-17T01:42:01.962Z Reads: 35

```
Really...

Well thank you very much for that information.  Do you have any idea where I might be able to get more educated about this? Can anyone else clear some of this up?
```

---
## \#42 Posted by: Brdchris Posted at: 2018-07-17T01:45:19.137Z Reads: 33

```
http://buildelectricboards.com/showthread.php?tid=164
```

---
## \#43 Posted by: kuphjr Posted at: 2018-07-17T02:04:32.437Z Reads: 33

```
This is a fantastic thread! Thank you so much!
```

---
