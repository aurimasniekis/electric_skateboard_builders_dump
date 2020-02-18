# Voltage Sag &ndash; What is the most suitable battery cell?

### Replies: 114 Views: 7160

## \#1 Posted by: FloRider Posted at: 2016-12-15T15:19:35.471Z Reads: 435

```
Gd day boys n girls,
using a dual motor setup in 10s3p I experience HEAVY voltage sag (some Chinese batteries of unknown origin). I typically draw 20amps continuous and peak (going up hill no more than 40amps). 

Thinking of building myself a proper battery pack 10s3p (can't go bigger than that unfortunately because of size) and would like to know if it would be better to use

aa) Sony 18650 VTC5  (20A // 2500mah)
or
bb) Sony 18650 VTC4 (30A // 2000mah)

to avoid this king of sagging.

My thinking is that having a larger buffer between my actual amp draw and the battery's theoretical max amperage draw ability would result in less stress on the battery......but of course I might be completely off track and it may have no effect whatsoever on preventing voltage sag?

Any ideas what would be the best to do while keeping the config at 10s3p?

Cheerio!
```

---
## \#2 Posted by: laurnts Posted at: 2016-12-15T15:28:12.362Z Reads: 415

```
3p is not good enough if you have cheap li ion chinese battery. Not powerful enough to discharge. Do 4p at least with constant capable 20-30A. The higher the constant amp the better. More than around 60A is not very useful.

If size hits you, I go for 6s5p. Should be more enjoyable to ride, powerful acceleration with less top speed.
```

---
## \#3 Posted by: evoheyax Posted at: 2016-12-15T15:30:15.776Z Reads: 406

```
I have gone back to zippy 8000 mAh lipos personally. The power I get from these are so much better than li-ion. Not quite as indestructable but I used to sag 50-80% of my 18650 12s4p battery pack at times. Now with high discharge lipos, I sag at most 15% on steep hills and less than 5% on moderate hills.

I'll probably be the only guy here trying to convince you lipos are the way, but from real world experience, lipos not only sag less, but their discharge curve keeps the voltage higher for longer. This means you don't slow down as much while late into your riding. It just drops off quicker near the end instead.

If performance is your top priority (as is mine), than lipos are the way to go. I personally think li-ion are not that much safer. Things can still happen in li-ion, look at boosted recalling their batteries due to venting with the A123 cells...
```

---
## \#4 Posted by: FloRider Posted at: 2016-12-15T15:35:55.941Z Reads: 385

```
thanks @laurnts @evoheyax. I will reconsider lipos, but for the time being for my enclosure i am kind bound to 10s3p., so cannot really go any larger than that, but 6s5p is certainly an option. i will see what kind of max speed that will give me.  

Have you guys heard of Nick Hayek (the guy owning the Swatch Brand) with his new company http://www.belenoscleanpower.com in Switzerland? Hope they bring out their new battery pack next year...unfortunately did not happen this year.
```

---
## \#5 Posted by: Ackmaniac Posted at: 2016-12-15T15:42:14.354Z Reads: 360

```
[quote="evoheyax, post:3, topic:14720"]
50-80%
[/quote]

Does that mean from 4.2V a cell down to 2.1V (50%) till 0,84V (80%) a cell? :joy:
Never trust a statistic that you didn't cheat yourself.
```

---
## \#6 Posted by: FloRider Posted at: 2016-12-15T15:45:04.917Z Reads: 355

```
I thought this related to the the voltage range up to the point where the low voltage kicks in?
```

---
## \#7 Posted by: evoheyax Posted at: 2016-12-15T15:52:02.338Z Reads: 350

```
No it means I can sag from 4.2 down to 3.4 or even less.

And as I tried to tell you a while ago, lipos solved all my sagging issues... higher discharge rating == less sag, this is just a fact That you seemed to want to deny...
```

---
## \#8 Posted by: Ackmaniac Posted at: 2016-12-15T16:03:11.133Z Reads: 356

```
[quote="evoheyax, post:7, topic:14720"]
No it means I can sag from 4.2 down to 3.4 or even less.
[/quote]

And with Lipo's?
I know that they sag less, but the sag is normal for the Li-ion batterys and for the most people no issue at all. 
And would you recommend a Lipo to somebody that has no glue about batteries. And would you sell a board that has Lipos to any person who orders it? 
Think about those who would put the board in the trunk of their car in the summer. Or who leave the board switched on for a week. Or who adjust the voltage cutoff to 0V.
Do you charge your lipos and leave the house and trust the charger that it will switch off?

Not saying they are extremely dangerous but you need some knowledge. Quality Li-ion battery's mostly just simply die when you handle them wrong. The chance that they fail badly is much lower.
```

---
## \#9 Posted by: evoheyax Posted at: 2016-12-15T16:17:40.199Z Reads: 339

```
With lipos, I sag from 4.2 down to 3.9 at 100 amps. With 18650 4p (larger battery), I sag from 4.2 down to 3.4 or more at 72 amps.

I never said the sag wasn't normal for li-ion batteries. But every manufacer gives you the volt with respect to mAh graph at different amp draws. The higher the draw, the higher the sag. Simplistic solution... use cells rated to higher a discharge.

I actually gained range with a 1/5th smaller battery... now I can do 8 miles, with lion, I could only get 6... 4 miles in and I only lose 2-3 mph off my top speed instead of 5 or 6 mph off my top speed. This is due to the curve.

Are Lipos safer than li-ion? No but li-ion batteries are not high discharge batteries. We are attempting to make them high discharge, but unless you build a 6p or higher, they aren't high discharge batteries.

Yes, people can mess them up, but if I ever sold a board with them, I would clearly state what you shouldn't do to avoid problems. Use a bms and and tell people not to mess with their battery settings. Don't leave it in a car above x degrees. And if your board blows up because you ignored my warnings, that's your problem, not mine.

If you would like to bottleneck your board with li-ion cells, then go for it. But let's not pretend they perform better cause lipos outperform li-ion any day.
```

---
## \#10 Posted by: Sander Posted at: 2016-12-15T16:23:20.718Z Reads: 310

```
[quote="evoheyax, post:3, topic:14720"]
I have gone back to zippy 8000 mAh lipos personally
[/quote]

Where did you buy the li-ions 18650?
```

---
## \#11 Posted by: evoheyax Posted at: 2016-12-15T16:30:45.163Z Reads: 305

```
30 of the cells were from the space cell, the other 18 where from Amazon. I checked carefully sellers and the comments for a seller who was supposed to have real cells.

But this brings up the other problem with 18650s. Fake cells are very common. Lipos can have this issue, but buy the respected lipo manufacturer cells from hobby king and your far less likely to get a fake than 18650s...
```

---
## \#12 Posted by: Sander Posted at: 2016-12-15T16:42:52.835Z Reads: 301

```
[quote="evoheyax, post:11, topic:14720, full:true"]
30 of the cells were from the space cell, the other 18 where from Amazon. I checked carefully sellers and the comments for a seller who was supposed to have real cells.

But this brings up the other problem with 18650s. Fake cells are very common. Lipos can have this issue, but buy the respected lipo manufacturer cells from hobby king and your far less likely to get a fake than 18650s...
[/quote]

Indeed! I was just wondering where you bought them. Because the lipo 18650 should be quite good if you buy some branded like LG/Samsung. 

But if you are going back to LiPo 18650 here is some recommended and legit sites:

https://batterybro.com/collections/18650-battery
https://eu.nkon.nl/
```

