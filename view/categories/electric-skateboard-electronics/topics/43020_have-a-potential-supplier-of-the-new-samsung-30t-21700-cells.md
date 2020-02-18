# Have a potential supplier of the new Samsung 30T 21700 cells

### Replies: 213 Views: 9072

## \#1 Posted by: uigiroux Posted at: 2018-01-07T01:22:48.060Z Reads: 681

```
Have been corresponding with a company in China and they claim they have the new Samsung 30T 21700 battery cell in stock finally.  I tried getting these late last year and it turned out incorrect, and was told they wouldn't be available until this year.  So it's pretty early in the year but I have been talking with a supplier in China and they say they have the 30T in stock.  She asked how many I might need.  I figured I'd these are legit that a lot of y'all would want on these so I told her probably about 1,000, maybe more, maybe less.  She said they'd be $6.25 at that amount.  So I am going to continue talking to them and get a feeling for if this is authentic or not, but if it is maybe someone can set up a group buy?  These have been tested by many tech publications and they said it's the best battery they've tested so far...  Here's a link to a detailed review of the battery. 

http://www.candlepowerforums.com/vb/showthread.php?431795-Test-review-of-Samsung-INR21700-30T-3000mAh-(Gray)

Anyways, yeah if this is the real deal I think we should try and get a group buy going.  I can't set up one, but hopefully someone will rise to the occasion, lol!
```

---
## \#2 Posted by: scepterr Posted at: 2018-01-07T01:42:47.905Z Reads: 620

```
How many cells do you personally want to get?
```

---
## \#3 Posted by: McPickle Posted at: 2018-01-07T02:37:40.021Z Reads: 612

```
Yeah, that would be cool. I’ve also been searching for these cells for a while.
```

---
## \#4 Posted by: pixelsilva Posted at: 2018-01-07T02:56:20.900Z Reads: 602

```
If is an Alibaba supplier ask for a sample. When you get it, test It.
```

---
## \#5 Posted by: thisguyhere Posted at: 2018-01-07T02:57:50.728Z Reads: 595

```
i don't really get these cells.

the Wh / $ ratio doesn't make sense.

it only excels in discharge so it'd be great for acceleration.

but the range you'd get on whatever configuration would be at about the same or less than 18650 cells, since you couldn't fit as many cells.
```

---
## \#6 Posted by: notepad Posted at: 2018-01-07T02:59:00.679Z Reads: 571

```
you bring up a good point,  I wonder if anyone has any links to papers to why these would be used over 18650's
```

---
## \#7 Posted by: uigiroux Posted at: 2018-01-07T03:01:56.329Z Reads: 561

```
http://www.candlepowerforums.com/vb/showthread.php?431795-Test-review-of-Samsung-INR21700-30T-3000mAh-(Gray)

Doesn't this basically say where it's advantages are and so on?
```

---
## \#8 Posted by: uigiroux Posted at: 2018-01-07T03:03:58.483Z Reads: 547

```
I will probably want to get between 50-100
```

---
## \#9 Posted by: thisguyhere Posted at: 2018-01-07T03:10:09.595Z Reads: 545

```
i mean, it's a forum for bespoke led flashlights, where they're using 1 to 3 cells to power super bright LEDs.  even in a vape, you're using two, maybe four cells so in these smaller applications, current delivery makes a huge difference.

what we're doing with esk8 is building huge packs to both increase amp delivery and multiply capacity to extend range.

so with these particular cells, it's 3ah which is the same as the 30q, which is also about half the price.  by the time you put a 30q in 3 or 4p configurations, it's delivering enough amperage to sufficiently power these power hungry motors we're using.

yes, the 30t in 3p would deliver over 100a safely.  in a dual drive, you'd be supplying 50a to each vesc, which also happens to be approaching the amp limit, but then the total capacity is still 9ah, which in a practical sense would get you about a 15 mile range.
```

---
## \#10 Posted by: Pedrodemio Posted at: 2018-01-07T03:17:37.211Z Reads: 487

```
They really shine in a low parallel count, for a short commute board a 10S1P or 12S1P wound be amazing
```

---
## \#11 Posted by: notepad Posted at: 2018-01-07T03:17:44.581Z Reads: 478

```
The only way I can see these useful for Esk8ing is for small battery packs w/ high Amperage output, or for cheap runaround boards.  Personally I would love to see a cell get released which is half the amp output, double the mAh -but we will have to wait to see if someone develops one
```

---
## \#12 Posted by: McPickle Posted at: 2018-01-07T03:19:00.473Z Reads: 470

```
I guess it comes down to priorities. These cells are good for a small and light pack (e.g 12s2p) with slightly more power than a 12s5p made with 30q cells. Of course the range will be less than half but again, priorities. ;)
```

---
## \#13 Posted by: thisguyhere Posted at: 2018-01-07T03:20:17.374Z Reads: 452

```
exactly. but sanyo has same sized cells with high output at 4.5ah, I'd go with those so you get the best of both worlds. 

I think with a bit of patience, in a year or two, we'll see this format cells with way more impressive figures start to show up.
```

---
## \#14 Posted by: Pedrodemio Posted at: 2018-01-07T03:30:42.082Z Reads: 451

```
In this case really depend on the current you need, I've run so far 20A battery current on an NCR18650B, it's been enough for me, sags a lot, but works, so running 15A on the NCR2170B may be enough if you encounter moderate climbs on the way

But, due to the higher internal resistance o 2170B you only get 12,5 Wh versus 10,5 Wh on the 30T with much higher discharge capability

In my opinion where the 30T really shines if for pedal assist ebikes, with a minuscule pack you can have high power for when you encounter hill and your legs do the rest of the job on flat
```

---
## \#15 Posted by: b264 Posted at: 2018-01-07T03:35:53.199Z Reads: 429

```
Unless you're looking to make a 2P or 1P, the Samsung 30T don't make sense.  I made a spreadsheet comparing different cells, and the 30T was one of them.  At this price,

high parallel is 6P or more, assuming at least 60A load, minimum

If you're looking for energy per Euro at high parallel, they're only 576mAh/€ whereas the Samsung 35E is 1278mAh/€.
If you're looking for energy per Euro at low parallel, the Samsung 30Q is the best at 1091mAh/€
If you're looking for energy density, by mass, they are only 23.0g/Ah whereas the LG MJ1 are 13.4g/Ah

TL;DR
To make a small board, use 30T
To make a cheap board, use 30Q
To make a long-range board, use 35E
To make a light board, use MJ1

Once the 40T are available this could change drastically
```

---
## \#16 Posted by: uigiroux Posted at: 2018-01-07T03:40:06.726Z Reads: 395

```
What about the Sanyo 20700A, or the Samsung 21700 48G?
```

---
## \#17 Posted by: b264 Posted at: 2018-01-07T03:44:08.040Z Reads: 398

```
I checked the Sanyo NCR20700B (wasn't better at any category) but didn't have info on Samsung 21700 48G or Sanyo 20700A

How many grams per cell?  How many euros per cell at 100 quantity? How many amperes continuous discharge? How much capacity in mAh?
```

---
## \#18 Posted by: uigiroux Posted at: 2018-01-07T03:46:19.451Z Reads: 406

```
This was said about the Sanyo 20700A 

Conclusion

This battery is a very good battery and one of the best high current cell I have tested to date. At lower current there is no reason to use this cell (Instead use the NCR20700B cell), only when the current is above 10A is this cell interesting.

http://www.candlepowerforums.com/vb/showthread.php?432105-Test-review-of-Sanyo-NCR20700A-3100mAh-(Red)
```

---
## \#19 Posted by: uigiroux Posted at: 2018-01-07T03:49:48.021Z Reads: 392

```
Samsung 48G

https://endless-sphere.com/forums/viewtopic.php?f=14&t=90515
```

---
## \#20 Posted by: uigiroux Posted at: 2018-01-07T05:50:11.925Z Reads: 377

```
Any thoughts on those last two batteries?
```

---
## \#21 Posted by: kane Posted at: 2018-01-07T06:11:33.537Z Reads: 349

```
I would love to see that spreadsheet. Care to share it?
```

---
## \#22 Posted by: b264 Posted at: 2018-01-07T07:20:29.885Z Reads: 348

```
Won't let me upload spreadsheets (ods files) here; says photos only
```

---
## \#23 Posted by: b264 Posted at: 2018-01-07T07:29:43.495Z Reads: 357

```
They're calling the Sanyo NCR20700A a "high current cell" but the only rating I can find is 6A and that's from 2008.  And I don't know where to even buy it


The 48G's claim to fame would be "grams per amphour" if not for the LG MJ1 being better for that metric.  The 48G doesn't seem to offer any benefits to esk8.

Stick with 30Q for 3P to 6P, and 35E for 7P or more

30T make sense for 2P only
```

---
## \#24 Posted by: b264 Posted at: 2018-01-07T07:32:02.654Z Reads: 348

```
edit: this info is out-of-date now, beware

<img src="/uploads/db1493/original/3X/5/5/559ea29fb837478f7bee7858b58f166a4c330a3d.png" width="690" height="70">
```

---
## \#25 Posted by: chuttney1 Posted at: 2018-01-07T07:37:11.818Z Reads: 340

```
Good thing I manage to figure out that level status. Imma get these cells when they release cause I need to drop from 24 cells to 50 cells. I know I'll get shafted for capacity for a 12S2P configuration.
```

---
## \#26 Posted by: pixelsilva Posted at: 2018-01-07T16:45:31.189Z Reads: 334

```
So Brian, for my 44" inch Mauna Super Cruiser, long range around the bay, and San Francisco Hills, the 35E will be the best battery option?

<img src="/uploads/db1493/original/3X/2/a/2aedb1814d3991870c7e3952da09450b5aac5d0b.jpg" width="281" height="500">
```

---
## \#27 Posted by: thisguyhere Posted at: 2018-01-07T17:56:14.629Z Reads: 311

```
definitely not.

the 35e has continuous discharge of 8a, maybe 10a.  even if you build a 4 or 5p pack, you pack discharge will be limited to 40, maybe 50a pushing it.

going up hills, especially going from a stop up a hill, demands the highest current draw.  limiting your current delivery to 50a, which would be 25a per motor in a dual setup, may not be enough.

in comparison, the 30q in a 4p pack would have 80a continuous, or 40a per motor in a dual setup.
```

---
## \#28 Posted by: Pedrodemio Posted at: 2018-01-07T18:09:25.734Z Reads: 301

