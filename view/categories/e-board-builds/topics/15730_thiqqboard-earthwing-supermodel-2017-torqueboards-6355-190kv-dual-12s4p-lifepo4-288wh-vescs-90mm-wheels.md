# Thiqqboard &#124; Earthwing Supermodel 2017 &#124; Torqueboards 6355 190kv Dual &#124; 12S4P LiFePo4 288Wh &#124; VESCs &#124; 90mm Wheels

### Replies: 20 Views: 2392

## \#1 Posted by: dimnsionofsound Posted at: 2017-01-06T20:39:01.614Z Reads: 301

```
Hi Everyone!

I've done a lot of reading on here (stickies and suggested topics, parts, etc.) and I've finally compiled a parts list for my first build. 

I'll be using it for cruising around and to/from campus, which has a lot of hills and a particularly steep one that I'll be going up almost every day, about a 20-25% grade at certain points. I also want it to be water resistant so I don't just have to walk if it's a little wet out. For reference I'm about 170lbs, but I'll have a backpack and I'll probably be gaining weight as the semester goes on, gonna keep hitting the gym like I did this summer :stuck_out_tongue:

Here's the parts list:

**Deck and Mechanical**
[Earthwings Supermodel 2017 Deck](http://www.earthwingboards.com/_p/prd1/4424377861/product/supermodel-2017)
[Two DIY Electric Skatebord 190kv 6355 Motors](diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/)
[DIY Electric Skateboard Trucks and Dual Motor Hardware - 16 tooth pully and 90mm wheels ](diy-electric-skateboard-kits-parts/torqueboards-dual-motor-mechanical-kit/)
[Ceramic Bearings for rust resistance](https://www.amazon.com/gp/product/B00KQPJUKA/ref=od_aui_detailpages00?ie=UTF8&psc=1)

**Batteries and Electronics**
[12 2S2P LiFePo4 3.6Ah batteries](https://hobbyking.com/en_us/zippy-flightmax-3600mah-2s2p-30c-lifepo4-pack.html)
[12S 120A BMS](https://www.aliexpress.com/item/12S-120A-version-S-LiFePO4-BMS-PCM-PCB-battery-protection-board-for-12-Packs-18650-LiFePO4/32767760750.html?spm=2114.01010208.3.22.FJ9TKu&ws_ab_test=searchweb0_0,searchweb201602_2_10065_10068_10000009_10084_10083_10080_10082_10081_10060_10062_10056_10055_503_10054_10059_10099_10078_501_10079_426_10103_10073_10102_10096_10052_10053_10050_10107_10051_10106,searchweb201603_2,afswitch_5,single_sort_0_default&btsid=d44fad20-85dd-41f9-ad99-52127bb2cd3b)
[MOSFET Switch built with plans from this thread](http://www.electric-skateboard.builders/t/eboard-mosfet-switch/5738/70)
[2 DIY Electric Skateboard VESC](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/)
[Winning Remote](http://psychotiller.com/product/winning-24ghz-mini-thumb-stick-controller)
[3A 12S LiFePo4 Smart Charger](http://www.batteryspace.com/Smart-Charger-3.0A-for-38.4V-LiFePO4-Battery-Pack.aspx)

Total cost of everything above, sans taxes and shipping: ~$1300

**Misc**
Connectors/cables
Kydex for custom enclosure
Hot glue
Yoga mat or rubber to seal enclosure and for padding
Hardware to secure enclosure
Battery eliminator circuit for receiver
Arduino for pack voltage/state of charge monitoring
LEDs for battery status
Stronger LEDs for headlights/taillights
Pushbutton on/off switch


The theoretical top speed at nominal pack voltage is about 34 MPH with the 90mm wheels but with a factor of 70% to account for efficiency, losses, etc (I read somewhere that this is a good number), it should top out at about 24MPH at nominal pack voltage. 

Looking forward to making this! But before I do, am I missing anything obvious? I'll make another thread for the build, with a name and lots of pics once I get started.

Thanks!
```

---
## \#2 Posted by: JdogAwesome Posted at: 2017-01-06T20:59:15.279Z Reads: 265

```
Looks great! Though tackling those steep hills will definetly be hard. I don't have much experience with hills so I'll let someone else advise you on that. One thing I would change is that BMS. Mainly because it's very expensive and I don't recommend you use the current protection which is why it cost so much. What I recommend you do is get a cheaper BMS that's much lower amperage, and then just bypass the overcureent protection. That's what most of us do. Also are you sure you want to go with LiFe? There good if you don't like watching your board voltage or just being more careless with them, which is fine, but they have a lot less capacity. And I don't know how far your going but if there's a lot of hills, you might want a bigger battery than that. With my 6S 5000mAh for my board I only got around 4 miles of range on level ground.
```

