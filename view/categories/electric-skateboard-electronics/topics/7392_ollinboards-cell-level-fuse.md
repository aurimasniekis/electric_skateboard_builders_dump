# OllinBoards - Cell Level Fuse

### Replies: 199 Views: 15956

## \#1 Posted by: chaka Posted at: 2016-08-09T21:05:27.300Z Reads: 902

```
Continuing the discussion from [Balancing/Equilibrium Board vs BMS. Whats the difference?](http://www.electric-skateboard.builders/t/balancing-equilibrium-board-vs-bms-whats-the-difference/7335/7):

This is how we are currently assembling our packs. This is just a basic mockup, we also apply a strip of fish paper over the brass strips before sealing the packs in heat-shrink for added electrical insulation. Nickel tabs are spot welded to the li-ion cells and the fuse wires are soldered onto the the tabs allowing for a serviceable connection. I'll post more photos with greater detail while we complete our latest build.

Cell level fusing is probably the best way to insure a failing cell does not take out an entire parallel pack of cells throughout the lifetime of your pack. This allows us to string together huge links of paralleled cells and build battery systems with incredible range without worrying if a faulty cell will ruin someones day a few years down the road.

<img src="/uploads/db1493/original/2X/1/111d73e348cd04b6de062ffb85e8d41e2acf67ef.jpg" width="690" height="388">


All together the packs measure under 22mm after heat-shrink is applied.

<img src="/uploads/db1493/original/2X/6/678c02941f5ae7e4cf866321329d22bcf55e932b.jpg" width="690" height="388">

If anyone is interested in these feel free to send us a message.

.stl file on thingiverse: http://www.thingiverse.com/thing:1712459
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-09T21:08:01.634Z Reads: 773

```
Beautiful, are those custom cell holders?
```

---
## \#3 Posted by: longhairedboy Posted at: 2016-08-09T21:11:43.817Z Reads: 764

```
Gorgeous! :)
```

---
## \#4 Posted by: chaka Posted at: 2016-08-09T21:11:48.240Z Reads: 768

```
Yes they are, I still need to make a few changes to speed up the print time but this is the final design for the beta builds.
```

---
## \#5 Posted by: Pantologist Posted at: 2016-08-09T21:13:21.272Z Reads: 747

```
Will these Tesla style packs last with all the vibrations of esk8ing?
```

---
## \#6 Posted by: Kaly Posted at: 2016-08-09T21:13:29.175Z Reads: 731

```
I have to handed it to you ;-) 
that is a clever solution. you are really a resourceful individual Mr. Clark.
Kudos to you :thumbsup: :thumbsup: :thumbsup:
```

---
## \#7 Posted by: chaka Posted at: 2016-08-09T21:17:01.005Z Reads: 710

```
> Will these Tesla style packs last with all the vibrations of esk8ing?

They handle vibration very well, probably much better than nickel strips since the wire helps isolate any movement from tearing the tabs from the cells.
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-09T21:19:50.782Z Reads: 686

```
The wires seem awful thin, are they able to carry higher currents?
```

---
## \#9 Posted by: chaka Posted at: 2016-08-09T21:28:57.389Z Reads: 694

```
The wires are sized according to the cells capability and internal resistance. Length and gauge play an important role here, for 20 amp cells you want a fuse that blows at 22 to 25 amps. If a cell begins to fail the inrush from the other cells in the pack quickly blow the fuse before any damage is done. 

You still want to run a fuse on your main terminals in the case of a short circuit in your electrical system.
```

---
## \#10 Posted by: Randyc1 Posted at: 2016-08-09T21:33:15.493Z Reads: 668

```
Does the fuse need to handle (Max Continuous A ) or Max A  of the Cell ....

 example:  (20A C vs 30A)
```

---
## \#11 Posted by: MrEpiquad Posted at: 2016-08-09T21:44:17.259Z Reads: 662

```
Awesome idea and great design !
Do you mind sharing telling what material the wire is made of ?
And how it will be connected to the cell and the strips ?
```

---
## \#12 Posted by: chaka Posted at: 2016-08-09T21:44:42.520Z Reads: 670

```
Let me know when you find an 18650 cell that can do 30 amps continuous. :) If you size the fuse too high it defeats the purpose of the fuse. If you are pulling 6000 watts constant from a 12s6p pack then you should probably switch to prismatic lipo's. High discharge 18650's shouldn't really be driven too close to their max constant rating. This chart gives you an ide of what happens and the level of voltage sag you can see at different loads. With voltage sag you will also see massive heat buildup.

http://lygte-info.dk/pic/Batteries2012/LG%2018650%20HE4%202500mAh%20(Yellow)/LG%2018650%20HE4%202500mAh%20(Yellow)-Capacity.png
```

---
## \#13 Posted by: chaka Posted at: 2016-08-09T21:49:14.957Z Reads: 652

```
> Do you mind sharing telling what material the wire is made of ?
> And how it will be connected to the cell and the strips ?

The fuse wire is nickel plated copper and they are soldered to the underside of the buss bar. Not shown in the photo is the welded nickel tabs, after they have been spot welded the cell fuse is soldered to the tabs.
```

---
## \#14 Posted by: Randyc1 Posted at: 2016-08-09T21:50:49.184Z Reads: 638

```
I meant a cell like the LG HG2 is good for 20A cont. or 30 A peak .
```

---
## \#15 Posted by: MrEpiquad Posted at: 2016-08-09T21:56:29.212Z Reads: 629

```
Thanks @chaka

Maybe you could apply this to largers cells like the A123 systems ANR26650M1-B 2500mAh which can do up to 70A.

And just one final question if you don't mind. 
Did you do tests on when these nickel plated copper wires break at a certain current and did you put that into a formula ?
```

---
## \#16 Posted by: chaka Posted at: 2016-08-09T21:56:58.434Z Reads: 624

```
The fuses are essentially "slow blow", meaning small peaks will not cause the fuse to break circuit. Even a direct short on the mains takes a bit of time before the fuses start popping off.  Look at that chart and you will see that individually the cells drop below 3.3v right away at 20 amps. Best to build a bigger pack or switch to A123's and higher gauge fuses if you need that much power.
```

---
## \#17 Posted by: Randyc1 Posted at: 2016-08-09T22:03:12.676Z Reads: 611

```
I really don't know how  many Amps my Single pulls, i just read about people here saying sometimes they are pulling like 60A going up hill ?
```

---
## \#18 Posted by: Kaly Posted at: 2016-08-09T22:04:16.350Z Reads: 612

```
The cell fuse idea in itself is great and the implementation that you have done here is superb in its simplicity.

But @chaka what implementation do you have for knowing when a fuse have blown once the pack is sealed ?
```

---
## \#19 Posted by: CSN Posted at: 2016-08-09T22:11:17.581Z Reads: 615

```
I think this is really important for DIY crowd to get these packs designed well.

What about OBC offering some kind of affiliate program that certifies reliable and safe pack design? 

Maybe call it high performance standards or something.

Wouldn't need to be expensive but would give buyers more confidence if they knew their expensive pack were going to last more 6 months to 1 year because it was reviewed by an respected designer.

Could also increase the expertise out there to use reclaimed batteries from laptops to make affordable large packs.
```

---
## \#20 Posted by: chaka Posted at: 2016-08-09T22:17:16.222Z Reads: 616

```
That is one of the great aspects of these styles of pack. A failed cell doesn't cripple your ride, you can still make it home if something goes wrong. Clear heat-shrink allows for easy inspection if you notice a loss of range or an unbalanced pack.

@CSN Tesla has already set the standard with this type of assembly. Unless you think Tesla Motors isn't well respected? ;)
```

---
## \#21 Posted by: Namasaki Posted at: 2016-08-09T22:26:22.046Z Reads: 557

```
On the cutting edge of battery technology
```

---
## \#22 Posted by: VladPomogaev Posted at: 2016-08-09T22:31:02.517Z Reads: 570

```
How are you going to attach the fuses to the cells themselves?
```

---
## \#23 Posted by: Nordle Posted at: 2016-08-09T22:32:54.053Z Reads: 582

```
Can you tell me where i can get fuse wire?
```

---
## \#24 Posted by: CSN Posted at: 2016-08-09T22:55:21.788Z Reads: 596

```
This is pretty interesting video about cell level fusing with a lot of explanation.

https://www.youtube.com/watch?v=raBWFsPlx7w

and another

https://www.youtube.com/watch?v=HR4pWQjDATc
```

---
## \#25 Posted by: karma Posted at: 2016-08-09T22:55:31.360Z Reads: 577

```
Alright, nickel plated copper wires that has to be adjusted to your batteries and setup so that the fuses blow when it draws too many amps but not when on normal load. Did I get this right? Seems straight forward but those 18650 spacers were really nice, are there space between the cells, couldn't tell in the pictures. If not I would suggest getting a little bit of room between them to help cooling. Awesome as always @chaka, keep it up :)
```

---
## \#26 Posted by: Nordle Posted at: 2016-08-09T23:00:18.634Z Reads: 555

