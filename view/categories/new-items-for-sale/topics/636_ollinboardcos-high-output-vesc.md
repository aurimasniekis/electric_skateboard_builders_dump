# OllinBoardCo&rsquo;s High Output VESC

### Replies: 121 Views: 14780

## \#1 Posted by: chaka Posted at: 2015-12-03T02:22:02.325Z Reads: 553

```
In our testing we have found the VESC mosfets to run a little hot when riding at roughly 30mph. This induced a few thermal shut downs when we exceeded the default high temp setting. You can raise the default limits within the BLDC tool to keep the VESC from shutting down but I think we have found a better approach to this situation.

We have mounted the VESC to an aluminum base which doubles as a heat sink for the bottom three mosfets and added individual heat sinks to each of the top mounted fets. 

This unit is now standard in our integrated decks and has alleviated any overheating during extended high output sessions. It will soon be available in our online shop too, feel free to contact me if you would like to get in ahead of its launch and order this model now.

<img src="/uploads/db1493/original/2X/b/bcf35d3d4bb245fca7d71ae43a90756d4e5221a5.jpg" width="690" height="388">
```

---
## \#2 Posted by: Jeff Posted at: 2015-12-03T02:33:32.719Z Reads: 508

```
Hey chaka, looks great!

I experienced a shutdown on my current dual VESC setup after some "spirited" riding. 

two questions:

1. Has anyone determined what the safe maximum operating temperature is for the VESC? It looks like it is set standard at 100. Could I safetly bump that up a bit?

2. I placed an order from Ollin about a week ago for a single motor build I am working on. Could I add this on?
```

---
## \#3 Posted by: chaka Posted at: 2015-12-03T03:02:13.362Z Reads: 486

```
Hi Jeff,

You could bump the temp up a bit but it is less than optimal.  Would decrease efficiency and increase resistance.

If you would like this model I will send you an invoice for the difference, a whopping $10!!!  This unit will list for $120 with cables, capacitors and heatshrink.
<img src="/uploads/db1493/original/2X/e/ebd0a73815fe8b850dbc88b341709cef91c24b29.jpg" width="363" height="352">
```

---
## \#4 Posted by: sk8ace Posted at: 2015-12-03T04:14:01.472Z Reads: 455

```
Pretty cool that little passive heatsinks make a difference. I've got some heatsinks around here somewhere and will put them on mine when it comes in.

Good work!
```

---
## \#5 Posted by: NNGG Posted at: 2015-12-03T07:04:23.937Z Reads: 437

```
They run hot at 30mph, but will they be hot at 20 mph? Do they need ventilation at 20mph?
```

---
## \#6 Posted by: chaka Posted at: 2015-12-03T14:58:21.104Z Reads: 437

```
No, the VESC handles that type of use very well as designed. At 30 mph we use almost three times as much wattage as when we travel at 20mph.
```

---
## \#7 Posted by: onloop Posted at: 2015-12-03T21:45:19.569Z Reads: 455

```
So the heat problem you are having is to do with the higher amps you are pulling, right?

Because I think that the speed you travel is not directly proportional to heat - Watts is though. I mean technically (without atmosphere) you could travel at 80-100mph and not generate much heat if there is no load on the motors.

So I think me must look deeper, I assume what creates too much heat is the sustained load on the motors, they keep pulling more & more amps until the load reduces, this can happen at any speed if the gearing is not setup correctly. So maybe the heat problem you are having is a gearing ratio problem? Are you still running 2:1 reduction? What size wheels?

What RPM are your motors at when riding at 30mph? Might you just need some higher KV motors & more reduction? 

Or perhaps if the gearing is already optimized you are now simply experiencing a speed point which most of the load is now due to wind resistance.

This chart shows how much more power is required to battle wind resistance on an ebike - 0ver 25mph you start wasting lots of power.
<img src='/uploads/db1493/original/2X/4/4437677ed1c4f6757388c04806da568136012437.jpg'>

Here is a similar chart, it shows the relationship between actual speed & required power.
<img src='/uploads/db1493/original/2X/0/0586b19bf91f288231ce2c2937f9c80e2920a425.jpg'>



I can ride at 25-28mph and there is no heat, at least not enough to cause system shutdowns. So i assume once you past that 30mph zone the effect of wind resistance really starts to hurt perfromance.

To help mitigate your heat problems I recommend optimizing your drive train & then maybe installing a wind shield.

*Also maybe a bonnet scoop with vesc inside.*
<img src='/uploads/db1493/original/2X/d/d30013a035b9616d00eb164cec2e74c9a8ee63de.jpg'>
```

---
## \#8 Posted by: sk8ace Posted at: 2015-12-03T22:26:12.001Z Reads: 408

```
Lol that would look hilarious on the front of a deck.
```

---
## \#9 Posted by: trbt555 Posted at: 2015-12-04T11:43:02.214Z Reads: 407

```
Aerodynamic drag is proportional to the square of velocity.
Double your speed and you'll quadruple the drag.
Power needed to maintain velocity is proportional to said drag.
Current drawn is proportional to power needed.
Heat generated is proportional to current drawn.
Hence heat generated is proportional to square of velocity.
20mph squared is 400, 30 mph squared is 900 so theoretically you'll generate 2.25 times more heat at 30mph than you would at 20mph.

Just sayin heat sinks make sense if you wanna go faster.
```

