# DIY 10S+ Cell Balancer

### Replies: 54 Views: 4893

## \#1 Posted by: jmasta Posted at: 2017-04-11T02:35:44.799Z Reads: 297

```
Here's a (dumb?/impractical?) idea to build your own **10S+ Cell Balance Charger** 

The system would be made from DC-DC step-down voltage regulators. You'd give it 12V input and adjust the potentiometer to your desired "balance voltage", say 3.85V (storage), 4.15V,  4.20V, or whatever

<img src="/uploads/db1493/original/3X/d/3/d32d679d9881f92a726a74b4c367d3b6bef14765.jpg" width="200" height="200">

Each cell would have it's own voltage regulator.  So, you'd need TEN of them for 10S.  _"Ten you say?!  You're crazy!"_  Well they are only about $1-2 each

So a 10S balancer would consist of 10 individual step-down voltage regulators.  Each regulator would require an isolated DC power source**.  Each 4.20V DC output would be wired in series to a JST connector, just like your battery.  The positive (+) output of module #1 would be wired to the negative (-) output of module #2, and so on...





**So tell me, why wouldn't this work?**

I feel like you'd need some way to limit the current. CC/CV step-down regulators with adjustable voltage and current can be found for only ~$1.50 a piece
.
.

** **UPDATE:**  Originally I had thought that the input for each voltage regulator could come from the same 12V power source.  However, this would not work, as pointed out below. This makes the design more complicated
```

---
## \#2 Posted by: Pedrodemio Posted at: 2017-04-11T02:59:05.505Z Reads: 261

```
It would work, but you have to use individual 12v supply to each module, otherwise you would be shorting all cells together 

In other words, each of the 12v adapters should be isolated from each other 

I remember seeing this bricks pretty cheap, so the project still would be feasible, but bulkier than a 10S charger + BMS

Maybe tearing apart each supply and arranging them in a clever way can result in a compact charger, just use caution since you'll be dealing with mains
```

---
## \#3 Posted by: lowGuido Posted at: 2017-04-11T03:36:54.992Z Reads: 252

```
I'm also pretty sure that you need more than just a buck converter to charge Lithium batteries.
Li chargers charge with a constant current until about half capacity and then constant voltage after that.

so I suppose your idea would work so long as you never go below 50% charge? not worth the risk IMHO.
```

---
## \#4 Posted by: jmasta Posted at: 2017-04-11T04:30:35.989Z Reads: 229

```
You're right, I don't think the above one would work.  This one however is CC/CV and says it will charge lithium ion batteries ($1.48/ea):

http://www.ebay.com/itm/152251963848

Unfortunately,  I think @Pedrodemio is correct, and the power supplies would need to be isolated for each module. Which makes this idea _much_ less attactive
```

---
## \#5 Posted by: Maxid Posted at: 2017-04-11T05:49:55.358Z Reads: 199

```
A step down needs higher input voltage than its output. To charge 10S you would need like 50V minimum. The better way is to use a boost converter that can use a laptop style PSU and has variable output. I did exactly that. I charge my 10S battery to 41V with a lenovo 90W 24V PSU and a DROK in a 3D printed case. Possible but cost was ~25€ not factoring in the PSU
```

---
## \#6 Posted by: jmasta Posted at: 2017-04-11T06:06:00.639Z Reads: 190

```
The whole idea was to charge each cell individually.  12V PSU to 4.2V output, for each cell.  So not 42V, but 4.2V x 10

It would be a cheap balance charger, _if_ you could find a clever way to power 10 different regulators.  Otherwise it's just a dumb idea

I have an adjustable power supply that works great. But it's not a balance charger. And my BMS sucks at balancing
```

---
## \#7 Posted by: Maxid Posted at: 2017-04-11T06:09:39.170Z Reads: 174

```
Sorry - I just read the first sentence on mobile and assumed this is going to be about a 10S charger with variable voltage output.
I am still wondering though why people want to balance so badly with all the good experience people had without a BMS and balancer on quality 18650 cells.
```

---
## \#8 Posted by: Eboosted Posted at: 2017-04-11T06:18:21.250Z Reads: 167

