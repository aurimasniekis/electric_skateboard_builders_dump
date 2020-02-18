# Project Greenmachine &#124; Kahalani Board &#124; Caliber II&rsquo;s &#124; Dual R-Spec &#124; Dual VESC &#124; S.P.A.C.E Cell

### Replies: 98 Views: 9422

## \#1 Posted by: Iceni Posted at: 2015-11-22T12:10:28.633Z Reads: 340

```
Thought i'd put up my build as well, the more the merrier right?
So the basic features are your standard dual rear drive, space cell powered r-spec machine, nothing really out of the ordinary.

Mounted both VESCs to a sheet so they won't move around.

Got all the components except for some JST connectors for the nunchuck and canbus connections, doubt they'll arrive before the snow hits, seeing as it's started in sothern and northern Sweden last night. Blah

So until they arrive i'm working on the enclosure, making it from sheets of polystyrene.

<img src="/uploads/db1493/original/2X/4/4339b7ccc2210c85f5685ed9dc4b157039b4397c.jpg" width="690" height="460">
Cut a path for the motor wires through a riser pad to get them running between the truck and board.

<img src="/uploads/db1493/original/2X/a/a14affb1a4a26d386d8927863b3ed319ad184fd4.jpg" width="690" height="460">


<img src="/uploads/db1493/original/2X/9/9b52d1d33ecfcb00af6984616ab665ce1a049e83.jpg" width="690" height="460">
Duct tape FTW! (More to come propably)

<img src="/uploads/db1493/original/2X/4/46d19bb1c1ada969ad7104309abe7c3ffee136b5.jpg" width="690" height="460">
Preliminary fitting of the lid, so far so good.
Gonna be painted green to match the trucks.
Might paint the motor mounts green as well, but will have to see how it looks before.
```

---
## \#2 Posted by: kai Posted at: 2015-11-22T13:00:08.161Z Reads: 297

```
Cool idea running the wires that way. Are they snug in there? Or they got a little play?
```

---
## \#3 Posted by: Iceni Posted at: 2015-11-22T13:08:00.676Z Reads: 290

```
They're snug, what's left of the riser pad got compressed when i tightened the bolts.
Will propably make a new riser out of some more rigid material in the future, but for proof of concept it works for now.
Made sure there's enough play on the cables so as to not get pulled on too much in a tight turn, so should't be a problem.
```

---
## \#4 Posted by: kai Posted at: 2015-11-22T13:28:39.443Z Reads: 273

```
Cool man. I look forward to seeing updates on how well that holds up
```

---
## \#5 Posted by: lox897 Posted at: 2015-11-22T20:22:31.848Z Reads: 263

```
Epic! I love how you routed those wires!
```

---
## \#6 Posted by: lowGuido Posted at: 2015-11-22T21:02:11.848Z Reads: 251

```
If I were you I would probably mount the VESC's a bit further apart. you will have a hard time getting a USB plug into the bottom one otherwise.
```

---
## \#7 Posted by: treenutter Posted at: 2015-11-22T21:15:11.232Z Reads: 244

```
Looks great @Iceni ! @siggs3000 had a bad experience w the PPM pins bumping into the capacitors and creating a lightning show; moral of the story is to consider heat-shrinking or protecting those areas so they can't create a short.
```

---
## \#8 Posted by: siggs3000 Posted at: 2015-11-22T21:23:46.689Z Reads: 243

```
OMG they are SO close to touching in these pics!
```

---
## \#9 Posted by: onloop Posted at: 2015-11-22T22:59:33.783Z Reads: 243

```
Actually the VESC with the USB Port with the **Blue Dot** on it is factory programmed as the master. So in BLDC tool you can connect to the slave VESC, via canbus, and setup the configuration parameters for the slave without ever connecting usb to it.

ALSO, it's actually already programmed with the R-SPEC motor parameters... technically that last batch of enertion VESC was plug & play with R-SPEC motors.

So in theory once you connect the two CANbus wires to the slave VESC you will never need access to that 2nd USB port.
```

---
## \#10 Posted by: onloop Posted at: 2015-11-22T23:03:00.517Z Reads: 237

```
Looks like he bent them up, one at 45 degree & one at 90deg.
```

---
## \#11 Posted by: lowGuido Posted at: 2015-11-22T23:51:56.723Z Reads: 228

```
even for firmware upgrades?
good to know anyway.
```

---
## \#12 Posted by: treenutter Posted at: 2015-11-23T00:55:28.979Z Reads: 228

```
[quote="Iceni, post:1, topic:537"]
So until they arrive i'm working on the enclosure, making it from sheets of polystyrene.
[/quote]

@Iceni could you pls comment on building an enclosure out of polystyrene? Where did you get it, how do you form it?
```

---
## \#13 Posted by: trbt555 Posted at: 2015-11-23T05:39:09.998Z Reads: 222

```
@onloop So if I order 2 VESC from Enertion they'll be ready to go as master/slave ? That's really cool.
```

