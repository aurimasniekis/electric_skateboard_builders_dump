# Dude Hubs - In Depth Dual Hubmotor Build

### Replies: 76 Views: 8072

## \#1 Posted by: The_Dude Posted at: 2017-04-21T19:39:08.235Z Reads: 521

```
Hi,
if you are interested how to convert an conventional outrunner to a hubmotor, this thread is thread is for you! I started this build more than a year ago - after some ups and downs I finally arrived at V2, which seems to work quite well. My first V1 looked like this

<img src="/uploads/db1493/original/3X/6/b/6bfda36609a82fbc220381b9e6439d40a35afd39.JPG" width="666" height="500">

... but the design had some thermal issues so to say (more about that later :grin:). But let's start from the beginning. The deck is a **Hackbrett Himmelreic**h (Flex 1) made in the black forest (south of germany) with **Paris Trucks** (195 mm), **Blanc Longboard Wheels** (90 mm), 2 x **VESC 4.11**, 2 x **APS6374 3.2 kW** (130 kV).

<img src="/uploads/db1493/original/3X/b/e/be95b1fbb5dbe5d54780b0f1e37c0d5c323371a3.jpg" width="666" height="500">

Technical drawings can be found in [Dude Hubs](https://www.dropbox.com/sh/5rwq2u1h83tnqbc/AABitDwG0UPnjqippgnFCq-Sa?dl=0).
```

---
## \#2 Posted by: Surfer Posted at: 2017-04-21T19:42:25.951Z Reads: 489

```
Mr Dude, we want more!!
```

---
## \#3 Posted by: Tuomalar Posted at: 2017-04-21T19:51:30.043Z Reads: 485

```
More info and pics!
```

---
## \#4 Posted by: The_Dude Posted at: 2017-04-21T20:11:53.229Z Reads: 491

```
For the BLDC outrunner I wanted a motor with low kV - protecting the VESC from being a heating plate (low current rules) and protecting me approaching speed of light using reasonable voltage @ 8-12s. At the time when I started my build the lowest available kV motor e.g. from APS was a 6374 130 kV with reasonable 3.2 kW power. I also thought about using a 6350 - could have been completely put inside the wheel - but these motor had really too high kV when designed for 3.2 kW. Another advantage I realized first after my V1 was build was that the motor length of 74 mm offers additional cooling area which indeed is needed (more about that later).
The first step I did was to convert the motor winding from Delta to Wye. How this can be done is described by @Duffman  somewhere on the forum I suppose. 

<img src="/uploads/db1493/original/3X/d/a/da1c8ae6e5fc83d118b478314a1d9f00dca45b96.JPG" width="375" height="500">

Doing so, the motor kV is further reduced by a factor of 1.7 resulting in 39km/h (8s, no losses, pure kinematics) with my 90mm wheels. Additionally the torque increases in the low rpm range.
```

---
## \#5 Posted by: The_Dude Posted at: 2017-04-21T20:18:42.490Z Reads: 484

```
This is how my motor looks when disassembled

<img src="/uploads/db1493/original/3X/e/9/e94e56996f6c203e245b0a0ec753ece2bf5c9c35.jpg" width="666" height="500">

and this is how I wanted the motor to look like after the transformation

<img src="/uploads/db1493/original/3X/e/6/e64742817170aaf8d45bc444719db2425faee835.jpg" width="549" height="500"><img src="/uploads/db1493/original/3X/5/a/5a36165945e7c41deee1bade9772af2fe54882db.jpg" width="558" height="500"><img src="/uploads/db1493/original/3X/a/4/a44b0f0a0d81211e6bebbac35e022c30277ce9fd.jpg" width="690" height="409">

Obvious to see, that compared to my first attempt there are several real ventilation slots. 

In the following posts I will describe the details of the construction and the practical issues I was facing in more detail. For the sake of simplicity here is a drawing of the cutting plane:

<img src="/uploads/db1493/original/3X/0/e/0e5c0ebc80047fae70ce623658c85cd4f5753c02.jpg" width="484" height="500">

>  1: urethane wheel
>  2: front cover
>  3: back cover
>  4: motor can (rotor)
>  5: anker (stator)
>  6: stator insert
>  7: stator endplate
>  8: axle (cast aluminium)
>  9: clamping sleeve
> 10: mounting nut
> 11: circlip
> 12: front bearing
> 13: back bearing
> 14: screw

If desired I can also post the 2D drawings later on. Please keep in mind that they are released under the license of Creative Common License "Attribution-NonCommercial-ShareAlike 4.0 International" [https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode) and you automatically agree to the license terms when using.
```

---
## \#6 Posted by: Rollbrett Posted at: 2017-04-21T22:06:40.001Z Reads: 450

```
Nice thread! I hope you'll be covering some details of the shaft-hub-joint as well.
```

---
## \#7 Posted by: caustin Posted at: 2017-04-21T22:39:00.362Z Reads: 446

```
Awesome work, congrats and thanks for sharing. Look forward to seeing more!
```

---
## \#8 Posted by: Wubbalubbadubdub Posted at: 2017-04-22T07:02:14.762Z Reads: 437

```
You are truly the dude of your time and place. Where are you in the black forest? I live near Stuttgart.
```

---
## \#9 Posted by: The_Dude Posted at: 2017-04-22T07:29:36.927Z Reads: 427