---
## \#3 Posted by: JdogAwesome Posted at: 2017-01-06T21:02:45.585Z Reads: 244

```
Oh and I also just saw you mentioned my MOSFET switch thread, thanks! If you need any help with it just message me!  Also I'm currently out of town but I have a kit for the switch which comes with all the parts to assemble it yoirself for sale if your interested.
```

---
## \#4 Posted by: dimnsionofsound Posted at: 2017-01-06T21:12:52.015Z Reads: 230

```
Ah, thanks for the recommendation on the BMS! - I'll look into a cheaper one. 

I wanted to use LiFePo4 because of its cycle life (>4x that of Li-Ion) and safety, primarily. I'd like to think that I'm careful but in case of a short, or damage to the batteries, I don't want to worry about them exploding or catching fire, and in that regard LiFePo4 is remarkably stable. I also want to be able to leave it unattended while charging. This board hopefully should last for years without battery replacement as well. 

In terms of capacity, I think it should be fine. The total watt hours in the pack is (3.3V * 3.6 Ah * 2P * 12S) = 285 Wh which is almost 3x the default capacity of the boosted board (100Wh), which they claim gets 6-7 miles of range, so based on those numbers I think I could get almost 17 miles! I don't think I'll ever ride it that far but I want the peace of mind.
```

---
## \#5 Posted by: JdogAwesome Posted at: 2017-01-06T21:22:20.071Z Reads: 208

```
Those are definetly some good points! Though those are still pouch cells so you can still damage them which could cause some problems. The best would obviously be LiFe 18650's, but that's adds a lot of complexity and I'm guessing expense.
```

---
## \#6 Posted by: dimnsionofsound Posted at: 2017-01-06T21:28:51.910Z Reads: 208

```
Indeed, to build a pack of the same Wh rating with 26650 A123 cells would add about $200 to the battery cost, the [supplier I'm looking at](http://www.batteryspace.com/A123-System-Nanophosphate-LiFePO4-26650-Rechargeable-Cell-3.2V-2500-mAh.aspx) has individual cells for $12.82, I would need 36.

I'll probably just use the yoga mat or rubber I'm gonna cut up and pad the batteries a bit inside the enclosure to keep them happy and vibration free haha
```

---
## \#7 Posted by: karma Posted at: 2017-01-07T17:13:56.754Z Reads: 200

```
Or you could use Samsung INR18650 25R cells with 2500mAH for 3€ each and get a 324Wh 12S3P for 108eur from nkon :)
```

---
## \#8 Posted by: dimnsionofsound Posted at: 2017-01-22T14:25:19.004Z Reads: 205

```
Still waiting for the deck to come in the mail, but since I've got everything else, I started some assembly today. Water resistance is taking a backseat for the moment so I can just get it working and see if there are any glaring problems.

Had to spin the bolts once they were all the way in the wheels to get rid of the wheel material they dig into - on the first one I didn't do it and the wheel pulley was a little lopsided and hard to screw in. 

<img src="/uploads/db1493/original/3X/f/f/ff35721617b41d30716972fffbb25017042d5840.JPG" width="666" height="500">

Unfortunately my soldering iron is not nearly powerful enough to handle the 10ga wires coming from the batteries to the XT60's so I'm gonna go to the hackerspace tomorrow to get that done. 

<img src="/uploads/db1493/original/3X/f/a/fa35400bc683bc03f886152dba915fc1a30a7260.JPG" width="375" height="500">

Forming Kydex for the enclosure (which is pretty deep/thick, where I came up with the tentative name for this build) was surprisingly time consuming! Making the middle parts was not too hard but to create the end pieces first I tried to stretch the material down over the corner and then push down the wrinkles. That didn't work well at all, so I ended up just cutting and "welding" the plastic by putting the heat gun right next to it and squishing it together. Copious amounts of clamps were used (no idea if I would have been able to do it without the wood and clamps...). But now the hardest part of the build is mostly over!

The (almost finished) enclosure:
<img src="/uploads/db1493/original/3X/8/c/8c104119d49f0613a76bb05c161e976cb9c3ff64.JPG" width="375" height="500">

Trying to figure out what way to best position the batteries in the available space (before I made the end pieces):
<img src="/uploads/db1493/original/3X/7/e/7ee83a73ef410a051e4a3c05437eb1f07049718b.JPG" width="666" height="500">

More to come soon! So hyped for this!
```