---
## \#14 Posted by: Iceni Posted at: 2015-11-23T06:05:20.943Z Reads: 244

```
[quote="lowGuido, post:6, topic:537, full:true"]
If I were you I would probably mount the VESC's a bit further apart. you will have a hard time getting a USB plug into the bottom one otherwise.
[/quote]

No problems with that, one is set higher than the other as to not block the usb port., worst case i just loosen 3 nuts and bring it up a bit further.

[quote="treenutter, post:7, topic:537, full:true"]
Looks great @Iceni ! @siggs3000 had a bad experience w the PPM pins bumping into the capacitors and creating a lightning show; moral of the story is to consider heat-shrinking or protecting those areas so they can't create a short.
[/quote]

Yea, i've read that, so i bent the pins up and hotglued everything that moved, so should't run into that.
And the vescs are mounted with 3 bolts each onto a board, so they won't move anywhere either.

[quote="treenutter, post:12, topic:537"]
@Iceni could you pls comment on building an enclosure out of polystyrene? Where did you get it, how do you form it?
[/quote]

Got the sheets from a local craftsshop, they also had some thin metal sheets, but to bend metal requires tools i don't have.
For the plastic sheets i just use a heatgun at low heat and use a little throw-together rig to get straight bends.
I can post up some pics later today for anyone that's interested.
```

---
## \#16 Posted by: kai Posted at: 2015-11-23T07:38:40.185Z Reads: 211

```
I am interested in seeing how you are building the enclosure too. Looks like you used rubber firewall grommets to adjust the height of the vesc?
```

---
## \#17 Posted by: Iceni Posted at: 2015-11-23T12:22:29.126Z Reads: 218

```
[quote="kai, post:16, topic:537, full:true"]
I am interested in seeing how you are building the enclosure too. Looks like you used rubber firewall grommets to adjust the height of the vesc?
[/quote]

Will get some pics up when i get home.

I used some rubber bushings for silencing harddrives i had left over from a PC build for setting the height. Used some M3 screws as mounting poles.
```

---
## \#18 Posted by: longhairedboy Posted at: 2015-11-23T18:42:32.467Z Reads: 215

```
Awesome! Very clever boring out the truck risers. That's almost as effective and way less time consuming than my way of doing it which involves dremels, fumes, and occasional swearing. Not that i mind swearing. 

This gives me a great idea for a product, actually... and i really wish i didn't suck so hard at CAD.
```

---
## \#19 Posted by: Iceni Posted at: 2015-11-23T19:48:19.423Z Reads: 240

```
Here's my kitchen tab.. I mean, uh, work bench! 
Using a piece of square metal rod to clamp the sheets down and a second piece to press down while heating it at the bending point.
And the all-important Oven-mitt-of-Not-burning-my-fingers-off-while-holding-on-to-hot-pieces-of-metal. +1
<img src="/uploads/db1493/original/2X/f/f4a776c43010d657cf6ae510ce21dbce5eb8e41f.jpg" width="300" height="500">
```

---
## \#20 Posted by: treenutter Posted at: 2015-11-23T20:02:00.823Z Reads: 238

```
Thanks @Iceni it's great to see a visual of how this is done. [Does this][1] look like the stuff you found at your local shop? If so, I'm impressed that you're able to get it to 350F with a heat gun! 

Could you comment on the thickness that you used?


  [1]: https://www.interstateplastics.com/Styrene-High-Impact-White-Sheet-STYWEH%7ESH.php?vid=201511231358-4p
```

---
## \#21 Posted by: Iceni Posted at: 2015-11-23T20:12:47.597Z Reads: 228

```
Seems like, i use 2mm thick sheets for the parts closest to the board, 1.5mm for the lid.
Not sure what that equates to in inches though.

The heatgun i use can go all the way up to around 600'c, which is around 1100'f
It has variable temperature from 80'c to 600, which is nice. And pretty expensive. But well worth it.
```

---
## \#22 Posted by: longhairedboy Posted at: 2015-11-23T20:50:43.549Z Reads: 199

```
Yeah i was about to say I have a DeWalt heat gun from a local store that will melt your face off. I've used it to bend all kinds of things, peel paint off of walls in single wall-sized sheets, dry fresh paint on a board, heat shrink tubing,  and it will set things on fire when turned up all the way. Damned hot is what i would say since I don't know how hot it actually gets.
```

---
## \#23 Posted by: sgaana Posted at: 2015-11-24T04:31:22.079Z Reads: 185

```
@Iceni, what type of bolt was used to attach Vesc. Where did you place those bolts? What type of material was used for pad? Sorry for so many questions 😬
```

---
## \#24 Posted by: Iceni Posted at: 2015-11-24T06:02:20.905Z Reads: 196