```
So i have to try myself and find the right wire... ?
```

---
## \#27 Posted by: jrpwit Posted at: 2016-08-09T23:11:26.881Z Reads: 555

```
Nice vid @CSN 

I want to try and include fuses on my 8s3p pack I'm working on but would the fuses create a lot of heat if you pull like 20 amps going up a hill? I dont know a lot about fuses but I would assume the heat would decrease the life of the cells. Is that right or just total crazy talk? I also wouldnt have much to lose cause my pack is made of only 24 cells but the extra protect wouldnt hurt.
```

---
## \#28 Posted by: chaka Posted at: 2016-08-09T23:16:13.489Z Reads: 550

```
I get mine from http://www.remingtonindustries.com/
```

---
## \#29 Posted by: chaka Posted at: 2016-08-09T23:20:05.143Z Reads: 540

```
I wouldn't use this method On an 8s3p unless you also add a 60 amp fuse to your main terminals. Still 8s3p is a little too small for comfort.
```

---
## \#30 Posted by: sl33py Posted at: 2016-08-09T23:24:26.221Z Reads: 543

```
@Chaka - seriously impressive.  Hats off to you Sir!

Does this also simplify your soldering - so you don't need a spot welder to make your pack?  I've been contemplating building a 18650 pack and the cost of a decent spot welder has been prohibitive.

where do i click to give a gold star... hehehe
```

---
## \#31 Posted by: chaka Posted at: 2016-08-09T23:48:16.411Z Reads: 525

```
I spot weld tabs and solder to the tabs but you could solder directly to the cell if you have a big soldering iron, 80+ watts.
```

---
## \#32 Posted by: sl33py Posted at: 2016-08-10T00:17:17.936Z Reads: 513

```
Thanks man - great of you to share your process and even materials.

Do you have any pics of how you solder and spot weld these to the 18650 cell?  I'm not visualizing this well - not much surprise as my 18650 pack experience is nil.
```

---
## \#33 Posted by: Jinra Posted at: 2016-08-10T00:18:34.853Z Reads: 508

```
Check out the video @csn linked to above, it gives you a pretty good idea how it's attached.
```

---
## \#34 Posted by: chaka Posted at: 2016-08-10T01:39:32.899Z Reads: 519

```
I'm uploading the cell holder .stl file on thingiverse, it will be 24 hours before I can publish. Send me a pm if you can't wait and need it now!
```

---
## \#35 Posted by: mishrasubhransu Posted at: 2016-08-10T02:14:49.924Z Reads: 519

```
So Tesla's batteries are also designed like this?
```

---
## \#36 Posted by: michaelcpg Posted at: 2016-08-10T02:21:55.789Z Reads: 527

```
Pretty much

<img src="/uploads/db1493/original/2X/a/ae1ceb5f2af952289c6eb7a0d1b2e7f223a3b760.jpg" width="690" height="388">
```

---
## \#37 Posted by: mishrasubhransu Posted at: 2016-08-10T03:07:24.183Z Reads: 517

```
Just using a normal wire won't be very efficient, I am guessing. Ideally it shouldn't produce any heat when operating below the max current, but above that current it should produce a lot of heat and melt off. @chaka are you using some specific fuse material or just wire that you found appropriate for the current?
```

---
## \#38 Posted by: Michaelinvegas Posted at: 2016-08-10T03:12:53.604Z Reads: 513

```
Very clean ... Nice design
```

---
## \#39 Posted by: mishrasubhransu Posted at: 2016-08-10T03:25:49.955Z Reads: 526

```
Found some more images online for the tesla battery pack

<img src="/uploads/db1493/original/2X/2/27d4fbae76f80468347f8ad5c95a5ef690a4e004.jpeg" width="690" height="387">
<img src="/uploads/db1493/original/2X/4/49a8173983a6e4f360a2d2c9138d9d63a0f4786c.jpeg" width="690" height="387">
<img src="/uploads/db1493/original/2X/3/3f3b3f84d20a6716a87794b1db18eb4915595236.jpg" width="496" height="500">
```

---
## \#40 Posted by: Eboostin Posted at: 2016-08-10T03:50:19.960Z Reads: 509

```
That last pack is pretty interesting. Surprised they solder rather than spot weld.
```

---
## \#41 Posted by: Pantologist Posted at: 2016-08-10T03:54:15.316Z Reads: 498

```
I'm not sure that is official Tesla.
```

---
## \#42 Posted by: Jinra Posted at: 2016-08-10T04:27:21.034Z Reads: 497

```
Current will always bring heat, and heat is what triggers fuses, so using a wire as the fuse is fine. In fact the reason fuses trip in the first place is because they surpassed a temperature ceiling.
```

---
## \#43 Posted by: lox897 Posted at: 2016-08-10T04:35:04.258Z Reads: 496

```
Where do you get the tabs for the cells? You have a talent for building packs. Awesome job!
```

---
## \#44 Posted by: Titoxd10001 Posted at: 2016-08-10T07:35:47.793Z Reads: 502

```
Would this type of fuse setup be good for a 12s4p pack?
```

---
## \#45 Posted by: michaelcpg Posted at: 2016-08-10T08:22:46.256Z Reads: 502

```
From my understanding, it shouldn't really matter too much what size battery pack you use as long as you use fuse wire appropriate to the current rating of your cells. I'm using a very similar design to @chaka's (although definitely not quite as professional looking with his custom 3D printed enclosures) and have had no issues. I've got a 10S4P pack. In my case, I'm using 20A fuse wire with LG HE4 cells which are rated at 20A continuous discharge.
```

---
## \#46 Posted by: Nordle Posted at: 2016-08-10T08:32:54.945Z Reads: 496

```
So i'd like to use 20A cells, therefore i'd like to use ~25A fuse wire. Someone knows what awg that would be?:)
```

---
## \#47 Posted by: Randyc1 Posted at: 2016-08-10T13:57:07.166Z Reads: 476

```
Did you have a build thread of this 10s4p battery , we would love to how this was built ?
```

---
## \#48 Posted by: chaka Posted at: 2016-08-10T14:13:17.129Z Reads: 475

```
It really depends on your supply, I have had to test every spool to get my own specs. There is some variance from one supplier to the next. Somewhere in the range of 22-24 gauge should do it. You can also use resistor legs but they vary greatly in spec, some blow faster than others.
```

---
## \#49 Posted by: longhairedboy Posted at: 2016-08-10T14:30:08.547Z Reads: 468

```
could a similar approach be used with a slightly heavier gauge wire in order to better distribute the load but not act as cell level fusing? I really like what's happening here.
```

---
## \#50 Posted by: chaka Posted at: 2016-08-10T14:56:40.476Z Reads: 496

```
That would defeat the purpose of the cell level fusing. They do not distribute the load any better than nickel strip, although the brass buss bar is less resistive than thin nickel strip. What cell level fusing does is prevent thermal runaway should a single cell become damaged resulting in increased resistance. If a cell is allowed to draw unlimited current it will also heat up the neighboring cells which causes their resistance to also go up resulting in a cascading effect. 

This construction is more about safety of the battery and rider rather than an increase in performance. 

Grin tech filmed a resistive load test to see what happens when a sealed 10s1p  pack goes into thermal runaway. 

https://www.youtube.com/watch?v=oBlac5gWLfI
```

---
## \#51 Posted by: longhairedboy Posted at: 2016-08-10T15:06:02.726Z Reads: 485

```
holy crap!
```

---
## \#52 Posted by: Nordle Posted at: 2016-08-10T18:55:16.011Z Reads: 482

```
How did you test those wires? Do i need such a big power supply or is there a trick i dont know maybe?
```

---
## \#53 Posted by: michaelcpg Posted at: 2016-08-10T21:34:50.132Z Reads: 495

```
No build thread sorry, didn't end up taking many photos. Here's a couple I took fairly early on though showing how I soldered the fuse wires. 

<img src="/uploads/db1493/original/2X/5/55e8f647a41845fce196a3341d9571691c0226ee.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/f/fb87c8597db89a7de6bc78bb63ca198525aba8a2.jpg" width="690" height="388">

My original plan was to build 5 separate 2S4P packs that could be connected together in series via bullet connectors so that I could pull the battery apart and take my board on a plane. However I ended up getting impatient waiting for a few things to arrive and ended up just wiring it all together into a single pack :p 

I'm going to pull the whole thing apart at some point when I've got some time and do redo my original modular idea but the main issue I'm having atm is deciding how best to secure the batteries together. Currently they're just hot glued but I'm trying to find a more permanent solution that better handles the vibration without making the pack longer as I don't have any more free space in my space cell enclosure. I might look at replacing the black wires with slimmer, flat brass rods or similar to reduce the thickness of the pack as well.
```

---
## \#54 Posted by: Nordle Posted at: 2016-08-10T21:44:49.335Z Reads: 470

```
Where did you find the right wire?
```

---
## \#55 Posted by: michaelcpg Posted at: 2016-08-10T21:50:53.567Z Reads: 472

```
A local electronics wholesaler had a range of different sized fuse wires with various current ratings
```

