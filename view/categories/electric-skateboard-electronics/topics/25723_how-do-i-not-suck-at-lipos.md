# How do I not suck at lipos?

### Replies: 27 Views: 1291

## \#1 Posted by: NickTheDude Posted at: 2017-06-19T21:42:15.544Z Reads: 139

```
So, since getting into this, I've probably ruined at least 2 or 3 lipo packs. Some had dead cells and some have died through neglect. I was wondering if any of you guys with more experience could give me some advice on how to properly take care of these.

Things I know:

* Take C ratings with a grain of salt and only use half of what the battery is rated for
* Don't charge over 4.2V
* Don't discharge under 3.0V
* Discharge to 3.7V for storage

If I do happen to over discharge a cell, what's the lowest "salvageable" voltage I should look for? Also, I've heard that internal resistance plays a large role in the health of a cell. How do I measure this and what kind of numbers should I be happy or concerned with? Thanks.
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-19T21:43:56.743Z Reads: 137

```
Lipos are much pickier about low voltages than Li-ion. I don't use them myself but from the discharge graphs I've seen I wouldn't discharge a lipo lower than 3.5v
```

---
## \#3 Posted by: sl33py Posted at: 2017-06-19T21:49:07.861Z Reads: 136

```
[quote="Jinra, post:2, topic:25723"]
I wouldn't discharge a lipo lower than 3.5v
[/quote]


Agreed!  Given sag when in use, i set my alarm for 3.7/3.6v and just make sure i'm going easy at the end not to over-discharge.  Example - it'll beep going up a hill, but then back to 3.8v+ on the flats - if i'm squeezing range i'll ride on the flats until it beeps again w/o high draw like hill or hard accelerating.

Gives some warning this way and i can moderate my acceleration or walk up a hill to make sure i can get where i need to go.  Instead of only beeping at 3.5v or similar when it's effectively "empty".

Overcharging and over-discharging - best way to kill a cell/pack/battery!
```

---
## \#4 Posted by: sl33py Posted at: 2017-06-19T21:52:42.283Z Reads: 123

```
[quote="NickTheDude, post:1, topic:25723"]
How do I measure this and what kind of numbers should I be happy or concerned with? Thanks.
[/quote]


my iCharger has a measure IR feature.  I think the legit iMax B6ACV2 does as well?

checking good 'ol Amazon:
[quote] Product description

The B6AC V2 is the upgraded version for well-known iMax B6AC. Compared with B6AC V1, it is more accurate and stable and also has some new features and functions. Users could set the terminal voltage by themselves and connect it to PC for PC control and firmware upgrade. **What's more, users could also use it as Lithium Battery Meter and Battery Internal Resistance Meter.** There are Automatic Charging Current Limit, Capacity Limit, Temperature Threshold and Processing Time Limit which makes the charger safer than V1. B6AC V2 is a high-performance, micro processor control charge/discharge station with battery management suitable for use with all current battery types, with integral equalizer for six-cell Lithium- Polymer (LiPo), Lithium iron phosphate(LiFe) and Lithium-Ion (LiIon) batteries; maximum 6A charge current and maximum 50W charge power.
[/quote]
```

---
## \#5 Posted by: Namasaki Posted at: 2017-06-19T22:11:39.658Z Reads: 96

```
My recipe for success has been:
1. Use guality Lipos with high C rating (60C+)
2. Balance charge every Cycle 
3. Try to not discharge below 3.6v at rest and never go below 3.2v under load.
```

---
## \#6 Posted by: wmj259 Posted at: 2017-06-19T22:13:53.008Z Reads: 96

```
[quote="NickTheDude, post:1, topic:25723"]
How do I measure this
[/quote]

Any good charger can do this. Its called a IR measurement, (internal resistance). Good numbers range in various conditions.
You would take the resistance and times it by the average amperage to get your voltage drop. 
If you look at the example under 
**Internal Resistance: The Mystery Number**
https://rogershobbycenter.com/lipoguide/

I have my lipo alarm set to 3.7, conveniently placed at the storage voltage. I have only once in the last 3 weeks had my alarm go off from voltage sag (was from flooring the throttle). I could go lower but that would mean once I'm done using the lipos I would have to recharge them.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-06-19T22:54:54.719Z Reads: 78

```
One thing I forgot to mention.
You should let your Lipo batteries rest for at least 15 min after charging them before running them.
And, you should let them rest for 30 min after running them before charging them. 
I read that somewhere but I can't remember where.
```

