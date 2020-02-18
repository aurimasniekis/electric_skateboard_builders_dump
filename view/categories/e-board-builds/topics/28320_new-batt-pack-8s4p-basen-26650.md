# New batt pack- 8s4p Basen 26650

### Replies: 30 Views: 1978

## \#1 Posted by: sprocket12 Posted at: 2017-07-22T22:55:21.381Z Reads: 218

```
Hey all. I'd like feed back on this here battery layout. I've got all the pieces but want a second, third,...nth opinion before I make irreversible changes. 

I'm using Basen 26650 4500mAh batts. I've loosely followed @namasaki earlier build. I'll be using a 'lightweight' BMS for charging only. Discharging will go to The no-longer-called-VESC thingy. 

<img src="/uploads/db1493/original/3X/e/8/e8519c1c4bc4b8675f83541ab175a4ff6a8e3b0e.JPG" width="375" height="500">

And are .15mm x 10mm pure nickel stripping a good choice?  I just ordered my suunko spot welder too. 

Thanks for taking the time to review this. I look forward to your feedback.
```

---
## \#2 Posted by: chsknight Posted at: 2017-07-23T04:19:07.113Z Reads: 192

```
Looks right to me.  Where did you get the sunkko from?
```

---
## \#3 Posted by: sprocket12 Posted at: 2017-07-23T06:09:11.768Z Reads: 178

```
I ordered from eBay.

Hmmm. I mis-spoke. It is an unbranded Chinese welder. I was juggling several listings. Oh well, I'll report back on how it performs too.
```

---
## \#4 Posted by: sprocket12 Posted at: 2017-07-23T18:39:16.180Z Reads: 157

```
Any other thoughts?  Just waiting for welder now. 

I'd like to add that I'm using a 4a charge 10a discharge BMS but only using it to charge.  Does that sound ok?

Hobby king now has these BMS's for $12. I also saw the name BesTech somewhere on the site.
```

---
## \#5 Posted by: Smorto Posted at: 2017-07-24T00:14:12.652Z Reads: 143

```
Thats gonna be a hell of a better pack. Hope you have the board for that battery :wink:.
```

---
## \#6 Posted by: Jinra Posted at: 2017-07-24T00:18:26.256Z Reads: 139

```
I heard from Namasaki that the Basens sag a lot under load, it may be more worth it to use a different cell.
```

---
## \#7 Posted by: Smorto Posted at: 2017-07-24T00:43:40.323Z Reads: 135

```
Assuring 30A continuous from each cell thats still 120A continuous... that should be enough no?
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-24T00:44:21.082Z Reads: 133

```
Enough discharge? Sure, but the amount of sag at higher discharge rates is unacceptable to me.
```

---
## \#9 Posted by: Smorto Posted at: 2017-07-24T00:45:11.586Z Reads: 132

```
No, wouldn't that discharge combat the sag at least a little?
```

---
## \#10 Posted by: Jinra Posted at: 2017-07-24T00:46:20.118Z Reads: 129

```
Not necessarily. Low quality cells, can still sag a lot even with higher discharge rates. For example, 30Q's have lower discharge than 25R's, but end up sagging less in real world performance.
```

---
## \#11 Posted by: Smorto Posted at: 2017-07-24T00:47:48.181Z Reads: 125

```
Are the basens low quality cells? I thought they were good. Either way, I guess we will see how this pack turns out if @sprocket12 decides to build it.
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-24T00:48:58.705Z Reads: 122

```
They're, just random chinese cells. @Namasaki said flat performance was decent, with okay range, but range and sag really suffered during hills or high draw environments.
```

---
## \#13 Posted by: sprocket12 Posted at: 2017-07-24T01:48:06.711Z Reads: 121