---
## \#56 Posted by: Randyc1 Posted at: 2016-08-10T22:13:32.495Z Reads: 461

```
Do big name companies like Boosted and Evolve use this technique,.. Hmmmmm ??
```

---
## \#57 Posted by: Jinra Posted at: 2016-08-10T22:21:10.206Z Reads: 467

```
Pretty sure my Evolve battery doesn't have this. I don't think it's used much in ESK8 since it's designed for saving parallel cells and we typically don't have that many cells in parallel. chaka likes to use larger parallel packs so his implementation makes more sense. Boosted runs 12s1P I believe which doesn't need cell level fusing.
```

---
## \#58 Posted by: racidon Posted at: 2016-08-10T23:02:26.218Z Reads: 473

```
Instead of guessing/calculating the amperage of wire. Why not buy actual fuse wire like the following:
https://www.bunnings.com.au/hpm-8amp-16amp-fuse-wire-card_p4331623

It's still used in some houses today and it's only downfall was that you had to replace it instead of flick a switch as is used today in homes.
With that said too. Has anyone thought of using trip switches?
```

---
## \#59 Posted by: Kaly Posted at: 2016-08-11T03:05:46.253Z Reads: 467

```
For holding the cells in place why don't you use fiberglass reinforce tape, it is thin and can hold the cells nicely.
```

---
## \#60 Posted by: michaelcpg Posted at: 2016-08-11T04:21:10.375Z Reads: 464

```
https://www.bunnings.co.nz/sika-fiba-tape-48mmx-15-2m_p00179289
Something like this?
```

---
## \#61 Posted by: lox897 Posted at: 2016-08-11T07:17:07.718Z Reads: 453

```
[quote="lox897, post:43, topic:7392, full:true"]
Where do you get the tabs for the cells?
[/quote]

Bump @chaka thanks
```

---
## \#62 Posted by: Nordle Posted at: 2016-08-11T09:57:47.592Z Reads: 443

```
i bought [such a wire](https://www.amazon.co.uk/ELECTICAL-FUSE-WIRE-30AMP-CARD/dp/B0030E3L5E) now, hope the 30A one works fine for my next 25r or HG2 pack, both 20A cells.
```

---
## \#63 Posted by: chaka Posted at: 2016-08-11T13:23:42.293Z Reads: 445

```
We cut them from nickel strips.  

If you build a pack like this be sure the buss bars are insulated from the cells. Before 3d printing holders used fishpaper for this.
```

---
## \#64 Posted by: evoheyax Posted at: 2016-08-11T15:58:53.398Z Reads: 446

```
I'm a bit confused maybe on the gauges needed in these packs. I'm building a 10s4p pack right now from LG HE2 cells and according to their rating, I can do 20 amps per cell. I plan on drawing up to 80 amps (probably a bit lower to lower the sag). From researching many charts, it seems like 10 gauge can do 80 amps without too much heat, 8 gauge can do 100 amps with little heat. Should I be using 8 (or 10) gauge wire (or stripping equal to 8/10 gauge) through out the entire pack? You say 20 amp fuses, but none of us are pulling only 20 amps as a max. I think my image of how the electricity flows in a battery pack might be wrong.
```

---
## \#65 Posted by: paragon Posted at: 2016-08-11T16:22:55.201Z Reads: 430

```
cells in parallel share the load

if you are using he2 cells in a 10s4p pack, each cell will provide 20a continuous (total of 80a) when needed, so 20a fuses on each cell are fine (if you draw more, it is unhealthy for the battery, and the fuses will burn to protect your cells).
```

---
## \#66 Posted by: Kaly Posted at: 2016-08-11T16:37:47.455Z Reads: 435

```
Remember this is a precausumary method the lg hg2 can discharge 20A constant and 30A burst. So you will want your fuse to be for 35amps other wise you'll be blowing fuses within the normal operational range of the battery.
```

---
## \#67 Posted by: chaka Posted at: 2016-08-11T16:45:15.674Z Reads: 429

```
Those ratings are for open air, these fuses are attached to infinite heat sinks so they will handle higher currents than those spec sheets state. If the fuse is too large then you can still get a thermal runaway.
```

---
## \#68 Posted by: mishrasubhransu Posted at: 2016-08-11T17:51:33.645Z Reads: 431

```
One important thing to consider is the heat wasting part of this arrangement should be as small as possible. That's why you see that the fuse box is cars have such small fuse element.  Here's my analysis.

For this analysis we consider that thick wires have **0** Ohms per cm and the fuse wire have resistance **r** Ohms per cm.  Heat energy wasted per unit time **I^2*R** (I: current R: total resistance). 

Say you pick 2 fuse wire with the same Ohms per cm (1ohm/cm) and both melt when 5 A current passes through them. However one is  2 cm long and the other 1 cm long. You will see that they both work when passing under 5A of current and both burnout at more than 5A, however the heat wasted through 1st one is 5(A)*5(A)*1(ohm/cm)*2(cm)=50Watts where as the 2nd one wastes 5(A)*5(A)*1(ohm/cm)*1(cm)=25Watts. 

So basically if you want to not wasted your precious battery capacity as heat, use small length fuse wire.

If I were to design my own battery pack, I would try to integrate the car fuses. They are easy to replace, safe(enclosed) and very cheap. You can get a 20Amp one from [here](http://www.kinequip.com/fuse-atm-20-optifuse.html) for $0.13
```

---
## \#69 Posted by: chaka Posted at: 2016-08-11T18:30:47.079Z Reads: 411

```
The design I have works very well and the fuses do not get hot under heavy discharge. Real world testing has always given me the best results vs speculation. I have been working on this design for nearly a year. :wink:
```

---
## \#70 Posted by: sl33py Posted at: 2016-08-11T20:00:12.579Z Reads: 421

```
Thanks for sharing this info to the community @Chaka!  Really elegant design and execution it seems.  The part i want to confirm here is how do you connect fuse wire to the cell top?  Is it just left pressing against the flat/button top of the cell, or soldered?  And the fuse wire to the back of the nickel bar - assuming it's held in place with solder?

I'm still trying to figure out how to wire these for balance charging - any completed pack *before shrink wrap* to reference?  

Do you sell just the 18650 holders by chance?  

Over a year on the design... damn man - thanks for your insight and giving back to the community!  Saves us a ton of time figuring it out ourselves...
```

---
## \#71 Posted by: chaka Posted at: 2016-08-11T20:37:57.862Z Reads: 406

```
I'll post some photos soon of the completed pack, it should be clear once you see the details. I need to finish another project before I can clear our battery assembly area and build more packs. Never enough space!

If you have your 3d printer up and running I can share my stl files with you.
```

---
## \#72 Posted by: Ulfberht Posted at: 2016-08-11T21:39:52.433Z Reads: 401

```
This is awesome. :astonished:Just freaking awesome.... This is clearly going to be the new standard of excellence. 
@chaka Thank you so very much for sharing your design! Those cell holders are over the top. Too cool.
I have a quick question about the nickel strips that you are using. Why are you not just soldering the fuse wires to the cells? Is it so that you can have a tab to solder to that isn't directly on the cell? For ease of maintenance?
```

---
## \#73 Posted by: chaka Posted at: 2016-08-16T23:51:26.236Z Reads: 402

```
Uploaded the latest .stl files to Thingiverse: http://www.thingiverse.com/thing:1712459

If anyone needs a lower or higher number of cells in parallel let me know and I will put it on my list of things to do. ;)
```

---
## \#74 Posted by: Pantologist Posted at: 2016-08-16T23:52:36.236Z Reads: 400

```
3 cells in parallel would be nice.
```

---
## \#75 Posted by: michaelcpg Posted at: 2016-08-16T23:57:38.846Z Reads: 407

```
4p would be awesome too :)
```

---
## \#76 Posted by: treenutter Posted at: 2016-08-17T02:41:22.395Z Reads: 418

```
Thanks so much for sharing this @chaka! The question this leaves me asking is how likely thermal runaway is with the commom cells that we see in use right now (18650)? What has to happen to push these cells to this point? Assuming they are authentic cells and that they wired and charged properly, is the risk great enough to warrant the additional complexity of the battery build? 

I agree that this might become a new standard for esk8 and I fully appreciate that you've shared your design, it's an earnest expression of your commitment to open-source thinking!
```

---
## \#77 Posted by: michaelcpg Posted at: 2016-08-17T03:22:08.164Z Reads: 413

```
While I can't answer most of your questions I can chime in on a few things. 
One advantage of fuse wires is that, if you're soldering your cells, using fuse wires makes the process much easier and is better for your battery as opposed to trying to solder thicker wire directly to the cells as less heat is involved.
I've had a couple of fuses break on two occasions while I've been riding due to riding on extremely rough roads with really hard wheels and the fact that my current battery pack needs to be redesigned as it's been a temporary build while I'm working on a modular design for taking my board on planes. In my case I have a 10s4p pack with two fuse wires breaking on a single 4p pack and it had no noticeable effect on the battery in the short period that I rode it afterwards. As long as you have enough cells in each parallel pack to handle the current then I don't think it should really be an issue, at least for short term use. I only realised what had happened after plugging my board in to charge and finding that I wasn't able to fully charge my board.
```

