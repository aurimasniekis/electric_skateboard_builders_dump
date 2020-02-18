# Which cells? IMR25? 25 or 30C?

### Replies: 38 Views: 3327

## \#1 Posted by: Fin420 Posted at: 2017-01-13T22:11:01.850Z Reads: 193

```
I'm about to build my own battery pack,  can anyone give me some advice as to which cells to buy?

 I'm going to build a 10s2p or maybe 3p if I have space, with no bms. 

I'm in the uk so probably going to buy them from http://ukvapers.org/attachment.php?aid=55352

But which ones are the best for eboards? I hear everyone talking about Samsung 25r's, is this the same as the IMR's? 

which C rating, and also which capacity is best? My understanding is that to an extent the higher the capacity, the lower the C rating.

 Also would anyone recommend a good place to buy them?
```

---
## \#2 Posted by: Okami Posted at: 2017-01-13T22:42:51.236Z Reads: 185

```
I will answer just to bring this topic further.. I believe a 10s 3p pack might be better from the discharge perspective and the longevity of the pack (also increased capacity - mileage for your board!

Your assumtion about higher capacity and lower discharge rate is true. Usually cells with over 3ah per cell have less discharge capability. 

Im not sure which cells would be the best. You need to find the sweet spot between price / capacity / dicharge rate.. but for that you also need to know what **discharge rate** you would like to have!

With discharge rate I mean continous amps per cell, it looks like most cells are at 20A or so, usually the ones which are over 3ah have it at 10-15A or so. 

So for a 2-3P pack, 15A per cell might be the minimum but some ppl can argue with that. 

I'd recommend just sticking with 25R or similar and trying to build 3s pack, this way you should have enough discharge (theoretically 60A) and also quite ok capacity.. ~7ah.

If you are willing to try and dont want the fastest board, you might choose cells with 15A discharge, though, if you pull 20-30A constant (have hills) it might be better off using 20A cells.
--
To be honest, there is a lot of contradiction how much power / watts an eboard need! It is also not entirely clear at which point cells do get damaged / harmed by pushing them too hard! So far it is known that it's not a wise idea to pull the max available amps from the cells all the time.. especially if they heat up, as heat kills the internal structure / chemical composition of the cells..
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-01-13T23:13:53.497Z Reads: 163

```
Get these ones from here. Nice price and it can be used as a 20A cell

https://eu.nkon.nl/samsung-inr-18650-30q-3000mah.html
```

---
## \#4 Posted by: Fin420 Posted at: 2017-01-14T16:07:04.081Z Reads: 164

```
@Okami Thanks! Why would a 3p rather than 2p be better from a discharge & longvity perspective?

I was going to build a couple of 10s2p packs so I could swap them out when one dies for extended range, (I'm using a loaded vanguard deck so taking flex into account I don't have a huge amount of space)

I know the current draw will vary as the load on the motor changes, but how do you calculate the maximum current your motor setup is capable of drawing?  Is this something you can limit using a vesc? I just don't want to go to the trouble of welding a battery pack together only to attach it to a propulsion system capable of damaging it by drawing too high a current..

I know the short answer to this is to use a bms chip...but there's a few reasons I don't want to use one, most of which this video agrees with https://m.youtube.com/watch?list=PLLeRyW109a4rqxsHaVMXyAuDB02lJX8s0&v=pljSZcEwc8Q
```

---
## \#5 Posted by: flatsp0t Posted at: 2017-01-14T16:34:16.942Z Reads: 159

```
There are some threads about this, maybe you are able to find some additional Info here:
http://www.electric-skateboard.builders/t/choosing-18650-cells/6240
http://www.electric-skateboard.builders/t/li-ion-18650-battery-comparison/11015

The correct Samsung cells are Samsung INR18650-25R

BTW.: I never heard of any of the battery manufacturers the shop you have linked has in stock. I would not buy there.
```

---
## \#6 Posted by: Okami Posted at: 2017-01-14T22:25:57.463Z Reads: 140

```
[quote="Fin420, post:4, topic:16056"]
I know the current draw will vary as the load on the motor changes, but how do you calculate the maximum current your motor setup is capable of drawing? **Is this something you can limit using a vesc?**
[/quote]

