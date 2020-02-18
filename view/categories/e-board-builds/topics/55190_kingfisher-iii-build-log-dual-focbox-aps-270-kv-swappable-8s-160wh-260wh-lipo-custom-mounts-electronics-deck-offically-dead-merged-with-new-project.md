# KingFisher III Build Log &#124; Dual Focbox + APS 270 KV &#124; Swappable 8S 160Wh / 260Wh lipo &#124; Custom mounts / Electronics / Deck \[\[\[OFFICALLY DEAD, merged with new project\]\]\]

### Replies: 34 Views: 1554

## \#1 Posted by: TowerCrisis Posted at: 2018-05-12T08:41:09.538Z Reads: 332

```
I'll be periodically updating this thread on my build progress. Here's a list of all parts I currently have:

Paris V2 Trucks x2
Focbox x2
APS 270 KV x2
CustomSkateboards.com deck
DIYEboard airless tires
76mm road hawgs

**Parts to aquire:**
Lipo cells x24 (8 for pack #1, 16 for pack #12s
Motor brackets
undecided size of middle wheel (100 ish mm. Not MBS)
3D printed enclosures
Custom PCB's and components

This board is going to be fully waterproof. Currently, I have solutions to many issues:

Motors have had internal bearings replaced with sealed ceramic equivalents. Stator will have thermally conductive high temp conformal coating. Outer bearing has an additional rubber gasket seal fitted into the motor mount, and will be greased between the seal and the bearing.

Battery case will be entirely gasket sealed shut. quick connect contacts will have a soft rubber seal to engage with the docking port on the board. The docking port will be bolted tightly to the deck using inset T nuts from the top, with a seal between. Power and signal wires to the battery will be hidden underneath the griptape in grooves. Grooves will be sealed with silicone once completed, then covered with kapton tape and then griptape over top.

Motor wires will plug into contacts inset into the deck. Heatshrink with internal contact glue will completely waterproof these connections.

Phase wires going from the ESC's will go through the deck, and be sealed from above. Will have quick connects internal to the case to allow you to remove the case.

All wheel bearings will be ceramic sealed Zealous. Larger bearings for the pulleys for the two smaller sized wheels will be sealed ceramic.

And finally, the main control box will be sealed against the deck from below using silicone gaskets and T nuts. There is only one exposed button on this board, and that is the power button. I've found a fully waterproof LED button for this.

In addition, it's using all anodized aluminum or 316 stainless steel, which is rust proof to even salt water.

By the end this board will be able to be thrown into a pool and still drive around on the bottom, and I'm not going to stop until it can do that.

Here is a preliminary design CAD. The trucks are moved to the limit before wheel bite on the 6 inch wheels. Using 5 degree risers with 180mm trucks.
![Capture1|690x254](upload://4SZDyOyCr4MBg7a2OvJ93iMrbZW.PNG)

And a side profile.
![Capture2|690x137](upload://jJEC06EIewnfxWUZjI4tkh5S9ZY.PNG)


Here's the front at full tilt.
![Capture3|690x330](upload://aiBVamrAatyFnK0seEpXINSwhnD.jpg)


Here's a closeup of the motor brackets.
![Capture4|690x422](upload://ttSLeAw3NasLKcbi2MnBdTQNqfr.PNG)

Now I'll talk a little about the custom electronics I'm creating (almost done with laying it all out :) ).

**Board side:**
Uart control of FOCbox, will read data from port

Relay controlling switching of antispark, allows for momentary switch for starting and stopping the board.

Control of underglow, headlights, and turn signals

Smart emergency stopping and unexpected disconnect control

SPI based high power NRF module for two way communication, using data encryption and packet verification

USB mini for programming / debugging

Battery pack has integrated antispark (exposed contacts are not live once the pack is disconnected) and a BMS for charge and discharge.

**Remote side:**

Haal effect based thumb stick control

cruise control button

turn signal buttons

Headlights / taillights switch

under glow cycling button

Digital display (can display ESC faults, temps, battery level, expected range, current trip distance etc. Contingent on software development.)

USB mini for charging, and flashing new firmware

**In conclusion:**

This is by far my most challenging build yet, but I'm up for it. My first build used custom mounts and custom electronics for the battery, controller, and receiver. My second build was similar. 

Hopefully my third build will be enough for me, using FOCboxes as the only COTS parts. Having all my wants such as swappable batteries and wheel sizes is a must for this build.

I hope you all enjoy watching this long process of me building and machining this board as much as I will creating it. I'll update when progress is made.
```

