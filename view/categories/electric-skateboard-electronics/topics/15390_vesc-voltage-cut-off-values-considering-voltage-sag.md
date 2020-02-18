# VESC voltage cut-off values considering voltage sag

### Replies: 60 Views: 4395

## \#1 Posted by: Maxid Posted at: 2016-12-30T14:09:15.966Z Reads: 391

```
I rode my dual-VESC board today which has a 10S3P battery made out of Samsung 25R cells.
The cut-off values are set to start at 35V and end at 33V - I chose those values to keep my cells healthy and happy (I also charge to just 4.1V per cell instead of 4.2V).
However I noticed some serious performance loss climbing a hill because of the voltage sag driving my cells almost down to 3.3V.
What kind of values are you guys using so that the performance stays usable while not hurting the cells too much?
@whitepony @Ackmaniac maybe you can help out here?

<img src="/uploads/db1493/original/3X/4/7/47d0bdadd2e1c6740d3fc4dee8631e6e4f3aa5a8.png" width="690" height="426">

When charging the battery received only ~4500mAh until being fully charged back to 41V. So there must have been quite some juice left.
```

---
## \#2 Posted by: Ackmaniac Posted at: 2016-12-30T14:18:39.734Z Reads: 355

```
Your cells are rated to 2.5V as cutoff voltage. But from 2.8V to 2.5V they go down rapidly. So i would recommend to set the cutoff start to 30V (3.0V a cell) and the cutoff end to 28V (2.8V) a cell. And just handle them normally and have fun. It think it is not worth to save some cell life to get some more charge cycles. If you think you will do more than 10000 km with this battery then it is OK. Otherwise i wouldn't care. People are always scared about their batterys instead of heaving fun with them.
And in your graph i can see that you only use like 18 amps in maximum on the battery for each VESC. So that is 36A in total. Your pack would be good for 60A. So you are not even pushing the limits.
I only would keep the voltage at 3.85V a cell when i want to store them for a long time. Otherwise you should enjoy them instead of being worried all the time.
```

---
## \#3 Posted by: PXSS Posted at: 2016-12-30T14:20:52.100Z Reads: 345

```
here's the curve for 15A. 
<img src="/uploads/db1493/original/3X/2/2/22fdcd3c546c208005c0aa045666cb955d1876f7.PNG" width="690" height="387">

So yeah, at 33v youre using almost %50 capacity. I would set it to 3.1v and 2.8v. At 3.1V you still have 10% left. And if you stop them at 2.8v you will keep them plenty happy since they go down to 2.5v

E: 15A/cell. Translates to 45A at the battery. So this is a little conservative but there's no graph between 10 and 15 online. 

Graph for 10A/cell
<img src="/uploads/db1493/original/3X/2/f/2f5ee509bc39c07895bae870c9453c22e5e1971e.PNG" width="690" height="387">
```

---
## \#4 Posted by: whitepony Posted at: 2016-12-30T15:22:30.100Z Reads: 290

```
there is something else going on, this is not normal sag! using a loop key? spin up the motor without load and check live monitoring. i had a very similar problem with my melting loop key on the trampa the moment strong currents were flowing. i bet something in your setup is getting really warm :grinning:
```

---
## \#5 Posted by: Maxid Posted at: 2016-12-30T15:24:06.515Z Reads: 280

```
I am using a Vedder Antispark Switch with a 40A fuse. Battery current is set to 20A in each VESC and Motor current set to the recommended value by Jacob (40A per Motor).
```

---
## \#6 Posted by: whitepony Posted at: 2016-12-30T15:25:38.307Z Reads: 272

```
this is not voltage sag, reduce your setup to an always on direct connection to vesc and try it again!

that aside, my settings are soft off 33V, hard off 30V! I have next to no sag with lg hg2!
```

---
## \#7 Posted by: Maxid Posted at: 2016-12-30T15:27:07.358Z Reads: 272

```
How can I try this again when this was while going uphill? And what should I look for in the no load scenario?
```

---
## \#8 Posted by: whitepony Posted at: 2016-12-30T15:28:30.120Z Reads: 263