```
@Wubbalubbadubdub  Me too - almost right in the middle between Karlsruhe and Stuttgart.
```

---
## \#10 Posted by: Wubbalubbadubdub Posted at: 2017-04-22T07:31:13.078Z Reads: 425

```
Sindelfingen. I have seen others on the forum from around this area. We should organize a ride or something. I mean, in a non-chalant place.
```

---
## \#11 Posted by: Nordle Posted at: 2017-04-22T12:30:39.083Z Reads: 427

```
Nice work! what is holding urethane on the motor can?
```

---
## \#12 Posted by: The_Dude Posted at: 2017-04-22T14:54:18.803Z Reads: 454

```
Just added some numbers to the cutting plane in my previous post to facilitate the description.
>  1: urethane wheel
>  2: front cover
>  3: back cover
>  4: motor can (rotor)
>  5: anker (stator)
>  6: stator insert
>  7: stator endplate
>  8: axle (cast aluminium)
>  9: clamping sleeve
> 10: mounting nut
> 11: circlip
> 12: front bearing
> 13: back bearing
> 14: screw
## Rotor and Wheel
I wanted to move the complete motor as far as possible inside the wheel (1) to get a minimum protrusion on the back part of the hub motor but also to maintain the trackwidth. Therefore the red anodized rotor cover was completely turned off the motor can. This has to be done quite carefully, in ordern not to damage the magnets.

<img src="/uploads/db1493/original/3X/a/3/a3f07536dc1dcffddb0ba030d001c06abecaecd5.JPG" width="375" height="500">

This opened up the possibility to make a complete redesign of the front cover (2), bearing a bigger (bigger than the usual 8 mm ones) front bearing (12) while giving it a nice looking front too. The fixed bearing (12) is held in place by the circlip (11).

The urethane wheel was completely drilled out with the diameter of the motor can. So the only way to fixate the wheel on the rotor can was using adhesive. This was the price I had to pay in order to move the motor as far as possible inside the wheel, so that there is nothing left from the former inner structure to get the inner motor hooked on the wheel. For bonding I choose _uhu endfest 300_ which seems to be strong but also elastic (at least until now). I read a lot in the forum about the slipping urethane issues some of you guys had so far. Imho the shiny surface of most outrunners, eventually together with a low number of "bumps" are not the best basis for a good adhesing, very durable connection. So I was lucky, that the older APS rotor cans have numerous groves on their outer surface - this is what adhesive needs. In addition to that I also sanded off the black coating on the can to a certain extend. I also thought of applying heat during the curing process to further strengthen the bonding but I didn't. I didn't want to weaken the magnets by applying a too high temperature. To conclude, so far I never had problems with slipping urethane - but I will keep my fingers crossed.

Now for the back cover (3) of the rotor. Normally, having an outrunner where the radial forces act on the rotating axle you have an open end. For the hubmotor you have to support the radial forces acting on the outer rotor not only from the front but also from the back. The back cover (3) which is indeed more like a sleeve, is also glued to the outer surface of the motor can. Last but not least, the back cover bears the large "loose" bearing of the hubmotor. 
Back and front cover are having several cooling slots to account for the generated heat inside the motor. By the way, the front cover is also glued to the rotor but to the inner surface of the motor can.

This is how it looks when assembled right before the wheel is fitted:

<img src="/uploads/db1493/original/3X/7/b/7b4c2801f53f0ece5813caf6b262172b28a5300f.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/3/0/3050294e1ff30ab0ce31d3287d6a34541bfe3d8c.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/b/c/bcd9233cac82ea89fba39061b142c72e437779b3.JPG" width="666" height="500">

And finally with wheel:

<img src="/uploads/db1493/original/3X/0/3/03c6fbd07ca874d3b5a2fed4fe9543f1a5d7009a.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/1/8/189ce9d1368f5a4fac073bf34cd1407a57ff28cc.JPG" width="375" height="500">
```

---
## \#13 Posted by: Surfer Posted at: 2017-04-22T15:37:30.532Z Reads: 413

```
Sh*t i cannot press more like it like it like it ... Amazing work dude keep it up
```

---
## \#14 Posted by: IsTalo Posted at: 2017-04-22T22:48:30.732Z Reads: 399

```
Hey man, do you have yours stl files? I want them to make the parts at the Cnc
```

---
## \#15 Posted by: IsTalo Posted at: 2017-04-22T22:59:25.228Z Reads: 407

```
[quote="The_Dude, post:4, topic:21519"]
to convert the motor winding from Delta to Wye.
[/quote]

Man, I don't found it. I also don't find anything about Delta and Wye, can you put a link or explain for me?
```

---
## \#16 Posted by: jdyer8989 Posted at: 2017-04-22T23:38:43.643Z Reads: 408

```
My guess is he was referring to this thread.

https://www.electric-skateboard.builders/t/lightweight-mbs-pro-90-dual-vesc-sensored-c6364-belt-drive-nrf/17143/5
```

---
## \#17 Posted by: chuttney1 Posted at: 2017-04-23T00:43:05.996Z Reads: 401

```
@The_Dude, Just to be sure. Part 8 is a cast aluminum axle?
```

---
## \#18 Posted by: The_Dude Posted at: 2017-04-23T05:48:10.537Z Reads: 398