```
You forget the diference between battery and motor current, you can easily start on a hill  with 40A, if you use 80A on each motor you can keep that up to 25% duty cycle, at 50% you are down to 40A on each motor, you will not climb the hill at top speed for sure since duty cycle can be roughly linear with % of top speed
```

---
## \#29 Posted by: thisguyhere Posted at: 2018-01-07T18:24:10.335Z Reads: 300

```
I understand, the comparison I was making is for the cells. yes, the 35e has a larger capacity but is less performing. for that same price bracket why under power your board, especially in high power demand builds. 

also, in dual the 35e in a 4p, that'd make it 20a batt max per motor
```

---
## \#30 Posted by: b264 Posted at: 2018-01-07T21:33:43.244Z Reads: 302

```
[quote="pixelsilva, post:26, topic:43020"]
So Brian, for my 44" inch Mauna Super Cruiser, long range around the bay, and San Francisco Hills, the 35E will be the best battery option?
[/quote]

Not unless you'll be running at least 7P deep, no.  At 3P to 6P, the 30Q looks better.  At 2P, VTC6 looks better.

Unless you have some unique space restraints (which you might) that limit you to certain numbers of either 18650 or 21700 or 20700 cells, I'd use 30Q
```

---
## \#31 Posted by: pixelsilva Posted at: 2018-01-07T22:49:19.350Z Reads: 313

```
Brian, I was thinking 10S5P...so according to you, that falls into the 30Q, 

...and according to Joe..

> in comparison, the 30q in a 4p pack would have 80a continuous, or 40a per motor in a dual setup.

..that cell also fit my motoring...

<img src="/uploads/db1493/original/3X/4/6/469a4534ae9862e8dbe689f70db818a602e43c1a.jpg" width="690" height="388">
```

---
## \#32 Posted by: uigiroux Posted at: 2018-01-08T03:24:17.124Z Reads: 306

```
I have a question that has probably been asked but I'd like some fresh responses since we have some new much better performing cells available now.

So as it was pointed out earlier, some cells are good for a small pack, other for a large pack, some for their high discharge ability, others for their range, and so on.... SO... is it possible to create day a pack with equal quantities of battery cells?  Like a 
  12s2p Samsung 30T
+12s2p Samsung 30Q
+12s2p Sanyo 20700A/B
-------------
12s6p with mixed mAh, discharge rates, Amps, etc... 

I'm sure this is probably possible, but it's it practical or a good idea at all? 

I imagine it is much simpler using the pack than charging it since some of the batteries have different capacities etc, but if you were to wire each type of battery as it's own so each one can be charged individually, and then be able to combine them to make a 12s6 battery so you have all the positive benefits from each, and then hopefully where each battery is lacking, another battery pack would be able to cover that area, thus creating a battery pack with only pros and the only con being the extra work you'd have to do to charge them separately and then reconnecting them back up, which really would not be difficult at all..  So is this a good idea, had anyone tried anything like this before?  Or is there something I'm missing that makes this is not impossible, nearly impossible?
```

---
## \#33 Posted by: PXSS Posted at: 2018-01-08T03:24:20.459Z Reads: 286

```
Have you tested any of these cells???
Please don't make suggestions based on datasheets of cells you've never used. That's how esk8 ended up with using 25Rs in the first place.
```

---
## \#34 Posted by: PXSS Posted at: 2018-01-08T03:26:34.396Z Reads: 281

```
I suggest looking up why it's a bad idea to mix cells
```

---
## \#35 Posted by: willpark16 Posted at: 2018-01-08T03:33:44.476Z Reads: 285

```
Bad idea man and there's quite a few reasons but simply put some cells have different capacity and discharge so imagine having a 3000 mah and 2500mah cell of course you will run the 2500mah cell down before the 3000mah, that's not including potential problems with cell chemistry and other reasons
```

---
## \#36 Posted by: uigiroux Posted at: 2018-01-08T04:24:47.471Z Reads: 278

```
Got it, thanks for the explanation!
```

---
## \#37 Posted by: b264 Posted at: 2018-01-08T05:16:11.205Z Reads: 289

```
[quote="PXSS, post:33, topic:43020, full:true"]
Have you tested any of these cells???
Please don't make suggestions based on datasheets of cells you've never used. That's how esk8 ended up with using 25Rs in the first place.
[/quote]

Nope; research for my own purposes.  Currently in the process of testing it.  I'd appreciate if you offered constructive criticism instead of destructive criticism.  I could just as easily not say a word and keep this information to myself.  Please let us know your test results!
```

---
## \#38 Posted by: PXSS Posted at: 2018-01-08T15:30:23.966Z Reads: 273

```
I cannot share my test results as they are work related. I can tell you that reading datasheets wrong can lead to big issues..:
```

---
## \#39 Posted by: deucesdown Posted at: 2018-01-08T15:34:49.151Z Reads: 282

```
Official specifications:
Standard discharge capacity: min. 3000mAh (1.5A charge 0.1A cut-off, 0.6A discharge, 2.5V cut-off)
Rated discharge capacity: min. 2650mAh (4A charge 0.1A cut-off, 10A discharge, 2.5V cut-off)
Nominal voltage: 3.6V
Charge voltage: 4.2V
Standard charge: 1.5A charge 0.1A cut-off
**Rated charge: 4A charge 0.1A cut-off**
Max. continuoys discharge: 35A at 25°C
Discharge cut-off voltage: 2.5V
**Cycle life: 250 cycles to 60% at 35A discharge.**
Cell weight: 69.0g max
Cell dimension: Height: Max: 70.40mm, Diamter: max. 21.22mm
Operating temperature (surface): Charge 0°C ~ 50°C (Recommended <45°C), Discharge -20C° ~ 80°C (Recommended <60°C)
Storage temperature: 1 month: -20°C ~ 60°C, 3 months: -20°C ~ 45°C, 1 year: -20°C ~ 25°C

I'm always looking at charge cycles (for true cost calculations) and max charge rate, for brakes (hub motors...). Weird numbers! I guess the spec'ed cycle life is at a bananas discharge rate, probably quite a bit better at 10-20a.

If these 2 numbers were better, it'd sit nicely between 30q and A123.
```

---
## \#40 Posted by: evoheyax Posted at: 2018-01-08T16:03:37.056Z Reads: 269

```
[quote="thisguyhere, post:9, topic:43020"]
3 or 4p configurations, it's delivering enough amperage to sufficiently power these power hungry motors we're using.
[/quote]

That's the problem, they don't... At least, not with out sagging from 4.2 down to 3.2 volts...

These cells are good because unlike at only 15 amps per cell, the 30q goes to 2.65 Ah, while the 30T still goes to 3 Ah.

<img src="/uploads/db1493/original/3X/3/d/3df1bc168c23e1e04fe3d3d1e094139642a3c6a3.png" width="690" height="468">

I don't use 18650's cause I can't get enough power from them. Unless I do a 12s6p, 18650s don't deliver enough power for my 4wd boards. And my board is already 25 pounds with a lipo equivalent to a 12s3p.

So in my case, this cell is much needed.

Also, if you wanted a small, lightweight board with some power still, you can do 12s1p and 12s2p configs and still deliver ok acceleration.
```

---
## \#41 Posted by: Vanarian Posted at: 2018-01-08T16:13:48.956Z Reads: 238

```
Everything as pretty much been said about this cell so next step is being able to confirm availability and prices ? 

30T and 40T are a good compromise for small packs, and powerful with good capacity btw. It's all about each max power needs too (take in account ESC and motor limitations).
```

---
## \#42 Posted by: evoheyax Posted at: 2018-01-08T16:14:02.297Z Reads: 245

```
[quote="b264, post:23, topic:43020"]
30T make sense for 2P only
[/quote]

Again can't get 120 amps from the 30Q without a lot of sag unless it's a 6p config. More sag leads to more amps, which leads to more sag, which leads to more amps, and so on. 

60 amps is too weak for me :)
```

---
## \#43 Posted by: evoheyax Posted at: 2018-01-08T16:17:20.198Z Reads: 245

```
[quote="Vanarian, post:41, topic:43020"]
30T and 40T are a good compromise for small packs
[/quote]

Define small packs? According to @b264, it's a 2p. I'd argue that it's useful in a 3p and 4p config also. Above that, doesn't make as much sense.

Everyone assuming that it's only useful for small configs are ignore the less sag and less wear and tear of the cell. It's not good to pull 20 amps for a 30Q cell for much time. That will shorten their life cycles.
```

---
## \#44 Posted by: Vanarian Posted at: 2018-01-08T16:24:44.511Z Reads: 237

```
Not saying it's not useful for bigger packs (keep in mind ESC and motor limitations), if you got the rig it is a beast for a cell.

But to me @b264 said something relevant : I'd literally run them in 1P or 2P packs because of space and weight constraints. 

It totally fits my bill as 2x12S1P if I were to replace my current 2x8S2P, as far as power rating goes and I save some space while raising max speed. 

Though comparing 32x 18650 cells and 24x 21700 cells, the 21700 comes heavier. It's all about different needs IMHO.
```

---
## \#45 Posted by: McPickle Posted at: 2018-01-08T16:34:00.470Z Reads: 236

```
Not sure, but boosted might using these cells in a 13s2p configuration on the new extended battery.<img src="/uploads/db1493/original/3X/b/3/b30a136b662e4a7ca3f934369c599deee4d2bdcb.jpeg" width="690" height="419"><img src="/uploads/db1493/original/3X/c/a/cae94380caaee110b0764595272b11ec3854ca7a.jpg" width="690" height="387">
```

---
## \#46 Posted by: evoheyax Posted at: 2018-01-08T17:16:07.514Z Reads: 226

```
Lets consider some board options:

4wd, with VESC6, capable of 80 amps per motor, means 240 amps possible.

30Q pack needed: 12s16p, 9216g total
30T pack needed: 12s4p, 3312g total

Another setup:

4wd, with VESC4.12, capable of 30 amps con with bad heatsinks (way more if good heatsinks), that's 120 amps.

30Q pack needed: 12s6p, 3456g total
30T pack needed: 12s3p, 2484g total

A 12s6p board needs to be almost twice as large. Space wise, the 12s6p 18650 is much larger than a 12s3p 21700.

So for me, as someone designing hollow core decks, my latest design that I hope to have samples in hand for in a few weeks, fits a 12s3p of 18650 or 21700 with space for 4x vescs and a bms. I don't need much more space for the 21700 cells. So being able to shrink the number of cells I need is huge for me.

[quote="Vanarian, post:44, topic:43020"]
Though comparing 32x 18650 cells and 24x 21700 cells, the 21700 comes heavier.
[/quote]

That's not a good comparison though. A good comparison would be 2 packs that are the same amp rating (and watthour) numbers, 32x 20Q 18650 cells vs 16x 30T 21700 cells. In this case, 1536g vs 1104g.

So if your after performance with less weight, the 30T is the winner.
```