```
just try revving your motors on your desk while vesc is hooked to your comp - i could see that melting loop key voltage sag the moment a stronger current started flowing (in the vesc voltage live monitor)! a normal setup wouldnt show any sag in that scenario. if you cant reproduce that issue on your desk, rule out uneccessary components like the vedder switch -> always on direct connection vesc to battery.
```

---
## \#9 Posted by: Maxid Posted at: 2016-12-30T16:40:26.321Z Reads: 262

```
Ok I opened it up with the limited tools I have right now (I am at the parents in law over christmas and new years).
I cannot connect the VESC directly to the battery because they use different connectors (VESC XT60, Battery 4mm female bullet) and I don't have the equipment needed - not even a Multimeter :scream:
I noticed however that the ground bullet connector was not inserted all the way - seems like the vibrations might have loosened it. 
This is before opening it - the slow increase in voltage worried me a lot.
<img src="/uploads/db1493/original/3X/a/0/a033c086785edf8f80e58e7be0f0de7f883c07fe.png" width="690" height="444">

After pushing the bullet connector in all the way again:
<img src="/uploads/db1493/original/3X/b/5/b52f5e6799fed627f67e2ced9715dd32f8dc1517.png" width="690" height="414">

Would love to test it now but it is already dark and freezing cold :cry:
```

---
## \#10 Posted by: whitepony Posted at: 2016-12-30T16:55:57.890Z Reads: 225

```
that was the problem in another melting loop key thread!
```

---
## \#11 Posted by: PXSS Posted at: 2016-12-30T17:18:20.756Z Reads: 244

```
LG HG2 are significantly better at handling voltage sag than 25Rs. Here's the comparison. 

10A/cell
<img src="/uploads/db1493/original/3X/1/1/111e5c386e2034b6423552392913b5f3cf98507a.PNG" width="690" height="387">

15A/cell
<img src="/uploads/db1493/original/3X/c/0/c08cab7c66e6b97466099cc9218fe351b7e2998f.PNG" width="690" height="387">

So although the cause may have been a bad connector acting as a fuse. The voltage sag on his setup is real.
```

---
## \#12 Posted by: evoheyax Posted at: 2016-12-30T18:20:40.298Z Reads: 231

```
And again, this is why I've gone back to lipos. Li-ion cells sag a lot. You need a massive pack to get rid of sag. As a result of sag, you end up getting less range, along with stressing your cells more. An HG2 at 20 amp continuous and going up to 100% and close to 0% will only get 400 charge cycles. Obviously, your not pulling that all of the time, but it will have an impact on the cells life. Instead of the 1500 cycles, I have had about 150 charge cycles and have experienced quite a bit of decreased capacity.

Until a better battery technology emerges, we are stuck with either less safe batteries (lipos) or lots of sag (li-ion).

There will always be out liars that don't have problems. Likely due to the fact they are light, and ride up little to no hills. You can't deny though that wen I climb a 20% grade hill, I pull 80 amps+ on a 12s4p. I sag a lot, and I could have predicted this by just looking at the 20 amp discharge curve of the cell.
```

---
## \#13 Posted by: Ackmaniac Posted at: 2016-12-30T19:02:15.286Z Reads: 229

```
**you end up getting less range** -> you need to get the cutoff right. Watt hours are watt hours. Doesn't matter if Li-Ion or LiPo. As far as i know you did set the cutoff to 3.3V for each cell which is too high and a result of my first post of this thread.
**stressing your cells more** -> You don't stress the cells more because that is what they are build for.
**will only get 400 charge cycles** -> that is roughly 10000km for a 10S4P

The only difference will be your max power output compared to a Li-Ion and the max speed because of the motors kv which depend on the voltage..

So at 80 amps under load for a 10S4P this would be 20A for each cell.

**Fully charged Li-Ion** can handle 3,7V at 20A load:
3,7V (cell under load) * 10S * 80A = 2960 Watts

**Fully charged Li-Po** can handle 3,9V at 20A load:
3,9V (cell under load) * 10S * 80A = 3120 Watts      (160 watts more)

**Close to empty Li-Ion**, so that we reach the voltage cutoff for the VESC at 2,8V:
2,8V (cell under load) * 10S * 80A = 2240 Watts

**Close to empty Li-Po**, so that we reach the voltage cutoff for the VESC at 3,3V:
3,3V (cell under load) * 10S * 80A = 2640 Watts      (400 watts more)


So the the LiPo Batterys can deliver more power at different discharge levels. But that's it. So if you only want to blast up the steepest hills then it makes sense. But i think many people don't even get close to those watts.
And if the cutoff end is set wrong for Li-Ion cells (like 3.3V) then you reduce the battery to half of what it would be capable. So 2.8V would be right.
```