```
Well, I've researched these a bit. There was a previous version of this battery that claimed 5000mAh. Fat chance. These have been tested by mooch and still claim second place for 26650's. The first being iJoy at a hefty price difference.  Even so, Liion Warehouse too rates these high. 

My tests show they are on average 4250mAh. I expected this. Also, they claim 40 amps continuous but real world reports state 30. 

All in all, I can't see where these won't perform well. And if I recall correctly, @Namasaki was running a 2p set up. I'm running a 4p. I've over built on purpose. I don't think I'll see the sag BUT hey! I'm doing this for science 😜. If you have real-world experience, I'd love to hear it!  My last pack was an 8s1p Lipo @ 8000mAh. This will have about 17,000mAh.  Should get me around 27 real-world miles!

I've already purchased everything and the 4-packs are nice and glued- no turning back now. 

Please, by all means, share your thoughts. That's how I learn here. This has been a great community to be a part of.
```

---
## \#14 Posted by: Jinra Posted at: 2017-07-24T01:51:02.418Z Reads: 116

```
How heavy will your pack be?
```

---
## \#15 Posted by: Namasaki Posted at: 2017-07-24T05:22:09.718Z Reads: 116

```
I ran the Bases 4500's in a 10s2p pack.
Range was great on flat gound at moderate speed,   28 miles on a charge.
When doing a lot of long hills, the range was cut more than in half by voltage sag.
I believe it's because a 60a battery is just not adequate for hill climbing no mater what cells your using.
I would be very interested in seeing how your 8s/4p pack with these cells would perform.
```

---
## \#16 Posted by: sprocket12 Posted at: 2017-07-25T05:21:16.984Z Reads: 105

```
Sorry @Jinra. I was out of town on an extended weekend. I can't find the shipping info at the moment but each battery is 100g. That is just over 7 lbs for the 32.
```

---
## \#17 Posted by: sprocket12 Posted at: 2017-07-25T05:31:29.040Z Reads: 108

```
Interesting. I was hoping that going with a 4p set up would provide that extra OOMPH to power through. 

Could you enlighten me further on what you mean by the higher amp battery no being a good fit? I thought you had gone back to Lipos for the higher amps in the mAh size for your board.
```

---
## \#18 Posted by: Namasaki Posted at: 2017-07-25T05:39:24.912Z Reads: 111

```
[quote="sprocket12, post:17, topic:28320"]
Could you enlighten me further on what you mean by the higher amp battery no being a good fit?
[/quote]

I don't recall saying that.
I've been preaching for a long time that the higher the battery's discharge rating, the better!

I did not find enough power with Basen cells in a 10s2p pack.
You might find enough in an 8s4p but I couldn't say for sure.
What I will say is that IMO, no 60a battery pack is enough for big people going uphill regardless of the type of cells.
A 120a battery pack like your planning might do the trick.
```

---
## \#19 Posted by: Titoxd10001 Posted at: 2017-07-25T06:12:54.374Z Reads: 98

```
Samsung 30q 3000mah 46g (20a)

2x 30q= 6000mah 92g (40a) 
basen 4500mah 100g (25a)

Amp rating based on Mooch ratings
```

---
## \#20 Posted by: sprocket12 Posted at: 2017-07-25T14:48:01.174Z Reads: 96

```
So, all things being equal...

18,000mAh pack is
48 x Samsung 30q button top @ $5.91/ea = $283.68
48 x Samsung 30q @ $5.18/ea = $248.64
32 x Basen IMR @ $7.26/ea = $232.32

Oh man! It's a wash on price difference. At least on one version of the 30q. And the 30q is a tested and true battery. And at a 6p it would have seriously more amperage available. 

Well, I'll just have to see how well this performs. I obsessed on batteries for months while planning. I guess I got it stuck in my head that as a single battery, these would do well. The weight is not an issues for me, as I'll be running this on my cruiser pintail.
```

---
## \#21 Posted by: sprocket12 Posted at: 2017-07-25T14:55:49.075Z Reads: 89

```
Sorry @Namasaki. My bad. I thought that was what you meant in your last post when you said you believed a 60a battery was just not adequate for hill climbing.
```

---
## \#22 Posted by: Titoxd10001 Posted at: 2017-07-25T16:03:19.968Z Reads: 87

```
People are buying 30q cells from nkon with good results. Looks like it would have been cheaper too
```

---
## \#23 Posted by: sprocket12 Posted at: 2017-07-27T20:52:24.423Z Reads: 78

