# Wiring and charging advice please

### Replies: 43 Views: 2027

## \#1 Posted by: riva_00 Posted at: 2017-07-05T12:25:27.175Z Reads: 177

```
All,

Can I get a bit of advice?
I've just bought 6 5s LiPo batteries and plan to buy a BMS, hopefully this one: -
https://www.electric-skateboard.builders/t/diebie-jtag-12s-bms-gauging-interest-nonprofit/20947

I'm not fantastic at electrical circuitry, so i'm playing it safe and posting how I'm going to do it here.
Below is how i'd like it: -
<img src="/uploads/db1493/original/3X/7/9/79a1a941b2672d665824a625ede4f84f534d4572.png" width="595" height="500">

Can anyone see any issues with it?

My real question is about the charger. As up until now I've balanced charged my previous 2 6S batteries every time, but now that I've almost tripled my WH, I need a temporary easier solution.
Until I get the BMS wired in, which'll be in a month or so I'm guessing, I'd like to charge using just a basic charger that lobs power back into the circuit.
Ideally I'd like one that just charged to 41V (for safety and battery health), but can't find one that'll do this, could anyone recommend a good charger that allows voltage adjustment?

*Could i use the Imax B6 charger?

Thanks for all replies :slight_smile:
```

---
## \#2 Posted by: Maxid Posted at: 2017-07-05T13:04:55.645Z Reads: 151

```
You have Lipos - they should be balanced everytime!
Also that BMS will not help much as you have parallel packs.
Ideally you would balance each pack individually and not in a parallel config.
```

---
## \#3 Posted by: riva_00 Posted at: 2017-07-05T14:13:31.916Z Reads: 143

```
@Maxid I don't like that answer, give me another one :slight_smile:

Best practice dictates that I stay near the charger and balance charge them one by one. Seeing as that would take about 7 hours charging at about 3.5A I'm not that keen.
I like to charge at a relatively low amperage, and to max 4.1V per cell. I'd also check their balance after every charge (I have a nifty portable balance check thingy) which I think is pretty safe practice..

I've got no choice with the BMS parallel charging, there's no better alternative (at least to my knowledge), but again i'd only charge to 4.1V and discharge to 3.55ish.
```

---
## \#4 Posted by: Maxid Posted at: 2017-07-05T14:15:32.294Z Reads: 136

```
well it also will be a pain to set up as you will have to connect the balance wires to the BMS in parallel.
Make sure to double and triple check polarity.
I already plugged my two 3S balancer cables together the wrong way - big spark but luckily nothing broke.
```

---
## \#5 Posted by: riva_00 Posted at: 2017-07-05T19:22:18.549Z Reads: 128

```
Shouldn't be difficult to set it up in parallel, and I'd only have to do it once then I'd (hopefully) be set for a long time.
Thing is, in theory should it work? I hope so.

Most lipo/li-ion balance charging threads I've read say that connecting batteries in parallel will balance them to a point. I'm thinking that if I check balances after every charge, only charge to 41V and occasionally balance charge (1 in 5 or 7 charges) I should be fine.
I'm also considering having 3 10s voltage displays on the side of the box. Largely useless but great for a control freak like me.

@Namasaki @longhairedboy @sl33py @whitepony (virtual tap on the shoulder for you all)
Please tell me Maxids being overly cautious, will my diagram and plan work?
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-07-05T19:34:20.306Z Reads: 112

```
he is not being overly cautious. It would be easy to make an alarmingly hot and vibrant mistake here. 

This is something i wouldn't even want to try. doing three series groups in parrallel... i'm not 100% but im' pretty sure involving a BMS here with parallel balance leads going to each pack in parrallel is going to cause a short.
```

---
## \#7 Posted by: sl33py Posted at: 2017-07-05T19:54:49.172Z Reads: 106

```
[quote="riva_00, post:5, topic:26839"]
only charge to 41V and occasionally balance charge (1 in 5 or 7 charges) I should be fine.
[/quote]


For Li-Ion sure, but for Lipo - i balance charge *every single time*.

I also like to pull and inspect them, and usually throw a thermal probe on them when charging so even if i'm not 100% paying attention it'll auto shut off before any thermal issue...

And lipos (or at least the inexpensive ones i have) *drift* **frequently** so should be _balanced every time_.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-07-05T20:13:04.895Z Reads: 103