---
## \#10 Posted by: longhairedboy Posted at: 2015-12-04T17:48:18.161Z Reads: 406

```
also, and i'm strictly being pragmatic here...

Adding heat sinks to the VESC just makes sense. So what if it runs fine without them under MOST conditions. Under MOST conditions, MOST things won't fail. What sets a quality product apart from MOST products is its ability to NOT fail even under conditions that rarely ever happen. 

Doing 30mph isn't a "regular occurrence" even on this forum. 95% of the time we're during 25 or under i would think because most of us aren't geared up to do those kinds of speeds all the time. 

Al of that being said, I think heat sinks should be a regular feature of the VESC. Its not like having them on there is going to make your box any bigger or make anything else any more inconvenient. All its going to do is raise the price $10 and allow the unit to perform much closer to its maximum performance level much more comfortably. After all, if it can take 30mph with a yawn, it will probably last damned near forever doing the regular cruising and carving most of us are doing on these most of the time.
```

---
## \#11 Posted by: Jeff Posted at: 2015-12-04T22:27:30.773Z Reads: 391

```
Not sure if I should post this here or in a new thread but it is along the same topic.

I was riding my dual VESC 4.10 setup from Enertion earlier today. After climbing a decent sized hill at ~25 mph, I felt the VESCs limit the power. I assume I had pushed them too hard and they went into shutdown mode so they don't damage themselves.

However, now that the board has 100% cooled off, the motors don't spin up anymore. I can connect the VESCs to the BLCD tool without issue, all the normal lights come on and the VESCs receive a signal when I pull the trigger (lights activate on VESCs).

The motors were barely hot at the time so I am almost 100% sure this is a VESC issue. Is there anything I can do to troubleshoot/fix this? Once I do get it running I will probably mount heat sinks to my VESCs to prevent the issue from happening again.

Thanks everyone!
```

---
## \#12 Posted by: kai Posted at: 2015-12-05T15:33:55.482Z Reads: 359

```
Are you using thermal double sided tape for the top heat sinks? Or are you using a thermal adhesive?
```

---
## \#13 Posted by: chaka Posted at: 2015-12-05T16:19:44.852Z Reads: 364

```
Thermal adhesive. This is just the proof of concept, now that we have measurable results we are switching to a single threaded heatsink so it will also be mechanically fastened.
```

---
## \#14 Posted by: kai Posted at: 2015-12-05T16:28:26.876Z Reads: 364

```
Very cool man. I will have to get a few of these eventually.
```

---
## \#15 Posted by: torqueboards Posted at: 2015-12-06T11:36:01.493Z Reads: 370

```
Can't wait to see the mechanically fastened option.
```

---
## \#16 Posted by: Humus Posted at: 2015-12-09T07:06:44.451Z Reads: 373

```
Hey, so I am building a eboard and am planning to use a 150kv outrunner at 10-12S. Will there be a noticeable difference using a high output vesc versus a regular esc?
```

---
## \#17 Posted by: chaka Posted at: 2015-12-09T14:48:26.676Z Reads: 372

```
The only modifications I have done to this VESC is add heat sinks. If you plan on pushing the envelope with the VESC I would suggest heat sinking but under normal use the VESC will operate fine without.
```

---
## \#18 Posted by: Skirk Posted at: 2015-12-09T21:26:35.967Z Reads: 371

```
What are the new dimensions of this VESC ? (also height)
```

---
## \#19 Posted by: chaka Posted at: 2015-12-09T22:54:32.472Z Reads: 374

```
Hey Skirk!

The dimensions are 40mm x 65mm x 23mm
```

---
## \#20 Posted by: Skirk Posted at: 2015-12-10T05:49:18.505Z Reads: 381

```
Thanks ! But, could you give me the dimensions of the unmodified VESC ? I have read that it is 1 inch, but I would like something more accurate.
```

---
## \#21 Posted by: longhairedboy Posted at: 2015-12-10T12:49:44.710Z Reads: 366

```
Thanks for posting this. I needed it too.
```

---
## \#22 Posted by: chaka Posted at: 2015-12-28T20:56:08.761Z Reads: 363

```
Here is where we are now, mechanically fastened heat sink and base plate. A little shrink tubing and this VESC will be ready to go!

<img src="/uploads/db1493/original/2X/4/4be87da4e1b0e06a083a771d8a5f4f400e8f376f.jpg" width="683" height="500">
```

---
## \#23 Posted by: sk8ace Posted at: 2015-12-28T21:01:29.606Z Reads: 347

```
Awesome! Can't wait to get mine.
```

---
## \#24 Posted by: Blasto Posted at: 2015-12-28T21:28:31.706Z Reads: 338

```
Will you offer the heatsink/mounting kit separately?
```

---
## \#25 Posted by: trbt555 Posted at: 2015-12-28T21:32:52.754Z Reads: 338

```
That looks good !
looking forward to mine too.
```

---
## \#26 Posted by: NNGG Posted at: 2015-12-28T22:43:19.241Z Reads: 330