```
Ok. Received welder. It is a Sunnko. A 788H model. Got for $120 after negotiating on eBay.
```

---
## \#24 Posted by: chsknight Posted at: 2017-07-27T21:36:59.736Z Reads: 83

```
that is a pretty solid deal.  I just got a sunko709a.   If you find a spot selling pure nickel strips, please let me know!   I have had no luck so far.
```

---
## \#25 Posted by: darkkevind Posted at: 2017-07-27T22:11:56.481Z Reads: 87

```
This one I can vouch for, it's what I bought.
http://www.ebay.co.uk/itm/263057602801

Not sure about this one though...
http://www.ebay.co.uk/itm/263057810676
```

---
## \#26 Posted by: sl33py Posted at: 2017-07-27T22:47:18.746Z Reads: 88

```
I'm with @Namasaki in recommending high amp/current batteries whenever possible.  it's why i've avoided 18650's for so long, because high C lipos were just a better match for me.  (40-60c rated lipos)

I'm delving into 18650's now to be like the cool kids...  I have a 3p HG2 setup in process which i expect will work well for mostly flats, and a VTC5a pack TBD (3 or 4p).  I've also been doing some testing to determine my true current consumption when riding.  Using an eagletree logger i have seen much less current draw than expected.  Peaking to around 46-50A on a single setup.  I'll do some more testing w/ some VESC Sixes since they have a higher current limit to see what my real-world worst case current draw would be - and then i'll overbuild from that measure.

I'm not a normal sized human (6'8"/2m - 265lbs/120kgs'ish) - on 'The Suga' (guest board) - 149kv 8s2p 60c (2x8s 5.8Ah 30c parallel) -  i saw 51A peak:
[img]https://goo.gl/Y6ou4z[/img]
(i have a nice bike path across the street and did a quick 4'ish miles with a couple nice long gradual hills, and a short steep one behind me i tried to stress it)  Most boards won't take me up, it did though slowed down midway to top.

On my GF's Vanguard - 190kv 8s 30c (2x4s 8Ah) -  i saw 46A:
[img]https://goo.gl/bYowz1[/img] 
Just a short ride to test, did not do the long gradual hill, just the one steep behind house.  (12mm belt started skipping and almost made the top of the last steep hill)

Both VESC 4.xx running FOC fw 3.26.

at 4p i think your setup will work really well - just somewhat bulky given the weight/size.
```

---
## \#27 Posted by: Namasaki Posted at: 2017-07-28T00:40:32.598Z Reads: 80

```
Looks like your 60C setup has very little sag regardless of high current peaks
```

---
## \#28 Posted by: sprocket12 Posted at: 2017-07-28T04:14:37.915Z Reads: 73

```
As @darkkevind has posted, eBay. I purchase 50x2" pieces of 10mm at .15mm thick but they are not enough and I will use them to connect the 4-packs. 

I found 10' rolls at about $4 on eBay. Of course I'll be waiting about 3-4 weeks to get them. That's ok. I'll keep going over plans and practice spot welding.
```

---
## \#29 Posted by: sprocket12 Posted at: 2017-07-31T20:27:10.689Z Reads: 67

```
So I've tested the 788H with a dead cell and watching a couple of YouTube videos. Disappointing results to say the least!

Any suggestions? I had sanded the welding tips as suggested elsewhere. I'll also clean everything with isopropyl alcohol too. But what have you found for settings on the spot welder? Amps? Pulses, etc?
```

---
## \#30 Posted by: sprocket12 Posted at: 2017-09-25T18:22:10.714Z Reads: 52

```
Build update.  The pack was finished but ran into other issues (broken switches, waiting on chargers, heatsinks, fans, ebay, amazon, etc.).  Ran maiden voyage of any distance this morning.  Went about 9 miles.  Everything seems solid.  :+1:

I started at about 76% charged as I had been doing short runs as I have been tweaking the VESC firmware.  After getting into work, I am at roughly 40% still charged.  That should put me solidly above the 20+ mile mark I was shooting for.

Incidentally, I was surprised when @Ackmaniac's Android app started telling me via my earbuds that my battery had discharged to 'x' level.  Pretty cool. :grin:
```

---