---
## \#78 Posted by: Titoxd10001 Posted at: 2016-08-17T03:55:56.888Z Reads: 394

```
Fuse wire failed due to vibration?
```

---
## \#79 Posted by: michaelcpg Posted at: 2016-08-17T04:10:47.910Z Reads: 401

```
More that the hot glue holding the cells together came unstuck due to vibration, allowing the cells to move about a bit and eventually break the fuse wires. When the cells are properly secured this should never really be an issue.
```

---
## \#80 Posted by: Titoxd10001 Posted at: 2016-08-17T04:15:04.540Z Reads: 401

```
Okay I might do the fuse wire for my next build with the cells stuck to the board with double side tape
```

---
## \#81 Posted by: andysurfs Posted at: 2016-08-17T04:58:39.748Z Reads: 374

```
+1 on the 3P design - I was about to start a spot weld a 10S3P battery pack this weekend, but thanks to @chaka 's magnificent efforts, I am going to rethink and give cell level fuse wiring a go.
```

---
## \#82 Posted by: Randyc1 Posted at: 2016-08-17T12:24:34.457Z Reads: 376

```
2 questions , 

How do you know when 1 fuse (wire) is blown ?

Is only the the thin Nickel strip handelling all the Current (30-60A) on the Series connections ??
```

---
## \#83 Posted by: chaka Posted at: 2016-08-17T13:21:33.424Z Reads: 395

```
I use 1/2 inch brass strip instead of nickel. I little more expensive but it handles the current much better with less resistance. You can also use clear heat shrink if you want to be able to inspect the pack for blown fuses but an out of balance pack is another sign that would let you know.

@treenutter Over discharging can lead to thermal runaway as well as damage or overcharging.
```

---
## \#84 Posted by: andysurfs Posted at: 2016-08-17T13:42:49.108Z Reads: 393

```
@chaka do you advocate using a BMS with this battery pack configuration, or is it possible to avoid using one, in the way @whitepony does with his builds (where cell drift doesn't seem to be an issue over time)?
```

---
## \#85 Posted by: chaka Posted at: 2016-08-17T14:14:41.271Z Reads: 402

```
I always recommend using a bms, trouble is if you use a cheap bms it can lead to headaches. Thats the main reason BMS units have had a bad reputation.

Running without a bms is risky business, I know @whitepony has popularized this idea but even he has had some close calls with over discharge draining the pack too low.

Ideally we will have a programmable BMS, this is actually something in development, it will allow for a much nicer method of protecting our packs.
```

---
## \#86 Posted by: whitepony Posted at: 2016-08-17T20:09:55.082Z Reads: 393

```
[quote="chaka, post:85, topic:7392"]
Running without a bms is risky business, I know @whitepony has popularized this idea but even he has had some close calls with over discharge draining the pack too low.
[/quote]

well, to be fair, I only discharged cells to 2.5V because of a bug I uncovered in the torqueboard 12S ESCs. after I started using vescs, I never had any problem anymore. my evolve battery is still reaching 50km range after 1.5 years and I still couldnt measure any drift. same thing for all my other batteries.

nevertheless, I still agree with you though - I would never advise anyone to run without a BMS unless you feel very confident that you know exactly what youre doing, i.e. you should know very well whats good and whats bad for cells. I think its very important to avoid any battery abuse - temperature, excessive load or maxed out charge and discharge cycles.
```

---
## \#87 Posted by: Ulfberht Posted at: 2016-08-17T21:09:30.043Z Reads: 371

```
[quote="chaka, post:83, topic:7392"]
I use 1/2 inch brass strip instead of nickel. I little more expensive but it handles the current much better with less resistance
[/quote]

Would it also be doable to just use 10AWG wire and solder the fuse wires directly? Is there a disadvantage to this method?
```

---
## \#88 Posted by: chaka Posted at: 2016-08-17T21:15:11.455Z Reads: 362

```
Brass strips keep it thin and is easy to secure.
```

---
## \#89 Posted by: Jinra Posted at: 2016-08-17T21:16:20.819Z Reads: 355

```
Where do you source your brass strips if you don't mind me asking?
```

---
## \#90 Posted by: chaka Posted at: 2016-08-17T21:17:08.473Z Reads: 356

```
If you are looking for a small supply you can find them on ebay.
```

---
## \#91 Posted by: sl33py Posted at: 2016-08-17T21:32:35.647Z Reads: 365

```
[quote="chaka, post:83, topic:7392"]
I use 1/2 inch brass strip instead of nickel. I little more expensive but it handles the current much better with less resistance.
[/quote]


Same .15 thickness, or what thickness do you recommend?

I'm pretty sure i finally have the connections visualized, but if you have a pic of the finished pack before shrink - that'd be great!

Thanks so much @chaka!  This is fantastic info and really helpful.
```

---
## \#92 Posted by: chaka Posted at: 2016-08-17T21:34:37.882Z Reads: 356

```
You don't need it that thick. I think you can take it down to .016 inch thick at 10s.
```

---
## \#93 Posted by: Eboostin Posted at: 2016-08-17T22:25:55.298Z Reads: 354

```
Do you have any plans to make a holder for density packing? @chaka
```

---
## \#94 Posted by: chaka Posted at: 2016-08-17T22:57:29.881Z Reads: 363

```
I have a project on the back burner right now that will have around 150 cells stacked in a staggered pattern. It's just a personal project so I haven't been able to give it any time lately. I plan to ride from San Diego to San Francisco stopping a couple times a day to recharge and hitting a few camp sites along the coast. Once I start working on it again I'll post the files for the holders.
```

---
## \#95 Posted by: Jinra Posted at: 2016-08-17T22:58:44.175Z Reads: 360

```
Let me know when you stop by SF!
```

---
## \#96 Posted by: Ulfberht Posted at: 2016-08-18T06:50:26.131Z Reads: 360

```
[quote="chaka, post:94, topic:7392"]
I plan to ride from San Diego to San Francisco stopping a couple times a day to recharge and hitting a few camp sites along the coast.
[/quote]

That would be an incredible ride. Are you going to take Hwy 101? It's an amazing drive up from San Diego, it would be a stellar ride.
```

---
## \#97 Posted by: Okami Posted at: 2016-08-18T07:34:45.555Z Reads: 380

```
Some cool ideas on this thread. Thanks for sharing and starting a conversation @chaka

Anyways, I think I came up with an idea how not to damage cells by soldering:

[quote="michaelcpg, post:77, topic:7392"]
One advantage of fuse wires is that, if you're soldering your cells, using fuse wires makes the process much easier and is better for your battery as opposed to trying to solder thicker wire directly to the cells as less heat is involved.
[/quote]



So the soldering iron should be only powerful enough to solder the small fuse wire to the bus bar, hence the cell won't receive a lot of heating and the only heat requiring place will be the solder point between bus bar and fuse wire.

Smart to find this out, will probably try this method and avoid soldering big wires to the cells directly. 2 in 1 solution, if you ask me.
```

---
## \#98 Posted by: chaka Posted at: 2016-08-18T07:52:27.233Z Reads: 364

```
It will be! I am going to attempt an average speed of 30 mph. Hoping to get over 50 miles of range at that pace. Haven't mapped out the route yet but will definitely be hugging the coast. I think it is about 580 miles total. 

@Okami If you use a powerful iron you can quickly wet the ends of the cells with solder in preparation for the fuse wire and then come back with the same iron and solder the fuse wire to the pre-tinned ends of the cells. The object of the procedure is to be quick. Might not be a bad idea to have a wet sponge on hand to cool the ends once you finish soldering each cell.
```

---
## \#99 Posted by: Okami Posted at: 2016-08-18T08:04:28.812Z Reads: 372

```
[quote="chaka, post:98, topic:7392"]
@Okami If you use a powerful iron you can quickly wet the ends of the cells with solder in preparation for the fuse wire and then come back with the same iron and solder the fuse wire to the pre-tinned ends of the cells. The object of the procedure is to be quick. Might not be a bad idea to have a wet sponge on hand to cool the ends once you finish soldering each cell.
[/quote]

That's a good tip. Was rather easy to solder a small wire to AA cell this way. I hope it goes similar with soldering to 18650's.
```

---
## \#100 Posted by: michaelcpg Posted at: 2016-08-18T08:54:22.779Z Reads: 358

```
Make sure to use flux :)
```

---
## \#101 Posted by: mason Posted at: 2016-08-18T12:00:25.859Z Reads: 338

```
bring a couple of solar panels and batteries!
```

---
## \#102 Posted by: sl33py Posted at: 2016-08-19T01:29:27.934Z Reads: 349

```
Sounds bucket-list epic man!  Hope you take lots of pics to share the adventure with the rest of us!

12 days of riding minimum - you will have iron legs at the end of it!  Wow - can't wait to hear about the trip and experience!
```