---
## \#2 Posted by: xilw3r Posted at: 2018-05-12T09:13:15.918Z Reads: 268

```
Impressive list of features. Going to be interesting this one. I guess you will write a custom fw for nrf control..what chip will you use ?
```

---
## \#3 Posted by: TowerCrisis Posted at: 2018-05-12T09:27:46.480Z Reads: 282

```
Currently undecided for what chipset. I'll have a few extra PCB's so I'm going to try ~3 different ones and test thoroughly.

As for custom firmware, it won't be too difficult. This kind of communication protocol is very simple, using TX and RX you can cut up the data you're sending and disperse it throughout expected data, such as specific base 16 values, which the other recieve will read and verify. If any of a string of values is compromised, that entire block is thrown out as bad data, and that one value that was sent can be ignored.

The option for data verification also is possible. The remote can signal to the board a value and a string of predetermined numbers. The board can then verify the predetermined numbers, which should match what it expects. It then reads the recieve value, and signals back to the remote the recieve value along with verification values. The controller then verifies the values, and the recieve value. It can then send another packet, which contains the next signal of the trigger, predetermined values, and a signal indicating that the last packet was valid.

If any verification values are corrupt in this back and forth process, the data is thrown out. If a series of let's say 40 out of the last 50 packets is invalid, it senses a disconnect and will stop safely.

This kind of data verification can result in 4 packet signals of delay between input and motor change. But on the scale of high baud rate, this time is hundredths of a second. The code is very simple once you figure it out, and is plain cause and effect based.
```

---
## \#4 Posted by: xilw3r Posted at: 2018-05-12T09:43:18.109Z Reads: 245

```
I'd love to learn more about this as you go along. Im really new at programming (just barely touching arduino), but i would like to incorporate simillar safety techniques when i advance further with my remote.

For starters it would be great to get the vesc reaponding to my pwm signal so im a long way off from even simple uart  :)
```

---
## \#5 Posted by: mynamesmatt Posted at: 2018-05-14T01:51:23.913Z Reads: 206

```
look forward to following this build! GL!
```

---
## \#6 Posted by: willpark16 Posted at: 2018-05-14T02:14:55.517Z Reads: 213

```
For ur swappable battery I would make a hollow deck so u can make a modular battery to swap in and out, or design the locking mechanism so that you can deal with the vibrations
```

---
## \#7 Posted by: TowerCrisis Posted at: 2018-05-14T07:33:46.292Z Reads: 192

```
Cad model of the battery swapping is almost complete. It's very slim and will be vibration proof. All connections in and out will use 5.5mm bullet connectors to prevent any disoconnects. Slight change of plans, I'm creating a custom antispark to use a momentary switch with.

Dropping pictures tomorrow once it's all refined.
```

---
## \#8 Posted by: willpark16 Posted at: 2018-05-14T08:00:26.861Z Reads: 184

```
Print nylon
```

---
## \#9 Posted by: TowerCrisis Posted at: 2018-05-14T16:51:16.922Z Reads: 179

```
E3d edge is my favorite ;)
```

---
## \#10 Posted by: TowerCrisis Posted at: 2018-05-15T03:28:02.201Z Reads: 202

```
![IMG_20180514_202449|375x500](upload://mLmghoDv8Xmg9bqMmLcjz7PgB8j.jpg)
![IMG_20180514_202440|375x500](upload://dRUO07atQuopBfxb1LCwUeXnKzA.jpg)

Slight progress! I designed and printed some wheel pulleys for 76mm zombie hawgs. Any interest and I can release the files.

Next is the 100mm version, and the 6" wheel already has a pulley.
```