---
## \#13 Posted by: evoheyax Posted at: 2016-12-15T16:58:09.667Z Reads: 274

```
They were all LG HE2. Not saying they aren't good cells, just that I draw too many amps due to hubs + I'm a heavier guy + San Francisco's hills, so to mitigate sag, at 12s, 120+ con amp rating is necessary.  With 18650s, that's a 12s6p. Most of us don't have that kind of space. So lipos make more sense to get a higher amp rating.

If your going to stick to 18650s @FloRider , the Samsung 25R is highly recommended by many in this community. The VTC4 might reduce your sag (since they are supposetly 30 amp con cells), but from looking at tests in the past, they may not be any better in terms of sagging than the other 18650s out there as they may not really be 30 amp con cells.
```

---
## \#14 Posted by: Okami Posted at: 2016-12-15T17:04:45.612Z Reads: 272

```
[quote="evoheyax, post:13, topic:14720"]
The VTC4 might reduce your sag (since they are supposetly 30 amp con cells), but from looking at tests in the past, they may not be any better in terms of sagging than the other 18650s out there as they may not really be 30 amp con cells.
[/quote]

[quote="FloRider, post:1, topic:14720"]
bb) Sony 18650 VTC4 (30A // 2000mah)
[/quote]

I would agree. There were vape tests on other forum and the guy who made the test said that these vtc 4 are more like 23A.. and already at such discharge they get quite warm or so. 

He did mention that they work better than other cells at load and does not get as hot as others.. but he went into detail that 30A is something like a theoretical discharge which is only meant for a short time anyways..

So, if I were in your place and price would be okay I would probably just go with vtc 5 and enjoy the added capacity..(on the contrary, samsung 25R seems to be similar (at least have not seen tests of both of them side by side) and samsung's might be a bit cheaper.
```

---
## \#15 Posted by: Sander Posted at: 2016-12-15T17:06:46.939Z Reads: 251

```
I think im gonna order these: https://eu.nkon.nl/lg-18650-hg2.html
I think they should quite good enough?
```

---
## \#16 Posted by: evoheyax Posted at: 2016-12-15T17:09:40.698Z Reads: 258

```
LG HG2s in the graphs posted here a few months ago showed similar performance to the LG HE2 and Samsung 25R.

Idk if that's a good source or not. This is my issue with 18650s right now. You need a good source or you'll likely get fakes that do a fraction of what you expect.
```

---
## \#17 Posted by: Okami Posted at: 2016-12-15T17:19:42.715Z Reads: 259

```
He's gonna get his batteries from Eu distributor of Li ion cells, not from some shady chinese seller.

Btw, here's where I look for tests / reviews:

http://lygte-info.dk/review/batteries2012/Common18650comparator.php

And here's a good one about vtc5.

https://www.e-cigarette-forum.com/forum/threads/sony-vtc5-20a-2600mah-bench-test-results-a-good-20a-cell.683772/

It states that the cell reaches 82 degrees celsius (at 20A).. that's crazy actually. But I think they keep the current for prolonged time when running at 20A..
```

---
## \#18 Posted by: Ackmaniac Posted at: 2016-12-15T17:25:10.279Z Reads: 245

```
Nobody of use drains his battery continuously at this amperage. I think I should implement the average consumption in my app. Actually that's not a bad idea.
```

---
## \#19 Posted by: Sander Posted at: 2016-12-15T17:57:28.429Z Reads: 238

```
There is one guy on this forum that buys 18650 and makes battery packs, he had no problem with them and he says they're legit.
```

---
## \#20 Posted by: Sander Posted at: 2016-12-15T18:00:09.205Z Reads: 236

```
[quote="evoheyax, post:16, topic:14720"]
Samsung 25R.
[/quote]

Do you think this battery is good?
https://eu.nkon.nl/review/product/list/id/1852/#review-form
They said its good vaping battery etc. 
And one guy has used this for over 8 months with no problems.

Nah I will buy the Samsung INR18650-30Q 3000mAh - 15A
Its cheaper and on the comparason it was better then lg hg2 on from 1 to 15 amp with Ah
```

---
## \#21 Posted by: evoheyax Posted at: 2016-12-15T18:23:03.627Z Reads: 223

```
My app does average amps (battery and motor). The issue with average is it takes in the time your not moving (unless you calculate it for only when your moving, but even then). You really want to look at the highest continuous that you do, and work around that number.

@Sander never seen anyone using it here. You need an efficient belt drive for a low discharge cell like that in at least a 10s4p.

All I can say is... Lipos fixed all of my issues!
```

---
## \#22 Posted by: Sander Posted at: 2016-12-15T18:33:59.992Z Reads: 228

```
[quote="evoheyax, post:21, topic:14720"]
@Sander never seen anyone using it here. You need an efficient belt drive for a low discharge cell like that in at least a 10s4p.
[/quote]

I will have 12s4p and the motor will not take more then 30 amps for the Carvon 2.5
But Im waiting for the Carvon 3 so I plan on buying, and I think the amps will be lower for it.

Max Amp on Samsung = 15A
Safe side Amp = 10A

4 in parallell = 10A * 4p = 40A

I can safley drive with 40 amps.
And in the settings of the vesc I can limit the amps taken from the batteries. So I can set the max 20Amp on one VESC because I will have dual.
```

---
## \#23 Posted by: Pedrodemio Posted at: 2016-12-15T18:36:18.003Z Reads: 219

```
Use this site to compare the cells http://lygte-info.dk/review/batteries2012/Common18650comparator.php

The best to reduce voltage sag is the VTC6, way better than the 25R, but expensive, i dont know how it behave on other aspects such as cycle life

its lower sag than the HG2 and a little bit better than the 30Q
```

---
## \#24 Posted by: Hummie Posted at: 2016-12-15T18:39:09.194Z Reads: 212

```
Li-ion are probably safer but has anyone tested if they are lasting longer than Lipo with the high discharges we do? The discharge ability of Lipo is awesome. 

boosted stopped using the a123 lifepo4 (lithium iron) and went to Li-ion and then had issues. Speaking of lifepo4 the headway cells are awesome with good discharge and way more cycles possible than Li-Ion and their screw terminals are nice. Bit heavier and more expensive but the safest high discharge stuff
```

---
## \#25 Posted by: chinzw Posted at: 2016-12-15T18:39:59.226Z Reads: 207

```
Why would you need 100A with 12s? Thats around 5000W o.O
```

---
## \#26 Posted by: Pedrodemio Posted at: 2016-12-15T18:41:12.434Z Reads: 210

```
They went to Li-ion just on the extended range pack that is not on the market yet, all the problems they are having is with battery packs that use A123 cells, the same as the previous gen board

One day i want to try a Lipo, with lower capacity but faster charge time
```

---
## \#27 Posted by: Ackmaniac Posted at: 2016-12-15T18:57:17.864Z Reads: 211

```
The biggest issue when it comes to life cycle is the temperature of the cells. When they test the cells then they always do the continuous discharge test. But that isn't they way we use the cells on our boards. We don't draw max amps all the time. Most of the time we don't even come close to that.
Next thing about life cycle is the voltage that we charge the cells and how low we discharge them.

But let's say we do the worst case scenario and use them the hard way and get only 300 charge cycles. After that they only have a capacity of 60%. So in average during those 300 cycles we have 80% capacity.
Let's go with a 10S4P with 10Ah. That is 360Wh. So for a average rider 36km. But we only have 80% in average so it is only 288Wh. Let's make it a bit worse and say we only can reach 25km instead of 28,8km with that.
That would be **7500 km** (25km * 300 cycles) on one battery pack. But that is under worst conditions with a max continuous discharge (nobody does that). In reality the pack should be good for 10000 km or more.
But the most will never drive that many km with their board.
```