Actually you bring up a good point!

 I think @Ackmaniac could try to answer this one, im not sure how busy is he, but me personally, have very limited (almost non at all) experience with vesc, so I wont be able to tell how good these battery / motor limits work (and their relation to each other!)

In short, for longevity purposes, it might be the best to discharge the cells at 1/2 or 2/3 of their maximum rating. At least, this is what I personally came up with from reading a lot of info concerning batteries. 

For the type im using, it turns out, if they are discharged at 20A+ constant, they get really really hot (something like close 80degrees celsius (~176F), such a temperature is bad for the cells in the long term and they just may not perform the same in the long run, if they are regularly pushed to such limit and held there.. 

Anyways, there is a big science behind all of this.. and unless ppl are able to measure and monitor each of these parameters at every ride / often etc.. then what is usually choosen, is just to choose a more ''conservative'' approach and dont ''push the limits'' but take it more safely (like picking up batteries with more ''buffer zone'' in terms of max discharge instead of discharging cells at their maximum parameters most of the time)

----

 Anyways, if you take a cell with 20A and make a pack with 2 in parallel fo each serial group (10S2P) you might be ok, as the regular usage might be in the 10-20A range, depending on  how fast you wanna go, how big wheels you have, how heavy are you and will you have any hills in your road.. 

Hills are probably the biggest challenge for batteries / motor, I dont have much experience with hills and battery performance personally, but perhaps, @evoheyax can also step in and **share his ''story'' about battery amps and hills.**. 

He does seem to ride quite extreme and I believe he has a 4wd setup now but perhaps he can point out some valuable info related to what you are dealing with here.. 

----

Ppl always recommend to take more ''safe approach'', so in this situation 3P instead of 2P (also depending on cells) might be the ''safer approach''. 

This is because with 3P, you would increase your battery's discharge rate by 1/3, You can compare this, perhaps, to a regular car or motorcycle.. Either you have 40hp available (1P), 80hp (2P) or 120hp (3P).. 

If you have to ride at max the motor can output (40hp) it will be a lot harder for the motor, (in 1P config) than if you ran it at 1/3 of its max performance (with 3P), with a 120hp ''reseve - resource'' total.

I hope you somehow understand the concept about the battery technology and their characteristics/performance from this. 

Anyways, some ppl might add to this or tell a different opinion, since this is basically from what I read and also a bit of little experience I have so far, im still learning (also by writing all this info out).. 

So there still might be things I have not included or dont know about.. though, I researched li-ion batteries for about 2months at least, so I have picked a few things and ideas along the road.. :) + little things I've done with electronics before that

---

Will try to be short in adding a few more things.

Basically, for choosing battery, you could take the max your motor can take, usually this rating is mentioned something (in terms of amps or watts) and then you can calculate what battery config (how many in parallel and what cells) you need, to be able to meet this criteria!

That's basically how I did it - my motor is able to output about 2500w / 75A (numbers are approx), so I chose a battery which is able to output 80A max. 

So far I've reached ~50A with half the voltage motor can take. This means, that instead of theoretical 2500w, I achieved more like 1250W, but the motor still had 50A draw. 

50A is peak(max) value, it might have been only for a short moment but sometimes to get upto that hill etc I think you might need these ''bursts'' of power. 

---

There are some commercial boards which batteries are nowhere as big / powerful as some ppl use here in the forum but they still get away with that! It usually just might mean that their max speed or available power wont be as high, as it could be but these boards will still be able to move forward - just not as fast or aggresive as it could be + there's always a question how hard it might be for the batteries to operate in such conditions..

So I think you should really find out is it possible to limit max current the vesc takes from the battery.. this way you could limit it and make it ''safe'' for the battery.. but that also widely depends on what you riding conditions might be.. 

---
I still need to test it out how it is to ride with a ''weak'' battery, in terms of max discharge.. 

For now, I just now that if the battery i really depleted, it is not possible to go really fast! 

This is also something that happens - if you discharge battery at higher rate, its capacity may also might be a lot smaller than ''shown on the label''.. For example, for that same 2500mah battery, if you discharge it at max rate, it might not give you all 2500mah, but only 2300mah or even less. This ''actual capacity'' is battery type depending, so you would need to check battery's datasheet to figure out how much each battery outputs (its capacity) at what discharge rate (either 2A, 5A or 10A).

