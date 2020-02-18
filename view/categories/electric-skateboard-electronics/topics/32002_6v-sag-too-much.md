# 6v sag too much?

### Replies: 52 Views: 2165

## \#1 Posted by: thisguyhere Posted at: 2017-09-01T05:20:36.476Z Reads: 201

```
just installed @Ackmaniac's bluetooth monitoring, this thing is awesome.

i noticed my 12s4p pack of LG HG2 cells is sagging roughly 6v under max hard acceleration.

should i be alarmed by this amount of sag?  reading other posts it seems people are seeing 4v with the 25Rs...

<img src="/uploads/db1493/original/3X/2/f/2f78fd71369faaa97dd05483fbbfedd5f7d245d9.jpg" width="690" height="415">

<img src="/uploads/db1493/original/3X/d/f/dffb2f0c05d5f39c5b755c5df0af31dfe620acd5.jpg" width="690" height="415">
```

---
## \#2 Posted by: Titoxd10001 Posted at: 2017-09-01T16:57:50.787Z Reads: 178

```
I'm not surprised by the amount of sag. I would say I see similar sag on with 25rs. Thats why I want to build a bigger pack with 18650s. I have 4p pack also but considering 5p for my next board for this reason (30qs). I would say you're cutting down range by a lot though as you might reach cutoff sooner than if you were pulling less amps. How much range you get?
```

---
## \#3 Posted by: Jinra Posted at: 2017-09-01T17:09:28.174Z Reads: 170

```
Looks pretty standard. Check the two squares I highlighted. In the first pic your at about 3.64v/cell resting. After you pull load (74A, rounding to 80A) that's about 20A/cell which gets to about 3.1-3.15v/cell at the same mAh which is about what you're seeing with 37.8v/12 = 3.15v/cell

<img src="/uploads/db1493/original/3X/a/2/a20de1d02ad997c18ae3687404640a3a63889149.png" width="690" height="397">

EDIT: I actually did the wrong color 25R, but the 25R green shows even worse sag, so you're actually getting better results than the tests!
```

---
## \#4 Posted by: MontPierre Posted at: 2017-09-01T17:14:50.885Z Reads: 152

```
Good god! I get up to 1V sag with my Li Pos and I get concerned - time to relax haha.
```

---
## \#5 Posted by: jmasta Posted at: 2017-09-01T17:23:24.815Z Reads: 153

```
Seems like a lot, but if you look at discharge charts, it is exactly what you'd expect

You're drawing about 75A, which is almost 20A/cell.  Your cells drop to 3.64V nominal voltage under this load.  Comparing the 0.2A line to the 20A line, you see a voltage drop of 0.5V/cell.  At 12s this equates to a 6.0V drop at 80A total 


<img src="/uploads/db1493/original/3X/f/8/f8b85033374f728247b61e95b63c4cece02e3b92.jpg" width="690" height="388">
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-09-01T17:26:25.755Z Reads: 141

```
[quote="Titoxd10001, post:2, topic:32002"]
you might reach cutoff sooner than if you were pulling less amps
[/quote]

ok, so let's say i have lower cutoff set at 35v in the vesc.  then let's say the pack is drained down to 37v, close to but not at cutoff yet.

at 37v, and i hit the throttle and voltage sags down to 33v, will the vesc cut out?  then come back on when voltage returns to normal?

[quote="Titoxd10001, post:2, topic:32002"]
How much range you get?
[/quote]

just redid this pack with @yummyblobs spot welder and officially finished last night.

so far drained pack down from 49.2 to 43.2v, so drained total of 6v.  out of that i got 13.9 miles so far, a mix of real-world riding and hard test riding.

that means i'm getting 2.3 miles per volt.  i have cutoff at 2.9v per cell, or 34.8v for the pack, and if the drain is linear (and i know it's not), i'm looking at 33 mile range with this pack.

