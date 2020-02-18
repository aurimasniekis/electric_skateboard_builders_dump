# La Croix Long Range Cruiser Carving Machine

### Replies: 121 Views: 5862

## \#1 Posted by: SkaterBoy58 Posted at: 2018-12-03T23:34:19.583Z Reads: 670

```
My latest DIY build is an extra long-range cruiser based on La Croix deck and enclosure and MBS trucks and wheels. This is part of five of these boards in a group DIY in Perth Australia. 

Basic details and major components of build are:

* La Croix deck and carbon fibre enclosure  [link](https://www.lacroixboards.com/product-page/board-carbon-fiber-enclosure-prototipo) 
* MBS Matrix II Pro Trucks [link](https://www.mbs.com/parts/12202-mbs-matrix-ii-pro-truck-system-1)   with MBS Rock Star hubs  [link](https://www.mbs.com/parts/13241-mbs-rockstar-pro-hub-black-1)  and 200mm Roadie tyres  [link](https://www.mbs.com/parts/13101-8-mbs-roadie-tire-black-1) 
* Flipsky DUAL FSESC 6.6   [link](https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-based-upon-vesc6-with-aluminum-heatsink) 
* Samsung 21700 51E cells [link](http://www.keeppower.com.cn/products_detail.php?id=583%20)    5Ah each in 10S 6P configuration to give 30Ah pack)   5Ah each in 10S 6P configuration to give 30Ah pack
* 2 x Maytech 6374 170KV 65A FLC 3.5kW sensored and with motor temp [link](http://www.maytech.cn/en/mto5065-170-ha-c/10845.html) 
* Custom made Aluminium Motor mounts with cross-struts (from @Idea)
* 72T Aluminium wheel hubs (from @Idea) and 18T motor gear [link](https://www.aliexpress.com/item/POWGE-18-Teeth-5M-Synchronous-Pulley-Bore-5-6-6-35-7-8-10-12mm-Fit/32871278064.html?)   with 20mm belts  [link]( https://www.aliexpress.com/item/5pcs-lot-Neoprene-5M-Timing-belt-180-5M-15-teeth-36-width-15mm-length-180mm-HTD180/32251225632.html?spm=a2g0s.9042311.0.0.66b54c4duXpVQ) 
* Metr Pro module https://metr.at/shopfor telemetry and vesc interfacing (with  antenna due to carbon fibre enclosure)
* Charging circuit designed for 20A but intend to normally charge board at 10A maximum (divided by 6 cells = 1.7A each = 0.34C – so  conservative)  
* External DieBieMS BMS https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639 for charging only (build includes a new external BMS charging box housing the DieBieMS BMS )
* Relay based board main switch (no failing anti-spark switches for me)
* On board headlights powered from main battery pack
* Rear Brake lights triggered from remote PPM signal passing below 50%

Basic design parameters considered were:

**Board Speed** – based on 90% vesc and overall mech/electrical efficiency, 4:1 gear ratio, 200mm wheels, total board mass of 93kg, no head wind and level path, 0.9 sq m frontal area, smooth asphalt path , steady state conditions -- the max speed at 95% duty cycle is as below. The gearing and motor KV was selected to give minimum 40km/hr board speed over all battery voltages.

**Range/Battery Pack** – desire on this build was to maximise range by installing maximum battery Ah in the La Croix enclosure compartments. After a bit of searching – settled on a brand new 21700 cell from Samsung 1NR21700 50E with basic specs -5Ah 10A continuous discharge capacity and 15A intermittent discharge capacity. Decided to go for 60 of these cells in 10S 6P which gives approx. 1,080Wh with 60A continuous discharge capacity.

Based on my current DIY board average consumption on Evolve pneumatics ATs of 13 Wh/km (average over approx. 1,500 km of rides over past 6 months) this gives a calculated range of 83km.

After looking at the La Croix enclosure battery compartments – determined that the compartment width was approx. 240mm - which would fit very nicely 11 x 21700 cells but not 12 (short by about 20mm). But decided to order the 60 Samsung 1NR21700 50E cells and have a play with a few options to see how they could be fitted with a fall-back position to go with 10S 5P or maybe 12S 5P with two parallel packs in rear compartment.

**Motor and motor mounts -** Decided to go with sealed Maytech 6374 motors with @Idea mount V7.3 with cross struts but without idlers. My current board (with 175mm AT tyres) has a pair of Racestar 5065 200 KV motors rated at 1,650 W with a pair of FocBoxes and this has plenty of power and acceleration torque – so the Maytechs 3.5kW motors are a bit of an overkill – but they should run very cool and efficiently.

All the major material and equipment was ordered during Nov 2018 including the lots of misc. stuff for building boards such as nickel strip (10mm x 0.15mm), 12 awg silicon wire, 14 awg silicon wire, 22 awg silicon wire, pack heat shrink, fish paper insulation, neoprene foam sheet, bullet connectors, switches, charge sockets, headlights, etc.

Boards rocked up from Canada last week - thanks Alex 
![la%20croix%20boards|666x500](upload://hAnAhTImAql8H9hZMkALGLfMBGf.jpeg)   

and cells rocked up from nkon and motors from Maytech ( about 4 week delivery for both)  


![cells%20and%20motors|666x500](upload://rIxQqktFcBmnormrG8qqa5dxUJs.jpeg) 

 so now the build starts :grinning:
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-12-03T23:44:46.561Z Reads: 567

```
@moone i think it's time for you to make some new friends
```

---
## \#3 Posted by: moone Posted at: 2018-12-03T23:49:50.692Z Reads: 562

```
These are the boys I skate with @mynamesmatt. They got scared of the evo build so they thought they better pick up their game. 

Isn't that right Roger 😂😂
```

---
## \#4 Posted by: venom121212 Posted at: 2018-12-04T00:02:46.439Z Reads: 542

```
Loving every bit of this build. Keep up the good work.
```

---
## \#5 Posted by: MattyG Posted at: 2018-12-04T00:03:23.598Z Reads: 541

```
Haha @moone catch us if you can 😉
```

---
## \#6 Posted by: SkaterBoy58 Posted at: 2018-12-04T00:23:09.651Z Reads: 555

```
So first thing is to sort out battery cell configuration 

