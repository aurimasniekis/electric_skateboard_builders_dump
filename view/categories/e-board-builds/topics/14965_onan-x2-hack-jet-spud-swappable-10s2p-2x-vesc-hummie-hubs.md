# Onan X2 Hack &#124; Jet Spud &#124; Swappable 10s2P&#124; 2x VESC &#124; Hummie Hubs

### Replies: 54 Views: 8525

## \#1 Posted by: faust Posted at: 2016-12-20T08:39:54.649Z Reads: 654

```
So, the Mellow Board looks really great except that (1) it's not out yet, and (2) I can't customize it (e.g., put it on 125mm trucks, for example). So I'm going the DIY route. 

The idea is the following:
1. Get an Onan X2
2. Get some good hubs (I have Hummie Steel Hubs)
3. 2 VESCs and a Switch (from DIYElectricSkateboards)
4. ???
5. Profit! 

So here's the basic setup. Just flip the X2 over and remove a bunch of screws to get to the electronics. Don't even mess about with the hubs. 
<img src="/uploads/db1493/original/3X/f/1/f150fb09d14f841c040c706f1e7ea81cee4f742d.jpg" width="281" height="500">

Detach the motor bullet connectors and the sensor wires and slide them through the small opening in the chassis. 
<img src="/uploads/db1493/original/3X/a/0/a0390ad8f2f891e121ff9b7de5e10cef37ca9928.jpg" width="690" height="388">

Now that you've got the wires out, you can remove the trucks+hubs assembly. 
<img src="/uploads/db1493/original/3X/7/4/74808f5c9515fdd99240ebeb8e36d3790f629c44.jpg" width="281" height="500">

This is the hard part. The board is in there pretty good. I actually gave up on the plastic wedges in favor of a mini crobar. Fortunately, it looks like I didn't damage anything. 
<img src="/uploads/db1493/original/3X/0/3/03f1ad22cce77fe9014bc44faaad58ba48c942a5.jpg" width="690" height="388">

The switch it came with was wired into the mainboard. It was also really annoying since you had to hold it down. I swapped that out. 
<img src="/uploads/db1493/original/3X/f/3/f3a8856567f23a6cab89e78a0807b399d4c88438.jpg" width="281" height="500">

Slide the wires through *before* you put the bullet connectors on. 
<img src="/uploads/db1493/original/3X/f/3/f3799b55b02e4f3578f2aa4fd754fbb4c2398454.jpg" width="281" height="500">

Screw it all in...
<img src="/uploads/db1493/original/3X/e/d/ed7c998ef241dab6dd6261efbd9bcf180b5787cf.jpg" width="690" height="388">

..., and attach it to your board!
<img src="/uploads/db1493/original/3X/a/1/a10a05617e546ac8b2845909c069b8398afc5add.jpg" width="281" height="500">

Now to somehow figure out how to get two VESCs in there...

Here's the video. I think I fried my first VESC with a short, so I've only got one drive wheel right now. Waiting on a new VESC replacement with much anticipation!
```

---
## \#2 Posted by: Evan Posted at: 2016-12-20T10:52:25.081Z Reads: 566

```
Amazing! Nice work mate!
```

---
## \#3 Posted by: ArmandR Posted at: 2016-12-20T12:45:22.977Z Reads: 549

```
What battery is that? 6s?
```

---
## \#4 Posted by: faust Posted at: 2016-12-20T16:13:04.091Z Reads: 531

```
It's 10s2p
```

---
## \#5 Posted by: ArmandR Posted at: 2016-12-20T17:01:18.255Z Reads: 525

```
No way, that's gonna end up so awesome!
```

---
## \#6 Posted by: Hummie Posted at: 2016-12-20T19:24:55.947Z Reads: 498

```
maybe stick some lipos in as 10s2p will very likely not be enough power and you have little room.  if you got 12s and 4mah or even 3mah and a high c rating things will really perform.

the video doesn't work.  
how'd you short your esc?
```

---
## \#7 Posted by: faust Posted at: 2016-12-20T21:24:35.202Z Reads: 476