---
## \#9 Posted by: dimnsionofsound Posted at: 2017-01-27T07:46:21.453Z Reads: 178

```
Update: Fried both my VESC's. Fuq

I did motor detection and switched to FOC on both, and separately, both were working fine. So I connected both via CAN bus, connected one to power, and then when I connected the other to power, the classic spark happened in the XT90, and boom, both are lights out and one of them whines. 

Mistake #1: Didn't connect them both to power at the same time
Mistake #2: Didn't use @JdogAwesome's MOSFET switch to do the connecting, that I had literally just built yesterday (Why? I don't know...)

Guess I"m out another $320. This time I'll be getting @chaka VESCs with the warranty and being even more careful with them. RIP DIY VESC's, you were lit while you lasted :'(
```

---
## \#10 Posted by: SirDiff Posted at: 2017-01-27T10:37:18.917Z Reads: 161

```
I think you have to reset the firmware before switching to FOC, otherwise you will fry your vescs
```

---
## \#11 Posted by: okp Posted at: 2017-01-27T10:38:39.866Z Reads: 157

```
not sure it was the appropriate move to go for FOC on 12S! this passion cost a lot of money!
```

---
## \#12 Posted by: dimnsionofsound Posted at: 2017-01-27T10:40:26.266Z Reads: 158

```
Strange, since I had both VESCs separately spinning up the motors in FOC, with braking and everything, before I connected them together and this happened. So that leads me to think that that wasn't the problem, possibly rather some voltage spike (?) generated by plugging in the other one without an anti-spark while one was already plugged in.

@unik even 12S LiFePo4? My fully charged pack voltage is only 43.2 volts. Why is FOC bad at higher voltages (even if I'm 75% sure that wasn't what did this)?
```

---
## \#13 Posted by: okp Posted at: 2017-01-27T10:40:51.583Z Reads: 157

```
oops, sorry didn't capture that :) do you really need FOC?
```

---
## \#14 Posted by: lox897 Posted at: 2017-01-27T10:41:28.725Z Reads: 154

```
You should've reset your firmware before switching. I am running my VESCX on 12S with no spark switch or anything on FOC and it's fine. Just have to reset firmware before switching.
```

---
## \#15 Posted by: dimnsionofsound Posted at: 2017-01-27T10:41:48.393Z Reads: 153

```
@unik I wanted it for the supposedly reduced noise and marginal efficiency increases that I've read about on here
```

---
## \#16 Posted by: dimnsionofsound Posted at: 2017-01-27T10:43:08.128Z Reads: 154

```
Yeah I'll be really careful next time! Don't want to fry more expensive components :open_mouth:
```

---
## \#17 Posted by: okp Posted at: 2017-01-27T10:44:15.193Z Reads: 154

```
really 12S on FOC ? that's awesome.
```

---
## \#18 Posted by: JdogAwesome Posted at: 2017-01-27T18:36:28.802Z Reads: 151

```
Oh shit that sucks! Sorry to hear that man, I hope my switch helps lol.
```

---
## \#19 Posted by: dimnsionofsound Posted at: 2017-02-14T07:29:15.185Z Reads: 143

```
Update:

Finally got my VESC's from Ollin in the mail this afternoon. I got home and configured them, did motor detection and canbus setup, etc. My limits right now are +- 80 Motor amps, +50, -5 battery amps, per VESC. 

The first ride was scary! The throttle response is very sensitive especially with the tiny torqueboards nano controller. I had to get used to barely moving it at first. Had to take it pretty slow so I could get to where my car was parked and grab my helmet, but once I had that, I tried acceleration and hills.

I don't think I've even used full throttle yet and the acceleration I'm getting is still amazing! The hill that I specifically designed this board to go up is absolutely no match for it, I sped up it at about 20 mph.

All in all I'm very satisfied with the power output, I think it may need some tweaking though for the throttle curve though, I may experiment with the modified BLDC tool's Watt Control mode.
```

---
## \#20 Posted by: Ackmaniac Posted at: 2017-02-14T07:52:02.043Z Reads: 146

```
BTW. Resetting the firmware before you switch to FOC doesn't make any sense. That's like you have to get completely naked before you put on a new pair of shoes. Otherwise you will brake your legs.
```

---
