# The Putting-My-Kids-On-A-Bread-And-Water-DIET-Build &#124; 97mm ABECs &#124; Single drive &#124; 10s4p &#124; Etcetera!

### Replies: 34 Views: 2806

## \#1 Posted by: Sebike Posted at: 2017-06-30T23:22:33.346Z Reads: 374

```
Hi all!!
This esk8 thing totally disturbed my mind and all I do day in day out this last month is reading on this forum and planning for my first build.. Did some skateboarding about 30 years ago, but no longboarding experience. Can't wait to be on a skateboard again though!

I'm in my early 40s, student with family, trying to figure out how to manage with this build and still put food on the table for my three girls. :slight_smile: 

I'll use the deck mostly for daily commuting ~ 8-10 km / day. One steeper 100m climb, but mostly flat. I weigh around 80 kg, that is 170+ lbs. Yes, I'm European and go with the metric system :smiley: I'd definately take torque over speed. 35 km/h top speed is good enough if torque is good. Limited to single drive though due to limited funds..

This is roughly what I have in mind for the build;

The trickier stuff;

**Deck** - Around 36" x 10" with some mild concave, stiff, but model/brandwise no idea. Seen a lot of boards in online shops and builds that look good. Scared of wheel-bite and not sure what would work with my 97 mms without using 4" risers. :smile: Any tips in the **sub** $100 range would be greatly appreciated!!

**Motor** - One of my -biggest concerns- - 6374 sensored 170 kv is what I have in mind, sealed would be nice and 8mm shaft would be good. Quality would be a plus of course. Can't seem to find one though. Want it to be strong enough to give good torque with my setup - start from stand still without push, make that one steep climb. Thoughts and/or tips?

**Motor mount** - interested in @WSB's "stealth motor mounts" if they'll become available again.

**Drive pulleys/ belt** - 14 or 15T / 40T from @Titoxd10001 and 15 mm belt (if there is room)

**Battery** - Aim is 10s4p 18650. Not sure if 25R is good enough or maybe 30q. One day I see myself soldering, next day I'm getting an Arduino spot welder... So many options...  

The less tricky stuff;

**Trucks** - Caliber II 50 10" - probably not so tricky..

**Wheels** - OG ABEC Flywheels 97 mm 75a  - on their way to me. Only part I've $$ for so far.

A reliable **BMS** for charge and discharge. 

EU built **VESC**

I'd like to get a Benchwheel **remote**, but hard to find at an ok price IF you find one, right?


Pull out spark plug. No fancy LED switches.



Some input on this setup maybe? :sunny:
```

---
## \#2 Posted by: NickTheDude Posted at: 2017-07-01T00:10:04.373Z Reads: 339

```
Just about all of that looks pretty good! Everything should work out to the type of speed/torque you are looking for. However if you're looking to save some cash it might be a good idea to build a smaller 18650 pack or get lipos instead. 8-10km a day would probably only take around 120Wh. A 10S4P of Q30s would be 333Wh. If you went with a 10S3P of Q30s I think you'd be fine in terms of voltage sag since you're going single motor and you'd still have a range of around 20km.
```

---
## \#3 Posted by: Sebike Posted at: 2017-07-01T10:02:11.712Z Reads: 301

```
Thanks. I've been thinking of maybe going 3p to save some money. It's tempting to have more capacity, but there's always a possibility to upgrade later on. Going 3p or 4p doesn't need any additional configuring/changes apart from the battery itself, right? 

You don't happen to have any tips on motors? Esk8.de and APS I believe have 6374s 170kv, but not in stock and with 10mm shafts. And I figure there isn't any easy way of adjusting 10mm motor shafts to fit 8mm pulleys? :smile:
```

---
## \#4 Posted by: karosass1 Posted at: 2017-07-01T10:54:17.214Z Reads: 282

```
If you are fine with paying a little bit additionally nkon.nl can pre-weld battery packs by your requirements. Last time I asked, he said it'd additional 40 euros for 10s3p
```

---
## \#5 Posted by: Sebike Posted at: 2017-07-01T14:32:28.500Z Reads: 270

```
Thanks for the tip. Definitely something to consider if they'd use adequately dimensioned nickel strips/copper... Did anyone get their batteries welded by them yet?
```

---
## \#6 Posted by: Sebike Posted at: 2017-07-05T11:15:51.027Z Reads: 263

