# How-To/HACK: Build compact controller using GT-2B &amp; Badwolf v2 Enclosure

### Replies: 56 Views: 14420

## \#1 Posted by: sl33py Posted at: 2015-08-18T16:32:48.337Z Reads: 657

```
Sharing a [url=https://endless-sphere.com/forums/posting.php?mode=edit&f=35&p=1085783&sid=bb5b11d2b7ef6deb18b9a11fbc93ff44]post from ES[/url].  

Credit to Badwolf and others who have obviously developed and done this before.    

Besides Badwolf's directions on thingverse, and some detail from others here on how they did theirs - there wasn't anything consolidated in one spot.  I'm a visual person and since couldn't find a step-by-step, i figured i'd build one while doing mine.  Hopefully to help out the next person who wants to do this, and give back to the ES community that's helped me so much!

I had some spare time today and figured i'd give it a shot.  Others might have more elegant or better steps, but these worked for me.  This does involve your ability to solder and handle delicate electronics safely.  If you really have no idea how to do this, i might suggest you get someone to help you.

[img]/uploads/db1493/original/1X/3c4e5b7beb0077f9d492844c0d73b039a500caa4.jpg[/img]
I have my HK GT2B, and the 3dhub printed Badwolf v2 enclosure (bit rough print quality, but not horrible):

[img]/uploads/db1493/original/1X/7d26deb1c8722ae6158eeb5091d911560274cb7e.jpg[/img]
There are 8 screws on the side (and under replaceable "backstrap" replaceable grip.  Cut or remove the top sticker behind antenna to split it in half).

Take your time.  There are a couple other screws on the CH3 mid grip, and 3 more on the steering servo/wheel control.  The antenna is super simple and just sticks up into the rubber ducky on top of the controller.

[img]/uploads/db1493/original/1X/49afa24c2fca57fbc513921f9e1cbfa6bdd79654.jpg[/img]
Top
[img]/uploads/db1493/original/1X/1c8aeb0823dfbfd0d8110a57c7c6ed2928e427fc.jpg[/img]
Bottom
Once everything is pulled out you should have this.

[img]/uploads/db1493/original/1X/a92dd47e61ea81bcb7ea965f6f364a8448ad7633.jpg[/img][img]/uploads/db1493/original/1X/1e4018941e2a1fff61661e9dd26d155139254427.jpg[/img]
Pop the labeled cover off, and disconnect the Steering channel.

[img]/uploads/db1493/original/1X/b4c391e4e0738282a637db342e5ce24fa76d841c.jpg[/img]
Looking at alignment and test fitting to v2 enclosure.

[img]/uploads/db1493/original/1X/1bf27e40a3895db8819b7a1df413079226133a32.jpg[/img]
[img]/uploads/db1493/original/1X/02a8cbb4a8dc2d12530788b3956c760084bbfa76.jpg[/img]
Top and Bottom of left side to remove.

[img]/uploads/db1493/original/1X/d105342baf433adb9166fd9ec1503db994835258.jpg[/img]
[img]/uploads/db1493/original/1X/37cb97c120435eb42297e8334d8306dd37b1af8f.jpg[/img]
slow and steady w/ a dremel cutting disk

Let me just say that i SUCK at desoldering... couldn't find my solder wick and finally resorted to slightly more "brute force" methods.  
[img]/uploads/db1493/original/1X/0b4432897dbd3ef98b0615992ff347b134a862ba.jpg[/img]
On each side of the USB Mini-B charging port there is this solder you need to remove.  Desolder or...

[img]/uploads/db1493/original/1X/bf4c67c7b6544ef7dd345bbe7315815da77579d0.jpg[/img]
I quickly grinded it off with the dremel cutting disk and then used my razor knife to "lift" it while heating the top and bottom solder/pins.
Time consuming and a PITA.  If you have good solder wick i think you'd have this done in just a few minutes.  I went slow and fiddled with it for entirely too long, but got it done eventually.

Battery steps:
[img]/uploads/db1493/original/1X/e3a757326c83af401b871e70fccdf955cf4ee388.jpg[/img]
Pry/peel off the plastic and cover around the battery.  I immediately made sure to label + and - , just to be extra sure i dont mix them up.

[img]/uploads/db1493/original/1X/44794d66be76ec3d59921e395eb05f435d490870.jpg[/img]
Test fit in other half of enclosure.

Waste not want not
[img]/uploads/db1493/original/1X/f47685f774bafd20ea8b926bc7717ad545a339de.jpg[/img]
Donor wires for both the battery and relocating the USB charging port (don't throw these away).

[img]/uploads/db1493/original/1X/a9fe2488bb94577efdac929e5c9c77cc9135db49.jpg[/img]
A bead of solder on the + and - terminals on the battery, notice i kept the connector for the battery to connect to the PCB.  Instead of hard wiring/soldering it later i could replace it easily.

[img]/uploads/db1493/original/1X/6cc62166de236682e7f01c1899d2d873b2d1915b.jpg[/img][img]/uploads/db1493/original/1X/fbf6f8ff8b3f10fcbf988ff57c72dd154fb1d653.jpg[/img]
Some electrical tape around the perimeter then gorilla taped it up.

[img]/uploads/db1493/original/1X/819264714be64da5b6d67c0b6837604278e75436.jpg[/img]
a simple loop of the antenna and electrical tape to hold it in place at the bottom.

I was going to run to the hardware store for the extra m3 screws i needed, then remembered i had this [url=http://smile.amazon.com/Teenitor-Spacers-Stand-off-Accessories-Assortment/dp/B00LGB2N1Q]"standoff kit" from Amazon[/url] for a quadcopter KK board - perfect!
[img]/uploads/db1493/original/1X/d19caf87d7b7571c449a41f1fcef88cce65a4fce.jpg[/img][img]/uploads/db1493/original/1X/2b54c42b45a52b2e3df96b6176f570060a1d0e99.jpg[/img]

Getting close to completed.  I'm not sure if it was just my print, or if all of them are going to be like this, but i found the range too restricted for full throttle to full brake on my enclosure.
[img]/uploads/db1493/original/1X/27c1dcdbe04a23f8bacea6b857c4a6ec12f3fdb7.jpg[/img][img]/uploads/db1493/original/1X/679f1ff59b2019db0e669299939d3e839696657c.jpg[/img]
I got it pretty well lined up.  Notice the almost flat bar extending out from the trigger pivot.  I marked it w/ a sharpie to cut and tried to keep it snug for good stability (going to be pulling/pushing on it).  I also notched out the part that slides down onto the m3 bolt so it went around both the bind and one of the adjustments (throttle iirc).

[img]/uploads/db1493/original/1X/e5fc45bb537cc9916696c3fee3ca8d1bf5a85c85.jpg[/img]
Bent the backside of the throttle/trigger board to sit flat (but contact the enclosure for more support).

[img]/uploads/db1493/original/1X/3536f5e42311180f04c0e6b074accacfe999dbbc.jpg[/img]
You can see how much i cut away to give full throttle range.

[img]/uploads/db1493/original/1X/f88e502fc1d6b5602dc903078e4c864c54814169.jpg[/img]
re-using the wires from the handle, the 3 wires to the USB Mini B charging port

[img]/uploads/db1493/original/1X/fd356aa554d37cb66d2d8a53b8e03d67855e1bd9.jpg[/img]
A bit of a closeup of the battery and charging ports.  Note that the USB charging port does use all 3 wires, but since i had to mangle it a bit when desoldering the port, i put the white wire in the middle to the bottom side (more room to work at the time as well).  So top has black and red, with the middle white connected on the bottom.  You can also see the notched out part of the throttle assembly to clear the bind button and throttle adjustment.  To keep it straight (what does what), i used the label from under the top cover to help keep them ID'd.

[img]/uploads/db1493/original/1X/95fb4879a0a0d8b742777077835480c9ff0f9823.jpg[/img]
Pretty much ready to screw it together and test.  Note - use the shorter screws to hold the halves together.  The longer ones i tried on the two bottom broke off part of the screw hole they went into.  I used the shorter screws on the top 2, then used the longer ones on the two bottom holes.  If you brake off the screw hole bottom piece - just re-use the longer screws.  I've had it apart a few times already and seems to be holding up ok w/ me being careful not to try to tighten it down too much.  Could be typical, or just the lower quality print (medium quality on 3dhub)...  

Moment of truth:
[img]/uploads/db1493/original/1X/7fdbd77091ddec7fec52d21915e92788f0a44eb5.jpg[/img]
plugged in and charging!  I then got it to bind up and control my board w/o any trouble.

Some issues i had:
- On/Off extension did not line up for me.  So i have to use a straw/keys/long-pokey-thing to turn it on.
- Broke the bottom 2 screw holes w/ longer screws from too much force/too thin or poor quality print, or gunk in the screw hole splitting it?
- I'm an idiot.  I wanted to dye the plain white PLA printed enclosure.  Directions on the RIT dye say to use boiling water.  [b]Don't do that.[/b]  One of the two enclosures is permanently warped.  Hot tap water actually did great cleaning up the adhesive residue w/ some soap before mounting the electronics into it.  seemed to also make the enclosure less "flexy" and more rigid w/o warping it.  I think my hot water heater is set around 125*.
- 680 Ohm resistors - not currently used.  Seems to work fine, but wanted to try it both ways.  (anyone with specifics on why you need them please chime in!)

I have 100 of the 680 Ohm resistors.  If anyone needs a pair for their new enclosure, just PM me.  I'll ask you to send a stamped envelope so i can drop them back in the mail to you.  

Bench testing this worked fine.  Will try to get it out and ride it soon.  Great conversion on the GT2B - now fits in my pocket!!

I hope this helps the next person trying to do this, and let me know if you have questions.  (Please like this post if it helps you)

-Rob
```