---
## \#47 Posted by: evoheyax Posted at: 2018-01-08T17:27:39.446Z Reads: 219

```
If your after range, than yes, this is a different story. Weight to range ratio on the 30T cell is higher.

But 6-20 miles (depending on weight and how you ride) is enough for most people, especially in a city.

12s4p is big enough for most people in terms of range. 60-80 amps though, is not enough if you want real power.

The other place I see these cells being used is in mountain boards. They need huge amp discharge rates, just like my 4wd boards need, and they will also benefit largely from these cells.

And again, even if 80 amps is enough for you, your 30Q cells are going to last a fraction of the life cycle of the 21700 30t cell in the same config. So even if you don't need 160 amps, and only 80 amps, your cells will last much longer than the 30Q cells.
```

---
## \#48 Posted by: evoheyax Posted at: 2018-01-08T17:50:54.018Z Reads: 220

```
If you want a weak performing board, stick with the 30Q, it'll do fine for you. But if you actually want to increase performance and the life cycle of your cells, the 30T is better.

I'm ignoring cost aspects, so I know that will come up.

Lets add up the costs of these packs.

Lets assume the 30Q cell is $3 per cell and the 30T cell is $7 per cell.

The 12s16p 30Q pack costs $597.
The 12s4p 30T pack costs $336.

So performance for your buck here, the 30T is cheaper.

Now we look at my second example, which is more practical.

The 12s6p 30Q pack costs $216.
The 12s3p 30T pack costs $252.

So in this case, performance for your buck, the 30Q is cheaper, but not by that much...

Now yes, again, I'm ignoring range. Lets assume at these higher amp draws, the 30Q dies at 2.65 Ah and 30T dies at 3 Ah (As the graph I posted above).

12s16p 30Q is 42.4 consumable Ah.
12s4p 30T is 12 consumable Ah.

And the second example.

12s6p 30Q is 15.9 consumable Ah.
12s3p 30T is 9 consumable Ah.

So yes, if your after range with these high amp ratings, the 30Q yields better results. But these larger 30Q packs need more space and take up more weight than the equivalent amp rated 30T pack to get this range.

If you want high performance with long lasting cells and range, the 12s5p or 12s6p of the 30T pack will be the winner. Long range, high amp rating, and a longer life cycle.
```

---
## \#49 Posted by: uigiroux Posted at: 2018-01-08T17:58:06.882Z Reads: 196

```
That was my opinion also with the 30T cells for a 12s6p configuration.
```

---
## \#50 Posted by: uigiroux Posted at: 2018-01-08T17:59:07.512Z Reads: 196

```
So I have these people contacting me asking if I was still in need of the cells.  Should I ask for a sample first then?
```

---
## \#51 Posted by: b264 Posted at: 2018-01-08T18:00:16.974Z Reads: 200

```
How about comparing 2 wheel drive boards?  Because frankly, I don't pay any attention to 4WD needs.  If you're making a 4WD board, you can fend for yourself LoL

The vast, vast, vast majority of boards are 1WD or 2WD
```

---
## \#52 Posted by: evoheyax Posted at: 2018-01-08T18:00:31.482Z Reads: 199

```
Ask them for samples and see if they are any good. If you need a level 3 to do the group buy, I would be fine with doing so. I just want to confirm these cells are legit, since the world has yet to see them supplied to the masses.
```

---
## \#53 Posted by: evoheyax Posted at: 2018-01-08T18:01:58.048Z Reads: 207

```
In my opinion, 4wd bards will become much more popular in the coming year.

For 2wd boards, lets assume the VESC 6 case, which means 160 amps:

30Q pack needed, 12s4p, 2304g, $144, 10.6 consumable Ah.
30T pack needed, 12s2p, 1656g, $168, 6 consumable Ah.

And the 2wd VESC 4.12 case, which means 60 amps:

30Q pack needed, 12s3p, $108, 7.95 consumable Ah
30T pack needed, 12s2p, $168, 6 consumable Ah (rate to 80 amp instead of 60, since 60 is not divisible by 40)

In this case:

If your priority is minimizing space and weight while maintaining power, the 30T is a better cell.
If cost and range is your priority while maintaining power, the 30Q cell is a better cell.

This also doesn't take into consideration the extra wear and tear done on the cells by running them close to their limits.

I will look more into the life decrease of these cells but the numbers I remember seeing said 1200 life cycles if you only do 10 amp per cell, vs 300 cycles at 20 amp per cell with the 25r. I'm assuming that mostly carries over to other 18650s, since it's the same battery chemistry. If you take this into consideration, the 30T in a 12s4p vs 30Q in a 12s4p might last 3 times as long. So even price wise, you might be better with the 30t...
```

---
## \#54 Posted by: Vanarian Posted at: 2018-01-08T18:06:50.043Z Reads: 216

```
I agree with your point for 4WD dragsters and I see your point about my comparison (why compare 12S to 8S) but here I reason in terms of max continuous wattage. 

I don't use 30Q I use HB2 btw (I think we've already discussed this) so I'm closer to your setup than mainstream setups seen here.

My Wh figures are also interesting because 2P HB2 = 1P 30T (again 30T might hold the charge longer so maybe a bit less).

I seek minimum 3200W continuous as conservative rating (means : battery should not exceed 80 degrees).

8S4P of my cells = 1376Gr and I can pull the 3200W continuous easy.

16x 30T in 8S2P will give me an average 2350W max continuous so it's under my goal. I want more.

24x 30T in 12S2P will give me an average 3360W max continuous !  And 24x 30T 21700 = 1656Gr so I still carry 280Gr more. That's more relevant to me.

_Note that a 10S2P brings me a bit under my goal_, 3060W average continuous. It weights 1380Gr , 4Gr more.

Let's be fair and add in equation connecting stuff, because there is much more cells to connect with my 8S4P. 

Including connections I'm up at 1424Gr for 8S4P ; I'm at 1687Gr for 12S2P ; **I'm at 1411Gr for 10S2P**

So I could switch for a 10S2P setup an shave space and 13Gr. But I'd lose an average of 100-200W of max power.

It's all about choices again.

_Edited the 10s2p, previous number was for 1P_
```

---
## \#55 Posted by: evoheyax Posted at: 2018-01-08T18:33:25.473Z Reads: 199

```
8s4p HB2: 8 cells x 4.2 v per cell = 33.6v x 120 (30a per cell x 4 cells) = 4032W

8s2p 30T: 8 cell x 4.2 v per cell = 33.6v x 80 (40a per cell x 2 cells) = 2688W

12s2p 30T: 12 cell x 4.2 v per cell = 50.4v x 80 (40a per cell x 2 cells) = 4032W

The 8s4p of the HB2 and the a 12s2p of the 30T are the same Watt ratings.

This also assumes you can actually get 30 amp per cell from the HB2, and from what I've read, 22a is the max you should pull. In that case, you have less Watts than the 30T cell in a 12s2p config.

Figured out were I went wrong my first time.

I see your point, but honestly the range you get from these HB2 cells are half that of the 30T on paper, probably less in the real world.
```

---
## \#56 Posted by: Vanarian Posted at: 2018-01-08T18:42:04.762Z Reads: 193

```
No problem :wink: but your maths are still wrong : you take the max voltage and max amp discharge where you should account for voltage sag per cell.

So I average different discharge at and below nominal voltage to get a continuous figure. 

HB2 are able to pull 35A under 85 degrees actually and 30A under 78 degrees continuous, for burst it hits harder but since we look for conservative. 

Else you're right, 8S4P of HB2 can hit 4000W continuous if pushing the amps a bit more and so does 12S2P 30T.
```

---
## \#57 Posted by: evoheyax Posted at: 2018-01-08T18:53:30.477Z Reads: 193

```
I see your point of view.

I think the 30T will be most interesting for 4wd boards where you have extra motor and esc power capabilities. I know I'm gunning for them :)

Still, compared to most 18650s, a 12s4p 18650 will have close to the same Watts as a 12s2p of the 30T. Meaning cost is really the only downside to the 30T.
```

---
## \#58 Posted by: Pedrodemio Posted at: 2018-01-08T20:34:44.297Z Reads: 184

```
Not doubting, just curious, are you logging the stats of your board and for how long do these massive current last? in a serious hill did you manage to pull 4000 W all the way?
```

---
## \#59 Posted by: rok Posted at: 2018-01-22T23:08:52.292Z Reads: 181

```
[quote="uigiroux, post:50, topic:43020, full:true"]
So I have these people contacting me asking if I was still in need of the cells.  Should I ask for a sample first then?
[/quote]

Just wondering if there is anything new regarding your inquiry?
```

---
## \#60 Posted by: rok Posted at: 2018-01-24T14:37:30.577Z Reads: 179

```
I´m not saying this is legit but it looks better than any Alibaba seller. 
I found this website that offers **Samsung 30T** 21700 cells. They are located in Israel tho. 
http://www.sdle.co.il/Default.asp?sType=0&PageId=56631

Waiting for his response via Email now. :crossed_fingers:
```

---
## \#61 Posted by: uigiroux Posted at: 2018-01-25T01:16:59.684Z Reads: 179

```
No, they contacted me again and suddenly were saying they didn't have 30T's, just the 48G for 2170's from Samsung.
```

---
## \#62 Posted by: evoheyax Posted at: 2018-01-25T01:28:49.509Z Reads: 173

```
I was in contact with someone who claimed to have the 30T cell. They asked me if I need a legit 30T cell. I said yes, and after contacting many times, I never heard anything again, lol.
```

---
## \#63 Posted by: pixelsilva Posted at: 2018-01-25T09:35:26.935Z Reads: 174

```
People in my forum keep saying the 30Q is much better than the 30T, cheaper, better range and hill climbing. Is all confusing because here all of you have a different opinion.... 30T seem to fit the glove much better. (??)
```

---
## \#64 Posted by: uigiroux Posted at: 2018-01-25T14:54:49.817Z Reads: 175

```
Yeah I don't see how anyone could claim the 30Q is better... The 30T has much higher power..
```

---
## \#65 Posted by: Vanarian Posted at: 2018-01-25T16:15:24.749Z Reads: 184