---
## \#14 Posted by: Maxid Posted at: 2016-12-30T19:10:53.959Z Reads: 220

```
your post looks like an answer to @evoheyax post - not mine.
I was the one using 3.3V as cut-off though - not him.
```

---
## \#15 Posted by: Ackmaniac Posted at: 2016-12-30T19:16:33.983Z Reads: 219

```
We had this discussion before and found out that he also set this value as the cutoff. Sorry to use this thread here for that but i want to avoid that the myth gets created that the Li-Ion cells are not good. 

Most people who say there Li-Ion cells perform badly just simply had the wrong settings. You just simply need to get the settings right with the cutoff start and end and then the Li-Ion cells work great. 

Lipos can do a bit better but they are more dangerous and you need more knowledge about them. If you know what you do then it is fine. But if you don't stay away from them.
```

---
## \#16 Posted by: Maxid Posted at: 2016-12-30T19:29:04.676Z Reads: 212

```
It's cool - just thought you confused him with me.
```

---
## \#17 Posted by: Esrapp21 Posted at: 2016-12-30T19:31:24.571Z Reads: 219

```
How are LiFePO cells with voltage sag? I just ordered a space cell.
```

---
## \#18 Posted by: Maxid Posted at: 2016-12-30T19:32:50.291Z Reads: 222

```
Space cells are not lifepo but liion afaik. They even use the exact same cell as I am (samsung 25r). I think it depends on the cell just like with liion. A123 cells for example are good for 70A - so will also have low sag.
```

---
## \#19 Posted by: evoheyax Posted at: 2016-12-30T19:33:23.548Z Reads: 228

```
Sorry, I don't mean to hijack your thread.

Just to clear things up, I used to have no low power cutoff. I ran them till I sagged and my lcd Volt meters turned off under sag (they bounce back up to 3.2 or so after the load is removed). I still had shitty range (and less than my smaller lipos). My point is with liion, you can't get the cells down to 2.8 when there's no load. When your at 3.3 or 3.2, under heavy load, they sag down to 2.8 instantly. My point exactly is that they can sag so badly, that you can't even use half of the battery. Yes, it's normal for li-ion to sag like this, the charts tell it all. But this amount of sag is not ideal for heavier guys who live in a hilly area. It's so unfavorable that I call it a problem, because I can't sell a board to the community with a battery that performs like this.

What other settings would I have wrong? I could lower my max amps from the battery more, but then I'll stall on steeper hills (or go up at 10 mph).
```

---
## \#20 Posted by: Esrapp21 Posted at: 2016-12-30T19:35:51.854Z Reads: 214

```
Wait, in the enertion website, on the SPACE cell 3 page, it says **Battery Chemistry: LiNiCoMnP**
```

---
## \#21 Posted by: Maxid Posted at: 2016-12-30T19:39:22.769Z Reads: 208

```
That is not lifepo but Samsung 25Rs
```

---
## \#22 Posted by: Ackmaniac Posted at: 2016-12-30T19:45:54.407Z Reads: 207

```
The Samsung 25R can deliver 20A until the cutoff of 2.8V till 2.25 mah. That means for 90% of it's capacity it can deliver 20A. Sounds good to me.

<img src="/uploads/db1493/original/3X/c/5/c521262bcffd9cf04ea35b00b87b44f2b5d9c98f.png" width="690" height="386">
```