```
Oh whoops. I forgot to hit "publish" on the video. It's up and running now. 

The specs on the batteries are 4400mah, 159Wh. I'm only guessing as to the discharge rate (30A, maybe?), as I don't know the precise cells, but I did pay extra for Samsung. The cells are strong enough to support the X2 (which actually has a good amount of power, it's just the urethane is way too thin), but you can tell from the wiring that they don't expect too much current flowing to the motors. I suppose I'll give it a go when I get my replacement VESC. If it doesn't work, I suppose I need to rebuild my 3 battery packs...

I'm actually not sure if I shorted the VESC or not. I saw the LEDs, connected the motors, then nothing. Not able to do R measurement on the motors, and the LEDs went off. When I looked, I noticed about half a mm of bare metal on my bullet connectors to the motors, so I assumed that caused it. Lessons learned.
```

---
## \#8 Posted by: faust Posted at: 2016-12-20T21:25:55.370Z Reads: 439

```
I should also say that I don't really need performance. I could be fine with lower top speed and less incline if that'll work with my current battery setup.
```

---
## \#9 Posted by: ArmandR Posted at: 2016-12-20T21:32:07.388Z Reads: 424

```
What are you gonna do with the parts you replaced?
```

---
## \#10 Posted by: JLabs Posted at: 2016-12-20T21:33:54.243Z Reads: 425

```
What a transformation.. I bet you paid a pretty penny for the X2. Did you ride it before taking it apart? If so how did it perform? I was talking to them a while ago and they wanted like $600 or something crazy (compared to their last model)
```

---
## \#11 Posted by: faust Posted at: 2016-12-20T21:48:07.898Z Reads: 422

```
I'm happy to sell them if there's interest. In fact, if Onan doesn't plan to add more urethane, I sent them an inquiry on this. I have a spare X2 complete sitting around that I might be willing to sell too. Otherwise, I might look into tinkering with Urethane next. 

As for my experience with the X2, I was actually pretty happy with it. There were two issues: (1) when you start and stop a lot in the space of a few minutes, it might jump skip the slow acceleration curve and (2) the urethane too thin. I think I could work around the first issue, but there's nothing I can do about the latter. The roads around my neighborhood are pretty crummy, so I rode it around the block once and my numb legs told me it was a no go. That's when I started taking it apart. 

That being said, it was super awesome on smooth roads. It's quiet as hell and didn't seem to be lacking in the power department (unlike my Blink S), though I expect the new hubs will have more power if I can figure out how to deliver the necessary juice. The batteries snap in real nicely.
```

---
## \#12 Posted by: ArmandR Posted at: 2016-12-20T22:01:34.467Z Reads: 404

```
Do you think it could be possible to get the plastic battery holder and trucks from Onan and put really good hub motors and fit in as much cells with 2 vescs and all the other switches and stuff inside?
```

---
## \#13 Posted by: faust Posted at: 2016-12-21T01:48:53.619Z Reads: 439

```
I'm using hummie's Paris trucks right now, which seem superior so I don't think I'll go back to the Onan ones. In addition, the Onan trucks have some nonstandard elements, so they wouldn't work for non-Onan hubs anyways. Also, one of the main reasons I'm doing this is to get a viable modular setup on 125mm trucks for one of my other builds (http://www.electric-skateboard.builders/t/mini-rover-22-carbon-fiber-125mm-trucks-hubs-12s1p-vesc-x/12851).

As for getting things to fit, I took a stab at that today. Dremeling some steel like an idiot and getting metal bits everywhere. I had to spend more time cleaning my station that the work itself. Here's a pic: 
 <img src="/uploads/db1493/original/3X/0/b/0b81e2d4f8f2be16d32a20ea3da39dd26b45c39c.jpg" width="690" height="388">

I went ahead and took my damaged VESC to see how it'd fit. I'm pretty sure I can get two VESCs in there now, as long as heat isn't too much of an issue. <img src="/uploads/db1493/original/3X/5/7/57647610d054818d57abc7fff80b5247a0b16d46.jpg" width="281" height="500">

Worst case scenario, I'd move my switch to the battery back itself, but I think that by hard-wiring some connections, I can get it all in there. One of the bulkiest items is the XT90 splitter.

As for the battery, I think I'm out of luck there. I see the following options:
1. Figure out how to get Hummie's hubs working on 10s2p. Maybe reduced speed/incline, just swapping out batteries earlier when voltage sag kicks in, etc... Maybe there's something I can do to get it to work. I'm after a solid commuter, not a racer. 
2. Move to different hubs or a belt drive system.  I'd rather not go belt if I don't have to, but if it's what's needed for low-current viability, then so be it. Maybe get a geared hub, to allow for better performance at low current. 
3. Build my own battery pack. I think I could probably fit 4 more cells into the existing pack, getting an 8s3p for added discharge. Or get higher end batteries or go lipo.  
4. Use my second X2. Hot swap both battery backs for a 10s4p. I don't really think this is viable because of space on my deck. 

Some questions I wonder if any of you know the answer to: 
* Do you think *any* batteries would work in 2p for Hummie Hubs? Or do I definitely need to be in 3p or greater. 
* Do you think my VESC placement will work?
```