```
Depends on how many you can pack and which power you need. 

The 30T are heavier and bigger so if you got lot of room for many parallel packs or only need limited continuous power the 30Q are the smartest choice. 

Now if you have limited room for parallel packs AND / or need big continuous power with limited voltage sag, the 30T are unrivaled as far as 18650/20700/21700/26650 cells go.

Note that apart from weight and overall size, a 30T beats a 30Q in every aspects (better range, higher max discharge, low voltage sag, cooler). It sums it up pretty well :slight_smile:

Edit : though  the real contender for e-skate will be 40T!
```

---
## \#66 Posted by: rok Posted at: 2018-01-25T17:27:22.960Z Reads: 175

```
They don't want to sell it to a private customer. Bummer.
```

---
## \#67 Posted by: barajabali Posted at: 2018-02-17T20:19:12.611Z Reads: 168

```
Anyone have any leads on 30t suppliers yet? I need these cells. I don’t want to settle for the Sanyo
```

---
## \#68 Posted by: rok Posted at: 2018-02-17T20:20:47.820Z Reads: 170

```
Second that! :point_up_2:
```

---
## \#69 Posted by: chuttney1 Posted at: 2018-02-17T21:02:52.475Z Reads: 165

```
No leads currently.
```

---
## \#70 Posted by: barajabali Posted at: 2018-02-17T21:05:48.392Z Reads: 175

```
Damnit. 
Sanyo 20700a is also impossible to find.
Sanyo 20650is rated for the same as the 27000a but graphs show other wise. But it’s available...
```

---
## \#71 Posted by: b264 Posted at: 2018-02-17T21:46:27.869Z Reads: 176

```
[quote="uigiroux, post:64, topic:43020, full:true"]
Yeah I don’t see how anyone could claim the 30Q is better… The 30T has much higher power…
[/quote]

Because the 30T are bigger, heavier, and more expensive.  By your logic, a truckload of lead-acid car batteries is better than the 30T
```

---
## \#72 Posted by: uigiroux Posted at: 2018-02-17T22:42:53.013Z Reads: 176

```
Yeah that's precisely my logic, you really nailed that one!  Comparing something that is only 3mm more diameter and barely more weight, it's somehow the equivalent of a truck load of shitty old tech batteries. 

And wtf where is that comment coming from I said that almost a month ago, do you just go around and check threads for things you can troll? Grow up..
```

---
## \#73 Posted by: b264 Posted at: 2018-02-17T22:44:29.067Z Reads: 170

```
Actually, it's 49% heavier and 89.4% more expensive.  Grow up ...

I hadn't checked the thread since then.  I'm not trolling you.  I want to make sure folks see how ridiculous and biased it is if they come and read this later.

There are many reasons a cell can be "better" and simply a higher power doesn't mean much at all without more details.  Hence the truckload of lead comparison.  It's on-point and relevant.
```

---
## \#75 Posted by: barajabali Posted at: 2018-02-17T23:08:17.805Z Reads: 163

```
The 30t is the best possible cell for my current build. Much better than the 30q.  4wd off road trampa with a 12s3p layout. I need super high discharge and 30q won’t cut it. (12s3p is just the on board battery)

It’s all based off of the application. There is no ultimate ‘best’ cel
```

---
## \#76 Posted by: uigiroux Posted at: 2018-02-17T23:11:46.683Z Reads: 161

```
Exactly the same for me.  There is a trade off for the extra weight and cost, you get more power in the long run than you can get from an 18650.
```

---
## \#77 Posted by: PXSS Posted at: 2018-02-18T00:11:46.079Z Reads: 162

```
Why not go for Lipos??? Way more power dense than 30T...

How much power do you need? Post a list of requirements and I can help you do the trade study (if you want).
```

---
## \#78 Posted by: barajabali Posted at: 2018-02-18T00:24:16.042Z Reads: 163

```
My design is already based off of 21700 or 20700 

Thanks for the offer though, I have some backups in case the 30t doesn’t come through
```

---
## \#79 Posted by: uigiroux Posted at: 2018-02-18T00:40:59.331Z Reads: 164

```
I heard the Samsung 30T was coming out mid 2018.  The Sanyo 20700A I read you can find in some power tool battery packs.
```

---
## \#80 Posted by: ZackoryCramer Posted at: 2018-02-18T00:44:56.505Z Reads: 160

```
LOL the wh/$ killed me.
```

---
## \#81 Posted by: barajabali Posted at: 2018-02-18T00:46:45.048Z Reads: 176

```
Yea ? Which ones? I see people selling them on eBay, for like 20 bucks a pop. They’re not even that great 

The 30t is ideal for me. I’ll wait if I have to to be honest. I’ve checked heart every cell on the open market and nothing compares
```

---
## \#82 Posted by: uigiroux Posted at: 2018-02-18T01:14:41.814Z Reads: 171

```
I don't recall, but yeah I'm waiting for the 30T or 40T looks maybe even better... Not sure which to go with..  Have you seen the 40T specs?
```

---
## \#83 Posted by: barajabali Posted at: 2018-02-18T01:17:02.124Z Reads: 172

```
Yea but it’s still not available
```

---
## \#84 Posted by: PXSS Posted at: 2018-02-18T01:20:23.481Z Reads: 180

```
30T vs 30Q

Cons
•42% larger volume. 
•47% heavier. 
•100% more expensive (This is assuming that 30T can be sourced at less than $7 per cell which is unlikely, more likely is these priced at ~$10 at least for a few years)

Pros
•9% more energy at 10A
•Same energy with 30T at 30A and 30Q at 7A (10Wh)
<Still the difference between the two at same current is less than 10%>
•30T gets the same voltage sag as 30Q when running 20A vs 10A. 
•30T runs 0.1V higher than 30Q at 10A due to voltage sag resulting in 3% higher power output at same current. 
•30T runs cooler than 30Q

---

3P30Q vs 2P30T
30T is 5.3% smaller in volume
30T is 1.1% lighter
30T has 27% less energy
30T runs ~0.05V higher @20A & 30A total (Still has higher power density)
30T is 25% more expensive (This is assuming that 30T can be sourced at less than $7 per cell which is unlikely)

---
4P30Q vs 2P30T
30T is 29% smaller
30T is 26% lighter
30T has 45% less energy 
Same power delivery through most of the range (30T still has higher power when under 20% charge)
Same price. (This is assuming that 30T can be sourced at less than $7 per cell which is unlikely)

---
I honestly don't see it. 
If you need that much power, Lipos are more power dense at nearly the same energy density (I have to check on this) at much cheaper
```

---
## \#85 Posted by: Kug3lis Posted at: 2018-02-18T02:35:52.712Z Reads: 167

```
From my opinion, if anyone wants more than 60A from 18650/20700 is playing with fire... Current is not scaling so nicely as you imagine, if you put 2 cells in parallel it does not mean the current will split 50% each can be 70/30 everything depends on the path, every sharp corner makes a problem and etc. I suggest using Li-Poly for high current builds.
```

---
## \#86 Posted by: PXSS Posted at: 2018-02-18T04:05:50.336Z Reads: 173

```
Yay and nay.

[quote="Kug3lis, post:85, topic:43020"]
if you put 2 cells in parallel it does not mean the current will split 50% each can be 70/30 everything depends on the path
[/quote]
Yes it may not be 50-50 but 70-30 is a gross exaggeration. You are talking about 41% higher resistance in one path than the other...

It all depends on the construction of the pack. I make packs that deliver upwards of 130A continuous and burst up to 500A with 18650.

Can it be done safely? Yes
Do I trust most members of this forum to do it safely? No
But that's up to them to decide...
```

---
## \#87 Posted by: Kug3lis Posted at: 2018-02-18T04:07:43.343Z Reads: 164

```
There are a lot of variables on that but it's possible :D But yeah high current paths on DIY packs without knowledge is a bad thing :) That's why I always suggest going for High C rated LiPos so at least cell will hold current :) As many people don't use BMS protection.
```

---
## \#88 Posted by: PXSS Posted at: 2018-02-18T04:11:19.725Z Reads: 164

```
High C rating packs isn't any safer if the builder sucks. 

[quote="Kug3lis, post:87, topic:43020"]
As many people don’t use BMS protection.
[/quote]
Dont even remind me. And for the stupidest reasons too.
```

---
## \#89 Posted by: Kug3lis Posted at: 2018-02-18T04:13:34.672Z Reads: 160

```
I mean simple thing ESC mosfet dies bridges motor on + and - same time, bamn 300A incoming and boom you are pack is on fire :D Because everyone puts oversized wires and connectors when if they had lower rating they could be like kind of protection from high current but now lets go we need current :D
```

---
## \#90 Posted by: PXSS Posted at: 2018-02-18T04:15:12.010Z Reads: 165

```
But dont you dare put a BMS or fuse in line! It wastes too much space! Moar Wires!!!
```

---
## \#91 Posted by: sMATTEr Posted at: 2018-02-18T07:12:42.233Z Reads: 166

```
[quote="PXSS, post:90, topic:43020, full:true"]
But dont you dare put a BMS or fuse in line! It wastes too much space! Moar Wires!!!
[/quote]

Did you make a write up on how to build a batterypack correctly? I thought so but upon searching I realize that it might have been someone else.

You really should though, I’m building my first big battery pack(second pack) and there is so much contradicting information..
```

---
## \#92 Posted by: ElskerShadow Posted at: 2018-02-18T07:25:04.396Z Reads: 159

```
But you have a battey on your backpack right ? So you don’t rely on those cells for range.. just for discharge... 
for me the problem is range /money the 30Q is unbeatable for this
```

---
## \#93 Posted by: barajabali Posted at: 2018-02-18T14:25:17.974Z Reads: 155

```
Exactly I rely on them for discharge. That’s why every cell Has it’s own application
```

---
## \#94 Posted by: PXSS Posted at: 2018-02-18T16:56:23.718Z Reads: 157

```
I've thought about it a lot but I do not have the time to do so, plus nobody here has access to the same equipment I do. 

I may do a guide on my next build with things commonly accessible. The issue is that it takes so much longer and I'm lazy lol. I'll tag you in it if I do decide to make one
```

---
## \#95 Posted by: sMATTEr Posted at: 2018-02-19T15:58:23.026Z Reads: 153

```
Yeah I get that it takes time to make a sufficient guide, right now I’m mostly taking tips from endless sphere where they(atleast to me) seem to have knowledge.

Please do tag me, I’ll post some battery build pics in a couple of weeks when I get the BMS, would be sweet with some input.
```

---
## \#96 Posted by: uigiroux Posted at: 2018-02-19T16:40:06.246Z Reads: 148

```
How do you make a pack that runs 130A with 500A bursts?!  What kind of motor would need that much power and how does that not fry the VESC?
```