---

Ok, so that's probably a lot of stuff to consider.. I hope I have given you some more info to think about, since you will probably be riding that board for quite a while.. unless you decide to sell it at later point.. so yeah, battery choice might be important, as it costs quite a bit (perhaps almost the most expensive part for single drive setup),

--

If some info seems off-topic or not so relevant, please say so @Fin420

You can try to check some ''vesc logs'' or ''vesc monitor app'' videos and look at Amperes section, it will also depend on gearing ratio, wheels, terrain (wind, road etc) and other things but in general you should be able to see the ''average numbers'' you might be dealing with.

 Try to look up a video where someone has 10S, as 12S might get a bit less amp draw.. 
--

Sorry for not giving a direct answer to this.. your best bet might be really to research and decide on your own.. same as I did.. I did choose higher discharge rate at a sacrifice of less capacity.. 

So im not entirely sure, did I choose longevity over short-term gain (longer distance vs longer battery life) or not.. It might be (in some cases) it is better to choose higher capacity, live with less power but longer travel distance and also shorter lifespan of battery (decreased capacity).

---

[quote="Fin420, post:4, topic:16056"]
I just don't want to go to the trouble of welding a battery pack together only to attach it to a propulsion system capable of damaging it by drawing too high a current..
[/quote]

Im not sure can you ''damage it'' right away.. It would depend on how you use it.. I think if you dont choose a too low specs (low discharge) for your batteries, so that they indeed would need to be at their max all the time, you can not ''permanently'' damage them that fast.

You would have to look for ''voltage drop'' though, and you might get less performance out of them - they would ''die'' a lot faster than they should because they would get a bit ''stressed'' by pulling a lot of current from them all the time.. 

Though, it looks like some setups of eboards use only about 5-10A constant, at 10S, this would be about 300-400w of power, probably. So unless you choose 5-10A cells, I think you will be good.
```

---
## \#7 Posted by: Ackmaniac Posted at: 2017-01-15T00:34:41.213Z Reads: 103

```
In my next app version a lot of these questions could be answered. You will see the average amp draw during your ride. And this even in total and in ride time.
Total = it counts it also when the board is not moving. Useful when you want get a feeling how the amps raise the Batterys temperature.
ride time = it only counts when the board is moving. Useful to know how much amps you draw in average when you are riding.

I hope that this will be a eye opener so that the people can see that it is no issue to allow max current draw from the cells because we never use it constantly at this high level. So if the battery is rated to 20 amps a cell you can allow a maximum amp draw of 20 amps. The battery's wont heat up to 80 degrees. Because that only happens when you really would draw these amps constantly.
```

---
## \#8 Posted by: Okami Posted at: 2017-01-15T01:35:40.447Z Reads: 107

```
@Ackmaniac I'm trying to find a 10S setup with vesc telemetry and data. Can you help out?

I just found a guy who pushed his board till like 50kmh and his power draw is quite constant close to 50A (~48A). (Metr.At app / topic)

Considering this, I think we I can release the info that a ''general rule of thumb'' here, is that 60A battery usually is a good mark.

 At leats that's what it looks like is usually recommended for longboards, here.

---
I also forgot to mention, that as you @Fin420 will probably use vesc anyway, you should be more concerned about its limits and not the motor ones. 

It happens that im using a car esc and they seem to be more powerful in terms of max amps they can sustain, so in my case, I was more concerned about not ''fulfilling the amps'' motor needs and not what esc can actually comfortably take..

--

On a side note - Im yet in a search of a **user who uses ''low discharge rate'' cells**, to see what his performance is.. everyone is usually using at least 3P setup with 20A per cell.. mhh

Ok, im probably ending here as I feel like I have crossed the line of what I know and what I speculate already by now.. Should let some other ''experts'' and eboard users step in :)
```

---
## \#9 Posted by: Okami Posted at: 2017-01-15T03:53:22.694Z Reads: 103

```
Some more info found elsewhere:

(A lot of quotes from Voltage sag topic):

_Might make seperate topic later, for others to find this.._

