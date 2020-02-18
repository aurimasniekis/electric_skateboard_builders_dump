# Old Man Cruiser New Re-Build

### Replies: 38 Views: 3034

## \#1 Posted by: sprocket12 Posted at: 2016-08-17T16:28:58.805Z Reads: 254

```
Hi all.  I've posted a few times as I was trying to work my way through a 'cheap' build but the more I read, it has become apparent the less I knew.

I had been building a 46" pintail cruiser.  I had purchased almost all of my parts second hand (though new)  but blew it thinking I could use some old 18650 batteries.  Most were Samsung or LG but they suck.  I tried using soldered battery sleds but during my first 'real' ride I had multiple failures.  Kinda discouraging.

My goals are still 10-12 miles on a single charge with a weighted speed up to 25 mph.  Can you all review this list and tell me if it looks ok?  I'm struggling with the batteries most.  Thanks...

**What I have:**
Turnigy Aerodrive SK3 - 6354-260kv
http://www.hobbyking.com/hobbyking/store/__18127__Turnigy_Aerodrive_SK3_6354_260kv_Brushless_Outrunner_Motor.html
Enertion VESC Ver 4.12 fw 2.18
http://www.enertionboards.com/electric-skateboard-parts/vesc-standard/
Sparkless On/Off Switch 2s-12s 120A/60V
diy-electric-skateboard-kits-parts/electric-skateboard-on-off-power-switch/
TorqueBoards 2.4Ghz Mini Remote Controller
diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-mini-remote-controller/
46" Pintail Cruiser Deck
http://www.ehlerslongboards.com/index.php/complete-longboards-skateboards/customize-your-own-pintail-9-5-x-40-complete.html
Enertion Trucks
http://www.enertionboards.com/electric-skateboard-parts/longboard-trucks.html
83mm Wheels
Pulleys- 14t/35t

**What I don't have:**
ZIPPY Flightmax 8000mAh 4S1P 30C x2
http://www.hobbyking.com/hobbyking/store/__20823__ZIPPY_Flightmax_8000mAh_4S1P_30C_US_Warehouse_.html
Turnigy P606 LiPoly/LiFe AC/DC Charger (US Plug)
http://www.hobbyking.com/hobbyking/store/__97456__Turnigy_P606_LiPoly_LiFe_AC_DC_Charger_US_Plug_US_Warehouse_.html

Will these batteries do what I want (in series)?  Or should I go with something else?  How about this charger?  Is it ok?  I am ready to pull the trigger....:grin:
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-17T16:51:11.652Z Reads: 216

```
Everything seems fine. You should hit almost 30mph (I'm assuming you meant 14/36 ratio, not 14/35) if not more. I'd consider dropping to 6s if you don't want to go that fast. 

I'd recommend getting a nice 18650 or 26650 pack instead, but lipos work as a cheaper alternative. You should get about 14 miles on flats on your battery.
```

---
## \#3 Posted by: zeno Posted at: 2016-08-17T17:02:59.064Z Reads: 211

```
Charger can only do 6s max reading from the specs.  This would work if you put the 4s in parallel to charge.  If you want to keep them  in series while charging  (==8s) you need to find a different charger.  

Dropping to 6s (2x3s, 1x6s) like @jinra suggest would obviously work as well :)
```

---
## \#4 Posted by: zeno Posted at: 2016-08-17T17:10:48.324Z Reads: 201

```
Hmm, if I put in your info in the calculator with **6s** I get a top speed of only 22mph (**unweighted**):

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":6,"motor-kv":260,"system-efficiency":80,"motor-pulley-teeth":14,"wheel-pulley-teeth":35,"wheel-size":83}|