```
@IsTalo @jdyer8989 exactly. There is also a german version available [http://www.elektro-skateboard.de/forum/eigenbauten-95/mbs-pro-90-4x-vesc-ntm5060-12s-4349-2.php](http://www.elektro-skateboard.de/forum/eigenbauten-95/mbs-pro-90-4x-vesc-ntm5060-12s-4349-2.php)
```

---
## \#19 Posted by: The_Dude Posted at: 2017-04-23T05:49:37.726Z Reads: 389

```
Yes, it's the aluminium cast of the truck after turning it on the lathe. I will describe this in more detail in the next post "Stator and Axle".
```

---
## \#20 Posted by: The_Dude Posted at: 2017-04-23T05:59:59.419Z Reads: 391

```
I will publish the 2D drawings you need at the end of the thread :wink:. Stl files won't be enough because you have to take care of several tolerances to get this thing running. The tolerances will be given in the drawings.
```

---
## \#21 Posted by: The_Dude Posted at: 2017-04-23T06:03:30.496Z Reads: 352

```
Yes, will be done in the next post "Stator and Axle".
```

---
## \#22 Posted by: Wubbalubbadubdub Posted at: 2017-04-23T08:02:01.428Z Reads: 357

```
that hub looks pretty smooth. do you have any issues with urethane slippage?
```

---
## \#23 Posted by: Rollbrett Posted at: 2017-04-23T08:53:13.596Z Reads: 361

```
Have a look at post 12:
[quote="The_Dude, post:12, topic:21519"]
so far I never had problems with slipping urethane - but I will keep my fingers crossed.
[/quote]
```

---
## \#24 Posted by: IsTalo Posted at: 2017-04-23T12:11:38.442Z Reads: 359

```
Thanks man, continue your topic, I'm anxious!
```

---
## \#25 Posted by: IsTalo Posted at: 2017-04-23T12:35:07.404Z Reads: 373

```
Thanks, but converting you'll have a 75kv motor, right? Could someone just buy the 60kv 6374 from alien? 
http://alienpowersystem.com/shop/brushless-motors/alien-6374-outrunner-brushless-motor-60kv-3200w/
```

---
## \#26 Posted by: The_Dude Posted at: 2017-04-23T13:16:10.379Z Reads: 396

```
Right - maybe the 90 kV will work too, depending on your desired speed. I would strongly recommend to use the sensored ones (together with FOC it's a dream) but actually I don't know if this will fit in the current design of my hubs. Will show you in a later post how I retrofitted hall sensors in my motors with minimum space requirements.
```

---
## \#27 Posted by: The_Dude Posted at: 2017-04-23T20:26:33.184Z Reads: 409

```
## Stator and Axle
The stator insert (6) is press fitted already by the manufacturer into the anchor (5). The insert has to be turned down in the outer diameter to fix the inner ring of the back bearing (13). 

<img src="/uploads/db1493/original/3X/3/5/35fae6a48303f37d5f2ccc3e0e4d15b660d5cc2f.JPG" width="666" height="500">

Inner fixation of the back bearing (13) is completed by the stator endplate (7) which also accounts for the centering and partly for the frictional connection of the stator to the axle. I used the existing threads of the stator insert (6) to bolt the endplate (7) onto it. In the stator endplate there are 4 holes for the screw connection to the stator insert and 8 holes for the cable lead-through.

<img src="/uploads/db1493/original/3X/b/8/b8fbdee6c6e4758bd653c231567b791a35dff9c6.JPG" width="666" height="500">

... and this is how the machined truck looks like.

<img src="/uploads/db1493/original/3X/7/2/72739101ff6d5f05e38dee1e5d65ac241c66fb82.jpg" width="511" height="500">

In general there are three possibilities to prevent the stator from spinning due to the "reactio" moment. Positive connection, frictional connection or using adhesive (which is indeed some sort of friction). To keep manufacturing lean and simple because I want to give it a try I decided to go with a frictional connection. I use the mounting nut to exert the necessary force, pressing the stator endplate to the flange of the cast aluminium of the axle. To get a high friction coefficient the stator endplate is made of aluminium too. The power flow is transmitted from the mounting nut via the inner ring of the front bearing to the clamping sleeve to the stator endplate. Therefore the mounting nut and the clamping sleeve are made of stainless steel.
Thanks to @ackmaniac's app and @duffman's recordings I was able to look at typical torques during hard riding. Accordingly, assuming a maximum torque of 20 Nm I'm pretty sure to be on the save side. I did a rough estimation of the maximum driving torque which can be transferred due to the friction connection in my current design. Glad it was almost an order of magnitude (!) greater than the assumed 20 Nm.

<img src="/uploads/db1493/original/3X/1/1/1148476777fa4ed7e8d311a9d09c8be780172f35.jpg" width="510" height="500">

My first ridings confirmed that the stator did not move at all on the axle in any way. After that, just to be safe I additionally use some Loctite 638 for high-strength shaft-hub connections. Putting it all together the stator is locked to the axle by two independent means, each of which offering enough potential to do the job. 

Disclaimer: I do not know what might happen to the joint when @Nowind get's the board under his crazy feet. Happy he's going only with eMTB's :grin:
 
<img src="/uploads/db1493/original/3X/a/3/a31689729333b54cfc0d6fc27fcf9ca19f7e69fb.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/7/3/73620cd8919a9cc7d14497d8e90b9c11ecc849e9.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/5/a/5ae96f26f7d5c42c24c3c380cca10945329a0ebf.JPG" width="375" height="500">
```