[quote="jmasta, post:15, topic:13875, full:true"]
That is 20A per cell, which why you see packs with 3+ cells in parallel.  A 10S1P pack would only have 20A rated discharge, but 10S3P would have 3x20A = 60A.

However you want a battery capable of providing more current than you would actually draw.  The more buffer the better. Pulling 60A on a 60A max battery results in significant voltage sag and reduces the cell's life.  So a 3P battery rated for 60A, should really be thought of as a 30-40A battery.
[/quote]

[quote="Ackmaniac, post:27, topic:14720, full:true"]
The biggest issue when it comes to life cycle is the temperature of the cells. When they test the cells then they always do the continuous discharge test. But that isn't they way we use the cells on our boards. We don't draw max amps all the time. Most of the time we don't even come close to that.Next thing about life cycle is the voltage that we charge the cells and how low we discharge them.

But let's say we do the worst case scenario and use them the hard way and get only 300 charge cycles. After that they only have a capacity of 60%. So in average during those 300 cycles we have 80% capacity.Let's go with a 10S4P with 10Ah. That is 360Wh. So for a average rider 36km. But we only have 80% in average so it is only 288Wh. Let's make it a bit worse and say we only can reach 25km instead of 28,8km with that.That would be 7500 km (25km * 300 cycles) on one battery pack. But that is under worst conditions with a max continuous discharge (nobody does that). In reality the pack should be good for 10000 km or more.But the most will never drive that many km with their board.
[/quote]

[quote="Namasaki, post:51, topic:14720"]
This doesn't make any sense. Why would voltage sage under max load shorten your range?

It's simple.The closer your amp draw is to the battery limit, the more it's voltage sags, The more its voltage sags, the more amps you need to maintain power. The more amps you draw the faster your battery depletes. As your battery depletes, its voltage gets lower compounding the problem. It's a vicious cycle.
[/quote]

[quote="Namasaki, post:60, topic:14720"]
This is how voltage sag affects range. More load = more sagMore sag = less range.
[/quote]

[quote="PXSS, post:63, topic:14720"]
Let's see if I can explain it better....

Basics:Power (P)= Vi*Ai = WEnergy (E)= integral(Vi*Ai*dt)= Wh