```
I agree with @Maxid
Lipos should be balanced at every charge Cycle. 
Lipos are great for high power in a small package but, you better give them a healthy amount of respect.
```

---
## \#9 Posted by: riva_00 Posted at: 2017-07-05T20:20:18.609Z Reads: 101

```
So I'm going to get a darwin award then.......Least i have all you lot to help me live a bit longer.

@!£$^%.......So is it possible (and safe) to get a 500+ Wh Lipo pack? I'd settle for about 400Wh
Ideally one that isn't too fat, Either the width or height needs to be under 44mm so I can get it in a good case and be high enough off the ground.

Since I've bought 6 of these batteries I could just run 2 at a time I suppose.....Carry the rest in a backpack maybe. But that's not living the dream of having all connected and charging easily.

I could have 3 of these in series: -
https://hobbyking.com/en_us/multistar-high-capacity-4s-10000mah-multi-rotor-lipo-pack.html

Not the best C rating but the high capacity makes it un-necessary i think.

How would all you guys do it?
```

---
## \#10 Posted by: Namasaki Posted at: 2017-07-05T20:32:25.242Z Reads: 93

```
Others have tried those packs with poor results. 
The C rating is too low regardless of the capacity
```

---
## \#11 Posted by: lowGuido Posted at: 2017-07-05T20:45:01.760Z Reads: 87

```
so you have two 5S in series and 3 in Parallel? 
making one 10S3P?
I see no problems here at all. why is everyone saying don't do it? did I miss something?
```

---
## \#12 Posted by: lowGuido Posted at: 2017-07-05T20:54:36.590Z Reads: 87

```
so I have read through this again and again. I see no problems. I say do it.
I do this everyday. have done for years.
parallel up the balance leads and terminate to two 5S JST connectors and charge with two imax B6 balance chargers.

job done.

also you are right about the multistars. the 10C rating is quite adequate given the 10000mah capacity. infact here is a video of my mate on a board powered by 10C multistars smoking my 30C zippys
https://www.youtube.com/watch?v=Arwcq_Cp9es


remember the C rating is multiplied by the mAh to give current output.
```

---
## \#13 Posted by: Maxid Posted at: 2017-07-05T21:49:48.624Z Reads: 83

```
[quote="lowGuido, post:11, topic:26839, full:true"]
I see no problems here at all. why is everyone saying don't do it? did I miss something?
[/quote]

It does work in principle. If he is cautious when setting it up it can work.
But personally I am overly suspicious of anything related to lipos so just want to tell him to be really careful.
He seems not too experienced with this type of thing (otherwise he would not ask in the first place right?) so the potential for failure is high.
Also when hooking the packs up in parallel permanently (like with a BMS) then you will not notice when a single cell goes bad (the same is true with Liion packs but when a Liion vents it is not as bad as when a Lipo burns).

@riva_00 as soon as you hook any of these packs up in parallel you should have more than enough current at your disposal :D
```

---
## \#14 Posted by: riva_00 Posted at: 2017-07-05T22:26:23.117Z Reads: 80

```
I was thinking about going for it anyway, however ignoring the advice of a few veterans would be tremendously stupid. I asked for everyone's advice for good reason.
No I'm not especially experienced, but I'm careful and doing the most intelligent thing I could think of, which is asking all of you. If i want experience, I have to do stuff.

I'll test using a 5s-6x jst parallel charging cable, and use an IMAX b6 (or 2 5s-3x jst cables with 2 chargers).
I have a safe area to charge and store the batteries (LiPo bags and steel boxes).

I may actually downgrade to a 10s2p setup, depends if the extra Wh makes a difference when I'm out riding.

I'm also wondering if i said i was using Li-Ion packs, lets say 10s3p, would you give the same advice of uber caution? Or is it just because of the fact I'm using LiPo's?

Lastly (sorry for all the questions) can you tell me if there's something similar to this: -
https://www.ebay.co.uk/i/291766384982?chn=ps&dispItem=1&adgroupid=41767405657&rlsatarget=pla-327666158629&abcId=1129006&adtype=pla&merchantid=115010295&poi=&googleloc=1007138&device=c&campaignid=861364981&crdt=0
But shows a balanced display (individual cell voltage, not combined voltage)

I actually have this: -
http://alexnld.com/product/skyrc-lipopal-self-voltage-balancer-2-6s-lipo-for-battery-voltage-checker/?gclid=Cj0KEQjwnPLKBRC-j7nt1b7OlZwBEiQAv8lMLP6E5d78pQqLmNTNiMzE4-7eIZtVm4XiZS2Z_0Xyh6AaAlVW8P8HAQ
But I have to open up the battery case and plug it into each battery's balance connector individually. Not the worst, but I'd like to make my board show a ridiculous amount of info on the outside if i can, just for fun (nothing to do with my OCD that means I have to check the back doors locked several times every night)
```