---
## \#23 Posted by: Esrapp21 Posted at: 2016-12-30T20:00:48.556Z Reads: 198

```
Got it. Thanks!
```

---
## \#24 Posted by: evoheyax Posted at: 2016-12-30T20:00:49.819Z Reads: 198

```
So when your cells hit the cutoff at 2.8, what is the voltage of your cell after you stop the discharge?

I would say maybe I've messed up with my battery, which is causing the sagging numbers and poor range numbers, but I had these issues before with the space cell. I had the 10s3p space cell, and I was lucky to get 4 miles on my route (had to be very conservative with the throttle and run stop signs when possible). You logic there seems good, but it the real world, I had very different results...
```

---
## \#25 Posted by: Ackmaniac Posted at: 2016-12-30T20:02:42.877Z Reads: 192

```
Of course it jumps back. But the shown discharge curve is under load.
```

---
## \#26 Posted by: evoheyax Posted at: 2016-12-30T20:10:13.000Z Reads: 187

```
What is your theory than for my poor range?

I could get 4 miles with a 10s3p and 6 miles with a 12s4p (LG HE2's). The calculations I did sowed I should in theory get 4 times this.

The most likely cause would be fake cells, but I would expect the space cell to have legit cells..
```

---
## \#27 Posted by: PXSS Posted at: 2016-12-30T20:19:36.407Z Reads: 182

```
I think we need a battery selection/technoly/voltage sag guide thread. I think we all agree on some basic points but all the thread jumping is making the info hard to find.
```

---
## \#28 Posted by: Ackmaniac Posted at: 2016-12-30T20:22:48.037Z Reads: 177

```
Thought you mentioned before that you set the cutoff end to 3.3 or 3.2V because we had this discussion already. Maybe you should do a little test when you find the time. You also have a app to show the data in a video. 
I would recommend to show a video with Lipos and Li-Ions on the same board with the same setup but of course correct voltage cutoffs. Would be very interesting.
```

---
## \#29 Posted by: PXSS Posted at: 2016-12-30T20:22:50.259Z Reads: 171

```
@Ackmaniac. You are wrong in your watt hour calculation. At 20A your average voltage is NOT 3.7v on the samsung 25r. It's more like 3.1v. Look at the discharge curve. Do your math with that number and you'll see why @evoheyax gets crap range from his cell.
```

---
## \#30 Posted by: PXSS Posted at: 2016-12-30T20:33:42.975Z Reads: 173

```
From the voltage sag thread a few weeks ago...

<quote>
Total Energy content varies with how hard you push, push 1A on a 10A cell and you get ~12.6Wh of energy. Push 7A on that same cell and your total energy drops to ~10.75Wh. 
If you have a 40cell battery in ANY configuration (1s40p or 10s4p don't matter) and you're drawing an average of 1000W, you just lost at the very least 14.7% of your range this is because your performance differs when you get on the board to halfway through your ride to towards the end of your ride, to draw 1000W at 3.8V/cell it takes 6.6A/cell, at 50% and 3.44V/cell it takes 7.27A/cell and towards the tail end at 3.0V/cell it takes 8.33A/cell So you can see how 14.7% is lost is really conservative.
Now if you have a lipo with the same rated capacity at the same nominal voltage and a 60c discharge rating your voltage sag is non existent and your discharge curve is pretty flat which means your battery energy doesn't change regardless of how much power you draw.

So yes, hills do reduce range. Same as a car.
</quote>
```

---
## \#31 Posted by: Ackmaniac Posted at: 2016-12-30T20:38:31.267Z Reads: 165

```
And what happens when you discharge the cell with 20A continious, and once you reached the 2.8V then you continue with only 1A. How much Wh do you get then from the cell?
```

---
## \#32 Posted by: PXSS Posted at: 2016-12-30T20:51:08.494Z Reads: 168

