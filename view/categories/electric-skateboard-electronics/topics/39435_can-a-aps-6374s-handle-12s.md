# Can a APS 6374S handle 12s?

### Replies: 16 Views: 1001

## \#1 Posted by: falesias Posted at: 2017-11-27T10:39:50.299Z Reads: 156

```
Hi eSK8 community,
is a APS 6374S motor capable of handling 12s configuration?
or is 10s really the max?
is it safer to choose a turnigy SK3? (the downside is it is not sensored)
I would really appreciate some wise words on this subject from you experienced builders out there...
thanks
```

---
## \#2 Posted by: Erniechan Posted at: 2017-11-27T10:46:54.100Z Reads: 156

```
I read they have a great customer service....
I guess your best choice is ....ask aps? They will know it for sure.
```

---
## \#3 Posted by: falesias Posted at: 2017-11-27T11:05:55.017Z Reads: 153

```
Brilliant!
```

---
## \#4 Posted by: ARetardedPillow Posted at: 2017-11-27T11:09:38.026Z Reads: 151

```
Lol ofc, even the sk3 is rated at 10s max but you can still take it up to 12s without a single problem, just that its the other components might be "unstable"
```

---
## \#5 Posted by: Kug3lis Posted at: 2017-11-27T11:16:21.763Z Reads: 145

```
also I think those specs are set for optimal performance and efficiency
```

---
## \#6 Posted by: falesias Posted at: 2017-11-27T11:17:40.666Z Reads: 144

```
I see, 
I ordered 2 FOCBOX Motor Controller, and was deciding on the motors...
My first idea was the SK3 6374, but then I realized it is not a sensored motor and it can be trouble at start for a stand still. 
So I turned my attention to APS because the are sensored motors but then... it says 10s in the specs.
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2017-11-27T11:19:44.620Z Reads: 140

```
If youre going dual 6374, you can still start from a standstill lol, I run dual 6374 and I never get off my board, I do full stops and accelerate with no problem, thing moves like Im not even on the board
```

---
## \#8 Posted by: ARetardedPillow Posted at: 2017-11-27T11:20:28.555Z Reads: 135

```
Havent tried sensored but I want to in the future, but dont worry lol 12s wont do anything to a motor, heck I dont even think 14s is a problem
```

---
## \#9 Posted by: rojitor Posted at: 2017-11-27T12:21:41.219Z Reads: 128

```
I ordered a few times from aps and they answered my questions within an hour. I can't understand why you ask this here. Just contact alien.
```

---
## \#10 Posted by: gogomrrobot Posted at: 2017-11-27T12:31:22.984Z Reads: 123

```
[quote="ARetardedPillow, post:7, topic:39435, full:true"]
If youre going dual 6374, you can still start from a standstill lol, I run dual 6374 and I never get off my board, I do full stops and accelerate with no problem, thing moves like Im not even on the board
[/quote]

Yes, mostly.  Now I have a 6365 from Maytech -- it has sensor wires which I am going to finally hookup.  But without them and the VESC6 motor output current set high enough -- the motors jitter. If I push just a little forward all copacetic. Maybe with 6374 that wouldn't be an issue.  But technically, 6374 of Maytech says 3550W. Whereas 6365 says 3520W.

Also, it depends on your weight. I am 185 with gear on -- you probably weigh less.  My friend is 118... I had a test trial with her on the board. No motor jitters.... less weight lower static coefficient of friction.

So the sensored or sensorless thing... it matters with VESC's... ESC is a different story of jerk you forward as long as you push the throttle hard enough...lol.

Anyways this is all a side bar... get sensored if possible... it's better in all different ways.  APS 6374 will have no issue with 12S. In fact here aren't any 6374 motors we talk about on this forum that can't handle 12S. Their motors are beastly.
```

---
## \#11 Posted by: rich Posted at: 2017-11-27T12:45:36.841Z Reads: 109

```
From my personal experience with sensored 6364 Motors (Trampa & Maytech) there was absolutely no difference in cogging compared to sensorless in BLDC mode. The jittering was awful but the low rpm control was better. Only sensored FOC solved all my problems and is so much better in performance. I can start from standstill without any cogging, even uphill. Sensored/hybrid BLDC couldn't deliver that.
```

---
## \#12 Posted by: falesias Posted at: 2017-11-27T15:16:06.779Z Reads: 104

```
Thanks very much for your comment
```

---
## \#13 Posted by: Namasaki Posted at: 2017-11-30T15:11:35.394Z Reads: 94

```
Based on my personal experience I recommend that if your priority is highest possible performance then 12s
If your priority is acceptable performance with dependability then 10s
```

---
## \#14 Posted by: falesias Posted at: 2017-11-30T18:09:21.249Z Reads: 89

```
Yes, im looking for performance. 
Not highest speed. Im looking for highest torque or climbing ability.
We have a lot of hills around here. You can't go anywhere without having to climb or/and descend hard.
```

---
## \#15 Posted by: Namasaki Posted at: 2017-11-30T18:36:28.928Z Reads: 83

```
You can have excellent climbing ability with 10s and have good reliability. 
I have a board built for hills. 
Dual drive
10s 60C Lipo pack for minimum voltage sag
6374 motors (noticeably more torque than 6355’s)
90mm Wheels
40/15 pulleys
From my experience, 12s does increase power and acceleration as well as top speed but it seemed to put more stress on the system. I often had issues with motors and electronics getting hot. 
One time just going 20mph for about 5 miles on flat ground against the wind, my external E-switch got so hot the shrink tube on it split open and the circuit failed.
```

---
## \#16 Posted by: pixelsilva Posted at: 2018-01-20T02:34:57.530Z Reads: 65

```
Think of 12S as a V12 engine and 10S as V10 engine..... V12 engines are use primarily in high end super sport cars, Ferraris, Lamborghinis, etc. Exotic AFk, temperamental, fragile, complex, powerful, difficult to tame. There, 3 cents.
```

---