when people used to ask me range and speed on my previous 10s4p build, i would just tell them "20 + 20."  now i can bump that up to "30 and 30" haha.
```

---
## \#7 Posted by: Titoxd10001 Posted at: 2017-09-01T17:44:46.370Z Reads: 123

```
The vesc won't cut out it will just reduce power. That can actually be a problem though because it won't cut power and you can still throttle very slowly under your cutoff end. It's pretty obvious you should stop though.

That's really good range I would say I only get about 16miles on 25r 12s4p pack the way I like riding.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-09-01T18:07:01.136Z Reads: 122

```
That is why I went back to Lipos. 
1v total sag with 10s/1p charging up a steep hill.
Only 0.5v total sag or less accelerating on flat ground
```

---
## \#9 Posted by: Titoxd10001 Posted at: 2017-09-01T18:09:31.489Z Reads: 119

```
Do you have ackmaniacs vesc monitor to see the numbers?
```

---
## \#10 Posted by: jmasta Posted at: 2017-09-01T18:12:24.033Z Reads: 118

```
Loved my lipos too.... for 6 months 

Now two or three of the cells have as much as 0.8V/cell voltage drop, while others only drop 0.05~0.10V/cell under the same load :cry:

(Zippy 40c 6200mAh Lipos.  If I go with lipos again, I will only buy Turnigy 60C+)
```

---
## \#11 Posted by: Namasaki Posted at: 2017-09-01T18:13:02.349Z Reads: 115

```
I have my inline volt meter mounted through the top of my deck so I can watch it realtime. 
<img src="/uploads/db1493/original/3X/1/2/12d8e9af237b3603988df30e7d544cbd54061a82.JPG" width="375" height="500">
```

---
## \#12 Posted by: Namasaki Posted at: 2017-09-01T18:17:09.565Z Reads: 110

```
I'm using Turnigy 60/120C  5000mah
They have been going strong for one year. 
No change in capacity or performance
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-09-01T18:20:53.793Z Reads: 111

```
I really should do this at some point with my 30Q 12S5P packs. 

behaviorally they seem to give you serious load support all the way up until the BMS shuts down but i'd love to see the actual numbers in action (meaning video overlays like this) without having to move to the android ecosystem. 

if anyone else has a similar config and can do so please post it.
```

---
## \#14 Posted by: thisguyhere Posted at: 2017-09-01T18:31:02.000Z Reads: 109

```
not to keep throwing money at things but there are cheapass android phones out there you could use just for this purpose?

<img src="/uploads/db1493/original/3X/9/5/9519022753a3e24ca157e0950db249a0b0c9da55.png" width="690" height="297">
```

---
## \#15 Posted by: longhairedboy Posted at: 2017-09-01T18:32:35.942Z Reads: 109

```
that's an idea.. maybe i'll just find a used phone somewhere. thanks!
```

---
## \#16 Posted by: MontPierre Posted at: 2017-09-01T18:32:42.083Z Reads: 108

```
I recommend 

http://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483?u=montpierre

Works very well on iPhone, i use it all
The time to keep an eye on the sag ;)
```

---
## \#17 Posted by: thisguyhere Posted at: 2017-09-01T18:36:34.932Z Reads: 106

```
does this record pack voltage over time?

getting telemetry is great, but scope of this discussion is sag.
```

---
## \#18 Posted by: Titoxd10001 Posted at: 2017-09-01T18:37:09.113Z Reads: 103

```
I'm more curious about your power consumption. Wh/AH there can be huge difference between riding style. For example slow cruising for me its 15 and normal riding it's 23 and going a little faster I've seen 30 wh/ah per mile so power consumption is a huge factor

How much range/miles do you get minimum or average with the lipo packs you have?
```

---
## \#19 Posted by: longhairedboy Posted at: 2017-09-01T18:45:06.553Z Reads: 103

```
i'm curious about this too because on the packs i use i get over 30 miles at what you consider normal riding speed, which is kind of fast for a lot of people. 

sag in very high discharge packs vs sag in lower discharge packs of higher overall power is a neat topic because the higher the cell count in the lower discharge packs the closer you get to being a higher discharge pack while simultaneously eliminating more sag. 