---
## \#97 Posted by: PXSS Posted at: 2018-02-19T17:55:25.594Z Reads: 139

```
I'm not using VESC. ;)
Airplanes use a lot more power than esk8... :)
```

---
## \#98 Posted by: uigiroux Posted at: 2018-02-19T18:30:14.851Z Reads: 139

```
Oh right on.  It's there any airplane ESC you can think of that would be useful for Esk8 at 14s-18s or so?
```

---
## \#99 Posted by: barajabali Posted at: 2018-02-19T19:00:35.988Z Reads: 140

```
Plane escs don’t usually have brakes
```

---
## \#100 Posted by: uigiroux Posted at: 2018-02-19T19:01:19.804Z Reads: 140

```
Oh, damn, those are pretty important, lol..
```

---
## \#101 Posted by: PXSS Posted at: 2018-02-19T20:17:51.017Z Reads: 146

```
None for under 2k a piece. We work with custom ESCs. This is for applications way different than esk8. We're talking about 100lbs airplanes.

MGM Compro does have a line of car ESCs for 16S-24S but again, you're talking about 1k each or so.
```

---
## \#102 Posted by: uigiroux Posted at: 2018-02-19T20:38:46.224Z Reads: 139

```
What about T-Motor? I heard there ESC's are super high quality and they're like around $150-$200 or so..
```

---
## \#103 Posted by: PXSS Posted at: 2018-02-19T20:47:00.107Z Reads: 139

```
Never worked with their stuff. They're big in the multicopter agriculture stuff but I don't know more than that...
```

---
## \#104 Posted by: E1Allen Posted at: 2018-02-19T21:29:30.653Z Reads: 145

```
http://www.evassemble.com/index.php?main_page=product_info&cPath=2&products_id=19

14s1p on these monsters.  100a continuous. Discharge 50a charge.

$70 more compared to 12s3p 30q and about 7bs more.  

If only weight was a little lower.
```

---
## \#105 Posted by: chuttney1 Posted at: 2018-03-29T19:42:53.343Z Reads: 144

```
I'm posting here to put in a link to a google spreadsheet for a quantity count if these cells become available. Enter the amount you plan to buy.


https://docs.google.com/spreadsheets/d/160G88FWLQBvPc49P6_jVgvT8bzklGjbxIckWOwvvj_k/edit?usp=sharing
```

---
## \#106 Posted by: uigiroux Posted at: 2018-03-29T19:47:12.402Z Reads: 143

```
Wait they're finally available?  How much per cell?  I'm thinking I'd want between 72-100.
```

---
## \#107 Posted by: b264 Posted at: 2018-03-29T19:51:38.831Z Reads: 141

```
Did anyone ever find discharge graphs for this cell?
```

---
## \#108 Posted by: chuttney1 Posted at: 2018-03-29T19:54:11.528Z Reads: 141

```
They are not available yet, neither is pricing. I just want a cell quantity count so whoever decides the group buy for this community has a number to work with.
```

---
## \#109 Posted by: chuttney1 Posted at: 2018-03-29T19:58:01.333Z Reads: 145

```
http://lygte-info.dk/review/batteries2012/Common18650comparator.php

and mooch did testing
https://www.e-cigarette-forum.com/threads/samsung-inr21700-30t-35a-3000mah-21700-bench-test-results-an-incredible-battery.798683/
```

---
## \#110 Posted by: moon Posted at: 2018-03-29T19:59:12.466Z Reads: 140

```
I think google form is better than this
```

---
## \#111 Posted by: uigiroux Posted at: 2018-03-29T20:04:08.928Z Reads: 140

```
I want to do a 12s6p build with these.  That should be pretty insane power!  Lol...
```

---
## \#112 Posted by: mmaner Posted at: 2018-03-30T14:15:14.345Z Reads: 135

```
That's a good way to kill yourself.  I would suggest you build a board and get some perspective before building something that ridiculously overpowered.  I mean, unless you weigh 600 lbs and wanna 200 mile range.
```

---
## \#113 Posted by: uigiroux Posted at: 2018-03-30T14:58:50.784Z Reads: 145

```
Kill myself?  How is building a large pack out of these any different than others who build large packs from any other battery?  I mean the more I parallel you have the less voltage sag you have, and the more batteries the more range and more accelerating I can do.  Is this really that unusual?  Is it just this specific cell that makes you say that or what exactly is it.  I've heard many say this cell would be great for a 12s2p pack, but why wouldn't it be equally as good in an even larger pack?
```

---
## \#114 Posted by: Jammeslu Posted at: 2018-03-30T15:09:19.770Z Reads: 140

```
It will if you have the money but otherwise hellll nooo
```

---
## \#115 Posted by: ElskerShadow Posted at: 2018-03-30T15:16:03.890Z Reads: 139

```
By reading many of your posts I kinda feel you change your builds plans every day :p
```

---
## \#116 Posted by: uigiroux Posted at: 2018-03-30T15:16:18.324Z Reads: 141

```
How much are the cells expected to cost? People are making packs from the Sanyo 20700A which is like $13/cell.
```

---
## \#117 Posted by: mmaner Posted at: 2018-03-30T15:18:13.879Z Reads: 146

```
Have you skated an electric board for any amount of time?  You need some perspective.  There's maybe 5 people on this forum that could handle the juice a 12s6p li-ion pack has the potential for.  Not to mention the difficulties in housing a pack that large.  

1st, you will likely need to fabricate your own enclosure for a pack that size.
2nd, you will likely eat a few VESC's running those kinds of parallel amps...if you the packs potential
3rd, ride a 10s3/4p and see if that's enough for you before you spend 2 grand building one
```

---
## \#118 Posted by: uigiroux Posted at: 2018-03-30T15:36:38.136Z Reads: 142

```
In getting one of the LaCroix boards, they're specifically made the enclosure to fit 12s6p. Also I'll be using ESCape's, so I am quite confident they'll be able to handle the power.  However I did just make a new thread regarding the A200S 16s 200A VESC, hoping someone will make one here for much less, like the ESCape and B-box did for the VESC 6.
```

---
## \#119 Posted by: mmaner Posted at: 2018-03-30T16:25:44.596Z Reads: 146

```
[quote="uigiroux, post:118, topic:43020"]
I am quite confident they’ll be able to handle the power
[/quote]

Your likely correct, but that's not the issue.  The issue is can YOU handle the power?  I repeat...

[quote="mmaner, post:117, topic:43020"]
There’s maybe 5 people on this forum that could handle the juice a 12s6p li-ion pack has the potential for.
[/quote]
```

---
## \#120 Posted by: uigiroux Posted at: 2018-03-30T16:32:16.258Z Reads: 140

```
I'll take my chances. :wink:  Yes I'm sure there will be a learning curve, but I highly doubt it's something that I won't be able to operate.  Also, I've read more builds than I can count where they use a battery pack the same size or greater... Where are you getting this statistic that roughly only 5 members on the forum can handle a battery pack of that size?
```

---
## \#121 Posted by: mmaner Posted at: 2018-03-30T16:50:12.073Z Reads: 141

```
I'm just trying to get you look for some perspective.   Im getting my statistics from having ridden for 30 plus years, built 16 electric boards in the last 2 years and calling bullshit on...

[quote="uigiroux, post:120, topic:43020"]
I’ve read more builds than I can count where they use a battery pack the same size or greater
[/quote]
```

---
## \#122 Posted by: uigiroux Posted at: 2018-03-30T16:59:50.094Z Reads: 142

```
Ok well I'm not going to argue.  I've seen plenty of people say they're making a pack that size or greater.  Can bs if you want I don't see the point.  I've ridden the last 25 years of my life but am doing my first build now.  Is this supposed to be a pissing contest?  If I want to build a battery pack a certain size that's my business.  This forum is here to help educate.  If you're trying to help me by advising me on another direction, I think being polite and stating your reasons would work much better, rather than trying to belittle me or how much experience I have riding vs you...

Regardless, I'll do some research and consider what you've said, thank you.
```

---
## \#123 Posted by: mmaner Posted at: 2018-03-30T17:03:22.260Z Reads: 151

```
[quote="uigiroux, post:122, topic:43020"]
I’ve seen plenty of people say they’re making a pack that size or greater.
[/quote]
There are very few packs of that size, I'm interested in the countless/plenty you are referencing.

[quote="uigiroux, post:122, topic:43020"]
If you’re trying to help me by advising me on another direction, I think being polite and stating your reasons would work much bette
[/quote]
I did that, you argued.  I began with trying to explain that using that kind of amp delivery is almost impossible and you said I was wrong.  I mean, I've only built 30 grand worth of boards in the last 2 years, guess I don't know shit.

[quote="uigiroux, post:122, topic:43020"]
rather than trying to belittle me
[/quote]

Nobody, specifically me was trying to belittle you.  Once again, was just trying to give you some perspective.

I really have a hard time understanding how people ask for info, you give it to them, they wanna argue about it...
```

---
## \#124 Posted by: uigiroux Posted at: 2018-03-30T17:12:32.890Z Reads: 149

```
I didn't argue, I simply said that the board and enclosure I was getting was made for that setup.  I could easily go through the build threads and find more than 5 builds with battery packs that size or greater.  And the way you say you "tried to explain" this and that to me, it came off as rude, hence why I said it felt like you were trying to belittle me.

REGARDLESS 

I'm done commenting on this as it is not contributing at all to the thread.  Can we leave it at that?
```

---
## \#125 Posted by: Instinct0224 Posted at: 2018-03-31T19:00:54.866Z Reads: 140

```
I live in Houston looking for a spot welder any ideas?
```

---
## \#126 Posted by: uigiroux Posted at: 2018-03-31T21:59:08.702Z Reads: 144

```
Well unfortunately they're not carried at any hardware store.  If I had one yet I'd let you borrow it, but I haven't ordered one either.  Basically you can go online and order one of those large ones like a Sunko but there about $150-$200, or there is the one you can order off this forum for roughly $100.  I was thinking of doing the small one on the forum, but I got on YouTube and Googled how to make one, and it's actually pretty easy it looks like, basically need a car battery and then a few other things, but that's probably the quickest, cheapest way.  Otherwise search for it on the forum and it's not too hard to order, the one problem is it has to ship from like Korea I think.
```

---
## \#127 Posted by: Instinct0224 Posted at: 2018-04-01T02:26:06.924Z Reads: 149

```
You don't have any friends that have one huh..i don't want to buy one..i rather dig up and try to see if anybody has one..i created a profile here to look for somebody that has one..i'll ask around..if you get to it let me know..i want to do it for i can pay like 15 bucks for somebody to solder some 18650...
```