---
## \#28 Posted by: The_Dude Posted at: 2017-04-23T21:00:51.714Z Reads: 394

```
Addendum: An important detail for the design is that the inner axle is uninterrupted inside the Paris trucks. I was afraid that it was two pressed axle stubs which can be pulled out of the castings by the mounting nut. Therefore, I have the truck in an X-ray machine for "non-destructive material testing" - lo and behold, one uninterrupted inner axle. 

In the previous post you can see, that I provided the cooling slots with a very fine metal fabric (400um mesh width) to protect agains debris. Also made some more pictures on that and on the locking tool.

<img src="/uploads/db1493/original/3X/9/7/9702a9227afaccefe31620c08efd1294f402682e.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/6/d/6d57c0fe0b7fa7a64e1cac00a7f93616460530e7.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/0/7/079e45b7349f456c16c9a7badc58326d219dec31.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/b/a/ba7e39b7e7a048d4479d04c474f603d545396d71.JPG" width="375" height="500">

Thats all for the moment. Next posts will be about "Hall Sensors" and "VESC Mounting and Housing".
```

---
## \#29 Posted by: squad Posted at: 2017-04-23T21:53:19.683Z Reads: 380

```
Awesome work! Did You use CNC machines, or just manual ones? Personally I'm thinking about DIY hub set up from quite some time and posts like Yours motivate me to give it a try!
```

---
## \#30 Posted by: The_Dude Posted at: 2017-04-23T22:10:50.720Z Reads: 380

```
Just manual ones. At some point I was not quite sure about the tolerances, so some manual work together with intermediate testing worked out the best (btw I don't have a CNC available).
```

---
## \#31 Posted by: Eboosted Posted at: 2017-04-23T22:43:38.958Z Reads: 370

```
This a truly awesome work.

I wonder if you are planing to sell a kit to be mounted on any outrunner motor, sell the complete set with rubber covers or share all information to the community so anyone can do it themselves?
```

---
## \#32 Posted by: whitepony Posted at: 2017-04-24T04:52:06.574Z Reads: 346

```
amazing things on the forum lately, love your work and all the details! :heart_eyes:
```

---
## \#33 Posted by: The_Dude Posted at: 2017-04-24T05:00:44.811Z Reads: 346

```
Currently I just want to share all the information so that everyone has the necessary background / prerequisites to give it a try. My intention is to get feedback from the community builds and eventually improve the design. Maybe we can take it to the next level.
```

---
## \#34 Posted by: The_Dude Posted at: 2017-04-24T06:29:29.081Z Reads: 342

```
Thanks! I always follow your work with great enthusiasm. I would love to have a @whitepony -like enclose on the bottom of this build :heart_eyes: :heart_eyes:
```

---
## \#35 Posted by: Nordle Posted at: 2017-04-24T14:51:39.427Z Reads: 354

```
[quote="The_Dude, post:33, topic:21519"]
My intention is to get feedback from the community builds and eventually improve the design. Maybe we can take it to the next level.
[/quote]
This is the way to go! Really lookin good, but i hadn't good experience with exact the same glue on my first attempt. Problem wasn't slipping, but the urethane went off sideways from the can while carving. You have a flange on the inner side, maybe if you would build one on the other side too it may be better.
Esthetically best hubs i know!
```

---
## \#36 Posted by: The_Dude Posted at: 2017-04-24T15:01:46.087Z Reads: 341

```
Thanks for the compliment! You had a smooth rotor can surface or also with circular grooves like from the older APS motors?
Where are you from? I would be glad if a hard carver drops by and gives my build a try!
```

---
## \#37 Posted by: Nordle Posted at: 2017-04-24T15:57:20.717Z Reads: 347

```
Almost smooth aluminium, just some scratches from a brush (so ne eisenbürste halt:), and alu is always shit to bond on... It may hold, hope the best for you!
```

---
## \#38 Posted by: Nowind Posted at: 2017-04-25T06:55:46.427Z Reads: 353

```
Really great work on this Hubs @The_Dude
I see the countless hours of work :+1: 
Very Nice Stuff
```

---
## \#39 Posted by: The_Dude Posted at: 2017-04-25T20:03:00.299Z Reads: 372

