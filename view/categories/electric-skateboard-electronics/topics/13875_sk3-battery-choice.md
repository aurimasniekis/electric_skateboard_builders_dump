# SK3 Battery Choice

### Replies: 22 Views: 2459

## \#1 Posted by: wmj259 Posted at: 2016-11-29T00:17:00.634Z Reads: 209

```
Hello,

Does anyone know if there is a graph of Torque to speed for any turnigy sk3 motor?
Doing a few calculations as for how much current a motor will draw, to find a good C-rating.
```

---
## \#2 Posted by: SteveS Posted at: 2016-11-29T01:46:39.772Z Reads: 198

```
Wouldn't you want to get a C rating that supports the SK3's maximum current rating?
```

---
## \#3 Posted by: wmj259 Posted at: 2016-11-29T01:51:22.835Z Reads: 195

```
So the max current would be 80Amps, I would want a C value times mAh that would max out at 80Amps? 20C times 12000mAh is more than the 80Amps, I think I am missing something.
```

---
## \#4 Posted by: SteveS Posted at: 2016-11-29T01:55:07.088Z Reads: 192

```
Close, 20c x 12ah = 240 a, so plenty of current potential.
```

---
## \#5 Posted by: Jinra Posted at: 2016-11-29T01:56:22.053Z Reads: 190

```
The higher the c rating the better. You want as much buffer room as you can get between max discharge potential and actual continuous discharge to avoid voltage sag.
```

---
## \#6 Posted by: jmasta Posted at: 2016-11-29T02:04:12.396Z Reads: 179

```
[quote="wmj259, post:3, topic:13875, full:true"]
So the max current would be 80Amps, I would want a C value times mAh that would max out at 80Amps? 20C times 12000mAh is more than the 80Amps, I think I am missing something.
[/quote]

Even if your battery can supply 250A maximum, for example, it will only supply as much current as the motor draws (80A max for your motor, if not limited elsewhere in the system... e.g., VESC settings, or BMS current limiting)

[quote="Jinra, post:5, topic:13875, full:true"]
The higher the c rating the better. You want as much buffer room as you can get between max discharge potential and actual continuous discharge to avoid voltage sag.
[/quote]

What he said
```

---
## \#7 Posted by: wmj259 Posted at: 2016-11-29T02:11:46.667Z Reads: 160

```
So in what way is it possible for the battery to blow up the motor? Only if the vesc is setup wrong?
```

---
## \#8 Posted by: jmasta Posted at: 2016-11-29T02:23:01.365Z Reads: 167

```
Even if your VESC setting was incorrectly set at 250A, the motor will still only pull 80A maximum from the battery.  (But really you should limit that to 50A or 60A in your settings to protect the VESC)

Think of it this way... If you have a giant water bottle with a tiny hole at the bottom, does all the water dump out of the hole at once?  Nope, the size of the hole controls the rate at which the water flows out
```

---
## \#9 Posted by: wmj259 Posted at: 2016-11-29T02:56:10.312Z Reads: 162

```
What batteries do you guys recommend? My mind is just blown from confusion of what to pick. Want to get 2 8,000-10,000mAh with a good C rating. I am looking through 700 batteries on HobbyKing
```

---
## \#10 Posted by: i2oadsweepei2 Posted at: 2016-11-30T12:33:50.321Z Reads: 150

```
I've used standard Turnigy, Zippy and Turnigy Nanotech batteries. They are all pretty descent batteries. I use Nanotech 65-130c lipos  for high power needs. You won't need anywhere near that. You are looking for 8-10,000mah capacity. That narrows down your choices. I didn't see any mention of motor kv, but I did notice you were going to use a vesc. I would assume you will be using 6, 8 or 10s for your project. Stick to 25-45c batteries based on your budget.

It would be wise to follow jinra's advice here even if it slightly stretches your budget.

[quote="Jinra, post:5, topic:13875, full:true"]
The higher the c rating the better. You want as much buffer room as you can get between max discharge potential and actual continuous discharge to avoid voltage sag.
[/quote]

Good luck.
```

---
## \#11 Posted by: jmasta Posted at: 2016-11-30T14:38:05.248Z Reads: 143