since you mentioned you want to go **at least** 25 mph **weighted** this would not suffice. 
8s would get you in the proximity of 25. Whilst 10s would definitely get you there. Problem with 10s is that you would have an eRPM of +/- 67000+ which as I remember is too much for the vesc to still be reliable :(
```

---
## \#5 Posted by: zeno Posted at: 2016-08-17T17:12:17.937Z Reads: 175

```
perhaps 8s with 90mm wheels? (32 mph unweighted, 25mph weighted with a guestimate of 80% efficiency)
```

---
## \#6 Posted by: sprocket12 Posted at: 2016-08-17T17:13:11.088Z Reads: 178

```
Hey thanks for the quick response!  

There are a few reasons for my going with the lipos...Mostly though, I don't trust my own handywork. I'm sure I'll have some bad soldering nail me about 5 miles into a ride! :stuck_out_tongue_winking_eye:  And then I'll incur further costs to fix or have someone else do it.
```

---
## \#7 Posted by: saul Posted at: 2016-08-17T17:16:12.424Z Reads: 163

```
Wow this is oddly similar to my build, I used the 44" bamboo pintail on 97mm clones. 

tried the 83mm's for a while but 97mm are so much smoother if you don't mind the weight... just keep riding and yo won't notice tho..
```

---
## \#8 Posted by: sprocket12 Posted at: 2016-08-17T17:21:01.059Z Reads: 152

```
Ok, this is what I needed to know!  I was thinking I could just unhook the series and charge them separately, but that would be a pain.  Any suggestions on a charger?

I like the 8s setup.  What happens if I drop to constant discharge of 10C per pack like in this one?
Multistar High Capacity 4S 10000mAh Multi-Rotor Lipo Pack
http://www.hobbyking.com/hobbyking/store/__64438__Multistar_High_Capacity_4S_10000mAh_Multi_Rotor_Lipo_Pack_US_Warehouse_.html
I know I'll go about 25% further but what about speed?  How much would it be affected?
```

---
## \#9 Posted by: Jinra Posted at: 2016-08-17T17:23:50.788Z Reads: 143

```
You should be fine with 100amp discharge. Speed is based on voltage, which should be the same if you run 8s.
```

---
## \#10 Posted by: sprocket12 Posted at: 2016-08-17T17:28:42.537Z Reads: 141

```
Wow!  I had a hard time even finding an 8S lipo charger.  When I did, they are like 4 times the cost.  Perhaps I should just put up with disconnecting the series to charge?  What do others do?
```

---
## \#11 Posted by: zeno Posted at: 2016-08-17T17:35:16.617Z Reads: 143

```
A lot of people just put up with the disconnecting hassle for charging I believe. Other choices could be a more expensive charger of buying a BMS that you attach to the board/batteries to pair up with a simpler charger. BMS's however do not seem to be that cheap either. :(

Perhaps you should start with the hassle of disconnecting first. Maybe it's not that big of a hassle and you'll be fine with it, and at least you get to ride! After that you can always opt for going a step further..
```

---
## \#12 Posted by: sprocket12 Posted at: 2016-08-17T17:37:22.582Z Reads: 136

```
Ok.  I'm purchasing the Zippy's and the 6s charger.  I'll open the case and charge the batteries separately.  Woohoo!
```

---
## \#13 Posted by: Jinra Posted at: 2016-08-17T17:37:47.384Z Reads: 127

```
+1 on the BMS option, super simple after you get it setup.
```

---
## \#14 Posted by: sprocket12 Posted at: 2016-08-17T18:09:27.814Z Reads: 129

```
Yeah!  Order confirmed and sent to warehouse for fulfillment!  Looking forward to riding...:grin:
```

---
## \#15 Posted by: zeno Posted at: 2016-08-17T18:29:50.148Z Reads: 133

```
Whoop whoop! :heart_eyes:
```

---
## \#16 Posted by: sl33py Posted at: 2016-08-17T19:25:14.531Z Reads: 143

```
[quote="sprocket12, post:10, topic:7806, full:true"]
Wow!  I had a hard time even finding an 8S lipo charger.  When I did, they are like 4 times the cost.  Perhaps I should just put up with disconnecting the series to charge?  What do others do?
[/quote]

I usually run 8s (a good moderate setup w/o as much likelihood of DRV issues) - plenty of power for me even on a single motor setup (geared correctly).  I also disconnect to charge - not a big deal and i find it plenty easy.

As for chargers - inexpensive ones i recommend is the iMax B6ACv2.  If you can swing a nicer one - go for it.  I especially like the advanced features of the iMax - similar to nicer ones like iCharger (great!) - like Internal Resistance testing.

I'd avoid any charger that charges via the balance plugs.  They are usually much slower and moving 5-6 amps across those small wires seems like a bad idea...  but others may do this and have no issues.
```

---
## \#17 Posted by: sprocket12 Posted at: 2016-08-17T22:25:14.363Z Reads: 140

```
How did you attach/protect your gear?  I didn't find anything that would work with the deck's curvature. I also wanted flex. I ended up using spray insulation sculpted down with silicone covering it. It's ugly but it works.
```

---
## \#18 Posted by: sl33py Posted at: 2016-08-17T23:04:17.153Z Reads: 182

```
a flexy deck is definitely a challenge.  The best solution i've seen is top mount power so the middle is clean (okp, whitepony, and squad's are all amazing).  Separate your batteries and ESC front and back so the middle can flex.  Less area for batteries - but let's everything work w/o flexing the enclosure and killing a flexy deck.