```
Mounted them on a piece of scrap plastic sheet i had left from making the enclosure.
The vesc has 4 mounting holes in the pcb, though i only used 3 of them, since one is located under the PCM connector.
The screws i used are regular M3 machinescrews, about 3 cm long, could use 2.5cm longscrews and still have enough clearance to access both usb ports.
And some rubber grommets to adjust height and making sure i don't short anything out when screwing on the nuts, noticed that the motor lead mounts would get shorted if i just screwed them on withough insulation.
```

---
## \#25 Posted by: monkey32 Posted at: 2015-11-24T14:11:22.810Z Reads: 194

```
All kinds of nice build. Super clean and props for the wire set up. Very useful to see the forming and bending case set up.
```

---
## \#26 Posted by: Iceni Posted at: 2015-11-25T21:13:02.302Z Reads: 197

```
Just a quick update, got my jst connectors in the mail today, so made the canbus cable and the nunchuck reciever plug.
Will plug everything in tomorrow and start doing some benchtesting.
```

---
## \#27 Posted by: Iceni Posted at: 2015-11-26T19:44:58.823Z Reads: 201

```
Some testing later one vesc runs motor detection and is running smoothly with keyboard kontrols.
The other vesc, not so much, motor only gives off one or two stutters during detection and when trying to run it with the keyboard.
Troubleshooting ongoing.
```

---
## \#28 Posted by: Iceni Posted at: 2015-11-26T21:03:56.093Z Reads: 204

```
After a bit of prodding around with my trusty multimeter i found two pins on one of the big chips that was bridged together by some stray solder.
Took a knife to it and lo and behold, it now works the way it should!

<img src="/uploads/db1493/original/2X/7/71c3416754102cff3bf8c6dfa4d5b5d03c6af6d1.jpg" width="300" height="500">
```

---
## \#29 Posted by: sgaana Posted at: 2015-11-27T05:55:34.087Z Reads: 198

```
@Iceni, any chance you can post pictures of canbus cable and nunchuck receiver plug? Thanks
```

---
## \#30 Posted by: Iceni Posted at: 2015-11-27T17:21:32.269Z Reads: 208

```
Not sure if all four pins on the canbus should be used, the guide says to connect the two middle ones, but doesn't say not to use the other two. If they shouldn't be connected, could someone please let me know?

For the nunchuck connector i used a breakout board so i won't need to disassemble the wireless dongle for testing.
Though it doesn't seem to work with the MadCatz Z-chuk, so i had to solder the wires directly to the dongle anyway, which didn't work either, so i guess it just isn't compatible.
The status led on the dongle only gives off a reeeeally dim blinking.
Tried with a wired nunchuck as well, no dice.
So another question: Anyone tried a wired one before?

<img src="/uploads/db1493/original/2X/d/d2e01e711131ba009036934eefff1569e67402d8.jpg" width="300" height="500">
```

---
## \#31 Posted by: elkick Posted at: 2015-11-27T18:18:11.795Z Reads: 197

```
DO NOT connect 5v and GND because that is likely to cause ground loops which can reset and/or kill the VESCs. Just use the middle ones only for the CAN bus connection.
```

---
## \#32 Posted by: Iceni Posted at: 2015-11-27T18:43:34.326Z Reads: 190

```
[quote="elkick, post:31, topic:537, full:true"]
DO NOT connect 5v and GND because that is likely to cause ground loops which can reset and/or kill the VESCs. Just use the middle ones only for the CAN bus connection.
[/quote]

Ah, right. Will remove them. Thanks!
```

---
## \#33 Posted by: kai Posted at: 2015-11-28T00:13:16.423Z Reads: 187

```
yeah supposedly not all wireless nunchucks work... chaka is building the nunchuck alterative that vedder and jacoby are working on and testing them. hopefully it works well and chaka will sells them. i assume onloop will too?
```

---
## \#34 Posted by: Iceni Posted at: 2015-11-28T08:52:11.115Z Reads: 187

```
Yea, but they were cheap, since i couldn't find a nyko inside EU at the time, so got two for less than half the price of one nyko from the states.
So i thought, what the heck, if they don't work at least i get two wireless chucks for my wii.
```

---
## \#35 Posted by: kai Posted at: 2015-11-28T13:32:53.290Z Reads: 190

```
For science! Madcatz is a crossed off from the list. If my nyko fails i will test a few other as well. Will probably get a reg gt2b for a back up. Chaka sells a gt2b in badwolf enclosure but 90usd. I may get one of those if the nunchucks  he is testing doesn't work out.
```

---
## \#36 Posted by: Iceni Posted at: 2015-11-28T14:04:40.512Z Reads: 186

```
Cool, found one nyko on amazon in europe and snagged it, so if that doesn't work i'll go with a 2.4ghz remote and hack it to bits propably.
```

---
## \#37 Posted by: elkick Posted at: 2015-11-28T17:52:52.080Z Reads: 183

```
I just heared today from a guy who claims that he got the VESC v4.10 working with a logic3 Nunchuk on FW1.14. Will test that myself tomorrow, that would solve some headaches especially here in Europe.
```