---
## \#128 Posted by: uigiroux Posted at: 2018-04-01T02:42:35.831Z Reads: 155

```
Well that's what I originally planned, I asked on this forum if I could rent one from somebody for like a week but the point was made that the cost of just buying the one sold on the forum would pay for itself very quickly.  Unfortunately from what I've seen, battery packs are the most overpriced, marked up items that are sold in the Esk8 world...  The most used battery is the Samsung 30Q which is about $3.50.  You could buy the cells yourself and make the battery pack and it would only cost a couple hundred, plus you could continue to make battery packs as needed with the spot welder.  However if you buy a battery pack through someone else, almost every one I've seen basically charges $10 per battery.  So if you got a 12s4p battery, you would pay around $480.  But if you made it yourself, the batteries would only cost like $170 and then if you used a BMS that's like $60, plus the wires and nickel strips, you would probably in total pay about $240, so easily save half in that case...
Here's the link to that spot welder. 

http://www.electric-skateboard.builders/t/boss-level-custom-spot-welder/25980

I wish it was possible to pay someone that amount to make a battery pack but unfortunately that's just not likely to happen...
```

---
## \#129 Posted by: Instinct0224 Posted at: 2018-04-01T02:57:30.022Z Reads: 152

```
I know i got over 100 cells 18650 2600 for 1.25 each here in Houston...got a great deal..but i want to build my own batter pack..bms is on the way..i already have the cables but no spot welder..plus is a hobby and i don't think i would use it forever and if you craiglist it..your not going to get @ least 50% of what you paid for..so what do you think we should do...you want to split the difference? then we can rent it here?? the only issue here i don't know you..lol...oh, yea i looked into that one already..looks good..so i'll think about getting that..good spot welder are expensive..i already email the guy..
```

---
## \#130 Posted by: uigiroux Posted at: 2018-04-01T04:53:07.996Z Reads: 157

```
I'd be open to that but I'm currently in Nebraska for awhile, don't know when I'm going to be getting back to Houston.  Hopefully I'll miss the miserably hot humid summer and make it just in time for fall and have my board all ready to ride :smile:
```

---
## \#131 Posted by: Vanarian Posted at: 2018-04-03T11:04:34.387Z Reads: 150

```
Bit back on track of the topic, @PredatorBoards @uigiroux guys I got an e-mail today from a seller claiming he has 21700 30T and 40T in stock, rewraped. 

Never asked him about these cells (back in the days I contacted him for 18650 models) so maybe just a pebble in the ocean, or a legit seller. I asked for samples to confirm specs, if he contacts me again I'll report for you guys.
```

---
## \#132 Posted by: uigiroux Posted at: 2018-04-03T11:25:19.203Z Reads: 150

```
Why would anyone rewrap a brand name cell?
```

---
## \#133 Posted by: Vanarian Posted at: 2018-04-03T13:02:16.541Z Reads: 152

```
Many possible reasons : contract to not sell under brand name (if cell is reserved for manufacturers), self visibility of the seller, etc... No news yet though.
```

---
## \#134 Posted by: uigiroux Posted at: 2018-04-03T13:08:36.684Z Reads: 150

```
Oh right on.  Did you get a rough price quote, or not sure yet?
```

---
## \#135 Posted by: Vanarian Posted at: 2018-04-03T16:58:42.876Z Reads: 143

```
Just got a quote, on the expensive side for now. 10.9$/cell 30T and 11$/cell 40T. Need to check Qty prices.
```

---
## \#136 Posted by: uigiroux Posted at: 2018-04-03T17:28:19.641Z Reads: 147

```
Were you able to peel the label off and see if it said Samsung?
```

---
## \#137 Posted by: chuttney1 Posted at: 2018-04-03T17:31:34.007Z Reads: 150

```
This was to be expected with low volume of supply. I would wait to pay half that price if I can wait.
```

---
## \#138 Posted by: Vanarian Posted at: 2018-04-03T18:54:38.463Z Reads: 146

```
Edited my post, only got quote for now.
```

---
## \#139 Posted by: Pedrodemio Posted at: 2018-04-04T02:37:26.223Z Reads: 145

```
I would be cautious mainly with the 40T, most reviews say that it would only be available mid of the year, that plus the rewrap doesn’t inspire confidence

But I’m anxious to my hands on them, 9S1P and I have the lightest board that is enough for my commute
```

---
## \#140 Posted by: Vanarian Posted at: 2018-04-11T12:51:18.781Z Reads: 140

```
Well they're sending them to Mooch for review so looks legit but still it is expensive. I'll hit them a message to see what's up (they contacted me again) didn't have time this week.
```

---
## \#141 Posted by: Eboosted Posted at: 2018-04-12T04:48:24.463Z Reads: 136

```
How much did they quote each cell?
```

---
## \#142 Posted by: Vanarian Posted at: 2018-04-12T07:20:29.767Z Reads: 136

```
10.8$/ Samsung 30T
11$/ Samsung 40T

Apparently this is the real stuff though : 

https://www.e-cigarette-forum.com/threads/bench-test-results-vapcell-purple-3100mah-35a-21700-appears-to-be-30t-an-incredible-35a-cell.859091/

At 35A 65 degrees and this voltage level, cannot be a fake cell.
```

---
## \#143 Posted by: NickTheDude Posted at: 2018-04-12T07:31:44.413Z Reads: 134

```
Damn, a 12S1P of these would be perfect for my Jet Spud commuter build. I don't need the range so this would probably work out to around the same power and (hopefully) less weight than a 12S2P of 30Qs. A little cheaper too, and in a smaller package.
```

---
## \#144 Posted by: Vanarian Posted at: 2018-04-12T07:41:57.638Z Reads: 132

```
Hit them a message (Szyfe Vapcell something)? Too expensive for me as is :x can't justify the price haha
```

---
## \#145 Posted by: evoheyax Posted at: 2018-04-17T03:29:44.076Z Reads: 125

```
They are live boys at $18 USD a pop:

https://www.imrbatteries.com/samsung-30t-21700-3000mah-35a-battery/

Only can buy 12 right now, but means bulk will be soon. Wish I had a way to get enough together for a 12s4p build.
```

---
## \#146 Posted by: Deckoz Posted at: 2018-04-17T03:51:17.191Z Reads: 122

```
[quote="uigiroux, post:128, topic:43020"]
battery packs are the most overpriced, marked up items that are sold in the Esk8 world…
[/quote]

I know this is old... But tell me how many hours it took to build your pack when you finish it ;)
```

---
## \#147 Posted by: b264 Posted at: 2018-04-17T03:54:35.858Z Reads: 120

```
[Samsung 21700 40T](https://www.imrbatteries.com/samsung-40t-21700-4000mah-30a-battery/) are live at $20.00 each, max 6
```

---
## \#148 Posted by: uigiroux Posted at: 2018-04-17T04:10:23.902Z Reads: 118

```
I will be sure to tell you that as soon as I build one.  Just for a little perspective though, how is it justified to charge for a battery pack that takes a couple hours, or even a day, what a set of 2WD or 4WD Hummie Hubs costs with over a years worth of R&D and work put into them?
```

---
## \#149 Posted by: willpark16 Posted at: 2018-04-17T04:28:18.931Z Reads: 119

```
Often higher battery prices are attributed to warranty, longhairedboy has some expensive shit!!!! But once you buy it you’re golden and have a great warranty which is essential in this game, and a crazy mastermind genius that likes building fast popsicle sticks
```

---
## \#150 Posted by: evoheyax Posted at: 2018-04-17T04:29:53.435Z Reads: 121

```
[quote="uigiroux, post:148, topic:43020"]
over a years worth of R&D and work put into them
[/quote]

2.5 years 10 char
```

---
## \#151 Posted by: uigiroux Posted at: 2018-04-17T04:32:30.391Z Reads: 119

```
Exactly...
```

---
## \#153 Posted by: DeathCookies Posted at: 2018-04-17T12:11:59.304Z Reads: 118

```
[quote="Deckoz, post:152, topic:43020"]
I dont like thier business model.
[/quote]

What Business Modell?
```

---
## \#154 Posted by: Pr0dy Posted at: 2018-04-17T12:14:48.523Z Reads: 115

```
The one in which customers are satisfied
```

---
## \#156 Posted by: uigiroux Posted at: 2018-04-17T12:32:05.702Z Reads: 116

```
You don't have to like their business model to understand the comparison I'm making between developing a product from scratch and putting years of work and R&D into something compared to building something from premade parts that takes at most a day.

Substitute whatever you want in their that costs a similar price and took about the same time to develop.

There you go, can you understand this terribly complex comparison now..?
```

---
## \#158 Posted by: uigiroux Posted at: 2018-04-17T12:38:32.171Z Reads: 108

```
Regardless of what product you want to compare it to, it literally makes no difference if you like their business model.  Use e-toxx, fatboy,  Carvon, Trampa, whatever!  You don't get to pretend to be ignorant of something because you don't like their business model.  You admitted that you have read there thread, so you clearly do know the difference.
```

---
## \#159 Posted by: uigiroux Posted at: 2018-04-17T12:40:44.609Z Reads: 107

```
By your very own words of only getting out of bed for nothing less than $75/hr, then those products should be priced at like $500,000 a set if your going to insist that's how the market should be.
```

---
## \#162 Posted by: uigiroux Posted at: 2018-04-17T12:44:19.859Z Reads: 104

```
Ok, have fun living in fantasy land...  I am not wasting my time on this pointless debate, your clearly just disagreeing for the sake of disagreeing.
```

---
## \#163 Posted by: uigiroux Posted at: 2018-04-17T12:45:57.512Z Reads: 108

```
Lol, that's not what insinuating means but ok.  Also, if that's your point, then why are you arguing that batteries are worth so much then?
```

---
## \#164 Posted by: Deckoz Posted at: 2018-04-17T12:50:42.107Z Reads: 107

```
... I'm not insinuating they are worth so much.. but do you want someone getting paid minimum wage getting paid to make your battery and hope it won't burn your house down?
```

---
## \#165 Posted by: Pr0dy Posted at: 2018-04-17T12:52:02.314Z Reads: 108

```
Guys let’s stick to the topic. Create a new thread if all you want to do is bash each orher
```

---
## \#166 Posted by: uigiroux Posted at: 2018-04-17T12:53:33.402Z Reads: 118

