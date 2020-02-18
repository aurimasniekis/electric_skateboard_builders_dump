# 12S LiFePO4 charger

### Replies: 19 Views: 2582

## \#1 Posted by: Pantologist Posted at: 2016-06-29T21:03:16.542Z Reads: 208

```
I'm having trouble finding a 12S a123 battery pack charger. I'm looking for brick style charger and I've only found wholesale versions. 

https://m.alibaba.com/product/60448153391/Li-ion-battery-charger-43-2V.html

Fully charged voltage would be 43.2V since the cells are fully charged at 3.6v. Any suggestions?
```

---
## \#2 Posted by: Jinra Posted at: 2016-06-29T21:05:53.609Z Reads: 208

```
http://www.ebay.com/itm/like/321751879896?lpid=82&chn=ps&ul_noapp=true

or maybe shipping is cheaper for you here

http://www.batterysupports.com/36v-438v-5a-lifepo4-battery-charger-12s-12x-32v-life-charger-p-161.html
```

---
## \#3 Posted by: Pantologist Posted at: 2016-06-29T21:26:19.867Z Reads: 195

```
Thanks. It seems to be decent but it looks huge! I would have thought that a 2A ~40v charger could have been smaller.
```

---
## \#5 Posted by: Ulfberht Posted at: 2016-06-29T22:43:18.176Z Reads: 176

```
NOt the cheapest, but the best I have found. THe customer service was super friendly and easy to contact someone that knows a thing or two. Check em' :thumbsup:
http://www.electricrider.com/lithium-and-sla-battery-chargers-s/1817.htm

Edit: Here's the direct link to a 12s 4A charger: http://www.electricrider.com/VeriBest-48V-4A-Lithium-Battery-Charger-p/li-48040.htm
```

---
## \#6 Posted by: lox897 Posted at: 2016-06-30T01:38:04.253Z Reads: 164

```
That one charges to 43.8v. That would overcharge to 3.65v per cell.
```

---
## \#7 Posted by: Jinra Posted at: 2016-06-30T02:14:01.098Z Reads: 150

```
woops! wrong search
```

---
## \#8 Posted by: Pantologist Posted at: 2016-06-30T02:36:44.323Z Reads: 149

```
Yeah I noticed that too. The cells should be fine with that since the BMS will be balance charging after the pack is full. Wouldn't it be fine?

I decided to search up what Boosted uses as their charger and it seems that they use something like this...

http://www.ebay.com/itm/Mean-Well-OWA-90U-42-Plug-In-Adapter-Single-OUT-42V-2-15A-90-3W-US-Authorized-/112028718369?hash=item1a156e9521:g:hxkAAOSwT5tWG~A7

Definitely that brand somewhere within the 2-5A range for the standard charger. It seems that they are only charging to 42V.
```

---
## \#9 Posted by: Trans-amers Posted at: 2017-02-09T13:10:06.402Z Reads: 91

```
How is your charger doing? Did they charge up to 43.8V?
```

---
## \#10 Posted by: Pantologist Posted at: 2017-02-09T14:34:21.602Z Reads: 90

```
I ended up buying a Boosted charger since it was already adjusted for 12S LiFePO4. The charger outputted 43.6v and came with a great DC plug.
```

---
## \#11 Posted by: Trans-amers Posted at: 2017-02-09T16:29:52.965Z Reads: 83

```
Are you living in the us?
I am based in the uk so i could hardly find a boosted charger here.
They dont even have a uk website
is your charger the first gen charger?
```

---
## \#12 Posted by: Pantologist Posted at: 2017-02-09T16:59:48.409Z Reads: 77

```
Yes the first gen charger. The second gen out puts like 54V. Decent for 12S builds but if you can't get it for cheap there is really no point. 

You can buy standard Mean Well power supplies within the range of your voltage and some are adjustable with a pot inside.
```

---
## \#13 Posted by: Trans-amers Posted at: 2017-02-18T01:29:19.800Z Reads: 71

```
Does this looks good to you?
http://www.ebay.com/itm/Two-wheel-self-balanced-vehicle-12S-43-2V-44-4V-Li-ion-Battery-Charger-50-4V-2A-/222180188366
```

---
## \#14 Posted by: Pantologist Posted at: 2017-02-18T01:45:55.661Z Reads: 68

```
Nope. That is for 12S Lithium ION not Lithium Iron phosphate. Unless you can adjust the power output to 43.2V I would not get it. Besides, it looks like a super generic Chinese one. Try to get a Boosted one second hand or a Mean well power supply. Same of them can be adjusted.
```

---
## \#15 Posted by: Trans-amers Posted at: 2017-02-18T02:25:35.867Z Reads: 63

```
I suppose lifepo4 batteries are called li-ion for short?
```

---
## \#16 Posted by: Eboostin Posted at: 2017-02-18T02:33:11.407Z Reads: 63

```
Are you using a BMS that is cutting off at 43.2 then?
```

---
## \#17 Posted by: Pantologist Posted at: 2017-02-18T02:40:51.605Z Reads: 63

```
Yeah I used a BMS to cut off the voltage. @Trans-amers They aren't. They are LiFePO4 for short.
```

---
## \#18 Posted by: lock Posted at: 2017-07-05T10:36:43.161Z Reads: 51

```
Picked up a MEAN WELL for my 12s a123 pack tonight. ELG-150-48**A**, the A models come with potentiometers on the back to adjust voltage and current over a limited range. 43.2v is the minimum voltage this one does, any lower and it seems to fluctuate quite a bit. Goes up to 53v, so I should be able to use it for a 12s lipo setup (maybe 13s lifepo4😬) in future.

<img src="/uploads/db1493/original/3X/1/f/1fb146e6869e299b418ba878f9e2a50fd69fbc32.JPG" width="375" height="500">

Couldn't quite nail 43.2v, but figure the batteries should be ok being overcharged by 0.004v.
```

---
## \#19 Posted by: Pantologist Posted at: 2017-07-05T11:22:35.578Z Reads: 46

```
Depending on which BMS you use, it should prevent over charging. 

Boosted's outputs 43.6V I believe. The BMS takes care of the rest.
```

---
## \#20 Posted by: lock Posted at: 2017-07-06T01:55:42.643Z Reads: 45

```
Yeah, looking for a BMS that will stop it right at 3.6v, and it's really only the 'smart' BMSs that I think will be able to pull that off. Most of the factory set models seem to do 3.65v for LiFePO4 chemistry. Given it's a power source (has no voltage cutoff) I'll be relying on the BMS to stop charging the pack even if it is at near zero amps.

I'll be putting a wattmeter between this and the BMS/battery, and will be watching with interest what actually happens with the constant current/voltage thing.
```

---