---
## \#103 Posted by: michaelcpg Posted at: 2016-08-21T22:11:36.057Z Reads: 357

```
Hey @chaka, what software did you use to make this? I'm sure you're super busy so I might have a go at modifying your design for 4p
```

---
## \#104 Posted by: chaka Posted at: 2016-08-24T02:50:48.086Z Reads: 373

```
 Added a 4p holder to our thingiverse page: http://www.thingiverse.com/thing:1712459
I will add more variations when I have time. ;)

http://thingiverse-production-new.s3.amazonaws.com/renders/24/f9/4a/3b/0d/5595fe4d00a906106bc1f1b83ff2ea0b_preview_featured.jpg

Let me know how it works for you @michaelcpg 

I made the files on FreeCad.
```

---
## \#105 Posted by: andysurfs Posted at: 2016-08-24T03:34:48.351Z Reads: 357

```
Hi @chaka, thanks for putting up the 4P holder. I am ready to go building my 10S 3P battery, and was wondering whether I could just get the your 6P holder at the top of this thread printed and then just cut them in half to suit 3P? It would mean one side would not be held in exactly, but I reckon I could sort it out with tape.
```

---
## \#106 Posted by: DeathCookies Posted at: 2016-08-24T06:04:14.475Z Reads: 345

```
I am Interessted in 8P and maybe 10P :smiley: Would be nice if you could share them too!
```

---
## \#107 Posted by: Jinra Posted at: 2016-08-24T06:06:06.363Z Reads: 341

```
10P?? How would you even fit that on a board unless you ran 6s.
```

---
## \#108 Posted by: DeathCookies Posted at: 2016-08-24T06:21:02.890Z Reads: 345

```
Pneumatic tires ;)
```

---
## \#109 Posted by: Jinra Posted at: 2016-08-24T06:23:33.730Z Reads: 353

```
I'll be honest, that would be an insane pack at 10s10p. I would love to see that
```

---
## \#110 Posted by: andysurfs Posted at: 2016-08-24T09:42:28.346Z Reads: 366

```
Thanks @chaka for sharing the design files for the cell holder. I just had a guy modify them for the 3P arrangement and he is printing up 10 of them for me now. Battery building on the weekend - Yew! 

<img src="/uploads/db1493/original/2X/3/38da9b04b9a4500334742623f7ce8c77feb9d1ce.jpg" width="595" height="494">
```

---
## \#111 Posted by: chaka Posted at: 2016-08-24T14:06:28.342Z Reads: 352

```
I'll spend an evening soon and produce as many variations as I can. 

@andysurfs  you will need 20 of them for 10s pack. ;)
```

---
## \#112 Posted by: andysurfs Posted at: 2016-08-24T14:42:09.000Z Reads: 344

```
Thanks @chaka. Yeah, I realised my mistake just after I posted. I've got 20 being made at the moment at $2/ea .
```

---
## \#113 Posted by: monkey32 Posted at: 2016-08-24T20:26:54.630Z Reads: 338

```
Chaka for president!!!!!!! Awesome thread thanks for sharing the design.
```

---
## \#114 Posted by: HTownBomber Posted at: 2016-08-24T20:45:05.730Z Reads: 342

```
A word of advice if you do that trip: take the bus up and ride down. The wind blows predominantly south down the CA coast. You don't want to ride 580 miles against headwinds.
```

---
## \#115 Posted by: oneafrikan Posted at: 2016-08-24T21:11:26.577Z Reads: 351

```
this is an awesome thread for someone new to this.

one of the things holding me back from trying to build my own battery pack ala @whitepony is that I don't have a spot welder lying about, and my wife will veto that once she knows what it's for (think toddler with wires in mouth one Saturday afternoon - well, that's what she's thinking!).

but from what i've picked up here soldering would work too, using a fuse wire?  i know that's super basic, but is it literally:

a) get your cells together
b) put a sled together in right config
c) solder fusewire to the batteries
d) solder fusewire to a thicker thread between batteries
e) attach to BMS etc
f) clean up and shrink wrap

obviously more in that, and a lot of the details discussed above, but that's the process, right?

Disclaimer: I work in spreadsheets most of my days, did Zoology at University, and kinda spent Chemistry getting drunk for a few years... so this is the first time i've touched battery theory since about 1997.  so be gentle ;-)
```

---
## \#116 Posted by: chaka Posted at: 2016-08-24T21:28:09.485Z Reads: 336

```
Better view too! Nothing set in stone yet so thanks for the recommendation. Hoping to show what is possible on a high performance ULEV so fighting a headwind might be better.
```

---
## \#117 Posted by: makevoid Posted at: 2016-08-25T10:37:28.367Z Reads: 328

```
you don't need a spot welder to do just one pack, order the cells with solder tabs on and use a normal iron to solder the cells, the price per cell will be higher  (+0.40 eur per cell on nkon.nl) but for one pack will be ok
```

---
## \#118 Posted by: mason Posted at: 2016-08-25T11:46:48.764Z Reads: 325

```
Make sure the iron is 70w+ to be quick and not damage the cells with heat.
```

---
## \#119 Posted by: andysurfs Posted at: 2016-08-25T13:19:33.354Z Reads: 332

```
Any advice guys on directly soldering fuse wire to the top of cells? Is it possible to do so if you use flux and directly solder with a powerful iron? Was hoping to avoid having to weld nickel tabs onto my LG HG2's before soldering the fuse wire on.
```

---
## \#120 Posted by: kovjanos Posted at: 2016-08-25T13:24:02.183Z Reads: 336

```
What about soldering the wire to a small piece of plate and then spot-welding the plate to the cell?

R, J.
```

---
## \#121 Posted by: chaka Posted at: 2016-08-25T13:27:29.274Z Reads: 310

```
Never spot weld "after" soldering! You will create dangerous fumes since the act of spot welding is much hotter than soldering. All soldering operations need to be after you have spot welded the tabs.
```

---
## \#122 Posted by: longhairedboy Posted at: 2016-08-25T13:35:36.127Z Reads: 316

```
also its difficult to solder directly on a spot weld, just thought i'd throw that in there. soldering right next to one is a easy though. I guess because the metal changes slightly or something.
```

---
## \#123 Posted by: kovjanos Posted at: 2016-08-25T13:37:53.712Z Reads: 323

```
Other than that? I mean in a well vented environment with proper safety those could be handled and would still prevent the cell from the soldering iron’s heat. 
Or the only option is to use proper soldering iron as even tabs spot welded to the cell would transfer heat to the cell, right?

Thanks, J.
```

---
## \#124 Posted by: chaka Posted at: 2016-08-25T13:45:32.743Z Reads: 344

```
Tabs are very thin in comparison to the cells so the soldering take much less heat than if you were to solder directly to the cell.
```

---
## \#125 Posted by: Jinra Posted at: 2016-09-07T12:37:34.520Z Reads: 360

```
About to start my first cell fused pack. Found this great resource for approximating current required to trip various wires.

http://www.powerstream.com/wire-fusing-currents.htm
```

---
## \#126 Posted by: andysurfs Posted at: 2016-09-07T14:17:13.263Z Reads: 365

```
Thanks @Jinra, that's a really helpful resource! Getting fuse wire is the last step to building my 10S 3P battery out of LG HG2's. The LG's have a rated max discharge of 20A, but I think I'll go with 30A rated copper wire (the cell holders are made out of glow in the dark plastic... unecessary, but awesome... )

<img src="/uploads/db1493/original/3X/3/9/398af73fc49f1e58467eb31d99818030da76df33.jpg" width="666" height="500">
```

---
## \#127 Posted by: Eboostin Posted at: 2016-09-07T14:18:53.728Z Reads: 354

```
Please post lots of assembly pics! :slight_smile:
```

---
## \#128 Posted by: chaka Posted at: 2016-09-07T14:21:50.097Z Reads: 353

```
You wont need those gaskets with the cell holders. ;)
```

---
## \#129 Posted by: andysurfs Posted at: 2016-09-07T14:25:28.023Z Reads: 355

```
Yeah, the gaskets were for when I was thinking of spot welding the pack :slight_smile:. Seems a waste not to use them - I was thinking of putting them on to see if they hold the cells a little tighter in the holders.

I'll make sure to take photos when I put it together.
```

---
## \#130 Posted by: Titoxd10001 Posted at: 2016-09-12T01:13:59.640Z Reads: 347

```
Where did you get those printed?
```

---
## \#131 Posted by: treenutter Posted at: 2016-09-12T03:47:58.563Z Reads: 339

```
[quote="andysurfs, post:126, topic:7392"]
unecessary, but awesome...
[/quote]

This quote should deserves to be repeated!
```

---
## \#132 Posted by: andysurfs Posted at: 2016-09-17T06:30:36.981Z Reads: 342

```
I saw an ad on gumtree here in Australia for a guy that will 3D print items. I sent him the file from Thingiverse for the 6 cell holder and he modified it for me and printed out the 3 cell holders. Cost A$20 for 20 holders (got a few spares just in case).
```

---
## \#133 Posted by: sl33py Posted at: 2016-10-05T20:54:58.883Z Reads: 306