---
## \#15 Posted by: lowGuido Posted at: 2017-07-06T05:18:46.226Z Reads: 66

```
It's just lipos mate. If you said 10S3P li ion every one would have been "hell yeah do that man"
```

---
## \#16 Posted by: wafflejock Posted at: 2017-07-06T06:06:50.412Z Reads: 64

```
I used 2 of those in series didn't see a big problem with the amperage drop but I also didn't really use them for long (also light and not in a hilly area).  I had a cell in one pack go too low and after that it never came back fully so basically had to abandon that pack and ran 6S for a short while waiting on some replacement 5S 5Ah 20C but those have been fine for quite a while (I set very conservative cut off voltage on the VESC)
```

---
## \#17 Posted by: lowGuido Posted at: 2017-07-06T06:45:06.220Z Reads: 63

```
I think the hard and fast rule is
DON'T OVER DISCHARGE.
i have been running my lipos on about 10 or mor boards for 3 years now and never have any problems with them balancing.

I usually only run them down to around 3.8v per cell.
```

---
## \#18 Posted by: Maxid Posted at: 2017-07-06T08:26:49.231Z Reads: 64

```
3.8V :scream: That is still above their nominal voltage which means you are barely using half the energy in your pack. You could have just used smaller batteries.
```

---
## \#19 Posted by: riva_00 Posted at: 2017-07-06T09:05:15.975Z Reads: 62

```
My cut-offs are going to be 3.7 initially, then 3.6 if the packs look fine after a few weeks. Plenty of time to fine-tune everything, just need to make sure i walk to the goal.

I normally open the pack up several times when riding and check how their doing during the initial rides
```

---
## \#20 Posted by: lowGuido Posted at: 2017-07-06T09:49:02.498Z Reads: 62

```
yeah or I could use the batteries that I have and regularly ride short trips and recharge and still have the juice to take a longer trip if I want to.
so much better to over engineer than under engineer. less stress on everything.
```

---
## \#21 Posted by: Maxid Posted at: 2017-07-06T10:07:10.286Z Reads: 54

```
Yeah and it explains why you never had any problems with Lipos
```

---
## \#22 Posted by: riva_00 Posted at: 2017-07-06T10:47:01.619Z Reads: 54

```
If the system works....

Reason why I wanted a 10s3p instead of a 10s2p is partly because of reduced stress on the batteries. I reckon i'll have 15 miles range using pneumatic wheels and I'll not have to worry about voltage sag.
Should also have superior LiPo battery life if i charge to a max of 41V and discharge to 3.6, and of course I won't have to charge that often either....
```

---
## \#23 Posted by: Namasaki Posted at: 2017-07-06T16:42:00.864Z Reads: 53

```
[quote="lowGuido, post:12, topic:26839"]
remember the C rating is multiplied by the mAh to give current output.
[/quote]

I love my Lipos but about the C rating x AH for current. There's no way that that's an accurate number.
And 10C multistar pack might work ok when your 120lbs running on flat ground. 
But when your 190+ going uphill, it's a different story
```

---
## \#24 Posted by: wafflejock Posted at: 2017-07-06T17:05:59.323Z Reads: 53

```
Just to throw in my cut off values I use 3.8-3.6 per lipo cell as the top and bottom cut off values most I've ever seen it put back in was around 3.4-3.6Ah on a 5Ah battery.... From what I've read 80% of Ah use is usually ideal for cell life.
```

---
## \#25 Posted by: Jinra Posted at: 2017-07-06T17:09:32.357Z Reads: 53

```
Given that lipos are "dead" at about 3.5-3.6v, it's not much of a loss. Plus it'll account for any voltage sag in case of stressful rides at low battery levels.
```

