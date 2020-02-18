# HELP! ABS overcurrent with dual Focbox on the bench

### Replies: 22 Views: 1233

## \#1 Posted by: Eboosted Posted at: 2017-07-09T23:38:53.069Z Reads: 150

```
I'm getting this error on the bench with no load at all, whenever I apply full throttle.

For instance I applied full throttle 4 times and got this error 4 times.

These are my settings:

Absolute Max is 130A, max motor I get is 51.1A, max battery 33.6A but as soon as I press the throttle 100% VESC would throw a DTC and reboots

<img src="/uploads/db1493/original/3X/e/0/e0cda6d2fe701c0fa94566908a1c74b14a0c00b5.png" width="281" height="500">f

<img src="/uploads/db1493/original/3X/d/6/d606a6f609e1452c72dd6f3d7ad54b8cc7e23486.png" width="281" height="500">
<img src="/uploads/db1493/original/3X/9/8/98d457a2b27c682205c78fdf361f5a82df940bfa.png" width="281" height="500">
<img src="/uploads/db1493/original/3X/7/4/74ae837e673ca02b3642a72b3508917a73732015.png" width="281" height="500">
```

---
## \#2 Posted by: rpn314 Posted at: 2017-07-10T00:37:38.428Z Reads: 138

```
Have you gotten this error out riding? Some things aren't very realistic on the bench.
```

---
## \#3 Posted by: Eboosted Posted at: 2017-07-10T02:04:54.986Z Reads: 133

```
Yes, I had it riding, it's a pretty scary feeling as the board keeps pushing and you loose control for a couple of seconds.

On the bench the current is even lower as no load is being applied and I also get >131A of filtered current.

I just opened the enclosure to check for loose/broken/crooked cables, everything was fine.

However I tried to make motor detection and I realized I can no longer make motor detection with one VESC, I even tried with the other motor and detection fails the same, the ABS fault is thrown everytime I tried to make motor detection with this VESC.

The other VESC can make motor detection perfectly on both motors.

I'm gonna install the firmware again and will report back in a few minutes
```

---
## \#4 Posted by: Eboosted Posted at: 2017-07-11T05:01:27.939Z Reads: 113

```
Hello guys, just a small update.

I was able make motor detection work after reflashing the formware again, however the the ABS overcurrent problem was still happening, so I switched the VESCs and the error followed the VESC, that confirmed the VESC (FocBox) was faulty.

I switched the bad FocBox with a new one and it worked perfectly, no more ABS over current fault.

Now I'm looking for a repair service in USA in order to ship  mu bad FocBox, I wonder if these parts have warranty
```

---
## \#5 Posted by: Jinra Posted at: 2017-07-11T06:20:29.002Z Reads: 113

```
I think @JohnnyMeduse is your guy
```

---
## \#6 Posted by: TranxFu Posted at: 2017-07-11T07:23:39.323Z Reads: 108

```
I've had a similar problem. Was working on my board and did motor detection(FOC) again. I noticed it would spit out somewhat higher values(noticeably higher) than before. When I pushed the throttle on the bench it would throw me overcorrect errors too. 

Changed the value back to before (just the Resistance value) from 0,6XXX to 0,3XXX (6374 190kv) and it ran as smoothly as before... Went for a 1hour ride without problems. Idk whats up, hope it is not a faulty focbox.
```

---
## \#7 Posted by: Eboosted Posted at: 2017-07-11T17:32:16.767Z Reads: 104

```
Can you please show me the location of this value on BLDC tool?
```

---
## \#8 Posted by: TranxFu Posted at: 2017-07-11T19:50:56.689Z Reads: 98

```
The "R" value which gets detected in the first step of FOC Setup
```

---
## \#9 Posted by: Eboosted Posted at: 2017-07-11T20:12:27.879Z Reads: 95

```
I had that issue on BLDC, still haven't tested on FOC. 

Is you Focbox holding FOC mode without issues on your setup besides you aforementioned problem?
```

---
## \#10 Posted by: TranxFu Posted at: 2017-07-11T20:24:12.295Z Reads: 94

```
Ah I see. 
Yep, pretty sure I made over 300km since I received it. No problems so far :) Running Strong.
```

---
## \#11 Posted by: Eboosted Posted at: 2017-07-11T20:27:24.337Z Reads: 93

```
Do you feel FOC is less powerful than BLDC?
```

---
## \#12 Posted by: TranxFu Posted at: 2017-07-13T15:17:17.181Z Reads: 92

```
I don't know if its just because it runs quieter but it certainly has the feeling that you lose quite a bit of power. I think top-end speed is going to suffer a bit though.

How'd you settle the issues with your faulty focboxes ? I'll check mine again. Where'd you get yours ?
```

---
## \#13 Posted by: trancejunkiexxl Posted at: 2017-07-13T15:49:22.008Z Reads: 88

```
glad you were able to find the faulty vesc.... man thats a sad feeling to have a vesc down!! thank goodness you had a backup =)
```

---
## \#14 Posted by: Eboosted Posted at: 2017-07-13T20:44:30.429Z Reads: 84

```
Thanks guys, the bad FocBox has a warraty of 60 days, that's what I've heard, I'm trying to ship the bad one as soon as possible to the vendor
```

---
## \#15 Posted by: Jebe Posted at: 2017-09-29T09:32:34.594Z Reads: 57

```
How did you go with this issue ? Did you try BLDC ? I've had this same issue and today went back to BLDC and the abs fault has gone away.
Belt cogging is back and that motor wine as well :angry:

really have fallen in love with foc.
```

---
## \#16 Posted by: Eboosted Posted at: 2017-09-29T15:08:05.904Z Reads: 55

```
The problem was a bad Focbox, it was one of the first versions with issues, it was replaced under warranty.

I switched the Focbox with a new one and problem went away. 

By the way that issue used to happen when accelerating against inclines from stand stills, when I flashed V3.29 it never happened again.
```

---
## \#17 Posted by: Jinra Posted at: 2017-09-29T15:37:52.423Z Reads: 52

```
Probably has to do with 3.29 switching back to current control instead of watt control. It may come back later when Ben releases a new version with watt control enabled again.

I fixed this issue by doubling my observer gain.
```

---
## \#18 Posted by: Jebe Posted at: 2017-09-29T22:46:07.043Z Reads: 48

```
Thanks guys. Have requested a warranty claim.
I'm still using ackmaniacs firmware 2.54
BLDC is fine just foc.
```

---
## \#19 Posted by: Eboosted Posted at: 2017-09-29T23:00:47.223Z Reads: 47

```
What VESC brand are you runing? 10S or 12S?
```

---
## \#20 Posted by: Jebe Posted at: 2017-09-29T23:02:17.543Z Reads: 46

```
enertion vescx 10s
```

---
## \#21 Posted by: Eboosted Posted at: 2017-09-29T23:17:26.144Z Reads: 46

```
You need to swap left and right VESCs and see if the over current fault follows the allegedly bad VESC, if it doesn't, the motor is shorted
```

---
## \#22 Posted by: Jebe Posted at: 2017-09-30T03:30:13.960Z Reads: 45

```
Don't believe it's the motor - it's fine in BLDC, all 3 phases measure the same, even works on one of those dinky di $70 ebay dual controllers. I will swap the master and slave over though, ordered replacements due to the 4.18's I had fail. they're due this week. If that doesn't work I'll pull my vesc 6's out of my trampa and try that.
```

---