---
## \#14 Posted by: faust Posted at: 2016-12-21T04:26:33.367Z Reads: 422

```
I took the plunge and opened up the battery back. Samsung ICR18650-22P :frowning:
<img src="/uploads/db1493/original/3X/e/1/e14e023e927ece76ff1bc31c49de6203542a3c5a.jpg" width="690" height="388">

This battery pack at 2p can only support 20A continuous. Even if I doubled up and went 4p, I think I'm not going to have enough current (at 40A).

How about these guys at 25A? https://batterybro.com/products/lg-hd2-icr18650hd2-2000mah-25a
Put these in an 8s3p configuration, and I can get 75A. This would get each motor at 37.5A each. 

I guess fundamentally, I'm not sure what the minimums are with dual hub setups. What's the minimum voltage/current I need?
```

---
## \#15 Posted by: Hummie Posted at: 2016-12-21T18:47:00.500Z Reads: 400

```
can the vesc or other esc be programed to have as much power at 8s as 12s?  Can you up the amps to the point ohm's law will allow...up to what the resistance will allow?  (assuming the esc  doesn't overheat and the batteries can put the amps out).  a bit less efficient in the esc and wiring but fine?
```

---
## \#16 Posted by: faust Posted at: 2016-12-21T19:06:40.313Z Reads: 401

```
I suppose that, looking to Mellow's 7s2p setup, the answer is that an 8s3p setup is likely. If heat's an issue, then perhaps cooling could be the solution. I suppose it's just a matter of the right configuration, the parts, and some experimentation. Time to get a spot welder, I suppose. I can then do a 10s2p vs. 8s3p comparison and measure my results. Maybe before then, I can measure just how bad the outcome of having 10A per motor is...
```

---
## \#17 Posted by: DIYtruck3 Posted at: 2016-12-22T09:52:01.512Z Reads: 375

```
I have one unit X2 too, its perfect!
```

---
## \#18 Posted by: faust Posted at: 2016-12-22T16:22:54.364Z Reads: 390

```
[quote="DIYtruck3, post:17, topic:14965, full:true"]
I have one unit X2 too, its perfect!
[/quote]

Interesting. On rough pavement, it was unusable for me. I prefer my old Blink Hub to the Onan X2, slower speed and everything. At least I could feel my legs afterwards.
```

---
## \#19 Posted by: faust Posted at: 2016-12-23T01:51:27.425Z Reads: 416

```
Batteries, batteries, batteries. It's all I've been thinking about lately. The way I see it, here are the options, in order of descending wattage: 
* 12S1P - A123 26650 Batteries (39.6V, 60A, 2376W, 2500mAh, >1000 cycles)
* 8S3P - 16850 LG HD4's (28.8V, 75A, 2160W, 6300mAh, ~200 cycles)
* 8S3P - 16850, 25R5's (28.8V, 60A, 1728W, 7500mAh, > 250 cycles)
* 10S2P - 16850, LG HD4's (36V, 50A, 1800W, 4300mAh, ~200 cycles)
* 10S2P - 16850, 25R5's (36V, 40A, 1440W, 5000mAh, > 250 cycles)

It's a tough call. I love the durability of the A123 batteries, and they'll *barely* fit into the pack. Here's a photo:
<img src="/uploads/db1493/original/3X/2/8/28de07b203f9ad21a22a750a2d30cf621a82d32f.jpg" width="281" height="500">
Those were cuts of wood dipole which happened to measure just a hair over 26mm in diameter. Man, those batteries are HUGE. However, I don't think the energy density is good enough to fit inside such a small pack. 

I'm thinking I'll build a few of the above, depending on what I can get, and also test them against the 10s3p's I'll be getting from the @JLabs group buy (thanks!). 

As an aside, I took apart the hubs today. Here's a peek: 
<img src="/uploads/db1493/original/3X/f/6/f6ec8868ccdb7ef8c75ae913dc4787eddee5fe75.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/d/d/dd2ec932e305c813d4267aef295cbc510abfe799.jpg" width="281" height="500">

It looks like my Onan X2's come with only 11mm of rubber, which is perhaps why things are a bit bumpy for me. There's some new rubber available, so I suppose I'll try that out before I sell off my existing electronics (since it could turn out this could be the fix I need for my unit).   
<img src="/uploads/db1493/original/3X/0/6/06404547f16a2743549eff6af105b62432587142.jpg" width="281" height="500">
```

