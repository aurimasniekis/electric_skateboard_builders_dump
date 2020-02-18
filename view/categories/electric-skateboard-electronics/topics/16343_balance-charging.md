# Balance Charging

### Replies: 13 Views: 1099

## \#1 Posted by: Sarky1 Posted at: 2017-01-19T16:28:39.308Z Reads: 101

```
Whats your solution. I went the no BMS route as I have balance chargers up the wazoo.

Whats your method for charging with a balance charger and keeping it clean??


Mine is a little panel I remove and can get to my batteries
```

---
## \#2 Posted by: anorak234 Posted at: 2017-01-19T16:34:41.081Z Reads: 99

```
Miamielectricboards (@oriol360) makes a one plug cable for balance charging. Really simple, really clean.
```

---
## \#3 Posted by: Okami Posted at: 2017-01-19T17:06:44.995Z Reads: 90

```
Can you give out some more details?

Charging just with one cable does sound convenient!

It is always a pain to stick that little balance connector to the charger.. especially if you dont have long balance wire extension harness!
```

---
## \#4 Posted by: anorak234 Posted at: 2017-01-19T17:09:03.049Z Reads: 85

```
http://miamielectricboards.com/shop-1/ez
```

---
## \#5 Posted by: mmaner Posted at: 2017-01-19T17:17:10.487Z Reads: 78

```
I have 2 of them from @oriol360, they are great, makes balance charging easy.  I actually prefer to balance change, rather than having to check behind a BMS to verify my cell integrity.  T

http://miamielectricboards.com/shop-1/ez

<img src="/uploads/db1493/original/3X/d/c/dca53ae205f2de4c7571a801cd93aa2d2a54b315.jpg" width="690" height="443">
```

---
## \#6 Posted by: Okami Posted at: 2017-01-19T17:19:21.341Z Reads: 71

```
You know.. I think the next level would be to build a wireless charging station! 

That would be a hit! 

I know phones can be charger with ''Qi'' pads now.. So I wonder can it be ''stepped up'' to charge larger batteries and also with higher current..

Otherwise, perhaps it could be made from many smaller pads, arranged in the right places! and the board also most be position in a certain way!

This is just a random Idea I got!

----

Looks like im not the only one with such an idea:

_Inductive charging for ebike:_

https://endless-sphere.com/forums/viewtopic.php?f=14&t=41064
```

---
## \#7 Posted by: mmaner Posted at: 2017-01-19T17:24:24.686Z Reads: 67

```
[quote="Okami, post:6, topic:16343"]
phones can be charger with ''Qi'' pads
[/quote]

It has been done successfully with remotes, but QI charging uses such a low amperage threshold that it would take many hours, probably a day or more, to charge just a 6S pack.
```

---
## \#8 Posted by: Hummie Posted at: 2017-01-19T17:40:42.177Z Reads: 63

```
Electric cars do it.
```

---
## \#9 Posted by: Michael319 Posted at: 2017-01-19T17:43:36.274Z Reads: 61

```
Wireless charging is getting better and better. Although it might not be accessible now, maybe eventually we will get something like:
https://www.pluglesspower.com
```

---
## \#10 Posted by: Okami Posted at: 2017-01-19T17:48:14.722Z Reads: 61

```
Some info I found interesting:


<img src="/uploads/db1493/original/3X/f/9/f9bab12b67696eb207ddb9af413c53a47ef6d5ed.jpg" width="571" height="234">

<img src="/uploads/db1493/original/3X/c/0/c0189f4420ea62c258f67bddeea77a3be62b4da3.png" width="255" height="96">

''Plug'' look:

<img src="/uploads/db1493/original/3X/8/c/8c0ba51bd626ce44bf33c67374a82ab34c6edfab.jpg" width="470" height="372">

''car's receiver pad''

<img src="/uploads/db1493/original/3X/8/c/8c2e3c9c482628904b38ae4407bc598119ae62e6.jpg" width="690" height="166">

It looks like there could be a really wide/big coil in that ''car mounted pad''
```

---
## \#11 Posted by: Michael319 Posted at: 2017-01-19T18:24:45.056Z Reads: 57

```
Yeah, wireless charging uses coils, but that's a seriously powerful coil.
```

---
## \#12 Posted by: Okami Posted at: 2017-01-19T18:30:07.559Z Reads: 54

```
It could be possible to mount at least a few coils over the board's surface..

Im just not sure yet how  mathematically coil's size impacts its power output/efficiency
```

---
## \#13 Posted by: Hummie Posted at: 2017-02-01T18:33:04.459Z Reads: 34

```
I dont think this high power 4v power source would work for balancing by hooking all  my 12 cells in parallel as it uses pwm.
http://www.trcelectronics.com/View/Mean-Well/HRP-450-5.shtml
but oo that would be nice.

But balancing should be doable with a constant 4.2 REAL voltage and all the cells in parallel.  I say real because I'm finding that a typical charger for lithium (such as above) uses pwm and has features which i think would not allow multiple cells in parallel to balance as the internal computer wouldn't get correct feedback from the cells.  I believe it's effectively giving higher voltages chopped in the interest of time saving at the end of a charge when the cells' voltage is close to the source voltage and current would otherwise be too low, and to reduce current when there is a large difference between the supply and cell voltage at the start of charging and therefore current could be too high, and at the end of a charge lithium cant handle any pwm with the voltage spikes and is turned off.  (I think I understand what's going on here but please correct me).

With a TRUE dc voltage, such as would come from out of the wall and then transformed to a smooth 4 volts after being rectified and smoothed, there's no variation in voltage and cells in parallel would balance and could be charged at huge power at the same time.  they would charge much quicker at a low state of charge with the greater discrepancy between the supply and cells, and that needs to be taken into account, and they'd be slow to charge at almost full charge, ...but so what and if I could make this thing...!!!!  anyone have any practical advice?  I'm waiting on my "stereo fixer" off craigslist to come up with a list of parts and costs but still fishing for feedback.  It's hard to find info on making a high power transformer.

the transformer would require 1 source coil and 12 "receiving" "secondary" coils so as to not form any electrical parallel connections since the cells are already connected in series and that would be effectively shorting.  but with the 12 transformer "secondary" coils it's good and power is transfered solely through a magnetic field and not electrical.

this thing will be inefficient.  a plus of the pwm method of charging is it's efficiency is much better than what will result from the transformer method.  But  electricity out of my wall is cheap and not a concern and happy to heat my room in the meantime.

I'm going to simply see if I can get it made by a transformer store.  duu.  a lot easier source of info as well.  I'll tell you what the obstacles are.
to me this is a win win with possibly huge power output and balancing. 
http://osbornetransformer.com/products/transformers/rectifier-transformers/
```

---