---
## \#26 Posted by: Maxid Posted at: 2017-07-06T17:14:10.460Z Reads: 52

```
It is huge loss as Lipos have a very flat discharge curve at their nominal voltage of 3.7v. check some discharge curves!
```

---
## \#27 Posted by: Jinra Posted at: 2017-07-06T17:15:05.400Z Reads: 52

```
I've seen them. Maybe @lowGuido can provide us some numbers on the range he gets vs the WH of his pack?
```

---
## \#28 Posted by: lowGuido Posted at: 2017-07-06T17:32:14.427Z Reads: 58

```
I dont have any real scientifically accurate figures, but from memory most of my rides are about 7km and use around 3000mah maybe 3500mah. I have so many different boards with different batteries but most are 6S ranging from 5000mah to 10000mah
during summer I might do the odd 16km skate and thats usually getting towards the deep discharge area. longest skate I ever had was 22km, and that was full discharge of 6S 8000mah.
```

---
## \#29 Posted by: JdogAwesome Posted at: 2017-07-06T17:52:54.152Z Reads: 58

```
Hey guys thought id jump in and give my 2 cents because I have a similar battery setup. Pretty much im running 4x 3S 5Ah Lipos in a 6S2P config for a total of 10Ah at 6S (gonna do a 12S1P eventually) so that means I have the balance leads of each 3S pack in parallel connected to my BMS. So far this has worked fine for me and none of my cells have had any problems. This is mainly due to the fact that cells in parallel like to keep each other at around the same voltage anways. Like @lowGuido said in theory I dont see any problems with this setup, however if you mess up then obviously theres gonna be some problems, though thats kinda the nature of LiPo's. Also for my charging setup I just have a 24V PSU I got off eBay and adjusted the voltage to 25.2V and its limited at 8A using a CC/CV boost converter. Also @riva_00 if you were planning on charging your board WITHOUT a BMS, I cant recommend that just in case one of your cells over discharges and causes them to overcharge, even if your only charging to 4.1V.

[quote="riva_00, post:14, topic:26839"]
Lastly (sorry for all the questions) can you tell me if there's something similar to this: -
[LINK](https://www.ebay.co.uk/i/291766384982?chn=ps&dispItem=1&adgroupid=41767405657&rlsatarget=pla-327666158629&abcId=1129006&adtype=pla&merchantid=115010295&poi=&googleloc=1007138&device=c&campaignid=861364981&crdt=0)
But shows a balanced display (individual cell voltage, not combined voltage)
[/quote]
They do sell those on eBay, they usually just show battery capacity in % and you just tell it what voltage pack your using, and it figures out the rest. I prefer to use the exact type of meter you linked that shows the complete voltage because im use to just knowing my pack capacity by that. Usually something like [THIS](http://www.ebay.com/itm/New-LY6-External-Mounted-LCD-Lead-Acid-Lithium-Battery-Capacity-Indicator-Tester/262501050575?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2055119.m1438.l2649).
```

---
## \#30 Posted by: wafflejock Posted at: 2017-07-06T18:08:10.366Z Reads: 56

```
That doesn't really make sense... when I'm down to 3.6V and I recharge 3.6Ah on a 5Ah battery that means I used 72% of the battery.  Am I leaving 28% in the pack unused... would I rather do that then have any single cell be below the low voltage limit where it will run away and ruin the whole pack... yeah.
```

---
## \#31 Posted by: lowGuido Posted at: 2017-07-06T18:18:34.101Z Reads: 53

```
[quote="Namasaki, post:23, topic:26839"]
There's no way that that's an accurate number.
[/quote]

thats what it is though. can't argue with facts? Thats what C rating is. It is literally C times capacity equals current.

and look at my mate! without being rude to him hes about 220lbs and smashing me with a 10C multistar.
don't even forget that its pushing a 430kv motor.

just think that over for a few moments... 220lbs.. 430kv.. the current from that multistar is amazing.
```

---
## \#32 Posted by: Maxid Posted at: 2017-07-06T19:25:56.931Z Reads: 49

```
What does not make sense here? Where do you think the remaining energy is?
```

---
## \#33 Posted by: wafflejock Posted at: 2017-07-06T19:49:56.143Z Reads: 47

