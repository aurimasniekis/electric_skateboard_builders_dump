# The Terminology, Formulae and Physical Assembly of Lipo Batteries - or - Wtf does &ldquo;C&rdquo; mean?

### Replies: 29 Views: 4097

## \#1 Posted by: Clonkex Posted at: 2017-09-14T23:46:31.477Z Reads: 434

```
I've seen a lot of confusion surrounding this subject, and not a lot of good explanations in terms of esk8. This is my go at explaining the terminology, calculations and physical assembly of lipo (lithium-polymer, aka LiPo, li-po or Li-Po) battery packs, and is designed to supplement the information already found the [FAQ post](http://www.electric-skateboard.builders/t/start-here-faq-for-diy-electric-skateboard-builders/215/17). This all applies to lithium-ion cells as well, but the nominal voltages are slightly different. Let's begin.

**Lipo Cells**

A single lipo cell has a nominal (which basically means "in name", or the average) voltage of 3.7 volts. That can go as low as 3.2v or 3.3v when depleted or as high as 4.2v when fully charged. Lipo cell sizes vary greatly and can go from a tiny 40mAh (which stands for milliamp-hour, or the number of milliamps that can be supplied for 1 hour; it's a measure of the energy contained in the cell) cells to huge 10000mAh cells (or even bigger). For esk8 you generally don't want less than about 5000mAh because your range will be too short to really have fun. When you're assembling batteries (which, incidentally, are called batteries because they're a "battery" of cells) you need to determine what voltage you want to run at, which brings us to the first number you'll encounter.

**The "S" Number**

If you want to run at 6S (generally accepted to be the minimum for esk8), that would be 3.7v (which, as you'll remember, is the nominal voltage of lipo cells) multiplied by 6, which is 22.2 volts. If you went 10S that would make your battery 37 volts. If you had a 6S lipo, you could take the plastic off the outside (CAREFULLY! If you pierce a lipo cell it **will** catch fire or explode) and you would find 6 individual lipo cells connected in series. So that's the "S" rating on batteries: it's the number of cells connected in series. Connecting in series increases the voltage by total voltage of the newly-connected pack, so adding a 3S (11.1v) pack in series with a 6S pack (or two other 3S packs, which is 22.2v) would make the total voltage 33.3 volts.

**The "P" Number**

Now, the "P" rating on packs means very little. It's how many batteries are connected in parallel. Connecting batteries in parallel increases the capacity (the mAh amount) of the total pack by the mAh of the newly-connected pack. So if you have a 6S 5000mAh pack and you connect another identical pack in parallel, the total battery capacity will be 10000mAh (and the voltage will still be 6S). Notice I said it's the number of "batteries" connected in parallel, not "cells". If you have a 10S2P pack, that's two 10S batteries connected in parallel. So if you took the pack apart, you'd find a total of 20 individual cells. The reason the "P" number means very little is that it only tells you how the pack is physically assembled, not how big it is. If your cells are 2000mAh, that's a much smaller 10S2P pack (it would be 4000mAh) than if the cells were 5000mAh (which would be 10000mAh).

**The "C" Number**

The "C" rating on batteries lets you calculate how many amps the battery is rated to discharge at any one point. It just stands for "capacity", so a 20C battery is 20 times the capacity in amp-hours. That means a 2000mAh 20C battery can only discharge a paultry 40 amps, but a 5000mAh 20C battery can discharge a much heftier 100 amps. So yes, they do expect you to do the maths yourself. It's worth noting that however you connect your batteries together, the "C" rating _never changes_. However, since C stands for capacity, if you connect two packs in parallel the capacity will increase, which means the amount of amps that can be discharged doubles. For example, if you have a 5000mAh 20C pack, that's 100 amps of available discharge current. If you connect another identical pack in parallel it'll make a 10000mAh 20C pack, but since the mAh has doubled, the available discharge current has increased to 200 amps. **It should be noted**, however, that these are _theoretical_ values. In reality, while the battery may be fine supplying the theoretical amps (depending on how accurate the manufacturer's C-rating is), the wires probably won't. A lot of batteries have 10 or 12 gauge wires, which is not enough to carry 200 amps; the wires will literally melt ;) For more information on wire gauges refer to [@jmasta's post](http://www.electric-skateboard.builders/t/the-terminology-formulae-and-physical-assembly-of-lipo-batteries-or-wtf-does-c-mean/33162/13?u=clonkex) for regular wire and [@Namasaki's post](http://www.electric-skateboard.builders/t/the-terminology-formulae-and-physical-assembly-of-lipo-batteries-or-wtf-does-c-mean/33162/16?u=clonkex) for silicon wire.

**Calculating Range**

And finally, the calculation you use to get the approximate range of your board is Wh (which stands for Watt-hours, or the number of Watts that can be supplied for 1 hour; it's a measure of the energy contained in the pack) divided by 10 equals the approximate number of kilometres you can go. So a 500Wh pack (a really big pack!) should have an approximate range of around 50km (which is a hella long way to ride on a skateboard!). To calculate the Wh of your pack you simply multiply the number of Ah (amp-hours) by the voltage. So with a 5000mAh 10S pack, that would be 5Ah (because 5000mAh is 5Ah) times 37 volts, which is 185Wh, and should have about 18.5 kilometres range. Note that this calculation is intended for street boards (i.e. standard urethane wheels). The range will be significantly reduced if you're on a Trampa/AT style board (i.e. mountainboards with pneumatic off-road wheels).

Something worth noting is that when assembling packs, you must _always_ ensure all the batteries you intend to connect together are the same voltage, the same C-rating, the same mAh and same chemistry (lipo or lion). Otherwise you risk wearing out your battery much faster or simply destroying it instantly (which, of course, risks a lipo fire or explosion). Preferably you should simply always use the exact same batteries from the same manufacturer.

Please feel free to suggest changes or corrections :)

**Quick-reference summary:**

- "S" is number of cells in series
- "P" is number of batteries in parallel
- "C" rating is the available discharge rate (eg. 3000mAh 20C = 60A discharge rate)
- "V" is voltage, which is determined by the number of cells in series (eg. 3S = 3 * 3.7 = 11.1V)
- "mAh" is milliamp-hours, or the number of milliamps that can be supplied for 1 hour
- "Ah" is amp-hours, or the number of amps that can be supplied for 1 hour
- "Wh" is watt-hours, or the number of watts that can be supplied for 1 hour
- Ah * V = Wh (eg. 5Ah * 22.2V = 111Wh)
- Two lipos connected in series only doubles voltage
- Two lipos connected in parallel only doubles mAh capacity
- "C" rating never changes, but increasing mAh increases available discharge rate
- Wh / 10 = approximate range in KM (eg. 111Wh / 10 = 11.1KM range) - only accurate for street boards
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-09-15T00:26:13.263Z Reads: 346

```
Nice essay
```

---
## \#3 Posted by: Clonkex Posted at: 2017-09-15T00:41:12.676Z Reads: 321

```
I'm going to assume you're not being totally sarcastic and say thanks! :P
```

---
## \#4 Posted by: Sapphirinia Posted at: 2017-09-15T01:09:16.442Z Reads: 300

```
So. Much. Math... I need to write this stuff down to understand my own batteries better. Thanks for helping out the noob like me. Much easier to understand.
```

---
## \#5 Posted by: Clonkex Posted at: 2017-09-15T01:20:21.199Z Reads: 267

```
Haha yep there's a lot but it's all pretty simply maths really so it shouldn't be too hard to get your head around :) The difficulty will be remembering everything at once to understand it all :P
```

---
## \#6 Posted by: stormboard Posted at: 2017-09-15T01:45:15.466Z Reads: 238

```
"anthony your an artist"
```

---
## \#7 Posted by: Clonkex Posted at: 2017-09-15T03:01:59.801Z Reads: 219

```
I don't know this reference :thinking:
```

---
## \#8 Posted by: jmasta Posted at: 2017-09-15T03:06:44.797Z Reads: 222

```
[quote="Clonkex, post:1, topic:33162"]
For example, if you have a 5000mAh 20C pack, that's 100 amps of available discharge current. If you connect another identical pack in **series** it'll make a 10000mAh 20C pack, but since the mAh has doubled, the available discharge current has increased to 200 amps.
[/quote]