```
Also your pricing out of a battery is exactly my point.  This is a DIY forum!  Yet the thing that can be built after a few hours of YouTube videos and general reading and save you the most money, the battery, is the most commonly not made DIY item. That is my point.  It costs $200-$300 to buy the parts and make one.  We bitch about the cost of a VESC 6 yet have no problem spending twice that on a battery we could build for the price of a ESCape.  Then, instead of people getting the good ESC's, they have to get cheaper ones cause they spent so much on the battery...
```

---
## \#167 Posted by: uigiroux Posted at: 2018-04-17T12:54:24.888Z Reads: 115

```
Your right, I'm sorry.
```

---
## \#168 Posted by: mmaner Posted at: 2018-04-17T13:01:03.372Z Reads: 115

```
[quote="uigiroux, post:166, topic:43020"]
We bitch about the cost of a VESC 6 yet have no problem spending twice that on a battery we could build for the price of a ESCape.
[/quote]

An ESCape or VESC6 cant burn your house down if it is built incorrectly.  Does it occur to you that you just spent an hour arguing with people that have actually bought and built a battery when you have yet to buy or build one?  Does this not seem a little tedious and pointlessly argumentative to you?
```

---
## \#169 Posted by: uigiroux Posted at: 2018-04-17T13:03:56.664Z Reads: 116

```
As it was pointed out just now we're derailing the thread.  I'd be happy to discuss this with you in PM.
```

---
## \#170 Posted by: uigiroux Posted at: 2018-04-17T13:44:54.086Z Reads: 119

```
Are the prices you got for the cells that were resleeved still the same... Cause if they are, then that's these 30T and 40T cells at much much less, just under a different brand name, but still the same cells... Right? 
![Screenshot_20180417-084115|349x500](upload://13EgH3vILR3dxdkLcE6Svc1bcr1.jpg)
```

---
## \#171 Posted by: Vanarian Posted at: 2018-04-17T23:34:58.072Z Reads: 110

```
Yep still same prices. 

@Deckoz finally you did change that thumbnail ! Who the hell are you now lol
```

---
## \#172 Posted by: Deckoz Posted at: 2018-04-17T23:36:01.576Z Reads: 109

```
A space man lol
```

---
## \#173 Posted by: evoheyax Posted at: 2018-04-18T05:06:45.852Z Reads: 119

```
[quote="Deckoz, post:157, topic:43020"]
No… because I don’t support this.

but getting money, running out of money, asking for more money, people still don’t have things
[/quote]

Not like we've asked anyone who paid for more money (except when it comes time to ship, since our prices don't include this). If they paid $400 a year ago, they are getting them for $400 + shipping. Instead, we find new customers. It's not like we don't have motors going to together every day. WE'd love to have parts in stock, everyone building a product from the ground up wishes they had inventory. But we have to test the machining places ability to meet specs, and the parts need to be tested, and the assembly process needs all the kinks worked out. These things take time. Their will be a day in the not too distant future where we get inventory. We might be supplying motors to a few large non-electric board companies turning electric, plus we're working on our own completes, and that'll help to keep things in stock for the community to use also. We are building this into a full time job, with the hope of transitioning within the coming weeks. We're getting ready to order the next round of motor parts as we speak, so we won't be out of stock for too long once these are shipped out. We have a few customers that will be receiving theirs within the next 2 weeks (because they want to do their own wheels, and that's the real hold up at this point. It takes time to test. 100 miles so far, no deterioration of core and no chunking of the wheels). We could have shipped stuff 6 months ago, but they were 2/3rds of this motor or less in terms of quality and design. We don't want anyone to be disappointed.
```

---
## \#174 Posted by: Eboosted Posted at: 2018-04-18T05:21:54.142Z Reads: 108

```
[quote="Vanarian, post:171, topic:43020"]
@Deckoz finally you did change that thumbnail ! Who the hell are you now lol
[/quote]

He is Daft Punk cousin
```

---
## \#175 Posted by: E1Allen Posted at: 2018-04-18T05:41:36.752Z Reads: 112

```
[quote="Deckoz, post:172, topic:43020, full:true"]
A space cadet lol
[/quote]

I agree with the whole burn down the house battery build thing.  Which is why people pay good money for a good battery pack. Plus it's time consuming to build.
```

---
## \#176 Posted by: Exiledd_Top Posted at: 2018-04-18T05:53:40.591Z Reads: 119

```
[quote="E1Allen, post:175, topic:43020"]
people pay good money for a good battery
[/quote]

In my opinion I think its like a real world a service that they can provide with there skilled knowledge and the equipment they have to making there life's easier. 
Its to factor ones time , there skill, warranty, and equipment cost. 
You can argue that yes its cheaper but you'd need to buy a spot welder for a one time use. Sure you can "look up youtube " and learn yourself for a one time use , but your going to mess up one way or another from learning and I am not willing to have a mess up on a battery can catch fire and   can cost me my entire build , so I understand that given that I will only need one battery pack, and will need to buy equipment, and study /watch vidoes about battery packs , given that I will mess up along the way with 12-16 hours to make after wards for a one time thing , I value my own time and I'd rather pay for the safety of knowing its well built , has warranty and was done with the right equipment
```

---
## \#177 Posted by: Vanarian Posted at: 2018-04-18T08:31:36.607Z Reads: 116

```
What about solderless instead then. You save time and money, no special tools. Insert in the good direction, latch it and voilà. For BMS & connector, solder wires to the strips before assembly with a good ol iron. Should shave many hours from your schedule. 

Anyway people **should** know a set standard about what they're using / buying or what they are building, and spend time looking tutos. Should be a golden rule even for pre-built boards. 

Did you follow the story of that kid plugging a high voltage charger in his 21v Riptide? It did happen because of ignorance. Not asking to be MIT, just a basic set of understanding.
```

---
## \#178 Posted by: Deckoz Posted at: 2018-04-18T15:11:17.826Z Reads: 120

```
What about this guy

https://www.liveleak.com/view?t=uVwGx_1524035828
```

---
## \#179 Posted by: uigiroux Posted at: 2018-05-08T15:35:29.358Z Reads: 116

```
I've been looking at all the websites that are selling the Samsung 30T and 40T, and they are crazy expensive at $18 and $20 a cell.  I found another cell that seems very good, but it's not a brand I'm familiar with.  Does anyone know anything about this battery or the brand?

https://www.imrbatteries.com/imren-21700-4800mah-battery/
```

---
## \#180 Posted by: Colson003 Posted at: 2018-05-08T15:57:02.330Z Reads: 111

```
I’m gonna go ahead and guess that’s a Samsung 48g rewrap. 4800mah and 8a max.
```

---
## \#181 Posted by: uigiroux Posted at: 2018-05-08T16:13:24.889Z Reads: 109

```
But it says it has 30A, that's much more than the 48G.
```

---
## \#182 Posted by: Colson003 Posted at: 2018-05-08T16:17:51.195Z Reads: 110

```
It’s a rewrap. They can put whatever they want on the wrapper. Doesn’t change what the cell can handle.
```

---
## \#183 Posted by: E1Allen Posted at: 2018-05-08T16:48:25.014Z Reads: 113

```
I'd recommend you visit here for your future battery questions.  
1. This guy has probably tested every battery for most of the sizes we use.
2. Rarely do you see eskate users picking batteries outside of the top five you see on the forum.

https://www.e-cigarette-forum.com/threads/bench-test-results-imren-30a-4800mah-21700…useless-30a-rating.844615/
```

---
## \#184 Posted by: uigiroux Posted at: 2018-05-08T17:00:30.595Z Reads: 111

```
Hey thanks for the link!  

Regardless of the price, what cell do you guys think the best cell currently available is? Excluding the Samsung 30T and 40T.  I guess regardless of price, with the exception of those two, as they are just comically over priced...
```

---
## \#185 Posted by: uigiroux Posted at: 2018-05-08T18:48:12.794Z Reads: 113

```
So I was just reading some of the tests they did on that site and one of them was for what they thought to be a rebranded Samsung 40T (which he also said that very is pretty much the most powerful cell out currently), the Vapcell Gold 4000mAh 30A 21700.  On some sites it's going for $17.99, which is better than the $20 price tag I've seen.  I looked some more and they have it on alibaba...  for between $10-12

https://www.google.com/amp/s/m.alibaba.com/amp/product/60748141212.html

I've never used alibaba though, so I don't know if that is reliable or not.  What do you guys think?
```

---
## \#186 Posted by: E1Allen Posted at: 2018-05-08T21:42:56.234Z Reads: 111

```
I think you're putting way too much thought into batteries.  Just run some 30q for your first build and go from there.
```

---
## \#187 Posted by: aethyr Posted at: 2018-05-10T07:13:07.212Z Reads: 110

```
Or just buy the vapcell gold on alibaba and test it out. I mean no eskate or ebike battery builder I know of has ever used them, so what could go wrong. One random guy thought the vapcell gold was in fact a 40T, so it must true. The most perfect battery with the highest current, capacity and cheapest price is out there. Of course, with all that current, a simple pack that just takes 2 hours to make of just single layer 0.15 x 7 mm nickel strips will handle that perfectly fine. 

I mean why in the hell would you want to use a proven battery like the 30Q when you can have the vapcell gold that provides 33% extra capacity at 33% extra volume but at 2x the cost? I mean its not like I can simply add 33% more 30Q cells and get that extra 33% capacity at only 33% extra cost or anything. Sheesh.
```

---
## \#188 Posted by: uigiroux Posted at: 2018-05-10T10:59:34.461Z Reads: 107

```
Lol, I not sure if your being very sarcastic or not.... but I agree with you!  :wink:
```

---
## \#189 Posted by: moon Posted at: 2018-05-10T11:04:47.004Z Reads: 109

```
Theres a factory I have been talking to that will have 30t and 40t cells in stock at the end of the month
```

---
## \#190 Posted by: Sebike Posted at: 2018-05-10T11:11:33.463Z Reads: 110

```
Isn't the volume of the 21700s actually nearly 50% more than the 18650s?
```

---
## \#191 Posted by: b264 Posted at: 2018-05-10T11:20:01.662Z Reads: 115

```
[quote="uigiroux, post:181, topic:43020, full:true"]
But it says it has 30A, that’s much more than the 48G.
[/quote]

It says right on the cell that's only a 10A cell.  The deceptive labeling makes me immediately distrustful and skeptical of this brand as well.

![1280|500x500](upload://fANYQ7amYMmWumBL0ko8O99UGR.jpg)
```

---
## \#192 Posted by: uigiroux Posted at: 2018-05-10T11:27:41.231Z Reads: 114

```
True, that one is no good, but this vapcell looks like a relabeled 40T..

http://www.vapcelltech.com/index.php/Show/index/cid/41/id/54.html
![Screenshot_20180510-062840|263x500](upload://f2g5ooG3sz9WHtKMnhHx0q9UcWi.jpg)
```

