# 10s BMS help - 11 balance leads?

### Replies: 37 Views: 1053

## \#1 Posted by: ryansinatra Posted at: 2019-01-02T03:38:25.936Z Reads: 124

```
So I just received this 10s BMS in the mail from used parts sale on here. Just confused as to why there are 11 balance leads? What's the extra one for?
```

---
## \#2 Posted by: ryansinatra Posted at: 2019-01-02T03:38:40.565Z Reads: 124

```
![IMG_20190101_223643|375x500](upload://mxviXpax8PoeWITvKBYnRNhEp13.jpeg)
```

---
## \#3 Posted by: J_Dizzle Posted at: 2019-01-02T03:47:36.475Z Reads: 120

```
That is for the negative lead, aka B-
```

---
## \#4 Posted by: ryansinatra Posted at: 2019-01-02T03:48:00.447Z Reads: 120

```
Awesome thanks!
```

---
## \#5 Posted by: b264 Posted at: 2019-01-02T04:39:49.821Z Reads: 117

```
If you have ten cells in series, there are 11 connections.  Lay them all out on a desk and look.  If you connect on the negative side of each cell, then on the one end there will be a positive-end connection for B10

All relative to battery negative:

B-: 0V
B+: 42V

balance wires:
B0: 0V
B1: 4.2V
B2: 8.4V
B3: 12.6V
B4: 16.8V
B5: 21V
B6: 25.2V
B7: 29.4V
B8: 33.6V
B9: 37.8V
B10: 42V

So 0 through 10 is eleven wires
```

---
## \#6 Posted by: b264 Posted at: 2019-01-02T04:54:11.930Z Reads: 111

```
Connect battery minus before you plug that in
```

---
## \#7 Posted by: ryansinatra Posted at: 2019-01-02T04:55:47.239Z Reads: 108

```
Still learning, so thanks for the more detailed explanation. Hoping to eventually use it to wire up a battery similar to this 

https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/24

Notice how that wiring diagram only shows a balance port with 10 wires

![28%20PM|665x500](upload://sGSGXItIgWw7dXJOEbFdEe2opsc.png)
```

---
## \#8 Posted by: b264 Posted at: 2019-01-02T05:02:34.421Z Reads: 102

```
Yeah, if your BMS has the extra wire (B0) you can wire it this way and you can charge through the balance leads and just run the big fat wires to the ESC only. (Leave B- unhooked, but first verify with a multimeter that it's connected to B0)

![28%20PM|665x500](upload://urPDf7YrmP9umWLCBslanH5OQ7w.png) 

https://www.electric-skateboard.builders/t/12s5p-30qs-charge-rate/78259/23
https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/132?u=b264
```

---
## \#9 Posted by: ryansinatra Posted at: 2019-01-02T05:22:28.210Z Reads: 88

```
Those last two diagrams really clear that up! Thanks yo
```

---
## \#10 Posted by: b264 Posted at: 2019-01-02T06:15:55.355Z Reads: 83

```
@ryansinatra I edited the bypassed diagram a tad, check it again.  It's slightly more clear now.  You need to verify that internal connection exists before leaving B- unconnected on the BMS.
```

---
## \#11 Posted by: Indiangummy Posted at: 2019-01-02T07:21:27.198Z Reads: 81

```
@b264 is it standard that if the bms has a "B- or B0" Balance lead, it is intearnally connected to B-? How can you be sure they are connected. Genuine question.
```

---
## \#12 Posted by: janpom Posted at: 2019-01-02T07:49:22.521Z Reads: 75

```
Before charging through the balance leads, you should make sure the wires are rated for the charge current. For example, if you have 24 AWG balance leads, you [shouldn't use more than 3.5 amps](https://www.powerstream.com/Wire_Size.htm) for charging or you should connect the big black wire to the B-.
```

---
## \#13 Posted by: TowerCrisis Posted at: 2019-01-02T07:49:53.589Z Reads: 70

```
You can use a multimeter and check reisstance between the two. Very low resistance means it's connected.

There also shouldn't be any kind of circuitry between them, as it likely connects to a common ground.
```

---
## \#14 Posted by: b264 Posted at: 2019-01-02T07:56:52.414Z Reads: 73

