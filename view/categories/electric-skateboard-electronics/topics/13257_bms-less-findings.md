# BMS-less findings

### Replies: 11 Views: 1826

## \#1 Posted by: Jinra Posted at: 2016-11-18T03:35:43.483Z Reads: 361

```
@Namasaki @evoheyax @Hummie   

So I've been using my board for the last 2 weeks without a bms since the one i bought was defective. I figured I'd just not charge or discharge it all the way (though i accidentally charged it all the way once) and it should be safe for the cells. After about 7ish recharge cycles i decided to test the voltage of the cells. You'd think there would be some shift right? Well...

There wasn't! Every cell was consistent and measured 3.65v. I'm not sure how long or under what conditions cells start to stray, but it looks like for the short term, you can run without a bms in normal conditions.

Board specs:
dual 63mm
10s4p
Samsung 25r cells
```

---
## \#2 Posted by: Hummie Posted at: 2016-11-18T03:57:31.954Z Reads: 353

```
With the lv cutoffs on the vesc a bms seems unnecessary if you like to monitor your cells anyway.  The little 10$ balance/dischargers I just stick on the packs and bulk charge and done.  I can charge and discharge at any wattage possible. 

I don't have much straying and with the Lipo keeping between 4.1 and 3.6 I have room so I don't worry.
```

---
## \#3 Posted by: Namasaki Posted at: 2016-11-18T04:14:03.723Z Reads: 341

```
I was riding the other day on a road that had some really rough section. 
After about 13 mile and my volt meter still showing around 36volts, my BMS suddenly shut down. 
When I got home i checked every cell individually and all cells where above 3.3v but when I tried to charge the pack, it would not take a charge. 
First I thought my BMS got blown. So I swapped it out for a new one but still no go. 
After further inspection I found that the main pos power wire from the last pack in series had an intermittent bad connection and even sparked a couple times when I turned the power switch on. 
Glad I had the BMS shut things down or I may have had my board catching fire!
```

---
## \#4 Posted by: Randyc1 Posted at: 2016-11-18T04:21:30.124Z Reads: 317

```
I just checked my battery pack 3 days ago after riding all summer without a BMS , all 10S balanced to within 2/100 of a volt !
```

---
## \#5 Posted by: Hummie Posted at: 2016-11-18T04:53:27.445Z Reads: 307

```
Trying to imagine a situation where a bms could save the day IF you're monitoring when charging and have the vesc's lv cut-offs...I can't think of any.   In  namasaki's situation where the series connection become loose...I think to have uneven discharging of cells the resistance would have to increase drastically for a stretch of the series chain and therefore be very thin and burn up.
```

---
## \#6 Posted by: TheImmortalJew Posted at: 2016-11-18T05:47:48.069Z Reads: 300

```
I've put 50 charge cycles on a 12s3p pack I made out of LG HG2's and they are doing great so far without a BMS. I balance charge with an Imax B6 and every time I plug in to charge I take note of the voltages of each cell. They have never varied more than .1 of a volt and I think that is just the charger internally rounding to two decimals. I keep an excel spreadsheet and record the starting voltage, charge time and rate, and mah delivered for each 6s battery. Have never gone outside of the 3.6-4.1V range yet and don't plan on it. 


I like jehugarcia on Youtube's opinion on the matter of BMS's and balancing. He is running BMS-less on his electric VW with cells of different chemistries and has been doing fine for a few years now.
```

---
## \#7 Posted by: Jinra Posted at: 2016-11-18T05:55:42.944Z Reads: 277

```
You wouldn't need a BMS anyway since you're balance charging on the imax b6.
```

---
## \#8 Posted by: Hummie Posted at: 2016-11-18T14:35:23.095Z Reads: 248

```
Do lg hg2 operate between 4.2 and 3.6 or maybe you could go much lower being Li-ion
```

---
## \#9 Posted by: Jinra Posted at: 2016-11-18T15:20:18.504Z Reads: 240

```
I think most of not all liion 18650 have an operational voltage of 2.5-4.2v though obviously you never want to go that low.
```

---
## \#10 Posted by: lowGuido Posted at: 2016-11-19T11:48:47.540Z Reads: 225

```
I have an ebike that I have been running BMS-less for over 5 years now.. guess what the cell balance is like?
```

---
## \#11 Posted by: Alextech Posted at: 2016-11-19T15:49:21.428Z Reads: 202

```
Pretty Even :stuck_out_tongue:
```

---