---
## \#28 Posted by: Hummie Posted at: 2016-12-15T19:01:16.564Z Reads: 197

```
I see. So their lifepo4 are smoking.  Surprising as they're touted as the safest. Not catching fire at least I think.
```

---
## \#29 Posted by: Okami Posted at: 2016-12-15T19:18:15.124Z Reads: 201

```
Good points. I think these EV guys (ebike users and other regular commuters) ''drain'' their packs capacity over time.. With lipo''s it seems to be happen faster than for li ion. Dunno about high stress and such but still..

One more point to add for these 300cycles. I saw that they also use 4A charging per cell, which is the max recommended, so that is basically the worst case scenario - high discharge and high charge rate. 

Average consumtion could be a good one but you should probably take out the time/data when board is not rolling, like evoheyax mentioned.
```

---
## \#30 Posted by: Ackmaniac Posted at: 2016-12-15T19:30:20.580Z Reads: 196

```
But that is the time the cells cool down. I am talking about the average consumption which brings the temperature up. just to have a realistic case. ´
The point i want to make is that i can't even overheat my laptop cells which i treat like a bitch. And they are not made for that. So we should enjoy our ride and don't feel bad when we have fun because we might do something bad to the cells and could loose a charge cycle.
```

---
## \#31 Posted by: evoheyax Posted at: 2016-12-15T19:42:08.497Z Reads: 197

```
[quote="chinzw, post:25, topic:14720, full:true"]
Why would you need 100A with 12s? Thats around 5000W o.O
[/quote]

You don't need to pull it, but if you can pull 100a continuous, you'll be able to pull 40 amps with far less sag than a battery with a max of 60 amps continuous.

Some sag will always exist. But you should try to mitigate it as much as possible. And easiest way to mitigate sag is to increase your max continuous amps far higher than you will ever pull.

If you pull close to your cells max continuous rating, you will sag very heavily.
```

---
## \#32 Posted by: Okami Posted at: 2016-12-15T19:49:39.037Z Reads: 202

```
If someone is on ES facebook group, this looks interesting -

https://www.facebook.com/groups/improved18650packs/permalink/1748144265506227/

Not entirely related with sag.. but more with temp of cells. 

> 14s6p brand new _Panasonic_ **PF** pack test at 20-25A :
> Room temp 12°C
> Start state : charged/balanced pack at 58.4V, ~20°C 
> Bms 30A continuous rated
> Note : the current is not constant, i have to use the CA current limiting feature in the future.

<img src="/uploads/db1493/original/3X/f/f/ffa6018996e4904056f15b788a6279ff251663c3.jpg" width="666" height="500">

I think PF's are rated for 10Amps, but he run them at +~3A or so (18/6 = 3).
He also pinpointed that you cannot rely on data sheet data or such.

---
<img src="/uploads/db1493/original/3X/b/a/ba7ca6c2f0e7057448304901e6d45a782797a9d5.png" width="690" height="92">
From: https://www.e-cigarette-forum.com/forum/threads/panasonic-ncr18650pf-10a-2680mah-18650-bench-test-results-a-great-battery-beats-mh1-and-mj1.692438/

---

My conclusion - if cells are discharged at the max specicified discharge rating, they do get quite warm. usually probably hot.. 

So in order not reach this state, they probably should be ''safely'' discharged only at 50% of their max rating or so..  

Though, like @Ackmaniac said, we dont push them such hard all the time and they have time to cool down also.. the only instance would be hills where it would be possible to put the strain on batteries for longer periods of time (but the vaping forum somewhat shows that this does not mean the cells will get bad instantly)
```

---
## \#33 Posted by: Okami Posted at: 2016-12-15T20:04:26.375Z Reads: 179

```
Agree about not loosing fun. I believe we should not baby sit them all the time.. just make sure they are not taken to the extremes.. like running the cells at 90C degrees more than they need to.

@Ackmaniac is it possible to add external temp sensors to the vesc and also show this data in the app?

Would be cool to see the realtime battery temp along with all the other parameters!

(or perhaps, some of the vesc/motor sensors can be placed in between the batteries..)
```

---
## \#34 Posted by: Ackmaniac Posted at: 2016-12-15T21:11:38.000Z Reads: 180

```
> So in order not reach this state, they probably should be ''safely'' discharged only at 50% of their max rating or so..

Can't agree on that. Then we are back at being worried all the time. Get some proper cells. If you have a 10S4P of Samsung 25R you will be fine running them at 80 amps battery max. You could even go higher than that because we don't draw that amps contentiously. 
When i buy a Ferrari then i don't reduce the throttle by half to be safe. If we would draw constantly the max battery amps then i would agree. But we don't do that.
```

---
## \#35 Posted by: evoheyax Posted at: 2016-12-15T21:23:15.566Z Reads: 177

```
[quote="Ackmaniac, post:34, topic:14720"]
If you have a 10S4P of Samsung 25R you will be fine running them at 80 amps battery max
[/quote]


Define fine?

Why do you think sag doesn't matter? The cells will live, shorter than you'd like, but they will live. Really though, you'll sag so hard though that you'll loose 1/3rd of your range due to sagging vs with lipos. This is why I get more range from my lipos than my 18650s, even though my 18650s are 1/5th larger...

How hard do you push your boards? I haven't seen any info about your builds, or your route/riding style. No offense, just trying to figure out were your mind set is coming from...

I'm telling you my numbers of sagging and the results I'm getting from it, and it seems like your saying I'm lying or something, cause your completely ignoring my results... It's not going to kill the cells, but it will kill performance. You get 10s performance with a 12s basically, because it sags down to a 10s voltage like that when you pull 80 amps from my HE2 cells, and the graphs for the 25R are pretty much the same.
```

---
## \#36 Posted by: Okami Posted at: 2016-12-15T21:41:03.885Z Reads: 177

```
[quote="Ackmaniac, post:34, topic:14720"]
When i buy a Ferrari then i don't reduce the throttle by half to be safe.
[/quote]

Sorry for the comparison / assumtion of 50%. That's is just my ''theory'' of **how not to make** the cells reach very high temperature. 

It is totally okay to push them to the limits.. I did so once with my pack and got 60A peak (if I can trust my wattmeter).. that made me to think whenever the batteries were not able to offer more or there was something else at play then.. The cells will probably live just fine if you do heat them up once or twice or even many times.. 

But Im seeing this more as a precaution - ''oh better not accidentally scratch my car (batteries)'' vs .. ''it does not matter whenever I scratch it or not.. I dont really care''.. 

So yeah, that's just my opinion which I got from reading that the cell can get to like 90C degrees.. and from other studies that I read that at higher temps the elements/chemicals just start to break down in the cell more.. 

If I were (or someone else is) running used laptop cells then I think it does not matter as much if you do heat them up or not.. but it might matter more, if the cells you use have been bought for ~4usd, assembled in the pack and you expect them to deliver good results for quite some time and not fail prematurely..

If it did not matter.. I think everyone could just buy 10A-15A (or even lower) discharge cells, make small packs and just drive them to the max limits without caring about the temperature.. but - with high discharge there's usually this counter-effect of getting less capacity, like @evoheyax mentioned..
```