```
Yes, what @TowerCrisis said and also why you should check to be sure.  Sometimes you don't even need a multimeter, you can see the copper traces connecting them if you look.  But you should use a multimeter anyway and verify zero ohms between them.

Also some BMS don't have B0 at all.
```

---
## \#15 Posted by: Indiangummy Posted at: 2019-01-02T08:06:36.684Z Reads: 72

```
thnaks for the info! im guessing a continuity test would also work?
```

---
## \#16 Posted by: ryansinatra Posted at: 2019-01-02T20:46:26.880Z Reads: 64

```
Still kind of new to all this, so I need to ask, what is this cable for? E switch install? 

![IMG_20190102_154515|666x500](upload://hVEp0tO5MGrPxnFX8iZb5XQuJmT.jpeg) ![IMG_20190102_154520|666x500](upload://8ti15Lxwu1RiVRRNnXf5Dswdd0Q.jpeg)
```

---
## \#17 Posted by: rich Posted at: 2019-01-02T20:55:54.038Z Reads: 64

```
That's the temperature sensor :grin:

If you use this BMS for discharge, too (what I recommend) then you should connect B- in any case. Discharge (-) and charge (-) goes to C- on the BMS, no connection at P-.
```

---
## \#18 Posted by: ryansinatra Posted at: 2019-01-02T21:19:28.401Z Reads: 65

```
Why do you recommend using it for discharge to rather than charge only? Just wondering
```

---
## \#19 Posted by: rich Posted at: 2019-01-02T21:29:05.270Z Reads: 64

```
Because of all the safety features like over-charge, over-discharge, over-temperature, short circuit protection for battery and charge port....

This BMS is for 60A cont. and can handle up to 110 or 120A for a short period of time. I use this BMS for discharge, too without any problems. And on my MTB I use a Bestech 50A BMS up to 100A. In the past I had a tiny BMS for charge only but I like the added safety.
```

---
## \#20 Posted by: Andy87 Posted at: 2019-01-02T21:32:38.478Z Reads: 63

```
Where you found the max characteristics?
I mean if a bms is rated for 60a, where I can find the peak current they can handle for which time?
In the specs from bestech for example it’s nowhere mentioned. Always wanted to know that. As i was never sure I also never used a bms for discharge, only a fuse where I knew which current I can draw for which time.
```

---
## \#21 Posted by: b264 Posted at: 2019-01-02T21:47:54.603Z Reads: 58

```
[quote="rich, post:17, topic:79595"]
Discharge (-) and charge (-) goes to C- on the BMS, no connection at P-.
[/quote]

Are you sure you don't have those swapped?
```

---
## \#22 Posted by: b264 Posted at: 2019-01-02T21:48:40.057Z Reads: 56

```
This is a "discharge" style high-amperage BMS best suited for discharging through.  There are pros and cons to both ways.  Neither is "better".
```

---
## \#23 Posted by: rich Posted at: 2019-01-02T21:54:57.364Z Reads: 57

```
[quote="Andy87, post:20, topic:79595"]
Where you found the max characteristics?
[/quote]

It's the over current protection, the BMS in this thread has 120A (data sheet of manufacture). So 60A cont. is no problem, the BMS would cut off at 120A +/-10A. If the total battery max of both Vescs is set to 100A together the BMS will never cut off. But of course it would get hot when pulling e.g. 90A continious. So for your 4WD it's maybe too small.

On a cheap/bad BMS the continious discharge rate is the same as over current protection (that's why I don't like Supower BMS). They claim 60A continious but in real life it's more 30-40A because the BMS cut off at 60A which is a joke IMO.

My 50A Bestech BMS is 10 times bigger than my 40A BMS which I used for charge only. Because the 50A is real and the 40A fake.

When I ordered the Bestech BMS they only had the 50A in stock so they set 110A over current protection. I had a chat with a Bestech engineer where he confirmed that like 80A for 5-10 seconds and 100A for 1-2 seconds is no problem at all, just not continious. On every ride I reach between 60-100A but only a short period of time, never had problems with heat or anything.

[quote="b264, post:21, topic:79595"]
Are you sure you don’t have those swapped?
[/quote]

As you can see on the diagram on the BMS, it's charge and discharge on the same port (C-) so it's 60A charge and discharge. I was confused in the beginning, too but had chats with manufacture who confirmed that only C- gets connected for both charge and discharge. And I have the same BMS in use connected to C- only so I'm sure.
```