except the battery weighs 5 pounds by then.
```

---
## \#20 Posted by: Jinra Posted at: 2017-09-01T18:52:12.069Z Reads: 101

```
You can compare sag on various cells pretty easily from the real world tests here.

http://lygte-info.dk/review/batteries2012/Common18650comparator.php

Use .2a as a baseline discharge curve and compare to what you can pull (20a for example). You can check the difference to see the sag on a particular cell.
```

---
## \#21 Posted by: MontPierre Posted at: 2017-09-01T18:56:05.875Z Reads: 98

```
Yes it does record a graph of voltage of the pack, amperage and lately you can pinpoint lowest and highest voltage from the whole record to a particular point on the graph and google map.
```

---
## \#22 Posted by: Namasaki Posted at: 2017-09-01T19:02:18.831Z Reads: 93

```
[quote="Titoxd10001, post:18, topic:32002"]
How much range/miles do you get minimum or average with the lipo packs you have?
[/quote]

With my 10s 5ah pack I've gotten up to 14 miles on flat ground and up to 12 miles with big hills.
```

---
## \#23 Posted by: longhairedboy Posted at: 2017-09-01T19:08:24.135Z Reads: 90

```
That's pretty damn good for only 180 watt hours (nominal V * Ah). The original space cell was 270 watt hours and I range tested it at 15 miles and change in the 15 degree weather going moderately slow. 

That was about two years ago with the LG cells i guess. Chemistry is always getting better.
```

---
## \#24 Posted by: jmasta Posted at: 2017-09-01T19:12:52.023Z Reads: 87

```
I got around 23 miles with hills on 12S 6.2Ah lipos, averaging over 20mph

Up steep hills I averaged 18Wh/mi. But on flats with nice concrete it was only 8-10 Wh/mi.  Overall average was 12Wh/mi

Now I can trigger BMS cutoff at ~47V  (3.9V/cell "nominal").  Zippy's suck...
```

---
## \#25 Posted by: MontPierre Posted at: 2017-09-01T19:14:25.814Z Reads: 84

```
Btw - would you know what cells Raptor 2 has? They seem to be very decent in terms of range and discharge - 432 Wh :fearful:
```

---
## \#26 Posted by: Jinra Posted at: 2017-09-01T19:14:39.774Z Reads: 87

```
Samsung 30Q's
```

---
## \#27 Posted by: longhairedboy Posted at: 2017-09-01T19:43:59.116Z Reads: 88

```
yeah they have 10S4P samsung 30Q packs. So your looking at 36v @ 12Ah so roughly 432 watt hours. 

Not sure what that translates to on a Raptor but on one of my boards that would get you about 25 miles at 25mph. Ish.
```

---
## \#28 Posted by: Titoxd10001 Posted at: 2017-09-01T19:50:25.033Z Reads: 87

```
That's pretty good range namasaki and jmasta but it's difficult to compare to 18650s because there seems to be different weight listed on different sights for the lipos you guys have. Seems to be close tho

@jmasta I average 23 wh/mi on flat land
```

---
## \#29 Posted by: Namasaki Posted at: 2017-09-01T20:10:08.181Z Reads: 86

```
 [quote="longhairedboy, post:23, topic:32002"]
That's pretty damn good for only 180 watt hours (nominal V * Ah). The original space cell was 270 watt hours and I range tested it at 15 miles and change in the 15 degree weather going moderately slow.
[/quote]

The lack of voltage sag really helps mileage and so does the moderate San Diego weather. 

15F is colder than I have ever experienced. 
Unless I'm mistaken, that kind of cold can have a huge effect on lithium cells and a huge effect on mileage.
```

---
## \#30 Posted by: thisguyhere Posted at: 2017-09-02T18:02:37.315Z Reads: 79

```
Ok so my pack still has about 5 volts until cutoff, or about 10 mile range, but due to sag vesc is hitting soft and hard cutoff during heavy load. I can't feel any power cutout while riding though, not sure how or why. 