Good write up!  

Quick correction: I think you meant "**parallel**" here.  Two 5000mAh 20C packs in series would still only be "100A". 

 I put "100A" in quotes because those numbers are usually very inflated.  For example, my Zippy 6.2Ah 40C lipos would "technically" be rated to ~248A continuous... on 10AWG wires. Yeahh... okay....  Not even close
```

---
## \#9 Posted by: Namasaki Posted at: 2017-09-15T04:35:08.277Z Reads: 199

```
[quote="jmasta, post:8, topic:33162"]
I put "100A" in quotes because those numbers are usually very inflated.  For example, my Zippy 6.2Ah 40C lipos would "technically" be rated to ~248A continuous... on 10AWG wires. Yeahh... okay....  Not even close
[/quote]

Hey @jmasta
I can top that,
I'm running 5ah Lipos with 60/120C rating. Thats a whopping 300a continuous and 600a burst on 12awg wires!!!!!
So what would really happen if I trusted the math and put a 300a-600a load on that battery.

I would not want to find out.....
```

---
## \#10 Posted by: Clonkex Posted at: 2017-09-15T04:50:48.420Z Reads: 187

```
Yes indeed I did, thanks for pointing that out! I've added something specifically noting that these are theoretical numbers only since it's worth mentioning directly and most people won't even consider the amps that the wires can carry without melting :P