---
## \#37 Posted by: Sander Posted at: 2016-12-15T21:44:34.366Z Reads: 176

```
[quote="evoheyax, post:35, topic:14720"]
it sags down to a 10s voltage
[/quote]

You could have a dead cell or a bad cell. Have you done capacity testing and voltage testing?
```

---
## \#38 Posted by: evoheyax Posted at: 2016-12-15T21:48:44.885Z Reads: 174

```
I haven't done testing for a dead cell or capacity testing, but did check the voltages of all cells before I built the pack, and the range at the beginning and sagging were still pretty poor.
```

---
## \#39 Posted by: Sander Posted at: 2016-12-15T21:49:41.587Z Reads: 172

```
[quote="evoheyax, post:38, topic:14720"]
I haven't done testing for a dead cell or capacity testing
[/quote]


There you have it if  one of them have very much lower capacity it can cause some issues I think
```

---
## \#40 Posted by: evoheyax Posted at: 2016-12-15T21:51:21.893Z Reads: 165

```
I don't know their capacities, but they all discharged and charged pretty close to each other. I don't think any cells had any flaws, as I would of expected the cells to charge and discharge at different rates is one was bad...
```

---
## \#41 Posted by: Sander Posted at: 2016-12-15T21:52:01.300Z Reads: 150

```
Have you done discharing one by one?
```

---
## \#42 Posted by: evoheyax Posted at: 2016-12-15T21:57:30.664Z Reads: 149

```
No, but they won't balance themselves while discharging, so I would expect one of the cells to become unbalanced while discharging if it had less capacity. Since I didn't see that, I should be able to assume they are pretty close. None of the cells ever got warm to the touch even. (because they never ran at 20 amp per cell for very long)

I also ran them through 10s for a few cycles as the "space cell" and I had a lot of sagging.
```

---
## \#43 Posted by: Sander Posted at: 2016-12-15T21:59:01.775Z Reads: 151

```
So  your problem can be you may have a dead cell or it charges wrong etc. If I were you I would charge all the battery one at the time and then discharge 1 by 1. I hope you haven't the welded them together :p

EDIT: Or not, it might be the brand you have, they are unknown!
```

---
## \#44 Posted by: Ackmaniac Posted at: 2016-12-15T22:21:13.022Z Reads: 157

```
I am not saying that you lie. I simply think it is wrong to compare lipos and li-ion in percent by a baseline that you define.
But anyway, lets sumarize the facts.

As far as i can remember your board is setup to
65 km/h max speed, for a 220 pounds rider in san francisco with the steepest hills and 4 hummie hubs with a average total consumption of 50Wh a km. You don't continue to ride when the board dosn't bring full performance anymore.

All those values are extreme (no offence to your weight). So i think it is wrong to say that this is the raw model of a board. This board really needs the most power it can get and in your case i understand to go with lipos. But many people here are absolutely fine with a normal board and they would have no issues with a li-ion battery. And you set the baseline where you think the voltage sag is not except-able anymore. But that is not where the limit of the battery is by the specs.

Next thing is that you didn't mention this as a problem for your board before the Raptor 2 came out. Could be coincidence but feels a bit strange to me.

But you are right that the lipos have less voltage sag as li-ion. But i say that this isn't a problem as long as you don't push everything to the extreme limits.
And if you have for example a 10S4P and set your battery max amps for each VESC to 30A (60A total) for a board that is setup to 45 km/h you will barely notice a difference between lipo and li-ion cells. The top speed might be 1 mile less but that's mostly it.
```

---
## \#45 Posted by: evoheyax Posted at: 2016-12-15T22:43:35.340Z Reads: 153

```
[quote="Ackmaniac, post:44, topic:14720"]
Next thing is that you didn't mention this as a problem for your board before the Raptor 2 came out. Could be coincidence but feels a bit strange to me.
[/quote]

I had mentioned in my thread that I had issues with voltage sag way before the raptor 2.

I also created a thread with a pole asking users how much sag they had, mentioning sag was a big issue for me.

I have mentioned sag long before it but it was just recently I finally had the money and time (due to the costs of college) to try lipos on this setup.

I don't stop also when I get to were the performance degrades. I just consider that an issue for me.

Maybe many won't have these issues that I have, I do do things on the bleeding edge. But what you can know then is that anything I produce has high standards of performance, under the most extreme of conditions :wink:
```

---
## \#46 Posted by: Pedrodemio Posted at: 2016-12-15T22:48:36.111Z Reads: 145

```
One way to counter that is to use more cells in series, that's what boosted done in their extended range pack, if I'm not mistaken it will be 13S2P, so even if the cells sag you won't loose top speed or significant power, it's basically to have a 10S board that has 25km/h top speed with the cells almost empty, so you limit the top speed to 25 and the rider will not notice the performance reduction
```

---
## \#47 Posted by: Ackmaniac Posted at: 2016-12-15T22:49:55.411Z Reads: 145

```
Some day i have to try a board with 65 km/h. Really curious how that feels. The difference from 45 to 50 is already like from fast but i can handle that to fuck that is fast and don't do a mistake now. But 15 km/h more must be quite impressive and scary. I think i will try next summer. But then with motorcycle leather gear.
```

---
## \#48 Posted by: chinzw Posted at: 2016-12-15T23:08:34.782Z Reads: 139

```
This doesn't make any sense. Why would voltage sage under max load shorten your range? You shouldn't be pulling max amps all the time, so you should also not see sag all the time. Now if you are riding only uphill and weigh 200kg, then you're a special case and should be treated as such.
```

---
## \#49 Posted by: Namasaki Posted at: 2016-12-15T23:52:35.311Z Reads: 149

```
I totally agree with @evoheyax
I started with 12s Lipo 5000/ 25c  125a continuous 
They where ok. 
Then I tried Li-ions 10s 9000mah  60a continuous 
I was very disappointed. 40% sag going up 10% grade. Ok on flat ground with light wind. 
Then I built an other Lipo system 10s 5000/60c 300a continuous. 
Now I can power up that 10% grade and my total pack voltage only sags 1 volt. 
Range also improves as sag is decreased. 
I learned this truth the hard way, you just can't have too much battery!
So if you want to eliminate voltage sag, I recommend a battery that's capable of 10 times the current your pulling.
It not easy to do this with Li-ions. You'll need a lot of cells. 
Lipos offer the most power per pound and are safe enough if you treat them with respect. 
Btw, my batteries don't even get warm pulling my 190lbs up hills.
```

---
## \#50 Posted by: Ackmaniac Posted at: 2016-12-15T23:57:48.001Z Reads: 142

```
Still doesn't make sense that a 10S 9000mah battery should have less range then a 10S 5000 mAh battery. What where the voltage cutoff start and end on both setups?
```

---
## \#51 Posted by: Namasaki Posted at: 2016-12-16T00:01:27.229Z Reads: 154

```
[quote="chinzw, post:48, topic:14720"]
This doesn't make any sense. Why would voltage sage under max load shorten your range?
[/quote]
It's simple.
The closer your amp draw is to the battery limit, the more it's voltage sags, 
The more its voltage sags, the more amps you need to maintain power. 
The more amps you draw the faster your battery depletes. 
As your battery depletes, its voltage gets lower compounding the problem. 
It's a vicious cycle.
```

---
## \#52 Posted by: evoheyax Posted at: 2016-12-16T00:06:56.779Z Reads: 151