```
Any ideas about the release date?
```

---
## \#27 Posted by: chaka Posted at: 2015-12-28T23:38:44.336Z Reads: 326

```
We are good to go now, we will likely keep it off menu for awhile. Send me a message and I will be happy to go over the extra cost of the heatsink package. 

Unfortunately there are a few constraints that make it unavailable in kit form.
```

---
## \#28 Posted by: Blasto Posted at: 2015-12-29T10:26:03.036Z Reads: 330

```
[quote="chaka, post:27, topic:636"]
Unfortunately there are a few constraints that make it unavailable in kit form.
[/quote]

i'm guessing the thermal adhesive on the fets and or the thermal gap pad? Looking at the picture, you isolated the motor phase wires (obviously yes)?

I still would be interested in the top and bottom plates :)
```

---
## \#29 Posted by: chaka Posted at: 2015-12-29T15:59:45.931Z Reads: 338

```
Yes you would need to get some thermal adhesive/plaster and possibly resolder you battery connections. The wires need to be routed around a few components to achieve a low profile. 

Honestly this is only necessary if you push the VESC hard on a single motor setup. Of course it looks cool and that is as good of a reason as any. :smile:
```

---
## \#30 Posted by: Blasto Posted at: 2015-12-29T16:56:13.162Z Reads: 338

```
I push the vesc pretty hard. Here's a video of them smoking. But still functional.

https://youtu.be/g2f_fZxJli0

I had a heatsink on them, but i like how you emplemented the heatsink, can also be used as a proper mount with tapped holes.
```

---
## \#31 Posted by: chaka Posted at: 2015-12-29T22:50:24.481Z Reads: 325

```
@Blasto I am curious as to what was smoking? Do you know which component you cooked on that run?

Send me a pm and we can exchange some information. I also build VESC's with the 5mOhm shunts for high current use although it looks like you guys have the chops to do that yourselves. 

That's a frisky little bot, I wouldn’t want it chasing me down.
```

---
## \#32 Posted by: Blasto Posted at: 2015-12-29T23:30:20.586Z Reads: 319

```
My best guess is excess flux... Everything was working fine after. 

Btw, these bots weigh about 200-300kg when on the arena.

I'll send a pm when i have time to sit down
```

---
## \#33 Posted by: trytagger Posted at: 2016-01-11T14:58:32.310Z Reads: 313

```
I would like to have 1. What is the ETA for this?
```

---
## \#34 Posted by: chaka Posted at: 2016-01-11T15:11:42.183Z Reads: 311

```
December was a big month for us and bumped us out to three weeks. We have two more team members now so we will probably be able to bring it down to one week very soon.
```

---
## \#35 Posted by: trytagger Posted at: 2016-01-13T00:04:09.480Z Reads: 309

```
How could i order 1?
```

---
## \#36 Posted by: psychotiller Posted at: 2016-01-13T00:33:44.442Z Reads: 316

```
http://www.ollinboardcompany.com/product/vedder-s-speed-controller
```

---
## \#37 Posted by: chaka Posted at: 2016-01-13T01:09:10.080Z Reads: 316

```
Leave a message during checkout and I will send an invoice for the added charges. The heat sink package is an additional $15.
```

---
## \#38 Posted by: mcoyle Posted at: 2016-01-25T21:49:32.911Z Reads: 325

```
Hey,
I'm waiting on the 4.10 release of the VESC, I'm just curious what changes and updates I should expect. I'll be running a dual motor rear drive set, each will be hooked up to the new VESC. Since I'm waiting till the middle of february, I'm just curious what differences make it worth the wait compared to getting an older model.
Thanks! I'm excited.
```

---
## \#39 Posted by: chaka Posted at: 2016-01-25T22:00:15.839Z Reads: 321

```
I don't think anyone is currently producing anything older than version 4.10
```

---
## \#40 Posted by: mcoyle Posted at: 2016-01-25T22:04:57.543Z Reads: 324

```
Oh i wasn't aware, new to the field. Thanks! the site I was looking at must've been out-dated.
```

---
## \#41 Posted by: chaka Posted at: 2016-01-25T22:36:02.006Z Reads: 311

```
You can find my listing here: [http://www.ollinboardcompany.com/product/vedder-s-speed-controller][1]


  [1]: http://www.ollinboardcompany.com/product/vedder-s-speed-controller
```

---
## \#42 Posted by: Jeff Posted at: 2016-01-25T23:29:51.655Z Reads: 323

```
Hey @chaka, I got the high output VESC hooked up finally. It looks great and I love how solid it makes the VESC feel!

I had a chance to go 5 miles today and so far so good. Do you have any insights as to how far we can push one of these? Should I implement a cooling system in my enclosure?

<img src="/uploads/db1493/original/2X/2/2d6512a8189fd098c0c73728454269b0b8d9f893.jpg" width="690" height="388"><img src="/uploads/db1493/original/2X/7/7adf3910e53bb10d74bf68e097d5d3d3b8ff79a6.jpg" width="281" height="500">
```

---
## \#43 Posted by: chaka Posted at: 2016-01-26T01:02:38.758Z Reads: 306