---
## \#193 Posted by: uigiroux Posted at: 2018-05-10T11:30:38.081Z Reads: 113

```
They give you prices yet?
```

---
## \#194 Posted by: moon Posted at: 2018-05-10T12:04:07.170Z Reads: 110

```
No not yet
```

---
## \#195 Posted by: uigiroux Posted at: 2018-05-10T12:36:15.149Z Reads: 117

```
In that y review the person says the 40T is the best battery currently for unregulated use, and the 30T is the best for regulated... Granted they were talking about vaps, but does anyone know what that means for Esk8?  I'm inclined to think the 40T is the better cell for Esk8...?
```

---
## \#196 Posted by: uigiroux Posted at: 2018-05-10T13:02:23.101Z Reads: 119

```
Ok how can this be possible...?  They're charging like hundreds for these?!  4000mAh and 40A...?

https://www.google.com/amp/s/m.aliexpress.com/item/32806627774.html
```

---
## \#197 Posted by: bevilacqua Posted at: 2018-05-10T13:25:11.639Z Reads: 129

```
they actually are, 
nkon has some on preorder : 
http://e-dampfen-forum.de/showthread.php?tid=2258

mooch vapcell test: 
https://www.e-cigarette-forum.com/threads/bench-test-results-vapcell-gold-4000mah-30a-21700-seems-to-be-samsung-40t-beats-30t-for-reg-mods.859265/
```

---
## \#199 Posted by: uigiroux Posted at: 2018-05-10T13:37:58.926Z Reads: 127

```
Lol, for 48 of them (12s4p) plus shipping it's $666 :wink:
```

---
## \#200 Posted by: aethyr Posted at: 2018-05-10T18:27:42.580Z Reads: 140

```
Oh, you're right its almost a 50% increase. A 18650 has V=5265*pi, a 21700 has V=7717.5*pi. The difference is 2452*pi units, which is almost 50% the volume of an 18650. 

So for merely 2x the space and 2-3x the cost you get only a 33% increase in capacity and current. All you have to do is simply double the number of 30Q cells and you would get a 100% increase in capacity and current at 2x the cost. Or buy 33% more 30Q and get that 33% increase in current/capacity at 1.3x cost. Or add 50% more 30Q cells (to get the same volume of a 21700) and get a 50% increase in capacity and current at only 1.5x cost. Either way, the 30Q wins.

Math, how do you work
```

---
## \#201 Posted by: PXSS Posted at: 2018-05-11T11:03:18.439Z Reads: 137

```
Thats what I said like a year ago...

https://www.electric-skateboard.builders/t/samsung-40t-3900mah-30a-cdr-45a-mva-avail-mid-2018/40847/9?u=pxss
```

---
## \#202 Posted by: silvers Posted at: 2019-03-09T12:26:13.522Z Reads: 88

```
I just got 100 LG M50 '5000' mAh cells. 
I tested them just last night for capacity ... with photos ... The ACTUAL capacity of these cells are 5370 mAh... The highest 18650 is 3400 but I'm willing to bet most people are getting something around 2800 to 3300 at best. The size difference is minimal and the capacity is EXACTLY 42.14 % more than a 3000 mAh 18650 for example. Theres no question its a better alternative in every way, but I can't blame anyone for doubting, I only now know and was surprised at the extra 370 mAh over 5000 the M50 gave me. Again I have photos of my battery tester with the battery, and the LCD display clearly showing 5370. The amps were tested around 19, but honestly most applications are under that or CAN be under that. And yes I bought from Efest on Alibaba.
```

---
## \#203 Posted by: Vanarian Posted at: 2019-03-09T13:21:03.590Z Reads: 85

```
How much did they retail for ?
```

---
## \#204 Posted by: Andy87 Posted at: 2019-03-09T14:02:50.550Z Reads: 84

```
@silvers did you test the cells for 19A?
I couldn’t find any discharge test which show that they able to do that much. Max was 7.5A constant. Would be great if they really could do that much 👌
```

---
## \#205 Posted by: moon Posted at: 2019-03-09T14:34:03.508Z Reads: 82

```
Always best to trust what mooch says, unfortunately I cant find his article about the LG m50
```

---
## \#206 Posted by: Holyman92 Posted at: 2019-03-09T14:58:57.465Z Reads: 83

```
I was just looking at these cells the other day on imrbatteries
```

---
## \#207 Posted by: thisguyhere Posted at: 2019-03-09T17:46:22.376Z Reads: 76

```
LG M50 is 7.2a max discharge current and sags to 3.8v from a full charge... Dont think they're suitable for high current settings, probably more for long distance cruisers. 

Imr has it for $7.5, not a bad price. 

https://electricbike.com/forum/forum/batteries/18650/68165-top-21700-cells-lg-m50-5000mah-vs-samsung-48g-4800mah
```

---
## \#208 Posted by: iKNOWaFATman Posted at: 2019-03-09T17:52:57.537Z Reads: 74

```
If i remember my math A 21700 needs to be OVER 4ah to be equivelent to a 30q from the vol perspective. If we could get a 20-30 amp continuous 4200-4500+ 21700 AROUND $5 A PIECE  id be all over it.
```

---
## \#209 Posted by: TowerCrisis Posted at: 2019-03-10T00:18:40.342Z Reads: 71

```
Wow, the math here seems REALLY off.

First of all, cylindrical volume means nothing for our use. Our packs are rectangular and you guys don't stick stuff in the empty spots between cells.

So EFFECTIVE volume for the 21700 cell is 30870mm^2

And the effective volume for an 18650 is 21060.

So the 21700 cell is effectively **1.46x** the size of an 18650. That is NOT 2x as large as I've read multiple times in this thread.

To add another layer onto this, for the most part we are NOT limited to horizontal space in our packs. Our biggest limitation is on the length of the pack and the height.

So if we're only looking at the cross sectional area of what MOST people care about the difference is 324 vs 441, so the 21700 cell would be **1.36x** as large **in the dimensions that we care about**.

Of course, these numbers only apply to a flat pack, they will change if you're using a trapezoidal format like @longhairedboy does in his packs.

The weight is an entirely different subject I'm not going to delve into (yet)
```

---
## \#210 Posted by: banjaxxed Posted at: 2019-03-10T01:28:42.196Z Reads: 71

```
I don’t understand why the Sanyo NCR20700B 4250mAh is not considered the 30Q of 2070s

...it does a solid 16A constant and 20A in burst with great capacity at a price which is much more competitive than the hot hot 40T
```

---
## \#211 Posted by: TowerCrisis Posted at: 2019-03-10T01:52:57.161Z Reads: 71

```
In general the format of a 21700 cell is superior to the 18650.
A few reasons Include:

The center tube used for rolling does not change size, so additional volume does not get lost with a larger format.

The outer casing does not need to increase in thickness, so there is a better inner volume to outer surface area ratio.

So I'm not at all surprised by that spec @banjaxxed
```

---
## \#212 Posted by: banjaxxed Posted at: 2019-03-10T01:59:58.344Z Reads: 71

```
Currently 1.3x as expensive and 1.42x the capacity as the 30Q on Nkon 

That is compelling
```

---
## \#214 Posted by: Pedrodemio Posted at: 2019-03-10T20:44:02.411Z Reads: 56

```
3750mAh in the GA? Isn’t that 7 supposed to be a 3? 3350mAh?
```

---
## \#216 Posted by: Pedrodemio Posted at: 2019-03-12T01:37:08.191Z Reads: 54

```
Discharged to 2v or something crazy like that? not doubting, but never seen anything close anywhere
```

---
## \#218 Posted by: TowerCrisis Posted at: 2019-03-12T03:42:16.572Z Reads: 48

```
For the love of god stop calculating volume treating the cells as cylindrical, the VAST majority of packs have them in a prismatic grid which means they can be treated as rectangular prisms. That affects the volume calculations significantly.
```

---
## \#219 Posted by: PXSS Posted at: 2019-03-12T05:32:17.888Z Reads: 48

```
I assume you calculate the area of a circle as a square. Do you also calculate the area of a triangle as a square? 

Just because to you, something seems more useful, it doesn't make it right. 

Sink a cylinder of 18650 dimensions in water and tell me how much volume they displace, will my numbers or yours be more accurate?

Cells are cylindrical. end of story. if you cant deal with that then go use lipos. They are prismatic...

As far as configurations go, you can offset stack cells which leads to much better packing desity than a regular square array. Do you then calculate volume of a cell as a triangular prism?

Giving accurate data is best so people can then use said data to their specific needs without skewing their particular results. Giving out inaccurate data leads to misinformation by people who may not know as much.

Regardless of whether you calculate the volume as a cylinder or a square prism, the ratio of volumes between an 18650 and 21700 (which is the topic at hand) remains the same.
```

---
## \#220 Posted by: TowerCrisis Posted at: 2019-03-12T06:52:51.899Z Reads: 47

```
[quote="PXSS, post:219, topic:43020"]
As far as configurations go, you can offset stack cells which leads to much better packing desity than a regular square array. Do you then calculate volume of a cell as a triangular prism?
[/quote]

Actually, packaging is still the same here. trapezoidal packaging is minimally more dense than a straight row. However it does not affect the ratio of 18650 to 21700.

[quote="PXSS, post:219, topic:43020"]
Just because to you, something seems more useful, it doesn’t make it right.
[/quote]
I'm currently working on a quick write up about the 30Q and 40T, so hopefully I can explain myself further there. For now I'm dropping this from this thread to not crowd things up.
```

---
## \#221 Posted by: TowerCrisis Posted at: 2019-03-13T23:22:51.047Z Reads: 40

```
For those of you curious, I've done a little research through the data sheets (including many other common cells)

https://www.electric-skateboard.builders/t/my-findings-on-18650s-and-21700s-and-a-little-awards-show-at-the-end/87095
```

---
## \#222 Posted by: mishrasubhransu Posted at: 2019-03-13T23:29:43.171Z Reads: 38

```
@TowerCrisis is right though. Given a definite amount of space how many WH can you fit should be the metric on which we choose our batteries(if cost is not the deciding factor). It's the volume of the biggest pack that can go in matters,  not the volume of individual cells* #ofcells.
```

---
## \#223 Posted by: TowerCrisis Posted at: 2019-03-13T23:31:21.213Z Reads: 36

```
It's important when comparing packs to cells, but as long as you're speaking the same "language" unit wise, you can compare different kinds of cells using any method of measurement.
```

---