```
Work in slow progress..
Have bought/ordered a few things;

Deck: Slipstream DFA 2015 - 36" x 9,4"
Wheels; ABEC Flywheels 97mm from Sickboards (NL) - apparently they were not in stock (listed in stock), but they say they're restocking on these. Fingers crossed..
Bearings; Bones Super Reds
Trucks; Caliber II 10" 50 from Blue-Tomato
Risers; MiniLogo 1/2"
Motor mount with belt cover; Stealth by @WSB
Wheel- and motor pulleys; 40T/15T 15mm via @Titoxd10001
BMS; 10S 60A from SuPower
Charger; Laptop style charger  from Aliexpress

I guess I'll go with an unsensored **SK3 6374 192 kv**, since I can't find any sensored 170kv that I like. Price also a factor here..
**VESC** - probably from @esk8 Attila,, magyar? :wink:
**Batteries** - will most likely choose 25R 10s4p over 10s3p 30Q. With better funds I would prob go with 30q x 4p though.
```

---
## \#7 Posted by: esk8 Posted at: 2017-07-05T17:46:29.218Z Reads: 227

```
Yes you're right :+1:
```

---
## \#8 Posted by: esk8 Posted at: 2017-07-05T17:52:50.759Z Reads: 225

```
Next Week we became delivered the new motors,
and now we have the sensor 6Pin cable for our ESK8 controller
soldered now.
So that you can used without soldering with the Vesc.
```

---
## \#9 Posted by: Sebike Posted at: 2017-07-05T19:17:51.077Z Reads: 214

```
Still only with 10mm shafts right? Is there any way to get these with 8mm?
```

---
## \#10 Posted by: sl33py Posted at: 2017-07-05T19:47:55.534Z Reads: 231

```
[quote="Sebike, post:1, topic:26469"]
Deck - Around 36" x 10" with some mild concave, stiff, but model/brandwise no idea. Seen a lot of boards in online shops and builds that look good. Scared of wheel-bite and not sure what would work with my 97 mms without using 4" risers. :smile: Any tips in the sub $100 range would be greatly appreciated!!
[/quote]

If you plan to run 97's - you are pretty limited on decks without MONSTER risers...  I would suggest a symmetrical deck - i'd also suggest a stiff deck to start for ease of setup.  Yes you can build a flex deck (and the flex is nice for smoothing a rough ride - but big soft duro wheels are great for this too), but it gets more complicated for your enclosure and typically you need to split your batteries and electronics leaving middle free to flex.  If you don't do this you will have issues with flexing inflexible things (like battery packs), or cracking enclosures etc.

I would look at daddies board shop and look for a shape you like - i like their quick view info around length/width, and flex.  I might also suggest wedged risers if you just need a smidge more room to avoid wheelbite.  It'll also make it more "turny" which is fun at low speeds - but might be a bit squirley at high speeds (depends on skill - but speed wobbles suck).

[quote="Sebike, post:1, topic:26469"]
Motor mount - interested in @WSB's "stealth motor mounts" if they'll become available again.
[/quote]
I'd also add @korryh to your list for an inexpensive motor mount.  Great quality and price, and has frequent stock so shouldn't need to wait very long.  Not sure of shipping cost though... 

[quote="Sebike, post:1, topic:26469"]
Drive pulleys/ belt - 14 or 15T / 40T from @Titoxd10001 and 15 mm belt (if there is room)
[/quote]
Last i heard he was out of both motor/wheel gears and only had wheel gears - get them while you can!  It's relatively easy to find motor gears online, with a bit of hunting, but usually without a 3mm keyway.  I've used w/o and just add a bit of extra blue loctite, and a good grub screw flat spot or drilled point to hold it securely.

[quote="Sebike, post:1, topic:26469"]
Battery - Aim is 10s4p 18650. Not sure if 25R is good enough or maybe 30q. One day I see myself soldering, next day I'm getting an Arduino spot welder... So many options...
[/quote]
Personally if on a budget I would stick to Lipo.  Yes you can get an 18650 pack (i'd suggest the 30q or VTC5A's), but still $$$ even if you have a spot welder already.  I'd suggest the highest C pack you can afford and fit.  

[quote="Sebike, post:1, topic:26469"]
Benchwheel remote,
[/quote]
I'm pretty consistent and almost always suggest the GT2b - you can ride it stock and 3d print a smaller enclosure later.  Super reliable connection even in high 2.4 congested areas (wifi and bt both use 2.4).

HTH - GL!
```

---
## \#11 Posted by: Sebike Posted at: 2017-07-05T22:30:34.841Z Reads: 220