---
## \#20 Posted by: ArmandR Posted at: 2016-12-23T01:54:27.532Z Reads: 388

```
[quote="faust, post:19, topic:14965"]
12S1P - A123 26650 Batteries (39.6V, 60A, 2376W, 2500mAh, &gt;1000 cycles)
[/quote]

Id go with those.
```

---
## \#21 Posted by: faust Posted at: 2016-12-23T01:56:07.832Z Reads: 375

```
[quote="ArmandR, post:20, topic:14965"]
Id go with those.
[/quote]
I'm tempted, but at 2500mah, I'm thinking I wouldn't even make it 6 miles before I'd need to swap batteries. That's roughly half the distance of the 10S2P 25R5! 

I may not even be able to fit the 12 A123's in there when I get the real thing. Would you still pick that option if it was 10S1P?
```

---
## \#22 Posted by: ArmandR Posted at: 2016-12-23T02:20:42.021Z Reads: 368

```
Your right, then I'd pick anything 10s.
```

---
## \#23 Posted by: DIYtruck3 Posted at: 2016-12-23T02:42:44.871Z Reads: 370

```
agreed! but that is the hub motor. There is no much difference in skateboard, belt electric skateboard or hub motor electric skateboard riding on rough pavement at same speed. just curious maybe Mellow can work this out..thick rubber??
```

---
## \#24 Posted by: faust Posted at: 2016-12-23T03:15:12.628Z Reads: 361

```
The solution is simple: more urethane. My cheap little Acton Blink Hub can ride on my bumpy road with little problem. The only difference is in like 5mm of urethane. I that if X2 made their wheels 5mm's thicker, I'd probably be quite content.

I definitely think Mellow has solved this already. This whole endeavor has me appreciate their design more and more. Of course, certain things sound like magic. Like how can they eke out 1000 charge cycles on 20R's when the spec sheet claims 250?
```

---
## \#25 Posted by: TarzanHBK Posted at: 2016-12-23T14:12:08.630Z Reads: 350

```
These magnets look a bit poor. Big gaps, small and most likely to come loose with a touch of heat.
```

---
## \#26 Posted by: anorak234 Posted at: 2016-12-23T16:16:07.541Z Reads: 346

```
[quote="faust, post:24, topic:14965"]
Like how can they eke out 1000 charge cycles on 20R's when the spec sheet claims 250?
[/quote]

It's all about how you treat the cells. Users on this forum sporting a good BMS and carefully checking the pack every once in a while are bound to get over 1000 cycles
```

---
## \#27 Posted by: faust Posted at: 2016-12-24T00:14:08.504Z Reads: 338

```
[quote="anorak234, post:26, topic:14965"]
It's all about how you treat the cells. Users on this forum sporting a good BMS and carefully checking the pack every once in a while are bound to get over 1000 cycles
[/quote]

I'd love to hear more. Do you have any links you can point me to? I'm thinking that there are two aspects to this: (1) use a BMS with balancing, and (2) don't use the full discharge of the battery (e.g., if you have 20A discharge, use max 10A). Any other tips?
```

---
## \#28 Posted by: anorak234 Posted at: 2016-12-24T01:39:45.190Z Reads: 336

```
http://batteryuniversity.com/learn/article/how_to_prolong_lithium_based_batteries
 I have family members who own Chevy Volts and they gauruntee a certain number of years on the battery because they don't charge or discharge the cells fully which allows for longer life. This does shorten the range of the car each trip but I believe it's worth it in the long run
```

---
## \#29 Posted by: faust Posted at: 2016-12-29T05:43:32.043Z Reads: 366