Total Energy content varies with how hard you push, push 1A on a 10A cell and you get ~12.6Wh of energy. Push 7A on that same cell and your total energy drops to ~10.75Wh. If you have a 40cell battery in ANY configuration (1s40p or 10s4p don't matter) and you're drawing an average of 1000W, you just lost at the very least 14.7% of your range this is because your performance differs when you get on the board to halfway through your ride to towards the end of your ride, to draw 1000W at 3.8V/cell it takes 6.6A/cell, at 50% and 3.44V/cell it takes 7.27A/cell and towards the tail end at 3.0V/cell it takes 8.33A/cell So you can see how 14.7% is lost is really conservative.
[/quote]

> PXSS29d
> Here's a good example on how to mitigate voltage sag and under performance on a li-ion battery

> Budget: 281.4€
> Options: 60 NCR18650GA, 44 Sony VTC6. (I get the 500+ discount since we buy a ton of batteries for work.)

> Possible configuration:
> 10S6P GA with max continuous draw of 60A
> 11S4P VTC6 with max continuous draw of 120A or temp cutoff of 80c

> 1KW load assumed.

> 1000/36v nominal / 6p = 4.62A/cell
> Now I can use Henrik's website (Lygte) to find my actual nominal voltage at this power setting.

> At 5A continuous, nominal voltage is closer to 3.48V
> 1000/(34.8*6) = 4.79A/cell
> So now we have nominal voltage and current draw for a continuous 1000W.

> At this power setting, the cells have 3.2Ah of capacity. So total energy can be measured by:
> 3.48v*3.2Ah*60cells = 668Wh.

> So I should be able to run roughly 40minutes at a constant 1000W. Which in reality is more like 35 (based on experience)

> Same process can be done for the VTC6. 
> 1000W/(39.6*4) = 6.31A
> @7A: nominal v= 3.58, capacity = 2.9Ah
> 1000W/(39.38*4) = 6.34A so we're being a little conservative by using the 7A curve. 
> Total energy = 3.58*2.9*40 = 415Wh
> Runtime @1000W: 25minutes.

> So if you constantly pulled 1000W then the 10S6P would be the way to go as it has 50% more endurance.

> Here's the upside to the VTC6s though. Your max power draw is capped at 2000W pulling 10A/cell with the GAs. Using VTC6, your max power draw is capped at 3000W pulling 20A/cell. In other words 50% more power.

> So if you need endurance, 10S6P GA cells
> If you want power 11S4P VTC6s. 
> You can most likely pull more power from both cells for short periods of time, but it'll most likely harm the life of your pack, (300 cycles, 80% capacity)
```

---
## \#10 Posted by: PXSS Posted at: 2017-01-15T04:07:56.985Z Reads: 91

```
I use low discharge rate cell @Okami. 
I use NCR18650GAs. They are only rated to 10A/cell but perform just as well as 25Rs honestly and have 3500mAh capacity. 

Here are the 5A and 10A discharge curves, GAs in red and 25Rs in blue. 
<img src="/uploads/db1493/original/3X/d/a/da55838904894c6f1cdde62422b21198be754e74.PNG" width="690" height="387">

I do not plan to run higher than 40A so the GA cells have a clear advantage for me due to the 40% extra capacity.

E: I run a 10S4P setup. 
<img src="/uploads/db1493/original/3X/7/0/70848155096f035cf4a01574f565945d5c22e967.JPG" width="375" height="499">
I dont have pics of the finished battery shamefully
```

---
## \#11 Posted by: Fin420 Posted at: 2017-01-16T21:53:26.398Z Reads: 84

```
Thanks for all the info, I've narrowed I down to Samsung 25rs if I go for a 3p configuration, or lg hg2s if I go for 2p.

Just to throw a another spanner in the works, is there a benefit to using a LiPo pack? I'm thinking at this point it would save a lot of work! 

Alien sells a 10s1p 10,000mAh 35C, price wise it's not a whole lot more than it would cost to make 2 smaller Liion packs myself.
```

---
## \#12 Posted by: Maxid Posted at: 2017-01-16T22:35:32.387Z Reads: 83

```
According to this http://lygte-info.dk/review/batteries2012/Common18650comparator.php
You should go for Samsung 30Q or LG He2 cells instead of the 25rs.
The 25rs sag heavily under load - especially in a 3p config.
```

---
## \#13 Posted by: DeathCookies Posted at: 2017-01-17T00:07:12.886Z Reads: 87

```
Instead of the HE2 i would choose the HE4.
The HE4 performs better and is even cheaper (nkon)
```

---
## \#14 Posted by: Maxid Posted at: 2017-01-17T06:18:10.124Z Reads: 86

```
According to the website I linked the HE4 sags more than the HE2 at high currents. How is it better then?
```

---
## \#15 Posted by: DeathCookies Posted at: 2017-01-17T06:39:59.650Z Reads: 88

```
Well i found different sites :D
https://batterybro.com/blogs/18650-wholesale-battery-reviews/19198431-what-is-the-difference-between-the-lg-he2-and-lg-he4-which-is-newer-better
http://ukvapers.org/Thread-LG-HE2-v-LG-HE4
https://scontent-fra3-1.xx.fbcdn.net/v/t1.0-9/10995458_852901944749128_3454517952344761327_n.png?oh=351eebfe64613e0313aec3cf8bf960c8&oe=5910D70E

Additionally it would not make sense to release a few month later a worse battery ;)
```

---
## \#16 Posted by: Maxid Posted at: 2017-01-17T07:03:19.329Z Reads: 85

```
Well seems like a typical case where @PXSS has to tell us about his experience.
I hate how there is conflicting info out there for something as simple as a discharge curve :cry:
```

---
## \#17 Posted by: PXSS Posted at: 2017-01-17T07:34:10.160Z Reads: 86

```
I've not had much experience with either cell but lygte-info shows HE2 to have a slightly better performance. I would not trust Battery Bro's review as they state that they sourced their cells from a questionable source and the HE2 seems to be defective?

I would go by spec sheets and discharge curves on lygte. As I said before, Henrik's test methods are very good and consistent plus they usually match the data that I measure too.
```

---
## \#18 Posted by: Okami Posted at: 2017-01-18T08:07:18.676Z Reads: 81

```
Consider this when going with lipo's:

> Source: https://traxxas.com/forums/showthread.php?8983235-Definitive-Word-on-Lipo-Storage-Mode-vs-Full-Charge Post 10#

>Two identical packs were both charged and discharged in the exact same matter.... except one pack was charged to 4.20v/cell and the other to 4.10v/cell. This was done in a very controlled environment... NOT in an RC. 
> After 500 cycles, the pack that was charged to 4.20v/cell had reached its life expectancy... it would not take more than 65% of its original capacity; meaning the LiPo was no longer able to be used safely.
> The pack that was charged to 4.10v/cell was still at 70% capacity after 1,000 cycles... so the .10v/cell difference more than doubled the life expectancy.

Im actually not sure what life expectancy you might get at ~300-500 cycles but if you did not know already then lipo's ''age'' faster than li-ions.. depends on for how long you are willing to go but it seems if you gonna use the board any other day.. (not sure about you climate situation).. you might get a big decrease in capacity after 1-2 or 3 years.. 

Not owning lipos nor have ran them that long but it just what a lot of ppl seems to be mentioniong. Not saying all of the lipos are that way but that's just how their chemistry work, I assume

--

Lipo might seem a cheaper / less labor intensive solution but there are some benefits when going with li-ions (and of course, a few drawbacks, like lower discharge rates)
```

---
## \#19 Posted by: PXSS Posted at: 2017-01-19T14:33:41.694Z Reads: 71

```
Most li-ions are only rated to 300 cycles to ~70%, so I doublt that longevity is any better than Li-Po.
```

---
## \#20 Posted by: Okami Posted at: 2017-01-19T15:55:49.388Z Reads: 77

```
Could you give such info? I heard that they can go to 80% or so.. 

Anyways - I thinked about this for awhile and I realized that phone batteries are actually quite durable.. that is the only and closest example I can come up with! 

I bet these RC guys which regularly talks about batteries, just overdischarge or fast charge them way too often! Hence their battery life decreases!

Also - the impression I got about Lipos comes from the fact that some ppl  said range was a lot worse after a year or so.. This made me come to realization that lipo batteries (as we can get them from hobby shops) does not last that long!

One other remark I have about lipo's - they seem to go out of balance way more quickly and dramatically than li-ions! This just suggests that their chemistry is not as stable or the cells are way too off from each other in their real capacities / ratings!..

And also this instability, which causes the cells to go out of level, may cause bigger damage to them in overall.. Im not sure how this principle works.. but it is generally said it is not a good idea to discharge some cells faster than the others.. especially if you may hit a low limit with one cell while the others are still working great..
```

---
## \#21 Posted by: PXSS Posted at: 2017-01-20T01:03:57.703Z Reads: 76

```
Cheap batteries mean not as good quality control and not as tight tolerances. So your internal resistance can vary a lot from cell to cell. 

We only buy LiPos from Thunderpower and we request that they come from the same batch and ir are matched as close as possible. We've never had issues with batteries but then again we do not run them hundreds of cycles. My personal RC LiPos also from TP are perfect after 1.5years of use, I only balance once every few charge cycles and make sure I don't discharge beneath 3.2V. 

As far as cycles on Liions. From the 25R spec sheet:
"Cycle life:
With standard charge and maximum continuous discharge. Capacity after 250cycles,
Capacity ≥ 1,500mAh (60% of the nominal capacity at 25°C)"
Sure, we do not run them at max continuous discharge but I do not see this number being any higher than 70% after 300 cycles at our discharge rates.
All the info is in the datasheets, I suggest looking it up, you'll learn more that way than asking others as there is a ton of useful information on them.

E: Cellphone batteries are lipos
```

---
## \#22 Posted by: Okami Posted at: 2017-01-20T10:09:26.770Z Reads: 75

```
Will try to look it up. Im familar with the such tests. Basically they take the maximum battery can withstand and then report the results.. you should also check the charge rate, at which they charged the cells (they have it in the datasheet).

Im not sure how reliable resource batteryuniversity is but it had a similar test but it also explained that such figures (60-70% capacity left at 300 cycles) only happen when batteries are discharged deeply every cycle, with a lot of amps and then charged at almost maximum charge rate or just a pretty high one (>1C)