```
I manually balanced my packs today

<img src="/uploads/db1493/original/3X/7/1/7188d3668c43aa36392e5acfceaec5a619a06cc1.jpg" width="374" height="500">

Would be awesome to just adjust the pack voltage individually
```

---
## \#9 Posted by: jmasta Posted at: 2017-04-11T07:02:26.363Z Reads: 157

```
$25 for 10x isolated DC outputs.  Each output is 100mA at 9V. Assuming a 92% efficiency for the CC/CV step-down regulators, that's about 200mA at 4.2V (for each cell), which would be the equivalent of 42V 2A overall

http://www.ebay.com/itm/Neewer-Aluminium-Alloy-Guitar-Pedal-Power-Supply-10-Isolated-DC-Outputs/311564990374

I'm not going to go through with this project, but it actually does seem possible.  $40-50 for a 10S 2A charger that balances each cell individually.   It would be super bulky though
```

---
## \#10 Posted by: Maxid Posted at: 2017-04-11T07:34:24.562Z Reads: 152

```
I think it will not work as your grounds are different from each other. This would only work if you have independent power supplies for each step down converter "port".
```

---
## \#11 Posted by: TarzanHBK Posted at: 2017-04-11T07:35:24.337Z Reads: 143

```
Awesome idea! #Tracked :slight_smile:
```

---
## \#12 Posted by: Maxid Posted at: 2017-04-11T07:38:59.073Z Reads: 146

```
This will not work without 10 PSUs which will make it more expensive than just a 10S balance charger.
To illustrate:
<img src="/uploads/db1493/original/3X/d/6/d661dabbd10df3f41677254f40b475c712fecd42.PNG" width="664" height="500">
```

---
## \#13 Posted by: jmasta Posted at: 2017-04-11T08:18:40.941Z Reads: 139

```
Not when each PSU costs $0.99 :grinning:

The transformer should isolate the output from the input 




http://www.ebay.com/itm/172306524675?var=471125700480

So your balancer charger would be one of each of these, for each cell.   $1 for the AC to DC 9v 280mA transformer.  $1.50 for the CC/CV adjustable step-down voltage regulator.  Comes out to about $2.50 per cell. $25 for 10S / $30 for 12S

http://www.ebay.com/itm/112034265855


Now I'm just curious.  I want to try to build a 2S version with a cheap 2S battery.  (Because if 2S works,  the same concept would work for 12S)
```

---
## \#14 Posted by: TarzanHBK Posted at: 2017-04-11T08:20:26.652Z Reads: 117

```
@PXSS maybe you could tell us something about this idea?
```

---
## \#15 Posted by: Maxid Posted at: 2017-04-11T08:25:30.222Z Reads: 118

```
Well at 280mA it will take 10h to charge a normal 18650 battery.
As soon as you use a PSu with more current capabilities price will go up.

It will work this way sure, but at the cost of convenience (just think about how many cables you will have to manually connect) and it will be slow.

You could just get a 6S RC balance charger and charge the battery as two times 5S. Will be cheaper, easier and faster.
I don't see the benefit in your method.
```

---
## \#16 Posted by: jmasta Posted at: 2017-04-11T08:31:14.643Z Reads: 113

```
This would be for balancing only. I already have an adjustable voltage charger.  I just want something you'd use occasionally to trim up all the cell voltages with a single plug

* 280mA @ 9V with a 92% efficiency is 2.31W (per cell)

* 2.31W / 4.20V = 550 mA balance current per cell (while my BMS can only do 60mA)
```

---
## \#17 Posted by: jmasta Posted at: 2017-04-11T09:26:14.688Z Reads: 116

```
Here's a 20W PSU for $2.17, bringing the total to $3.65 per cell.  Ten of them gets you a  200W balance charger for $37-ish. Still pretty reasonable for 10S @ 4.7A

http://www.ebay.com/itm/10W-20W-30W-50W-100W-High-Power-LED-Driver-Power-Supply-85-265V-Constant-Current-/192014536760?var=&hash=item2cb4f55038:m:mQXiNXkA3-HwL73-Ssxy5xw
```

---
## \#18 Posted by: Maxid Posted at: 2017-04-11T09:37:00.178Z Reads: 118