```
It does feel pretty stout with the base and heatsink. You should be good to 30 mph on a single Maybe more. Pay attention to the auto back off feature while hill climbing. If you feel a little power loss back off a little. Keep me posted on the performance!
```

---
## \#44 Posted by: Jeff Posted at: 2016-01-26T01:46:34.789Z Reads: 313

```
I will definitely keep you updated.

In the spirit of unlocking the maximum potential, will you take a look at my settings?

Most of the items are determined from motor limit (80A) and battery limits (10C 12S 5200 mah LiPo). Is there a reason duty cycle is defaulted to 0.95? Isn't that just removing the last 5% of throttle? Can I switch it to 1?

<img src="/uploads/db1493/original/2X/a/a6b96bc0803615e0a88d3ef4e7c3388fa11dcb4a.png" width="690" height="317">
```

---
## \#45 Posted by: chaka Posted at: 2016-01-26T01:52:15.683Z Reads: 305

```
You probably want to keep things where they are at. The defualt settings are pretty good for most people. If you start adjusting parameters too far from where they are at you could end up with drv8302 failure.
```

---
## \#46 Posted by: Sonic1 Posted at: 2016-01-26T18:23:48.290Z Reads: 308

```
Do they have some sort of magnetic force that is supposed to be giving them extra gravity pull?
```

---
## \#47 Posted by: Blasto Posted at: 2016-01-26T19:17:24.285Z Reads: 310

```
<img src="/uploads/db1493/original/2X/0/0931e51d8ad677b0d45f94af3f560f2fedda60ed.jpeg" width="690" height="458">

Yes 34 3/4" N42 cupped magnets

http://www.kjmagnetics.com/proddetail.asp?prod=MMS-D-C

The white pucks are teflon, our frame was deforming without them
```

---
## \#48 Posted by: Jeff Posted at: 2016-02-02T01:36:47.763Z Reads: 305

```
Hey @chaka, finally got to put the high output VESC through its paces today. I basically went as fast as I could on my way home today with lots of hard accelerations.

The same hill that apparently killed my dual enertion vescs was handled easily by your single vesc!

I am running it in a sealed container and the temp after riding was only 37C. Awesome!

<img src="/uploads/db1493/original/2X/8/8ca1753c1d255ffc5470857bd0b8824d7c45ba79.png" width="281" height="500">

 <img src="/uploads/db1493/original/2X/c/c05c65fdc613290b23017dbaafb8436d7cf8e558.png" width="281" height="500">
```

---
## \#49 Posted by: torqueboards Posted at: 2016-02-02T01:49:45.370Z Reads: 284

```
Awesome.. Was the issue the heat?
```

---
## \#50 Posted by: Jeff Posted at: 2016-02-02T02:04:24.898Z Reads: 291

```
Hard to tell. The details of the problem are here: http://www.electric-skateboard.builders/t/vesc-not-powering-motors-after-heavy-riding/703.

One was a DRV fault and the other was an over temp fet. I was also surprised Enertion would ship their VESCs with such poor wiring as well. I don't like bad mouthing other companies but I was really left disappointed by my Enertion VESCs.

Since Enertion wouldn't do anything to right the problem, I sent the broken VESCs to ollin board company for repair, proper high strand silicone wiring, and the high output treatment.
```

---
## \#51 Posted by: NNGG Posted at: 2016-02-02T04:47:34.295Z Reads: 281

```
what motor do you have connected to that vesc?
```

---
## \#52 Posted by: Jeff Posted at: 2016-02-02T04:56:44.497Z Reads: 280

```
Right now I have a 170kv 6374 outrunner, 3kw.
```

---
## \#53 Posted by: chaka Posted at: 2016-02-02T15:42:02.534Z Reads: 282

```
Awesome! I love those beefy sk3 motors. They don't get enough credit for their quality. Only motor I have seen eboarders use with a large support bearing for the inner can wall too.

I have repaired a number of those green VESC's but I am starting to think there may be other problems since they continue to blow drv chips on the regular. I am hoping it is just user error. 

In any case if the VESC's I repair for you end up being lemons I will credit the repair cost towards a new set and switch over the good components to the high end pcb's from OshPark. Waste not, want not!
```

---
## \#54 Posted by: NNGG Posted at: 2016-02-03T02:00:29.648Z Reads: 275

```
What voltage do you have on it?
```

---
## \#55 Posted by: Jeff Posted at: 2016-02-03T02:20:57.479Z Reads: 277

```
I am running 12S currently.
```

---
## \#56 Posted by: NNGG Posted at: 2016-02-03T03:47:38.461Z Reads: 271

```
Cool, how does it handle hills?
```

---
## \#57 Posted by: onloop Posted at: 2016-02-03T03:54:43.955Z Reads: 301