Your brand of Thunderpower lipos might explain why you dont witness problems some other ppl might get when buying cheaper lipo batteries. I cannot tell from memory now but the small lipo 6s battery I had was very quickly apart in voltages between cells. I think the worst were 3.5v 3.6 3.65 3.55 or so.. Cannot cite that as useful information but it was way more than for li-ions which I have now.

--
Anyways, you brought up a topic about li-ion and lipo lifecycle time. I think we somewhat answered that but I would still like to compile a few charts or other info, where it is said in graphs.. unfortunately I don have that much time to look into that now but I know that some of this info is on battery university.

Anyways, you got a good point that with quality lipos these problems I mentioned (cell inbalance, possible lifetime decrease) are somewhat minimized or non-existant..) and with quality lipos, they might not be that far apart from li-ions in electrical durability.
```

---
## \#23 Posted by: TarzanHBK Posted at: 2017-01-20T10:58:12.901Z Reads: 68

```
All smartphone batteries are Liion!
```

---
## \#24 Posted by: Maxid Posted at: 2017-01-20T11:08:16.105Z Reads: 70

```
They are Liion polymer (=Lipo AFAIK)
http://cdn.shopclues.net/images/detailed/38707/blt9_1465225577.jpg
```

---
## \#25 Posted by: Okami Posted at: 2017-01-20T11:09:57.724Z Reads: 70

```
Yeah, that's the reason why they puff up sometimes :D
```

---
## \#26 Posted by: TarzanHBK Posted at: 2017-01-20T11:30:26.295Z Reads: 70

```
Li-ion is a general term for at least 6-different major lithium-battery chemistries that are used for different applications (LCO, LMO, NMC, LFP, LTO, LNA). For now, it's sufficient to know that most cell phones use the LCO chemistry (LiCoO2); because it offers the highest Wh/kg or specific-energy (some calls it gravimetric energy density).

:confused: I think this is deeper than expected..
I maybe go into this a bit later on when i find some time..
```

---
## \#27 Posted by: Okami Posted at: 2017-01-20T11:33:00.170Z Reads: 73

```
@TarzanHBK Actually you brought up a good point!

I also looked into this and concluded that the chemistry is probably not the same for lipos and li-ions we use on eboards (at least in some cases).. hence this may also impact cycle life and other stats.. just need to find a more detailed comparison for li ion chemistry differences.. besides some of them having high discharge capability or high capacity, which I already kind of knew.
```

---
## \#28 Posted by: Maxid Posted at: 2017-01-20T11:38:08.647Z Reads: 69

```
Don't understand your point - LiCoO2 is the chemistry used for RC Lipo batteries (and mobile phones). @PXSS is right.
```

---
## \#29 Posted by: TarzanHBK Posted at: 2017-01-20T11:42:19.349Z Reads: 73

```
yep thats the point!
We have to differ from different names, because we have different stages.
Our example here:

Battery
Li-Ion
Lithium Polymer
LiCoO2

So we often mean the same things :slight_smile:
```

---
## \#30 Posted by: Okami Posted at: 2017-01-20T11:43:30.501Z Reads: 71

```
<img src="/uploads/db1493/original/3X/5/4/542acf3828bbe5036f8f528c3fe3835ab7e426d7.png" width="690" height="185">

<img src="/uploads/db1493/original/3X/f/3/f31d328f37479f254d31d80649b45b458035401a.png" width="690" height="88">

It looks like the lipo outside structure and soft material is a bit to blame for diminished capacity in some cases.. I can imagine all the vibrations etc happening, especially, if lipos are not contained and get to rattle a lot inside..
```

---
## \#31 Posted by: Fin420 Posted at: 2017-01-21T16:55:01.645Z Reads: 63

```

`So my options are - pay more for a LiPo, but get a higher discharge rate, but reduced performance after one year.

Or build my own Liion pack for nearly half the price, with a slightly lower discharge rate, but overall longer life from the pack before reduced performance.

Seeing as Nkon have a price break at 40 cells, looks like I'm welding together a 10s4p pack of either Samsung 25r's, 30Q's or LG HG4's!

Now....which charger? :stuck_out_tongue:
```

