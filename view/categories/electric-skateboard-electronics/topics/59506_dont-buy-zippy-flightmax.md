# Don&rsquo;t Buy Zippy Flightmax

### Replies: 20 Views: 836

## \#1 Posted by: kuphjr Posted at: 2018-06-20T18:11:41.949Z Reads: 265

```
I'm sure I'm not the first to have this experience, but just a heads up for any builders out there; Zippy Flightmax batteries suck.  I have wasted damn near $200 so far this summer buying replacement 8000mAh 3s LiPo batteries.  It seems as soon as I get the next battery installed, a week later another battery has a dead cell.

If you are doing a budget build, you will not save money by purchasing Li-Po batteries.  You will end up spending twice as much buying replacements for the crap quality batteries.  Get yourself a quality Li-ion pack. I promise you it is worth it in time, money and headache.  I have a spot welder now and I can build you a pack or one of many other people on the forum can as well.
```

---
## \#2 Posted by: abenny Posted at: 2018-06-20T18:16:54.445Z Reads: 257

```
i have 2 4s flightmax batteries i run in series for over a year now no problems. maybe you got from a bad batch or something.
```

---
## \#3 Posted by: kuphjr Posted at: 2018-06-20T18:18:14.150Z Reads: 250

```
I have bought batteries in the past that have lasted 4-5 months, but for the past 6 months I have not received a battery from them that lasted more than 2 months.
```

---
## \#4 Posted by: b264 Posted at: 2018-06-20T18:18:27.541Z Reads: 238

```
If you mix old and new ones and don't keep them balanced correctly then you might be destroying them.  Are you using a BMS?  How low are you running them?
```

---
## \#5 Posted by: mmaner Posted at: 2018-06-20T18:25:42.302Z Reads: 221

```
There are literally thousands of Zippy FlighMax lipos in use in esk8s and 99% of people don't have an issue.  Im not dogging on you, but its likely something you are doing to the batteries not the batteries themselves.
```

---
## \#6 Posted by: wafflejock Posted at: 2018-06-20T18:28:25.021Z Reads: 211

```
What're you using for cut offs?  Do the cells end up far off from each other after discharge/riding?  Personally using some turnigy 5Ah 5S (20-30C, nothing special) but I have conservative cut offs since there can be appreciable voltage dip under load (also I just avoid punching it if I know I don't have a lot left in the batteries).
```

---
## \#7 Posted by: kuphjr Posted at: 2018-06-20T18:54:27.662Z Reads: 193

```
I'm not sure what I could be doing wrong.  I have a BMS that seems to be balancing just fine.  I am pretty sure it is just the last batch of batteries has been bad.  I am pretty aggressive with the acceleration, but I'm not sure what else I could be doing that kills batteries this fast.
```

---
## \#8 Posted by: Benjamin899 Posted at: 2018-06-20T18:57:39.401Z Reads: 184

```
i shorted my zippys and they are still in good condition after a year. What are your specs?
```

---
## \#9 Posted by: kuphjr Posted at: 2018-06-20T18:57:47.126Z Reads: 176

```
My voltage cutoff is 3.4v per cell (12s setup).  After I ride the cells are usually vary by .1-.2 volts, but I always charge with my BMS and that balances the cells just fine.  My battery max setting on my FOCBox is set to 60A on a dual motor setup, but that should still be well within the capability for a 25C 8000mAh battery pack.

If someone has some recommendations to help me from burning through batteries it would be greatly appreciated.
```

---
## \#10 Posted by: kuphjr Posted at: 2018-06-20T18:58:15.651Z Reads: 170

```
4x3s 8000mAh to make a 12s pack.
```

---
## \#11 Posted by: Benjamin899 Posted at: 2018-06-20T18:59:49.737Z Reads: 164

```
i drive mine only down to 3.7v and they are perfectly balanced even without a bms
```

---
## \#12 Posted by: mmaner Posted at: 2018-06-20T19:11:17.771Z Reads: 151