```
Thanks! As my next step is batteries, this is good stuff to know. I plan to do a three way comparison of batteries that should be able to fit in the swappable pack:

* 25C LIPOs @ 4Ah (100A discharge at 2x5S)
* A123 26650 LifePo4's @ 2.5Ah (50A discharge at 12S1P)
* LG HD4 16854 Li-ion's @ 2.1Ah (75A discharge at 8S3P or 50A discharge at 10S2P)

With the above in mind, I've been having fun getting ready with spot welding.
 <img src="/uploads/db1493/original/3X/f/e/fe7828551224e0188d8085d057e879c7342c09f3.jpg" width="281" height="500">

I also acquired a bunch of volt meters, a hobby charger, a voltage alarm, and a bunch of other stuff. I'm going to take some good advice and not prototype with a BMS. It just introduces another point of failure.
```

---
## \#30 Posted by: faust Posted at: 2016-12-31T03:37:24.049Z Reads: 356

```
It was a challenge, but it looks like I'll be able to get 12S1P with the A123 26650 cells! Ultimately, the dowels were about 0.3mm thicker than the batteries, and I couldn't get them to fit. So I capped each mostly-discharged battery with Kapton tape and took the direct approach. I used those soft earplugs as a sort of putty to help me get the cells at just the right height.

<img src="/uploads/db1493/original/3X/4/5/45c2b89815e714ee88cc0af35a186aa97eedf144.jpg" width="281" height="500">

I think I'll do a four-way comparison of batteries: 
* 10S1P 4000mAH LIPO (100A discharge) -- maybe... 
* 8S3P 6300mAh LG HD4 (75A discharge)
* 10S2P 4200mAh LG HD4 (50A discharge)
* 12S1P 2500mAh A123 (50A discharge)

Taking some good advice from @Hummie, I'm going to skip the BMS for now. It just complicates things. Instead, I've got a Hobby Charger, temperature sensors, and a boat load of voltage LEDs coming in.
```

---
## \#31 Posted by: Hummie Posted at: 2016-12-31T03:43:00.463Z Reads: 333

```
But will ur charger do a high enough voltage? 

 Maybe get some 6s balance plugs u can wire to the cells to use the battery monitors more easily. 
Maybe solder to cells directly or better just solder the wires to copper foil around magnets taped on.
```

---
## \#32 Posted by: faust Posted at: 2016-12-31T04:09:19.532Z Reads: 345

```
That's the plan! I'm going to spot weld two packs of 6, soldering two wire between each nickel joint. One for balancing, and another for monitoring. My hobby charger only goes up to 10S anyways, so it's much more convenient this way. My voltage alarm also only goes up to 8S.
```

---
## \#33 Posted by: faust Posted at: 2016-12-31T09:47:55.930Z Reads: 360

```
Got the 12S1P to fit, and it's all ready to go for the balance connectors! 
<img src="/uploads/db1493/original/3X/6/f/6fead73bba4f04b5fa46d3d5d7de30a6f1fe4e17.jpg" width="690" height="388">
```

---
## \#34 Posted by: faust Posted at: 2017-01-15T23:38:28.911Z Reads: 368

```
I received my new LG HD4 batteries, which are capable of 25A discharge. My plan was first to simply build a 10S2P setup, which would get me 50A, but then I realized I could do 8S3P by removing the BMS and going with the hobby charger approach. So I ordered 4 more batteries and waited... Then I realized that, with a little more case hacking, I could fit 30 batteries in that little enclosure! So I ordered 7 more batteries and waited... 

I've finally got my perfect hot swappable battery. It's capable of 75A discharge and 6300mAh @ 36V and I can simply plug it into my hobby charger to balance while charging. So I should no longer be current-limited in my builds. 

First, I made some more room in the case with the dremel and cut a small square hole for the female 10pin JST-XH connection. I then glued that in, ensuring there was enough clearance for the little guiding slots on the male connector to fit. 
<img src="/uploads/db1493/original/3X/3/e/3e824979535cbc1a292079bf0d504c8d185a07ba.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/9/e/9eedd4a312e18ec519198f2537942b804029085f.jpg" width="281" height="500">

I then ran through a dry run, just like I did with the A123 26650 batteries. Figuring just the right placement to ensure everything will fit. <img src="/uploads/db1493/original/3X/d/9/d9459fa1ecb1687affb928d25b677e8e6b91f598.jpg" width="281" height="500">

Learning from last time, my approach to building the pack was do all my soldering first, then to do the spot welding. This is MUCH easier than soldering between batteries. It also looks a lot nicer. 
<img src="/uploads/db1493/original/3X/b/5/b53db71c6e161b911d1e885dc5d9fb06ecbb57f3.jpg" width="690" height="388">

I also labeled everything on a sharpie, so I wouldn't have to think while welding. 
<img src="/uploads/db1493/original/3X/e/b/ebaed734b693ecbf13a1541ed5679fe5b0cc730b.jpg" width="281" height="500">

And there you have it!
<img src="/uploads/db1493/original/3X/4/a/4adb34eb701fdac68cd4b3ea1e84216aff9d4586.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/4/d/4d705ea4cbacde4c224ef4abf1eeada182fc17ee.jpg" width="281" height="500">

This is a really powerful battery for its size. I'm really happy with the results. Next steps are to weather product and heat shrink and all that, but I'm still waiting on materials. I think I'll go back to the chassis/VESC hacks while I wait.
```