---
## \#2 Posted by: longhairedboy Posted at: 2015-08-18T18:24:06.730Z Reads: 442

```
This is an excellent post! Thanks for sharing. I've had a printout of BadWolf's mod shell sitting on my desk for months now, and i keep finding other things to do besides start this project. Things like fiberglassing a new enclosure and setting inlaid motor wires (as in epoxied into channels in the deck) between my box and the rear truck, which i will be posting here very soon. 

But what has me so very interested in this particular post is that you used the existing battery pack. The mod tuts I've seen suggest buying a smaller lipo pack to squeeze it into the remote handle. Here you didn't have to do that. I think tonight when I get home i'm going to take another look at my GT2B battery and see if the badwolf version I have printed out will take it. If so, I have less of an excuse for not doing this.
```

---
## \#3 Posted by: sl33py Posted at: 2015-08-18T21:07:30.265Z Reads: 402

```
His v1 (angular edges vs rounded) still requires a smaller battery.  And relocating the power switch (which i might end up doing since mine doesn't line up).
```

---
## \#4 Posted by: lowGuido Posted at: 2015-08-18T23:02:13.273Z Reads: 378

```
this is a really good how to. you have made a much nicer control than the clunky GT2B.

however it does seem like a lot of work when the wii nunchuck is readily available and practically plug and play.
```