```
[quote="jmasta, post:16, topic:20767, full:true"]
* 2.31W / 4.20V = 550 mA balance current per cell (while my BMS can only do 60mA)
[/quote]

You don't seem to know how balancing works. You will be in the CV stage so the current will be dynamic and go down to almost 0

I am still not convinced where the benefit is compared to getting one or two 6S RC chargers.
Why even do 10 simultaneously when you just want to do this occasionally.
```

---
## \#19 Posted by: jmasta Posted at: 2017-04-11T09:48:44.189Z Reads: 108

```
[quote="Maxid, post:18, topic:20767"]
You don't seem to know how balancing works.
[/quote]

You don't seem to know how to engage in respectful discussion.

I already have a dual 6S balance charger. That's not the point.  There's the potential to build a homemade balance charger for the same price as a standard brick charger
```

---
## \#20 Posted by: Maxid Posted at: 2017-04-11T09:57:15.507Z Reads: 111

```
I don't feel I was direspecting you. I was trying my best to keep you from burning your house down with the initial idea of using one PSU to power your step down converters.

Your answers made me honestly think you might not know (which is not a bad thing - you can always learn).
You cannot increase balancing current - that is the whole point of the CV phase.
[quote="jmasta, post:19, topic:20767, full:true"]
I already have a dual 6S balance charger. That's not the point.  There's the potential to build a homemade balance charger for the same price as a standard brick charger
[/quote]

My 6S RC charger was like 20bucks - how is this more expensive than your proposed system? Especially when you don't even want to use it for charging but only for balancing. So you'll need two systems?
```

---
## \#21 Posted by: jmasta Posted at: 2017-04-11T10:23:12.538Z Reads: 102

```
I think it makes more sense to just build a single (1S) cell charger.  So for example, bulk charge to an average cell voltage of 4.10V. Some cells will be 4.13V, while others might be 4.07V.  Individually charge them all to 4.15V.  This would manually balance the pack. You'd only need to do this occasionally. Often the pack will stay nearly perfectly balanced with no maintenance

The problem I have is my BMS doesn't seem to balance very well.   Some cells consistently lag behind 0.05V at EOC
```

---
## \#22 Posted by: Nordle Posted at: 2017-04-11T10:31:14.584Z Reads: 96

```
0,05V apart is well enough...
```

---
## \#23 Posted by: Maxid Posted at: 2017-04-11T10:31:35.809Z Reads: 94

```
0.05V is not worth talking about. This is probably already in the range of the measurement error of your voltmeter.
```

---
## \#24 Posted by: TarzanHBK Posted at: 2017-04-11T10:39:51.702Z Reads: 93

```
the cool thing about this would be to simply choose how much cells you want, so a modular charging system, where you could charge your 6s board aswell as your 10s, without using a bms!
To me that sounds really cool!
Also cool for people with things like 9s Boards, where you normally have to use two rc chargers..
```

---
## \#25 Posted by: Maxid Posted at: 2017-04-11T10:46:39.153Z Reads: 96

```
[quote="TarzanHBK, post:24, topic:20767, full:true"]
where you normally have to use two rc chargers..
[/quote]

I don't understand you guys. how is having ten chargers better than one that you need to hook up twice but ultimately takes less time? There are even wiring diagrams out there on how to split a >6S battery to charge it in parallel.
This proposed mechanism (if you go for multiple cells at a time and not just one) will be a wiring mess, complicated to connect and can do more harm than good.
[quote="TarzanHBK, post:24, topic:20767, full:true"]
the cool thing about this would be to simply choose how much cells you want, so a modular charging system, where you could charge your 6s board aswell as your 10s, without using a bms!
[/quote]
this can be easily achieved like I explained above with a simple boost converter - no explicit balancing but you can keep it hooked up until it reaches your desired current in the CV phase.
```

---
## \#26 Posted by: TarzanHBK Posted at: 2017-04-11T10:57:42.012Z Reads: 98

```
You build this thing by your own and throw everything in a cool housing, then you only have one cable with a few phases out. Different cables with different phases for different boards like 6s or 10s.
Hook it in the wall, hook it to your battery and you´re done. No BMS, no worries to overload your battery. Sounds cool to me :slight_smile:
```

---
## \#27 Posted by: Pedrodemio Posted at: 2017-04-11T11:00:53.311Z Reads: 99