enclosures - they've done custom CF, and abs(Vacuum formed) to fit the vanguard.  

i'd read through @whitepony's build here:
http://www.electric-skateboard.builders/t/loaded-vanguard-tesseract-jet-spud-vacuum-bagging-boards-enclosures-with-carbon/4218

Tons of great pictures and ideas how to do it.  GL!
```

---
## \#19 Posted by: sprocket12 Posted at: 2016-08-18T19:57:40.704Z Reads: 176

```
I can't believe that my Zippy's and charger have already arrived!!!  Now I need VESC experts review my settings.  I would rather be a little conservative then burn something up.  I can't pull screenshots (At work and didn't expect overnight delivery)  but have written down what is currently configure.  The hardware is the same as listed at the top of this thread.  Is this good?

**Motor Configuration**
**Motor Tab**
_Current Limits_
Motor max: 70.00 A
Motor min: -30.00 A
Batt max: (not sure. 100 A? My 30c at 8000mAh says 240 A but Vedder says absolute max no higher than 150 A.  So...?)
Batt min (regen): -15.00 A
Absolute max: 150.00 A ??
Slow absolute max: CHECKED

_Temperature Limits_
MOSFET Start: 80.00 C
Mosfet End: 100.00 C
Motor Start: 80.00 C
Motor End: 100.00 C

_Other Limits_
Minimum duty cycle: 0.005
Maximum duty cycle: 0.950

_RMP Limits (BLDC Only)_
Limit ERPM with negative torque: CHECKED
Min ERPM: -100000.00
Max ERPM: 100000.00
Max ERPMN at full brake: 300.00
Max ERPM at full brake in current control mode: 1500.00

_Voltage Limits_
Minimum input voltage: 8.00 V
Maximum input voltage: 57.00 V
Battery cutoff start: 26.00 V
Battery cutoff end: 24.00 V

**BLDC Tab**
Sensorless: SELECTED
_Sensorless_
Min ERPM: 600.00
BR ERPM: 80000.00
Phase advance at BR ERPM: 1.00
Max brake current at dir change: 10.00

_Sensorless - Communication Mode_
Comm Mode: Integrate
Integrator Limit: 72.00
Int Limit Min ERPM: 1100.00
BEMF Coupling: 920.00

_Hall Sensors (failed during *ALL* attempted detections)_
Table: -1/1/3/2/5/6/4/-1
Sensorless ERPM (hybrid mode): 2000.00

_Detect Parameters_
Current: 6.00 A
Min ERPM: 600.0
Low duty: 0.05

**App Configuration**
**PPM Tab**
_Control Mode_
Current no reverse with brake: SELECTED

_Settings_
PID max ERPM: 15000.00
Deadband: 0.15
Minimum Pulsewidth (ms): 1.15
Maximum Pulsewidth (ms): 2.05
Use Median Filter: CHECKED
Safe Start: CHECKED
No other settings configured except Display for monitoring remote control
```

---
## \#20 Posted by: Jinra Posted at: 2016-08-18T20:24:11.719Z Reads: 158

```
Battery cut off is a bit low for lipos. may want to take it to 3.5 or 3.6 per cell start with a 3.4 per cell end, though it really depends on your pack.

Have you done motor detection? Integrator limit seems a bit low.

Batt max just match to your motor max.
```

---
## \#21 Posted by: sprocket12 Posted at: 2016-08-18T20:34:10.483Z Reads: 144

```
I have done motor detection.  The motor settings are from the previously run with old batteries.  I'll run detection a few times with the new batteries and update from there.

So my updates are:

* Battery cutoff start: 28.80 V
* Battery cutoff end: 27.20 V
* Batt max: 70 A
* Integrator Limit: (**TBD**)

Should the 'Absolute max' be the same at 70.0 A too?
Thanks!
```

---
## \#22 Posted by: Jinra Posted at: 2016-08-18T20:36:29.885Z Reads: 141

```
Try running detection 5 times and averaging the result. Round down to the lowest 5 for int limit and lowest 50 for bemf coupling.

You should probably just leave absolute max at the default 130A
```

---
## \#23 Posted by: zeno Posted at: 2016-08-21T17:15:12.794Z Reads: 138

```
Did you get it all working?

 And..  Show us pics! :)
