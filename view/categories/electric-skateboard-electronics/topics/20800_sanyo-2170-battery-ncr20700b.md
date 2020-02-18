# Sanyo 2170 battery NCR20700B

### Replies: 41 Views: 9617

## \#1 Posted by: thisguyhere Posted at: 2017-04-11T16:31:02.818Z Reads: 419

```
has anyone started a build using the Sanyo NCR20700B 2170 cells yet?

they're still kind of expensive but would be nice to reduce parallel packs to make a more compact battery.

their continuous discharge rate is rated at 10a, is that too low for a eboard?

this is a pretty good writeup on the cells: http://budgetlightforum.com/node/51822
```

---
## \#2 Posted by: SimosMCmuffin Posted at: 2017-04-11T22:01:19.546Z Reads: 408

```
They are rated for 15 A continuous discharge. https://akkuplus.de/mediafiles/Datenblatt/Panasonic/Panasonic_NCR20700B.pdf

They do have an equal energy density as with high capacity 18650s.

They are currently cost / kWh wise worse than the 18650s available at the moment.

To put it simply.  Not too sensible choice before the prices drop.


----------


A comparison for a bulk purchase of 100 pieces of (prices taken from NKON, without VAT): 
Panasonic/Sanyo NCR20700B 4250 mAh 15 A 
Samsung INR18650-25R 2500 mAh 20 A
Samsung INR18650-30Q 3000 mAh 15 A
LG INR18650-MJ1 3500 mAh 10 A

**Sanyo:** 492 €, 696 Wh/l, 322 €/kWh
**Samsung 25R:** **244 €**, 540 Wh/l, 271 €/kWh
**Samsung 30Q:** 298 €, 641 Wh/l, 275 €/kWh
**LG MJ1:** 306 €, **756 Wh/l**, **242 €/kWh**

At the moment there are cheaper options available in the 18650 selection. Once the price for the Panasonic/Sanyo/Tesla 20700 comes down, then it'll make sense.
```

---
## \#3 Posted by: Okami Posted at: 2017-04-11T22:04:00.099Z Reads: 376

```
@SimosMCmuffin  Good comparison of cells. IT does point out that MJ1 is currently the best cell cost wise, eur/per kwh (when ordering from nkon)
```

---
## \#4 Posted by: SimosMCmuffin Posted at: 2017-04-11T22:05:34.784Z Reads: 368

```
It's one of the best "bang for your buck" cells available at the moment, but is restricted by it's output current, so you might need to add more parallel cells to get your rated/wanted current and that'll end up in a bigger battery pack overall, but you'll also go further.

It all really can be boiled to:

1. How many cells do you put in your pack, so it fits on your board. (overall pack size)
2. How many cells do you want in series. (voltage)
3. How many amps does the battery need to provide. (current)

And then you go around looking for the cells, which can provide the current you need with the X parallel cells you decide to build the pack with and then by price point select the cell capacity, for how much you want to pay. Of course makes sense to go to the low cost / kWh options so you'll get most range for your money.
```

---
## \#5 Posted by: captainjez Posted at: 2017-04-11T22:17:04.855Z Reads: 328

```
It's actually not 2170 they are 2070. 2170 is the new cell design by Tesla and Panasonic. :slight_smile:
```

---
## \#6 Posted by: Okami Posted at: 2017-04-11T22:24:40.887Z Reads: 325

```
yeh, that needs to be considered that MJ1 is also 10A cell.

I think the best option to ''value'' cells power output is in watts.

If you take 3.6v nominal times 10A for example, you get 36w..

Now, if you normally wish to draw 500w and at peaks 1500w, you need at least:

**42 cells** 

In 6S 7P config, this would give massive range.. and max power output of about: 

70A / 1512 W.

--
10S 4P would also be possible and would still ''yield'' about 1400W of power, with ''comfortable'' output of still 400w I believe.

(even though some would consider this a bit low maybe).. but range should still be quite good.

<img src="/uploads/db1493/original/3X/7/2/727a13073f22f13d469daa101907e8a2b3f80d74.png" width="690" height="205">

Considering 400w ''normal usage'', with 10S system, that would translate to about 400w/36 = 11.11 A total per pack, with 2.77A per cell.

This gives us about **11wh per cell** (when really drained), so maybe ''usable'' capacity could be closer to **10.5 wh per cell.**

with 40cells:

440wh (close to max)
420wh (with some ''reserve'')

Would probably give ''longboard'' about ~42km of range (~26miles)

--

For mountainboard (15-20wh per km)
This might give 21-28km of range, but then again power output might be a bit on the low side, especially if 2 motors need to be fed from the same battery.

--

So yeh, for crazy longboard range these cells might fit but otherwise for high power setups they might be a bit on low side.
```

---
## \#7 Posted by: Pantologist Posted at: 2017-04-11T23:27:27.511Z Reads: 270