```
Thanks a lot for taking your time @sl33py!  
[quote="sl33py, post:10, topic:26469"]
you are pretty limited on decks without MONSTER risers
[/quote]
I actually bought a deck already so I'll do my best to make it work with the 97s. The deck has a concave that, tigether with cut outs, lifts the edges to around 4/5"-ish. Hopefully that'll be ok with 1/2" standard

 risers. We'll see though.. Deck is stiff. <img src="/uploads/db1493/original/3X/b/d/bd38a6067fb248692bbe374601fc84e71accffdc.jpeg" width="690" height="388">

[quote="sl33py, post:10, topic:26469"]
Last i heard he was out of both motor/wheel gears
[/quote] I might have gotten his last set :slight_smile:
[quote="sl33py, post:10, topic:26469"]
almost always suggest the GT2b
[/quote]

Great tip.
```

---
## \#12 Posted by: Sebike Posted at: 2017-07-25T23:41:54.003Z Reads: 209

```
Slow progress and waiting for more parts. 
Deck is a Slipstream DFA 36" x 9.4" 
Caliber II 50° trucks and wedge risers
97mm 75a ABEC11 Flywheels with Bones super reds bearings
<img src="/uploads/db1493/original/3X/d/a/da780f367eb87048fabd848ebb2772e05b03f977.jpeg" width="271" height="500"><img src="/uploads/db1493/original/3X/2/1/215eae5e1692f789ba629242a163ef6a419180d0.jpeg" width="236" height="499"><img src="/uploads/db1493/original/3X/a/7/a769501c17e4191c11293206a42b74b4b7dee866.jpeg" width="229" height="500"><img src="/uploads/db1493/original/3X/8/f/8f521f88a89e13c2a06cf7bcbb622b2fb4c8ac12.jpeg" width="272" height="500">
```

---
## \#13 Posted by: sl33py Posted at: 2017-07-26T23:04:53.467Z Reads: 200

```
Nice looking deck!  Now get your electronics installed and get it powered!

I'd also double check your clearance at full lean - realizing that a hard turn in motion is more energy/compression than just tilting it on the carpet!  Make sure you don't get wheel bite.

Look for good bushings that are correct for your weight while at it - makes a *huge* difference in quality of ride.  I like the super high rebound bushings from Venom, Blood Orange, Riptide, etc. 

GL!
```

---
## \#14 Posted by: Sebike Posted at: 2017-07-26T23:27:21.123Z Reads: 200

```
Some changes were made to the initial plan and most of the stuff I have bought already, so here is what my setup will look like;

**Drivetrain;**
Motor mount - @WSB's Stealth motor mount 
Drive pulleys - 15T / 40T steel pulleys from @Titoxd10001 
Belt - [15mm wide](https://www.aliexpress.com/item/5pcs-HTD5M-belt-265-5M-15-length-265mm-width-15mm-53-teeth-5M-timing-belt-rubber/32635385264.html?spm=a2g0s.9042311.0.0.P0rutm) (AliExpress - China)
Idler pulley - [with bearing](http://www.ebay.com/itm/6mm-Bore-Smooth-Idler-Pulley-With-Bearing-15-20mm-Width-HTD-5M-3M-8M-Timing-Belt/262637181390?ssPageName=STRK%3AMEBIDX%3AIT&var=561539977995&_trksid=p2057872.m2749.l2649) (ebay - China) Don't know yet if I will manage to fit this on the mount..


**Battery**  
10s4p  - 40 Samsung 30Q 18650s ordered from https://nkon.nl 
[KaeptnBalu's](https://malectrics.eu/product/diy-arduino-battery-spot-welder-prebuilt-kit-v2-2/) spot welder from https://malectrics.eu
10mm wide [nickel strip](https://www.aliexpress.com/item/SuPower-flexible-1m-10-x-0-15T-Pure-Ni-plate-Nickel-26650-battery-welding-strip-tape/32808886861.html?spm=a2g0s.9042311.0.0.P0rutm) (SuPower) and [12mm tinned flat copper braid](http://www.ebay.com/itm/1-10M-12mm-Flat-Tinned-Copper-Braid-Sleeve-Screening-Tubular-Cable-DIY-Z1061-ZY/152374214870?ssPageName=STRK%3AMEBIDX%3AIT&var=451629883269&_trksid=p2057872.m2749.l2649) (ebay - China)
BMS - [SuPower 60A](https://www.aliexpress.com/item/SuPower-10S-36V-37V-42V-60A-Li-ion-Lithium-LiPo-Battery-BMS-Management-System-Balance-PCB/32801166001.html?spm=a2g0s.9042311.0.0.P0rutm) for charge and discharge
Charger - Cheap [2A Laptop-style charger](http://www.ebay.com/itm/42V-2A-Power-Adapter-Charger-For-36V-Li-ion-Lithium-Battery-Two-wheel-Vehicle/332154131763?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649) - probably should have gone with a better one though...

**Motor and electronics**
Waiting for @fottaz to have the [190 kv 6374 sealed and sensored motor](http://eskating.eu/product/electric-skateboard-motor-6374-190kv-sealed-sensored/) re-stocked
Controller - FocBox from @JohnnyMeduse
Remote - GT2B from Fly-Sky via [amazon.co.uk - Trend Mall](https://www.amazon.co.uk/gp/product/B00EDALCWI/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1)
Will probably get a 3D-printed enclosure for the remote; "Sparkle" by @okp - 
  
**Skateboard;**
Deck - [Slipstream DFA 36"x9,4"](http://slipstreamlongboards.com/quiver2015/dfa-2015/) with concave and kicktail
Trucks - Caliber II 50 10" from [Blue-Tomato.com](https://www.blue-tomato.com/sv-SE/products/brand/Caliber-10000020/categories/Skate-00000015--Longboardar-00000018--Longboard+Truckar-0000001H/)
Wedge risers "Slant" 1/2" - 1/4" 
Wheels -[ ABEC11 Flywheels](http://www.hungryhills.de/detail/index/sArticle/21777) 97 mm 75a from HungryHills.de
Bearings - Bones Super Reds + Spacers
```