```
[quote="chaka, post:53, topic:636"]
I am hoping it is just user error.
[/quote]

Yeah, you are probably correct.

I have just built over 30 Dual Raptors with a full range of motor testing carried out over many days, that's 60+ VESC's, they all have the same PCB. - There were 360 units from that particular batch with that same PCB, all have been shipped out to customers.

.... So far there have probably been around 8-10 known reports of failure on that PCB due to various reason. I acknowledge some had really bad wiring that got missed during the QC This may have been a contributing factor, Out of these reports some of the faults have turned out to be directly contributed to user error. 

This equates to around 2-3% failure rate. So very unlikely there is something wrong with the PCB itself. Vedder himself openly admits to having DRV issues with units he has built himself. The DRV chip actually can fail for many reasons and at this stage of VESC development not all faults are well understood. 

Also it's worth considering the varied environments that these micro electronic devices are being used in. What precautions are being taken by the end user to prevent ESD which can damage many of the components on the VESC. Simply handling the VESC could be risking failure.
```

---
## \#58 Posted by: chaka Posted at: 2016-02-15T20:27:34.430Z Reads: 300

```


We made a listing for an add-on package for the VESC on our site. It should make ordering the heat sinked VESC a little easier: [http://www.ollinboardcompany.com/product/vedder-s-speed-controller-heat-sink-package][1].

 It is not the most ideal way of implementing heat sinks on a motor controller but it has been proven to extend the output range of the VESC considerably. It definitely provides better passive cooling and thermal mass so we are making it more widely available.
<img src="/uploads/db1493/original/2X/4/4be87da4e1b0e06a083a771d8a5f4f400e8f376f.jpg" width="683" height="500">


  [1]: http://www.ollinboardcompany.com/product/vedder-s-speed-controller-heat-sink-package
```

---
## \#59 Posted by: hexakopter Posted at: 2016-02-15T20:53:16.917Z Reads: 291

```
Do you have done a side by side comparison? I am very interested in also cooling my VESC FETS, but I don't know how good it is to put a heatsink on top of the FET plastic housing. Would be great to see the temperatur of a VESC with against one without a heatsink in normal drive conditions.
```

---
## \#61 Posted by: chaka Posted at: 2016-02-16T15:07:07.338Z Reads: 294

```
I have done trials with it, yes. As you approach the thermal cutoff setting on the VESC it will start to loose power as the VESC employs the current back off strategy. Heatsinking the top and bottom fets has show significant benefits by staving off these temperature spikes during heavy acceleration or hill climbing. 

Personal trials were done on the same board with the same VESC on the same hill. Prior to heatsinking the VESC would engage the thermal backoff strategy about halfway up, with heatsinks I had full power all the way up.
```

---
## \#62 Posted by: Jeff Posted at: 2016-03-02T01:41:28.244Z Reads: 277

```
Have you done any experimentation with completely waterproofing one of these?

I can see an original VESC overheating if it was encapsulated in something (say silicone or PU) but for the high-output design would it be possible to encase everything except for the ports and heatsinks and still not overheat it?

I know it would be impossible to service if something went wrong but I imagine a relatively indestructible VESC at that point.
```

---
## \#63 Posted by: chaka Posted at: 2016-04-15T04:00:01.029Z Reads: 263

```
I would say fully encapsulating the VESC will have to wait for v5.0 with the direct fets but I could be wrong. We could probably get away with fully encapsulating 4.12 if we limited the load with a proper reduction otherwise I think heat would just build up and you would have to let it sit while it cooled.
```

---
## \#64 Posted by: Jeff Posted at: 2016-04-15T04:15:42.866Z Reads: 262

```
Maybe a thermally conductive potting material? http://www.epoxies.com/products/thermally-conductive/

I would have to do some heat transfer calculations to see the effect it might have. I would be optimistic though since my high-output vescs are in sealed enclosures with minimal convection cooling and they run like champs.
```

---
## \#65 Posted by: trbt555 Posted at: 2016-04-30T16:21:47.806Z Reads: 252

```
Does anyone else have Ollinboard's heat-sinked vesc running in a closed box ?

I do and I'm having problems with the vesc limiting power after roughly 10 minutes of riding. Stop, wait for 5 minutes and back to normal.
Outside temp isn't even that high, like 14 deg C or so.

It's weird because I've done quite some heavy riding before and haven't had the vesc drop the power. Only lately.

I upped the temp limits in the vesc to 120/140 to see what gives.
```

---
## \#66 Posted by: laurnts Posted at: 2016-04-30T16:27:43.665Z Reads: 240

```
I am running in the same box as yours, even alot thighter with more components. I have experience that esc can be hotter if motors and batteries are not compatible. My car esc almost cooked when running my hub motor. Also thr motor gets extreme heat with rc car esc.
```

---
## \#67 Posted by: Hummie Posted at: 2016-04-30T16:35:21.733Z Reads: 251

```
I can't even get my vescs hot no matter what I do. The fets get warm at most 

I plan to pot some this week and had heard that as long as the fets aren't potted its ok. But now I'm second guessing with Chaka's words.  I think you might be talking about fully potting though.  I plan to use some 90 duro polyurethane that isn't special or thermally conductive.  Same as wheel rubber 

How fragile are the fets?  I wanted to pot the vescs and have the fets exposed under the board.  Should I make some protective cover for them?

When will u have more vescs Chaka?
```

---
## \#68 Posted by: trbt555 Posted at: 2016-04-30T16:43:04.655Z Reads: 247

```
I guess my problem may be related to one particular vesc.
One that failed earlier and was repaired.

Got some warmer days coming next week, I'll swap it out for an other one and see what happens.
```