My concern is when per cell voltage goes down to 3v, let's say, and sags down to 2.4v under load, would this cause permanent damage to the cells since their charge should be kept well above 2.5v?
```

---
## \#31 Posted by: Jinra Posted at: 2017-09-02T19:00:28.495Z Reads: 79

```
when you hit cut off's you shouldn't be drawing nearly the same current, so you shouldn't be sagging as bad, just make sure your cutoff start is at a sane value like 3.0~
```

---
## \#32 Posted by: Ackmaniac Posted at: 2017-09-02T21:05:49.172Z Reads: 79

```
If your cutoff start is set to 3.0V and the cutoff end to 2.8V then the VESC will start to reduce power linear ones it reaches 3.0V.

So if you give 100% throttle and your motor max is set to 60A it will be behave like this.
100% throttle at 3.0V single cell voltage = 60A
100% throttle at 2.95V single cell voltage = 45A
100% throttle at 2.9V single cell voltage = 30A
100% throttle at 2.85 single cell voltage = 15A
100% throttle at 2.8V single cell voltage = 0A

And the VESC is extremely fast to redice the power. So when your cutoff end is at 2.8V it will very unlikely be possible to go below that. And 2.8V a cell is still relatively conservative so that you don't need to worry when you feel that the VESC reduces the power. 
You can even drain until the board barely moves and still be on the safe side.
But it is of course important that you use other cutoff start and end values for LiPos (3.5, 3.3).
```

---
## \#33 Posted by: thisguyhere Posted at: 2017-09-02T21:23:49.861Z Reads: 76

```
This is exceedingly helpful, thank you. 

I'll send you some beer money for all the work you've put into this, and your continuing support here.
```

---
## \#34 Posted by: Jinra Posted at: 2017-09-02T22:25:42.039Z Reads: 76

```
I did notice that a vesc will still run the motor at reduced speed beyond cutoff end, but this is unloaded. It'sd probably fail to drive anything loaded.
```

---
## \#35 Posted by: deucesdown Posted at: 2017-09-03T02:45:32.977Z Reads: 73

```
I'm around 200lb, I get 20-23wh on my commutes (very spirited). This is on 12s2p A123 with a variety of stuff. Carvon v2.5 dual, banggood 5065 single, jlabs 6355 dual. Amazingly consistently around 20wh/mile.

What's everyone's weight @Jinra @Titoxd10001 @jmasta?

Are the lipo guys relatively light? Or does lipo really delivery more efficient wh/mile? A123 have very good voltage sag characteristics, but not as good as lipo, I think.

And I've found it's really hard to squeeze out the last few % out of the pack. The voltage sags crazy when the pack is near depleted. But A123 kind of have weird behavior.
```

---
## \#36 Posted by: Namasaki Posted at: 2017-09-03T05:28:38.501Z Reads: 81

```
[quote="Ackmaniac, post:32, topic:32002, full:true"]
If your cutoff start is set to 3.0V and the cutoff end to 2.8V then the VESC will start to reduce power linear ones it reaches 3.0V.

So if you give 100% throttle and your motor max is set to 60A it will be behave like this.
100% throttle at 3.0V single cell voltage = 60A
100% throttle at 2.95V single cell voltage = 45A
100% throttle at 2.9V single cell voltage = 30A
100% throttle at 2.85 single cell voltage = 15A
100% throttle at 2.8V single cell voltage = 0A

And the VESC is extremely fast to redice the power. So when your cutoff end is at 2.8V it will very unlikely be possible to go below that. And 2.8V a cell is still relatively conservative so that you don't need to worry when you feel that the VESC reduces the power. 
You can even drain until the board barely moves and still be on the safe side.
But it is of course important that you use other cutoff start and end values for LiPos (3.5, 3.3).
[/quote]