---
## \#8 Posted by: Jinra Posted at: 2017-06-19T23:01:10.956Z Reads: 76

```
Yea this is pretty standard practice, I think battery university says something on their site as well.
```

---
## \#9 Posted by: oldguy Posted at: 2017-06-19T23:18:24.101Z Reads: 70

```
Is there a battery capacity meter that will display the voltage in a cell (or the average) instead of a cumulative measurement or a percentage? What is this voltage alarm you speak of?
```

---
## \#10 Posted by: Jinra Posted at: 2017-06-19T23:20:36.828Z Reads: 70

```
@evoheyax did exactly this with his board, he has like 12 LCD's that display the voltages of each cell group. You'll pretty much have to do that if you want readings from every cell group.
```

---
## \#11 Posted by: evoheyax Posted at: 2017-06-19T23:24:01.104Z Reads: 65

```
Yea, theres not really a better solution than that at this moment. I am looking into using the bms to feed individual cell data to the vesc, and modifying the vesc firmware to take in this extra info and pass that along to my iphone app. However, the issue with this will be you'll have to use certain or maybe even one particular bms.
```

---
## \#12 Posted by: oldguy Posted at: 2017-06-19T23:26:28.478Z Reads: 61

```
So is there anyway to get some indication while riding that things are getting perilosly low, aside from performance degradation? This will be my first time with lipos to care for as well and I had intended to ask this same question so I am glad it was posted.
```

---
## \#13 Posted by: Jinra Posted at: 2017-06-19T23:28:02.572Z Reads: 60

```
If you're using a VESC you can set a battery cutoff start in which you'll notice performance degredation but not harm the battery if the value is sufficient. Otherwise voltage alarms will scream like a banshee when you're voltage is too low.
```

---
## \#14 Posted by: oldguy Posted at: 2017-06-19T23:28:05.391Z Reads: 59

```
Yes, you would need some sort of wireless protocol from the bms to get that info I would think
```

---
## \#15 Posted by: oldguy Posted at: 2017-06-19T23:30:16.494Z Reads: 60

```
My first build I am using the x-car beast. Hoping that by the time I am ready for another build the vesc-6 will be out and tested (and the other "stuff" currently surrounding the vesc is sorted out)
```

---
## \#16 Posted by: Jinra Posted at: 2017-06-19T23:39:55.314Z Reads: 60

```
I wouldn't hold my breath. I'd say just pick up a VESC4 as it's tried and true as long as you get it from a reputable source such as Ollin, Axle, esk8.de, Enertion, and others
```

---
## \#17 Posted by: evoheyax Posted at: 2017-06-19T23:42:58.656Z Reads: 61

```
Well I have a vesc to iphone system, so if I could modify the firmware to add that data to the vesc's data structure, and then pass it off with the COMM_GET_VALUES. But the bms needs to communicate to the VESC and vice versa.
```

---
## \#18 Posted by: wmj259 Posted at: 2017-06-19T23:45:44.848Z Reads: 60

```
[quote="oldguy, post:9, topic:25723"]
Is there a battery capacity meter that will display the voltage in a cell
[/quote]

I got these, you can also set a voltage for the alarm to beep at.
https://www.amazon.com/Readytosky-Battery-Checker-Voltage-Indicator/dp/B01FHIMU0M
```

---
## \#19 Posted by: oldguy Posted at: 2017-06-19T23:47:35.347Z Reads: 61

```
You might get the data from the bms to feed into an off board BT xmitter but then your app wouldn't be able to talk to anything else and it might interfere with your remote receiver..,it would be an interesting project.
```

---
## \#20 Posted by: oldguy Posted at: 2017-06-19T23:48:28.235Z Reads: 60

```
@wmj259 that's great, thanks!
```

---
## \#21 Posted by: oldguy Posted at: 2017-06-20T03:47:41.746Z Reads: 45

```
One last thing, as I am new to lipos I'd prefer to charge them outside the immediate confines of my home (read garage) but I know there are lots of spells and incantations that go along with using, charging, and storing these power sources. Can I assume that ambient temperature is one of them? My garage is in southern Florida (which works out great because so is the home it is attached to) - this means that temps can get into the low 100's for about half the year, particularly when closed. Is that an issue or is their room-temp limit at a higher threshold? 
 I WILL get one of those fireproof bags, but I'd prefer to store that in the garage as well. This is a big problem for me, I married the fire chief's daughter. If I burn this house down I'll be in the doghouse for the rest of my life (hell, it would probably make the local paper). 
Tell me I don't have to keep them inside under AC...?
```