```
## Hall Sensors
Now comes the hardest part. If you have tried the VESC with FOC you won't miss that any more. To get a good startup performance, hall sensors are mandatory. The easiest and space-saving alternative is to place the three hall sensors into the gap of the anchoring grooves at an angle of 120°.

<img src="/uploads/db1493/original/3X/1/3/135dee3d822365b3214970bede160947ff4570ba.JPG" width="375" height="500">

If you are lucky, there's enough space in between the copper windings and it looks like this after filling the gaps with epoxy resin.

<img src="/uploads/db1493/original/3X/3/1/31053b36499b5b34fd66a2ed9310f35089581d9f.JPG" width="375" height="500">

This only worked with the second (spare) one of my motors. My first motor was used for the single hub motor V1. The design was as I already said "thermally suboptimal". My son revealed that very clearly when driving at maximum throttle while pulling his friend on his skateboard ... after a while the motor got absolutely hot so that the paint on the stator wires melted and stucked together. I had a hard time to dismantle the motor:

<img src="/uploads/db1493/original/3X/a/c/acbed5d86b6733718d6f6310056d305a53c3e75f.JPG" width="666" height="500">

After unwinding the brick I had to Wye-rewind the motor :sweat: several hundred meters of wire but finally I got it made  :sweat: :sweat:

<img src="/uploads/db1493/original/3X/c/0/c00d3af2bfbdfbbccf36da05b037f387ecb5ada8.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/3/c/3c9910deafa00cce39d383148b73bd835ec9d408.JPG" width="375" height="500">

I probably choose a wire with a larger core diameter (hard to estimate exactly because of the paint), so I probably got a very good copper filling ratio. Good for the torque but definitely too less space for the hall sensors in the gap of the anchoring grooves. So I had to take a different route using my Dremel :mask:

<img src="/uploads/db1493/original/3X/5/2/523bee2954161fc76ea6a5dcd15054e82e887e0e.JPG" width="375" height="500">

Grinding has to be done carefully in order not to touch the windings. Since I had that much copper in the stator I wasn't able to grind further as shown in the picture.

<img src="/uploads/db1493/original/3X/6/d/6d5b7a148ca5440e99827976bc4d7b1e7ab5a713.jpg" width="466" height="500"><img src="/uploads/db1493/original/3X/8/c/8c151c03034e60aa533c324f3b14e073f22d6f6c.JPG" width="375" height="500">

Fixed the hall sensors with epoxy resin, but finally they still were too much in height so they scraped at the magnets of the rotor. Again I used the Dremel to flatten the after I cut one spare sensor apart to see how far I can go.

Finally :stuck_out_tongue_winking_eye:
[https://youtu.be/MUvyfU1geIY](https://youtu.be/MUvyfU1geIY)
```

---
## \#40 Posted by: Pedrodemio Posted at: 2017-04-25T21:01:20.971Z Reads: 351

```
@The_Dude nice work, how did you managed to drill the wheel? I'm in a similar path of designing a hub motor from scratch, but it's hard to find pourable urethane here, so using an available wheel would help, but in my previous experience working with urethane and keeping the dimensional tolerance was hard since it deforms easily
```

---
## \#41 Posted by: The_Dude Posted at: 2017-04-25T21:24:46.114Z Reads: 340

```
It's indeed a little bit of try and error. You have to find the right point where the chuck of the lathe clamps hard enough to turn the wheel evenly during processing and at the same time having only the minimum affordable deformation of the wheel.
Another possibility would be do turn yourself a slotted can which fits tightly on the wheel, applying even pressure. I only thought of that option but didn't use it by myself. Instead of turning with a lathe tool you can use  a hole saw if you find one with the appropriate diameter.
```

---
## \#42 Posted by: Hummie Posted at: 2017-04-25T21:47:56.794Z Reads: 328

```
I think making a mold and pouring pu is a sure thing compared to cutting up expensive wheels where it's very hard to get a good cut or it centered.
Have you tried increasing the motor amps instead of a sensor. If the motor only has access to tiny amperage at the slowest speeds/ duty cycle, especially relevant on a hub motor, it cogs a lot in my experience, but with the amps available I can go from 0 without almost any cogging or sound.
Motoramps.com was put up by Devin which shows how to chose for consistent wattage at all rpm.
```

---
## \#43 Posted by: Pedrodemio Posted at: 2017-04-26T00:17:52.909Z Reads: 323

```
@The_Dude thanks for the tips, I will see what turns out better

@Hummie I agree, the problem is that here in Brazil I didn't manage to find the urethane, my idea was to 3D print a mold and pour
```

---
## \#44 Posted by: whitepony Posted at: 2017-04-26T05:12:23.545Z Reads: 319

```
[quote="Hummie, post:42, topic:21519"]
I think making a mold and pouring pu is a sure thing
[/quote]

could you do a tutorial on that? how is the pu quality compared to kegel/flywheels?

I was thinking about making my own urethane rings for the trampa hubs but not sure if ill accept the pu quality. :thinking:
```

---
## \#45 Posted by: Hummie Posted at: 2017-04-26T05:32:45.819Z Reads: 320

```
Compared to kegel wheels the room temp pu I got from bjb enterprises grips just as good, can be just as coshy soft, but it doesn't have the rebound and won't roll as far on a "push". Hot pour stuff is harder to get and has better rebound but it's largely unnoticeable 
Making a mold I'll make a video next time maybe.  I like to use coconut oil's ability to melt and do two part silicone 50duro molds .  Prop the wheel with anything in a big enough can an inch off the bottom, half cover in liquid coconut oil, harden, pour silicone over second half, melt off the oil, flip, and then pour the second half,  with a wide pour hole and breather out of wax.   That's pretty much it. Bjb or jbj enterprises stuff is what I used. Get the long pot life.  A vacuum chamber and pump you might be able to get away with if you mix it slowly at the bottom and use a solid color.
```

---
## \#46 Posted by: The_Dude Posted at: 2017-04-26T06:40:59.584Z Reads: 304

```
Video tutorial would be great.
```

---
## \#47 Posted by: The_Dude Posted at: 2017-04-26T07:14:19.323Z Reads: 318