---
## \#38 Posted by: trbt555 Posted at: 2015-11-30T07:07:59.327Z Reads: 192

```
Frankly I've been seeing too many pictures of shoddy quality VESC assemblies.
Not what I would expect from a $100+ piece of kit. Even if it's regarded as beta.
Are these from Enertion ?
I hope the November batch turns out better.
```

---
## \#39 Posted by: Iceni Posted at: 2015-12-01T06:22:34.055Z Reads: 192

```
Yes, from enertion.
Though from what i've seen, enertion has been good about trying to get them fixed if something is broken.
And I guess i was lucky it was as simple as a solderbridge that just needed cutting, hopefully it didn't cause any permanent damage.
```

---
## \#40 Posted by: Iceni Posted at: 2015-12-07T20:30:18.322Z Reads: 207

```
While fiddling with the cover i found out the bends i made were too brittle and would propably break.
So used some aluminium brackets i had from an old project.
The frame is a single length of aluminium, just cut pieces of one side to make two 90' bends, so it should be sturdy enough.

Glued the plates to the inside of the brackets, will put a few bolts or rivets when the glue has hardened.

<img src="/uploads/db1493/original/2X/8/8dad1214a89432204e99dae32c2ed758d7c9d81d.jpg" width="690" height="460">
Sneakpeak of cover mk.2
```

---
## \#41 Posted by: Iceni Posted at: 2015-12-12T21:36:11.334Z Reads: 206

```
So i got a rivet tool earlier today and finished up most of the case, decided to scrap the formed plastic altogether and go for aluminium sides on both the base and the cover.
I'll be surprised if this bends while riding!

<img src="/uploads/db1493/original/2X/a/a51e0062ac2c536f9891b56abd6e0248bdcebae8.jpg" width="690" height="460">
The cover will be mounted on hinges so it'll be just two locking screws at the other end propably.
Might use a rod through the whole case though.

<img src="/uploads/db1493/original/2X/f/f2d725cb421374fc32da3605494f29a3ae646b2c.jpg" width="690" height="460">
Looking pretty good if i get to say so myself ;)
```

---
## \#42 Posted by: cmatson Posted at: 2015-12-12T22:02:07.354Z Reads: 192

```
[quote="Iceni, post:41, topic:537"]
Looking pretty good if i get to say so myself :wink:
[/quote]
heck ya! I love the super clean look- just a simple box done right. The contrast between the black and aluminum is really neat too!
```

---
## \#43 Posted by: lox897 Posted at: 2015-12-13T01:18:21.647Z Reads: 188

```
Nice box! Is there a special type of hinge you used? I was gonna use hinges and then I just went for a couple more screws instead.
```

---
## \#44 Posted by: Iceni Posted at: 2015-12-13T08:29:36.430Z Reads: 189

```
[quote="cmatson, post:42, topic:537"]
heck ya! I love the super clean look- just a simple box done right. The contrast between the black and aluminum is really neat too!
[/quote]

The plan was to paint it metallic green, but that was before the alu sides, now i'm not so sure.. Might keep the alu look and just put a coat of black on the plastic part, as it is now it's not the prettiest when looking at it close up.

[quote="lox897, post:43, topic:537, full:true"]
Nice box! Is there a special type of hinge you used? I was gonna use hinges and then I just went for a couple more screws instead.
[/quote]

Nothing special, just some basic hinges from the hardwarestore, did have to cut one side of them in half and drill a few new holes in them, but otherwise just your standard cheap-o hinges.
```

---
## \#45 Posted by: broshi Posted at: 2015-12-14T08:46:49.987Z Reads: 170

```
Nice, have you tested the specs for this board?
```

---
## \#46 Posted by: Iceni Posted at: 2015-12-14T11:05:27.429Z Reads: 173

```
Not yet, had a wireless nunchuck that was incompatible, so waiting for a nyko to arrive in the mail, should come any day now.
Though it's getting too late in the season, temps just hit freezing outside.
```

---
## \#47 Posted by: broshi Posted at: 2015-12-15T04:55:19.663Z Reads: 169

```
ohhhh man I'm so excited to see how this turns out. I'm really on edge about 
Hub motors vs External
```

---
## \#48 Posted by: longhairedboy Posted at: 2015-12-15T18:50:12.873Z Reads: 165

```
Hell yeah! I love the hinge idea. I've been mentally working out a sort of slide-lock type thing you see in battery compartments on toys where its just one screw holding the whole thing in. I have absolutely no idea how i will do it. I'm glad to see some more innovation in the box department.
```

---
## \#49 Posted by: Iceni Posted at: 2015-12-19T19:06:28.618Z Reads: 171

```
[quote="longhairedboy, post:48, topic:537, full:true"]
Hell yeah! I love the hinge idea. I've been mentally working out a sort of slide-lock type thing you see in battery compartments on toys where its just one screw holding the whole thing in. I have absolutely no idea how i will do it. I'm glad to see some more innovation in the box department.
[/quote]

Hmm, why didn't I think of that? That might have actually been easier :stuck_out_tongue:
Still, the hinge is working really well, working on the locking screws on the other side atm, waiting for some epoxy to harden.
Two screws to hold the lid closed isn't so bad after all.
```

