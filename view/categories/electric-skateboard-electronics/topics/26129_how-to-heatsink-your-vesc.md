# How-to: Heatsink your VESC!

### Replies: 66 Views: 7973

## \#1 Posted by: sl33py Posted at: 2017-06-25T09:29:00.332Z Reads: 878

```
Credit to @Chaka and Enertion for offering their VESC and VESC-X/FOCBOX in some sexy aluminum enclosures/heatsink sandwiches!  (just llaid hands on @smurf's direct-FET Ollin VESC - gorgeous!!!) 

But i don't have either.  And I want a heatsink.  As much for cooling as **secure flat mounting!**

So i'm going to start off focusing on the base plate (easier w/ no "cutouts" needed for UART/Sensor/etc. plugs).

A quick trip to the local hardware store had some 1/8" aluminum that is *perfect* width:
[img]https://goo.gl/GTPYS9[/img]
(4 feet should give me plenty for a few!)

Working with basic tools (no CNC yet), i took some measurements of hole spacing (not perfect i'm sure), and found the intersections and punched them:
[img]https://goo.gl/d9cL1Z[/img]
I measure it out, cut with dremel cutoff wheel, and sanded the ends to clean them up a bit.  Again - not perfect (and i'm totally OK with this - function over form).

Once i confirmed alignment with the VESC holes, I used the first as a template and clamped them together to drill the rest out on the drillpress w/ 1/8 bit (closest - smidge bigger than VESC holes in mm).
[img]https://goo.gl/JGm9bG[/img]

Spacers to raise the PCB above and clear the aluminum...  I got a bunch of fiddly little copper squares in different thicknesses specifically for this...  and then i tested one of the pieces of aluminum and the 1/8" thickness worked *GREAT* as the standoff/spacer!  So i cut 2 before my dremel needed re-charge and it was starting to get late...  I cut them 12mm wide.  So even after sanding edges smooth - still a bit generous. Plus a bit of overhang of the FET and leeway for less-than-perfect alignment/placement.  

Some Arctic Silver adhesive, a stir stick and VOILA!
[img]https://goo.gl/uEPdgm[/img]
(rough sanding to get burrs - will have a thermal pad or arctic silver thermal paste to fill in the scratches and imperfections for good heat transfer).  This is not the 90's AMD Athlon i lapped for OC'ing...

It's getting on "stupid late" and need to crash, but a quick test fit to show the plan:
[img]https://goo.gl/6hZTSR[/img]

I will cut back (but not fully remove) the heatshrink - so the FETS are flat and in contact w/ the aluminum spacer/riser block, and use some plastic m3 to secure to VESC.  I'll try to show some pics tomorrow when i start those next steps.

So that's the plan folks - a quick and _easy_ DIY heatsink for a VESC!  Mostly simple tools, and absolutely doable with nothing but hand tools!  About ~$15 for 4 feet of aluminum (share w/ your friends!)... plus fun fiddling in the garage = _Winner winner chicken dinner._  Soon some flat mounting VESC's that happen to have a bit more cooling (i hope).  I'll work on the top solution next and show you all what i plan there too.

Hope it helps the next OCD DIY'er who is tired of wobbly velcro'd VESCs!

Night all!
```

---
## \#2 Posted by: sl33py Posted at: 2017-06-29T09:19:33.083Z Reads: 810

```
More progress.

Test fit complete.  I need to clean up the pins and some hot glue to ensure none poke into power wire (bad short - easy to avoid).  Then i'll re-shrink and re-mount.

But here's the goal (at least bottom - still figuring out top heatsink):
[img]https://goo.gl/WweM7Y[/img]
[img]https://goo.gl/A97do6[/img]
[img]https://goo.gl/rt49gG[/img]

Simple m3 nylon screws and standoffs.  you can see a bit of a gap but it tightens down securely and feels really solid!

Super pleased at my hole alignment and fit.  just a bit more cleanup and add the heatsink paste and should be GTG!
```