After cells and enclosures arrived - first mock up was 
![initial%20moick%20up|666x500](upload://2DcVd5HaXH1phaI774VEObbUcn.jpeg) 

on closer inspection the raised cell was sitting just proud on the enclosure lip - so then the idea was hatched to raise two outer cells to reduce the height .
something like 
![2018-10-24_7-52-32|300x195](upload://p3TMNmny82e0UV0fX9zjvo5LuGY.jpeg) 

@Brucey0 ( one of the gang of 5 and a master craftsman) then build a wooden jig to enable pack hot gluing with cells in correct position 
![battery%20jig%20bare|373x280](upload://v3Q4R46waVxtQguctiApuHqDzQl.jpeg) 
(a patent has been applied for this jig)  

What a pack looks like in the jig
![battery%20jig%20no%201%20|373x280](upload://wY8GUE5f5NF2ytkLEJwNrlpJCVx.jpeg) 

and what the packs look like in the enclosure
![pack%20%202%20raised%20|373x280](upload://fxz4fnQPHpzf056TmlLqjlg8nsN.jpeg) 

Then hot glued two trial packs complete with heat shrink and trial fitted in all four compartments using this configuration - and looked at the deck underside clearance to top of packs. 
 No 2 (from front) and No 5 are the closest due the decks 3D concaveness . A bit more group discussion was had and @MattyG was tasked with some mod to gain a 1-2 more mm clearance- details to follow

The very front compartment will need a different configuration due to lack of enclosure depth - so plan is to run 11 cells ( 1x 6P pack and 1x 5P pack) across the enclosure with one loose cell to make up the 6P on front face
```

---
## \#7 Posted by: venom121212 Posted at: 2018-12-04T00:40:04.808Z Reads: 515

```
Have you tried a silicone gasket? Waterproofed, black, and adds a bit of enclosure height.
```

---
## \#8 Posted by: SkaterBoy58 Posted at: 2018-12-04T00:42:19.055Z Reads: 512

```
looking at a foam/neoprene/soft rubber strip around enclosure lip (to replace one that comes with deck) - want it look mint from outside the enclosure
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2018-12-04T05:31:28.654Z Reads: 506

```
@SkaterBoy58 nice project you have, but I'm not really sure the enclosure will allow a double stack of battery, as @pat_arch  already explain the deck s a concave and is not completely straight, maybe you should check with @Arch before starting to build your battery, if you don't want to end up having to rebuild it again at some point. 

https://www.electric-skateboard.builders/t/lacroix-board-co-wood-and-cf-deck-segmented-flex-carbon-fiber-enclosure-group-buy-completed/49051/63?u=johnnymeduse
```

---
## \#10 Posted by: Arch Posted at: 2018-12-04T15:34:47.529Z Reads: 473

```
Yeah, agreed. The double stack might work for the cell on the extremity, but the double stack near the center of the board will likely not work.
```

---
## \#11 Posted by: briman05 Posted at: 2018-12-04T16:07:43.062Z Reads: 456

```
You may want to change out the baseplate on the matrix trucks as some people have had them snap because they are made out of nylong i think etorxx made some metal baseplates for them that would be a much better upgrade.
```

---
## \#12 Posted by: legend27 Posted at: 2018-12-04T19:23:57.690Z Reads: 444

```
Really cool build!
```

---
## \#13 Posted by: SkaterBoy58 Posted at: 2018-12-04T23:47:57.076Z Reads: 452

```
@JohnnyMeduse @Arch    Thanks for your comments

yeah It is not a double stack of cells per se the whole width - just two cells slightly raised closest to lip of enclosure to fit 2 packs of 6P in the 240mm compartment width 

The jig sets all 6P packs to be identical with 119mm width for the 6P pack .

This only works in compartments 2 - 5  ,  the front compartment will be different and will contain a 5P flat pack , a flat 6P flat pack and one loose cell connected to the flat 5P pack.

This is not a build that inexperienced people can copy as the cell configuration is being pushed to the limit a bit and inter-pack insulation is a big consideration - but  with the reward being the additional Ah offered by the 60  x 21700 cells.   

Will post a close up photo of two completed 6P packs in the enclosure over next few days 

Cheers
```

---
## \#14 Posted by: Pedrodemio Posted at: 2018-12-05T00:13:59.048Z Reads: 416

```
Nice build, really looking forward to how these cell handle, at last some high capacity and acceptable discharge cells are available to buy
```

---
## \#15 Posted by: maxbicyclemax Posted at: 2018-12-05T02:55:54.988Z Reads: 414

```
Following... and part of the RAMMMs squad👌
```

---
## \#16 Posted by: SkaterBoy58 Posted at: 2018-12-05T07:23:05.189Z Reads: 452

```
A bit of battery pack stuff
**Nickel Strip**  Using 2 x 10mm wide x 0.2mm thick pure nickel strips for the 6P packs .  Had to order from an Aussie supplier after the Chinese eBay seller send 8mm x 0.15mm in lieu of ordered 10mm x 0.15mm strip.

Using my just developed nickel strip resistivity calculator ( [SkaterBoy58 nickel strip purity calculator link](https://www.electric-skateboard.builders/t/nickel-strip-purity-checker-excel-calculator/76860) )  I checked both the Chinese eBay seller nickel strip and the aussie 10mm x 0.2mm - both checked out as pure nickel so all good - results of 5A test below

![nickel%20strip%20test|690x450](upload://84YJJGH4VqTtcCtdtjvL7BSCKJH.jpeg) 

**Pack Series Connections**   - using 2 x 12awg silicon flexible soldered onto top nickel strip

First task was to cut up nickel strip with 2 x +ve strips and 2 x -ve strips per pack. 
+ve strips have a radius end to avoid contact with cell shell with -ve strips just a square cut end. 

RAMMMs Group member @maxbicyclemax portrayed a hidden skill in neatly cutting up nickel strips

![nickel%20strips|682x500](upload://wSxwiCbEKpvCELYBgCUtc3qfJkK.jpeg) 

 plan is to spot weld first nickel strip to cells - then put solder blobs on second strip - then spot weld second strip to first strip leaving solder blobs for series 12 awg soldered connections .


![nickel%20strip%20plan|522x233](upload://ipC8XqREkTSbmtXOiuYxT5BprAb.jpeg) 

this is a 6P pack hot glued in precise position in the jig , then wrapped end on end with 20m wide Kapton tape , then with outer heat shrink applied . these packs are exactly 119mm wide for 2 to fit in the 240mm wide enclosure compartment with 2 pieces of fish paper cardboard between the two packs. 

![6P%20Pack%20with%20heatshrink|690x388](upload://ovBHg96lhWCNz582uXCRLzyWyHx.jpeg) 


@maxbicyclemax is going for a 10S 5P configuration - so all of his packs can be flat (and much simpler)

![5%20pack%20flat|666x500](upload://jTOCemAdhOOYo07xfRfDsrMIXuW.jpeg)  

Next task is to finish heat shrinking all 24 x 6P packs and 10 x 5P flat packs  , complete spot welding of both nickel strips layers and prepare packs for installation in enclosures
```

---
## \#17 Posted by: dareno Posted at: 2018-12-05T23:39:23.160Z Reads: 417

```
I get seriously jelly everytime I see someone building with the lacroix deck and enclosure.  Absolute work of art.  Going to follow this build with avid interest.  Awesome stuff.  Hopefully one of you guys will do a thane version a la @Sender
@moone  then the evo might be under threat mate.
```

---
## \#18 Posted by: moone Posted at: 2018-12-05T23:52:12.355Z Reads: 412

```
It might be @dareno, but only because @SkaterBoy58 is the master. 

But then again it's an evo 😍❤
```

---
## \#19 Posted by: dareno Posted at: 2018-12-06T00:15:02.729Z Reads: 411

```
I love the lacroix but never would I take a set of mbs trucks where I would the rkp's.
```

---
## \#20 Posted by: SkaterBoy58 Posted at: 2018-12-11T23:32:58.916Z Reads: 421

```
Bit of an update - motor mounts have arrived from @Idea  - very impressive machining 

![%20Mounts%20-%20opened|497x280](upload://9BNnXl89ev1MODWLSeNCeLbrn4E.jpeg) ![%20gear%20thickness|280x497](upload://qvK9kPzLKcoTLsd5dgSQHBDJyBK.jpeg) ![%20motor%20mount%20thickness|280x497](upload://9ts7uLyBQLTkasqjM71iSsU3MEC.jpeg)  
![%20mounts%20close%20up|497x280](upload://Ab50SXjAIh5IM6Kxh0qJuVZNpce.jpeg) 

motor mounts are 10mm thick for the whole length - so super strong

Next was a trial fit of the mounts on the mbs trucks - needed to slightly file out the motor mount plate aperture that fits over the mbs truck - the mbs truck axle is a weird pattern - part circle part straight edge - but eventually it fitted fine.

The Maytech 6374 motors are very beefy compared to the 5065s I run on current DIY board.

Went with 20mm belts to match the 3.6kW available from each motor! 

It all fitted OK with a loose mock up .including cross-strut

![%20mock%20up%20wheel%20close%20up|666x500](upload://nJYBtBliyBaKmVU3oCBqUekKxAv.jpeg) ![%20rear%20showing%20strut|666x500](upload://tBbAlSEPukQG88U31mkwtphn8RS.jpeg) ![%20rear%20mock%20up%20|666x500](upload://2hYyMGm4FqaRaWhkAVEqQSU0cvG.jpeg)
```

---
## \#21 Posted by: venom121212 Posted at: 2018-12-12T00:40:50.372Z Reads: 392

```
Are many people using RKPs on a mountainboard build?

@SkaterBoy58 are you considering using a wedge? Not sure of the nose angle on the deck but MBS matrix trucks claim they want 30°
```

---
## \#22 Posted by: SkaterBoy58 Posted at: 2018-12-12T00:56:16.233Z Reads: 374

```
The La Croix deck is designed for MBS trucks
```

---
## \#23 Posted by: venom121212 Posted at: 2018-12-12T00:57:19.579Z Reads: 376

```
Oh right on, I never saw that mentioned. Thanks
```

---
## \#24 Posted by: dareno Posted at: 2018-12-12T06:58:34.901Z Reads: 364

```
@sender has rkps and a lacroix

Did i already say that?  I'm tired.  Leave me alone.
```

---
## \#25 Posted by: venom121212 Posted at: 2018-12-12T12:50:24.539Z Reads: 357

```
Shit right after I told him I didn't like the design of the Lacroix hotdog deck... Time to eat some words I guess
```

---
## \#26 Posted by: mutantbass Posted at: 2018-12-12T13:37:11.898Z Reads: 355

```
Any reason you didnt get the mount with idlers?
```

---
## \#27 Posted by: SkaterBoy58 Posted at: 2018-12-12T23:24:50.529Z Reads: 354

```
they couldn't  fit on these V7.3 mounts with 72T wheel hub
```

---
## \#28 Posted by: SkaterBoy58 Posted at: 2018-12-12T23:57:06.098Z Reads: 365

```
See this thread for external BMS and Charging box build details.

[External BMS and charging-box](https://www.electric-skateboard.builders/t/external-bms-and-charging-box/79444)
```

---
## \#29 Posted by: banjaxxed Posted at: 2018-12-16T07:40:50.858Z Reads: 362

```
I use those connectors for standard charging they are nice quality and waterproof too, I like your thinking
```

---
## \#30 Posted by: SkaterBoy58 Posted at: 2018-12-17T23:45:06.669Z Reads: 383

```
**battery pack building continued** 
first 10mm x 0.2mm nickel strip is spot welded directly to cells

![5%20pack%20|375x500](upload://z22QcXaN4auCQyUTDjQxaMDf9xD.jpeg) 

second paralleling nickel strip has series connection solder blobs completed prior to spot welding to first nickel strip. Solder blobs are positioned for best current sharing position and not directly on top of a cell with a third small solder blob for balance lead connection.

![solder%20blobs|375x500](upload://dbd84vDErje6QS0k86RHdetpAS6.jpeg) 

then directly solder two series connections to each pack quickly with a hot iron ( at least 100W) . Laid out battery configuration with a few labels to avoid stuff-ups

![IMG_4104|375x500](upload://qQALMcU2JTtexsoRsZatgbx9Nd7.jpeg) 

The sides of each enclosure compartment have fish paper to avoid any issues with pack connections conducting through the carbon fibre.  Each compartment has 2mm neoprene rubber on bottom for shock absorbance ( and another insulation medium)  . 
The two 6 pack cells in a single compartment will have fish paper wedged between them ( another insulation medium ) 
![pack%20compartment|375x500](upload://yrbYXouiC7mp5VjEIdk33fdmfEF.jpeg) 
![IMG_4107|666x500](upload://fDbpXFxRCYUn0JrmaRodsSO95lZ.jpeg) 

the complete LHS of battery pack completed and in enclosure

![lhs%20complete|375x500](upload://63OC8CaOUUwYxKLRg7hd8OtGW9x.jpeg) 

with the RHS under construction on a timber board
![rhs%20under%20cons|375x500](upload://cy6KJMGvKR2K0tkG2dy5xJWWsuI.jpeg) 

with a bit of Kapton tape covering all exposed nickel strip  and series connections for good measure. 

The very front compartment has both a 6P and 5P flat packs due to much reduced clearance from deck. The additional cell for the 5P pack will sit in front of both packs with separate connection to the 5P pack.

The 11 balance wires will run down the centre of the enclosure in a loom to the back enclosure.
```

---
## \#31 Posted by: SkaterBoy58 Posted at: 2018-12-18T04:50:28.669Z Reads: 370

```
**Rear Compartment planning**
rear compartment will contain Flipsky DUAL FSESC 6.6, all external sockets/switches , remote receiver and misc other small stuff.

Plan is to mount the Flipsky DUAL FSESC 6.6 on a thin aluminium plate ![main%20view%20|667x499](upload://gueSFIvwdt2jR46s2iUURAYLYcx.jpeg) 

with the sockets/switches on both sides. Will have 2 pin weatherproof charging sockets on both sides  [sd13 2 pin weatherproof socket](https://www.aliexpress.com/item/SD13-2pin-Male-and-female-connector-Outdoor-waterproof-connector-panel-mount-13mm-2-pin-plug-and/32672034511.html?spm=a2g0s.9042311.0.0.27424c4dbduUOf)

so will need 12 pin socket , main XT-60 isolation plug, on/off switch , two charging sockets and a receiver binding switch ( to enable binding to a different remote without the hassle of opening enclosure) 
![lhs%20|666x500](upload://gOYjslevAYpb5JhHKhwXceOUJiB.jpeg) ![rhs%20|666x500](upload://f5ONapjxhm0rbNkYZ8dldQVKXyr.jpeg) 

One of the builders in the gang built some thin aluminium plates (to stick on inside of enclosure) to mount everything on. This will relieve the very thin carbon fibre enclosure of any stresses  when unplugging any plugs from sockets. 
![al%20plate%201%20|666x500](upload://gZ9z6FmUgnsn986aOL6WjPcrSaT.jpeg) ![al%20plate%202%20|666x500](upload://64PfCu6ShUB8jzoQnM8zgEZcZLR.jpeg) ![al%20plate%204%20|666x500](upload://ad01flwflAT0m1dtcKPqigUhH8U.jpeg) ![al%20plate%205|666x500](upload://1UKJFa3A7YdYBSOCf77g909D1hC.jpeg)
```

---
## \#32 Posted by: SkaterBoy58 Posted at: 2018-12-20T01:49:03.719Z Reads: 365

```
Next bit of building is to fix neoprene rubber strips to the edge of the enclosure to provide clearance from bottom of deck to top of battery packs.

After a bit of group measuring, eye-balling and plasticine compression checking when battery packs placed in enclosure and deck fitted on top – settled on 4.5mm thick neoprene rubber strip 25mm wide.  [Link to Neoprene Strip](https://www.ebay.com.au/itm/Neoprene-Rubber-Sealing-Strip-4-5mm-3-16-Thick-x-25mm-Wide-x-10-Metres-Long/122945809008?_trkparms=pageci%3A33605d4a-03e8-11e9-b098-74dbd180dabc%7Cparentrq%3Ac8dc5c721670aade2a9d62fafffb585e%7Ciid%3A1&_trksid=p2481888.c100675.m4236&fbclid=IwAR3fVQnsx_PoqTu0vVfIX9-Ybs14PEyVSfeVbhxouSbjAAKmay1b19sF-IE)

The neoprene rubber strip has the right hardness characteristic (won’t compress much), good sealing performance to keep out dust and has good UV resistance. 

The foam rubber sealing strip that comes on the deck will sit nicely on the neoprene strip.

A strip template was made to get the curvature horizontal cut-outs right, enclosure holes marked and then punched.![strips%20with%20cut-out%202%20|666x500](upload://8hGFaMl55Ybk4Wnf9IyDJImROHD.jpeg) ![strips%20with%20cutout%201%20|375x500](upload://s3wJkmuxSyt0egt2IXgUmkV8yKz.jpeg) ![strips%20with%20cutout%20and%20enclosure%202%20|666x500](upload://lwFm7zYEjPcH3Oj8xMzSdiQHnkM.jpeg) 

Bolts were then placed through enclosure holes and up to strip to hold it in exact right position for gluing.

After a full trial fit – rubber strips were then glued on and clamped for glue setting (approx. 24 hours). Pegs and small clamps were the go to hold rubber strip down to enclosure between bolts.
![strips%20being%20applied%201%20|690x388](upload://kF5SGX1QjU4Qg8q1R5l6sslKr1n.jpeg) ![clamping%20strips%20|666x500](upload://wE7wb9qf7EjJdzn6DpRlZ9xjhTk.jpeg) 

Rinse and repeat for all three enclosures!

![rinse%20and%20repeat%20x%203%20|666x500](upload://8AeU053W1IRIDgreOCeRkZOXyq2.jpeg)
```

---
## \#33 Posted by: dareno Posted at: 2018-12-20T02:32:22.094Z Reads: 345

```
@moone was right you are the man!  Love the remote cabling ideas so much I will probably steal them.  Great build  Can't wait to see the finished article.
```

---
## \#34 Posted by: maxbicyclemax Posted at: 2018-12-22T23:58:06.419Z Reads: 333

```
What are you taking between cell 6 & 7?
Auxiliary 12V supply?
```

---
## \#35 Posted by: SkaterBoy58 Posted at: 2018-12-23T00:21:47.763Z Reads: 329

```
Max -If you want a LV supply for lights etc 
better off using a BEC step down converter with 42V input after you loop key

[Hobbyking BEC](https://hobbyking.com/en_us/yep-20a-hv-2-12s-sbec-w-selectable-voltage-output.html?___store=en_us)
```

---
## \#36 Posted by: SkaterBoy58 Posted at: 2018-12-23T00:22:44.108Z Reads: 322

```
The wire on cell 6 is for the loose one cell paralell connection
```

---
## \#37 Posted by: Arch Posted at: 2018-12-24T18:31:06.024Z Reads: 315

```
Great work guys. You Aussies are legit!
```

---
## \#38 Posted by: SkaterBoy58 Posted at: 2018-12-30T03:07:40.600Z Reads: 334

```
**now for rear compartment stuff update -**
aluminium plates were made for mounting the flipsky dual 6 vesc  to bottom of enclosure 

 @Brucey0 (master craftsman) build some aluminium clamping brackets to fix flipsky dual 6 vesc to bottom aluminium plate . 
basically the rear and front small plates clamps onto the vesc heatsink and holds it in firmly place - very nice - 

![vesc%20plate%20in%20enclosure|666x500](upload://zKivA2kHUYm1aLalP9Cw2VmmdXs.jpeg) 

![tray|666x500](upload://nWfpWdrq5E76PttokLYqzbTzZF9.jpeg) 

![vesc%20mounted|666x500](upload://zGFHVuwW7jL89rUI2uk1v5o1zr9.jpeg)

first job is to stick vesc aluminium plate to bottom on enclosure 

![glueing%20vesc%20plate|666x500](upload://xMmwVDcNtIsm3T5bE2cpgOsps9J.jpeg) 

then stick aluminium plate to enclosure bottom - many hands are better 

![glueing%20vesc%20plate%20in%20enclosure|666x500](upload://g4EATydvInzqJ2IcudKlAMLd5VG.jpeg) 

then stick side aluminium plates to insides of enclosure and clamp in place for glue to set

![clamp%20and%20glue|666x500](upload://o6c3P1qgRRtDxk6QLICgmrFIBCh.jpeg) 

rinse and repeat for all three enclosures

![all%20three%20glued|666x500](upload://lPhc3LGpuF8R6zNjTDJLmk50LRB.jpeg) 

several days later after glue had set - time to make holes in side of carbon fibre enclosures - with a small pilot hole , then using glass and tile bit - drill larger hole - then finally made to size with a circular grinding paper bit on a dremel

![%20clamps%20removed|666x500](upload://gaNmNGtNlZGb81ICMgP3RGrfWM1.jpeg) 

![%20second%20side%20clamps%20removed|666x500](upload://89DuvHIJ2Trtxbuj6ARjJWLdyNH.jpeg) 

![%20holes%20all%20done|500x500](upload://lABrL6HHMoLDAE6I6dxZN7KrSJp.jpeg) 

 
![3A|500x500](upload://dlqDM6PygtMvLhZUDTIMI5zNAKL.jpeg) 

then fit the stuff in the holes - and ready for final wire up

![%20all%20fitted%202%20second%20side%20fitted|666x500](upload://blWD2XASG1vfgk0IAtcLpbCWsRB.jpeg) 

![%20all%20fitted%201|500x500](upload://zRfoPnaxLLlA0kEzo6hnBSbeIXO.jpeg) 

the XT-60 socket will be used as an isolation point on main +ve  from battery 

There are charging sockets on both sides of enclosure ( for versatility, redundancy and to power an external dc-dc converter for charging another board from battery pack)
```

---
## \#39 Posted by: Riako Posted at: 2018-12-30T09:58:05.832Z Reads: 305

```
A true source of inspiration! I love your attention to detail :sparkles::ok_hand:
quickly, the following :relaxed:
```

---
## \#40 Posted by: banjaxxed Posted at: 2018-12-30T16:23:09.224Z Reads: 299

```
Agreed this is all very masterful, detailed, well written and beautifully shot, you’re in with a shot for BOTY 2018/2019
```

---
## \#41 Posted by: billappleton Posted at: 2018-12-30T21:11:01.371Z Reads: 286

```
i like the external BMS. thought about building my own charger like this build has. its hard to find external chargers that are 10 to 12s. lots of people do two 6s banks for charging.
```

---
## \#42 Posted by: Toughook Posted at: 2018-12-30T22:08:20.690Z Reads: 286

```
Really loving this thread. Nothing to add, just watching and learning 👍
```

---
## \#43 Posted by: janpom Posted at: 2018-12-30T22:30:23.932Z Reads: 292

```
This is great. I want to do something very similar for my board. I also already installed the same 12pin connector.

Why the DieBieMS? That seems like overkill, especially since you already have a solution for monitoring individual cell voltages and even for manually balancing with the bleed resistors. That alone is already good enough. Overcharge alarm can be configured on BS12, so you would be notified that you should disconnect the charger. Seems like you need no BMS at all. If you do want extra protection, any cheap bypassed BMS would do.
```

---
## \#44 Posted by: Indiangummy Posted at: 2018-12-30T22:34:36.419Z Reads: 280

```
@JLabs has 10s charges if you need. Also @barajabali has some aswell I think
```

---
## \#45 Posted by: Indiangummy Posted at: 2018-12-30T22:37:28.371Z Reads: 282

```
@dareno is this the one you ment? About bms integrated charger? 

@SkaterBoy58 I think you should start a separate theard on this charge once you get more into it. Abosolutly love the idea.
```

---
## \#46 Posted by: dareno Posted at: 2018-12-30T22:39:21.007Z Reads: 272

```
Thats the one.  Looks like a cracking idea.
```

---
## \#47 Posted by: SkaterBoy58 Posted at: 2018-12-31T03:26:33.457Z Reads: 286

```
OK  
Will start a new thread for my external BMS/Charger see [https://www.electric-skateboard.builders/t/external-bms-and-charging-box/79444](https://www.electric-skateboard.builders/t/external-bms-and-charging-box/79444)
Cheers
```

---
## \#48 Posted by: SkaterBoy58 Posted at: 2018-12-31T23:55:19.167Z Reads: 296

```
neoprene foam hot glued to bottom of compartments for battery cells to sit on 
and fish-paper cardboard hot glued to sides of compartments for insulation - with the middle strips to fit between cell packs

![foam%20and%20fishpaper%20stuck|666x500](upload://pQDNIkdvD9dg9Mz5ncD9NE5x5lo.jpeg) 

![enclosure|375x500](upload://dQluuBcoM0UjzDVeikBaa1Qu34K.jpeg)
```

---
## \#49 Posted by: SkaterBoy58 Posted at: 2019-01-09T11:47:27.843Z Reads: 285

```
Completed building battery pack with all series connections and balance wires connected to enclosure socket. 

Charged battery to 4.15V per pack using DieBieMS BMS (with cell misbalance set to 5mV) and CC set to 0.5A for final charge above 41.0V. Total battery voltage was 41.5V

Next step is to complete a battery discharge to confirm battery Ah and Wh capacity and to confirm that all cell packs discharge uniformly.  

 The load for this test is my trusty old 8-ohm 100W wire wound resistor mounted on a fan that I have used for discharge testing of previous battery builds. This provides approx. 4A current. 

![62B88702-3768-48F3-95C5-77292EF8AE96|666x500](upload://bAlCuNYn1bVAz0nux8ae4ilrYrV.jpeg) 

The Samsung 50E 217000 cells are advertised as 4,900 mAh minimum with nominal capacity of 5,000 mAh. These stated mAh capacities are for full discharge from 4.2V to 2.5V.  

I have 10 x 6P packs of these cells so am expecting approx. 27Ah battery capacity for this discharge test from 41.5V and stopping at 3V with a Wh capacity of approx. 975 Wh.

The discharge test should take about 7 hours.

 Measurements of discharge current and all cell pack voltages (using real-time data on DieBieMS Tool) were taken every 15 minutes for the first hour and then every 30 minutes after that.

The Ah was calculated over every time interval using the average current over the interval multiplied by the minutes – and then accumulated for duration of discharge test.

The Wh was calculated over every time interval by multiplying the time interval average current by the time interval average voltage (sum of all 10 cell pack voltages) multiplied by the minutes – and then accumulated for duration of discharge test. 

Discharge test completed on 9 Jan with headline results of:

•	Battery Voltage at start of discharge test   41.5 V
•	Battery Voltage at end of discharge test    29.9V
•	Total discharge test time  420 minutes    (7 hours)
•	Total discharge test Ah   28.5
•	Total discharge test Wh 1,051
•	Cell misbalance at start of discharge test   7 mV
•	Cell misbalance at end of discharge test  49 mV

Put discharge data into excel workbook for some graphs.

![Discharge%20Test%20No%201|690x416](upload://6rgkZ3Od1wRtN3dUuXHZMAFryuW.jpeg) 



![Discharge%20Test%20No%202|690x435](upload://jwXOsrOVrzHWITeXc33Kr5oa3pF.jpeg) 

Initial impressions are that these Samsung 21700 50Es are very good cells. 

Next is to do some real-life range testing!
```

---
## \#50 Posted by: maxbicyclemax Posted at: 2019-01-11T05:37:09.527Z Reads: 257

```
Certainly shows why the default low V soft shutdown voltage on vesc tool is 34V for 10s
What voltages are you planning on setting your soft and total shutdown???
```

---
## \#51 Posted by: SkaterBoy58 Posted at: 2019-01-15T00:08:04.213Z Reads: 271

```
Battery and vesc wiring all complete - powered up board and Dual FSESC6 unit with no magic smoke so all good.

Flipsky Dual FSESC6  connected to VESC tool 0.95 with no issues
(units came with FW 3.40 pre-installed)

Ran motor detection OK and set-up normal master/slave canbus settings (with unit can-bus switch set to off for set-up) 
  
FSESC6 settings as below
![vesc%20config%2014%20Jan|299x500](upload://eu9Q0cUKSbqNvEwxjayOrLAnoKL.jpeg) 

 with throttle curve like this
![Throttle%20curve|690x415](upload://dkqWf0xObBbJyzsEI4ZYFx7GeY3.png) 

with first test ride up and down local street 

Still a bit to tidy up inside board for auxiliary stuff such as headlights , brake light etc but for now it is ridable with range test ride planned next weekend.
```

---
## \#52 Posted by: lrdesigns Posted at: 2019-01-15T00:53:18.348Z Reads: 250

```
How did you make that fancy excel with all the settings?
```

---
## \#53 Posted by: SkaterBoy58 Posted at: 2019-01-15T01:37:53.535Z Reads: 255

```
its called a keyboard!
```

---
## \#54 Posted by: lrdesigns Posted at: 2019-01-15T01:43:30.116Z Reads: 248

```
lol, surely there is a way to automate the process as it saves as xml? 

Its quite nice to have though, like a setup sheet for motor racing. Maybe add bushing and truck angles.
```

---
## \#55 Posted by: SkaterBoy58 Posted at: 2019-01-15T01:44:51.339Z Reads: 240

```
yeah - you can save config motor and app settings as xml file from vesc tool
```

---
## \#56 Posted by: lrdesigns Posted at: 2019-01-15T01:51:53.401Z Reads: 242

```
No I mean like automatically convert the raw xml into a pretty excel that is easy to read/print. With some sort of copy and paste into a premade format. Im no excel pro though.   Sorry to clog up your thread with stuff about excel. :sweat_smile:
```

---
## \#57 Posted by: sleekjazz Posted at: 2019-01-15T09:52:57.591Z Reads: 241

```
Woot - Board is ready to Roll!!!
```

---
## \#58 Posted by: Riako Posted at: 2019-01-15T20:25:20.744Z Reads: 250

```
Yes ! Make photos and videos ;P :+1: 

[quote="SkaterBoy58, post:53, topic:76960, full:true"]
its called a keyboard!
[/quote]
@lrdesigns, what is probably trying to tell you [SkaterBoy58](https://www.electric-skateboard.builders/u/SkaterBoy58) , it's maybe that he tap it itself C/P info from the xml vesc file to make a pretty tabler ...?..

Good ride :v:
```

---
## \#59 Posted by: SkaterBoy58 Posted at: 2019-01-16T00:06:35.862Z Reads: 253

```
Basic schematic diagram of board electrics  - happy to answers any queries 

![Board%20Schematic%20Diagram%20c|690x487](upload://egclm0LE5U2AGU9VhyHzZHh3ah0.jpeg)
```

---
## \#60 Posted by: AlexBE Posted at: 2019-01-16T05:29:09.263Z Reads: 245

```
Very interesting to see a different approach to charging/power switch. Do you use two charging sockets to do very fast charge? You have a charger that can max that out and what current ends up going into each cell at max charge rate?
```

---
## \#61 Posted by: SkaterBoy58 Posted at: 2019-01-16T05:49:40.159Z Reads: 241

```
Two charging ports ( each with its own 20A fuse ) on each side of board because

1. You can charge La Croix board batteries with two separate chargers ( but a rare instance) with no technical worries

2. Convenience to charge on either side of board either on ground or vertically hanging up

3. Redundancy if charge fuse blows due to fault outside of board on one charging port (opening enclosure to replace fuse is a pain)

4. Ability to charge two other ( lower battery capacity) boards on group rides with external DC/DC Converters ( mother ship approach)


The Samsung 21700 50Es have a nominal charge of 0.5C (2.5A) so for 6P = 15A and a max. charge rate of 1C which is 30A for the 6P packs. 

But I only intend to charge up to 10A (depending on when the next ride is)  with a normal charge of 5A but I can charge up to 20A using two of my chargers - one through each charging port - if required.
```

---
## \#62 Posted by: AlexBE Posted at: 2019-01-16T06:15:16.985Z Reads: 231

```
Ahh interesting mothership approach. I've always considered mothershippin' by towing the low capacity boards and have them brake. I would expect pretty much any board/chargers to be able to handle multiple chargers connected at the same time.
```

---
## \#63 Posted by: SkaterBoy58 Posted at: 2019-01-16T07:12:49.013Z Reads: 228

```
yeah - just use one (or two) of these - plug input in your board charging socket and charge other boards with unit output set to 42V ( 10S) and up to 5A CC setting. They are also all over Ebay 

[DC DC CVCC Boost Module](https://www.aliexpress.com/item/900W-Digital-Control-DC-DC-Boost-Module-0-15A-IN-8-60V-OUT-10-120V-Step/32842450108.html?tt=sns_none&fbclid=IwAR1V6qoyaDJVWOuovaoE-k-sk-1R2Z7g3VDNN7OLhYZ8EzNqlvvtJ6mrDwc&aff_platform=default&cpt=1547622481174&sk=zbwKGRA&aff_trace_key=4a10c61d39c844cdb082cc67a1f8d8d3-1547622481174-03320-zbwKGRA&terminal_id=e1df75e020d1422a8f785c90cb5580d2)
```

---
## \#64 Posted by: janpom Posted at: 2019-01-16T08:10:17.038Z Reads: 228

```
Nice diagram! Can you please share what do you use as the 1A fuses on the balance leads? I plan to add some on my build as well.
```

---
## \#65 Posted by: SkaterBoy58 Posted at: 2019-01-16T09:00:53.980Z Reads: 249

```
from RS Components - just solder em in balance wires near battery with two layers of heat shrink ( you hope they will never need to be replaced)

[link Wire Fuses from RS](https://au.rs-online.com/web/p/non-resettable-wire-ended-fuses/5413265/)

close up ![IMG_4396|666x500](upload://lgsWd2yxQC9pXF7OVcYtGUPgOvN.jpeg) 

![IMG_4397|666x500](upload://eKZT9vPAcdj1WB3PALfwYbOVTp9.jpeg)
```

---
## \#66 Posted by: SkaterBoy58 Posted at: 2019-01-16T23:37:25.608Z Reads: 252

```
A few more photos of one of the boards in the group build - this one has a Flipsky anti-spark switch with XT-90s plug and play concept 
. The electrics are complete in enclosure and it ready to bolt to deck 
![92053356-A123-4DDC-BCC4-91077C33DB32|375x500](upload://9GScEi31CiBhcaoZBJvAUKbzHbO.jpeg) 

![IMG_4397|666x500](upload://eKZT9vPAcdj1WB3PALfwYbOVTp9.jpeg) 

![mark%20esc|500x500](upload://y5uGZAqZaTeWfc0fnVQ6aUTYw6O.jpeg)
```

---
## \#67 Posted by: SkaterBoy58 Posted at: 2019-01-16T23:48:47.136Z Reads: 245

```
One of the main concerns in trying to fit 10S6P  60 21700 cells in the enclosure was deck clearance to the top of the highest point in the packs - particularly in compartments no 2 and 5 ( from front) 

![IMG_4107|666x500](upload://fDbpXFxRCYUn0JrmaRodsSO95lZ.jpeg) 

This is the reason why we went with the 4.5 thick rubber strips fixed to the enclosure lip to provide more clearance. This rubber strip also provides very good sealing to inside of enclosure.

![%20clamps%20removed|666x500](upload://gaNmNGtNlZGb81ICMgP3RGrfWM1.jpeg) 

Did a trial fit of enclosure on deck with 20mm high plasticine blobs on cell pack high points with the objective to see how far the blobs compress down to when the deck is bolted on . This test gave approx. 5-7mm compression on the plasticine blobs - so this is the clearance from the highest point of the cells to the deck. Will fill this with some foam rubber . 


![looking%20down%20deck|500x500](upload://ge4qjGgJjrrIsYWoXaumhAmaZ2y.jpeg)
```

---
## \#68 Posted by: lrdesigns Posted at: 2019-01-17T01:07:01.736Z Reads: 237

```
I have considered using [these glass fuses](https://www.aliexpress.com/item/100PCS-3-10mm-4A-Axial-Fast-Glass-Fuse-with-Lead-Wire-3-10-4A-New-and/32798660272.html?spm=a2g0s.8937460.0.0.1a742e0e1Zn0gb) for balance wires, but the ones you listed probably have better vibration resistance. Seems like they are well tested. 

![image|635x500](upload://qXTRl0hAbLQe1XIWBE6phgPEGBw.png)
```

---
## \#69 Posted by: SkaterBoy58 Posted at: 2019-01-17T01:12:18.301Z Reads: 224

```
yeah 
I would never use a glass fuse in the enclosure
```

---
## \#70 Posted by: briman05 Posted at: 2019-01-17T03:26:44.194Z Reads: 220

```
This is a great build very innovative and I like the xt90 plug with the anti spark switch.
```

---
## \#71 Posted by: banjaxxed Posted at: 2019-01-17T10:56:33.368Z Reads: 220

```
I like the idea of this in-line fuse, here is the fuse on farnell which I prefer as they deliver for free in some cases
https://ie.farnell.com/littelfuse/0251001-nrt1l/fuse-axial-1a-very-fast-acting/dp/2723063RL?st=1A%20Axial%20Fuse
```

---
## \#72 Posted by: janpom Posted at: 2019-01-17T11:22:34.173Z Reads: 217

```
That's super helpful, thanks! One more question: Why not put the fuse at the end of the wire, i.e. between the wire and the battery? I believe the closer the fuse is to the battery the better as you want to minimize the risk of a short happening somewhere on the wire between the battery and the fuse.
```

---
## \#73 Posted by: banjaxxed Posted at: 2019-01-17T11:51:30.680Z Reads: 218

```
The fuse is really, really close to the battery, I guess a short in the lead wire between the battery and the BMS can be best mitigated by having the fuse as close to the battery as possible, the pic shows this in essence, the only unprotected part is between the fuse and the actual battery, an inch maybe

Oh right I see what you mean, the fuse could be closer to each terminal
```

---
## \#74 Posted by: janpom Posted at: 2019-01-17T12:03:31.461Z Reads: 222

```
Before I saw this thread, what I considered doing is soldering one leg of the fuse to the battery terminal and the other to the balance wire, so the fuse would be sitting between the battery and the balance wire. That seems the safest way of doing it. I imagine the difference between this and having one inch of wire between the battery terminal of the fuse is marginal. Still, putting the fuse at the very end of the balance wire even seems easier to do, so I wonder if I'm missing any obvious problem with doing it that way.
```

---
## \#75 Posted by: lrdesigns Posted at: 2019-01-17T12:14:38.350Z Reads: 215

```
Not much but the fuse is not flexible like silicone wire so it would need to be mechanically fixed to something.
```

---
## \#76 Posted by: SkaterBoy58 Posted at: 2019-01-17T12:39:06.597Z Reads: 214

```
seems a bit of good discussion here -which is interesting considering 99% of diy builds dont have any fuses in balance leads !
```

---
## \#77 Posted by: janpom Posted at: 2019-01-17T13:26:41.619Z Reads: 217

```
Well, same as you, I now have this connector on my board to use an external BMS:
https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/c/5cada7289bff7e0d1ce7ea16790f5bdeb78ddb8f.jpeg

First, @mmaner has warned me that he has had several similar connectors and they all broke down.

Second, I'm sure that sooner or later my kids figure that the rounded connector is a perfect fit for a coin. :sweat_smile:
```

---
## \#78 Posted by: SkaterBoy58 Posted at: 2019-01-17T13:29:04.953Z Reads: 216

```
so why do have the male version with exposed pins and not the female version socket?
```

---
## \#79 Posted by: janpom Posted at: 2019-01-17T15:37:35.775Z Reads: 215

```
Good point. The other way around would make a whole lot more sense, but that's just the way this particular connector works. The female part doesn't have the panel mount. I would have to modify it... which might have been worthwhile. I just never really thought of swapping them. Thanks for the idea.
```

---
## \#80 Posted by: janpom Posted at: 2019-01-17T17:19:38.924Z Reads: 218

```
Ha, looks like both versions are available.
- [female with panel mount](https://www.aliexpress.com/item/SP2110-12-pin-waterproof-connector-IP68-LED-power-cable-connector-pancl-cutout-21mm-12pins-Plugs-and/32767770117.html)
- [male with panel mount](https://www.aliexpress.com/item/SP21-12pin-Outlet-Opening-Waterproof-Aviation-Plug-Panel-Mount-plug-socket/32920827543.html)

I got the wrong one. :| Good to know.
```

---
## \#81 Posted by: banjaxxed Posted at: 2019-01-17T17:25:19.233Z Reads: 214

```
Substitute the threaded cap for one you find on a childproof medicine bottle winky winky
```

---
## \#82 Posted by: SkaterBoy58 Posted at: 2019-01-19T06:35:54.409Z Reads: 232

```
first real range test today in 40 degree C perth heat

Total distance 51.9 km [range test ride 19 Jan ](https://www.strava.com/activities/2088097082)

basically gunned it wherever possible and accelerated up hills .  The board was superb in handling and felt very stable even at high speed. The power and torque is a big step up from my other diy build with dual 5065 motors.

Pack starting voltage was 41.5V with balanced packs to within 10mV

End of 52 km ride pack voltage = 36V with balanced packs within 9mV

 ![end%20of%20range%20test%2019%20Jan%202019|690x340](upload://xSjieexXwyhqWx8N5HnbVUk01c7.jpeg) 

Will do a longer range test (maybe 75 km) on a cooler day!

Will now measure how many charge Ah it takes to get back to full charge.

And a few shots of completed board- all that remains to do is to fit headlights and a brake light 

![8A321614-80D8-4A1D-BA7B-4FA826D61F08|666x500](upload://buT2Hi2XknEgwqJ2aACZHXmFsWy.jpeg) 




![IMG_4414|666x500](upload://oZ5Q4T2s6BxSI5LOIY2Uo7fVcSe.jpeg) ![IMG_4411|666x500](upload://vRq4U25nlliTtY7XXsXVnKCcC41.jpeg) ![FD7A8057-D897-4AD2-A456-1C812E33B7B4|666x500](upload://dgullc3ijj2td1rUxFGTUpaYLMw.jpeg) ![IMG_4410|666x500](upload://tyDuRW4pA9e0kKfcgIYNGxPDNgC.jpeg) ![IMG_4413|666x500](upload://rbxEySZwOs8u1B0U5acrjUgfdQa.jpeg)
```

---
## \#83 Posted by: SkaterBoy58 Posted at: 2019-01-20T03:10:09.291Z Reads: 214

```
So it took 730Wh to get back to fully charged after range test yesterday.

This means board consumed 14 Wh/km yesterday which is not too bad considering the agressive riding at times.
```

---
## \#84 Posted by: billappleton Posted at: 2019-01-20T13:14:34.284Z Reads: 208

```
Throttle curve looks upside down. Don't you want an S shape? So that the throttle is more touchy close to zero and less touchy in the power zone?
```

---
## \#85 Posted by: SkaterBoy58 Posted at: 2019-01-20T23:11:51.274Z Reads: 207

```
check the axes on your tool !
```

---
## \#86 Posted by: AlexBE Posted at: 2019-01-21T01:47:37.628Z Reads: 211

```
No generally not. You want smooth control of throttle at low values because there is a bigger difference in feel between 0-10A than 10-20A.
```

---
## \#87 Posted by: SkaterBoy58 Posted at: 2019-01-28T00:23:07.068Z Reads: 208

```
And then there was three -all built to same electrics/battery recipe but slightly different motor mounts and wheels

![image|666x500](upload://58W9BP5zIHwW7hTXp7dtsZbpdGQ.jpeg) ![image|666x500](upload://z3h6tsRZjZJdU3FaZu14EyOT4zb.jpeg) ![image|666x500](upload://lgEhZyKQSwawtvopowkHPto5G0N.jpeg) ![image|666x500](upload://thNrSk1WE55mJlD6xDntVdwXymf.jpeg)
```

---
## \#88 Posted by: SkaterBoy58 Posted at: 2019-01-28T00:28:53.057Z Reads: 194

```
These builds take all 11 balance wires to a socket for external bms and portable voltage meters etc. so the main purpose of the fuse is to protect against external to board accidental shorts of the balance leads
```

---
## \#89 Posted by: Pedrodemio Posted at: 2019-01-28T03:53:25.426Z Reads: 197

```
Really great build, wished I went with the 50E on my build, but to expensive for now

And 14 Wh/km is really great on pneumatics
```

---
## \#90 Posted by: sebaszz Posted at: 2019-01-29T14:13:47.888Z Reads: 190

```
really nice built and very good built in safety features :+1:

have you considered using separate receiver for the ppm/ brake light unit? my concern is if something happens with the brake light/wiring/module it could affect your ppm signal.
```

---
## \#92 Posted by: SkaterBoy58 Posted at: 2019-01-29T23:34:53.337Z Reads: 184

```
yeah 50E are performing very well - went for a 51km ride last weekend - flat out where possible - average speed 29.5 km/hr - top speed 46 km/hr and gunning it up hills

Started fully charged 41.7V and end voltage 35.1V ( and cell pack balance within 20 mV) 

Still to do a 75/80km ride to fully test range of board  !
```

---
## \#93 Posted by: SkaterBoy58 Posted at: 2019-01-29T23:35:42.384Z Reads: 188

```

yeah - forgot to put it on the board schematic - but on my earlier build with brake lights actuated on PPM signal - I put a 5k resistor in series with the control wire from receiver to brake light module to overcome concern of brake light module messing up PPM signal to VESC. Will do the same thing this time.

For the mini remote - haven’t tried it but I am not sure you can bind one remote to two receivers -in any case you will still need a 5V supply for second receiver!

Cheers
```

---
## \#94 Posted by: Airfox Posted at: 2019-01-31T20:08:57.739Z Reads: 174

```
What would you say the best motor mount would be?  I'm considering building one of these.

Thanks 
Scott
```

---
## \#95 Posted by: Sn4pz Posted at: 2019-01-31T20:14:35.860Z Reads: 174

```
holy freak im getting a pack like yours and I thought the 30mile range was a big joke, to be honest.... very excited

How did you program your VESC? and How punchy was it?

Im getting a 12s6p of the 50Es and I just want to make sure the ride is torquey enough for me to not want to upgrade for at least a little while
```

---
## \#96 Posted by: SkaterBoy58 Posted at: 2019-01-31T23:11:23.453Z Reads: 170

```
Scott - What is your criteria for "Best" ?
```

---
## \#97 Posted by: SkaterBoy58 Posted at: 2019-01-31T23:12:39.347Z Reads: 173

```
VESC settings are in a post above - plenty of torque/speed throughout battery range with the 10S6P 50E Pack.
```

---
## \#98 Posted by: Airfox Posted at: 2019-02-01T00:50:50.936Z Reads: 185

```
I'm new to Esk8 so inexperienced.  The LaCroix seems to meet my needs.  I used to skate as a teenager and long time wakeboarder/ski/showboard.  I am in the market for an Esk8 for transportation and carving fun.  I built and fly a bush plane and want a Esk8 with a/t wheels to take with me on trips.  Light weight carving machine is what I'm looking for.  

I've been watching Esk8 on social media and concluded the Lacroix is the closest to meet my needs.  I saw a post of a guy who built a Lacroix on the Facebook page.  The post claimed it was even better than a factory LaCroix.  It used the Unity, better battery and it had better performance.  My thinking is if I can build a better board than ordering one then I'm all in.  I posted questions asking about a parts list.  The builder pointed me to this thread. 

 I am trying to build a list of parts needed to build an ESK8.  I like the look of the 3 boards that you posted.  I know I can order the board, trucks and battery case from LaCroix.  The Unity can be ordered from Enertion.  Not sure specs on the Motors or mounts.  There may be other stuff I don't know about yet?  From your post you used 3 motor mounts.  I'd like to know which would be best.  I am in the US if that helps with your advice.  

If you have time a parts list an where to order would be awesome.  
Thanks

Scott
```

---
## \#99 Posted by: SkaterBoy58 Posted at: 2019-02-01T04:06:41.306Z Reads: 173

```
Scott 
there is bit of a parts list on very first post
```

---
## \#100 Posted by: hyperIon1 Posted at: 2019-02-01T08:31:07.222Z Reads: 187

```
I'm fixing to start a 10s6p of Samsung 50E cells for a custom La Croix. 
![20190127_005927|375x500](upload://2H1dCHVeRCQeBtNky4zizIbr7s2.jpeg) ![20190127_010127|640x480](upload://5cWATGHJt9rLViNpseYSHMwEf5F.jpeg)![20190125_032425|666x500](upload://ljhC2fuBveDdJcyxXXrsrPp4nQk.jpeg) ![20190127_004119|375x500](upload://zxspRcfiLt8XU1GHnJ55slZrqFE.jpeg)
```

---
## \#101 Posted by: SkaterBoy58 Posted at: 2019-02-06T00:46:21.715Z Reads: 188

```
Completed a few other minor bits to finish off enclosure electrics

**Brake Light**

Using a Turnigy RC ON/OFF switch here to drive a brake light ( [link to Turnigy RC Switch ](https://hobbyking.com/en_us/dr-mad-thrust-electronic-on-off-switch.html))  with switch PPM input wired in parallel with mini remote receiver channel 2 with a 1k resistor in signal wire to switch.  This RC switch providers a 5V output which is on with throttle above 50% ( neutral 1.5 mS) and off below 50% (braking) . I wired this 5V output to a miniature 5V relay which was hot glued to the switch. Using a NC contact off the relay will provide a brake light voltage when remote is below 1.5 mS PPM .

![IMG_4459|666x500](upload://lR1we1ZlH9HB4CNPvXQgGYq2P54.jpeg) 

![IMG_4460|666x500](upload://7wheq5Za2PHq8BlB0jvtZrIUxqT.jpeg) 

Have ordered a brake light from AliExpress ([link to Brake Light](https://www.aliexpress.com/item/Universal-6-LED-Motorcycle-Brake-Tail-Strobe-Light-Flash-Running-Lamp-Red/32966220235.html?spm=2114.search0104.3.287.abe43720FBhzRF&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_10130_10547_319_317_10548_10696_453_10084_454_10083_10618_10307_537_536_10131_10132_10902_10133_10059_10884_10887_321_322_10103,searchweb201603_56,ppcSwitch_0&algo_expid=e454a710-cdfa-4734-8767-f8a33daedfd6-42&algo_pvid=e454a710-cdfa-4734-8767-f8a33daedfd6&transAbTest=ae803_3)) which will mount on motor mount cross struts. 
![brake%20lights|473x500](upload://7c0GCwRjsFkqNQsrjk1w3SqfrZv.jpeg) 
This has functionality of a strobing tail light and then a bright flashing braking light. It is operated of 12V so installed a 12V BEC module off vesc dc supply. Schematic below 
![brake%20light%20schematic|690x487](upload://kstwWdCeBRv95d1zjsEvtHLfr0m.jpeg) 

**Warning Bell**

Using another Turnigy RC ON/OFF switch here but connected to receiver channel 1 ( mini remote steering wheel) . This will sound the pedestrian/dog warning bell when the mini remote steering wheel is activated.
schematic below
![warning%20bell%20schematic%20|690x487](upload://nGgL0UtWFGtTHZXNzyxZKRY9Bpj.jpeg) 

Using this warning bell with small lipo removed and powered by mini  receiver 5V supply with a dropping diode to reduce voltage to 4.2V . The device will be mounted inside enclosure - it is quite loud at 120 dB.
![warning%20bell|690x469](upload://h5uVtZsxP6E5cESM1S1PjYhAFYQ.jpeg) 






**Front Headlights**

Using two of these lights that have proved very reliable on previous builds and they are very cheap (A$13) . They can output 7,000 lumens each and have low/medium/high/strobing beam modes. They normally run off a 2S LiIon battery pack (8.4V) but I have tested them on 9V with good results ( and slightly less current than 8.4V).

![lights|494x373](upload://bvlIlWrzSYbiV5bzE5U8uawbNYM.jpeg) 

Will mount then on front trucks using supplied rubber bands initially – with a fancy metal bracket to follow later.
```

---
## \#102 Posted by: SkaterBoy58 Posted at: 2019-03-08T00:29:12.649Z Reads: 179

```
Build is totally complete now with following items recently completed


**Flipsky DUAL FSESC 6.6**  - updated firmware to latest release V6 FW 3.48 with no hardware limits. Works fine and annoying brake grab at 4-5km/hr now vanished. No other noticeable differences.

**Flipsky DUAL FSESC 6.6**  **BLE Module - https://flipsky.net/collections/accessories/products/core51822-ble4-0-bluetooth-2-4g-wireless-module-nrf51822-onboard-ws82013**
![flipsky%20BLE%20NRF51%20module|464x486](upload://lfJB2ETg6afDUeoyfRSWm0zBBwb.jpeg) 

Connected a Flipsky V6 NRF51 module in slave UART port. Main function of this is to be able to use the VESC Tool 1.0 in full functionality over the phone. Worked fine with no issues. It keeps connection over about 20 metres. BLE 2.4 GHz whip antenna is inside enclosure. Also use this to connect to XMatic App on phone - so can run both Metr (from master uart )and XMatic ( from slave uart) app at same time.

**Enclosure bolts** – changed over to M3 button socket screws on enclosure  for nicer look and strength. 

![enclosure%20m3%20bolt|473x368](upload://AmdieAOgTl7k7RFdFLKPh7U9tP6.jpeg) 

**Brake Light** – mounted tail/brake light on rear cross-strut with a piece of angle aluminium. This acts as tail light and much brighter brake light which is activated when remote is below mid trigger position (coasting) . Fitted a 100-ohm resistor in tail light circuit to reduce brightness a bit. Reduces tail light to approx. 8V. 

![IMG_0050|666x500](upload://rJmOxBcGbUFGPCLhyUbtm2FDUfG.jpeg) 

![brake%20lights%20photo%202|666x500](upload://7QFda76hJiBvCULiaOsHjkrmgUw.jpeg) 

**Warning Bell** – originally had this installed inside enclosure but sound level was too low – so moved it to rear of enclosure on outside . This is operated by steering wheel on mini remote (Channel 1) and works well.

**Front Headlights** – mounted these on front truck using supplied elastic rubber grip. Used these on a few rides now and the mount appears to hold OK. Usually run on low beam on paths with other traffic and switch to high beam when no other traffic around.

![front%20headlights|666x500](upload://yJEobKdNGN9tXnCH6wjHyhv7LUX.jpeg) 

![front%20headlights%20photo%202|666x500](upload://meCjONADVkH8U8Vci3nWrKxbHSr.jpeg) 


Have completed approx. 600km on the board with thoughts

* Board handles awesomely and is a level above everything else for long range cruising rides
* Extremely stable at high speed (+45 km/hr) whilst still having carvability at lower speeds
* No issues with MBS “roadie” tyres
* No troubles with MayTech 6374 motors ( but others in group build have had problems with rotor shaft becoming loose at cowling end)
* I did have a problem with one of the MBS Pro 2 trucks axles, but this was replaced under warranty OK
* Flipsky  FSESC 6.6 has been faultless and normally runs at 10-degree temperatures rise above ambient . Max motor current is set to 100A for max torque .
* Main power ON/OFF  mechanical relay has been faultless ( pleased that no ASS in this board)
* Battery pack – Samsung 50Es have been superb with high capacity and very even pack discharge ( within 30mV ) . Longest ride has been 65 km pushing board aggressively to max speed and  arrived home with 35.0V . So estimated range is easily 75km + . Consumption is approx. 13-14 Wh/km . I keep tyres pumped up to 50 psi.
* Enclosure strip and sealing – opened up enclosure recently and the inside is very clean with no sign of dust etc. The internals looked identical to the initial build.

Looking forward to this board being trouble free for a long time and completing a lot of long-range cruises covering a lot of km .

Overall – I think this DIY build is substantially better than the stock board and well worth the effort in the build.  

All five La Croix in the DIY group build are now complete with happy campers all round.!

Thanks a lot to @Arch  for providing decks and enclosures all the way from Montreal to Perth Australia  on the opposite side of the planet !

![boards|666x500](upload://yuOQBS2NI4fx6wk2hG0oIh9cdAr.jpeg) 

( mine is second from right)
```

---
## \#103 Posted by: MattyG Posted at: 2019-03-08T00:55:11.744Z Reads: 167

```
great wrap up of our build mate! very pleased with everything we were able to deliver on this build 👍🏼 (mine is second from the left 😃)
```

---
## \#104 Posted by: deucesdown Posted at: 2019-03-08T02:33:43.375Z Reads: 172

```
awesome awesome.

I remember you had a horn glued to the mini remote. Do you prefer the RC activated one mounted to the board?

And, did you do anything different with the relay switch? pics? :slight_smile:
```

---
## \#105 Posted by: SkaterBoy58 Posted at: 2019-03-08T04:21:23.475Z Reads: 174

```
For Remote - yeah use the mini remote with inbuilt horn on my other Land Yatch build - still going strong. RC activated one on bottom of enclosure would probably be my choice going forward for future builds. 

ON/OFF Relay - in this build went for any even easier solution than last build - a non latched mechanical relay with a simple pushbutton ON/OFF switch. 

![80A%20relay|487x437](upload://ccwlwchfDryXHpj9Rml0dENqNqU.jpeg) 

This works very well to date -( I soldered all connections to relay)

and very cheap [link - 80A 36V Relay from AliExpress](https://www.aliexpress.com/item/Black-universal-4-pin-DC80A-12V-24V-36V-48V-electronic-relay-auto-relay-for-Battery-car/32833941490.html?spm=a2g0s.9042311.0.0.76674c4ditBzmn)  

not sure why people still use expensive and prone to failure electronic anti-spark switches!
```

---
## \#106 Posted by: deucesdown Posted at: 2019-03-08T05:07:09.383Z Reads: 165

```
Verrry interesting.

[quote]
working temperature:-40 to+125℃
Contact Form:1a，1b,1c
Contact Rating:
1a/2a:80A 14VDC      
1b:60A 14VDC
1c:80A/60A 14VDC
Coil Voltage:
9vdc,12VDC,24VDC,
36VDC,48VDC,72,VDC,
Coil power:1.8w
Contact Resistance:≤50mΩ
Insulation Resistance:≥1,00MΩ
Environmental temperature:-40℃~+125℃
[/quote]

Please forgive my lack of actual knowledge. :) This means the coil has good wide voltage range, and uses 1.8w when the relay is in "on" position?

But the power path is actually rated for 14vdc only (contact rating)?

And no power means switch is open?

So cheap!
```

---
## \#107 Posted by: SkaterBoy58 Posted at: 2019-03-08T05:11:57.172Z Reads: 163

```
it works

suggest you start a new thread if you want to debate vesc switching duty and relay contact rating
Cheers
```

---
## \#108 Posted by: hyperIon1 Posted at: 2019-03-08T07:11:21.355Z Reads: 166

```
Samsung 50E 21700 
12s5p 1260 Wh
![20190227_131950|375x500](upload://ft7vqC3pJoFXIA3VlKWXNnOH4xL.jpeg)
```

---
## \#109 Posted by: sayekim Posted at: 2019-03-08T17:09:44.600Z Reads: 162

```
1.26 kWh no?

1260 kWh = 1260000 Wh 😱
```

---
## \#110 Posted by: hyperIon1 Posted at: 2019-03-08T21:07:01.956Z Reads: 159

```
If this calculation is correct in a 12s5p configuration 
![30%20PM|634x500](upload://budBW7ouJQGAoZsoxNxzFaCLRKp.png) 


![image|642x500](upload://rFgEi5pWW9tA2Liqoph6heThmT.png)
```

---
## \#111 Posted by: deucesdown Posted at: 2019-03-08T21:21:04.972Z Reads: 154

```
5000ah is wrong, one cell is 5000mah aka 5ah.
```

---
## \#112 Posted by: hyperIon1 Posted at: 2019-03-08T21:33:37.653Z Reads: 153

```
I see what you're saying it's just the way I have used the calculator to get the capacity, I just forget to drop the k
1.26 kWh = 1260 wh
```

---
## \#113 Posted by: celica39 Posted at: 2019-03-10T04:44:27.682Z Reads: 148

```
i don't know where you get 75km with  30ah pack with a 80kg board lol! you must be 5.2 with 130 pound 
my complete board weight 25kg with lipo 16ah/ 12s (9pounds)  pack  and  l weight 190 pounds and i can do 23km with some mostly flat surface at 25-30kph average  my chain drive is  10/48 (5/1) top speed on gps 53kph
to acheive this range i have to be very smooth on trottle and if i do speed this will drop at 15km range 
I am very  lite compare to your set up
```

---
## \#114 Posted by: hyperIon1 Posted at: 2019-03-10T08:11:45.268Z Reads: 145

```
all true, but that is just a capacity calculation, not a range calculation a lot more info is needed to roughly calculate range.  Even at 27lb it will get well over 30 miles. So far I haven't seen anyone do a true range test on one. I would assume their legs turn to jelly before they hit bottom. Soon this will be on a board and we may get a report
```

---
## \#115 Posted by: SkaterBoy58 Posted at: 2019-03-10T08:50:29.323Z Reads: 147

```
not sure what you are saying here

see above for my discharge test = 1,051 Wh from 42V to 30V.

I average about 14/15 Wh/km on this board and this is similar to my other pneumatic tyre board

The rest is maths =70/75km range

Cheers
```

---
## \#116 Posted by: celica39 Posted at: 2019-03-10T09:04:22.836Z Reads: 152

```
Happy for you if you get 14-15 Wh/km with all that weight you probably run mostly on flat surface.  The thing l don't like about high gear ratio (58 teeth and up)  is the top end come too quickly ,btw at 40k/h my motors are not screaming so its great to have some juice left to get 53-54 top speed if needed
```

---
## \#117 Posted by: SkaterBoy58 Posted at: 2019-03-27T23:32:33.019Z Reads: 137

```
All five boards in DIY group build together on a 95km ride earlier this week

![image|690x354](upload://spfLXNSCLtjNNGaU2OdxX2TR4Mq.jpeg) ![image|666x500](upload://l5kdbrAkAb6Hcq1KahafiuoSfdg.jpeg) ![image|280x500](upload://9nBfQqPwhVBulFap4FY7pjGbd1.jpeg)
```

---
## \#118 Posted by: hyperIon1 Posted at: 2019-03-28T00:04:02.695Z Reads: 129

```
So, 95km (60 miles) ride any stop and charge? 
or is this on one charge with the 50E 12s5p?
```

---
## \#119 Posted by: lrdesigns Posted at: 2019-03-28T02:52:22.660Z Reads: 130

```
I thought watt hours of a pack should be calculated with nominal voltage? As that is roughly the average voltage of the pack under load over a full discharge. 

[quote="hyperIon1, post:108, topic:76960"]
Samsung 50E 21700 12s5p
[/quote]
Cool pack though!! Very neet.
```

---
## \#120 Posted by: celica39 Posted at: 2019-04-05T02:57:42.030Z Reads: 118

```
i ride since 2015 and i made several change in ratio and the esk8 calculator is 
very close to my top speed and range  real 30-35 km with  (25kph average speed )and  again it depend on weight  of the person and if you soft with the trottle  if someone can proof i can  do 60km  with a 12s  16ah lipo pack  give  me magical  the recipe please !!  i use dual 190kv 6374 motor
```

---
## \#121 Posted by: hyperIon1 Posted at: 2019-04-05T14:29:30.296Z Reads: 108

```
All very true, feather-light guys get much more range than the heavy guys, and so for the throttle if your hard on the acceleration and braking. everything is a factor. 
We are currently working on a set of batteries made with the Sanyo 20700c 35A cells and think they will surpass some of the High Amp lipo set ups....
```

---
## \#122 Posted by: peppoonline Posted at: 2019-04-15T19:02:40.536Z Reads: 85

```
Good Job! 
What a great build... if you ever gonna sell ---> neeeeed :grin:
```

---