---
## \#50 Posted by: Iceni Posted at: 2015-12-20T12:24:42.664Z Reads: 185

```
So i made the final fabrications today, now it's only some minor fixes left.
And waiting for the new transmitter which should have been here last week..


<img src="/uploads/db1493/original/2X/0/0f084ef2e74d61df8a02a85e0f0eff6bf45482ca.jpg" width="690" height="460">
Did a flextest once i had it mounted, had to put quite a lot of weight into the jumps to make the board hit the enclosure so it should be fine.


<img src="/uploads/db1493/original/2X/a/aa84d4d280cf1e8917a85c84e6ebee65754f0a47.jpg" width="690" height="460">

<img src="/uploads/db1493/original/2X/d/dc1c9ee84796da87b6e0b89bedbe4c721a052f70.jpg" width="690" height="460">
Had to make brackets from scratch to hold the nuts in place on the inside and some epoxy to keep them from moving when screwing in the bolts.

Will try to seal the opening where the motor wires enters the case somehow.
```

---
## \#51 Posted by: kai Posted at: 2015-12-20T13:52:51.344Z Reads: 179

```
looks good. did you try standing and bouncing on the board yet? looks like that board will flex a lot
```

---
## \#52 Posted by: Iceni Posted at: 2015-12-20T18:18:13.378Z Reads: 175

```
Did bounce on it, it does flex a bit, but there is enough clearance between the board and the box, will use slightly longer spacers just in case.
Got enough grund clearance to sacrifice a few more mm me thinks
```

---
## \#53 Posted by: Iceni Posted at: 2015-12-26T11:58:56.950Z Reads: 180

```
Small update, did some final touches on the enclosure, drilled holes for the charging port, power switch and battery indicator.
Added a rubber seal over the hole for the powerbutton.
Still need to find a good way to seal up the charging port, might make a plug out of oogoo.
And the last thing to add is a transparent sheet over the battery indicator.

Oh, and cover up the holes left over from when i cut off like half of the transmitter.
Did i mention i bought a 2.4ghz transmitter? :stuck_out_tongue:
Not quite as slim as the gt2b, but good enough.
```

---
## \#54 Posted by: Iceni Posted at: 2015-12-26T17:10:24.497Z Reads: 190

```
<img src="/uploads/db1493/original/2X/a/a3bd0baf34fe08f6fa62266b2fda2f6081a69540.jpg" width="690" height="460">
Holes! With plugs and stuff!

<img src="/uploads/db1493/original/2X/7/74b75433f60d710bd163ad9680651d7af44cca50.jpg" width="690" height="460">
Not quite the controller it used to be.
Gotta let the glue dry, then sand off the sharp edges.

And with that the board can be considered complete and ready for it's shakedown run outside.
```

---
## \#55 Posted by: lowGuido Posted at: 2015-12-26T22:31:45.053Z Reads: 176

```
thats a pretty cool case mod.
got any before photos?
```

---
## \#56 Posted by: Iceni Posted at: 2015-12-27T08:13:56.818Z Reads: 175

```
Can put up some more when i've sanded down the edges and fixed the powebutton, as it is now it's not exactly the best solution.

Did integrate a rechargeble battery with charging circuit into the case too, no idea what the batterylife ends up at.
```

---
## \#57 Posted by: Iceni Posted at: 2015-12-27T19:45:11.537Z Reads: 186

```
Controller is all done, changed the power button from a push-button to a slide switch.

<img src="/uploads/db1493/original/2X/6/6ded024961a76dec4d4a613267bc4e2c3b36067c.jpg" width="690" height="460">
Managed to make the edges pretty smooth with some plastic putty andsandpaper.
Covered it all up with a coat of matte black paint.

<img src="/uploads/db1493/original/2X/5/5d7ffc1e1965dc20920580aa232204e3ac416e89.jpg" width="690" height="460">
The pcb holding all the knobs on the top was really wide, so decided to just keep most of the case intact.

Never took a before photo, but found one on the store i bought it from:
<img src="/uploads/db1493/original/2X/5/5da6984ba48faf62eb4203390c41a9a516eebadc.jpg" width="640" height="480">
```

---
## \#58 Posted by: kai Posted at: 2015-12-28T01:08:17.287Z Reads: 182

```
looks better man. nice job
```

---
## \#59 Posted by: Iceni Posted at: 2015-12-29T19:22:14.940Z Reads: 176

```
Funny story, I just got a note from the postal service today saying i had a package to collect that arrived on December 15, so now i have a nyko kama as well as the modded 2.4GHz controller.
GG Well played Postnord..

Did a quick benchtest and it works without a hitch.
Now to wait for the damn snow to go away so i can do some real testing..
```