```
I'm waiting for Samsung and LG to release their 2170/2070 cells. Hopefully the price drops then. These cells aren't really anything special tbh.
```

---
## \#8 Posted by: Pedrodemio Posted at: 2017-04-12T03:38:34.365Z Reads: 263

```
Samsung release one of them, capacity wise is "bad", but look at the IR and discharge capability 

For a 10S1P or 12S1P and a range of 12Km it would be awesome and light, but with no power compromises 

http://lygte-info.dk/review/batteries2012/Samsung%20INR21700-30T%203000mAh%20(Gray)%20UK.html
```

---
## \#9 Posted by: Pantologist Posted at: 2017-04-12T03:42:12.583Z Reads: 259

```
Yea capacity wise that sucks. Hopefully they will have another version.
```

---
## \#10 Posted by: thisguyhere Posted at: 2017-04-12T04:10:57.330Z Reads: 264

```
Geez 3000mah, what's the point of the larger cubic area?
```

---
## \#11 Posted by: Pedrodemio Posted at: 2017-04-12T04:19:20.197Z Reads: 253

```
Look at the discharge current no other cell (maybe A123 26650) can do that and not suffer massive sag

All cells are a tradeoff between energy, discharge capacity and cycle life, in this case the pushed a lot towards discharge capacity, my guess is the market is tools

@Pantologist I've read on candlelight forums that they have a 5300mah version almost ready to market, but it sounds to good to be true and has no sources
```

---
## \#12 Posted by: Pantologist Posted at: 2017-04-12T04:31:48.091Z Reads: 247

```
I doubt that. I don't think that is even possible with the same chemistries.. it will have really bad discharge output too.
```

---
## \#13 Posted by: SimosMCmuffin Posted at: 2017-04-12T06:25:20.809Z Reads: 238

```
@Pedrodemio @Pantologist
if the 21700 cell has a capacity of ~5200 mAh, it has the same energy density as the LG MJ1 3500 mAh cell, so capacity wise it's absolutely doable, but it will most likely be pretty low discharge rate as Panto mentioned, but Tesla has so many cells in their cars overall I don't think it'll be a problem for them to still get crazy cyrrents.
```

---
## \#14 Posted by: Pedrodemio Posted at: 2017-04-12T12:33:57.313Z Reads: 244

```
Exactly, by even so they are still limited by battery discharge, if I'm not mistaken they peak around 20A per cell, if using a different chemistry they could break the 1MW barrier, but at cost of lower autonomy
```

---
## \#15 Posted by: onlytesla Posted at: 2017-07-26T15:04:52.882Z Reads: 238

```
Beside the NCR18650GA cells, I started to design battery packs with [Panasonic Sanyo NCR20700B](http://www.uavfpvbattery.com). Are more powerful than shows specs from data sheets!
<img src="/uploads/db1493/original/3X/7/8/78f9d64c11e75e0dc7b2d55d4ba69a80824a7c87.jpg" width="500" height="281">
<img src="/uploads/db1493/original/3X/9/9/996dfd97fb7f9afd2973dcfb46e263dea53be408.jpg" width="500" height="281"><img src="/uploads/db1493/original/3X/4/e/4e8e039aa792bf86e8b7741ad25742434e1a3d47.jpg" width="500" height="281">
```

---
## \#16 Posted by: barajabali Posted at: 2017-07-26T15:10:26.870Z Reads: 236

```
I used these cells a few months ago on a 12s2p config. Work beautifully
```

---
## \#17 Posted by: fuelre Posted at: 2017-07-27T12:19:16.508Z Reads: 231

```
I use them in a 10S3P config now for around 4 Months

The big advantage over the 18650s is the spaceconsumtion: a 12Ah needs with this cell 3P compared to 4P with 18650s

if you dont need more than 40A batterycurrent then these cells are the best in my mind
```

---
## \#18 Posted by: chaka Posted at: 2017-07-27T15:28:18.661Z Reads: 230

```
Using these in a 10s6p configuration right now. Very little voltage sag.
```

---
## \#19 Posted by: fuelre Posted at: 2017-07-28T07:16:49.871Z Reads: 229

```
@chaka: like your style - just double everything

whats you range with 6P? probably around 70km/45miles?
```

---
## \#20 Posted by: chaka Posted at: 2017-07-28T16:27:44.593Z Reads: 240

```
I have yet to do a full drain on the pack. I'm sure it has plenty of range. 45 miles should be reachable but I would be happy if it gave me 30 miles of aggressive riding.
```

---
## \#21 Posted by: fuelre Posted at: 2017-07-30T16:20:48.739Z Reads: 227

```
I get on 3P and aggressive riding close to 30km, after that the Vesc pulls the power down (conservative at start / end cutoff)
But I have only a 6355 with 60A on that build that max. out at about 40kmh
```

---
## \#23 Posted by: Vanarian Posted at: 2017-08-06T09:46:46.854Z Reads: 224

```
Had anybody had his hands on the Samsung 21700-30T instead? 

I fail to find them.
```