---
## \#5 Posted by: sl33py Posted at: 2015-08-18T23:06:39.370Z Reads: 365

```
True.  I actually really like my wiiceiver setup on GF's board.  BUT in some areas w/ lots of 2.4 interference - it disconnects *frequently* which sucks.  Luckily I've never had any major issue, but i've heard horror stories about run-aways and crashes as a result.

GT2B is rock solid and rechargeable.  Now it's also pocketable!
```

---
## \#6 Posted by: lowGuido Posted at: 2015-08-18T23:24:45.182Z Reads: 345

```
[quote="sl33py, post:5, topic:114"]
y wiiceiver setup on GF's board.  BUT in some areas w/ lots of 2.4 interference - it disconnects frequently which sucks.  Luckily I've never had any major issue, but i've heard horror stories about run-aways and crashes as a result.
[/quote]

I have solved the wii ceiver drop outs by soldering the nunchuck reciever dongle direct to the board. no more drop outs.
```

---
## \#7 Posted by: torqueboards Posted at: 2015-08-19T05:47:56.058Z Reads: 328

```
Nice @ lowGuido. I'll keep that in mind. Do you have your Wiiceiver set away from your motor wires?

GT2B is 100% rock solid. I need to make a new badwolf enclosure that doesn't require any soldering or re-positioning any components.
```