---
## \#35 Posted by: daanstoorvogel Posted at: 2017-01-24T16:52:29.279Z Reads: 335

```
@faust   enything yet ? i am excited for this one !
```

---
## \#36 Posted by: faust Posted at: 2017-01-25T06:33:31.145Z Reads: 369

```
Now that I got the batteries good to go, I started work on the enclosure. My biggest issue was with the connectors taking too much space and the 10AWG wire not being flexible enough, so I had to do quite a bit of work on the VESC. Here's what I did: 
1. Replaced the 10AWG wire leading from battery to the XT90 with 2x14AWG wires direct to the battery connector. Given the battery enclosure already has 2x14AWG, I think this should be sufficient. If not, I've got a lot of work modding the battery pack. 
2. Replaced the 10AWG wire to the motor leads with 12AWG wire, this enables me to bend the connectors so that I can mount a 5.5 bullet connector in the case itself. 
3. "Split" the VESC so that it rests on the capacitors and secure in place with Kapton tape.
4. Hack the GIANT sparkless switch from DIY to give it a reduced profile. 
5. Drill holes directly into the case to mount the motor connectors. Increase the current hole so that I can fit the sensor wires through. 

I tested this with two VESCs, and with the above changes both will fit fine. Right now, so I'm testing a simple single belt drive setup. I'm going to put in on my little bench "dyno" and ensure that the heat isn't an issue or anything before I hack apart another VESC to get it to fit in there. It's SO quiet in FOC, it's amazing! I'll send a video later. 

<img src="/uploads/db1493/original/3X/f/e/feac82a7f1a91f4a4a599fefaf38fa30734e12a9.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/a/4/a47f77a77697bcfb7c6dfc80ad69afbb645b6461.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/4/d/4d0ce06c3080e9ca0a81c674a4b7e45b77082808.jpg" width="690" height="388">

I'll clean everything up later, once I have it tested. 

The main downside with the Onan X2 hack is that it doesn't work all that well for belt drive, since the motor lacks clearance under the board. Anyone know where I can get a longer motor mount? I need it to be about 3/4" longer so that I can use this approach for my Mini Rover build.
```

---
## \#37 Posted by: Eboostin Posted at: 2017-03-11T21:07:45.275Z Reads: 335

```
Any updates? Great work so far!
```

---
## \#38 Posted by: faust Posted at: 2017-03-17T05:42:43.711Z Reads: 339

```
Thanks! Unfortunately, one of my VESC-X's from Enertion was DOA, so this build is waiting on that. However, I implemented a second Onan hack with my Rover Build. 
<img src="/uploads/db1493/original/3X/d/9/d916072bc1f12cf5f3fcb99bee5bd8789ecfd539.jpg" width="281" height="500">

Here's a quick clip: https://www.youtube.com/watch?v=0fWOcp-MFo4&feature=youtu.be
```

---
## \#39 Posted by: oct0f1sh Posted at: 2017-05-21T06:00:40.266Z Reads: 298

```
Hey man, we met at the makerfaire today and I gotta say I'm super inspired by your builds. Hot swappable batteries are a great idea, and it's pretty awesome that you were able to fit 10s3p in that tiny enclosure. I'm going to have to try to play around with the idea of a removable battery.
```

---
## \#40 Posted by: edwardlui531 Posted at: 2017-05-22T07:49:44.683Z Reads: 285