```
I meant going down to 3.8ish V (maybe a bit lower really I go down to 3.6) is using more than 50% of the pack.  Yes I think the remaining energy is in the pack but I'm saying I think that's fine the main point is to not let any cell sag so low that it dies or gets damaged not to get the pack to 0%

https://endless-sphere.com/forums/viewtopic.php?f=14&t=61672&start=175
```

---
## \#34 Posted by: Maxid Posted at: 2017-07-06T19:55:48.663Z Reads: 48

```
I don't get it. 3.8ish is not 3.6 - there is like the entire capacity in between.
3.8 is not using half while 3.6 is using more than half of the capacity.
What does "fine" mean? You can discharge to only 3.8 and never have a problem so obviously it is fine.
You should know though that a cutoff of 3.5V will allow you to go much further as there is a lot of unused energy in the pack.
```

---
## \#35 Posted by: wafflejock Posted at: 2017-07-06T19:59:58.176Z Reads: 50

```
Yeah about 28% of 12 miles or about an extra 3 miles but I've burned out a cell before and basically had to ditch the whole pack because of it so stick with more conservative values.  You can have more than .5V drop while the battery is under load it's just a small bit risky imo but do what works for you.
```

---
## \#36 Posted by: Maxid Posted at: 2017-07-06T20:03:24.770Z Reads: 48

```
there is more than 28% left in the pack if you stop at 3.8V - looks like 60%
https://endless-sphere.com/forums/viewtopic.php?f=14&t=62932#p940866
```

---
## \#37 Posted by: wafflejock Posted at: 2017-07-06T20:05:19.752Z Reads: 47

```
Yeah I start my battery cut off at 3.8 and end at 3.6 per cell lowguido said 3.8ish I realize there's a good amount of capacity with typical loads between 3.8 and 3.6 but ish was good enough for me.
```

---
## \#38 Posted by: Namasaki Posted at: 2017-07-06T20:18:05.823Z Reads: 44

```
[quote="lowGuido, post:31, topic:26839"]
thats what it is though. can't argue with facts? Thats what C rating is. It is literally C times capacity equals current.
[/quote]
I know the theory, what I'm saying and others have pointed this out to me before I realized it, is that the C value is often over rated making the current calculation inaccurate. 
For example my 5ah/ 60/120C packs
300a cont and 600a peak. I say it's rubbish. 
If it where true, why are the battery wires only rated for 75a
And why do I still get some sag when only drawing 30-40a
I love these batteries and they do perform well compared to others but 600a? Really?
I bet if I laid a 600 amp load on this battery even for a second that it would explode. 
Do you see what I mean?
```

---
## \#39 Posted by: wafflejock Posted at: 2017-07-06T20:20:58.253Z Reads: 41

```
Because bigger numbers are better :wink:
```

---
## \#40 Posted by: Maxid Posted at: 2017-07-06T20:22:20.594Z Reads: 42

```
[quote="Namasaki, post:38, topic:26839, full:true"]
I bet if I laid a 600 amp load on this battery even for a second that it would explode. 
[/quote]

600A load - I guess that would be a short :joy:
```

---
## \#41 Posted by: lowGuido Posted at: 2017-07-06T20:30:14.398Z Reads: 38

```
you are right 600A is a stretch of the imagination.
but the 10C multistars 150A rating is not as unrealistic. 

but what it says on the box is what we have to go by.  we can only ASSUME that the company isnt lying to us.

I can't talk for your 600A lipos, but the multistars in my mates board has been hawling him around for years, and one time when we forgot a remote his board pulled BOTH of us. thats around 380lbs.
I would have liked to see the current draw on that day.
```

---
## \#42 Posted by: wafflejock Posted at: 2017-07-06T20:54:47.932Z Reads: 36

```
Yeah unfortunately ammeters always include some bulky component (either a shunt or a loop) and I keep breaking them... think I'm going to have to hook up a bluetooth module and get metr working.
```

---
## \#43 Posted by: riva_00 Posted at: 2017-07-07T11:44:08.807Z Reads: 35

```
I should have the equivalent of 75c and 15A when i'm finished, which means a constant current draw of 1125 amps :slight_smile:
Voltage sag isn't a problem I need to worry about, even if Zippy is drastically exaggerating their C ratings.

Hoping to do some testing with the new set up over the weekend, just finished soldering the new cables together.

I'm also designing some modular battery enclosures, which I'm now thinking about incorporating some fire retardant fabric on the inside.....
```

---