```
[quote="kuphjr, post:9, topic:59506"]
My voltage cutoff is 3.4v
[/quote]

3.4v is pretty low for lipos.  I have run them down to 3.2 but it drastically reduces the lifetime.  The accepted cutoff for lipos is 3.6v.
```

---
## \#13 Posted by: wafflejock Posted at: 2018-06-20T19:51:40.121Z Reads: 136

```
On 10S I have mine setup for 37V soft limit and 35V hard cut off I noticed if I go any lower I end up with cells that are much further off from one another after a run (possibly a bit more off than you're saying).  If they are only drained to 3.5V typically don't have much drift but 3.6V is a safe bet since you can have .6V dip from there and not drop below 3.0V.
```

---
## \#14 Posted by: kuphjr Posted at: 2018-06-20T21:20:11.167Z Reads: 120

```
While I have my voltage set that low, I almost never run them lower than 3.8v.  When I was riding today, I started at 4.2v, rode to class and my cells were at 4.1v.  Then, on my way home I saw the voltage suddenly dip.  I knew I had blown a cell.  When I finished pushing home and opened it up, all the cells except the dead cell were within .1-.2v of 4.0v.

I would think the cells wouldn't be so likely to blow unless they are closer to their nominal voltage.
```

---
## \#15 Posted by: mmaner Posted at: 2018-06-20T21:22:44.581Z Reads: 118

```
I assume you've checked the solder joints where they are put together in series?  Also, do you have the cells secured and padded?  Sounds like vibration or resistance may be an issue.
```

---
## \#16 Posted by: kuphjr Posted at: 2018-06-20T21:24:43.818Z Reads: 116

```
I do have the batteries pretty securely mounted, but I can add padding.  They never seem to be loose solder joints that are the problem though.  Every single time I blow a cell, it is obviously puffy.
```

---
## \#17 Posted by: kuphjr Posted at: 2018-06-20T21:31:13.392Z Reads: 113

```
I have a Bestech 15A bms with bypass discharge.
```

---
## \#18 Posted by: b264 Posted at: 2018-06-20T23:37:45.630Z Reads: 104

```
The problem may be your mixing of new and old cells in series.  Your balance charging may not be able to keep up.  Do you leave it on green for a long time?
```

---
## \#19 Posted by: deucesdown Posted at: 2018-06-21T02:09:57.133Z Reads: 96

```
[quote="kuphjr, post:9, topic:59506"]
My voltage cutoff is 3.4v per cell
[/quote]

:sweat:

What's your bat min?

If you stay between 4.2v and 3.8v per cell (checked at each cell) and not shooting a crap-ton of current in regen, and all the mechanicals and electrical connections are sound, you probably got bad packs. HK does a decent job replacing bad packs though -- have you tried?
```

---
## \#20 Posted by: lrdesigns Posted at: 2018-06-21T02:35:44.186Z Reads: 91

```
My tip to get lipo's to last longer, only use them with a individual cell voltage alarm set to 3.6v

While the vesc can measure total pack voltage, its easy for one cell in a pack to drop below 3v **under load** if your batt min is 3.4v per cell ... and you would never know...

Also if you don't need the range charge to 4.1v

https://www.amazon.com/LiPo-Battery-Checker-Monitor-Indicator/dp/B07BQWSXC4/ref=sr_1_14?ie=UTF8&qid=1529548367&sr=8-14&keywords=lipo+battery+alarm

[https://www.aliexpress.com/ version](https://www.aliexpress.com/item/1pcs-BX100-1-8S-Lipo-Battery-Voltage-Tester-Low-Voltage-Buzzer-Alarm-Battery-Voltage-Checker-with/32762110584.html?spm=2114.search0104.3.37.7e637ebd0FPgmt&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10151_10065_10344_5723115_10068_5722815_10342_10343_10340_5722915_10341_5722615_10696_10084_10083_10618_10307_5722715_10059_100031_10103_10624_10623_10622_5722515_10621_10620,searchweb201603_1,ppcSwitch_5&algo_expid=8ad7e134-5366-48bd-8968-1964512719ef-5&algo_pvid=8ad7e134-5366-48bd-8968-1964512719ef&priceBeautifyAB=0)
```

---