---
## \#8 Posted by: sl33py Posted at: 2015-08-19T17:08:33.780Z Reads: 326

```
Hey Torque - i think this is doable w/ a bit of ingenuity.  I think you could knock out a square'ish hole for the USB charging port to stick out the back bottom of the case.  It would probably poke your palm if you have a death grip, but perhaps a small piece of sugru to mold it would probably work!

The desolder and reposition of the USB charging port was definitely the hardest part for me.  With some desolder wick and practice it shouldn't be too hard.  I just suck at desoldering i think.

Don't forget lots and lots of hot glue!  Mine is not going anywhere, anytime soon...
```

---
## \#9 Posted by: lox897 Posted at: 2015-08-20T06:09:53.091Z Reads: 326

```
Hey sl33py, I think that the white wire is the data cable. I might be wrong but maybe it delivers the signal when channel 3 is clicked?
```

---
## \#10 Posted by: sl33py Posted at: 2015-08-20T13:43:39.585Z Reads: 351

```
@lox897 - yes, that makes sense.  Two wires from battery, then 3 from CH3 switch (in grip handle) to the power plug on PCB.

When i saw Badwolf use 3 wires on his v1 setup, i simply mirrored that on this v2 setup.  The desoldered USB Mini-B charging port has 3 wire leads to connect to.  Unsure what the 3rd wire is used for, but it doesn't hurt to have it from my experience (charging fine).  Likely not needed though.

Here's the v1 image i saw that showed the 3 wires used for the USB charging port:
[img]/uploads/db1493/original/1X/d87d1e8606c3a53aa0d39ebff09e9875e14b6bc6.jpg[/img]
```

---
## \#11 Posted by: lowGuido Posted at: 2015-08-20T16:30:27.086Z Reads: 338

```
how do you guys using the GT2B go about cruising? is it easy enough to hold a consistent speed? maybe my next build will use a GT2B.
```

---
## \#12 Posted by: sl33py Posted at: 2015-08-20T16:47:20.095Z Reads: 329

```
Definitely easy to cruise.  While you don't have a "cruise control" button like wiiceiver, i haven't had issue holding a steady speed on my longer 6-9mi cruises.  BUT that is with a fair number of people traffic so quite a bit of slowing down and re-accelerating as well.

Even if you don't convert into the smaller badwolf enclosure, the GT2B is a *fantastic* Tx!
```

---
## \#13 Posted by: cmatson Posted at: 2015-08-20T17:14:40.542Z Reads: 328

```
I have two GT2B controllers, one wii receiver, and two boards. 

the wii receiver has been used a few times, but the GT2B is just solid- the only negative being size, which still, isn't too bad. Not only is it still easy to maintain a cruising speed, but I just feel like the throttle inputs are much more precise and less jerky. You also don't have to worry about pairing it, or the signal cutting out.. it just plain works.
```

---
## \#14 Posted by: longhairedboy Posted at: 2015-08-21T19:16:37.033Z Reads: 323

```
ditto on all of that. I love my GT2B. Even on hour and a half cruises at lower speeds its no problem. Also, its tough. I've dropped mine i don't know how many times and have even broken it, but its easy to fix when it does break and it takes quite a beating to break it.
```