```
Thanks for your answer. I was also thinking about moulding on my own but I really have no clue how to do it. Any help is appreciated. My motivation is not the money I have to spend for some wheels, I was more thinking of a better and durable connection between rotor can and pu-wheel. Do you think it is possible to use the rotor can as the inner boundary of the mould? Best case there will be no urethane slipping any more. 
Btw. Another question - has anybody tried PU-Adhesive to bond the wheel to a rotor?

Hall sensors vs. motor amps. The startup stuttering I get using FOC does not depend on motor amps/torque at standstill. I even get it on the bench where there is really no load on the wheel. Sometimes you have this stuttering sometimes not (and I already tried different motors). It only depends on the rotor position when starting. The only thing what helps with the current firmware is using hall sensors when using FOC. BLDC is a completely different issue - clean startup every time even without halls.
My motor amps are "almost" unlimited (2 x 80 A) - so I had the issue that when testing my board the first time it went WOHHHHHHH, while leaving me on the asphalt :confounded: 
I know the Devin-theory, I understand and did the math but doing so I think you will get deficiencies either in the low or high ppm range. It is always a compromise and for the sake of even acceleration you cut down the abilities of the drive somewhere. What helped was defining a suitable throttle curve (thanks @ackmaniac) and also introduce more PT1 delay in the BLDC-tool advanced tab.
```

---
## \#48 Posted by: Hummie Posted at: 2017-04-26T07:42:13.109Z Reads: 323

```
O I see there's no grooves on the rotor to adhere to. Does it slip, have you got it going yet?  Maybe you could epoxy some symmetrical grooves on and then get a 3D print made of what tire will match make a mold like that. But that's problematic and time and think u should skip it and just glue it on
Using the rotor I think is more trouble then pvc then 
Maybe you missed Jacobs hub motors that slip and people are gluing them on or adding attachment ribs to the rotor.  Gluing on might be an easy solution as long as it's not too hard to get off.  You could make a mold of a simple inside diameter then and could make the tire plug/dummy with just pvc or something.  Making the mold will be easy and with the pvc dummy especially cheap.

I don't get you with the ppm efficiency.  I though simply low duty is a bit less efficient but that's it. What's the pt1 delay do ?
```

---
## \#49 Posted by: peter Posted at: 2017-04-26T08:26:56.790Z Reads: 324

```
Nice! I used tiny hall sensors to fit it between the stator slots. 

https://www.electric-skateboard.builders/t/surfs-up-loaded-dervish-sama-circles-custom-sensored-dual-hub-motor-sk3-6374-6s-lipo-xerun-150a-esc-90-mm-flywheel-clones/3233/27?u=peter
```

---
## \#50 Posted by: peter Posted at: 2017-04-26T08:37:33.424Z Reads: 323

```
A hole saw in a drill press works too.
```

---
## \#51 Posted by: The_Dude Posted at: 2017-04-26T10:01:01.199Z Reads: 317

```
Bummer - why didn't I read your thread before? Great solution with these tiny halls - would have saved me several hours and headaches. Thanks!
```

---
## \#52 Posted by: HTownBomber Posted at: 2017-04-26T13:06:03.518Z Reads: 314

```
Sweet build, dude. Incredible documentation.

As for the wheels, I have an idea that might be worth a try. Back when I was a golfer, I used to build my own clubs. They have a tried-and-true way a keep the rubber grips securely fastened to the steel shaft of the club. Essentially they use double-sided tape that adheres securely to both the shaft and the rubber, and a solvent that temporarily turns the glue into a lubricant. 

So you pour or lathe your urethane to 1-2mm smaller than the rotor can and apply the double-sided tape to the can. Heat up the urethane with a blow dryer so that it expands just enough to be pushed on. Spray that tape down with the solvent and jam that wheel on while the tape is nice and slick. The solvent will evaporate, leaving the glue which creates a very strong bond. 

This method prevents slippage against the torque forces of swinging a golf club; it may work for wheels.

https://www.amazon.com/dp/B00SRGJ53W/ref=cm_sw_r_cp_apa_uCjazbV9RXVWT
```

---
## \#53 Posted by: The_Dude Posted at: 2017-04-26T17:49:24.689Z Reads: 308

```
Until now I have no issue with slipping urethan - I even think I know why, in the post above I described this in detail.
 
Regarding pwm (sorry not ppm, parts per million) I meant not efficiency but rather deficiencies/shortcomings. Approximately you have the low pwm / high motor current range at startup and the high pwm / high battery current range at end speed. If you go for constant power you will not be able to get the full available power/performance what your system is able to provide, esp. if you have high power LiPos.
PT1 is a term from control theory. Practically this is a measure how fast the motor reacts or how fast he will adhere to the controller input. Benjamin Vedder showed this in one of his earlier videos. The corresponding parameter is "Positive ramping time constant" in the Nunchuk tab.
```

---
## \#54 Posted by: Hummie Posted at: 2017-04-26T19:01:29.778Z Reads: 307

```
I don't know what u mean by going for "constant power". What u wrote above makes sense abou motor and bat amps.  The way I have the vesc it puts out the same 900watts regardless of rpm/duty. I could increase that constant or unbalance it with more power at high speeds or low.  

The pt1... Does that change the ramping of power so while the motor/bat amps may be set to something it determines the speed it's applied after the throttle is applied?
```

---
## \#55 Posted by: The_Dude Posted at: 2017-04-26T19:37:37.471Z Reads: 334