---
## \#24 Posted by: ryansinatra Posted at: 2019-01-02T22:27:01.761Z Reads: 53

```
Really appreciate the helpful people that chimed in on this thread. I'm gonna have to get @Namasaki in here to help when I go to wire this BMS with lipos like the one in his famous 10s high power lipo thread.
```

---
## \#25 Posted by: b264 Posted at: 2019-01-02T23:09:10.968Z Reads: 49

```
You first need to decide whether you will discharge through the BMS or bypass it and run it charge-only.  You cannot know how to wire it until you decide that.  There are pros and cons both ways.

The BMS in [this photo](https://www.electric-skateboard.builders/t/10s-bms-help-11-balance-leads/79595/16?u=b264) is best suited to discharge through.
```

---
## \#26 Posted by: ryansinatra Posted at: 2019-01-03T00:35:19.988Z Reads: 48

```
I will probably run it for both charge and discharge then
```

---
## \#27 Posted by: rich Posted at: 2019-01-03T01:30:03.095Z Reads: 43

```
Do you plan to use 5x2s Lipos?
```

---
## \#28 Posted by: ryansinatra Posted at: 2019-01-03T01:39:45.329Z Reads: 42

```
Most likely yes. Need to take some measurements. Either that or 2x 5s
```

---
## \#29 Posted by: rich Posted at: 2019-01-03T01:58:42.815Z Reads: 48

```
Modified the diagram above to your needs for 5x2s.

![diagram_sameport|665x500](upload://sTbQOLlnWgNacbUhiecF20sJeGl.jpeg) 

2x5s would be easier but more bulky.
```

---
## \#30 Posted by: b264 Posted at: 2019-01-03T02:02:36.461Z Reads: 47

```
We need to add [fuses](https://www.mouser.com/ProductDetail/576-099707.5WXN) on the charge port negative on these diagrams

I just haven't fired up GIMP yet today

https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/132?u=b264
```

---
## \#31 Posted by: rich Posted at: 2019-01-03T02:11:43.869Z Reads: 45

```
Shouldn't the charge port be protected against short circuit anyway? I mean in both configurations, charge only and discharge/charge? Or is my brain not working? It's 3:10am here :laughing:
```

---
## \#32 Posted by: b264 Posted at: 2019-01-03T02:14:00.368Z Reads: 44

```
After [this](https://www.electric-skateboard.builders/t/that-was-a-close-call/79409/16?u=b264) and [this](https://www.electric-skateboard.builders/t/liion-fire-survivor/63042) I cannot ever recommend not using a $0.67 fuse there
```

---
## \#33 Posted by: rich Posted at: 2019-01-03T02:51:52.993Z Reads: 43

```
Damn, had to re-read the topics. @Andy87 didn't use a BMS but  @amazingdave did, that's scary. But I also read about successful shut downs of BMS after shorting the charge port. That's what I normally would assume.

![short|561x98](upload://sMYV4ni6zcjgVC4SrwfeLJXIUjM.png) 

But a fuse on charge port can't be wrong.
```

---
## \#34 Posted by: b264 Posted at: 2019-01-03T02:52:57.570Z Reads: 42

```
I actually shorted on of my charge ports once too by accident.  It's an unfused older one.  It has a BMS.  Melted the end of the pin right off.  It's still jacked-up to plug in to this day.  I was drunk at the time, too.
```

---
## \#35 Posted by: rich Posted at: 2019-01-03T02:57:44.976Z Reads: 39

```
Damn!
A charge port should be drunk-proof.

With how many amps do you charge when using 5A fuse? I guess it's not the best when charging with e.g. 4A because the fuse could get hot (just my theory).
```

---
## \#36 Posted by: ryansinatra Posted at: 2019-01-03T03:18:20.996Z Reads: 36

```
The build I'm working on currently might not have the surface area on the deck for the 5x 2s but I can always add risers to make room for 2x 5s so that's why I may end up choosing that option. We will see
```

---
## \#37 Posted by: b264 Posted at: 2019-01-03T03:59:19.474Z Reads: 37

```
I usually don't charge at 4A unless I'm out and about and need to charge.  At home it's usually 2A.  If there's 3 other boards charged and ready, no reason to stress the cells.  4A charging is why I would use the [7.5A fuses](https://www.mouser.com/ProductDetail/576-099707.5WXN) though
```

---