---
## \#32 Posted by: Okami Posted at: 2017-01-21T19:04:07.801Z Reads: 65

```
Well from what @PXSS said it looks like quality lipos also work great, though they will cost more than zippys from hobbyking, i believe

I would still stick to li ions.. personally

If i can i will post some more lipo/li ion soon

--

@Fin420 How fast do you want to charge? What's your budget?

Will you go with bms or not? Depending on that you need to choose charger with integrated balancing (balance charger) or just almost a simple power supply unit (bulk charger) which just feeds the right voltage and amps to the bms circuit to charge batteries..

With your pack size I wouldnt choose 50-80w chargers.. they will take something like 3+ hours till you will finish charging your pack..
```

---
## \#33 Posted by: Fin420 Posted at: 2017-01-21T21:00:46.253Z Reads: 64

```
I would agree good quality lipos work great, but in the uk my options for buying them are quite limited! 

I was looking at http://alienpowersystem.com/shop/batteries/alien-10s-10000mah-35c-lipo-battery-flat-configuration/ but who knows what's inside it, and for the same price I could build a decent sized Li-ion pack.

My lack of knowledge regarding lipos means im probably safer sticking to Li-ions considering I'm not planning to use a bms chip.

it would have to be a balanced charger @Okami I don't want to break the bank but I also don't want to wait a few hours for a full charge.
```

---
## \#34 Posted by: Okami Posted at: 2017-01-21T21:06:20.354Z Reads: 68

```
I would suggest to order somewhere from eu.. (if you dont have to pay tax, for receiving from eu)

This way you would avoid the tax..

Im just actually having a discussion about chargers on another topic:
http://www.electric-skateboard.builders/t/my-first-and-second-oops-electric-longboard-build-log/13712/49

Anyways, the cheapest will probably be somewhere in the 20-30 Eur range + you will always need a power supply for the balance charger..

If you want to get something for the later time (for future, when your energy needs /demanded charging speed might increase) then I would suggest buying a charger in 50-70 eur range.. 

You would probably need some sort of ''splitter'' to split that 10s pack, into two 5s packs.. After that you should still need 5A capable charger at 5s, to do the charging in 2 hours..

That would be 105w in power, so 105 x 2 = 210W charger preferably..

I would advise ''Anti matter 10A 250W charger.. but the only source for it now seems to be china.. which might give you awful tax, which would make the price worse.. in the webshop its price is around 50usd

---

I actually have to run my numbers again.. im not sure whenever I calculated everything ok.. anyways.. ''general knowledge'' of me.. tells me, that for 6s ~8-10A pack, a 4-6A charger is a must.. So, with you having basically 2x 5s packs at 10.000mah, you would preferably need twice as that.. so about 8-10amps..

There is this nice little program called Calc RC, it has a seperate ''tab'' for charging.. you can play with the numbers there:


http://calcrc.software.informer.com/2.5/
(might be a bit glitchy and it is probably only for windows, so i hope you are not a mac user haha)
```

---
## \#35 Posted by: Fin420 Posted at: 2017-02-03T22:57:12.447Z Reads: 62

```
https://m.youtube.com/watch?v=Gk3vrKc4Y1w

I wonder if this if possible without frying your batteries...
```

---
## \#36 Posted by: TarzanHBK Posted at: 2017-02-04T12:24:14.928Z Reads: 58

```
we discussed that method before somewhere here and it´s nothing you should do!
The guy is shorting a battery and creating really bad solder spots.
So just don´t do it :fire:
```

---
## \#37 Posted by: Fin420 Posted at: 2017-02-05T01:30:39.382Z Reads: 54

```
That's exactly what I thought, I had all the parts handy and 10 minutes spare, so tried it out with an AA battery to see how bad it would be, it just zapped right through the nickel, and took the coating off the battery 😂 

<img src="/uploads/db1493/original/3X/a/9/a9f1c41f3635f8e877192fc9e46fdad077e78603.JPG" width="666" height="500">
```

---
## \#38 Posted by: TarzanHBK Posted at: 2017-02-06T15:40:20.131Z Reads: 49

```
yep! Imagine what would happenend if you not only scratch through the coating, but through the anode and damage the cell. Booof fireworks!:boom:
```

---