I'm not an expert on wire gauges, though, so I can't offer any specific guidance in that area.
```

---
## \#11 Posted by: Mobutusan Posted at: 2017-09-15T06:06:29.153Z Reads: 169

```
Nice write up. Very clear descriptions and examples. Only thing I noticed is that watt hours are a measurement of energy, not power. Looks like those terms got flip flopped.
```

---
## \#12 Posted by: Clonkex Posted at: 2017-09-15T06:21:20.257Z Reads: 175

```
Hmm true. Not flipped, just mistaken. I forgot Watt-hours are a measurement of energy. It's Watts that are a measurement of power. I'll just remove that link and mention of power until I can write up a clearer and more correct explanation of that.

Thanks for the compliments though! :D
```

---
## \#13 Posted by: jmasta Posted at: 2017-09-15T06:31:06.291Z Reads: 169

```
[quote="Clonkex, post:10, topic:33162, full:true"]

I'm not an expert on wire gauges, though, so I can't offer any specific guidance in that area.
[/quote]

This is what I usually go by:  https://www.powerstream.com/Wire_Size.htm




* **Main power lines:** 10 ~ 12 AWG is most common.  8AWG is used sometimes but probably overkill for most setups

* **Motor phase wires:**  12AWG is most common, because 10AWG is just too bulky



* **Charging port:**  At least 18 ~ 22 AWG

* **Balance leads**:  26AWG is plenty, but I prefer 22AWG

The following table could be greatly simplified for our purposes.  Odd numbered wire gauges are uncommon.  8~26 AWG covers all practical applications for e-skate. _Keep in mind the current ratings in this table are pretty conservative numbers_

<img src="/uploads/db1493/original/3X/d/8/d8337e60211e39ed42c5aa2df7d71092b1a2492d.png" width="299" height="500">
```

---
## \#14 Posted by: Clonkex Posted at: 2017-09-15T06:33:40.791Z Reads: 147

```
Nice, good information! I'll link your post in the OP.

I'm aware of the most-used gauges in esk8, and I've seen that image before but I wasn't sure if there was some other factor I wasn't aware of because the current ratings seemed too low to make sense. I guess burst ratings would be much higher though.
```

---
## \#15 Posted by: TarzanHBK Posted at: 2017-09-15T06:45:52.246Z Reads: 149

```
nice to see someone taking time to do a writeup like that. Always helpful for some people :slight_smile:
```

---
## \#16 Posted by: Namasaki Posted at: 2017-09-15T11:02:42.713Z Reads: 149

```

@jmasta 
Silicone wire has different ratings than standard chassis wire

http://www.4-max.co.uk/silicone-wire.htm