```
Even on flat ground, I sag a decent bit and on slight up hills, I sag pretty bad. I have very little flat ground anywheres to ride on. San Francisco in the sunset district is almost exclusively hills. Probably under 10% of the roads here are flat or under 2% grade of steepness. This means I'm always sagging pretty heavily. So when I get my cells down to 3.6v, I must stop. If I have steeper hills to tackle, I must tackle them before I hit 3.8v or I'll sag down past 3.2v per cell. In effect, I'm losing about 30% of my range due to sag. Now with high discharge lipos, I can get my cells down to 3.3v before I sag before the cutoff. The effect is most range. I know I'm over simplifying this, but my real world tests with lipos and with liion showed me that a 12s 10 Ah li-ion got 6 miles of range while a 12s 8 Ah lipo got 8 miles of range. This is one of the reasons why I nag so much about sag. It slightly dampens performance (which may not be a big deal to some, it should be if your buying the quote un quote "most powerful" direct drive board IMO), but also reduces range, as you must stop at a higher voltage. With the VESC, this will just mean I can't climb the hills I need to climb when my battery is suppose to have 50% left, as my voltage cutoff will start to kickin. Even with 25% of my lipo left, I can climb the hills I need to without sagging below 3.2.
```

---
## \#53 Posted by: Ackmaniac Posted at: 2016-12-16T00:10:48.460Z Reads: 141

```
That's not correct sorry. Because watts is voltage multiplied by amps. So the power drawn from the battery is still the same. As long as you don't reach maximum duty cycle the motor doesn't care where the watts he needs come from. But more amps is also more heat so you might loose a bit but 80 % (5000 compared to 9000) is beyond my imagination. Expecially when you take into account that the voltage difference is only 15 %.  So at a full charge under 80A load you need 15% more amps for the same power. But this is only for the short moments when you draw max amps. 
To me it sounds that your cells had issues.
```

---
## \#54 Posted by: Ackmaniac Posted at: 2016-12-16T00:24:11.694Z Reads: 141

```
With li-ion you can go down to 3V or even 2.8V as cutoff. I set mine to 2.66 for example. With lipos a cutoff at 3.2V is already very low. So this is of course a explanation for the range difference. And you don't need to worry about the cutoff. Because it doesn't switch off the board. It starts to reduce the power until it reaches that level. 
So the vesc helps you to stay in the range you have set as cutoff end. 
That means it starts to reduce the power when it reaches the cutoff start and doesn't give any power anymore when it reaches the cutoff end. 
With a lipos you can get the feeling that it shuts off if you go as low as 3.2V. Because the lipos cells collapse at that low voltage already. Should mean when you reach that voltage under load it is OK. But when you reach that voltage without load then they can jump from 3.4V to like 3.0V in a couple of seconds. Of course that also depends on the lipos. So you need to set different cutoff start and cutoff ends for a lipo and a li-ion battery. 
That is also the reason why I said that you can't compare  the voltage sag in % if you have the same cutoff start and end.
```

---
## \#55 Posted by: Namasaki Posted at: 2016-12-16T00:36:00.577Z Reads: 135

```
I tested my Li-ion pack 10s 9000mah on flat ground and got 27 miles
Then I tested it on a a road with long hills and only got 10 miles. 
My 12s 5000/25 would go 12 miles on flat or hills. 
My 10s  5000/60 went 13 miles with using it up. 
I'm not just throwing theory out there. 
Like I said, I learned this the hard way and have proved it myself.
```

---
## \#56 Posted by: evoheyax Posted at: 2016-12-16T00:36:28.218Z Reads: 134

```
[quote="Ackmaniac, post:54, topic:14720"]
That is also the reason why I said that you can't compare  the voltage sag in % if you have the same cutoff start and end
[/quote]

I can see your concern, which is why I said I'm oversimplifying it. The discharge curves of lipos vs li-ion are different and thus, it screws any data immediately. But what I also said is from real world testing, this was the case. I knew my limit with the 18650s very well, and with the lipo, I got 2 miles more past that limit.
```

---
## \#57 Posted by: Ackmaniac Posted at: 2016-12-16T00:41:45.783Z Reads: 139

```
By the way when you set the cutoff for the Samsung 25R to 3.2V the you only use 40% of the capacity under 20A load.


@Namasaki what were your cutoff levels with li-ion and lipos? 

http://www.mountainprophet.de/wp-content/uploads/2015/06/Samsung30q.png
```

---
## \#58 Posted by: Namasaki Posted at: 2016-12-16T00:52:45.020Z Reads: 144

```
My BMS cutoff was set at 2.8v so if any cell hit that, the BMS would shut down. 
I ran the Li-ion pack till the BMS shut down. 
But really, I see your having trouble believing our report even though we have tested and proven what where saying. 
So the best solution if you want the truth is to go build different types of battery systems like @evoheyax and I have and prove it to yourself.
```

---
## \#59 Posted by: Ackmaniac Posted at: 2016-12-16T00:59:46.856Z Reads: 151

```
Doesn't make sense to me.
The 12S 5Ah battery has the same range on flat or hills.  The 10S 5AH battery goes further than the 12S battery. And the li-ion does great on flats but fails on hills with 80% more capacity. I am confused now. 
One last question. What li-ion cells where that? And I hope you don't use the same bms for the lipos.
```

---
## \#60 Posted by: Namasaki Posted at: 2016-12-16T01:53:26.328Z Reads: 155

```
This is how voltage sag affects range. 
More load = more sag
More sag = less range. 
I did not use a BMS on my 12s Lipos. I monitored
Voltage. 
I'm using the same BMS on my 10s Lipos but monitoring voltage and not depending on BMS cutoff. 
My stoping point with 12s Lipo was normally 42v
Which usually got me around 12 miles
The 10s Lipo, I have not yet gone below 36v and have not had a chance to finish testing it however, I did get 13 miles with the battery still above nominal voltage. 
The Li-ion cells I tested where Basen black 26650's
4500mah 30a continuous in a 10s 2p pack.
```

---
## \#61 Posted by: Pedrodemio Posted at: 2016-12-16T03:40:21.956Z Reads: 147

```
According to this test the Basen has 24,6mOhm internal resistance, pack total is 123mOhm, and with at 60A current will sag 7V approximately 

https://cdn.ampproject.org/v/s/amp.reddit.com/r/electronic_cigarette/comments/41wcya/26650_bench_test_results_and_ratings_table/?amp_js_v=6#

Using the VTC6 in 10S3P that has a 20mOhm resistance(calculated from the actual discharge charts from lygte) you get 66mOhm pack resistance and 4V sag, lower if you use 4p, in my opinion your experience with Li-ion used the wrong cells and configuration for your specific requirements

Voltage sag sucks, I made the same mistake in my current board and went with Panasonic NCR B that has a 110mOhm IR, I sag more than 7V at only 20A, but if arround me had less hills, it would be perfectly fine
```

---
## \#62 Posted by: Namasaki Posted at: 2016-12-16T05:01:24.391Z Reads: 146

```
Good point, The internal resistance is a very important factor. This is another fact that I like about Lipos is that they generally have very low internal resistance.
I'm currently using Turnigy packs that are around 1.5 milliohm per cell.
```

---
## \#63 Posted by: PXSS Posted at: 2016-12-16T06:15:14.761Z Reads: 151