---
## \#15 Posted by: longhairedboy Posted at: 2015-10-01T17:54:54.448Z Reads: 326

```
i just uploaded the v2 models from Thingiverse into Shapeways and it looks like its about $50 to have all three pieces printed there in strong, polished plastic. For those of us without access to a 3D printer, that's not a terrible deal, especially since you can get it in just about any color you want, though they seem to have slightly different prices for colors than for black or white, but it only varies by about a dollar. That puts you at about $70 or $80 total if you include the price of the remote itself. 

You can also get your Bad Wolf in stainless steel for about $150 if you so desire. Or even porcelain for around $70 if you want to print one for grammy's curio. They do different materials for the switch because its a smaller size, so don't be afraid to drop $430 on an 18k Gold switch if you just have to have that bling. lol

Importantly, USPS First Class shipping looks to be about $5 for these parts. This is certainly one case where they've got UPS Ground beat by a large margin.
```

---
## \#16 Posted by: sl33py Posted at: 2015-10-01T20:01:29.880Z Reads: 316

```
I did the same for my last two (i have 3 now).  I go the polished strong plastic as well.  Nice matte look.  Unfortunately i don't think it's as thick as one i got just doing cheap-o PLA from 3dhubs.  Much nicer finish, but thinner walls and the screw holes sucked to hold it together.  Ended up ghetto gluing it together so if it ever breaks it'll be a PITA to get into and fix.  But looks good in orange and pink matte.

I'd really love to see a v3 with thicker walls throughout.  Sturdy and make the screw holes more secure.
```

---
## \#17 Posted by: lowGuido Posted at: 2015-10-02T00:18:31.452Z Reads: 312

```
question to you guys that are stateside, how much is a nyko karma delivered?
```

---
## \#18 Posted by: sl33py Posted at: 2015-10-02T00:33:54.834Z Reads: 308

```
I have a couple.  Typically around $10 on ebay shipped.  Might need a little searching but that was my going rate a while back.
```

---
## \#19 Posted by: lowGuido Posted at: 2015-10-02T00:37:52.618Z Reads: 316

```
far out.. cost me like $40 AUD to get one here..

on topic.. has anyone tried vacuum molding ABS into a shape like bad wolf's box?
```

---
## \#20 Posted by: psychotiller Posted at: 2015-10-02T00:50:11.519Z Reads: 305

```
I may try something soon.
```

---
## \#21 Posted by: longhairedboy Posted at: 2015-10-02T16:24:31.354Z Reads: 276

```
i've been thinking a lot about that. It would take some trimming/finishing work to get it all straight, but the electronics are so rock solid reliable that I'm not even sure you really ever need to crack open the case, so things like screw posts likely aren't even necessary when you can just spot-hot-glue or plastic weld the thing together. You could always crack it open again with a dremel.
```

---
## \#22 Posted by: lowGuido Posted at: 2015-10-02T22:30:01.073Z Reads: 273

```
I was thinking nylon nuts/botls straight through the case.. I cant imagine 3D printed screw posts lasting too long anyway.
```

---
## \#23 Posted by: sl33py Posted at: 2015-10-05T21:25:41.225Z Reads: 281

```
OKP did a gorgeous hand laid CF case for his!  It's a work of art.  He put in screw retainers as well to secure it.  Great work and i'm just lazy with my 3d printed Badwolf enclosures...
```

---
## \#24 Posted by: lowGuido Posted at: 2015-10-05T21:40:39.168Z Reads: 272

```
1yeah i saw that too. I was thinking about making a carbon fibre case if i ever go the gt2b route
```

---
## \#25 Posted by: treenutter Posted at: 2015-11-24T19:59:11.714Z Reads: 277

```
[quote="lowGuido, post:6, topic:114"]
I have solved the wii ceiver drop outs by soldering the nunchuck reciever dongle direct to the board. no more drop outs.
[/quote]

Hey @lowGuido do you have a  pic of the Nyko Kama receiver soldered to the PCB of wiiceiver? I keep trying to picture this and I can't figure it out...
```