The problem with this theory is that the vesc doesn't monitor single cells, it only monitors the battery as a whole.
So trusting the vesc to fully protect your battery is false security because if your cells become too unbalanced, you could wind up over discharging cells before the vesc backs off.
A BMS on the other hand, can provide full protection by monitoring individual cells or cell groups.
```

---
## \#37 Posted by: Namasaki Posted at: 2017-09-03T05:39:12.296Z Reads: 81

```
[quote="Titoxd10001, post:9, topic:32002, full:true"]
Do you have ackmaniacs vesc monitor to see the numbers?
[/quote]

I have the Metr app and module.
Here is a record of some riding I did today with some long gradual hills and some short steep hills.
Numbers recorded from just 1 of 2 Vescs.
Motors are 6374 200kv
gearing is 15/40 with 90mm wheels
https://metr.at/r/Wgq3g
```

---
## \#38 Posted by: Ackmaniac Posted at: 2017-09-03T06:58:57.022Z Reads: 75

```
Because of that I recommend to use 2.8V as cutoff end. Gives you some wiggle room. But the cell drift on li-ion cells is very little. At LiPo cells it is much worse.
```

---
## \#39 Posted by: jmasta Posted at: 2017-09-03T08:33:32.075Z Reads: 71

```
[quote="deucesdown, post:35, topic:32002, full:true"]
...
Are the lipo guys relatively light? Or does lipo really delivery more efficient wh/mile? 
...
[/quote]

Watt hours per mile is the overall efficiency of the entire system (and driver).  I'd argue battery chemistry is somewhat irrelevant to this value. It's simply how much power did you draw, for how long, and far did you travel? The VESC only knows how much power it consumed, not where it got it from
```

---
## \#40 Posted by: rich Posted at: 2017-09-03T11:57:44.616Z Reads: 67

```
Wow, after reading this thread I'm concerned about my next build with 10s4p VTC5. I didn't know that the voltage sag is so extreme with Li-Ion :fearful:. On my mountainboard with top mounted voltage meter and 10s1p 10Ah Turnigy Graphene Lipo the worst voltage sag I've ever seen was about 0.6V :grin:
```

---
## \#41 Posted by: MontPierre Posted at: 2017-09-03T12:32:19.449Z Reads: 66

```
Same here, started from Li Po's - I'm very happy with them and I wanted to move into glorified Li-ons. After reading a lot I'm considering staying with Li Pos for longer :)
```

---
## \#42 Posted by: deucesdown Posted at: 2017-09-03T15:32:20.919Z Reads: 63

```
Actually I think different chemistries waste differing amouts of energy under heavy loads. I think its related to internal resistance and voltage sag.

Personally it seems very apparent to me when my pack is nearing empty. I bet I could pull out the last 20 wh at .5C loads, but can't do it going uphill on my board.
```

---
## \#43 Posted by: Titoxd10001 Posted at: 2017-09-03T16:15:34.166Z Reads: 63

```
Your pulling very little amps. If my math is right your     at 12.87 wh/mi.

I pull 23 wh/mi average on flat land. I think how much power you consume has a lot to do with rider weight, riding style and board setup. I'm over 200lbs   and hit 30mph on my normal route. I estimate if I go slow I can get 15 wh/mi but once I go fast it can double the wh consumption. 

So if your lipo pack is 185wh/12.87=14.37mi range.
Which is close to the range you said

If I were to ride my board with your battery I would in theory get 185/23=8.04mi range

Granted with a 18650 pack you can't get the full wh because of voltage sag.
```

---
## \#44 Posted by: Namasaki Posted at: 2017-09-03T16:44:36.607Z Reads: 61

```
Agreed, going 30 mph will create a lot of wind resistance that can greatly reduce mileage even more so than weight. 
I'm currently 195 lbs which isn't far from your weight. 
However, I did not have much wind resistance riding at moderate speeds on a relatively calm day.
```

---
## \#45 Posted by: Namasaki Posted at: 2017-09-03T16:53:32.077Z Reads: 59

```
[quote="Ackmaniac, post:38, topic:32002"]
But the cell drift on li-ion cells is very little.
[/quote]