```

---
## \#24 Posted by: sprocket12 Posted at: 2016-08-22T15:42:20.742Z Reads: 145

```
Sorry.  What free time I've had I have been working on getting up and riding...

I got the Zippy's in a day after ordering and started charging at .5 amps (i wasn't in a hurry).  That took a couple of days.  I had to re-work a couple of bullet connectors as I had XT60's on my 18650 set up.  Anyway,  that all got done.  I next updated my VESC settings based on feedback.  I took it out on another easy run on Saturday.  Wow!  What a difference!  Plenty of power/torque.  It was perfect... until it started slowing down. :sob:

It was 97F outside.  I had some slight hills (if you could even call them that).  It would come to a crawl even on flats.  I figured it was heat related.  I'd let it cool down for a couple of minutes and the power was right back!  When I returned home, I took of the bottom to the case and checked components for heat.  The batteries were negligibly warm at best.  They had dropped to about 90% charged and rebounded to 100% after a few minutes inside.  The motor was hot to the touch but bearable.  The VESC was really hot but touchable.  I figure I need to get some venting in my case?  It has but one small hole on the bottom...

I'm somewhat embarrassed of my build quality.  Due in part to my lack of ability and impatience to get riding.  The board is a bit of a mess.  Sorry to disappoint.  But since help is appreciated, I'll more than accept some constructive criticism on improving this neophyte's first build.

<img src="/uploads/db1493/original/2X/e/edda251381f83adf8e942b72b48b673a025c4f28.jpg" width="638" height="500">
Before any hardware installed...

<img src="/uploads/db1493/original/2X/b/bbf32dcaeba6c4418d65996ed60a8d6d938d058b.jpg" width="690" height="388">
After a hot and dusty ride.  The anchors aren't completely tightened on the bottom cover here...

<img src="/uploads/db1493/original/2X/e/ee74155b28d10188c9d08a6dd528fa5a05724ecd.jpg" width="281" height="500">
Another after my first ride.

<img src="/uploads/db1493/original/2X/0/0158417a52abc6dc8a5df415f05a588a01ab398a.jpg" width="690" height="388">
Facing down, I have a sparkless soft switch and battery meter embedded in the silicon.  

I didn't take any shots with the case open.  I have some wire shortening to do once I get the layout finalized.  I used packing foam for vibration to keep the VESC, remote control receiver, and software switch board from getting beat up.
```

---
## \#25 Posted by: sl33py Posted at: 2016-08-22T16:39:34.091Z Reads: 133

```
Looks really good man!  I'd definitely get some airflow for your VESC if you can.  On a hot day it sounds like that's the issue.  Might also look to add some small heatsinks to the FETs.

Your enclosure looks good to me!  I've ridden a lot worse - especially when impatient and want to ride right away!

One of my "test" setups was just painter's tape!  Worked with velcro as backup just in case.  Not pretty though!
[img]https://goo.gl/yXZ1Za[/img]

One of the best things i did was get a decent solder station - and learned how to make my own wires.  Really makes a difference when you have "spaghetti" wiring shoved into an enclosure - shorten it and clean it up will also help w/ any airflow.

I'd measure the FETs for right size to get but something like this:
http://www.ebay.com/itm/8pcs-Lot-Small-Aluminium-Heatsink-For-Computer-Xbox360-PS-VGA-Chips-Cooling-/221576571622

HTH - GL!
```

---
## \#26 Posted by: sprocket12 Posted at: 2016-08-22T19:17:30.907Z Reads: 123

```
Thanks @sl33py!  I have mixed feelings on the heatsinks from reading through the forum.  What experience have you had?  How long have you used them?  How well have they stayed in place?  Are you using the adhesive that was already on the heatsink or other?  Questions, questions, and more...  The desert heat and dust from eastern Washington gets into everything.  

I will definitely shorten and re-solder once I finalize how everything is laid out on the board.  I really like the size of the cruiser.  I hit about 20 mph with fantastic stability.  Now if I can stop reading about controller lockups I'll put more trust into my setup. :stuck_out_tongue_winking_eye: 

As for my enclosure, what I really want is one formed in a shape similar to what I have, maybe a little smaller (with a lip to screw down to board) but made from a single extruded ABS or vacuum process.  That would be perrrrrfect. However, I'm not up to taking that on... If anyone can do that for a fair price, I would be very interested.
```

---
## \#27 Posted by: zeno Posted at: 2016-08-22T20:34:04.744Z Reads: 112

```
Looks pretty decent to me! 
Love that deck BTW! :) 