---
## \#26 Posted by: lowGuido Posted at: 2015-11-24T23:11:01.724Z Reads: 279

```
its covered in heatshrink so I could take a photo but it wont really show the wiring.

Edit
You might need to use your imagination a little 
<img src="/uploads/db1493/original/2X/b/b6db11d2f47b2265c0444886c515e43725841491.jpg" width="690" height="388">
```

---
## \#27 Posted by: treenutter Posted at: 2015-11-30T15:39:29.271Z Reads: 275

```
thx @lowGuido ! This helps but how do you solder the contacts points on the Nyko Kama receiver to the wiiceiver? Do you tin all three contact points on the plug and then melt each with very small solder iron tip? Or maybe use short wires between the dongle and the wiiceiver? Here it looks like you removed the casing (and the plug) from the NK dongle. 

I've switch over to the GT2B camp until I can sort out a more reliable nunchuck solution! I miss perpetual steez!
```

---
## \#28 Posted by: lowGuido Posted at: 2015-11-30T20:58:36.020Z Reads: 273

```
I tinned the contacts on the wiiceiver and then I removed the PCB from the nunchuck dongle and soldered the wires directly to the contacts.
```

---
## \#29 Posted by: cmatson Posted at: 2016-01-14T01:40:22.704Z Reads: 278

```
<img src="/uploads/db1493/original/2X/2/2cd3874428f6edcd070539ad6238908f0f15cc76.jpg" width="500" height="500">

I'll be doing this some time after mid term exams!

Pretty good print on 'medium' (except for the supports stuck on the edges.. not too hard to get off though) with a makerbot 5th gen.
```

---
## \#30 Posted by: NerijusM Posted at: 2016-01-24T16:34:16.272Z Reads: 283

```
Made a mod and video about that.
https://www.youtube.com/watch?v=2pFNdJmjMkg
```

---
## \#31 Posted by: treenutter Posted at: 2016-02-27T17:50:47.140Z Reads: 277

```
Here is OKP's carbon mod. A work of art!

https://www.youtube.com/watch?v=QTgnRmonFzo
```

---
## \#32 Posted by: NIK Posted at: 2016-03-31T16:16:02.498Z Reads: 280

```
Hi guys, i have a new flysky gt2b, and sometimes it will produce drop out when riding. Do u guys happen to know how to correct that? thanks
```

---
## \#33 Posted by: Freeflyer Posted at: 2016-04-04T01:46:14.034Z Reads: 290

```
Just finished putting this case I got from eBay together. Quality seems good with 3mm walls and only had to do very minimal dremel work. It looks like the bad wolf v2 as I did not have to de solder the USB port. I added two 470ohm realtors to the steering channel. Spins an rc motor on testing and range is fine. Now I just need my Carvons and space cell!!!

https://www.ebay.com/ulk/itm/252330751004 

<img src="/uploads/db1493/original/2X/e/ea1f03514f0cdbc56ea761045b1b762ac5eb2b73.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/d/d2524d492e00a500bbcc6b9aafca14f6a898d900.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/9/90ca4c4e1a8ebb66c36eb00fe0ad39e3e1ed8077.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/3/3b9e59f385ee4b9d24c4fa36752324f7c522798c.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/a/a8ece2884e2d99f2f5667094730ebde30e1f51ea.jpeg" width="375" height="500">
```

---
## \#34 Posted by: Ulfberht Posted at: 2016-04-04T06:50:55.571Z Reads: 268

```
NIce work! much nicer looking than the Badwolf mod. IMO.
```

---
## \#35 Posted by: broshi Posted at: 2016-04-12T16:41:55.368Z Reads: 266

```
how do you apply breaking on that build?
```

---
## \#36 Posted by: Freeflyer Posted at: 2016-04-12T17:55:19.809Z Reads: 281