---
## \#22 Posted by: Namasaki Posted at: 2017-06-20T03:55:46.130Z Reads: 38

```
I always have charged my Lipos inside the house.
The trick is to use a good reliable charger.
Money spent on an expensive charger is not money wasted.
I have never had a Lipo catch fire while charging.
still fire safe bags are not a bad idea if your taking the packs out of the board to charge them.
And it's best to keep an eye on them while they're charging.
So, are you gonna stay in that 100+ deg garage to keep an eye on your batteries?
You know, if you catch the garage on fire, you can probably kiss your house goodbye as well.
You could get a fire cabinet to store them in.
```

---
## \#23 Posted by: wmj259 Posted at: 2017-06-20T04:06:28.677Z Reads: 40

```
I agree with the buy a good charger. The money you spend on the charger is how dearly you care about your life basically. If you get a wonky charger, the chances of your batteries not being well charged/taken care of are much greater. Spend the extra $20-30-40 bucks. Hopefully no-one will ever have to use their home-owners/renters insurance. 🤞

I charge them inside as-well, but I have a fire extinguisher within a arms reach. Also for storage I have a BBQ grill out on the balcony that I just pop open, put the box of lipos in and close that thing up nicely. If anything does seem to go boom, there are vents along the side of the grill shooting the fire out towards empty air from the 2nd floor.
```

---
## \#24 Posted by: sl33py Posted at: 2017-06-20T04:25:04.970Z Reads: 44

```
[quote="oldguy, post:21, topic:25723"]
I know there are lots of spells and incantations that go along with using, charging, and storing these power sources.
[/quote]


Great suggestions already from @Namasaki and @wmj259, but i'll add 2 more suggestions.

Fireproof bags are nice, but you can also use inexpensive pyrex dishes.  I found a few used at value village for a few bucks total.  And no itchy fiberglass or whatever is in those bags when they fray.

Temp probe!!!  Seriously it makes it almost failure proof.  For the 8-10$ you plug in a temp probe and set on the battery while charging.  *Before* any sort of major failure the cells will get really hot - and if the temp probe is used it'll shut down the charge automatically.  

Love my iCharger 306B.  The nicer high amp chargers need AC-->DC power supplies.  You can get really nice ones, but i'd also suggest looking at some of the dell power supplies that are pre-modded for 12v (sometimes 50-60A output too) for a fraction of the $ of equivalent 350w power supplies w/ a ton more output.  

You won't really need the 30A output until you charge big batteries, or a lot in parallel.  I like to charge at 1c, or even .5c to give better battery life.  BUT it is nice when you want to quickly charge and ride after work...

GL!
```

---
## \#25 Posted by: Namasaki Posted at: 2017-06-20T04:34:42.008Z Reads: 44

```
This is the one I use or use to use until I went down the bms road.
Now it spends more time in the closet than on the bench.
https://www.amazon.com/dp/B00SZ1CBVC/ref=psdc_2234135011_t1_B00VOYR6MQ
```

---
## \#26 Posted by: oldguy Posted at: 2017-06-20T04:37:18.176Z Reads: 44

```
Thank you both! I just feel like I'm playing with..,well, right.
```

---
## \#27 Posted by: lrdesigns Posted at: 2017-06-20T04:45:58.675Z Reads: 44

```
I have used lipos since they first became available for RC models. Was really into the hobby before Eska8.  

* **Be conservative with low voltage.** Try to never go below 3.5 because the voltage drops off a cliff past there. It will soon be at zero before you know it. Using the voltage alarms like above is really the best way as they monitor individual cell voltage not pack voltage. If you only monitor pack voltage one cell can drop below and you wouldn't know. 

* High quality high C rated batteries last longer, they start of with much lower resistance then low C batteries and will be less stressed during use. 

* Using larger higher mah then you need will effectively give you a higher C rating and the batteries will be under less stressing during use.

* Balance regularly, Every charge if possible.

On several occasions I have had one cell in a pack drop down to 2.0 volts. I put them on the charger asap. Its still usable but after this but that cell is damaged and will discharge faster than the others so needs to be babied and balance every charge. (Not recommended)

I have only seen 3 cases where they can catch fire.
1. Over charge. 
2. Massive over discharged amperage to the point of thermal run away. Would probably never happen to an esk8. More mild cases cause puffing of the pouches.
3. Physical damage.
```

---