Hope you can figure out the problems you're having.
```

---
## \#28 Posted by: sprocket12 Posted at: 2016-08-23T05:32:53.502Z Reads: 109

```
OK. Cooler day today in the desert, mid 80's. Did a test run without cover. Everything good until one of my lipos fell and got drug around! It came out ok. Used a shoelace (MacGyver style ;P). Headed home, almost all uphill and under power. No problems!

Ordered heatsinks that @sl33py referenced. Now I need to modify the case...
```

---
## \#29 Posted by: sl33py Posted at: 2016-08-23T17:42:06.960Z Reads: 108

```
Sounds like airflow is really needed.  Adding heatsinks and then covering them isn't likely to help much if at all.

I have some heatsinks, but haven't installed them yet.  Did you measure your FETs to make sure the ones i linked on ebay fit?  I'm pretty sure they'll work, but i did not measure to confirm.
```

---
## \#30 Posted by: sprocket12 Posted at: 2016-08-31T01:41:31.867Z Reads: 97

```
Update: rides smooth now.  I added more venting and the heatsinks.   All is well in the land of sun again! :blush:
```

---
## \#31 Posted by: sprocket12 Posted at: 2017-05-02T18:25:40.691Z Reads: 63

```
Spent time over winter and rebuilt...again. version 2.0
<img src="/uploads/db1493/original/3X/5/c/5cc2bd4ffd14c5da1002257454902c72403bc894.jpg" width="374" height="500">

And fixed cases
<img src="/uploads/db1493/original/3X/0/b/0bda0385f1c0e3460a9c221c86f27e620d74ebe2.jpg" width="374" height="500">

Added fan with switch for VESC
<img src="/uploads/db1493/original/3X/3/d/3d3b3c42acb8d601c1cc54a3be8fffdca2efe857.jpg" width="374" height="500">

Learned a lot about working with Kydex too.
A few more sbots....

<img src="/uploads/db1493/original/3X/a/e/aef1011089ae68cdfc455e2870931b28df7de4a6.jpg" width="374" height="500">
```

---
## \#32 Posted by: sprocket12 Posted at: 2017-05-02T18:45:07.742Z Reads: 58

```
Trying to upload more lics

<img src="/uploads/db1493/original/3X/3/7/37c5e7ba6c73353dec137adf7f3ac95eb22d768f.jpg" width="374" height="500">
```

---
## \#33 Posted by: sprocket12 Posted at: 2017-05-02T18:58:42.334Z Reads: 56

```
<img src="/uploads/db1493/original/3X/d/3/d3c6dd420c30b1dd7682c2050344b124232f6f22.jpg" width="374" height="500">
```

---
## \#34 Posted by: sprocket12 Posted at: 2017-05-02T18:59:40.609Z Reads: 59

```
<img src="/uploads/db1493/original/3X/9/5/95e80d457a8d639e77b4e041f9bf853270d43fa4.jpg" width="374" height="500">
```

---
## \#35 Posted by: sl33py Posted at: 2017-05-03T18:17:47.119Z Reads: 52

```
Nice!  Did you hydro-dip your enclosure?  Love how it incorporates the battery enclosure to the deck graphics!
```

---
## \#36 Posted by: sprocket12 Posted at: 2017-05-03T18:39:29.699Z Reads: 49

```
@sl33py do you mean plasti-dip paint?  I had used it in the past, but dust sticks to it like "nobody's binness"!  If that is not what you meant, please enlighten me.

I did use spray paint for plastic to clean things up after sanding.  I'll be using some 3M adhesive to cement all the vinyl stickers more permanently.  Arranging and applying took a long time but I am happy with the results.
```

---
## \#37 Posted by: sl33py Posted at: 2017-05-03T19:03:50.904Z Reads: 48

```
I've tried it on some electronics enclosures w/ mixed success.  Mostly just takes a bit of practice.

It's an ink transfer process basically.  A film is set in warm water - then "activated" w/ a spray to adhere to the part you dip.

Here's a little how-to from a kit seller:
https://youtu.be/eAc2y6JixHk

Look at the "sticker-bomb" film - similar to yours but w/ color stickers.
[img]https://images.duckduckgo.com/iu/?u=https%3A%2F%2Fimages-na.ssl-images-amazon.com%2Fimages%2FI%2F61KUVQBpO6L.jpg&f=1[/img]

HTH - GL!
```

---
## \#38 Posted by: sprocket12 Posted at: 2017-05-03T20:41:47.646Z Reads: 38

```
Cool.  I see.

I just did the layout by hand with a pack of vinyl stickers.
```

---