```
@jmasta use this, TP4056 modules, they are limited to 1A max, but work quite well and are very cheap, now you only need 10 USB wall adapter, again, isolated with one USB each

 
Look what I found on AliExpress
http://s.aliexpress.com/VBJNnyea
```

---
## \#28 Posted by: Maxid Posted at: 2017-04-11T12:06:20.323Z Reads: 101

```
https://media.giphy.com/media/l2Je4zlfxF6z0IWZi/giphy.gif

;)

@Pedrodemio poblem with those is that you can't adjust the voltage.
```

---
## \#29 Posted by: Pedrodemio Posted at: 2017-04-11T12:45:13.349Z Reads: 99

```
Yeah, that would need a bit of tinkering, but is doable
```

---
## \#30 Posted by: jmasta Posted at: 2017-04-11T18:23:06.837Z Reads: 100

```



[quote="Maxid, post:23, topic:20767"]
0.05V is not worth talking about.
[/quote]

0.05V is not a huge deal.  0.50V is a different story

If you have a welded pack and you find one cell group very out of balance...  What do you do?  Your BMS won't take care of it if the voltage difference is significant.  I have a 0.05V difference now.  What happens when that grows to 0.10V?

The following scenario resulted in permanent cell damage

[quote="Eboosted, post:121, topic:19302"]
I went for a long ridde tonight anfd I ran my board with my unbalanced pack until it reached cutoff start voltage which is 30V

Before the ride, this were the voltages of each pack:

1) 4.16
2) 4.10 
3) 4.09 
4) 4.16 
**5) 3.75** 
6) 4.08 
7) 4.12
 8) 4.16 
9) 4.10
**10) 4.18**
[/quote]








[quote="Maxid, post:15, topic:20767"]
I don't see the benefit in your method.
[/quote]



Tell me why it won't work. Provide suggestions if you are so inclined.  Not to be rude, but whether or not you see a use for the technology irrelevant.  The need exists


[quote="Maxid, post:25, topic:20767, full:true"]
this can be easily achieved like I explained above with a simple boost converter - no explicit balancing....
[/quote]

We already have that.  This thread is about balance charging individual cells simultaneously
```

---
## \#31 Posted by: Maxid Posted at: 2017-04-11T18:46:19.525Z Reads: 92

```
I don't know what to say. I told you multiple times that it will not be that easy (just think about how many power outlets you'll need for 10 separate USB chargers). One RC charger does what you want - and is easier to use, faster and cheaper.
There is no need for this because the solution already exists.

You need to start thinking what the benefit of your method will be.

Just as an example: I already have my battery set up as two 5S packs that I can charge individually on an 6S charger. This way I can test the individual voltages from time to time. Normally I charge with my DROK. This is as easy and cheap as it can get and I have full control over the voltages I charge my battery to.
```

---
## \#32 Posted by: Nordle Posted at: 2017-04-11T19:06:52.172Z Reads: 86

```
[quote="jmasta, post:1, topic:20767"]
Here's a (dumb?/impractical?) idea
[/quote]

yes, both...

_if you absolutely have to buy something from aliexpress just get a BMS there_
```

---
## \#34 Posted by: Pedrodemio Posted at: 2017-04-11T20:37:58.347Z Reads: 85

```
If the goal is to be cheaper I agree with both of you

But building a charger this way could be a fun project
```

---
## \#35 Posted by: SimosMCmuffin Posted at: 2017-04-11T21:18:09.498Z Reads: 91

```
As an electronics engineer, there's a lot.... _interesting_ ideas presented here. Surely out of the box ideas for me, but how sensible? Not so much. 

The easiest and best practical way would be to wire your S>6 pack so that it can be charged as two S<=6 packs and use RC chargers as @Maxid suggested. Otherwise you're going to be babysitting your battery pack and checking cell voltages and adjusting your charging currents and voltages. A RC charger will lower the charge current once a cell hits 4.2 V and then trickle charge the rest of the way while discharging the 4.2 V cells so they don't overcharge.

Other possibility is the @raphaelchang 's BattMan BMS module.
```

---
## \#36 Posted by: PXSS Posted at: 2017-04-11T23:34:47.187Z Reads: 89