```
@andysurfs - Those looks great man!  

I finally ordered up some 18650 batteries to go with my arduino spot welder i built!  (Fun project btw)

Do you have the 3p modified files on thingiverse or can you share them possibly?  I am looking to 10s3p or 12s3p (not certain yet), and until @Chaka invents the 25th hour or has the time to share/upload the 3p holders i'm trying to figure out alternatives.

Also what rating wire did you go with for your cell fuses?  20A or 30A?  or somewhere in-between?

Thanks and look forward to pics of your pack assembled!

Thanks again Chaka for sharing these!
```

---
## \#134 Posted by: michaelcpg Posted at: 2016-10-05T21:05:44.992Z Reads: 301

```
I'm using 20A fuse wire on my 10S4P pack with no issues. my VESCs are only set to 20A batt max each though, so half of the current my battery is rated for.
```

---
## \#135 Posted by: Okami Posted at: 2016-10-05T22:27:15.591Z Reads: 300

```
Do you have international source for fuse wire? Asked in 2 local shops, they were quite clueless..

just please dont tell me that you had to take bunch of 20A fuses and then broke the plastic to get the metal part out - could work though the form and shape of these fuses makes it hard to solder them, I think.
```

---
## \#136 Posted by: michaelcpg Posted at: 2016-10-05T22:29:27.680Z Reads: 291

```
Unfortunately not sorry. I bought mine from a local electrical supplier. It just came in a big roll.
```

---
## \#137 Posted by: Okami Posted at: 2016-10-05T22:33:11.870Z Reads: 306

```
Ok, perhaps just simple wire can be used, will check that chart one of the users here gave.

--

Theory time!

What will happen if one or few cells trigger the fuse?

Assume we have 10S 4P pack

if, one of the parallels pack cells die, that leaves you with 9s4p + 1s3p
So what would be the effect of such setup?

I assume it work work, if the cell failed (if it was one cell which made serial connection) and that serial chain would be broken.. Though, this does not make sense, as there would be needed some circuitry, to switch the pack to 9s connection and a physical connection should be made directly to each parallel group of cells, 10 in total in this case.

@chaka, do you have experience with failed cells and the battery's pack behaviour after that? Would love to find out the results!
```

---
## \#138 Posted by: chaka Posted at: 2016-10-05T22:42:23.491Z Reads: 297

```
> if, one of the parallels pack cells die, that leaves you with 9s4p + 1s3p
> So what would be the effect of such setup?

It is important to use a bms or cell monitor of some kind to see if cells start to drift since that will be the effect of a failed cell. That particular string of cells would then have less capacity than the rest of the pack and will sag a little bit more than the rest of the pack.

@sl33py You might be able to use tinkercad to modify the file. I recently used it to emboss the mad munkey enclosure and it wasn't to hard to use. should be a youtube video around explaining how to crop an stl file using it.
```

---
## \#139 Posted by: sl33py Posted at: 2016-10-05T22:45:31.221Z Reads: 305

```
[quote="Okami, post:137, topic:7392"]
Ok, perhaps just simple wire can be used, will check that chart one of the users here gave.
[/quote]


Same here.  I went to the link that @Jinra provided:
http://www.powerstream.com/wire-fusing-currents.htm

And if i want a 20a fuse it suggests 26awg.  So then went to @Chaka's link to remingtonindustries.com and found their 100' 26awg "Tinned, Copper Buss wire" - [here](http://www.remingtonindustries.com/tinned-copper-wire/tinned-copper-wire-buss-wire-26-awg-silver-100-length/).  <$10 and hope this is the right stuff...  

Sound about right Chaka?  Tempted to also order up some 28awg (rated from Jinra's link to 15a) and test.  Because it's such a short length it may have more capacity than anticipated?  Or as much as needed?

The question then is - how do i simulate/test to confirm it will blow exactly at 20amps?  (or 25, or 30, etc.)
```

---
## \#140 Posted by: Jinra Posted at: 2016-10-05T22:53:22.427Z Reads: 306

```
chaka recommended 22-24 awg for 20A continuous discharge cells. I got 22 awg to be safe. You don't want a wire that burns up at continuous 20A as you may need room for burst current.

You can simulate with a controlled power source to deliver a set amount of current through the wire. Keep in mind the same fuse can blow at different currents depending on environmental factors such as being enclosed or being soldered to a heatsink such as a brass/nickel tab or buss bar.

Traditional fuses don't blow at their rated current, you would have to exceed the rated current by a certain amount of time depending on how far you exceed it.
```

---
## \#141 Posted by: chaka Posted at: 2016-10-05T22:53:38.872Z Reads: 294

```
There are two schools of thought on how to fuse a pack. 

You can fuse the pack based on the individual cell = a very light gauge of wire.... this is important to protect against the worst case scenario.

Or you can fuse based on the remaining cells "current" capability. This would only protect you from a cell internally shorting out and would not protect against a thermal overload scenario. This still protects a pack from a bad cell taking out your whole pack but it wont save your house if your pack goes thermal.

Edit: it is very rare for a pack to go thermal when not in use. Even in use 18650's have proven to be the most stable of all li-ion in this regard.
```

---
## \#142 Posted by: Okami Posted at: 2016-10-05T22:58:43.402Z Reads: 294

```
@chaka thanks for the quick info, man!

So - it just makes the 3 parallel cells work harder, is this correct? Which would later lead to cell drift and a need to balance them, if you run them quite low.. 

Now I get it, I think. Thanks for showing this concept.

-----


----

[quote="Jinra, post:140, topic:7392"]
Traditional fuses don't blow at their rated current, you would have to exceed the rated current by a certain amount of time depending on how far you exceed it.
[/quote]

Do u have estimates on how long that time is ? I've witnessed fuses to be blown quite quickly if there were a short in dc circuit (the dc plug car offers), though the current is quite high for short circuits so I assume for batteries if would take a lot of time to trigger it (if current is only marginally higher)
```

---
## \#143 Posted by: Jinra Posted at: 2016-10-05T23:00:49.826Z Reads: 292

```
It depends a lot on other factors such as if the fuse is outside or inside an enclosure. I don't have any estimates from experience, though. I only know this from research. A fuse blows from excessive heat. So even if you were running a current beyond the rated amount on a fuse, it wouldn't blow if you were cool the fuse somehow by increased airflow, a heatsink, or other means.
```

---
## \#144 Posted by: Okami Posted at: 2016-10-05T23:01:58.969Z Reads: 288

```
ok, I assume a lab power supply would be an exellent helper here! Hard to fine tune the current otherwise.. at least dont know any other reliable methods.. Old PSU and load high enough would probably also do the trick.
```

---
## \#145 Posted by: Titoxd10001 Posted at: 2016-10-05T23:09:32.845Z Reads: 286

```
Can we use bare copper wire if it's the correct gauge?
```

---
## \#146 Posted by: chaka Posted at: 2016-10-06T02:12:41.182Z Reads: 282

```
Should work. I use nickel plated copper wire.
```

---
## \#147 Posted by: Okami Posted at: 2016-10-06T02:23:37.130Z Reads: 308

```
Can u please update me a little bit more on the ''unleveled serial pack'' concept:

It turns out, that if one pack looses a cell, the total capacity goes down too, so, even if ''nominal / rest'' voltage would be the same for all the ''serial modules'', it turns out that when load is applied, the ''defective'' module would yield lower voltage. 

So my question is:

**What stress is put and where, when running unbalanced cells?**

-----
I do believe that running cells down to cutoff voltage or close to that will be bad in this scenario but does it have any meaningul effect on the performance and other factors if the cells are allowed to reach the ''safe limit'' and not stressed any further?

 Of course, the ''defective'' / lower capacity ''module'' will run out of juice faster (the first) compared to the rest of the pack/modules, hence the total usable (safe) capacity would be lower, too (like in laptop packs when one pack starts to fail).

---

So the next question would be: 

**is there also some sort of balancing action for serial ''modules'' or it only works for parallel ones?**

 I just want to figure out what else might happen when one of the cells or few of them goes out of business :)

-----

Answer from batteryuniversy:

> Let’s look at what happens to a weak cell that is strung together with stronger cells in a pack. The weak cell holds less capacity and is discharged more quickly than their strong brothers. Going empty first causes their strong brothers to overrun their feeble sibling to the point where a high load can push the weak cell into reverse polarity. Nickel-cadmium can tolerate a reverse voltage of minus 0.2V at a few milliamps, but exceeding this will cause a permanent electrical short. On charge, the weak cell reaches full charge first, and then goes into heat-generating overcharge, while the strong brothers still accept charge and stay cool. The weak cell experiences a disadvantage on both charge and discharge; it continues to weaken until giving up the struggle.

> The capacity tolerance between cells in an industrial battery should be +/– 2.5 percent. High-voltage packs designed for heavy loads and a wide temperature range should reduce the capacity tolerance further. There is a strong correlation between cell balance and longevity.

I assume if ''weak cell'' pack would be divided from the rest of the pack and it's voltage monitored, then you could switch it off, once the cells start to hit the low-cut off coltage. This way it would make it more possible to combine strong cell pack with a weak cell pack.

It does not work that great, if weak cells are connected to the strong cells in one system. In this case the scenario happens as the battery university's article informed about - weak cells over discharge and / or over charge while in the same pack, especially if the pack is not balance charged but bulk charged.
```