---
## \#60 Posted by: treenutter Posted at: 2015-12-29T20:18:21.776Z Reads: 174

```
@Iceni the Nunchuck w VESC is my favorite controller setup so far; keep a close eye on it at first for dropouts and make sure the wiring and signal are solid before you take it up to max speed.
```

---
## \#61 Posted by: Iceni Posted at: 2015-12-29T20:55:54.774Z Reads: 182

```
Will make the wiring bulletproof and keep an eye out when the time comes.

Until then i might make some minor cosmetic changes to the enclosure just to keep me ocupied.
Gonna switch out the black plastic sheets on the lid to a single one, it bugs me that they're not completely in line :P
```

---
## \#62 Posted by: Iceni Posted at: 2016-02-07T13:47:47.697Z Reads: 182

```
Working on version two of the enclosure atm.
Cracked open the space cell to move the chargeport, powerbutton and display to another spot.
Need to get some extra wire to extend the charging leads.
Will propably get a water resistant powerswitch as well. Not sure if the original is.
And propably another chargeport as well.

<img src="/uploads/db1493/original/2X/7/774f7f8c4db5c8050757f01253c4e3791375dda3.JPG" width="690" height="459">
@onloop I'm sorry man, but it had to be done!
 
<img src="/uploads/db1493/original/2X/b/b09949163973155f08524ab0b3bb56e9b1fa672a.JPG" width="690" height="459">
Noticed that the cable to the charging port had a  cut in it, some shrinktube fixed it easy though.

<img src="/uploads/db1493/original/2X/e/e47e94c0f65904103ef071c0fd6b2efee840f492.JPG" width="690" height="459">
Quick draft of the layout.
Button, charge port and display will end up on the short side facing backward to keep the bottom of the case clean.
```

---
## \#63 Posted by: Iceni Posted at: 2016-02-24T19:21:28.428Z Reads: 174

```
So, finally finished it, again.
Except it's now better!

<img src="/uploads/db1493/original/2X/e/eadcf8d0939e62c2f85f88dbaadf1ed98499fcd5.JPG" width="690" height="459">
As i said before, there would be more ducttape ;)

<img src="/uploads/db1493/original/2X/4/45c31999de9e90309a6c1cf595dc4959ba9110c2.JPG" width="690" height="459">
No need to make holes in the lid anymore, woo!

<img src="/uploads/db1493/original/2X/0/0405d1b03005cac840ce0b920b3530f500be74c1.JPG" width="333" height="500">
Looks shinier in real life.
```

---
## \#64 Posted by: Iceni Posted at: 2016-03-03T20:20:01.761Z Reads: 163

```
First shakedown run ended with three things to fix:
-Loose screw on one motor mount.
-Loose set screw on one motor pulley.
-One loose ESC, no big deal, pretty cramped in the box so it couldn't move around even if it wanted to.

And another thing I found out when I tried to charge it was that I soldered the negative charge lead to the wrong pin on the plug, oops.

I'm thinking I need to buy a new bottle of thread locker.. The one I have is going on 10 years now.
```

---
## \#65 Posted by: Iceni Posted at: 2016-03-10T18:10:16.672Z Reads: 162

```
Waterproofing electronics, oh yea!
<img src="/uploads/db1493/original/2X/a/a70dbe59dbdb89d0442480b0f2eedf17cf946c83.JPG" width="690" height="461">
```

---
## \#66 Posted by: NIK Posted at: 2016-03-11T08:03:21.366Z Reads: 157

```
After you applied the corrosion x, did you wipe the excess of it or you just leave it? I have the corrosion x HD and will try to waterproof it when I have free time.
```

---
## \#67 Posted by: Iceni Posted at: 2016-03-11T15:56:52.692Z Reads: 158

```
I let it drip dry over night, then just dabbed it with a paper towel to get the leftover blobs off.

And it's been drying all day today as well, was still semi wet in the morning, I'll give you an update when I get home.
```

---
## \#68 Posted by: Iceni Posted at: 2016-03-11T18:44:47.193Z Reads: 157

```
So, after about 24 hours it's still hasn't dried completely, but no matter.

Went for a run to get some food, and that damn motor mount shook loose, again!
Guess I'll have to clean it out more thoroughly this time.
And use new threadlocker..
```

---
## \#69 Posted by: Iceni Posted at: 2016-03-11T21:26:48.516Z Reads: 162

```
Got tired of having to carry it in my hands, so I made this:
<img src="/uploads/db1493/original/2X/4/463c45caada80af1f8e64b6b8fbb49afad591a3f.JPG" width="690" height="459">
```

---
## \#70 Posted by: Iceni Posted at: 2016-03-12T08:51:09.326Z Reads: 153

```
With a bit of cleaning the threads with acetone and breaking open a fresh tube of threadlocker the cursed motor mount held up the test run, woop.

Now to see if there's any other bolts I need to clean up and relock, hope not.
```