```
I've been out of town @TarzanHBK
Will read through the thread when I get a chance.
```

---
## \#37 Posted by: lowGuido Posted at: 2017-04-12T12:34:47.167Z Reads: 87

```
[quote="Maxid, post:18, topic:20767"]
I am still not convinced where the benefit is compared to getting one or two 6S RC chargers.
[/quote]

 This^
-----
```

---
## \#38 Posted by: PXSS Posted at: 2017-04-12T22:36:24.008Z Reads: 90

```
[quote="Maxid, post:7, topic:20767"]
I am still wondering though why people want to balance so badly with all the good experience people had without a BMS and balancer on quality 18650 cells.
[/quote]

It pretty much comes down to these reasons:
Not everyone uses quality cells.
Not everyone uses quality welders.
Not everyone has good soldering/welding skills.

Any of the above plus not having a BMS will ruin your batteries.
As an example @denton had a battery pack in which welds failed and he was also using a charger with way too high voltage, but since he was using a BMS to charge and discharge no damage was ever done to his batteries.
```

---
## \#39 Posted by: Maxid Posted at: 2017-04-12T22:43:18.639Z Reads: 82

```
Someone with a wrong charge voltage is kind of unfair to use though as an argument no? ;)
It is not hard to make a setup without a BMS work well, so I still feel like they are not really necessary.
```

---
## \#40 Posted by: PXSS Posted at: 2017-04-12T22:45:04.716Z Reads: 90

```
His charger was not the reason his cells were out of balance, it was the bad welding tabs. Still a valid argument. Look at eboosted and all the trouble he's having with drifting cells.

It's not trivial....
One, you have to buy or make a quality welder.
If you are soldering, you have to have good soldering skills and even then by the fact that you're soldering onto batteries, you will damage them some.
Two, you have to buy quality cells.
Three, you have to have very conservative settings. Have you looked at whitepony's settings? He only uses like 70% of the available capacity in his cells and doesn't discharge them at high currents either.
Four, if vibrations work a weld/solder joint off a cell, your pack is F'd. (this is where my example came into play really)

There are plenty of reasons to use a BMS. If you prefer to baby your pack instead then fine, I do it that way just because I like to know the state of my batteries all the time.
```

---
## \#41 Posted by: Maxid Posted at: 2017-04-12T22:50:09.443Z Reads: 96

```
Not sure what to say - as usual I get your point but am personally not convinced that a BMS is crucial. Put some balance leads on the pack and check from time to time and it should work fine. I used a DIY welder and have no problems with my packs.
People with faulty packs will obviously benefit from a BMS but I'd rather pay attention when building my pack in the first place and make sure everything is well.

All I am saying is that when you know what you are doing they are not crucial.
```

---
## \#42 Posted by: PXSS Posted at: 2017-04-12T22:53:46.956Z Reads: 94

```
[quote="Maxid, post:41, topic:20767"]
All I am saying is that when you know what you are doing they are not crucial.
[/quote]

When you know what you're doing, want to be conservative and prefer to do the monitoring yourself, yes. They are not crucial. For everyone else, it kinda is.
```

---
## \#43 Posted by: Pedrodemio Posted at: 2017-04-13T04:09:52.644Z Reads: 99

```
You can't use without BMS because or you buy a board that is a BMS or you become the BMS 🙃
```

---
## \#44 Posted by: Quezacotl Posted at: 2017-10-25T13:55:54.873Z Reads: 90