---
## \#3 Posted by: Alanhunt123 Posted at: 2017-06-29T12:24:33.266Z Reads: 752

```
It's really surprising how much power these 4.12 boards are capable of when the MOSFETs have a proper way to remove heat. Any plans for the upper MOSFETS?
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-06-29T14:15:49.160Z Reads: 740

```
this is my kind of thread. Simple and effective and accessible.
```

---
## \#5 Posted by: chaka Posted at: 2017-06-29T15:11:00.921Z Reads: 738

```
I have tried thermal pads, thermal paste and heatsink potting compound. Lots of debate over what is best so I will just say potting compound is what I use and recommend. You can get a tube for a few dollars on ebay and it doubles as a good setting compound for stabilizing wires coming out of a jst connector.

 With potting compound you can interface with more surface area. Potting the gate, source and drain produces some decent results. 

If you go down this road be sure to clean the vesc well before applying any type of coating or compound. Moisture can accumulate in areas with poor adhesion. I recommend using an acrylic conformal coating before applying potting compound to further guard against possible moisture issues down the road. 

While we are on the topic, it would be easy to make a breakout board with direct fet footprints. It could be designed so that it replaced the irf7430 and not take any extra space. I wont say it would be easy, you would need some reflow skills and a hot air machine.
```

---
## \#6 Posted by: sl33py Posted at: 2017-06-29T17:53:53.266Z Reads: 689

```
[quote="Alanhunt123, post:3, topic:26129"]
Any plans for the upper MOSFETS?
[/quote]


Still thinking on the top FETs.  I have a few finned aluminum heatsinks i know will work - the challenge is mounting them reasonably securely without permanent thermal paste.  

I'll play with it some more and come up with something.
```

---
## \#7 Posted by: sl33py Posted at: 2017-06-29T18:03:28.921Z Reads: 675

```
[quote="chaka, post:5, topic:26129"]
I have tried thermal pads, thermal paste and heatsink potting compound. Lots of debate over what is best so I will just say potting compound is what I use and recommend. You can get a tube for a few dollars on ebay and it doubles as a good setting compound for stabilizing wires coming out of a jst connector.

 With potting compound you can interface with more surface area. Potting the gate, source and drain produces some decent results.
[/quote]


Thanks @chaka!  I'm intending to keep this non-permanent so i can remove if needed (and move to another VESC - i have a few).

I know you push the limits, so let me be clear on my goals:

1. better flat mounting.
2. improved cooling and thermal capacity (able to load the heatsink for longer uphill run)
3. be *kinda* cool, but not CNC cool like yours.  DIY cool maybe.

That's it - simple and something doable w/ handtools (drill press really helps, but steady hands totally would work).

Of course i'm going to go look at thermal potting compounds anyway.  I've always used arctic silver compounds on my PC's and know they provide *excellent* thermal transfer - so i was intending that between FETs and lower plate, and again between upper FETs and TBD heatsink.

I have some conformal coating already - i'll need to check if it's acrylic based.

Really appreciate the insight and contribution to my little project man!
```

---
## \#8 Posted by: Alanhunt123 Posted at: 2017-06-29T18:19:03.622Z Reads: 622

```
You could make some kind of bridge to go over them and try to transfer the heat through screws to the base. That's what I did with mine, and it seemed to work well. Then again, literally anything is better than constricting the MOSFETs inside a silly layer of heatshrink!
```

---
## \#9 Posted by: JLabs Posted at: 2017-06-29T19:03:44.159Z Reads: 630

```
<img src="/uploads/db1493/original/3X/a/7/a78fefce8aac34d32f59e27b28e336004ab3529d.JPG" width="690" height="363">
Be careful, you don't want the pins of the jst connector to punch a hole in the power wire. I would add some hot glue to the bottom of the pins or cut them off.
```

---
## \#10 Posted by: sl33py Posted at: 2017-06-29T20:42:26.151Z Reads: 620

```
[quote="JLabs, post:9, topic:26129"]
Be careful, you don't want the pins of the jst connector to punch a hole in the power wire. I would add some hot glue to the bottom of the pins or cut them off.
[/quote]

