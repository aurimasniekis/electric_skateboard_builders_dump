# First build, help appreciated

### Replies: 8 Views: 975

## \#1 Posted by: Quent17 Posted at: 2017-04-28T17:18:24.603Z Reads: 122

```
I have been lurking a lot these past few days and I'm almost ready to start ordering the parts. However, I have a few question and I'd like to make sure I'm doing everything right. Thank for you for taking the time to help me.

My project is to build a single motor boosted board clone like this guy https://www.electric-skateboard.builders/t/full-diy-revived-boosted-board-2-0/21296. I want to start with a single motor and maybe expand it to a dual motor later.

**My mass**: 60 kg.
**My usage**: Mostly for my commute, contains small hills.

Characteristics:

* **Desired top speed**: 25-30mph
* **Desired range:** 10-15 miles (16-24km); can be less (like 12km).

Here are my parts:

**Deck**: Similar to Loaded Vanguard (38")
**Trucks**: Caliber II 50’s
**Wheels**: Kegel 80 MM 80A Orangatang
**Bearings**: Bones Super Reds ([link](https://www.amazon.co.uk/d/Skateboard-Bearings/Bones-Super-Precision-Skate-Bearings/B002NES3MS/ref=sr_1_3?ie=UTF8&qid=1493235576&sr=8-3&keywords=bones+reds))
**Mount**: [Carbon motor mount by @Shogu12](https://www.electric-skateboard.builders/t/eu-us-22-carbon-motor-mounts-anodized-aluminum-clamp/20795)  
**Pulley System**: [Enertion 12mm pulley system](http://www.enertionboards.com/electric-skateboard-parts/12mm-wide-drive-pulley-kit/)
**VESC**: [DIY](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/) or [ENERTION](http://www.enertionboards.com/electric-skateboard-parts/vesc-x-programmable-brushless-motor-controller/) VESC
**Remote**: [2.4Ghz mini remote controller with receiver](https://www.aliexpress.com/item/2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32735708994.html?spm=2114.01010208.3.41.pWwY55&ws_ab_test=searchweb0_0,searchweb201602_1_10152_10065_10151_10068_10130_10136_10137_10060_10138_10155_10062_10156_10154_10056_10055_10054_10059_10099_10103_10102_10096_10148_10147_10052_10053_10142_10107_10050_10051_10084_10083_10080_10082_10081_10110_10111_10112_10113_10114_10179_10181_10182_10078_10079_10073_10070_10123_10124,searchweb201603_4,ppcSwitch_5&btsid=48383dcf-aca6-43fc-9e8d-04418c118f80&algo_expid=1a1d7cc6-5a06-45d3-b60e-e96c6273a117-5&algo_pvid=1a1d7cc6-5a06-45d3-b60e-e96c6273a117)
**VESC Case**: [3D Printed boosted board style VESC case](http://www.thingiverse.com/thing:1817161)
**Battery Case**: [3D Printed boosted board style battery case](http://www.thingiverse.com/thing:1834035)
**Motor**: This where I don't know, I've read about the SK3 - 6374 -192kv. Only thing I'm afraid if it will be too large if I add a second motor.
**Battery**: Also need help here. But my maximum size for the case is 240 x 140 x 30mm.
**Battery charger**: Also need help here.

Thank you so much for your help.
```

---
## \#2 Posted by: jaykup Posted at: 2017-04-28T17:39:41.994Z Reads: 106

```
**Motor:**

For dual rears on Caliber IIs you will need 6355 motors.  I've found a single 6355 and 6374 very comparable in power and not a massive difference at 12s.  Voltage plays the biggest role in power from what I've found.  You could do a dual diagonal setup with 6374s.

**Battery:**

Some reference for me:
16/36 gearing, kegels, 6355 or 6374, 12s will do just under 30mph at 800-1000 watts.  I do have my max ERPM set a bit below 60,000 so that's probably limiting my top speed.  Average ride speed is around 25mph and the board has no problem maintaining that at 1/4 throttle.  With taller gearing I have no doubt a single motor will take me to 35-40mph.

Amp draw from the battery rarely exceeds 40-50 amps, mostly on harsh take-offs or full throttle hill climbs.

12s4p single motor range is 20 miles +/- 2 miles with 25mph average speed and a few hills.  Tested this on at least 3 long continuous rides.  Motor size seemed to have no measurable effect on range.

Lot of people go with 10s, but if you are looking for crazy power that will put a smile on your face all day in amazement, 12s is really the way to go.  It will also throw you off the board if you accidentally grab full throttle when you aren't ready for it - a reason why I moved to the thumb throttle style controllers.  Leg still hurts.

Since you don't need the extended range, a 12s3p (15 miles) would be perfect, you might be able to get away with a 12s2p (10 miles) but then you'd be drawing 20-25 amps per cell under full acceleration and might be a problem in the long run.

**Battery Charger:**

I've had good luck with the meanwell led drivers - adjustable voltage and current.

<img src="/uploads/db1493/original/3X/3/0/307898f381649bbc696b5af9577a1d319359bd04.png" width="690" height="102">

HLG-185H-48A http://www.mouser.com/ds/2/260/HLG-185H-SPEC-806126.pdf

*adjustable voltage means I can deliberately undercharge my pack (4.0-4.1v per cell) to increase (perhaps up to 2x) my total cycle life.
```

---
## \#3 Posted by: Quent17 Posted at: 2017-04-28T18:15:41.392Z Reads: 92

```
Thank you for the high quality answer.

So I will go for 6355 motor.

Thank you for advising a 12s3p or 12s2p battery pack. My only constraint is that it must fit into a 240 x 140 x 30mm case.
Two questions:
1 - Should I get a lipo battery or lithium ion?
2 - Do you recommend a product in particular ?

Thank you very much.
```

---
## \#4 Posted by: jaykup Posted at: 2017-04-28T20:43:35.312Z Reads: 84

```
A 12s2p battery made of 18650 cells (lithium ion) should fit your case - but no room for VESC or anything else.

I prefer to make them my self out of Samsung 25r ($70) or Samsung 30q ($90) cells.

DIY and Enertion I think have pre-assembled packs, and a few people on the forums here make and sell packs.  A bit more expensive but worth it if you are apprehensive about building one.
```

---
## \#5 Posted by: Quent17 Posted at: 2017-04-29T17:18:58.020Z Reads: 73

```
Thank you, I'm going to buy my board today!
```

---
## \#6 Posted by: recursiveSlinky Posted at: 2017-04-30T22:43:20.374Z Reads: 61

```
@jaykup where are you finding your 25r's for ~2.90 a pop? least that's my approx for a 12s2p for $70.
```

---
## \#7 Posted by: jaykup Posted at: 2017-05-01T15:25:49.778Z Reads: 56

```
https://ru.nkon.nl/samsung-18650-inr18650-25r.html

Takes a while to get them (2-4 weeks) but lowest price I've found for genuine cells.
```

---
## \#8 Posted by: pyttroll Posted at: 2017-05-01T19:21:06.203Z Reads: 48

```
I would suggest getting 30Q's instead of the 25R, more capacity, small price difference.
```

---