---
## \#148 Posted by: andysurfs Posted at: 2016-10-08T13:58:33.250Z Reads: 288

```
Hi @sl33py, sorry mate, I've been off the forum for a few days.

I'm afraid I don't have the modified files for the 3p holder - the random guy who printed it for me modded the design and didn't provide me with the file. 

In terms of the fuse wire, I referred to the table @Jinra provided above. For a fusing current of 29.2 Amps, it suggested 0.51054mm copper wire (~24 AWG). I got a 100g roll of 0.5mm for about $5. Still haven't built the pack yet - will try and start tomorrow :grinning:
```

---
## \#149 Posted by: chaka Posted at: 2016-10-11T01:22:27.338Z Reads: 284

```
@barajabali someone remixed my file to hold 18 cells! You wont be able to add a buss bar for the middle row but it could be reworked a little more.

http://www.thingiverse.com/thing:1819003
```

---
## \#150 Posted by: im-done Posted at: 2016-10-11T01:58:33.713Z Reads: 277

```
Thanks for the 18650 holder.
```

---
## \#151 Posted by: sl33py Posted at: 2016-10-11T20:35:27.620Z Reads: 282

```
[quote="chaka, post:28, topic:7392, full:true"]
I get mine from http://www.remingtonindustries.com/
[/quote]


Thanks @Chaka for recommending this vendor.  Got a small assortment of 22-28awg wire to test.  Short lengths and really inexpensive.  Still likely way more than i need and will last a long time!  They also shipped it *really* quickly and got it already.

I also am getting some of the holders printed to build my pack.

@Chaka - do you have any pictures of the completed pack - specifically how you solder the fuse wire to the top of the cells?
```

---
## \#152 Posted by: sl33py Posted at: 2016-10-21T00:03:49.958Z Reads: 295

```
[quote="sl33py, post:151, topic:7392"]
I also am getting some of the holders printed to build my pack.
[/quote]


Got my printed holders last night!  A slight remix of @Chaka's design w/ a sliding holder on one side, and smooth bottom side.  Not sure if that will be an issue to spot weld around... haven't gotten that far yet.

The sliding part is intended to allow me to use 8mm nickel strip, or the 1/2" brass strip like Chaka uses.  I'll be placing a couple dabs of hot glue to secure them when done before shrink wrap.  Trying to keep weight down and keep it somewhat modular for most flexibility.  At 3p, it's quite a bit different from his holder.  Once i have it assembled, and no need for v2, i'll see how i can add it as  a remix on thingiverse.  I had someone do this before getting it printed - no real skill w/ this...  But the intent is to get a final version that works and share it like Chaka did w/ his original.

I'll get a few additional pics tonight w/ some 8mm nickel and 1/2 brass to compare, but here it is so far:
[img]https://goo.gl/XBNvDD[/img]

HTH!
```

---
## \#153 Posted by: Jinra Posted at: 2016-10-21T00:13:59.225Z Reads: 292

```
My finished pack if you'd like some reference :slight_smile:

<img src="/uploads/db1493/original/3X/5/8/58cca4c4aa9232e96e0e0307d65a5268758dfc72.jpg" width="668" height="499">
```

---
## \#154 Posted by: sl33py Posted at: 2016-10-21T00:21:42.271Z Reads: 295

```
Thanks Jinra!  My idea is to be difficult and instead of horizontal stacking like you have, try vertical stacking each 3p.  So two 6s packs side by side.  I have 2 boards i think this will fit in them better.

So i will spot weld the bottom strip on, and then cell level fuse the top in the little fiddly adjustable clamp...

Do your packs have any glue or anything besides that kapton tape to keep them separated (avoiding rubbing w/ vibrations)?
```

---
## \#155 Posted by: Jinra Posted at: 2016-10-21T00:24:44.755Z Reads: 299

```
It's hard to see but I have @chaka's cell holders on there (they're black). I'm also planning to woodglue the whole pack to the enclosure to avoid it bouncing around in there.
```

---
## \#156 Posted by: chipoi84 Posted at: 2016-11-05T11:03:45.427Z Reads: 286

```
Here is a download link for the 3P cell in case anybody need it: https://drive.google.com/file/d/0B3kP5gAJvG6WcVA5VHlBV1lLQTg/view?usp=sharing
```

---
## \#157 Posted by: DanButcher Posted at: 2016-11-05T19:57:41.650Z Reads: 284

```
Guy's i did create an file with information which diameter should be used for which current:

https://docs.google.com/spreadsheets/d/1oOBtC18OJ0GT_ac2A-HZHJp5IIYTlfh6HR8yYz-T7oo/pubhtml
```

---
## \#158 Posted by: Okami Posted at: 2016-11-05T20:00:23.911Z Reads: 281

```
Good to know - though it looks like you have set it to ask a request from google drive to see it!
```

---
## \#159 Posted by: DanButcher Posted at: 2016-11-05T20:07:46.672Z Reads: 287

```
Thank you for information, I'm a bit newbie with google docs :P. Now it should be ok. Basicly this is how fuses were made some time ago, and a lot of people were just changing the wire inside. And i think that the fuse wire itself can meltdown printed holder and in some specific cases shorten cell. 

@chaka you should consider to put those fuses in ceramic tube or any other tube that can hold high temperature. Like this http://www.ebay.com/itm/BUNDLE-SMALL-DIAMETER-THIN-WALLED-HIGH-PURITY-ALUMINA-CERAMIC-TUBES-No-22-/291041819040

**I would never ever use that kind of fuse for higher current than 20A, it's not safe without protection cover.**
```

---
## \#160 Posted by: Aeroquiv Posted at: 2017-03-27T23:37:23.389Z Reads: 262

```
Seems like you answered your own question mostly. The BMS in our battery packs **should** be able to detect the voltage drift from the "weak cell group" and will ideally shut off your skateboard when the pack hits the indicated low voltage that you set. So say you set it at 2.5V, the "weak cell group" would reach this voltage sooner than the healthier cells as the internal resistance of that group would increase. This makes the "weak cell group" to sag more and will reach low voltage in comparison to the other healthy cells. The BMS should notice this anomaly and react by indicating that the battery pack is out of juice. The end result would be a premature shut off with the healthier cells never depleting to 2.5V. Which you then experience as shorter than expected range. 

I haven't done a lot of research, but there are ways to actively balance batteries within serial modules. This would require a more complex BMS circuitry that connects wires to each individual cell. So instead of the usual 11 balance wires, you would need 4 times the amount of them in order to pull charge from individual higher capacity cells to lower ones. In this scenario, the BMS would be able to detect a dead cell within serial packs, but realistically speaking, a skateboard just does not have enough space, nor is the technology priced competitively to be used on one. Active BMS is expensive as fuck.
```

---
## \#161 Posted by: Luuke Posted at: 2017-11-09T14:45:15.790Z Reads: 212

```
3 cells in parallel would be nice.
```

---
## \#162 Posted by: Acido Posted at: 2017-11-09T15:13:03.537Z Reads: 208

```
man this is a great idea, this is the way im going to assemble my next pack in a few weeks
```

---
## \#163 Posted by: psychotiller Posted at: 2017-11-09T15:19:02.904Z Reads: 215

```
I personally don't suggest securing everything to your enclosure. The 1/8 thick flange and screws are not suited to holding all of that weight. The enclosure will be stressed and break. Possibly damaging all of your expensive components. Secure the weight to your deck. Then use the enclosure as an enclosure.
```

---
## \#164 Posted by: Jinra Posted at: 2017-11-10T00:56:45.132Z Reads: 208

```
Oh I didn't mean gluing the enclosure, I was talking about the battery pack TO the enclosure, like on the retail space cell pros.
```

---
## \#165 Posted by: psychotiller Posted at: 2017-11-10T00:59:46.073Z Reads: 209

```
I know! How many of those spacecell enclosures cracked? If you arent going to attach your battery to the deck, it will be supported by thin abs. (the enclosure) You're asking for problems.
```

---
## \#166 Posted by: Jinra Posted at: 2017-11-10T01:00:26.225Z Reads: 207

```
Not sure how gluing the battery to the enclosure has any bearing on the enclosure cracking when attached to the deck.
```

---
## \#167 Posted by: psychotiller Posted at: 2017-11-10T01:02:10.291Z Reads: 201

```
Dude. The weight of everything in your enclosure will be hanging from screws that are going through the thin abs into the deck. Structurally -Not Sound.

I'm not sure how you're missing what I'm saying...
```

---
## \#168 Posted by: psychotiller Posted at: 2017-11-10T01:02:58.228Z Reads: 195

```
Unless you're putting everything on the top of your deck. Then it's good
```