Under normal conditions the cell drift may be minor but in case something goes wrong like welds failing and separating cells in a cell group which could cause that cell group to discharge much faster than other groups. 
There have been reports of weld failures just recently. 
This is just one reason why it is so much better to use a BMS and not bypass it during discharge so that the BMS can't shut the system down if such a situation occurs.

Vesc as primary voltage control
BMS as emergency backup control
```

---
## \#46 Posted by: Ackmaniac Posted at: 2017-09-03T17:01:37.830Z Reads: 58

```
There is a much higher chance the BMS fails than that the battery fails. And when you have it included in the discharge cycle it can shut the system down during braking. And there were already many people who had issues with their BMS who did exactly that. Also people who used the BMS you sell.

So if you ask me i think they should only be used for charging. But that's personal preference.
```

---
## \#47 Posted by: Namasaki Posted at: 2017-09-03T17:21:44.745Z Reads: 60

```
[quote="Ackmaniac, post:46, topic:32002, full:true"]
There is a much higher chance the BMS fails than that the battery fails. And when you have it included in the discharge cycle it can shut the system down during braking. And there were already many people who had issues with their BMS who did exactly that. Also people who used the BMS you sell.

So if you ask me i think they should only be used for charging. But that's personal preference.
[/quote]


First allow me to make clear that I have no affiliation with Bestech and I am not in the business of selling bms's.
The few extras that I have sold, I sold only to help others and I sold them at my cost + shipping so my promoting of them is not motivated by monetary gain.

As far as them failing, I can only give my account which is that I have been using them for over a year now with no problems. Often times I have rode my brakes down steep hills with a full battery and the bms did not shut down but rather took control of the regen charging not allowing it to exceed the overcharge setting of the bms and once I stopped braking, the bms proceeded to trim the cells back down as it does during the balancing process.

Maybe I missed some posts but I have not heard of this particular bms failing lately although I have heard of the cheap bms's from eBay failing.
```

---
## \#48 Posted by: deucesdown Posted at: 2017-09-03T21:01:42.198Z Reads: 58

```
Ah I think I see it now. Speed as you say. Your top speed / avg speed are 26kph,12kph. In our backwards miles units that is 16mph,7.5mph.

I'm running 29mph top speed 13-14mph avg. Sounds like totoxd10001 is in the same ballpark.

I should try a slower ride to see if the number shift dramatically. But if feels safer in front of the cab then behind it...

Adding to the BMS conversation, my beef is that I don't know what they're doing. I'd like some kind of error indicator and a way to access individual cell voltage. I suppose we have 2 open source BMS projects going for that now.

With no BMS I'm forced to check regularly, but I feel like I'd need to do that anyway. I live in fear like lowguido and his distaste for solid state switches.
```

---
## \#49 Posted by: Titoxd10001 Posted at: 2017-09-04T09:12:55.489Z Reads: 53

```
Yes going fast reduces range by a lot. It's kind of funny that some claim you can get max efficiency by going close to top speed
```

---
## \#50 Posted by: thisguyhere Posted at: 2017-09-05T22:20:49.830Z Reads: 50

```
so at full charge (49v roughly) max sag is about 4v, usually less than 3v.  which makes sense, higher voltage, less amp draw.

so...i'll just keep the pack charged up, this should mitigate the ridiculous sag issue.
```

---
## \#51 Posted by: Jebe Posted at: 2017-09-29T09:57:29.066Z Reads: 46

```
a good bms can. A bad BMS is worse than no BMS. I try and charge to 41 volts using samsung 30q's checking voltages manually from time to time. seems fine.
edit - the bestech BMS shipped here is about 1/4 the costs of the cells. that's a big factor why I don't use them
```

---
## \#52 Posted by: Namasaki Posted at: 2017-09-29T12:33:03.482Z Reads: 44

```
[quote="Jebe, post:51, topic:32002"]
a good bms can. A bad BMS is worse than no BMS
[/quote]

This is why I try to discourage people from buying cheap bms's on eBay
```

---