---
## \#69 Posted by: chaka Posted at: 2016-04-30T21:08:22.822Z Reads: 247

```
Let me know if it continues to act up, did you reduce your motor max recently?
```

---
## \#70 Posted by: Hummie Posted at: 2016-04-30T23:40:42.473Z Reads: 251

```
When will U have more vescs and how fragile are the fets
```

---
## \#71 Posted by: eskateking Posted at: 2016-05-01T00:49:46.547Z Reads: 270

```
@chaka will you please look at my settings. I have your vesc.  

<img src="/uploads/db1493/original/2X/d/dc29887997a65a34f28a8122870898ac39f790f5.JPG" width="690" height="184">
<img src="/uploads/db1493/original/2X/b/b446f315a0dfb6b50e8ecb318603ce2a57594c25.JPG" width="690" height="372">
<img src="/uploads/db1493/original/2X/e/e7ce32eab4faf6bed4416a1d477bf5048ef971f6.JPG" width="690" height="375">
<img src="/uploads/db1493/original/2X/8/832bb30daf101c23493b3c20659e9b04726b005e.JPG" width="690" height="337">

I have my enertion receiver connected to vesc via servo cable but It won't work. I'm not sure if I did something wrong.
Here is my build thread: http://www.electric-skateboard.builders/t/i-need-some-help-connecting-my-motor-to-my-vesc-and-my-vesc-to-my-receiver/2642/26
```

---
## \#72 Posted by: chaka Posted at: 2016-05-01T01:35:04.202Z Reads: 249

```
Hey @eskateking glad to see your connector issue was resolved. Don't feel bad your are not the first to make that mistake.

Looks like you still need to apply your detection results and write them to file. 

In app configuration you need to select PPM write to file and configure it on the PPM tab.  Take your time and do some research, it is really easy to burn up perfectly good hardware if you are not too experienced.
```

---
## \#73 Posted by: jacobbloy Posted at: 2016-05-01T01:41:06.126Z Reads: 248

```
You can still use ppm uart,  but yes make sure in the ppm tab you have actually sellected current with brake no reverse, 
Basically by default the ppm tab current isnt activated
```

---
## \#74 Posted by: eskateking Posted at: 2016-05-01T02:49:46.573Z Reads: 241

```
I don't quite understand.
```

---
## \#75 Posted by: chaka Posted at: 2016-05-01T03:23:50.098Z Reads: 244

```
Everything you need to know is on this page: http://vedder.se/2015/01/vesc-open-source-esc/

A few very helpful videos too!
```

---
## \#76 Posted by: jacobbloy Posted at: 2016-05-01T04:14:54.806Z Reads: 246

```
I think he fixed it, he didn't do a reset after setting the application. 

Iv been in this rut before I swear I pressed reset but guess what I didn't!
```

---
## \#77 Posted by: trbt555 Posted at: 2016-05-01T07:45:09.503Z Reads: 247

```
I upped the temp limits to 120/140 and did some pretty hard riding without problems. It's still too soon to say but I'm guessing the temperature sensing on this particular vesc is off somehow.
```

---
## \#78 Posted by: eskateking Posted at: 2016-05-02T18:16:00.566Z Reads: 239

```
I watched some videos. Still quite confused. If possible, I would like to have a phone call with you.
```

---
## \#79 Posted by: eskateking Posted at: 2016-05-02T18:17:46.163Z Reads: 240

```
I'm pretty sure I pressed reboot since I've tried so many times I must have done it at least once.
```

---
## \#80 Posted by: eskateking Posted at: 2016-05-04T19:39:27.723Z Reads: 235

```
@chaka is this possible
```

---
## \#81 Posted by: chaka Posted at: 2016-05-04T19:52:28.197Z Reads: 244

```
Hey Caleb,

I might be able to give you a few minutes today but, I am going to be really honest , I think you bit off a little more than you can chew with your project. Please don't take this as harsh, I am happy to help but I dislike having to spoon feed people info when it is so freely available.

PM your phone number to me and I will give you a call a little later when I have some VESC's in the reflow oven.
```

---
## \#82 Posted by: DougM Posted at: 2016-05-04T20:57:31.902Z Reads: 250

```
Looks familiar :-)
<img src="/uploads/db1493/original/2X/1/1aa7290acecd86f5af458fe415935cd6e20cda26.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/6/6302420542d343139ce96f04b18de0259e171c40.jpg" width="690" height="388">

DougM
```

---
## \#83 Posted by: onloop Posted at: 2016-05-04T22:25:31.798Z Reads: 247

```
[quote="chaka, post:81, topic:636"]
I am happy to help but I dislike having to spoon feed people info when it is so freely available.
[/quote]

very few people will understand this as much as I do.....
```

---
## \#84 Posted by: chaka Posted at: 2016-05-04T22:31:10.146Z Reads: 244

```
Looks like it's almost finished. Nice job @DougM I'l have some revised gerberfiles going soon with mosfets on one side, we'll see how they do on testing but it is still a long way out.
```

---
## \#85 Posted by: laurnts Posted at: 2016-05-04T22:57:13.015Z Reads: 242

```
Means they didnt search or read before asking questions. So please people if you read this do your research first, if you cant find the answer then ask.
```