---
## \#71 Posted by: Iceni Posted at: 2016-03-12T17:14:27.187Z Reads: 146

```
So after a run of about 9km (5.5 miles) everything held up nicely, finally!
Only thing is that there seems to be a problem with one of the motors, but that's for another thread.
And i'm gonna switch out the nunchuck to my modded rc controller, since i'm riding rightfoot forward and holding the controller in my right hand the signal drops as soon as i put my body between it and the reciever.

Apart from that, maaan, this thing is awesome!
```

---
## \#72 Posted by: AbrownMN Posted at: 2016-03-14T02:05:16.144Z Reads: 147

```
Love your enclosure! Very clean build man..I want to do something similar, that would fit a 12s pack @ 18.25 x 6 x 1, plus two VESC's. Trying to get an idea of how big it needs to be, and figure out what deck I will need to buy in turn. Would a pack that size still fit this enclosure with the two vesc's?
```

---
## \#73 Posted by: Iceni Posted at: 2016-03-14T06:00:08.178Z Reads: 144

```
My enclosure is a pretty tight fit as is with the components I have.
To fit your planned battery it needs to be around 2.5" longer.
If you plan to use the same layout inside it needs to be around 25" long minimum.
And the distance between the trucks would need to be around 34" with a traditional belt drive.
Maybe a couple inches shorter if you forego the hinge mechanism in the front.
```

---
## \#74 Posted by: AbrownMN Posted at: 2016-03-14T13:02:02.281Z Reads: 135

```
Great, thanks for the info! I will be using dual hub motors so I should have a little less space taken up by those, though I don't know exactly how much. Just looking for a rough idea so I can buy the proper deck once Psychotiller comes up with an enclosure for me.
```

---
## \#75 Posted by: Iceni Posted at: 2016-03-14T13:09:13.532Z Reads: 137

```
Hub motors will probably save you around 3-4 inches on your deck.
```

---
## \#76 Posted by: AbrownMN Posted at: 2016-03-14T16:50:01.974Z Reads: 141

```
Nice, so I would be coming close to about the same size enclosure. What's the wheelbase on that deck?
```

---
## \#77 Posted by: Iceni Posted at: 2016-03-14T17:20:59.947Z Reads: 133

```
Yep, only marginally longer case.
My board has a 30" wheelbase.
```

---
## \#78 Posted by: AbrownMN Posted at: 2016-03-14T17:35:56.471Z Reads: 141

```
Awesome, that will help influence my decision on the deck. I will definitely need to go a bit longer so I'll probably have to get a super stiff downhill deck. Have you tested how waterproof your enclosure is by chance?
```

---
## \#79 Posted by: Iceni Posted at: 2016-03-14T18:19:08.162Z Reads: 141

```
Not yet, but I've sealed it as good as I can, so until I can test it I'd say it's puddle proof at least.
And I've waterproofed the electronics with CorrosionX, so even if it takes in some water it shouldn't really matter. Hopefully.
```

---
## \#80 Posted by: AbrownMN Posted at: 2016-03-14T18:28:13.992Z Reads: 135

```
Nice. I will have to pick up some of that for my connections as well.
```

---
## \#81 Posted by: Iceni Posted at: 2016-03-14T18:37:39.313Z Reads: 135

```
You should if you plan to run it in wet conditions.
Did a lot of reading up on that stuff, a lot of people use it for their electronics in RC sea planes, with it they can literally drive their planes underwater, even saltwater.
```

---
## \#82 Posted by: AbrownMN Posted at: 2016-03-14T18:40:40.930Z Reads: 134

```
Damn..I was just mentioning in my thread how wet it can get here and how I want to ride every day. Ordering a can now! That should help. I also plan to do a similar encasement as you, but with a custom enclosure from Psychotiller. I was thinking of laying down a thin sheet of rubber (neoprene?) and then monthing everything to that, cutting the edge to sit perfectly inside the case and then cutting a small channel for a gasket around that to seal in the flats of the enclosure. I think with that setup and some of that spray I should be good. Did you just dip all your connections, or did you spray it right on everything lightly?
```

---
## \#83 Posted by: Iceni Posted at: 2016-03-14T18:50:29.051Z Reads: 140

```
Oh yea, just read that as well :p
I just dropped the electronics in a can of it letting it soak for a few minutes.
I'd suggest doing it in a well ventilated room, preferably far away from where you live, it's gonna stink something awful :p
And it will take a few days for it dry enough to handle afterwards.
Don't necessarily have to dip the connectors, but people say it doesn't hurt.
Oh, and you'll never ever ever ever ever be able to glue something on to anything you've treated :p
```

---
## \#84 Posted by: AbrownMN Posted at: 2016-03-14T19:21:14.244Z Reads: 139

```
Haha, all good to know. There's just some dichotomy in my brain about dropping $200 worth of electronics into any container of liquid..Will I ever need to glue anything to them? I hope not..I am a total newb with these types of electronics. I have worked with building plenty of PC's but the worst you have to usually worry about there is static discharge.
```