---
## \#11 Posted by: TowerCrisis Posted at: 2018-05-15T06:31:17.712Z Reads: 197

```
Swappable battery pack is completed. Next job is the dock board side, and the charging dock for the pack.

![Exploded|690x388](upload://9RXfQCAVxXzqDTif0e3c5UfndqU.JPG)
![closed bottom|690x388](upload://8vOvn27uo4Qb33nq7SQlKeNKpWf.JPG)
![closed top|690x388](upload://tyTd7ALNV5Zdz00RBYf8Of2XfOm.JPG)
```

---
## \#12 Posted by: Naysh Posted at: 2018-05-15T07:37:06.693Z Reads: 173

```
I think you'll be the first DIYer that's come up with a swappable battery pack. Swappable like click-in and not disconnecting XT-90s. What CAD program you using? Fusion 360?
```

---
## \#13 Posted by: TowerCrisis Posted at: 2018-05-15T07:59:46.573Z Reads: 175

```
Always a first :slight_smile: Hopefully it works well, the pack isn't very large right now. Only 8S1P with 5000mah cells rated for 20C :man_shrugging: But it'll be lightweight. 

 Using Solidworks 2017
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-05-15T08:35:43.417Z Reads: 175

```
How would you fix in so it  would jump back on those bolts?
```

---
## \#15 Posted by: TowerCrisis Posted at: 2018-05-15T08:37:30.445Z Reads: 176

```
@Kug3lis The side that the battery interfaces with has a pin on each side that slides into the clearance hole closest to the plugs.
```

---
## \#16 Posted by: Kug3lis Posted at: 2018-05-15T09:10:34.715Z Reads: 172

```
Oh ok... I was looking into something similar but the problem is 5kg or 8kg battery pack :D
```

---
## \#17 Posted by: TowerCrisis Posted at: 2018-05-15T09:37:28.133Z Reads: 167

```
It's possible. I've seen some that use a clip that snaps up at the end opposite of the plugs. I didn't like that look.
```

---
## \#18 Posted by: TowerCrisis Posted at: 2018-06-03T07:31:38.200Z Reads: 159

```
![Capture|303x500](upload://7GkUE4p2KI9tsx1A6csqQ0lVprG.PNG)

Quick little update before I post some more stuff in the coming days. I've been sitting on this doc for a while now but I figured I'd post it now.
```

---
## \#19 Posted by: TowerCrisis Posted at: 2018-06-20T07:54:57.629Z Reads: 159

```
Here's a preview of the underside, I finished both enclosures.
![bottom|690x247](upload://4RC7g5n3MmmblxoGbRpSlyq6SbW.jpg)

I designed a 5 degree wedge with integrated phase cable plugs.
![IMG_20180620_004310|375x500](upload://gk6UUkkPXblWyp3p68u8vQwRZdz.jpg)


![IMG_20180620_004540|375x500](upload://8fgbUjOBpisBhevXitgQM3x13gf.jpg)
```

---
## \#20 Posted by: Toughook Posted at: 2018-06-20T10:12:53.958Z Reads: 148

```
good to see someone else doing the cable riser option. What size bullet connectors are you using. Mine are 4.5mm and seem pretty robust when fitted, but there is a very small amount of slip and I'm concerned that vibrations may cause some slipage of the plugs. To counter this I propose to use some copper shim to wedge the plugs in and make them extremely tight when connected. Reckon that should do it as I really don't want to go back to a having a thick black wire loom on show for each motor now I can see how clean the board looks with a cable riser.

Great work on the swappable battery idea as well :fu::fu::fu:
```

---
## \#21 Posted by: TowerCrisis Posted at: 2018-08-08T21:11:50.261Z Reads: 132

```
![IMG_20180807_172754|666x500](upload://6ATc0mowG18wUdgTIvJIzD7ZJeA.jpg)

Update to the battery:

Added two additional ports for a deadmans switch to ensure the battery is only live when plugged in.

Using a LHB antispark that's been slimmed down.

Refined circuitry for momentary button switching (click on, hold off) which will not consume power when on. (Not shown)

Soldered all lipos and BMS together.

Case is complete, awaiting more filament to print the release buttons.
```

---
## \#22 Posted by: brenternet Posted at: 2018-08-08T22:04:02.301Z Reads: 125

```
Looks very tidy in there. What's the weight of the spare battery going to be that you will carry?
```

---
## \#23 Posted by: Jmding Posted at: 2018-08-08T23:30:10.416Z Reads: 126

```
Hey man, I'm starting a build with the same wheels.  Any chance I could take a look at your pulley files?  I was planning on modeling my own 40T wheel pulley, but this might be perfect!
```

---
## \#24 Posted by: TowerCrisis Posted at: 2018-08-09T02:19:57.273Z Reads: 117

```
Sure, I don't have access to them this instant but I'll get them posted soon. Did you mean for the 76mm zombie hawgs or the diyek8 90mm wheels?
```

---
## \#25 Posted by: Jmding Posted at: 2018-08-09T03:17:38.861Z Reads: 116

```
the zombies
going down in diameter to try to save weight
```

---
## \#26 Posted by: Jmding Posted at: 2018-08-09T04:08:47.031Z Reads: 116

```
actually, no worries I ended up seeing a cool idea in another thread about adding a bearing that rides on the aluminum of the truck to help ensure a concentric pulley, so I modeled up a new version of the pulley with a large bearing seat to explore that idea

![image|673x500](upload://vOtEznyyyJ9y10fOirtEsG0I73C.png)

![image|673x500](upload://fKoXkf9Xcmnt0sPFQq35FH6hNty.png)
```

---
## \#27 Posted by: Sinned800 Posted at: 2018-08-09T06:59:03.160Z Reads: 105

```
really nice and tidy battery :clap::clap::clap:

How do you plan to lock the bat in place ? are you planing some kind of intersection with lock mechanism or just screw it in Place ? (im starting my own project right now and have as well a swappble concept in mind)
```

---
## \#28 Posted by: brenternet Posted at: 2018-08-09T07:28:14.274Z Reads: 105

```
@Jlabs has these in hand now, I appreciate that you are making this yourself but though I'd mention it in case you wanted to skip the fabrication part! I'm sure you spotted it but the pulley and wheel would need to share a wide bearing on the Paris truck to fit, or you'd need to modify the truck to shorten the arm slightly.
```

---
## \#29 Posted by: TowerCrisis Posted at: 2018-08-10T08:07:44.005Z Reads: 93

```
It uses a tool-less removal. It's got 6 wall hanger style slots on the topside which interlock with shoulder bolts on the board. Two spring pins lock into holes in the battery which can be pushed back in to release via buttons on the battery.
```

---
## \#30 Posted by: Risewithin Posted at: 2018-08-20T12:41:05.341Z Reads: 81

```
Following!! Nice build so far!
```

---
## \#31 Posted by: Socalscare Posted at: 2018-09-07T14:06:15.357Z Reads: 76

```
Following, I like the full water proofing. My board build will be a year round commuter so I'm looking at mostly dry with a few heavy rains living in Southern California.
```

---
## \#32 Posted by: skyblaster Posted at: 2019-05-11T03:59:06.945Z Reads: 28

```
Awesome work on those Zombie Hawg pullies @TowerCrisis and @Jmding.
I've been playing around with the parametric pulley library in OpenSCAD, but would love to see your files if possible? Cheers!
```

---
## \#33 Posted by: TowerCrisis Posted at: 2019-05-11T05:19:28.664Z Reads: 26

```
Of course, I'll upload my cad for the wheels and pulleys onto grabcad. Will post the link asap.
```

---
## \#34 Posted by: TowerCrisis Posted at: 2019-05-11T05:23:38.047Z Reads: 26

```
https://grabcad.com/library/zombie-hawgs-75mm-wheel-with-36t-htd-5m-pulley-1

Here it is.
```

---