---
## \#86 Posted by: willpark16 Posted at: 2016-05-04T23:07:13.307Z Reads: 235

```
I honestly am starting to not come on here as much just because nooks have been repeatedly asking the same stupid questions
```

---
## \#87 Posted by: Ulfberht Posted at: 2016-05-05T01:20:09.077Z Reads: 237

```
It's kind of annoying when people don't even try to learn before they ask. It's really all available and that is a fantastic thing!! I regularly feel stoked and grateful that ES and ESK8 are here!! I can get pretty much any knowledge that I need. Sometimes I gotta dig a little more than I would like, but it's worth it in the end because you come away with not just a superficial knowledge, but a deeper understanding of what makes it all tick.  I am grateful for the help that people have given to me, but I really try actively to not "drag down" the people that are actively serving our community here. Be mindful of their lives and families y'all!! Much love!! 
@onloop @chaka Thanks for all that you do! I can't imagine how tired you guys must be of wiping bottoms! :stuck_out_tongue_winking_eye:
```

---
## \#88 Posted by: evoheyax Posted at: 2016-05-05T02:58:41.834Z Reads: 234

```
I second that one. Thank you you @chaka and @onloop for all your work here. Especially @onloop, you really took on the challenge of educating the masses, and while I see places for improvement in the structure, you've stood there and kept helping n00b after n00b. So thank you for that.
```

---
## \#89 Posted by: DougM Posted at: 2016-05-05T04:02:54.812Z Reads: 232

```
Thanks @Chaka - I still have some reliability problems, but I think I have finally found the root cause.  I need to do some road testing before I declare success, though.  

In any event I'll look forward to your new design :-)  

DougM
```

---
## \#91 Posted by: chaka Posted at: 2016-05-05T18:04:55.697Z Reads: 229

```
You should post that on the appropriate thread @eskateking

I think I have been more than gracious with you but at some point I need to tell you practice a little courtesy and show some forum etiquette. 

Stop hijacking this thread!
```

---
## \#93 Posted by: 3sly Posted at: 2016-05-06T13:02:26.445Z Reads: 223

```
Hey @chaka. I've got a VESC incoming from esk8.de (can't order from outside of EU due to import taxes).
I've gone through this thread and your site and couldn't directly find it, but: Would you mind sharing the type of heatsink/ or the dimensions. I understand if you'd rather not ;).
Going through mouser, conrad and farnell is a pain :stuck_out_tongue:
```

---
## \#94 Posted by: chaka Posted at: 2016-05-06T13:23:56.052Z Reads: 212

```
40mm heat sinks are ubiquitous. They need to be cut down to size to fit the VESC. We have plans to machine a matching heat sink to cover the entire VESC, making contact with the mosfet tabs, drv and stm32 chip but we need to finish a few other projects before we tool up for production milling.
```

---
## \#95 Posted by: 3sly Posted at: 2016-05-06T13:58:54.660Z Reads: 213

```
Great to hear, an entire cover sound great, next step a low profile/thickness enclosure around the rest of the VESC?
So they're cut down to size, that's probably why I couldn't find them, thanks!
```

---
## \#96 Posted by: Trademarc Posted at: 2016-05-09T19:41:26.269Z Reads: 211

```
Hey @chaka Just curious what the time frame would look like if I ordered a VESC from your site. I apologize if it's already on the forum somewhere else. I'm new and still trying to figure things out. I have most of the other parts, just trying to get a VESC to finish it up :)
```

---
## \#97 Posted by: Hawkmoon269 Posted at: 2016-05-10T05:26:02.985Z Reads: 214

```
I ordered mine Sunday 2 weeks ago and got a shipping label on the next Monday. Post office didn't ship the package for some reason but he sorted it out and I recieved it today. Definitely worth it and great quality. You're probably looking at around 1-2 weeks minimum depending on how busy they are.
```

---
## \#98 Posted by: Trademarc Posted at: 2016-05-10T06:21:44.464Z Reads: 217

```
Hey, thanks so much for the info. Really appreciate it :)
```

---
## \#99 Posted by: willpark16 Posted at: 2016-05-10T06:23:09.279Z Reads: 223

```
where can i get another capactor for @chaka vesc?
```

---
## \#100 Posted by: chaka Posted at: 2016-05-10T12:21:17.052Z Reads: 221

```
Do you have a bad cap @willpark16 ?
```

---
## \#101 Posted by: willpark16 Posted at: 2016-05-10T14:55:30.309Z Reads: 219

```
yea so i soldered it off
```

---
## \#102 Posted by: chaka Posted at: 2016-05-10T15:13:49.605Z Reads: 224

```
If you purchased the VESC from us we can send you a fresh cap. You can also check mouser : http://www.mouser.com/Nichicon/Passive-Components/Capacitors/Aluminum-Electrolytic-Capacitors/Aluminum-Electrolytic-Capacitors-Leaded/_/N-75hqwZscv7?P=1z0zlbmZ1yx4avu&FS=True

Get something with 5mm lead spacing to fit vedder's cap board.

I have another cap board coming out to hold 2 larger caps totaling 6600uf in the next day or two.
```