@JLabs - yep!  I just test fit this, but at the start called out i was going to hot glue, then re-shrink to give some protection:
[quote="sl33py, post:2, topic:26129"]
More progress.

Test fit complete.  _**I need to clean up the pins and some hot glue to ensure none poke into power wire (bad short - easy to avoid)**_.  Then i'll re-shrink and re-mount.
[/quote] 

It's super important, but i also think that if i use a washer to avoid PCB flex/movement - it shouldn't be able to pressure down on the wires now that they are between the fixed mount and PCB to puncture.  I'm still going to clip and hotglue them because it just takes a minute and ensures no short.
```

---
## \#11 Posted by: sl33py Posted at: 2017-06-29T20:46:14.824Z Reads: 587

```
Yeah, thought about some side mount attachment monstrosity... but think i'll try to stay simple.

If you need to *REALLY* push your VESC and this extra cooling is _make-or-break_ for you - go buy @chaka's/Ollin Board Co's new sexy CNC Direct FET VESC.  I've held them - they are gorgeous!

If you want _some_ improved cooling for occasional heat/throttling issues - and want a more sturdy flat mount - THIS DIY IS FOR YOU!
```

---
## \#12 Posted by: JLabs Posted at: 2017-06-29T20:47:46.410Z Reads: 565

```
Woops I mostly look at the pictures :smile:
```

---
## \#13 Posted by: sl33py Posted at: 2017-06-30T09:56:15.198Z Reads: 591

```
Well - for folks who find this and want to see what we are talking about (and how to fix).