```
That is an unrealistic scenario but sure, I'll bite.

Scenario
10s4p samsung 25r pack on a quad drive, that pulls 80A total on a hill, you discharged till 2.8 but then it's flat home and you can cruise at 4A...

Here are both curves on a per cell basis...
<img src="/uploads/db1493/original/3X/1/d/1dc48aa2ac6f7b7972f4bcd13bd5a343ba58e4e5.PNG" width="690" height="387">

You ride at 20A until you reach 2.8v.
Average voltage: 3.1v
Total Ah: 2.2
Total energy used: 6.82Wh/cell

Continue riding at 1A until 2.8V again.
Average voltage: 3.1v
Total Ah: 2.45-2.2 = 0.25Ah
Total energy used: 0.775Wh

Sum of energy used: 7.595Wh/cell
Times 40 cells: 303Wh

"Rated" = 40*3.6*2.5 = 360Wh

You lost 16% of your rated energy by running at 20A continuous.
```

---
## \#33 Posted by: Ackmaniac Posted at: 2016-12-30T21:12:42.304Z Reads: 154

```
Very nice. Now we get closer. A realistic average discharge rating for a average ride would be around 16A (4A a cell on 4P) in total. That is more than 500 watts on average which is quite high. Can you do the Wh Calc please for that.

If I am not wrong it should somewhere around 3.6V * 2.45A * 40 = 352Wh
Sounds good to me.  Of course you have some bursts with 20A but we are very far away from 20A continuously.
```

---
## \#34 Posted by: evoheyax Posted at: 2016-12-30T21:27:43.550Z Reads: 157

```
[quote="Ackmaniac, post:33, topic:15390"]
A realistic average discharge rating for a average ride would be around 16A (4A a cell on 4P) in total
[/quote]

Problem with average is, average for who? Since we are all using different motors and configurations, are different weights, and ride in different environments, there is no average discharge. This is why I focus more on max discharge. If it works well in the harshest of conditions, than its good.

Even calculating average amps is tricky, because how do you calculate it with real world data? I ping the vesc every .25 seconds, so I just add them all up and divide by however many amp data points I have. This is bad though, because I factor in the times when I'm not moving. so say I have 10 10 0 15 8 8 0 0 0 0 4 as your amp data points, that would be 55/11 = 5 amps average. But that's not a good indication because while pulling 0 amps, I likely was not moving, so It shouldn't be counted. If I leave the zeros out, that's 55/6 = 9.166, which is more accurate. So how you calcualte average amps even could skew your numbers.
```

---
## \#35 Posted by: PXSS Posted at: 2016-12-30T21:33:59.376Z Reads: 144

```
Load up his custom vesc firmware or attach a wattmeter in line and find out what your average power draw is. I'm sure we can get you to give up lipos :wink: :wink:
```

---
## \#36 Posted by: Ackmaniac Posted at: 2016-12-30T21:37:32.553Z Reads: 149

```
I can understand your statement. But your board is something I would definitely not call average. For me the average rider is 80 kg with clothes and the board has a max speed of 45 km/h. And there are some hills in the area. But of course not like in SF. And 500 watts average would already be a average speed above 30km/h. And I don't think many of us even ride that speed on average.
So I think that those values are not bad when it comes to the average rider.
```

---
## \#37 Posted by: PXSS Posted at: 2016-12-30T21:39:37.494Z Reads: 145

```
(3.55v * 2.125ah + 3v * .25ah) * 40 = 331.75Wh ish
```

---
## \#38 Posted by: PXSS Posted at: 2016-12-30T21:43:25.648Z Reads: 145

```
You cant really relate average power to average speed as that is truly dependent on road conditions, rider's weight, gear ratio, etc.

Why do I feel like we are repeating the same conversation from 2 weeks ago? Lol
```

---
## \#39 Posted by: evoheyax Posted at: 2016-12-30T21:45:55.768Z Reads: 142

```
I'm working on some new data points for my app. I'll be able to give you more info about my board soon that should explain more. I'm mostly curious as to how many Wh I actually get from my 12s4p li-ion battery.
```

---
## \#40 Posted by: PXSS Posted at: 2016-12-30T21:45:57.873Z Reads: 139