```
Push the trigger out like any other r/c car transmitter. The enclosure does not alter the function of the trigger
```

---
## \#37 Posted by: FLATLINEcustoms Posted at: 2016-04-13T13:55:10.773Z Reads: 290

```
@freeflyer did you design that or just purchase from ebay?
```

---
## \#38 Posted by: Mobutusan Posted at: 2016-08-07T08:32:24.275Z Reads: 256

```
I don't know if this is on topic enough for this thread, but can anybody tell me how the Mad Munkey or Master Cho mods differ from this Bad Wolf tutorial? Is there less de/resoldering, battery disassembly or PCB cutting involved?

Paging @FLATLINEcustoms & @MasterCho...
```

---
## \#39 Posted by: sl33py Posted at: 2016-08-07T19:57:08.344Z Reads: 268

```
[quote="Mobutusan, post:38, topic:114"]
Is there less de/resoldering, battery disassembly or PCB cutting involved?
[/quote]


@Mobutusan - looking at the pics above of Master Cho's enclosure (Purchased via ebay it seems) - the PCB is not cut (you can see the left side wires routing through the notch i cut off).  The usb charging port is not moved.  And the battery is connected w/ the regular/stock connector.  So besides notching the trigger and cutting off to fit in top left of case it looks relatively mod-less.  

I have two more GT2b's on order and looking forward to trying flatline's or baby buffalo mods to compare w/ my badwolf ones i've done previously.  I would consider Master Cho's as one of the least modify necessary, but since there is no open source files (free) - i'm not willing to pay the $30 to try.  my .02 as there are several others that are as good or better possibly for free.
```

---
## \#40 Posted by: FLATLINEcustoms Posted at: 2016-08-08T15:43:22.845Z Reads: 239

```
@Mobutusan, The Mad Munkey V1 is the same as the build for the Bad Wolf except the trigger piece needs to be cut shorter and the battery needs to be covered. But I believe that is it.
```

---
## \#41 Posted by: Raf Posted at: 2016-08-09T21:51:25.251Z Reads: 222

```
I'm having trouble figuring out the wiring setup for the battery? can anyone help me, i don't understand why you have to desolder the mini usb and how to wire it for the charging?

All i know is you plug the RBW wire on the PCB and the other side goes to the battery.
```

---
## \#42 Posted by: sl33py Posted at: 2016-08-09T21:59:16.096Z Reads: 229

```
[quote="Raf, post:41, topic:114, full:true"]
I'm having trouble figuring out the wiring setup for the battery? can anyone help me, i don't understand why you have to desolder the mini usb and how to wire it for the charging?

All i know is you plug the RBW wire on the PCB and the other side goes to the battery.
[/quote]


It's pretty straightforward.  Just ignore the white wire if you want to be even easier (not needed for charging).

desolder the USB - then add any wires you'd like (i reused some) to the + and - like this:
[img]http://www.electric-skateboard.builders/uploads/db1493/optimized/1X/f88e502fc1d6b5602dc903078e4c864c54814169_1_281x500.jpg[/img]

Then at the bottom you reconnect the + and - to these contacts:
[img]http://www.electric-skateboard.builders/uploads/db1493/optimized/1X/fd356aa554d37cb66d2d8a53b8e03d67855e1bd9_1_432x500.jpg[/img]
(see them just to the right and above the blue radio module?)

That help clarify for you?
```

---
## \#43 Posted by: Raf Posted at: 2016-08-09T22:06:48.391Z Reads: 205

```
so you have a black and red wire attached to the USB (image above) and those wires go around to the other side of the PCB  above that blue module?
```

---
## \#44 Posted by: Raf Posted at: 2016-08-09T22:10:37.873Z Reads: 213

```
like this?

<img src="/uploads/db1493/original/2X/a/a4480e9b0e6efbdbd2145e79a84cbd8017374391.png" width="620" height="386">
```