```
Last chapter:

## VESC and Mounting and Housing

This is not really closely related to the hubs, but it think it's a good conclusion to the project. Dual hubs, so dual VESCs are needed. I decided to mount the VESCs directly onto the board, for convenience. Since the board has some reasonable flex I put them onto small rubber dampers. The assembly is shown in the next pictures - no words.

<img src="/uploads/db1493/original/3X/8/1/81758c9f8b26cf0d63cd55257edf602be802aa1c.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/9/1/911d9e644629218363d05237101ec671053f76c7.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/5/4/5415d32adaf59511012aabd48546f3058b83e79e.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/3/a/3a4b3cc740e64b3c8a0e1fdedc900151924d5863.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/5/5/55ef066f553a74978bcb37a91d8ce86e0eb0fca7.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/d/2/d2bc94d530d837fb888c33c152195c52fe062a6c.jpg" width="598" height="500">

I'm a little proud to say that I successfully soldered both VESCs on my own :relieved: The master VESC is connected to the receiver for my Nunchuk RF or Kama, the slave to a bluetooth LE module for the connection with the @Ackmaniac app. 

<img src="/uploads/db1493/original/3X/5/e/5e746d6dd10af8f75a02e107a6ea710210a37f69.jpg" width="690" height="492">

The controllers are covered by an 3D printed enclose, contour crafted to the boards shape.

<img src="/uploads/db1493/original/3X/7/7/779abd860538b94e51d90508d285b43c97eab5a5.jpg" width="689" height="325">

<img src="/uploads/db1493/original/3X/9/9/9931f3a5fa0f8b3bf95d2f9d7cc889195e71bef0.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/0/8/08b782edb45342410619d217e0cc3d3c0429c0ee.JPG" width="666" height="500">

And this is how the board looks right at this very moment. 

<img src="/uploads/db1493/original/3X/c/b/cb154a510befa01302bdbd15b0030702441af2bf.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/e/d/ed33bca413db74b5f5955f6ee086b2c150e9e94c.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/5/8/589f9ff0e9e504ff9fa73ab7dca9266fe536b737.jpg" width="690" height="393">

Currently I use some LiPos which I reshaped to smaller height, fitted with velcro and three of my puristic Dude clamps. No switches, just an XT90 anti-sparc plug and balance plug. From an aesthetic viewpoint I would love to go for the beautiful lower surface covers and housings of @whitepony. We'll see ... I already looked for some fancy vacuum pumps and epoxy resin tools :stuck_out_tongue_winking_eye:. LiIon batteries are also on my list. My spot welder is already made and ready for use - but that's another story.

<img src="/uploads/db1493/original/3X/8/8/8821dd89b27ab0e0b89511d008f39cdd470e36a7.JPG" width="666" height="500">

The link to the 2D-drawings is now added to my first post. Thanks for reading!
```

---
## \#56 Posted by: whitepony Posted at: 2017-04-26T19:40:10.710Z Reads: 317

```
that spot welder looks really familiar :smiley:
```

---
## \#57 Posted by: The_Dude Posted at: 2017-04-26T19:42:14.019Z Reads: 313

```
True, true :sunglasses:
```

---
## \#58 Posted by: The_Dude Posted at: 2017-04-26T20:06:07.962Z Reads: 315

```
[quote="Hummie, post:54, topic:21519, full:true"]
I don't know what u mean by going for "constant power". What u wrote above makes sense abou motor and bat amps.  The way I have the vesc it puts out the same 900watts regardless of rpm/duty. I could increase that constant or unbalance it with more power at high speeds or low. [/quote]
 
With constant power I mean exactly what you said, e.g. 900 watts regardless of rpm/duty. I prefer to go for the maximum (to be honest, almost) for motor, batt no matter if this reveals different watts for different rpm/duty and adjust the behaviour by max_watt and the shape of the throttle curve.
[quote="Hummie, post:54, topic:21519, full:true"]
The pt1... Does that change the ramping of power so while the motor/bat amps may be set to something it determines the speed it's applied after the throttle is applied?
[/quote]

Suppose according to your joystick deflection (watt or current mode) you are traveling in a steady state. Then, you suddenly pull the joystick further for some amount/degree. The parameter now determines how fast the VESC is aiming to reach the new state you are demanding through your input. You can experience this very easy, while putting the board on the bench and observe what happens when you quickly move the joystick, depending on the value you've set. When I remember it correctly the default is 0.9. If you set it e.g. to 5 the response of the motor to changes is more smooth.
```

---
## \#59 Posted by: Ronny_CTS Posted at: 2017-04-26T20:17:17.378Z Reads: 298

```
I was contemplating soldering my own vesc as well. Did you start from a semi assembled board? Any pointers you can give (such as where to buy a quality pcb board)?. Is it doable with a soldering iron (soldering station with adjustable temperature) or do i need a reflow station?
```

---
## \#60 Posted by: IsTalo Posted at: 2017-04-26T20:53:03.660Z Reads: 303

```
Man, upload more videos, your work is just amazing
```

---
## \#61 Posted by: The_Dude Posted at: 2017-04-26T21:26:49.461Z Reads: 313

```
I ordered the pcb's from oshpark and the parts from mouser. You need a soldering iron with temperature control with a very fine soldering tip, fine tin, flux, SMD hot air station, 

<img src="/uploads/db1493/original/3X/2/9/2958f161940c02ab43f092f40273d600fcc15962.jpg" width="500" height="500">

SMD soldering paste ... and a mircoscope or a real goog magnifying glass to control what you've done.
```