```
Also met you at the faire today.
Check out my board "fishie"
```

---
## \#41 Posted by: faust Posted at: 2017-05-24T01:36:49.302Z Reads: 275

```
Hey octof1sh! Thanks for the compliment, and I'm glad you liked the board. It was really fun being able to ride it around the faire :) 

It makes me wonder if the should be an esk8 builders meetup in the bay area or something... There's was quite a lot of us at the faire. Anyhow, feel free to drop me a note or post here if there's anything I can help with in your endeavors.
```

---
## \#42 Posted by: faust Posted at: 2017-05-24T01:43:04.625Z Reads: 267

```
Will do, checking out the build now! Thanks for dropping me a note.
```

---
## \#43 Posted by: edwardlui531 Posted at: 2017-05-24T03:29:06.020Z Reads: 262

```
We should have a esk8 booth next year at the fair, you think we can make that happen?
```

---
## \#44 Posted by: faust Posted at: 2017-10-12T03:47:40.327Z Reads: 222

```
Definitely.
```

---
## \#45 Posted by: typhoon Posted at: 2018-01-26T10:55:59.037Z Reads: 196

```
tell me please the base ESC on ONAN is it vesc ? I wanna make some hack like you but i place TORQUE Single Hub Motor (collections/electric-skateboard-hub-motors/products/torque-single-hub-motor)  so i wanna know what the type of esc and battery be better
```

---
## \#46 Posted by: ploek Posted at: 2018-05-28T16:24:12.399Z Reads: 160

```
does anyone know if it's possible to program the ESC on onan booster x2.1?
```

---
## \#47 Posted by: rey8801 Posted at: 2018-05-29T13:45:01.000Z Reads: 162

```
If the ESC is the standard chinese one (meepo, woogo, ownboard, backfire ecc...) and I am afraid this is the case, no it's not possible because it is not open source. You can either replace it with 2 VESC (dual hub at least for onan booster, right?) or in order to save money now the chinese companys had released a new ESC that seems having a smoother acceleration and brakes. Depend of what youare looking for and the budget available.
```

---
## \#48 Posted by: faust Posted at: 2018-06-22T00:25:12.587Z Reads: 146

```
The base ESC is most definitely not VESC. To make this build work, you need to gut the Onan and put a VESC in there. Two is a tight fit, but doable.
```

---
## \#49 Posted by: ploek Posted at: 2018-07-05T13:32:17.877Z Reads: 146

```
So it is possible to control the onan x2 hubs with two vesc 6 controllers insteat of the cheap chinese esc inside?
```

---
## \#50 Posted by: faust Posted at: 2018-08-24T01:12:35.472Z Reads: 122

```
Yep! Of course, you've got to wire up the sensor connections.
```

---
## \#51 Posted by: Bart_Dood Posted at: 2018-09-23T05:26:06.234Z Reads: 94

```
Hi Faust, (and others) I just got an onan (labelled as nuff board) and it has a dead controller board. Is anyone who has gutted their onan unit willing to sell me their old controller pcb? I believe the big board in mine is ok it's the daughterboard that is fried, so even if someone's main pcb was damaged I could probably still use it. I'm in northern California... Thanks!

UPDATE: I got VESC controllers instead. I actually wrote to ONAN in china and at first they offered me a new control board for $85 but then started to bait and switch me up to $345 for everything including shipping. Real rip off, so I went VESC instead
```

---
## \#52 Posted by: Richter Posted at: 2018-10-01T01:08:02.394Z Reads: 82

```
Hey mate, how difficult would it be to get a drive belt motor and just swap the 3 power cable's out for the ones already connected to the hub? 

Could we make an off road conversion using this technique?
```

---
## \#53 Posted by: faust Posted at: 2018-10-21T19:18:37.644Z Reads: 77

```
Unfortunately not. The cables are low-current and I believe the ESC wouldn't supply enough current anyways. You'd need to swap in 2 VESCs. There's also the clearance issue (since the AT wheels would have wheelbite on the chassis). 

I managed to do this by moving the chassis forward, but it was basically a full overhaul.
```

---
## \#54 Posted by: City-Blade-101 Posted at: 2019-05-07T17:06:34.824Z Reads: 41

```
Why weren't 12s2p 30Q by skipping the bms anyways an option?
```

---