```
I know where @Ackmaniac is stuck.
Let's see if I can explain it better....

Basics:
Power (P)= Vi*Ai = W
Energy (E)= integral(Vi*Ai*dt)= Wh

Total Energy content varies with how hard you push, push 1A on a 10A cell and you get ~12.6Wh of energy. Push 7A on that same cell and your total energy drops to ~10.75Wh. 
If you have a 40cell battery in ANY configuration (1s40p or 10s4p don't matter) and you're drawing an average of 1000W, you just lost at the very least 14.7% of your range this is because your performance differs when you get on the board to halfway through your ride to towards the end of your ride, to draw 1000W at 3.8V/cell it takes 6.6A/cell, at 50% and 3.44V/cell it takes 7.27A/cell and towards the tail end at 3.0V/cell it takes 8.33A/cell So you can see how 14.7% is lost is really conservative.

Now if you have a lipo with the same rated capacity at the same nominal voltage and a 60c discharge rating your voltage sag is non existent and your discharge curve is pretty flat which means your battery energy doesn't change regardless of how much power you draw. 

So yes, hills do reduce range. Same as a car.
```

---
## \#64 Posted by: Pedrodemio Posted at: 2016-12-16T11:50:48.954Z Reads: 145

```
Yeah, and what about cycle life? The only ones I saw test was the Graphene series, but they too expensive at the momment, even the bare generic turnigy cells are pretty expensive, and with that I get half of the range than 10S3P

@PXSS that's pretty much it, and is important to remember the resistance relation between load and cell, at 60A, without sag, 37V, your load is approximately 600mOhm, this number goes lower with increasing current, to the point where the load resistance is equal than the battery internal resistance, this is the maximum power transfer point, the same amount of power going into the motors is heating the battery, not good since half of the energy is being thrown away and things will get hot quickly, I believe @Namasaki was getting here pretty often with this crazy 100A draw, and thus explains the 50wh/km
```

---
## \#65 Posted by: PXSS Posted at: 2016-12-16T12:27:27.670Z Reads: 138

```
You should never even be in that region imo. 
The internal resistance of the cells is less than 40mohm, 10 in series: 400mohm, 4 in parallel: 100mohm at the battery level. For their internal resistance to quadruple, you would need to be running them hot (60+c) near their low end while pulling ridiculous amounts of current. If you require to constantly pull 100A, your system has been designed wrong. Hell, if you're constantly drawing 60A on a 10s4p, your system has been designed wrong. You most likely needed a different kv motor with more torque
```

---
## \#66 Posted by: Norco Posted at: 2016-12-16T12:39:39.999Z Reads: 133

```
I just bought some Samsung 25R from NKON. All batteries weighed in as genuine and within 0.01 of a V on delivery, positive cap pattern is correct too so I'm pretty confident they are the real deal. I sacrificed a bit of capacity to gain on the amp draw and price which means I can put together a 10s4p.
```

---
## \#67 Posted by: DeathCookies Posted at: 2016-12-16T12:40:34.655Z Reads: 136

```
[quote="PXSS, post:65, topic:14720"]
You most likely needed a different kv motor with more torque
[/quote]

If you want a speed monster with great torque you will probably need 100A?
```

---
## \#68 Posted by: PXSS Posted at: 2016-12-16T12:53:01.693Z Reads: 134

```
[quote="DeathCookies, post:67, topic:14720, full:true"]
[quote="PXSS, post:65, topic:14720"]
You most likely needed a different kv motor with more torque
[/quote]

If you want a speed monster with great torque you will probably need 100A?
[/quote]

Then use the appropriate sized battery. A 10S4P is definitely not it.

Depending on your top speed/torque/max power draw, you could run 8S9P, 10S7P 12S6P. They will all be most efficient at different rpms so take the most efficient system and run that for something that could easily provide 2000W+ with @ 7A/cell. 

This setup would be very costly as it requires 72cells, but you'll be running for days and days.
```

---
## \#69 Posted by: Sander Posted at: 2016-12-16T13:03:01.976Z Reads: 122

```
how much amp and capacity has the 18650 u have?
```

---
## \#70 Posted by: Norco Posted at: 2016-12-16T13:15:31.949Z Reads: 121

```
2500mAh and 20 amp max draw per cell. 
10s4p 10000mAh and 80amp max draw (to be set at 80amp via VESC)

Additional cost of 3000mAh and lower max draw wasn't worth it for me.
```

---
## \#71 Posted by: PXSS Posted at: 2016-12-16T14:24:48.478Z Reads: 126

```
80A will kill your endurance and your max power draw is 2500W avg. I would suggest 60A as your max: you gain a good amount of endurance, increase life cycles and you can still pull 2000W avg. l say average because your max power draw decreases as your battery discharges.
```

---
## \#72 Posted by: Sander Posted at: 2016-12-16T14:25:17.561Z Reads: 131

```
Is this right:
Does your board drive around 30km in distance?

10s * 3.7 * 10Ah = 37km
```

---
## \#73 Posted by: PXSS Posted at: 2016-12-16T14:27:32.904Z Reads: 130

```
Depends on more than that. You need wheel size, gear ratio, motor kv etc to calculate range. It cannot be calculated from the battery alone unless you assume a specific W/km consumed by the mechanicak system
```

---
## \#74 Posted by: Norco Posted at: 2016-12-16T14:52:21.435Z Reads: 125

```
What @PXSS said. Also I have no idea as I haven't finished my build yet. I am a heavy guy but in pretty much 100% flat terrain. I am not expecting that distance though. Probably more like 10miles or 16km on 14/36t , 90mm wheel and 192kv motor.

Maybe I will go 60amp (to begin with for sure) I doubt I will have many occasions to go max amps anyway.
```

---
## \#75 Posted by: Namasaki Posted at: 2016-12-16T15:16:20.937Z Reads: 125

```
I never said I was drawing 100a. 
I've monitored amp draw from the battery while hill climbing. Only 18a at 12s
And around 35a at 6s
I didn't test 10s but would guess around 20a
But in my tests, drawing 20a constant from a 60a battery caused a lot of voltage sag. 
Drawing 20a from a 300a battery causes very little sag.
```

---
## \#76 Posted by: Pedrodemio Posted at: 2016-12-16T15:17:36.130Z Reads: 120

```
I agree, but I should not have lost a lot of performance drawing "only" 20A
```

---
## \#77 Posted by: PXSS Posted at: 2016-12-16T15:21:51.934Z Reads: 121

```
How many volts are we talking about and what cell? Maybe I can help troubleshoot, but yes Lipos are going to see minimal voltage sag and deliver way more power, thats why RC airplanes use them and not li-ions

If you were running a 12S3P that actually sounds about right... You were running 6A/cell which is right around where you start losing performance without using VTC6 cells which can handle the sag much better
```

---
## \#78 Posted by: Sander Posted at: 2016-12-16T15:26:10.428Z Reads: 124

```
[quote="PXSS, post:73, topic:14720"]
that. You need wheel s
[/quote]

So can you tell me the whole formula, for flat ground. Also with weight, motor kv etc.
```

---
## \#79 Posted by: PXSS Posted at: 2016-12-16T16:25:39.940Z Reads: 130

```
Eek. If only I remembered it...
Lets see...

Electric power = mechanical power
Mech Power = Torque * RPM
RPM = kv*V
Torque = Mech Power/RPM
Not sure how the throttle works on vescs...

Speed = RPM * Pi * Diameter

Your torque needed is related to your weight, and friction between the wheel and the ground. 
Not sure what that equation is. 

Someone around here must have a calculator already done in excel.
```

---
## \#80 Posted by: johnny_261 Posted at: 2016-12-16T19:09:44.991Z Reads: 131