```
I have made the same idea disgussed here.
It consists from 10 of TP4056-modules, 10 of 1A/5V power supplies and 7-segment voltage-meters.
It is able to charge at 1Ah rate. Usually it took about 5h to charge after riding. It has been good enough for me.

Then i attempted to charge simultaneously with 42V/2A charger, and about 3 of the modules died. I don't know if the 42V charger was the cause or something else. If you think about it, what could be the thing that would kill those modules if it was the 42V charger?

Anyways, it was pain to troubleshoot and repair because of the design i made. I broke it all to pieces except the voltage meters.
Nowadays i'm just charging with only the 42V charger and voltage displays attached, so i see when any of the cells reach the 4,2V. Usually all the rest are about 0,1V-0,15V lower that the best.

I stumbled upon to this thread when i was searching info about those lm2596-modules. The TP4056 is not adjustable, so they can't really be used on separate charger if you want to auto-cut the voltage when full, because the wires make additional resistance. lm2596 can be adjusted, though it will not cut the charge, but it is still better, because it heats less.

<img src="/uploads/db1493/original/3X/6/3/63e85193bf92168dbe82064d34b54153378d5476.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/f/9/f9923c95044808d742cbb7aedd61a1342f06c7e8.jpg" width="375" height="500">

I'm actually moving to "normal" balance-charger now. A FET per cell loses the excess current into heat while series charging. But that's out of this topic.
But i'll try the lm2596-modules as parallel-project though :slight_smile: 

<img src="/uploads/db1493/original/3X/0/6/063c175ad4158b23eef423da58b631cc1d3d3a2d.png" width="690" height="378">
<img src="/uploads/db1493/original/3X/1/4/14186a33583c52e0330d9e51ee220084fe2b239d.png" width="690" height="378">
```

---
## \#45 Posted by: Okami Posted at: 2017-10-25T14:51:43.491Z Reads: 84

```
Well.. that is some in-depth info you got there.. 

On a side note.. I also witnessed that TP4056 overcharges the cell, if left for loo long.. so yeh, either manual cut-out or a circuit is needed... otherwise they dont seem very reliable when in parallel config
```

---
## \#46 Posted by: deucesdown Posted at: 2017-10-25T17:16:21.550Z Reads: 85

```
epic necro post, nice!

Read the whole thread, and my thoughts:

- the ultimate charging method is to cc/cv charge 1 cell with 1 charger. so @jmasta is going toward the one-true-path, not away from it.

- cc/cv power supplies are different from charging circuits in that they do not have termination. The lithium ion charging profile is to hold constant current until termination voltage is reached, then hold the voltage constant until the current hits some minimum threshold (C/10 or C/20 usually). So cc/cv PSU will get you close but is not following charging protocol, and you'll terminate at different states of charge on each cell.

- if you use cc/cv psu, you're gonna need a voltmeter per cell to tell you when to pull the plug.

- those $1-2 electronics boards, I believe most of them overstate their capabilities. You need to burn-in test a bunch of them, and run them way under max spec, or add active cooling.

- many lithium ion charging ICs don't behave correctly. I thought TP4056 was okay though...

- BMS has very limited balancing capabilities, and termination is not adjustable (are there exceptions?) so if you want to charge to 4.1v/cell to extend cycle life, balancing never kicks in

- hobby chargers have better balancing capabilities but is also limited. so individual 1s chargers will actually finish faster.

- failed BMSes seem to be a fairly frequent killer of packs? I feel you need to babysit the cells whether you use BMS or not.

I think this application makes the most sense for people who are running without BMS, to periodically check on the pack. It's not so horrible to break the 6s series connection and balance charge each subpack once a month, but I think this thread's premise is worth considering.
```

---
## \#47 Posted by: jmasta Posted at: 2017-10-25T21:49:11.207Z Reads: 78

```
@Quezacotl I've got to say, well done!  That thing is awesome! :clap:

It's cool to see that the idea is indeed feasible. Sounds like there might be a few bugs to work out, but what you built is basically exactly what I had in mind, even though we came up with the idea independently   

I kept brainstorming this project a bit after posting but never updated the thread.  I will post the schematics when I have more time.  I'd love to see this progress further


---
----------

Great points, @deucesdown! 


[quote="deucesdown, post:46, topic:20767"]
It's not so horrible to break the 6s series connection and balance charge each subpack once a month, but I think this thread's premise is worth considering.
[/quote]

This is basically what I am doing.  I have a SuPower BMS and also an adjustable 12S charger.  I almost always do a partial charge, which means the BMS balancing never actually kicks in (since it starts at 4.15V/cell).  Despite not balancing each charge, the pack stayed very well in balance after probably 50 or more partial charges.  My board has a built-in 12S cell voltage checker with a switch, so I can easily monitor individual voltages of all 12 cells.  Occasionally I break the battery down into 6S "subpacks" and give them a proper balance with a hobby charger on the slowest balance setting.  Currently I am using 4x 3S Lipos but will be replacing that with 2x 6S li-ion packs in series, so that I can still use the hobby charger for balancing or discharging if needed.

_Side note:_  Even if you don't use the BMS for balancing all the time, I still think they are very important to include in your design.  It's the only way to get cell-level voltage protection for over-discharge and over-charge; I see so many people using a bypassed BMS, which means you are losing most of the BMS's safety features.  Also, having some form of over-current protection is a must (in other words, if you bypass your BMS or don't have one at all, you really should have a fuse in your system!)
```