---
## \#103 Posted by: willpark16 Posted at: 2016-05-10T15:19:59.495Z Reads: 220

```
yes this was purcased from ollinboards
```

---
## \#104 Posted by: willpark16 Posted at: 2016-05-10T15:21:02.147Z Reads: 219

```
can i us any 63v 680uf capacitor with 5mm spacing. if so do i have to change out all of the capactitors
```

---
## \#105 Posted by: chaka Posted at: 2016-05-10T15:22:30.119Z Reads: 230

```
Yeah you can use any and just replace the bad cap. PM your info and I will send one out today.
```

---
## \#106 Posted by: willpark16 Posted at: 2016-05-10T15:23:06.102Z Reads: 228

```
alright and thanks man
```

---
## \#107 Posted by: LukeM Posted at: 2016-05-19T06:03:22.766Z Reads: 233

```
@chaka Probably tired of hearing this but I placed an order 2 weeks ago and haven't gotten shipping info yet. 

Order #UOYS-954076 

Thanks
```

---
## \#108 Posted by: chaka Posted at: 2016-05-19T06:14:40.842Z Reads: 236

```
Hey Luke, I posted this in another thread today. We should have everyone who has been waiting out by Friday.  Checked your order number and you are 3rd in line as of this evening!
```

---
## \#109 Posted by: Vito Posted at: 2016-05-19T18:02:55.176Z Reads: 235

```
I got my vesc today!!! Thanks @chaka so perfect!! I set my vesc with 12v lead acid battery. No im running on bldc tool mode no problem. But i wanna try FOC mode. Should i configure FOC ( read the parameters) with the 12v lead acid battery or with my 12s3p pack from torqueboards?
```

---
## \#110 Posted by: chaka Posted at: 2016-05-19T18:07:37.593Z Reads: 239

```
I would say no. FOC has been damaging the drv chips on some customers VESC's. If the calculations are not perfect it can cause some bad spikes in current.

But if you have money to burn and want to be on the bleeding edge you can give it a shot but know that it can burn up the drv and kill your stoke.
```

---
## \#111 Posted by: Vito Posted at: 2016-05-19T18:19:31.505Z Reads: 233

```
I don't wanna take that risk. So i will keep running on BLDC mode and be happy with it!!!
```

---
## \#112 Posted by: Bender Posted at: 2016-05-19T20:56:54.383Z Reads: 233

```
Could you elaborate on this. I've been running FOC almost exclusively and have been thrilled, but I certainly don't want to damage my VESC.
```

---
## \#113 Posted by: chaka Posted at: 2016-05-19T21:00:54.443Z Reads: 240

```
Don't switch back to bldc then. That is usually when the trouble starts. So far emax and maytech motors are the most finicky. What motor are you running.
```

---
## \#114 Posted by: elkick Posted at: 2016-05-19T21:05:38.663Z Reads: 235

```
Definitely true! The most failures I have seen were with 12s and those motors mentioned by Chaka. And some Alien/Saite motors too. You need to know what you're doing if going with FOC.
```

---
## \#115 Posted by: Bender Posted at: 2016-05-19T21:24:31.126Z Reads: 236

```
TB 6355 listed as 230k but we determined is probably 190k
I've been running 6s, 9s, and 12s to see which I like best
Single drive
```

---
## \#116 Posted by: flatsp0t Posted at: 2016-05-19T21:42:43.953Z Reads: 240

```
What about really low kv hubs (Hummie / Jacob)?
```

---
## \#117 Posted by: Vito Posted at: 2016-05-19T21:48:15.062Z Reads: 242

```
How do you guys set cut off start/ cut off end on 18650 packs? Same as lipo? 3.4 start/ 3.2 end?
```

---
## \#118 Posted by: boards Posted at: 2016-05-27T04:18:59.425Z Reads: 231

```
Are you caught up now?
```

---
## \#119 Posted by: evoheyax Posted at: 2016-06-02T06:48:45.084Z Reads: 221

```
I'm running and hummie is running FOC with hummies motors. Works great. You hear nothing, great torque.

What do you think about the carvons and FOC? I was thinking of buying another pair for my carvons, since I have my vescs setup for hummies motors.
```

---
## \#120 Posted by: flatsp0t Posted at: 2016-06-02T06:51:24.282Z Reads: 227

```
As they also have below 150kv, there should be at least no problem with too high ERPM.
```

---
## \#121 Posted by: evoheyax Posted at: 2016-06-02T06:57:11.631Z Reads: 234

```
so 149 kv (carvon) should be fine in FOC then?
```

---
## \#122 Posted by: flatsp0t Posted at: 2016-06-02T07:10:31.132Z Reads: 240

```
Yes, if i remember correctly, 150kv up to 12s, 190 up to 10s

Edit:
these values are to stay far away from the zone where it gets dangerous for your vesc or for cheaper vescs than the ollin ones
```

---
## \#123 Posted by: flatsp0t Posted at: 2016-06-02T07:13:41.567Z Reads: 243

```
Details are somewhere buried around there:
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125/35?u=flatsp0t
```

---
## \#124 Posted by: mason Posted at: 2016-07-02T22:17:27.588Z Reads: 215

```
Is this with the bottom + top heatsink?
```

---