---
## \#15 Posted by: Sebike Posted at: 2017-07-26T23:43:55.461Z Reads: 182

```
Thanks! I'll probably try to replace the bushings that came with the trucks. I can't get the wheels to bite even at full lean with untightened trucks  on a stand still (standing on two wheels with bottom bushings so compressed that the hanger meets the bottom washer), but there's only a few mm's clearance.. Might be different when in motion though as you mentioned.. :scream: The 1/2" risers allowed a little more clearance than these wedge-risers though.
```

---
## \#16 Posted by: WSB Posted at: 2017-07-27T16:29:19.989Z Reads: 172

```
You can add the Idler to the mount, But you need to drill a extra holl, let me know of you plan to use it and I will make a Sketch for you where to drill.
```

---
## \#17 Posted by: Sebike Posted at: 2017-07-28T22:09:52.251Z Reads: 168

```
Yes, please! That would be great @WSB!
```

---
## \#18 Posted by: darkkevind Posted at: 2017-07-28T22:46:52.069Z Reads: 171

```
@WSB are you selling your mounts again?
```

---
## \#19 Posted by: WSB Posted at: 2017-07-29T06:28:34.311Z Reads: 158

```
Not in stock yet, But in production!
```

---
## \#20 Posted by: WSB Posted at: 2017-07-29T06:30:59.782Z Reads: 159

```
OK, I will fix a sketch when I am home from vacation. Build Looks solid so far 👍🏻
```

---
## \#21 Posted by: Sebike Posted at: 2017-08-01T09:21:23.313Z Reads: 157

```
Things that make you happy.. 
40x30q 
<img src="/uploads/db1493/original/3X/8/f/8f00f16adce61c25b4a919c166360a1a43e103e1.jpeg" width="281" height="500">
```

---
## \#22 Posted by: Sebike Posted at: 2017-08-03T16:50:32.747Z Reads: 148

```
@sl33py Just got the new bushings, SHR from Venom. 97,5a on rear and 93a on front. I weigh around 78-79 kg. What a difference! I now run the trucks pretty loose which allows for great carving, still pretty stable but smooth and quick response from the board. The stock bushings I had to overtighten (until back bushing ripped) cause I was scared of getting wheelbite. Board was not very stable, wobbly and pretty unresponsive. Love it now. Wow! Not even close to getting wheelbite with wedge risers on both trucks. (With stock bushings I could get rear wheel bite if forcing down the board standing on one/two inner wheels with full lean.)<img src="/uploads/db1493/original/3X/1/b/1bc36ee1d558c55fe98bb0d895339fb4309c7ff3.JPG" width="374" height="500"> Thanks for the tip!
```

---
## \#23 Posted by: sl33py Posted at: 2017-08-03T19:59:54.716Z Reads: 143

```
AWESOME!  Glad that helped get you sorted.  

Quality bushings - correct for your weight - they can make a *HUGE* difference - glad that is helping you.

Love the high/super high/ultra etc. rebound bushings.  I also like to run the harder elim bushings board side and then a softer high rebound street side - kind of a dual rebound setup - definitely likes to pull back to center, but can setup super carvy still!

Anyone who has their bushings super tight/squashed should definitely try better quality and higher duro bushings!
```

---
## \#24 Posted by: Sebike Posted at: 2017-08-23T11:18:51.139Z Reads: 134