```
[quote="wmj259, post:9, topic:13875, full:true"]
What batteries do you guys recommend? My mind is just blown from confusion of what to pick. Want to get 2 8,000-10,000mAh with a good C rating. I am looking through 700 batteries on HobbyKing
[/quote]

If you want that kind of capacity, your best bet for LiPo's is the 8000mah Zippy Flightmax line.   You will have to wire multiple batteries in series to get the desired voltage.  The following 2S, 3S, or 4S batteries have the same footprint but increase in thickness accordingly.  Choose the thinnest battery based on how much area you have for mounting.

**2S Batteries:**  12S = 6x 2S, or 10S = 5x 2S 
https://hobbyking.com/en_us/zippy-flightmax-8000mah-2s1p-30c.html

**3S Batteries:**  12S = 4x 3S, or 9S = 3x 3S
https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html

**4S Batteries:**  12S = 3x 4S
https://hobbyking.com/en_us/zippy-flightmax-8000mah-4s1p-30c.html


Alternatively, skip LiPo's all together and go with a lithium ion pack.  This might be a much easier option for you
```

---
## \#12 Posted by: wmj259 Posted at: 2016-12-02T00:35:46.981Z Reads: 121

```
Heavy Duty 5000mAh 7S  60C / 120C (Burst) Lipo Pack 
[Turnigy Heavy Duty 5000mAh 7S 60C Lipo Pack](https://hobbyking.com/en_us/turnigy-heavy-duty-5000mah-7s-60c-lipo-pack.html) for $59.99  
or
ZIPPY Compact 4000mAh 10S 25C / 35C Burst Lipo Pack
[ZIPPY Compact 4000mAh 10S 25C Lipo Pack](https://hobbyking.com/en_us/zippy-compact-4000mah-10s-25c-lipo-pack.html) for $59.99. 

From the advice given I should probably go with 2 of the Heavy Duty ones?
```

---
## \#13 Posted by: jmasta Posted at: 2016-12-02T00:47:08.105Z Reads: 113

```
Each of those batteries you linked are two inches thick (50mm).  It would work, but you are greatly reducing your clearance.  Using multiple 2S batteries in series would mean your battery would be only 0.6" (15mm) thick.   The 3S batteries are just an inch thick, which is still very thin

Not to mention, anything over 6S because more difficult to change. You can get 10S balance chargers but they are usually twice the price of a 6S charger
```

---
## \#14 Posted by: wmj259 Posted at: 2016-12-06T16:52:46.100Z Reads: 105

```
Why do people go with Li-ions when the C rating for a samsung-25r  is only 20A?
```

---
## \#15 Posted by: jmasta Posted at: 2016-12-06T17:18:11.142Z Reads: 101

```
That is 20A per cell, which why you see packs with 3+ cells in parallel.  A 10S1P pack would only have 20A rated discharge, but 10S3P would have 3x20A = 60A.

However you want a battery capable of providing more current than you would actually draw.  The more buffer the better. Pulling 60A on a 60A max battery results in significant voltage sag and reduces the cell's life.  So a 3P battery rated for 60A, should really be thought of as a 30-40A battery.
```

---
## \#16 Posted by: wmj259 Posted at: 2016-12-06T19:51:27.016Z Reads: 95

```
Oh I think I got it confused with the C-rating for lipos.
Alrighty I might actually buy li-ions then since its kinda cheaper and less hassle. But if I am not mistaken, it will be charged through the BMS? I might go through the route of buying laptop batteries and taking them apart. I would guess a 10S 2/3P would be the best route?
```

---
## \#17 Posted by: wmj259 Posted at: 2016-12-24T17:05:42.809Z Reads: 88

```
How do<img src="/uploads/db1493/original/3X/4/b/4bd4122fae5d0770bd840c7dc91144052ca26ca6.png" width="690" height="478"> these batteries look?

3S 11.1V 8000mAh 40C
US $36.18 Free shipping

If I get 3 of these it will top out to 33.3 Volts
Discharge would be 40C * 8 Ah to get 320Amps. 
Would this be a good choice? Only reason I am going for lipo's at the moment is I would have to invest an additional $100+ for a battery welder+~100 for cells.
```

---
## \#18 Posted by: Charster10 Posted at: 2016-12-24T19:47:23.878Z Reads: 80

```
Sounds alright to me! @wmj259
```

---
## \#19 Posted by: wmj259 Posted at: 2016-12-25T00:56:25.208Z Reads: 72

```
In that case I jsut got 3 for $100 bucks.
```

---
## \#20 Posted by: PXSS Posted at: 2016-12-25T02:18:47.625Z Reads: 74

```
33.3V nominal. 37.8V full and 27V empty. 
Be careful that they actually are 8ah batteries, I would do a test run on the charger to verify capacity
```

---
## \#21 Posted by: wmj259 Posted at: 2017-01-14T20:08:01.737Z Reads: 66

```
Should I go with 9S will that 37.8V be good for a 44V sk3?. I am getting more than enough Amps.
```

---
## \#22 Posted by: OskarCastrone Posted at: 2017-01-14T21:07:38.395Z Reads: 59

```
That amount of voltage will be totally fine for your motor
```

---