```
Seems like there is a lot of non-believers out there!

I have experienced the exact same results as @evoheyax and @Namasaki except on 6s setup.  Started with 6s lipo, moved to 6s lion for safety.  Realized I need a crap load more amps on the lion.  Everything they've experience with range, sag, etc I've also encountered. Probably won't move back to lipo like these guys did, but will just build packs with more cells in parallel and might try using A123s as well.
```

---
## \#81 Posted by: Pantologist Posted at: 2016-12-16T19:18:59.858Z Reads: 127

```
The best middle ground between Li-ion and Lipo is LiFePO4 cells. 

A123s can do 70A continuously and 120A pulse. A 12S2P pack would be perfect. 38.4V nominal and 140A continuous discharge. 5000mAh is nothing special but it would be fine for most people. Guessing around 8 miles range.
```

---
## \#82 Posted by: Namasaki Posted at: 2016-12-16T21:13:34.919Z Reads: 125

```
I haven't personally tried A123's but judging by there specs, they look like a better alternative than Li-ions
```

---
## \#83 Posted by: Pantologist Posted at: 2016-12-16T21:38:00.649Z Reads: 125

```
Boosted uses them and I also made a Boosted spec pack. I am not 100% sure about voltage sag but it still sagged a bit on hard acceleration but it was never an issue going up hills and such. 

To match lipo specs, 2P a123 cells would work.
```

---
## \#84 Posted by: johnny_261 Posted at: 2016-12-16T21:51:18.792Z Reads: 123

```
I'm want to try them, just hard to find a place to source legit ones for a reasonable price. This is one thing I hate about buying non-lipo batteries.  You never 100% know if you're going to get legit ones or some counterfeit stuff...
```

---
## \#85 Posted by: Pantologist Posted at: 2016-12-16T21:53:53.767Z Reads: 117

```
A123s are pretty easy to source. There are a bunch of overstock ones on eBay from accredited sellers.
```

---
## \#86 Posted by: Namasaki Posted at: 2016-12-16T21:54:16.410Z Reads: 114

```
Even my 300a Lipo pack sags a little. 
I don't know what it would take to eliminate sag completely.
```

---
## \#87 Posted by: johnny_261 Posted at: 2016-12-16T22:05:37.152Z Reads: 113

```
Do you have any sellers you can recommend?
```

---
## \#88 Posted by: PXSS Posted at: 2016-12-16T22:30:37.667Z Reads: 122

```
A 0ohm internal resistance cell that has a non thermal reaction. 

[quote="Namasaki, post:86, topic:14720, full:true"]
I don't know what it would take to eliminate sag completely.
[/quote]
```

---
## \#89 Posted by: PXSS Posted at: 2016-12-17T07:11:02.028Z Reads: 132

```
Here's a good example on how to mitigate voltage sag and under performance on a li-ion battery

Budget: $300
Options: 60 NCR18650GA, 44 Sony VTC6. (I get the 500+ discount since we buy a ton of batteries for work.)

Possible configuration:
10S6P GA with max continuous draw of 60A
11S4P VTC6 with max continuous draw of 120A or temp cutoff of 80c

1KW load assumed. 

1000/36v nominal / 6p = 4.62A/cell
Now I can use Henrik's website (Lygte) to find my actual nominal voltage at this power setting. 

At 5A continuous, nominal voltage is closer to 3.48V
1000/(34.8*6) = 4.79A/cell
So now we have nominal voltage and current draw for a continuous 1000W. 

At this power setting, the cells have 3.2Ah of capacity. So total energy can be measured by:
3.48v*3.2Ah*60cells = 668Wh. 

So I should be able to run roughly 40minutes at a constant 1000W. Which in reality is more like 35 (based on experience)

Same process can be done for the VTC6. 
1000W/(39.6*4) = 6.31A
@7A: nominal v= 3.58, capacity = 2.9Ah
1000W/(39.38*4) = 6.34A so we're being a little conservative by using the 7A curve. 
Total energy = 3.58*2.9*40 = 415Wh
Runtime @1000W: 25minutes.

So if you constantly pulled 1000W then the 10S6P would be the way to go as it has 50% more endurance. 

Here's the upside to the VTC6s though. Your max power draw is capped at 2000W pulling 10A/cell with the GAs. Using VTC6, your max power draw is capped at 3000W pulling 20A/cell. In other words 50% more power. 

So if you need endurance, 10S6P GA cells
If you want power 11S4P VTC6s. 
You can most likely pull more power from both cells for short periods of time, but it'll most likely harm the life of your pack, (300 cycles, 80% capacity)

The same trade study can be done with LiPos and I would have done an example but I dont have data in front of me rn. 

Cheers!
```

---
## \#90 Posted by: Okami Posted at: 2016-12-17T08:43:47.534Z Reads: 117

```
Good overview/calculations! 

Just proves if the power demand is not as high, to go with bigger capacity pack but with less max power available.

This again brings us to the ''calculation'' - prediction, on what the typical power demand might be in the situation - environment the eboard is gonna be used.
```

---
## \#91 Posted by: Pedrodemio Posted at: 2016-12-17T14:34:11.219Z Reads: 115

```
That part is pretty easy, for the air drag we can simplify and assume a 1m^2 frontal area and a 1Cd, and just calculate the torque on the wheel related to the grade and mass of the rider+board, the only factor missing is drivetrain and electric efficiency that can be guessed, or calculated using the motor parameters, but that is more complex, but the mechanical power/torque on the wheel that we need is easy
```

---
## \#92 Posted by: PXSS Posted at: 2016-12-17T14:40:41.590Z Reads: 115

```
I actually have the exact cd for a human standing, sitting, etc... (Dont ask, aerospace engineering stuff lol)
Will look it up when I get home
```

---
## \#93 Posted by: Okami Posted at: 2016-12-17T15:17:23.030Z Reads: 114

```
 [quote="Pedrodemio, post:91, topic:14720"]
for the air drag we can simplify and assume a 1m^2 frontal area and a 1Cd, and just calculate the torque on the wheel related to the grade and mass of the rider+board, the only factor missing is drivetrain and electric efficiency that can be guessed
[/quote]

If from this we come up with a realistic energy use - demand calculation that would be great!
Would make it possible to more realistically calculate max mileage, system max amps etc..
```

---
## \#94 Posted by: evoheyax Posted at: 2016-12-17T16:06:39.633Z Reads: 107

```
[quote="PXSS, post:71, topic:14720"]
I would suggest 60A as your max: you gain a good amount of endurance, increase life cycles and you can still pull 2000W avg.
[/quote]

But the raptor 2 can pull 120 amps with the Samsung 25r in a 10s4p (with manufacturers rating of 80 amp without impacting the cells life and you can still get 25 miles!!!!!

(Ps I'm being sarcastic)
```

---
## \#95 Posted by: Pedrodemio Posted at: 2016-12-17T16:30:14.550Z Reads: 115

```
[quote="PXSS, post:92, topic:14720, full:true"]
I actually have the exact cd for a human standing, sitting, etc... (Dont ask, aerospace engineering stuff lol)Will look it up when I get home
[/quote]

Nice, looking forward to it, i measure the frontal area in myself and was something like 0,7m^2, the cd i found various papers with modeling, but the numbers were far off from each other

[quote="Okami, post:93, topic:14720"]
If from this we come up with a realistic energy use - demand calculation that would be great!Would make it possible to more realistically calculate max mileage, system max amps etc..
[/quote]

If i have time i will plot it today so we can see whats happening
```