---
## \#45 Posted by: sl33py Posted at: 2016-08-09T22:22:56.612Z Reads: 210

```
No!

You remove/desolder the USB charging port.  You connect wire from that USB plug from the red/black to +/- on it - down a few inches on the PCB (the brains of the GT2b) - to the bottom right connections.  In my pic you can see them just above and to the right edge of the blue radio module - i have them sunk into hot glue to insulate.

That make more sense?
```

---
## \#46 Posted by: Raf Posted at: 2016-08-09T22:39:27.054Z Reads: 208

```
so those two wires i connect to the usb plug goes there on the bottom right like the picture?
```

---
## \#47 Posted by: sl33py Posted at: 2016-08-09T22:56:25.395Z Reads: 219

```
When you remove the module - all you are doing is reconnecting the contacts w/ wire in-between to move the USB up to the top location.  So if you mark the USB plug and the PCB as you remove it - they should be easy to identify what to reconnect.

here you can see the bottom of the board - as you remove the USB plug you can mark what wires to connect A->B:
[img]http://www.electric-skateboard.builders/uploads/db1493/optimized/1X/bf4c67c7b6544ef7dd345bbe7315815da77579d0_1_281x500.jpg[/img]
```

---
## \#48 Posted by: Raf Posted at: 2016-08-09T22:59:27.923Z Reads: 211

```
Thank you for your help. I understand now, I have the mod  made by @MasterCho and he's just let me know I don't have do anything with the USB port as the mod is perfect size for it
```

---
## \#49 Posted by: sl33py Posted at: 2016-08-09T23:05:14.895Z Reads: 222

```
Wow.  OK.  that would've been good to know as the thread is about GT2b into badwolf enclosure...
```

---
## \#50 Posted by: Raf Posted at: 2016-08-09T23:06:35.267Z Reads: 224

```
Yeah sorry about that, I didn't realise his mod was specifically built for this reason
```

---
## \#52 Posted by: Rob69de Posted at: 2016-10-28T23:00:26.772Z Reads: 173

```
just finished the install.
was woried my battery was to big, but than i saw badwolf, took it apart, and it was much smaller.
<img src="/uploads/db1493/original/3X/7/b/7ba5cc4351c4f4ae3a589b304ccb2cee2f0e9292.jpg" width="281" height="500">
```

---
## \#53 Posted by: Blacksheep Posted at: 2017-04-24T01:51:53.470Z Reads: 114

```
Where do you buy this ?
```

---
## \#54 Posted by: Smorto Posted at: 2017-04-24T01:56:15.579Z Reads: 113

```
There are files here on the forum, just search up OKP GT2b mod and it should come up.
```

---
## \#55 Posted by: Blacksheep Posted at: 2017-04-24T02:02:58.688Z Reads: 116

```
Ok thanks 😀
```

---
## \#56 Posted by: Conor Posted at: 2017-06-14T01:24:57.349Z Reads: 90

```
So what does the white wire do/where is it Connected?
```

---
## \#57 Posted by: sl33py Posted at: 2017-06-14T03:22:43.864Z Reads: 78

```
[quote="Conor, post:56, topic:114, full:true"]
So what does the white wire do/where is it Connected?
[/quote]

I'm guessing you are talking about the Mini USB center white wire?  I think it is for data.  Others have done only the red and black w/o issue.

[quote="sl33py, post:10, topic:114"]
When i saw Badwolf use 3 wires on his v1 setup, i simply mirrored that on this v2 setup.  The desoldered USB Mini-B charging port has 3 wire leads to connect to.  Unsure what the 3rd wire is used for, but it doesn't hurt to have it from my experience (charging fine).  Likely not needed though.

Here's the v1 image i saw that showed the 3 wires used for the USB charging port:
[img]https://www.electric-skateboard.builders/uploads/db1493/original/1X/d87d1e8606c3a53aa0d39ebff09e9875e14b6bc6.jpg[/img]
[/quote]
```

---