If your pins under the power wires aren't clipped the issue is it can pierce the wire sheathing and short - killing your VESC and let the magic smoke out!  I also add some hot glue as extra insurance-  here's what it will look like (the two sets of pins i've seen pierce and kill a VESC):
[img]https://goo.gl/K6aVNf[/img]
[img]https://goo.gl/kLjZsR[/img]

Then clipped (i use some sharp nail clippers or small flush snips):
[img]https://goo.gl/adbap7[/img]

Then a small dab of hot glue to cover:
[img]https://goo.gl/SyCGrw[/img]

There ya go @JLabs - pictures!  hehehe

back on topic (my thread so i'll wander if i wanna!)...

Made a few more, and cleaned them up a smidge:
[img]https://goo.gl/kMxqQN[/img]

Then on a @zmoney / Axle VESC (very nice quality w/ upgraded BOM components - just wish it wasn't XT60 i'm swapping):  Already snipped and some glue to protect.
[img]https://goo.gl/k9bG8X[/img]

I'll work on the top heatsink tomorrow...

Night all!
```

---
## \#14 Posted by: monkey32 Posted at: 2017-06-30T10:45:48.637Z Reads: 570

```
Awesome work man. Wish I was still in Sea town i would love to have met up and ridden. Everything you post is stupidly useful both here and ES. Props brother, on yet another helpful thread.
```

---
## \#15 Posted by: sl33py Posted at: 2017-07-02T21:14:49.682Z Reads: 572

```
Fun long weekend and spending a lot of the time in the garage!

Working on this a bit more, I'm trying a couple different setups.  Since my stable/bevy of beautiful VESC's have been pretty problem free (besides a few i killed on the bench w/ 12s) - i'm going to adhere the bottom mount on a few and try both permanent and thermal paste (vs adhesive) on the top.

I double checked all pins are cut flush, hot glue to protect from possible puncture/short (also less likely since flat mount with standoffs prevent pressure), then screwed m3 nylon w/ washers and spacers - finally re-shrinking VESC and cutting out only minimum needed (trying to keep it somewhat protected, but not water or splash proof by any stretch.)  

So here's the mount, and a re-shrinked VESC w/ all my cutouts ready:
[img]https://goo.gl/LcxEus[/img]
Top
[img]https://goo.gl/xDjTpG[/img]
Bottom
(a smidge OCD on the cutouts... i know)

Thin layer of Arctic Silver Adhesive (this is the Arctic Alumina which does not conduct - in case a small bit gets on a leg/trace):
[img]https://goo.gl/s2LThg[/img]
[img]https://goo.gl/yt3jWJ[/img]
(quick clamp to give even pressure and let it set (pretty fast - maybe 15-20 min in 70* temp)

In the garage and up way too late, but great Saturday!
[img]https://goo.gl/KjUWRn[/img]

Off to keep it going and get some more projects done!
```

---
## \#16 Posted by: Tomer Posted at: 2017-07-03T09:03:30.237Z Reads: 527

```
Thank you for sharing! I'm going to try this on x2 VESC that I have. Living in a hot weather area will not do well for my poor VESCs.
```

---
## \#17 Posted by: monkey32 Posted at: 2017-07-04T06:49:56.806Z Reads: 524

```
sl33py , where are you getting firmware to throw onto your 4.12 VESC? I have two Ollin 4.10 is like to throw on a couple boards but realized that since purchasing I have upgrades computers and now can't seem to find any of my old bldc folders ( new v 6.0 is bright and shiny though).
```

---
## \#18 Posted by: Vanarian Posted at: 2017-07-11T17:08:52.085Z Reads: 519

```
Hi, 

Funny I recognize some names from ES here! 

Topic here is very important and I've been working on finding DIY level cooling solutions for VESC 4xx (I use another VESC type so searching solutions for custom and 6xx too) ;

Now a tip since you have access to a CNC machine, don't bother gluing Alu on top of the plastic. Thermal resistance of the casing is very high, you will gain nothing by cooling it no matter the heat sink. You must cool the PCB and the solder areas. Cooling the metal on side of the FETs also works. 

Using a fan to direct air through this area is also valid to gain few degrees. 

I'll post my solution once I've gotten the parts tested (I'll serve as self Guinea pig). Keep on the good job!

ÉDIT : I forgot, you better be cautious about arctic silver. In couple years it will lose its thermic  property and become hard as rock.
```

---
## \#19 Posted by: sl33py Posted at: 2017-07-11T19:58:54.660Z Reads: 507

```
Hey @Vanarian - yeah i see a lot of the folks from ES here too!
[quote="Vanarian, post:18, topic:26129"]
Now a tip since you have access to a CNC machine, don't bother gluing Alu on top of the plastic. Thermal resistance of the casing is very high, you will gain nothing by cooling it no matter the heat sink. You must cool the PCB and the solder areas. Cooling the metal on side of the FETs also works.
[/quote]

I cut out the heatshrink to expose the top of the FETs - so these are in direct contact, not to the plastic.  Am i missing something?  Look at pics above and you'll see where i coated them w/ Arctic *alumina* (not Arctic Silver).

I wish i had access to CNC - not quite yet.  All done by hand and you can see some rough edges as a result!

I'm using the alumina instead of silver so that it's non-conductive - in case a bit of the paste touches a leg or trace.  

It seems to help, though i haven't tested side by side w/ one without heatsink yet.  I'll have to give that a shot and see if it makes any noticeable improvement.

Thx!
```

---
## \#20 Posted by: Vanarian Posted at: 2017-07-11T20:20:39.737Z Reads: 491

```
To me on the pictures it seems that you put the alumina layer on top of the individual black plastic cases of the FETs? These small boxes have a thermal resistance very high, that's what I was talking about.

For example I don't have heatshrink on my VESCs, I should put some to avoid hazardous shorts though. 

How is the durability of Arctic Alumina?
```

---
## \#21 Posted by: monkey32 Posted at: 2017-08-27T06:21:01.220Z Reads: 450

```
You cant properly remove the black casing so I believe @sl33py is trying to passively direct heat away from it...... 


Hey @sl33py 
How are these working for you. I especially like that Alu. piece in your early one - serves to protect the VESC against bumps. Any reports as to which dissipate better?
```

---
## \#22 Posted by: GhettoFab.rictation Posted at: 2017-11-09T09:16:29.447Z Reads: 440

```
What if we used an L shaped piece to connect to actual unit?<img src="/uploads/db1493/original/3X/6/e/6ebd18554af4f3a2947aaa25bf47843a03d8aeec.jpg" width="281" height="500">
```

---
## \#23 Posted by: GhettoFab.rictation Posted at: 2017-11-09T09:17:10.578Z Reads: 426

```
With the correct size and aluminum of course..
```

---
## \#24 Posted by: ThierryGTLTS Posted at: 2017-11-09T09:39:34.936Z Reads: 419

```
Copper is far more easy to solder and better heat dissipation.
```

---
## \#25 Posted by: ThierryGTLTS Posted at: 2017-11-09T09:41:10.024Z Reads: 418

```
And pay attention to the voltage present in the drain tab!
```

---
## \#26 Posted by: Vanarian Posted at: 2017-11-09T10:53:23.715Z Reads: 409

```
You got it right there! You should try copper as Thierry said and apply also heatsink on other side of PCB.
```

---
## \#27 Posted by: GhettoFab.rictation Posted at: 2017-11-09T11:25:39.450Z Reads: 402

```
Drain tab?
```

---
## \#28 Posted by: Vanarian Posted at: 2017-11-09T15:58:10.254Z Reads: 402

```
Yep cause there is current going through the tabs of the FETs so you need to make sure no current goes into the heatsink piece.
```

---
## \#29 Posted by: Acido Posted at: 2017-11-09T16:56:47.094Z Reads: 396

```
Where did you buy these black heatsinks like one
```

---
## \#30 Posted by: sl33py Posted at: 2017-11-09T21:56:56.224Z Reads: 403

```
I would suggest measuring to confirm, but got these i think:

https://www.amazon.com/BNTECHGO-Aluminum-Heatsink-Cooling-Silicone/dp/B01HSBM5JM

I think i got mine on alibaba a few years ago... or similar site - was in my misc drawer from another project.
```

---
## \#31 Posted by: sl33py Posted at: 2017-11-09T22:00:46.650Z Reads: 400

```
[quote="monkey32, post:21, topic:26129"]
Hey @sl33py 
How are these working for you. I especially like that Alu. piece in your early one - serves to protect the VESC against bumps. Any reports as to which dissipate better?
[/quote]


Seattle - wet.  haven't had much chance to test.  Work/Life bullshit going on so been away and dealing w/ that.  I will eventually run both with heatsink and without (as close to identical as possible) with my eagletree logger to compare actual draw and differences.  I have a FLIR too, but haven't had a chance to dedicate time to test.  I look at it as a bonus for protection and easier/more-secure mounting w/ the flat plate.  Con is definitely increased mounting height.

I've run my guest board (Omen Sugar single 6374) the most of these and it's been bulletproof! (arctic alumina)

HTH - GL!
```

---
## \#32 Posted by: GhettoFab.rictation Posted at: 2017-11-11T06:13:27.157Z Reads: 360

```
What if I use thermal paste for the heat sink that will cool without connecting as a conductor or if it does I might put a fan on it and re shrink wrap it
```

---
## \#33 Posted by: faithfulpuppy Posted at: 2017-11-11T06:26:11.067Z Reads: 353

```
thermal paste/adhesive is difficult to control/apply. the pads are your best bet or you seriously risk frying your hardware.
```

---
## \#34 Posted by: Vanarian Posted at: 2017-11-11T17:27:33.762Z Reads: 374

```
Thermal pads have very limited K/W conductivity so you get low benefits from it. I recommend you use Gelid compound as thermal paste, it is insulated so not electrically conductive. Even if you were to make a mess during appliance it won't short. It will also smooth out all irregularities of silica glass and aluminum.

You can use a drop of Loctite on the black plastic case to get the heatsink fixed steady.
```

---
## \#35 Posted by: SpeedyGonzales Posted at: 2018-01-11T16:22:07.759Z Reads: 357

```
I built a heatsink case.![Vesc case 1|690x388](upload://n74DjZXsMsMdofaT5hcDQbYqN1Q.JPG)![VESC case|690x388](upload://bKLN3nebJaz8EULv1veggiOSfzP.JPG)
```

---
## \#36 Posted by: E1Allen Posted at: 2018-01-11T21:59:32.362Z Reads: 339

```
That looks solid
```

---
## \#37 Posted by: GrecoMan Posted at: 2018-01-12T01:36:35.205Z Reads: 331

```
is that a truck clamp?
```

---
## \#38 Posted by: Mikenopolis Posted at: 2018-01-12T01:37:57.480Z Reads: 333

```
Looks like a bike tube clamp
```

---
## \#39 Posted by: GrecoMan Posted at: 2018-01-12T01:38:20.608Z Reads: 340

```
ahhhh yea that would make sense
```

---
## \#40 Posted by: SpeedyGonzales Posted at: 2018-01-12T02:11:14.787Z Reads: 342

```
You are correct. ![Avian without battery|690x388](upload://hgQaZelnfYJjUiclyiwOdVYCncR.JPG)
```

---
## \#41 Posted by: SlimSh8y Posted at: 2018-06-10T09:27:16.822Z Reads: 291

```
Really? I used Arctic Silver on Xbox 360's for many years when fixing the RROD and I have never had any turn hard as a rock even after a decade of abuse. Gummy and firm for sure, but never have I had to chip it off of anything. What were you using it on when you had this experience with Arctic Silver?.
```

---
## \#42 Posted by: suntorytime Posted at: 2018-06-10T14:27:45.853Z Reads: 280

```
For the lazy like me:

https://ebay.to/2l3obP4

https://ebay.to/2MdpUxz
```

---
## \#43 Posted by: Vanarian Posted at: 2018-06-13T15:09:36.928Z Reads: 255

```
I don't recall what I wrote back then, but I suppose you were referring to thermal paste turning rock solid and being unusable ? I met this issue on an air-cooled i7 processor (first or second generation), I forget which Arctic range it was. Was not a conductive one tho, possibly MX-2 :thinking: 

Some other pastes might be affected too, as it *might* happen. I should find back some infos I searched ! 

Anyway you're lucky if it did well in your case.
```

---
## \#44 Posted by: jens_c Posted at: 2018-06-13T19:22:20.909Z Reads: 241

```
Anny idea on how much current the vesc with the heatsink can handle ??
```

---
## \#45 Posted by: Brontech Posted at: 2018-06-14T02:29:20.973Z Reads: 245

```
@jens_c 
From my knowledge, strapping a heatsink with no active cooling component like a fan will only add to the thermal mass of the component you are trying to cool. 
This can be useful when you are going to power up a hill and you are going to be using more amps than what your VESC is able to provide continuously, without overheating.
So lets say that a given vesc can provide 50 amps for one minute before overheating without any passive cooling installed.
With a heatsink, that time may be among the lines of 70+ seconds depending on how much mass you can strap to the Fets or Drv.

Natural convection may help out the heatsink achieve a higher continuous output, depending on if the heatsinks has fins and space around the VESC to breathe.

So strapping just heatsinks to your vesc will not increase the continuous amps your vesc can output (maybe slightly), but rather slow down the process of the vesc overheating.
Someone correct me in I'm wrong
My 2 cents.
```

---
## \#46 Posted by: danielz Posted at: 2018-06-14T03:43:01.740Z Reads: 231

```
I find it hopeless for my second gen i7 in my laptop too, works for a while, idle in the 40s. However a few months later its back in the 70s. Reapplied it several times. Happened each time.
```

---
## \#47 Posted by: Blacksheep Posted at: 2018-09-08T04:40:19.707Z Reads: 184

```
You should sell kits
```

---
## \#48 Posted by: Rithblu Posted at: 2018-10-11T20:54:38.608Z Reads: 165

```
Would love to build one, you won't happen to have the list of components?
```

---
## \#49 Posted by: moon Posted at: 2018-10-11T21:10:52.451Z Reads: 166

```
Me too, I was going to ask but I realised he wasn't very active here
```

---
## \#50 Posted by: SpeedyGonzales Posted at: 2018-10-12T01:50:39.839Z Reads: 154

```
Are you asking about the bike the VESC case or something else?
Please be more specific.
```

---
## \#51 Posted by: moon Posted at: 2018-10-12T01:53:34.130Z Reads: 151

```
Well I am asking about the bike, not sure about him
```

---
## \#52 Posted by: Rithblu Posted at: 2018-10-12T02:07:59.309Z Reads: 145

```
Part's you use for the bike.
```

---
## \#53 Posted by: SpeedyGonzales Posted at: 2018-10-12T02:36:48.713Z Reads: 139

```
The bike is Giant Trance XO.
If comes to kit it's custom made.
You can read about it here:
https://endless-sphere.com/forums/viewtopic.php?f=3&t=90432
Any of you guys live in San Diego?
```

---
## \#54 Posted by: Rithblu Posted at: 2018-10-12T02:43:54.035Z Reads: 135

```
I'm in Oceanside, all my family are in SD..
```

---
## \#55 Posted by: SpeedyGonzales Posted at: 2018-10-12T03:00:19.681Z Reads: 139

```
Cool, let me know if you will be interested to take the bike for a spin and let me know what you think.
```

---
## \#56 Posted by: moon Posted at: 2018-10-12T03:01:50.814Z Reads: 139

```
I want to lol but guess where I am
```

---
## \#57 Posted by: SpeedyGonzales Posted at: 2018-10-12T03:09:55.143Z Reads: 139

```
Moon dah!!!
```

---
## \#58 Posted by: Rithblu Posted at: 2018-10-12T03:17:02.692Z Reads: 134

```
I'll be going down to SD next weekend, meet take you on that offer.
```

---
## \#59 Posted by: SpeedyGonzales Posted at: 2018-10-12T04:22:09.622Z Reads: 131

```
PM sent.
10 char
```

---
## \#60 Posted by: SpeedyGonzales Posted at: 2018-10-13T16:35:25.071Z Reads: 120

```
I sent you PM and you didn't come back to me with what time you can make it.
What happened?
I hope that you are OK.
BTW: Your parts look awesome.
```

---
## \#61 Posted by: Rithblu Posted at: 2018-10-13T17:15:49.539Z Reads: 109

```
Hey, sorry I get busy sometimes. I ment next Saturday.
```

---
## \#62 Posted by: Rithblu Posted at: 2018-10-13T17:28:05.475Z Reads: 108

```
Just was told by girlfriend, going to TJ that Saturday, so not sure if comeing back across in time to meet up.
```

---
## \#63 Posted by: SpeedyGonzales Posted at: 2018-10-13T17:40:06.270Z Reads: 115

```
No problem and good to know. Have fun in TJ.
```

---
## \#64 Posted by: Bor.inc Posted at: 2018-10-15T13:36:32.798Z Reads: 109

```
![IMG_20181015_153131|375x500](upload://nsQ57We5IGcorZSfXYrCtHae9Fk.jpeg) 
Imagine using these strips, already got the cooling fins hahaha
```

---
## \#65 Posted by: whaddys Posted at: 2019-06-17T03:11:05.028Z Reads: 49

```
@sl33py what did you use to adhere the two aluminum plates (heatsink and 12mm spacer/platform?)  I think I'm going this route for TB 4.12 VESC
```

---
## \#66 Posted by: whaddys Posted at: 2019-06-17T03:13:28.410Z Reads: 49

```
[quote="sl33py, post:1, topic:26129"]
Some Arctic Silver adhesive, a stir stick and VOILA!
[/quote]

nevermind, found it!
```

---