---
## \#62 Posted by: whatthejess Posted at: 2017-04-27T00:39:44.856Z Reads: 300

```
Where did you get those tiny hall sensors?! they are fantastic!
```

---
## \#63 Posted by: yaca Posted at: 2017-04-27T09:04:18.267Z Reads: 304

```
What do I have to know about hall sensors? Maybe I want to put them in jacob's hubs. I would have an old RC motor (4s) with hall sensors. Could I use them or do I need special hall sensors?
```

---
## \#64 Posted by: The_Dude Posted at: 2017-04-29T11:47:23.680Z Reads: 300

```
Forgot that one - overview of the 2D-drawings. <img src="/uploads/db1493/original/3X/7/1/71e9d7a437881aca3da82194b4be6c601777cb6f.jpg" width="653" height="500">
```

---
## \#65 Posted by: squad Posted at: 2017-04-29T11:53:16.792Z Reads: 286

```
Is there any chance You could upload those drawings in higher quality?
```

---
## \#66 Posted by: The_Dude Posted at: 2017-04-29T11:54:26.420Z Reads: 282

```
The link to my dropbox is already in the first post. Gimme a notice if you can access the drawings.
```

---
## \#67 Posted by: squad Posted at: 2017-04-29T11:57:53.114Z Reads: 284

```
Thanks! Downloaded the files, everything looks great!
```

---
## \#68 Posted by: hexakopter Posted at: 2017-05-06T19:58:02.718Z Reads: 282

```
Thank you for opening this thread. :+1: Nice to see that there are also some "real DIY" people out there. This build rocks. Do you have done some real world testings since your last update. Would be interesting to see how they perform compared to your belt drive system.

And are there any infos available about your spot welder. (I remember to saw @whitepony's similar one somewhere, but maybe there is a extra thread somewhere that I haven't seen) Thanks. Keep up that awesome work.
```

---
## \#69 Posted by: whitepony Posted at: 2017-05-06T21:00:27.289Z Reads: 282

```
mine is here: https://endless-sphere.com/forums/viewtopic.php?f=35&t=70435#p1062504

good old days :smiley:
```

---
## \#70 Posted by: hexakopter Posted at: 2017-05-06T21:38:13.366Z Reads: 280

```
Thanks. The good old phpBB. :blush:
```

---
## \#71 Posted by: The_Dude Posted at: 2017-05-06T22:37:08.114Z Reads: 281

```
Basically I build the V1 of this arduino spot welder [DIY-Arduino-Battery-Spot-Welder](http://www.instructables.com/id/DIY-Arduino-Battery-Spot-Welder/), added TVS and Schottky diodes to allow for freewheeling current and prevent avalanching the MOSFET as described here: [TVS & Schottky](https://endless-sphere.com/forums/viewtopic.php?f=14&t=81400&start=550#p1218325) .
Power Source is the capacitor I found in the description of @whitepony (see above). For the power source I used my current limited lab power supply. Using a battery charger should also be possible but with 17V pump charged in the cap I got only melted holes even for the shortest welding time. 12 V with the power supply works fine for me.
```

---
## \#72 Posted by: akira Posted at: 2017-05-08T07:44:47.004Z Reads: 256

```
Hi Dude,
Fantastic work !! Your hubs are amazing !
I have small questions about your hybrid capacitor-arduino spot welder : 
- How is the circuit to power up the cap. You just wire it to your current limited lab PSU and that's it ? You keep it wired when you trigger the soldering ?
- Which shottky diodes are you using ? I could not get my arduino welder to work when I add the shottky.
```

---
## \#73 Posted by: The_Dude Posted at: 2017-05-08T09:30:41.634Z Reads: 261

```
[quote="akira, post:72, topic:21519"]
I have small questions about your hybrid capacitor-arduino spot welder : - How is the circuit to power up the cap. You just wire it to your current limited lab PSU and that's it ? You keep it wired when you trigger the soldering ?- Which shottky diodes are you using ? I could not get my arduino welder to work when I add the shottky.
[/quote]

Yes, directly connected to the PSU with a small automotive breaking bulb in series - when it goes off I know the cap is charged and ready to fire. The PSU is wired all the time. Regarding the Schottky, I will check when I'm back home.
Checked: Schottky MBR4045PT-E3 (switching diode, 45V), TVS-Diode Uni-Directional 1N6275AG
```

---
## \#74 Posted by: akira Posted at: 2017-05-08T15:09:37.750Z Reads: 243

```
Thank you very much for your help !
```

---
## \#75 Posted by: MrCheatak Posted at: 2017-06-10T12:07:46.060Z Reads: 217

```
This is a serious motor modification, yet necessary, because most outrunners have only one bearing support.
In terms of home DIY not everyone has a lathe and a milling machine, so approximately how much would all the machining job cost? Excluding material expenses.
I guess clamping sleeve (9) won't be need with a 8 mm shaft motor.
```

---
## \#76 Posted by: The_Dude Posted at: 2017-06-10T21:14:03.070Z Reads: 203

```
Sorry, but I can't tell you the machining costs since I'm not a professional. Just made the parts in my spare time, luckily I could use the lathe of my company and had the help from a friend. 

The clampung sleeve is essential, no matter what the shaft diameter is. It is necessary to generate/transmit the friction force frim the nut to the axle, preventing the stator from spinning.
```

---