```
San Francisco hills are crazy though. I see why you run LiPos... @evoheyax. You could probably get away with a liion pack but it would be extremely expensive, although if you solve the power issue, you could be looking at twice the range as your lipo counterpart.

Give me numbers and I'll get you a solution.
```

---
## \#41 Posted by: evoheyax Posted at: 2016-12-30T21:48:07.892Z Reads: 129

```
I honestly like li-ions better. Really, I would want to pull no more than 15 amps, and to do that, I need a 12s6p, which I just can't fit onto my board and keep some amount of thin appearance.

@PXSS what numbers do you want?
```

---
## \#42 Posted by: PXSS Posted at: 2016-12-30T21:53:51.605Z Reads: 129

```
Find out your max power draw and average power draw on the board you ride with LiPos. I'll get you a configuration that won't sag too bad. 

How many cells can you fit?
E: PM me or start another thread, I feel like we're hijacking @Maxid's thread lol
```

---
## \#43 Posted by: Maxid Posted at: 2016-12-30T22:19:33.386Z Reads: 131

```
It's cool. We solved my issue (at least so far) and are talking battery technology now - i am all for that.  We should just make sure to make all the information public somehow instead of "hiding" it in here
```

---
## \#44 Posted by: PXSS Posted at: 2016-12-31T14:10:39.997Z Reads: 129

```
I started doing an excel calculator late last night that will hopefully solve the power requirement guessing. So far I can estimate the drag force from a standing human and the rolling resistance of our wheels on asphalt. I need some help from you guys to verify my numbers for rolling resistance, on a nonpowered board have someone tow you while each of you hold to different sides of a fish scale to measure the force required to tow, (I attached a rope to a door and pulled myself... i have no friends :sweat: jk). Either way, if you can give me your total weight incl board and pull force, then I can fine tune the rollimg constant. 

Now I need to figure out the mechanical torque equations... Does anyone have no load data? I need voltage, rpm, current, and power draw vs time. 
(I'd do it myself but I still haven't finished my build)
```

---
## \#45 Posted by: Ackmaniac Posted at: 2016-12-31T15:01:15.031Z Reads: 132

```
Maybe this video helps. I was trying to make a constant ride with the cruise control at 25 km/h. But you can't compare the voltage sag here with proper high discharge Li-Ion cells because i ride with Laptop Cells which are not made for that. But they do the job. But of course the voltage sag is really high with them.

https://youtu.be/Y2RGmAlJJy8
```

---
## \#46 Posted by: PXSS Posted at: 2016-12-31T16:14:28.074Z Reads: 131

```
Have you ridden your board yet??
Was it fixed?
```

---
## \#47 Posted by: Maxid Posted at: 2016-12-31T16:33:41.329Z Reads: 127

```
I tried but could not ride long due to cold temperatures. At -4°C it is not a lot of fun to ride - also to see those levels of discharge I would have to first use up quite some battery after charging it yesterday. I changed the cut offs though - will get back to you guys once I have some graphs again.
```

---
## \#48 Posted by: PXSS Posted at: 2016-12-31T16:41:14.326Z Reads: 125

```
And your battery performance is also greatly diminished at those temperatures.
```

---
## \#49 Posted by: Ackmaniac Posted at: 2016-12-31T16:52:41.629Z Reads: 126

```
I think that is no problem when you keep the board inside your house and go directly out for a ride. So they will be at room temperatur when you start and during the ride they get a little temperature by being used. You only shouldn't let them cool down.
```

---
## \#50 Posted by: Ackmaniac Posted at: 2016-12-31T17:14:18.631Z Reads: 129

```
Here is also another video with the same round but this time with lots of accelerating and braking. When you compare the used Wh with the previous video then i used roughly 70 % more. It always looks so slow on the videos.:joy:

https://youtu.be/jmV2Q9WTbGk
Video was made with my Android app so everybody can make his own video. Just check for my other thread if your interested.
```

---
## \#51 Posted by: Kaden56 Posted at: 2017-01-01T07:21:29.131Z Reads: 124