<img src="/uploads/db1493/original/3X/6/0/60427c8fab8ada45fe1a110cb1d565e657d7a9f1.jpg" width="281" height="499">
```

---
## \#17 Posted by: Yecrtz Posted at: 2017-09-15T11:41:33.230Z Reads: 150

```
Good info! Note that calculating range with that formula works excellent for your average street board. For trampa/AT boards the power consumption will be considerably higher.
```

---
## \#18 Posted by: Clonkex Posted at: 2017-09-16T00:01:53.968Z Reads: 144

```
Good points good points, added :)
```

---
## \#19 Posted by: Cobber Posted at: 2017-09-16T11:50:50.285Z Reads: 138

```
Yeah I'm with Nama, for calculating wire diameter/gauge I like the [this calculator as it incorporates cable length](http://www.solar-wind.co.uk/cable-sizing-DC-cables.html) and often for a eSk8 we use a really short run.
```

---
## \#20 Posted by: GrecoMan Posted at: 2018-02-19T22:09:12.518Z Reads: 114

```
is it really called formulae? 😲
```

---
## \#21 Posted by: Clonkex Posted at: 2018-02-19T22:10:17.318Z Reads: 104

```
It's the plural of formula ;)
```

---
## \#22 Posted by: GrecoMan Posted at: 2018-02-19T22:10:50.650Z Reads: 107

```
my life has been forever changed for the better.
```

---
## \#23 Posted by: City-Blade-101 Posted at: 2018-10-09T20:01:55.218Z Reads: 57

```
Thank you...that seems to be the perfect start for electric epileptics like me.
```

---
## \#24 Posted by: Clonkex Posted at: 2018-10-09T21:45:51.097Z Reads: 54

```
I feel there's a few things I could have explained better but I can't edit the post now so hopefully it's not too bad :stuck_out_tongue:
```

---
## \#25 Posted by: City-Blade-101 Posted at: 2018-10-09T22:22:25.242Z Reads: 50

```
No its not to bad though.
I learned a lot from this post, and I know now that my beloved Onan x2 has a 10s2p batterie hahahaha yeah! Feels great to know about that 🤓...
and i know it has 158wh that means it can reach a distance of almost 16km what is pretty similar to reality...awesome
```

---
## \#26 Posted by: AreaKruzer Posted at: 2018-10-10T01:55:14.887Z Reads: 44

```
sorry Clonkex, the "C" number stands for Coulombs, not Capacity. the "mAh" or "Ah" stands for the Capacity.

Coulombs is the SI unit of 1 amp/sec

So if a battery is rated at 10C with a stated capacity of 5000mAh, the calculation will be 10 x (5000 / 1000) = 50A.
```

---
## \#27 Posted by: Clonkex Posted at: 2018-10-10T02:41:06.327Z Reads: 47

```
I'm well aware of how the calculation works. If you read the OP you'll see I do actually explain that.

And unfortunately, you're wrong. C does in fact stand for capacity. It's using the standard maths shorthand for multiplication, so 20C is 20 * C, or 20 * capacity. It would make no sense for it to stand for coulombs. 1 coulomb is [the amount of charge transported by a constant current of 1 amp for 1 second](https://en.wikipedia.org/wiki/Coulomb), so 1 coulomb == 1 amp over 1 second. If the C in 20C stood for Coulombs, that would mean 20amp-seconds (which is nonsensical when it's used to measure maximum current delivery, and 20A-seconds would be a very small battery, only 5.555mAh), and that would be the same for every battery. In reality the C stands for capacity, so 20C for a 5000mAh battery means that battery can deliver 100 amps nominal, but 20C for an 8000mAh battery allows 160 amps nominal.

But if I got any of that wrong, please correct me :slight_smile:
```

---
## \#28 Posted by: AreaKruzer Posted at: 2018-10-10T03:12:40.782Z Reads: 48

```
I guess the C doesn't refer to either Capacity nor Coulomb. The C rate on the battery stands for the discharge rate. so a 1C means that it can discharge the capacity of the battery within an hour. 10C refers to a tenth of an hour.

Meaning to say that if your battery is rated 5000mAh with 1C, it will discharge the entire capacity of 5000mAh within an hour. if 10C, it will mean that it is capable to discharge 5000mAh in 6mins.

For a battery with a capacity of 100 Amp-hrs, this equates to a discharge
current of 100 Amps. A 5C rate for this battery would be 500 Amps, and a C/2 rate would
be 50 Amps. 

http://web.mit.edu/evt/summary_battery_specifications.pdf

so i guess this clears the teminology behind the C and Capacity. the C is most likely to be described as discharge rate.
```

---
## \#29 Posted by: Clonkex Posted at: 2018-10-10T03:49:46.017Z Reads: 43

```
I guess you could read it that way. Personally I think it's easier to understand as simply meaning capacity since that's how the formula works, even though I wouldn't expect C to mean capacity except in the context of defining a discharge rate. Either way we all know the C-rate of a battery is the discharge rate, so I guess it doesn't matter what C stands for ¯\\\_(ツ)_/¯
```

---