---
## \#169 Posted by: Jinra Posted at: 2017-11-10T01:04:41.661Z Reads: 196

```
Calm down man, I'm legit trying to understand what you're saying, not be an asshole. I'm not sure how my point of gluing my battery to my enclosure has anything to do with the enclosure having thin ABS. That just seems like a separate issue. Unless you're saying to attach my battery to my deck and put an enclosure over it? Either way I've been using the enclosure for over a year now with no cracks. My first SCP4 **did** crack in the corner because I over tightened it, but the following 2 I have have had no problems.
```

---
## \#170 Posted by: psychotiller Posted at: 2017-11-10T01:07:14.884Z Reads: 203

```
[quote="Jinra, post:169, topic:7392"]
Unless you're saying to attach my battery to my deck and put an enclosure over it?
[/quote]

This! You need to attach everything to the deck. The spacecell was a backwards design and broke alot. I know because I replaced a bunch of them. Relying on the abs to hold everything to the underside of your board is bad mechanics.
```

---
## \#171 Posted by: psychotiller Posted at: 2017-11-10T01:09:24.237Z Reads: 204

```
[quote="Jinra, post:166, topic:7392, full:true"]
Not sure how gluing the battery to the enclosure has any bearing on the enclosure cracking when attached to the deck.
[/quote]

If you don't ride your board it will be fine. But bumps and vibrations while riding will break the enclosure, which shouldn't be supporting all of your components.

I'm just trying to help
```

---
## \#172 Posted by: Jinra Posted at: 2017-11-10T01:11:24.249Z Reads: 203

```
Fair point, though I disagree that it's entirely bad design. With sufficient and quality material you can design an enclosure that doesnt have weak stress points on the screw mounts. Both the original SC enclosure and TB enclosure fail to do this, however.

I do like the Raptor 2's solution that does what you're saying and only uses the enclosure lid to hide everything, but that's a much more time consuming to do vs just slapping on an enclosure containing your electronics.
```

---
## \#173 Posted by: guyguy Posted at: 2017-11-10T01:13:38.575Z Reads: 201

```
How have you been securing the pack to the deck out of curiosity?
```

---
## \#174 Posted by: psychotiller Posted at: 2017-11-10T01:15:42.027Z Reads: 196

```
You are right. You could use .250 abs and it would be thick enough. Still wouldn't be the strongest part of your build though and it would weigh a ton.
```

---
## \#175 Posted by: GrecoMan Posted at: 2017-11-10T01:16:01.881Z Reads: 201

```
[quote="Jinra, post:172, topic:7392"]
With sufficient and quality material you can design an enclosure that doesnt have weak stress points on the screw mounts.
[/quote]
This.  I attached my battery to my enclosure from TB and every single screw hole cracked within a week. i attached the same battery to an enclosure from @psychotiller (ironically) and didn’t have a single issue
```

---
## \#176 Posted by: psychotiller Posted at: 2017-11-10T01:17:05.641Z Reads: 195

```
I use velcro for all of the components. Sometimes adhesive strips on some stuff. The enclosure is just a cover.

Now, back on topic!
```

---
## \#177 Posted by: guyguy Posted at: 2017-11-10T01:21:30.299Z Reads: 201

```
Interesting tip man, makes sense to me though. I don't think a lot of builders follow that convention, at least from the threads I've seen. Even production boards that use enclosures like meepo, boosted or the R2 don't attach the components to the deck. Even still, I think what you're saying makes a lot of sense.
```

---
## \#178 Posted by: Jinra Posted at: 2017-11-10T01:22:27.477Z Reads: 199

```
The raptor 2 actually does attach the components to the deck, the enclosure is just a lid.
```

---
## \#179 Posted by: GrecoMan Posted at: 2017-11-10T01:23:44.843Z Reads: 207

```
i plan on buying some alu strips and bending them to go over my battery and screwing them to my board seeing as my battery weighs about 10lbs so abs might have issues supporting it.
```

---
## \#180 Posted by: Jinra Posted at: 2017-11-10T01:24:38.066Z Reads: 205

```
the constant rubbing of the battery pack against metal might make the strips cut into the pack and potentially short it, be careful with that.
```

---
## \#181 Posted by: guyguy Posted at: 2017-11-10T01:24:46.758Z Reads: 197

```
All the components of the R2 are in the enclosure, they're not attached to the deck. I watched moja do a deck swap, you see it here: https://www.youtube.com/watch?v=i7DBdq2ux0o
```

---
## \#182 Posted by: GrecoMan Posted at: 2017-11-10T01:25:29.163Z Reads: 205

```
will make sure to insulate the inner side of the strips with foam + kapton as a bit of a last resort. my battery is also crazy well insulated
```

---
## \#183 Posted by: Jinra Posted at: 2017-11-10T01:26:39.958Z Reads: 213

```
they're in A enclosure, that is attached to the deck (not held on by screws). I've done repairs on R2's they are attached to the deck as the "enclsoure" is essentially part of the deck. The part you unscrew is only a lid.
```

---
## \#184 Posted by: guyguy Posted at: 2017-11-10T01:27:48.540Z Reads: 220

```
<img src="/uploads/db1493/original/3X/d/f/df8fabadfb904ccfb693370964165eaad06914b3.jpg" width="465" height="500">

This is all held to the deck by screws.

It's not a knock on the R2, I think their enclosure is put together very well.
```

---
## \#185 Posted by: Jinra Posted at: 2017-11-10T01:29:21.102Z Reads: 220

```
Yes but screws where the enclosure lid is attached to the deck does not support the weight of components, which is what discussion is originally about.
```

---
## \#186 Posted by: Jinra Posted at: 2017-11-10T01:31:39.273Z Reads: 229

```
See here

https://i.imgur.com/4TMvLjA.jpg

The enclosure lid is off (see missing screws) but the components are held to the inner enclosure which is essentially part of the deck
```

---
## \#187 Posted by: guyguy Posted at: 2017-11-10T01:33:52.384Z Reads: 226

```
Dude, that bottom layer between the the components and deck is held by screws... Watch the video of him swapping decks. 

Just because you have a layer between the deck and all the components doesn't mean it's not held there by bolts.
```

---
## \#188 Posted by: Jinra Posted at: 2017-11-10T01:35:07.476Z Reads: 225

```
I see you're failing to see my point. No matter, I'll let you think what you want and we'll just agree to disagree.
```

---
## \#189 Posted by: guyguy Posted at: 2017-11-10T01:36:39.768Z Reads: 230

```
oh - hmm are you saying the components are attached to the layer between the deck and components -- so if you flipped the board over with the road side cover nothing would fall out? I think I get what you're saying now...
```

---
## \#190 Posted by: Jinra Posted at: 2017-11-10T01:38:04.534Z Reads: 233

```
Yep, the stress points aren't on the enclosure (lid) mounting points and instead on the flat parts of the enclosure where there's much less stress. 

However, with the way the raptor 2 enclosure (lid) is designed, I don't see it cracking even with weight from the batteries and parts.
```

---
## \#191 Posted by: guyguy Posted at: 2017-11-10T01:38:43.269Z Reads: 237

```
Gotcha, thanks for explaining. Very thoughtful design there.
```

---
## \#192 Posted by: trigger4point7 Posted at: 2018-01-14T23:46:06.746Z Reads: 215

```
I know this is a pretty old thread, but @chaka did you have a flat 6p design or did you stack these somehow? I'm trying to create a battery design with two layers of cells that have cell level fusing.
```

---
## \#193 Posted by: scrapheap Posted at: 2018-01-14T23:52:38.405Z Reads: 219

```
He no longer visits the forums.

If you want to talk to him, you will have to contact him directly, either by phone or email.

[http://www.electric-skateboard.builders/t/merry-christmas-and-goodbye/41826](http://www.electric-skateboard.builders/t/merry-christmas-and-goodbye/41826)
```

---
## \#194 Posted by: trigger4point7 Posted at: 2018-01-15T00:02:17.690Z Reads: 224

```
Aw man, I just found his post saying goodbye. Bummer. Thanks for letting me know.
```

---
## \#195 Posted by: twan Posted at: 2018-03-20T04:59:06.112Z Reads: 199

```
I'm planning to build a 10s4p pack using samsung 30Q what gauge fuse wire should I use. 
24awg is rated ~30amps, 30qs are only rated 15amp and some people say 20amps. Should I go for 26awg wire? since those are rated ~20 amps fusing.
```

---
## \#196 Posted by: Cobber Posted at: 2018-03-20T05:25:42.108Z Reads: 198

```
Above Chaka suggested a fuse rated to 110-120% of the cells cont. rating.
```

---
## \#197 Posted by: twan Posted at: 2018-03-20T16:41:51.141Z Reads: 188

```
Oh so that would mean 15A * 1.20 ?
```

---
## \#198 Posted by: GrecoMan Posted at: 2018-03-20T16:51:30.742Z Reads: 184

```
30q’s can do 20a
```

---
## \#199 Posted by: Shaz Posted at: 2019-06-17T10:55:15.825Z Reads: 66

```
Is there a 5p stl file available?
```

---