```
[quote="evoheyax, post:26, topic:15390"]
I could get 4 miles with a 10s3p and 6 miles with a 12s4p
[/quote]

You were really only getting that kind of millage? That seems like something was wrong. I haven't messed with my vesc setting much at all and got a pretty easy 15 miles on my 10s4p the other day, and I wasn't being very conservative on accelerating or speed. However only two large hills in that time and no head wind. I do weigh 190lbs though and my board is about 45 lbs.
```

---
## \#52 Posted by: evoheyax Posted at: 2017-01-01T17:53:59.429Z Reads: 119

```
Yea, I live in a very hilly area. Most of my riding is either up or down a hill around 11% grade. And regen braking doesn't replace all of the power needed to get me up the hill, just a bit. I run hubs though, which explain some of that lost range. Generally, hubs need a lot more power.
```

---
## \#53 Posted by: wmj259 Posted at: 2017-01-01T18:10:30.438Z Reads: 119

```
Good info here.
```

---
## \#54 Posted by: Hummie Posted at: 2017-01-01T18:13:08.712Z Reads: 117

```
I think hubs need more power to create torque but maybe hubs could be more efficient on continuous flats.  Will see soon.  Anyone near SF with a pulley set-up who wants to come out and compare this week?
```

---
## \#55 Posted by: Kaden56 Posted at: 2017-01-01T19:54:31.947Z Reads: 116

```
Ok that makes a lot more sense! If hub motors were more effecient they would totally monopolize the market. It would be so nice to now have a separate motor, mounts, pulley/sprocket, belt/chain. Lots of weight, room, and build time saved. Potentially money too!
```

---
## \#56 Posted by: evoheyax Posted at: 2017-01-01T21:15:04.746Z Reads: 114

```
To me, it's a trade off well worth it.
```

---
## \#57 Posted by: cliofreak Posted at: 2018-02-22T22:57:47.685Z Reads: 59

```
Hey,

I have serious voltage sag when going up medium hill and pretty much just stops on steeper inclines.
Im running 10s4p 30Qs with Vesc and 6374 200KV motor.

I think it might be because Ive got conservative settings in my Vesc but I could be wrong. Here is a bit of a screen grab from the Metr app. Any ideas whats going on!?

When I pushed it up the same hill for 20 secs then jumped on and gave it power, it starting pulling really well… for about 15secs then starting bogging again.

These readings are from a 15min ride with some flat areas and down hill in parts too. The last 5 mins was a significant hill but I felt the bogging even on a slight incline.![08|690x116](upload://sAEnFxE8Xyb6DQEIlBUhoBdwi1l.png)![59|690x86](upload://jYAwql3bKLHKcOayzHh2IJpQnD6.png)
```

---
## \#58 Posted by: PXSS Posted at: 2018-02-22T23:54:40.908Z Reads: 58

```
Can you upload the whole log from the metr app?
Also post your VESC settings, we can't point to what is causing the issue without those :)

It looks like your ESC is might be overheating. 78A is pretty hot. I think the foldback starts at 80C so maybe not.

I don't think you are having voltage sag issues since your battery is nore than capable of providing 60A continuous. Something else is wrong
```

---
## \#59 Posted by: cliofreak Posted at: 2018-02-23T00:02:39.186Z Reads: 58

```
![IMG_0187|230x500](upload://kAdy6Q9lC77pzJPaFscZm1WlSTL.jpg)![IMG_0185|230x500](upload://rsZZ5qdyHHzd9seoWWNnK7WGM3W.jpg)![IMG_0184|230x500](upload://kBX1k8ul8WMZv3ARNyQ9HHFGcmv.jpg)![IMG_0186|230x500](upload://Jpv5GPUcZyBaQlMesknfyXgM5t.jpg)
```

---
## \#60 Posted by: PXSS Posted at: 2018-02-23T00:04:10.801Z Reads: 56

```
Lets move over to the other thread... I was already commenting on your settings there. Please try to keep your comments contained to a single thread for one problem unless nobody replies for a day or so :)
```

---