---
## \#85 Posted by: Iceni Posted at: 2016-03-14T19:27:03.731Z Reads: 132

```
Tell me about it, i just had to trust the flier people to know what they were talking about ;)
I havn't seen any info on coating the batteries though, so for now i've left mine as is.
```

---
## \#86 Posted by: monkey32 Posted at: 2016-03-14T19:48:00.105Z Reads: 129

```
Hot glue is incredibly useful for securing and connection.....I know many people use it to insulate/isolate VESC pins and soldered pieces. Sounds like with the electronics proofing you just want to double check that what you got is nailed down as solid as possible before taking it for the swim in the goo.
```

---
## \#87 Posted by: AbrownMN Posted at: 2016-03-14T20:38:30.910Z Reads: 126

```
Okay, I was wondering if that was actually hot glue I was seeing all over and not some electrical compound. Thanks for that. I suppose it makes sense for covering up stuff that just needs to stay together that you won't need to access much.
```

---
## \#88 Posted by: Iceni Posted at: 2016-03-14T20:45:31.513Z Reads: 133

```
I removed all the hot glue before dipping them and made some rails on the bottom of the enclosure to be able to strap the vescs down with Velcro.

I can take a new photo of how it looks if you want.
```

---
## \#89 Posted by: AbrownMN Posted at: 2016-03-14T22:14:09.535Z Reads: 140

```
I would like that, and appreciate it greatly. Right now I am in the stage of just getting a deck/enclosure figured out so I am throwing all the ideas around in my head about how to best arrange it all. So, I will take all the info I can.
```

---
## \#90 Posted by: Iceni Posted at: 2016-03-15T19:10:24.310Z Reads: 142

```
This is how i fasten my vescs, the bottom of the enclosure is sheets of polystyrene, which made it really easy to build the raised platforms.
Using scraps left over i just glued them together using smaller pieces between the plate and the bottom to get some room for the velcro to go under.
Polystyrene and glue for plastic models works really great, melts the parts together creating a permanent bond.
<img src="/uploads/db1493/original/2X/0/05570e4a965535e27b70700664c955d8f35ea348.JPG" width="690" height="460">
```

---
## \#91 Posted by: AbrownMN Posted at: 2016-03-15T21:08:15.205Z Reads: 136

```
Great info! Thanks for the photo. I like that securing method and I suppose it also helps keep it insulated from grounding anything out etc..will definitely be utilizing a similar method.
```

---
## \#92 Posted by: Iceni Posted at: 2016-03-17T21:49:32.285Z Reads: 131

```
So yea, i managed to bust up the motors, minor setback.
Will rewind them for fun and science.
```

---
## \#93 Posted by: AbrownMN Posted at: 2016-03-17T23:33:44.872Z Reads: 124

```
Whaaaat? What happened to them man?
```

---
## \#94 Posted by: claudiofiore88 Posted at: 2016-03-18T03:56:07.815Z Reads: 127

```
It's in this thread.

http://www.electric-skateboard.builders/t/one-r-spec-motor-hotter-than-the-other/1780
```

---
## \#95 Posted by: Iceni Posted at: 2016-04-10T19:19:48.913Z Reads: 116

```
After that minor setback it's now back on the road with a freshly wound motor (and sore thumbs on my end)
Unfortunatly it's only gonna be a single motor for a while.
When the motor shorted out it seems to have damaged the vesc as well, is getting a drv error when trying to run the motor now.
Luckily the second vesc still works fine, so that's something.

Gotta find someone that can replace the dead chip in sweden.

Still, it runs fine enough on one motor, but i miss the crazy acceleration of the duals.
```

---
## \#96 Posted by: Iceni Posted at: 2016-04-11T19:10:37.118Z Reads: 120

```
So after about a 5 mile testrun it didn't run as fast as i expected, so it got me thinking, never thought about the original wind being delta.
So after some more calculations it made a whole lot more sense.
I terminated my winding as star, so i's approx 140 kv instead of 240 as i thought, which seems to be correct according to my top speed test and using the gearing calculator.

Oh well, 30km/h is still good enough for getting to know the board properly.
WIth duals i should be able to switch to a bigger motor pulley without problems for a bit more speed.
```

---
## \#97 Posted by: Iceni Posted at: 2016-04-28T17:40:57.774Z Reads: 115

```
I can now say that CorrosionX works as intended, got attacked by a downpour on my way to work today, pretty much drenched the electronics and they still ran like dry.
The funny thing is that the waterproof powerbutton I got was not so waterproof, it is now a permanent on button :stuck_out_tongue:
Time to switch it out for a loop key.
```

---
## \#98 Posted by: Komamtb Posted at: 2018-01-18T11:35:07.962Z Reads: 45

```
are those 184 trucks?
```

---
## \#99 Posted by: Iceni Posted at: 2018-01-21T09:01:14.912Z Reads: 33

```
I think so, they're standard calibers.
```

---