---
## \#24 Posted by: onlytesla Posted at: 2017-08-06T13:22:05.656Z Reads: 218

```
2170 or 2070 are pretty the same (2070 have dimensions 20,5 x 70,3 mm)
```

---
## \#25 Posted by: captainjez Posted at: 2017-08-07T01:44:05.925Z Reads: 210

```
Dimension wise they're similar. But chemistry wise they're completely different cells.
```

---
## \#26 Posted by: chaka Posted at: 2017-08-07T01:53:51.737Z Reads: 205

```
No they are not, they are both li-ion. The biggest difference is the 21700 is made in Nevada USA.
```

---
## \#27 Posted by: captainjez Posted at: 2017-08-07T01:55:32.337Z Reads: 199

```
Yes and lithium Ion has slight variances in chemistry. The 20700 and other Panasonic cells are LiMnCo2. The new Tesla Panasonic cells are a modified chemistry to this.
```

---
## \#28 Posted by: chaka Posted at: 2017-08-07T01:56:22.310Z Reads: 197

```
Pure speculation, do you have the 21700's in hand?
```

---
## \#29 Posted by: captainjez Posted at: 2017-08-07T01:56:41.012Z Reads: 194

```
We have a few yes.
```

---
## \#30 Posted by: chaka Posted at: 2017-08-07T01:57:42.557Z Reads: 191

```
Show us the pics! This is huge! I had no idea they were available already!
```

---
## \#31 Posted by: captainjez Posted at: 2017-08-07T01:58:57.153Z Reads: 189

```
They're not readily available. We buy all our cells from Panasonic direct. We were able to get a few sample cells sent to us. It's going to be at least a year or so before they will readily available.
```

---
## \#32 Posted by: chaka Posted at: 2017-08-07T02:02:36.446Z Reads: 192

```
I have only been able to get my hands on the sanyo and samsung 20700/21700 cells. What color are the Panasonic cells if you don't mind me asking? I have yet to see any press photos. Do you have the specs on them?
```

---
## \#33 Posted by: captainjez Posted at: 2017-08-07T02:13:22.411Z Reads: 191

```
They're not wrapped the few we have. Just bare cells. We're not allowed to say much due to NDAs with Panasonic. But they're amazing. :slight_smile:
```

---
## \#34 Posted by: chaka Posted at: 2017-08-07T02:57:38.212Z Reads: 193

```
Since they are bare cells it wouldn't hurt to show a few pics, what I am really interested in is the size. The Sanyo 20700's are just a hair under 21mm and I am hoping the cells coming out of the Giga factory will be the same!
```

---
## \#35 Posted by: onlytesla Posted at: 2017-08-07T11:53:13.788Z Reads: 185

```
Not too much, maybe diff cathode chemistry, more C6 or Co27
```

---
## \#36 Posted by: Titoxd10001 Posted at: 2017-08-09T18:18:25.795Z Reads: 181

```
Aren't 18650s alot better in terms to weight/power. Based on weight 20700 would need to be 4000mah and 30a to be worth it. They do seem to fit in a smaller space though.
```

---
## \#37 Posted by: chaka Posted at: 2017-08-09T18:24:39.307Z Reads: 186

```
The 20700B cells perform better at 10 amps than any other cell I have tested. When you consider I am using these in a 10s6p and 12s5p format you will see that is 60 amps at 36v and 50 amps at 44.4v with bursts up to 90 amps or more being possible. 

Short story is, these are the choice for a big pack, 60 cells.
```

---
## \#38 Posted by: Titoxd10001 Posted at: 2017-08-09T18:49:21.602Z Reads: 189

```
So the the 20700b has better amp output then 30q? If you're set on cell count makes sense but what I mean is a 12s4p 30q (46g) will weigh less/same than a 12s3p 20700b (63g) pack. 20700b has mAh advantage but 30q has more amp output. I am considering a 60 cell pack but the weight seems a bit much.
```

---
## \#39 Posted by: gmurad Posted at: 2018-07-22T17:12:41.950Z Reads: 101

```
Hi, can you recommend cut-off start and end voltages for 20700b cells?
```

---
## \#40 Posted by: Sebike Posted at: 2018-07-22T17:22:26.225Z Reads: 102

```
your wait will be long. chaka is no longer on the forum.
```

---
## \#41 Posted by: bevilacqua Posted at: 2018-07-22T17:27:58.914Z Reads: 103

```
like on 18650s it depends of the voltage sag at lower voltages and also the P configuration. 

on direct comparison (103p to 103p for example) only because the 20700 have 4ah compared to 3ah I would set the cutoffs of the 20700 0,1 lower. But not much more.
```

---
## \#42 Posted by: thisguyhere Posted at: 2018-07-22T19:02:06.138Z Reads: 90

```
on the conservative side 3.3v soft start, 3v cutoff.

-0.1v of that may still be okay, but no lower.

for my builds at least.
```

---