---
## \#48 Posted by: deucesdown Posted at: 2017-10-26T01:21:57.512Z Reads: 70

```
[quote="jmasta, post:47, topic:20767"]
Also, having some form of over-current protection is a must (in other words, if you bypass your BMS or don't have one at all, you really should have a fuse in your system!)
[/quote]

This is something I'm struggling with too. vesc will progressively reduce power, but bms is BAM off, and throw you to the ground. the fuse I agree with, but struggle with how many and what level.

I'm similarly paranoid about e-switches, I think @lowGuido ruined me.
```

---
## \#49 Posted by: lowGuido Posted at: 2017-10-26T02:24:21.800Z Reads: 65

```
You should be. I mean this is your life that you are playing with.
```

---
## \#50 Posted by: PXSS Posted at: 2017-10-26T02:37:00.477Z Reads: 62

```
Your BMS cutoff should be lower than your esc cutoff. That is what makes it a secondary safety. The fuse is the last resort. 

Cutoff order:
ESC - linear drop in power till halt. 
BMS - hard cutoff as to not damage battery
Fuse - hard cutoff in case all else failed
```

---
## \#51 Posted by: PXSS Posted at: 2017-10-26T02:56:22.696Z Reads: 69

```
[quote="deucesdown, post:46, topic:20767"]
BMS has very limited balancing capabilities, and termination is not adjustable (are there exceptions?) so if you want to charge to 4.1v/cell to extend cycle life, balancing never kicks in
[/quote]

Limited balancing capabilities:
Definitely but if your cells are more than 50mV out of balance after a single cycle there is something very srong with your battery. 

I build batteries and power systems for unmanned aircraft and have never seen one of my packs even with up to 13 cells in parallel go out of balance more than 5mV. As long as you use quality cells from the same production batch to build a pack, you'll rarely have balancing issues with a BMS that can do 100mA.

The problem arises with poorly manufactured packs where you are relying on the BMS to mask a greater issue. 

Termination is not adjustable:
Negative sir. Quality BMS with comms have adjustable limits. If you choose to go with a cheap BMS then they will more than likely have an analog balancing scheme which can be adjusted by changing certain components. Bestech BMS come with several configurations that you can choose from. If you want a real BMS, TI has reference designs but they are usually $300-400 for evaluation modules. 

Either way, limits are adjustable. My BMS starts balancinng at 4V/cell and cuts off at 2.5V per cell. I requested it this way from Bestech , I think I paid $50 for it. 

My supower BMS kicks in at 4.1V and has a lower limit of 2.9V. This is meant more for a Lipo pack as they dont go below 3v/cell. 

---
Again, the BMS is not supposed to be the main protection, but a redundancy in case the ESC fails
```

---
## \#52 Posted by: Fatos Posted at: 2017-10-26T21:24:29.016Z Reads: 63

```
There are just so many S. ideas in this thread that I keep wondering maby this one of the reasons why Li-ion  has got the reputation of being dangerous.

Please people, for your own sake and the people around stick by the book. This batteries can become dangerous, if not treated properly. And remember when you see a board burning that next time it can be yours. 

Let Tesla, Samsung, Panasonic do the testing of methods. When they say that you don't need BMS, and balancing than you can start with that. Until then try to stick to the working solutions. That are proved and tested in many years.

Rules : 
1) Get a quality BMS  
2) Make good welds
3)Use same batteries, from same batch if possible, at same voltage.
4)Connect balancing leads. Don't start balancing just yet.
5)Good connectors all the way, don't cheap out on that
6)isolate the cells from each other,
7) Do at least 2 charges and discharge in bench. Check voltage drift from balancing leads time after time. This will tell you if your pack is properly welded. 
8)Shrink wrapping after you found out that everything is OK.
9)Connects balancing leads and do one or 2 discharge and check again.
10) After a week of use one more check.
11) And do some checks time after time.
Remember those pack are put to real stress all the time. Vibration, high current discharge,  high current charge at reg breaking. So at least try to improve there where you can.
```