```
Kaeptnbalu spot welder up and working with my very DIYish welding pen. You like? :smile: Let's weld some batteries! <img src="/uploads/db1493/original/3X/3/8/38fa7d942c7ab63ab67eb2a52bbd7277b143596c.jpeg" width="690" height="388">
```

---
## \#25 Posted by: darkkevind Posted at: 2017-08-23T12:07:33.846Z Reads: 132

```
Although that will work fine.. you really don't need that much insulation. You could cut that block down to make it a bit more manageable to around 10mm surrounding the probes and you'll be absolutely fine. :thumbsup:

<img src="/uploads/db1493/original/3X/3/b/3b45741d696e67f9d2a959142ece89230d5a55bf.jpg" width="500" height="281">
```

---
## \#26 Posted by: Sebike Posted at: 2017-08-23T17:59:54.744Z Reads: 129

```
Thanks for the input @darkkevind, however, the copper rods were insulated already, so the wooden block is only to have them fixed at a good angle so that I would always get the same width on the welds. Also with this size I felt I could apply an even pressure when welding. Maybe it's a bit big, but if works fine :wink:
```

---
## \#27 Posted by: Sebike Posted at: 2017-08-24T11:55:42.980Z Reads: 123

```
Parallels welded with 1 layer of nickel and 1 to go. This is what the 10s4p pack with BMS will look like. Dimensions without series connections are 222x130x32mm. 
<img src="/uploads/db1493/original/3X/8/7/87016e0c92b89bd39b2ea4e1b8f58666f3f49b46.jpeg" width="690" height="388">
```

---
## \#28 Posted by: Sebike Posted at: 2017-09-03T08:49:00.115Z Reads: 109

```
Preliminary mounting and testing! 
I believe battery pack came out pretty slim, considering it being a 10s4p with SuPower 60A BMS; 33x138x225mm.  <img src="/uploads/db1493/original/3X/a/3/a374679c285047f19dda193ebccad7221963b8a8.jpeg" width="281" height="500">
```

---
## \#29 Posted by: Sebike Posted at: 2017-09-05T15:09:01.340Z Reads: 96

```
<img src="/uploads/db1493/original/3X/2/9/29c07faf6965457bc786b7ba4321225ebf45145c.jpeg" width="281" height="500">
```

---
## \#30 Posted by: Sebike Posted at: 2017-09-10T15:59:39.069Z Reads: 86

```
Been riding this board for a couple of days now and I'm in love. Maxed it today at 75% charge to 41km/h - 25.5 mph! What a feeling!! :heart_eyes:
```

---
## \#31 Posted by: surprisebirthday Posted at: 2017-09-11T01:51:51.917Z Reads: 77

```
Congrats on the board!  Love the thought that you put into your build.

How do you like the motor?  I'm thinking about trying a single motor belted drive, coming away from [my dual hub motors](http://www.electric-skateboard.builders/t/globe-maiden-deck-dual-hummie-hub-motors-ollin-vescs-psychotiller-enclosure-paris-trucks-space-cell-10s3p/6932) so that I can ride with more urethane.  I've been eyeing an sk3 192kv, but your sensored motor sounds like it has a lot of potential.  How does it sound and how would you describe how powerful it is?  

Thanks, and congrats again!
```

---
## \#32 Posted by: Sebike Posted at: 2017-09-11T07:25:46.791Z Reads: 73

```
Thanks! This is the first and only esk8 I have ridden, so my board is my reference so to speak. However, to me the ride is really smooth with great torque and plenty of power going up hills. Didn't climb any steeper hills yet, but so far I can accelerate uphill with good power. 

No cogging when taking off from stand still. Runs pretty quiet especially at lower speeds, but even at higher speed it doesn't get loud. Have only run FOCmode with sensors though, so don't know how loud it gets running on BLDC. 

Before riding it outside I tried BLDC sensored and experienced some minor cogging at stand still, but switching to FOC made a huge difference. 

This motor is advertised as sealed, but that means the holes are a bit smaller, so it's not really sealed I guess. 

Doesn't run hot, luke warm at most. So to me it's been great, but so far I've only put 25ish km on it.
```

---
## \#33 Posted by: Sebike Posted at: 2017-09-11T07:37:15.330Z Reads: 67

```
If you're buying that motor from eskating.eu, make sure to get 2 sga8-circlips for the shaft, cause that wasn't included, neither was a key for the keyway.
```

---
## \#34 Posted by: surprisebirthday Posted at: 2017-09-11T16:10:04.795Z Reads: 60

```
Excellent, thanks for the great write-up of the motor and for the tips on the circlips and key.  This sounds like a motor I'll definitely be looking at.
```

---