---
## \#96 Posted by: Ackmaniac Posted at: 2016-12-17T19:17:37.336Z Reads: 116

```
Just simply use my android app and make a video of it. There you can see the actual voltage, motor and battery amp draw, actual watts, speed and consumed, charged and average wh and ah. Then we can share the videos and have a much better picture what really happens to the VESC when we ride.

Here is a example how the video looks like then. this video is not modified. That is exactly the result you get. So you can record your ride and see the realtime data. You need a HM-10 bluetooth module for it which you can get here. 
https://de.aliexpress.com/item/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module/32516357718.html?spm=2114.13010608.0.0.cbyTeS&detailNewVersion=&categoryId=400103

If you want to switch change the motor amps configuration you need to flash the VESC with my firmware as well. But to only watch the realtime data the standard firmware works as well.


https://youtu.be/0y_CKa4OoKY

Available in the Google Play store

[App in Google Play Store](https://play.google.com/store/apps/details?id=ackmaniac.vescmonitor&hl=de)

or here

[Windows BLDC-Tool, Modified Firmware, Ubuntu BLDC-Tool and Android app](https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0)

More information you can read here.
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-and-individual-throttle-curve/12286
```

---
## \#97 Posted by: PXSS Posted at: 2016-12-17T19:27:00.566Z Reads: 113

```
Experimenting only gets you so far if you don't understand the math/physics. You cannot get a full picture without understanding. Different setups with different sized people and different riding conditions should be taken into account and unless we have a model to explain things, you might as well just guess.

This is just the way I was taught to approach an engineering problem.

Edit: You'd need a dyno to run an accurate experiment the way you show your video to get any relevant data. 

It is pretty cool though
```

---
## \#98 Posted by: Ackmaniac Posted at: 2016-12-17T19:59:39.870Z Reads: 113

```
The good thing is you get the exact data for your board. So it helps to analyse and understand your own board. And you can also see how much of your time you are really drawing max or high amps. And i guess the most will be surprised. 
Another great thing is that we can also see the VESC max min motor and battery settings in the video.
But that only works with my firmware.
```

---
## \#99 Posted by: PXSS Posted at: 2016-12-18T04:18:57.332Z Reads: 113

```
Will give it a go next week once the build is completed
```

---
## \#100 Posted by: Jebe Posted at: 2016-12-18T04:47:13.775Z Reads: 113

```
18650 GA's
```

---
## \#101 Posted by: NNGG Posted at: 2016-12-18T08:17:22.295Z Reads: 108

```
haha I went prone on my speed run for 12S. I beat physics
```

---
## \#102 Posted by: PXSS Posted at: 2016-12-18T11:23:51.512Z Reads: 110

```
I think you mean you proved physics if you ended up face down on the concrete :yum:
```

---
## \#103 Posted by: Pedrodemio Posted at: 2016-12-19T01:53:45.754Z Reads: 111

```
@PXSS did you managed to find the Cd for a person? Here it is using a 0.9Cd (Wikipedia value for a general cyclist) and a frontal area of 0.65 m^2 that i found in a paper, when i have time i will take a picture of myself on the board and measure it

Most important, this is mechanical power on the wheels, not the power your VESC on power meter shows, no losses are being taken into account 

<img src="/uploads/db1493/original/3X/0/b/0bd34e5faf5f604ae9ab59c2304402181839be33.jpg" width="690" height="339">

Edit: i think i messed up something on the torque calculation, i will look into it latter

Edit2: found it, i forgot to convert the speed to m/s, now it makes sense
```

---
## \#104 Posted by: PXSS Posted at: 2016-12-19T02:24:15.041Z Reads: 104

```
I went to the office and completely forgot to look it up in my aero book. There is a pretty big difference between standing person and cyclists as they do whatever is possible to reduce drag
```

---
## \#105 Posted by: Pedrodemio Posted at: 2016-12-19T02:26:59.277Z Reads: 107

```
I agree, on another paper I found the Cd of a standing person to be 0.6, but on our case is a twisted standing up, anybody have a wind tunnel laying arround?:laughing:
```

---
## \#106 Posted by: PXSS Posted at: 2016-12-19T02:32:15.782Z Reads: 108

```
I'll make a note to look at it first thing in the AM. 
You can assume 1.2, it'll be something like that. 

@Pedrodemio: between 1.0-1.3 based on size. The reference was a 5'9" 180lbs male. 
FIY: you can lose 10% drag by losing your clothes... ;-)
```

---
## \#107 Posted by: Okami Posted at: 2017-01-15T03:36:40.368Z Reads: 102

```
@Pedrodemio Could you post a bit more detailed graphs - with smaller units ?

I would like to take a look at torque needed and also exact power (watts) needed at certain speeds..

As it is a picture format, I dont feel very confident to try draw some lines and tell is it 300w or 400w..

--
Other than that - I think this is pretty cool topic with lots of valuable info.. so sorry for bringing it up once again ( :D ) 

I might actually draw out a few quotes / texts out of this topic and insert - make a new topic about batteries in general.
```

---
## \#108 Posted by: Pedrodemio Posted at: 2017-01-15T13:28:56.923Z Reads: 96

```
Sure, as soon I get home I'll plot them

What range you would like? 10% max grade should provide a clearer picture
```

---
## \#109 Posted by: Okami Posted at: 2017-01-15T14:22:05.005Z Reads: 97

```
Yes, the flat, 5, 10, 15% values might be good to see more clearly :)
```

---
## \#110 Posted by: Pedrodemio Posted at: 2017-01-15T23:51:23.992Z Reads: 91

```
<img src="/uploads/db1493/original/3X/7/b/7ba935a70a9ec7b21957403a63a8ed65e5fb6966.jpg" width="690" height="339">
```

---
## \#111 Posted by: Ackmaniac Posted at: 2017-01-16T00:06:21.818Z Reads: 94

```
@Pedrodemio Very nice. One remark i have is that it would be nice to have the acceleration not in m/s. Better would be the speed gain per second. This way it would be easier to understand it.
So 1m/s² would mean that we are 3,6 km/h faster each second. So after one second we reached 3,6 km/h , after 2 seconds 7,2 km/h and so on.
```

---
## \#112 Posted by: Pedrodemio Posted at: 2017-01-16T02:02:56.611Z Reads: 95

```
I will do that if makes easier to understand

Next step will be to model rolling resistance and no load motor power and belt drag, the last two is gonna be a little more complicated since I have to design and assembly a dyno for it and the results will be exclusive for my board setup
```

---
## \#113 Posted by: Ackmaniac Posted at: 2017-01-16T02:13:30.376Z Reads: 96

```
To have a very precise reading you can reduce your boards power to exactly 250 watts or 300 watts. Find very flat track and see how fast you can go with that power. Then it is easy to use that for calculations.
It is nice to know the exact power that is needed for a specific speed. But in the real world we want to know to which watts we have to adjust the VESC to reach those speeds. Because then also motor efficiency comes into place. Means we know what goes in the motor but we don't know what comes out exactly. 

With 300 watts at the vesc I get around 31 km/h on flat ground. But I have to test that again because I never did a precise test run.
```

---
## \#114 Posted by: Pedrodemio Posted at: 2017-01-16T03:04:14.457Z Reads: 96

```
That's one way to do it, I just need a way to get real time data, my next remote might sold this with a screen. My only fear is that I will pay more attention to the screen that on the road :grin:
```

---