---
## \#53 Posted by: jmasta Posted at: 2017-10-26T22:26:11.255Z Reads: 58

```
I have a non-bypassed BMS, system fuse, charge fuse, and my batteries are permanently housed in "fire-resistant" bags.  I have built-in cell voltage monitors for all 12 cells. And I have a log book of every cell voltage for almost all of my discharge cycles

This idea was never meant to replace a BMS.   Cell level charging has the potential to be safer than bulk charging.   So don't rag on someone for having a new idea :kissing_heart:
```

---
## \#54 Posted by: Fatos Posted at: 2017-10-27T05:44:02.731Z Reads: 67

```
It was not directed to you. It was more general..It's not you asking that is the problem, because people who ask and discuss rearly make mistakes. But what grind my gears is people deciding that you should do things  this or that way. Because it worked for them just fine, for 2-3 months. And that is just not enough testing. 
So I didn't mean to offend neither you or anyone else. Just trying to raise the awareness a bit, because I feel that not everyone has understood that Li-ion should be treated with respect.
```

---
## \#55 Posted by: deucesdown Posted at: 2017-10-27T14:32:57.127Z Reads: 64

```
OMG sorry for the wall of text lol

Generally I agree with you and appreciate you taking the time to type out the recipe.

But if you're playing with lithium ion, precisely because they're capable of so much mayhem, really I think one would be much better off considering how things work and how things break, rather than blindly following rote advice, especially if they don't have the background to read between the lines, or the skills/knowledge/equipment to execute.

And there's always room to improve, like all the cell level fusing discussion. Without critical thinking and discussion we'd just stay where we are. And while we can learn from industries with established standards, many of these standards are difficult or impossible or too expensive to apply to our hobby.

There's also tons of grey area, I'm gonna rattle some off that I'm still trying to resolve in my head (I'm not looking for responses, just raising things I've been trying to learn about)

Are nickel strips good enough for series connections (I think no for typical 2x6355 and up), and is it okay just to do the series connections at the end of a parallel group (not ideal).

What is adequate mechanical support -- puncture resistance, water survivability, friction rub-through of insulation, embrittlement of solder joints through movement, is hot glue flammable and does that matter.

What is adequate cell isolation (kapton tape? fish paper? cell holders?) Is it worth it to leave room for ventilation/cooling between cells.

Is cell level fusing worth the trouble -- I think we're pretty close but haven't quite figured out proper implementation for eskate (do the fuse wires drop voltage, is it significant, how to acquire proper fuse wire, how to protect from vibration, how to detect broken fuse wires).

How much current can silicone wire really carry (ampacity of copper doesn't really change, I believe the super high amp ratings of silicone wire is solely due to the 200deg rating of the insulator, and 200deg is TOO HOT inside our enclosures and next to our batteries).

Bottom balancing and bulk charging vs top balancing via bms.

If using BMS, how to detect failures (broken balance leads, fried components). I think like @jmasta, per cell voltmeter of some sort is the only way I'd feel comfortable.

Crimped vs soldered wire splices (crimp is the winner, but need proper equipment/technique)

Corrosion of contacts -- charger ports and balance wires

After seeing @Eboosted board fire (sorry dude!), quick disconnect (loop key) and quick release enclosure and battery mount seem worth thinking about.

I think the e-switch situation sucks -- $50 is expensive for a switch, and the $50 ones blow up (in "ON" position) on high powered boards. Mechanical switches also suck, with DC arcing problems above like 6s. Anti-spark loop key also sucks, you have exposed contacts when turned off, the contacts wear with cycles, and you can lose the key. BMS integrated e-switch seems like a good idea except for all the BMS's blowing up, and [crashes like these](http://www.electric-skateboard.builders/t/ate-shit-today-and-loop-keys/33613) (looks like e-switch failed and bms cut off power, sorry Joe!). There are some high cycle circuit breaker switches for marine, that look like they might work? But bulky and expensive.
```

---
