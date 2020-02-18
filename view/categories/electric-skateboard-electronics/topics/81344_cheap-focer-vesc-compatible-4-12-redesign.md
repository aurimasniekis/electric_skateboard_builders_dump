# Cheap FOCer! (VESC compatible 4.12 redesign)

### Replies: 436 Views: 9616

## \#1 Posted by: shaman Posted at: 2019-01-19T03:28:21.442Z Reads: 756

```
![vesc%20angled|690x379](upload://li6EeWZOFLimP2PAfwl5ugFb9p.png) 
Top

![vesc%20bottom|690x341](upload://wpSrVgn0lVl4eJmSX4B1xDYKhTK.png) 
Bottom

Hey there. I’m rehashing the VESC into a cheaper 2 layer version with external FETs. I’ll call it the Cheap VESC for now. You may notice it resembles the generic ebike controllers that you can find on ebay/aliexpress. This is a version that would probably cater more toward the ebike/e-scooter community but probably could still fit just fine on a skateboard. The primary goal here was to make a version of the VESC that is cheaper to create by reducing the original design to 2 layers (check out JLC PCB for super-duper cheap 2 layer boards) and reduce BOM cost a little. The secondary goal was simply to improve my own PCB layout and design skills by taking on this challenge. I still haven’t finalized the design but I would say I am at least 95% done with only a few minor problems to tidy up. I also have a thread on the endless sphere that I encourage you to check out. Feel free to make suggestions and ask questions. Note that this is my most complex board design for me so far with my previous experience being only with simple audio effect boards and circuits.

Cheap VESC

Advantages

* Lower build and BOM cost

* TO-220 FETs allow for big heat sink attachment for better thermal performance

* SMD components no smaller than 0805 make hand assembly practical

* Added ON/OFF capability to turn off control circuitry when controller is not in use. A simple mechanical switch will achieve this when connected to the “ON/OFF” 2-pin header.

* Can fit in typical "350W" ebike enclosures

* Can fit in Hammond 1590b enclosures

Disadvantages (that I know of)

* Larger than original VESC. Cheap VESC is 45mm x 92mm

* Higher profile with TO-220 package FETs

* Additional assembly steps to beef up high-current traces. 2 layers of 1oz copper can’t handle the current flowing through during operation. Assembler will have to apply wire/solder wick/bus bar to the exposed Power, Ground, and Phase traces that you can see in the “bottom” image.

*Less than ideal layout for reducing loop area and inductance. Nothing crippling IMO but will be addressed in the future HV version.

Features of Future Versions (Calling them the High Voltage (HV) 6 and 12 FET versions)

* Implementing DRV8353 for higher voltage operation (I estimate at least 20s capable). Will need stable version of VESC 6 firmware/software for the 3 phase current sensing and stuff.

* On-board circuitry for no-spark connection

* On-board Bluetooth capability for interface with Open Source Android app for the VESC

*A 12 MOSFET version with the FETs in parallel for even greater power.

*Experimentation with mineral oil filled enclosure for improved thermal dissipation. I am aware of potential wicking issues. I am aware that circulation improves thermal performance. I will be conducting a "before and after" analysis for seeing if it's all worth it.

Further Notes:
I intend to test the design rather thoroughly after I get a version assembled. I intend to power a motor under load with different loads while observing temperature with a thermal camera. I will test other features of the design to ensure quality. Because of all this, it will be some time before I release the design files as Open Source. I don’t want to give the community a broken thing.

See existing thread here [https://endless-sphere.com/forums/viewtopic.php?f=7&t=97699](http://)

All this wouldn’t be possible without Benjamin Vedder’s hard work to build on. Please consider supporting him for his efforts through the link below.

https://vesc-project.com/donations
```

---
## \#2 Posted by: mishrasubhransu Posted at: 2019-01-19T03:56:21.807Z Reads: 625

```
This is awesome. I would be interested to use something like this for bikes. Especially since I can attach to a massive heatsink.

What's the estimated cost at the moment?
```

---
## \#3 Posted by: shaman Posted at: 2019-01-19T04:02:18.065Z Reads: 615

```
Just the board and BOM is $30ish USD if you use JLC PCB, LCSC, and get free samples from TI. You can make an account on their website and snag 5 free samples of most ICs. Also, you can get cheap STM32s the same way you just gotta pay for shipping. 3 STM32s were $9ish with domestic shipping from the ST site.
```

---
## \#4 Posted by: moon Posted at: 2019-01-19T10:43:50.263Z Reads: 585

```
Hey

I was the person who invited you here on endless sphere, welcome

@b264
```

---
## \#5 Posted by: b264 Posted at: 2019-01-19T10:47:36.503Z Reads: 549

```
This is really awesome!

[quote="shaman, post:1, topic:81344"]
I’ll call it the Cheap VESC for now.
[/quote]

"VESC" is supposedly trademarked, so I would give it a different name and say "Based on VESC 4.12" so folks know it's software-compatible

Maybe like TallESC or something
```

---
## \#6 Posted by: Andy87 Posted at: 2019-01-19T11:15:04.095Z Reads: 523

```
Great to have you here!
Finally somebody working on higher voltages instead of just pumping up the amp capability.
20s sounds crazy but would make the current 12s projects way saver.
Maybe I overread it, but what you think which currents your esc will be able to handle.
```

---
## \#7 Posted by: Bor.inc Posted at: 2019-01-19T11:20:15.349Z Reads: 499

```
Wow 30$ is not much, im following this thread
```

---
## \#8 Posted by: Acido Posted at: 2019-01-19T11:45:34.675Z Reads: 488

```
30$ is dirt cheap..
Can we expect a simmilar performance to the flipsky vesc or tb?
```

---
## \#9 Posted by: ryansinatra Posted at: 2019-01-19T11:49:06.723Z Reads: 475

```
Watching this as well 👌
```

---
## \#10 Posted by: AlexBE Posted at: 2019-01-19T12:14:50.108Z Reads: 466

```
Guys, $30 is the board + BOM cost. Still need to add assembly, test, programming, shipping, margin........
```

---
## \#11 Posted by: moon Posted at: 2019-01-19T12:18:43.561Z Reads: 462

```
He is making this possible by hand soldering

And it's open source so you are free to make it for $30 if you wish

Compare it to a vesc 6 bom where the value is $60. Nothing stops you making it for $60 unit cost
```

---
## \#12 Posted by: shaman Posted at: 2019-01-19T12:51:08.147Z Reads: 481

```
[quote="b264, post:5, topic:81344"]
“VESC” is supposedly trademarked, so I would give it a different name and say “Based on VESC 4.12” so folks know it’s software-compatible

Maybe like TallESC or something
[/quote]

Thanks for catching that. I'll release it under a different name when the time comes.

[quote="Andy87, post:6, topic:81344, full:true"]
Great to have you here!
Finally somebody working on higher voltages instead of just pumping up the amp capability.
20s sounds crazy but would make the current 12s projects way saver.
Maybe I overread it, but what you think which currents your esc will be able to handle.
[/quote]

I expect this to handle at least the same current from the original 4.12. Ideally it handles even more due to the ability to heatsink the FETs. I will be testing it's current handling limits in a lab with a motor on a dyno.

[quote="Acido, post:8, topic:81344, full:true"]
30$ is dirt cheap…
Can we expect a simmilar performance to the flipsky vesc or tb?
[/quote]

This idk unfortunately. I'm not an experienced user of the VESC or it's spin-offs so I personally can't compare them. I will be having a few people test this design in their rigs to get feedback on performance.

[quote="moon, post:11, topic:81344, full:true"]
He is making this possible by hand soldering

And it’s open source so you are free to make it for $30 if you wish

Compare it to a vesc 6 bom where the value is $60. Nothing stops you making it for $60 unit cost
[/quote]

Exacly! Thank you. This is meant to be cheap if you DIY. Prices for large quantity manufacturing is a different story. 

I appreciate the warm welcome from everyone so far! I hope to have some initial results soon as I'm populating my first board today. Wish me luck!
```

---
## \#13 Posted by: rey8801 Posted at: 2019-01-19T13:16:15.320Z Reads: 412

```
Amazing! I would like to know what performance can we aspect from it and if it possible to make like a basic and pro version for a 12s,13s set up.
```

---
## \#14 Posted by: b264 Posted at: 2019-01-19T13:23:51.345Z Reads: 406

```
More current is always good, but what we've noticed around here is it's actually the voltage limits that are constraining next-gen engineering.  It's the 60V DRV8302 that's the #1 limiting factor
```

---
## \#15 Posted by: shaman Posted at: 2019-01-19T13:24:31.581Z Reads: 409

```
[quote="rey8801, post:13, topic:81344, full:true"]
Amazing! I would like to know what performance can we aspect from it and if it possible to make like a basic and pro version for a 12s,13s set up.
[/quote]

I see this performing at least as well as the VESC 4.12 but probably better because of the ability to heatsink the FETs well. The future HV versions will be candidates for your "pro" versions.
```

---
## \#16 Posted by: shaman Posted at: 2019-01-19T13:26:10.308Z Reads: 406

```
[quote="b264, post:14, topic:81344, full:true"]
More current is always good, but what we’ve noticed around here is it’s actually the voltage limits that are constraining next-gen engineering. It’s the 60V DRV8302 that’s the #1 limiting factor
[/quote]

Exactly. That's why I'm looking at the DRV8353 for the HV versions. More voltage, More better.
```

---
## \#17 Posted by: rey8801 Posted at: 2019-01-19T13:29:19.936Z Reads: 393

```
The external fet is brilliant. I now start making some CNC work and it will allow perfect cooling.
```

---
## \#18 Posted by: AlexBE Posted at: 2019-01-19T13:31:33.228Z Reads: 400

```
So is the BOM cost $30 if you are only building one board? If so, the volume cost should be $10. Or is the volume cost $30?
```

---
## \#19 Posted by: Bor.inc Posted at: 2019-01-19T13:41:09.794Z Reads: 407

```
Well if you need testers? ;)
```

---
## \#20 Posted by: shaman Posted at: 2019-01-19T13:50:08.253Z Reads: 411

```
[quote="AlexBE, post:18, topic:81344, full:true"]
So is the BOM cost $30 if you are only building one board? If so, the volume cost should be $10. Or is the volume cost $30?
[/quote]

Yes. 1 board for the DIYer is $30ish. Volume would be cheaper like you said depending on which FETs you use and a few other variables.

[quote="Bor.inc, post:19, topic:81344"]
Well if you need testers? :wink:
[/quote]

Look for a PM.
```

---
## \#21 Posted by: Benjamin899 Posted at: 2019-01-19T14:29:28.210Z Reads: 361

```
I don't mind the thickness. Normal 4.12 vesc takes alot of space in terms of length because of the capacitors. 
What are the final measurements (Lenght/width/height)?
```

---
## \#22 Posted by: rey8801 Posted at: 2019-01-19T14:31:09.110Z Reads: 360

```
Well I am making my own direct drive motors and planning to pair with a 12s setup. I still miss the vesc so if you need tester I could try the "pro version" of you end up making it. Are you thinking to a single vesc or a dual configuration? Most of the builders use it for dual set up anyway, maybe that will keep the cost lower since you would need only one board and some hardware is shared.
Are you going to use a hot air station for making it? 
Of course I do not want anything for free. I could try it and send it back to you or other users. I can also buy it later if it performs well. If the heatsink is needed then I will make the design and machine it. Anyhow, great work! :wink:
```

---
## \#23 Posted by: shaman Posted at: 2019-01-19T15:17:20.998Z Reads: 351

```
[quote="Benjamin899, post:21, topic:81344, full:true"]
I don’t mind the thickness. Normal 4.12 vesc takes alot of space in terms of length because of the capacitors.
What are the final measurements (Lenght/width/height)?
[/quote]

92mm x 45mm x 23mm(approx). I reduced the Caps from 1000uf to 680uf so the board height would allow for fitting in the hammond enclosure. Before the change the caps were taller than the FETs.
```

---
## \#24 Posted by: shaman Posted at: 2019-01-19T15:23:20.336Z Reads: 351

```
[quote="rey8801, post:22, topic:81344, full:true"]
Well I am making my own direct drive motors and planning to pair with a 12s setup. I still miss the vesc so if you need tester I could try the “pro version” of you end up making it. Are you thinking to a single vesc or a dual configuration? Most of the builders use it for dual set up anyway, maybe that will keep the cost lower since you would need only one board and some hardware is shared.
Are you going to use a hot air station for making it?
Of course I do not want anything for free. I could try it and send it back to you or other users. I can also buy it later if it performs well. If the heatsink is needed then I will make the design and machine it. Anyhow, great work!
[/quote]

I haven't considered a dual setup before but I believe it could be a future variant. Shouldn't be too hard to combine the layouts of 2 boards into one. I will be using a hot air reflow station for soldering. I've already done the top side and just gotta finish the bottom. My idea of the heatsink would just be an aluminum bar attached to the FETs, then mounting the aluminum bar to the inner wall of the enclosure. This would the easy way for a DIYer but by all means machine an awesome heatsink!
```

---
## \#25 Posted by: Benjamin899 Posted at: 2019-01-19T15:23:49.098Z Reads: 319

```
Just to compare a 4.12 cnc case is 121mmx45mmx21.5mm
So i personally think your dimensions are much more to my liking.
```

---
## \#26 Posted by: shaman Posted at: 2019-01-19T15:25:13.792Z Reads: 322

```
Cool. Just to be clear the dimensions I gave are for the populated board without an enclosure. The 1590b enclosure would be about the smallest  profile you can get away with.
```

---
## \#27 Posted by: b264 Posted at: 2019-01-19T15:25:17.430Z Reads: 325

```
Dual setups mean that if one side breaks, you have to replace both sides.  A modular setup is much better.
```

---
## \#28 Posted by: shaman Posted at: 2019-01-19T15:27:31.503Z Reads: 308

```
good point!
```

---
## \#29 Posted by: Benjamin899 Posted at: 2019-01-19T15:30:21.124Z Reads: 310

```
Still. it is easier to make your enclosure under your board a bit thicker at the spot your Vesc comes, than longer. At one point you run out of board.
```

---
## \#30 Posted by: moon Posted at: 2019-01-19T15:56:09.404Z Reads: 310

```
[quote="shaman, post:1, topic:81344"]
* On-board circuitry for no-spark connection
[/quote]

What do you mean by this?

Also is that USB type C?
```

---
## \#32 Posted by: Andy87 Posted at: 2019-01-19T16:26:46.586Z Reads: 306

```
Just wanted to say that too.
Please @shaman stay with a single design.
A dual heat sink box is more than enough, no need to combine the pcbs and share components.
One thing you maybe could consider to solve if not solved yet. The old 4.12 design had the problem that if you use CAN bus to control both vesc and the CAN bus got disconnected while both where powered on it was very likely that the communication port got fried too.
In some newer designs of the focbox for example was this problem solved (unfortunately idk how)
```

---
## \#33 Posted by: moon Posted at: 2019-01-19T16:33:08.363Z Reads: 291

```
Btw, the focbox is a VESC 4.12 based ESC.
```

---
## \#34 Posted by: shaman Posted at: 2019-01-19T16:33:10.987Z Reads: 305

```
[quote="moon, post:30, topic:81344"]
> * On-board circuitry for no-spark connection

What do you mean by this?

Also is that USB type C?
[/quote]

I was referring to no-spark connection for when one is connecting the battery.  Essentially would be a pre-charge circuit for the bulk caps. The connector for the cheap vesc is mini usb (idk what was i thinking...) and was going to use micro for the HV versions. USB C seems overkill.
```

---
## \#35 Posted by: moon Posted at: 2019-01-19T16:33:50.681Z Reads: 292

```
[quote="shaman, post:34, topic:81344"]
I was referring to no-spark connection for when one is connecting the battery. Essentially would be a pre-charge circuit for the bulk caps. The connector for the cheap vesc is mini usb (idk what was i thinking…) and was going to use micro for the HV versions. USB C seems overkill.
[/quote]

paging @b264

USB C is nice imo
```

---
## \#36 Posted by: b264 Posted at: 2019-01-19T16:35:14.318Z Reads: 289

```
MiniUSB is way better than MicroUSB

MicroUSB are crap and always stop working.  USB-C are very good.

The only benefit to microUSB is that everyone already has them on phone chargers
```

---
## \#37 Posted by: b264 Posted at: 2019-01-19T16:36:14.399Z Reads: 317

```
[quote="shaman, post:34, topic:81344"]
I was referring to no-spark connection for when one is connecting the battery. Essentially would be a pre-charge circuit for the bulk caps.
[/quote]

So then, you know about this :sunglasses:

https://www.electric-skateboard.builders/t/vedder-antispark-design-problem-or-implementation-problem/77967/4?u=b264
```

---
## \#38 Posted by: b264 Posted at: 2019-01-19T16:37:47.167Z Reads: 316

```
Honestly I think it's better to keep a separate antispark switch / power supply because it allows more freedom.  For example, some folks want auto poweroff, some want roll-to-start (no power switch) and all the other things regarding integrating other lights and accessories mean that builtin antispark switches are less desireable.  Plus, if they fail, then the whole ESC has to be replaced...
```

---
## \#39 Posted by: Andy87 Posted at: 2019-01-19T16:38:21.621Z Reads: 313

```
That’s why is said in the latest version of focbox 😉
```

---
## \#40 Posted by: moon Posted at: 2019-01-19T16:39:12.446Z Reads: 307

```
Yeah, I am not sure if @shaman is up to date with all these vescs - don't know though
```

---
## \#41 Posted by: moon Posted at: 2019-01-19T16:43:36.712Z Reads: 310

```
@shaman

Has hit his reply limit so  no responses for 11 hours
```

---
## \#42 Posted by: Andy87 Posted at: 2019-01-19T16:47:27.104Z Reads: 294

```
That’s sad 😔
```

---
## \#43 Posted by: deucesdown Posted at: 2019-01-19T17:10:47.221Z Reads: 305

```
For reference, I think he's intending to house it in these things.

http://hammondmfg.com/jpeg/1590BInt_B.jpg

For scale

https://t2conline.com/wp-content/uploads/2018/05/pedalboardredchucksEDIT.jpg

Cool idea! Guitar toys is another area where I have an addiction.
```

---
## \#44 Posted by: Bor.inc Posted at: 2019-01-19T17:22:34.724Z Reads: 297

```
Oh is that sort of a rule for newcommers (im not that familiar with the perks of all the ranks) can we still pm him?
```

---
## \#45 Posted by: moon Posted at: 2019-01-19T17:25:01.363Z Reads: 290

```
Dont think there is anything stopping you
```

---
## \#46 Posted by: Vanarian Posted at: 2019-01-19T17:33:09.575Z Reads: 298

```
[quote="shaman, post:1, topic:81344"]
DRV8353
[/quote]

So there **is** a higher voltage DRV chip, FFS! 

Welcome here man, I'm impatient to see your work running!

Edit : Quick question, is the trade-off about max source current and max sink current relevant for our use? 50mA to 1A peak and 100mA to 2A peak instead of 1.7A and 2.3A?
```

---
## \#47 Posted by: shaman Posted at: 2019-01-20T14:36:23.172Z Reads: 307

```
So yeah I couldn't respond to anything... even PMs.  I believe the rule is to mitigate spam from noobs but it was kind of a bummer that I couldn't keep up with my thread. I will have to limit my responses for a while and try to lump as many responses into one post as I can.

[quote="b264, post:36, topic:81344, full:true"]
MiniUSB is way better than MicroUSB

MicroUSB are crap and always stop working. USB-C are very good.

The only benefit to microUSB is that everyone already has them on phone chargers
[/quote]

Ok. It's not a bid deal from the design perspective wither way. USB C is the future anyways.

[quote="b264, post:38, topic:81344, full:true"]
Honestly I think it’s better to keep a separate antispark switch / power supply because it allows more freedom. For example, some folks want auto poweroff, some want roll-to-start (no power switch) and all the other things regarding integrating other lights and accessories mean that builtin antispark switches are less desireable. Plus, if they fail, then the whole ESC has to be replaced…
[/quote]

I appreciate the insight as I'm not an esk8 user and am not familiar with the configurations people like. This is the advice I need from this community so that my design makes the majority happy.

[quote="deucesdown, post:43, topic:81344"]
Cool idea! Guitar toys is another area where I have an addiction.
[/quote]

This is exactly the enclosure I have in mind and the idea came from my own guitar effect pedal design/fabricating experience.

[quote="Vanarian, post:46, topic:81344"]
Quick question, is the trade-off about max source current and max sink current relevant for our use? 50mA to 1A peak and 100mA to 2A peak instead of 1.7A and 2.3A?
[/quote]

This is a very good question that I looked up myself back when I was investigating the DRV8323 as an option. Source/sink current limits for driving FETs is a very important number. It translates to how large of a a gate charge your FETs can have or how many in parallel can you run. The DRV8353 has lower current source/sink numbers but this will be ok with FETs that have an appropriately sized gate charge to match. TI's NEXFETs can offer low Rds on still with low gate charges that will do well here.
```

---
## \#48 Posted by: shaman Posted at: 2019-01-20T17:13:07.497Z Reads: 282

```
So thinking about the names for my controllers since VESC isn't an option. I have one idea but it's not exactly the most professional. I'll just leave this here...

Cheap controller = Cheap FOCer
6 FET HV version = Uncle FOCer
12 FET HV version = Mother FOCer
```

---
## \#49 Posted by: rich Posted at: 2019-01-20T19:51:43.853Z Reads: 280

```
First of all great project, looking forward to the finished ESC.

If you need a hardcore tester who is trying to kill it offroad then I'm your man :laughing:

What about calling it a Shesc or ShamanESC?
```

---
## \#50 Posted by: shaman Posted at: 2019-01-21T00:23:24.087Z Reads: 271

```
[quote="rich, post:49, topic:81344"]
What about calling it a Shesc or ShamanESC?
[/quote]

I might work Shaman into the name somehow. We've got time to think about it.
```

---
## \#51 Posted by: shaman Posted at: 2019-01-21T00:32:56.861Z Reads: 278

```
So I have several people interested in testing my controller between here and the sphere. I do need these testers so that I get good data form several different use cases. The problem is sourcing the amount controllers needed for the testers. There's no way that I can make multiples of these controllers by hand during my spare time. Some testers may be able to solder the boards up themselves but that leaves plenty of opportunity for human error (just like in my own prototype so far). I'm considering having a PCB assembly service make some of these for me but I don't have the cash to front for that. https://www.7pcb.com/ quoted me about $600 for 15 boards. I have a couple of questions for this community...

Do you guys think it would be successful to have a gofundme or patreon or something like that to help with these kinds of things? If not, what would be the alternatives?
```

---
## \#52 Posted by: moon Posted at: 2019-01-21T00:37:05.185Z Reads: 273

```
![image|300x356](upload://6ieQnPGjdRtMfEOouWPHpxcBq09.jpeg)
```

---
## \#53 Posted by: moon Posted at: 2019-01-21T00:38:39.894Z Reads: 277

```
[quote="shaman, post:51, topic:81344"]
I’m considering having a PCB assembly service make some of these for me but I don’t have the cash to front for that. https://www.7pcb.com/ quoted me about $600 for 15 boards. I have a couple of questions for this community…

Do you guys think it would be successful to have a gofundme or patreon or something like that to help with these kinds of things? If not, what would be the alternatives?
[/quote]

Theres group buys. But your are too new here to facilitate one of those 

Or theres a user called @Samau18 who lives in Hong Kong and seems like he has good thing going when it comes to PCBA. Maybe he can make some of these boards. He already makes BMS's for this forum and it looks like he has a good attention to detail
```

---
## \#54 Posted by: shaman Posted at: 2019-01-21T01:43:43.379Z Reads: 254

```
I don't get the ork thing....
```

---
## \#55 Posted by: shaman Posted at: 2019-01-21T01:44:48.339Z Reads: 252

```
Does @Samau18 have a website that you know of or should I just hit him up by PM?
```

---
## \#56 Posted by: moon Posted at: 2019-01-21T01:45:40.204Z Reads: 268

```
https://dota2.gamepedia.com/Shadow_Shaman

[quote="shaman, post:55, topic:81344, full:true"]
Does @Samau18 have a website that you know of or should I just hit him up by PM?
[/quote]

I don't know about that, I guess he'll see these messages and respond, or you can PM him
```

---
## \#57 Posted by: shaman Posted at: 2019-01-21T01:52:51.779Z Reads: 272

```
Ok. Shadow Shaman is pretty cool name. Too bad it's taken. Maybe I'll reverse and do something like the Shaman Shadow or Shaman Spirit. Less crude than my other idea.
```

---
## \#58 Posted by: shaman Posted at: 2019-01-21T02:01:38.118Z Reads: 284

```
![pedal|281x500](upload://xmQ3b2IUpDrUpooLoJCPPmoXdOi.jpeg) 

So I've done acid etched graphics in the past with my effect pedals. I could theme some custom enclosures for my controllers with shaman-ish spiritual/ritualistic symbols kind of like mine from the pic. Don't know how popular that would be or if it's worth the hassle. I don't know how to do this kind of thing in volume.
```

---
## \#59 Posted by: Samau18 Posted at: 2019-01-21T02:05:07.341Z Reads: 268

```
I am here, but don’t think I will get into vesc 4.  “Maybe” if vesc 6 later
```

---
## \#60 Posted by: shaman Posted at: 2019-01-21T02:06:29.043Z Reads: 267

```
No worries. I'll let you know when it's time for my VESC 6 based high voltage controllers. I appreciate giving me an answer so quickly.
```

---
## \#61 Posted by: moon Posted at: 2019-01-21T02:27:13.302Z Reads: 262

```
Something like this could be laseretched or something?
```

---
## \#62 Posted by: shaman Posted at: 2019-01-21T02:32:26.226Z Reads: 250

```
Sure. Then polished and clear coated. It's not a complicated process I'm simply not familiar what services would do that if I sent them 100+ enclosures. I'm sure 10 mins of googling would yield something but I'm feeling lazy at the moment.
```

---
## \#63 Posted by: moon Posted at: 2019-01-21T02:33:13.628Z Reads: 240

```
How much does the enclosures cost?
```

---
## \#64 Posted by: shaman Posted at: 2019-01-21T02:36:46.285Z Reads: 252

```
https://www.aliexpress.com/item/10-Pcs-The-Original-1590B-Type-Now-PB-N1160-Type-Guitar-Effect-Pedal-Box-112-L/1761953011.html?spm=2114.search0104.3.1.370b1c9cCNRF2a&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10068_10130_10890_10547_319_10546_10548_317_10545_10696_453_10084_454_10083_433_10618_431_10307_537_536_5736111_5736011_10059_10884_10887_100031_321_322_10103-10890,searchweb201603_51,ppcSwitch_0&algo_expid=93d9a14c-efdd-4bf2-a8e0-c395689a9e9b-0&algo_pvid=93d9a14c-efdd-4bf2-a8e0-c395689a9e9b

Real hammonds are $6ish USD in bulk. You can get clones for $4 or better buying 5 at a time
```

---
## \#65 Posted by: moon Posted at: 2019-01-21T02:38:20.440Z Reads: 247

```
OK thats seriously cheap. I do have access to a laser cutting machine so when this takes off I can do some for fun
```

---
## \#66 Posted by: shaman Posted at: 2019-01-21T02:40:31.896Z Reads: 248

```
Yep. That's why I targeting the hammond style for the choice enclosure of my controllers. Cheap, effective, and you can get the gasket for them that seals out water and dust.
```

---
## \#67 Posted by: moon Posted at: 2019-01-21T02:44:37.634Z Reads: 251

```
Yes, and this forum is very powerful. So I hope you get motivated and make a quality product, maybe get into esk8ing yourself
```

---
## \#68 Posted by: dareno Posted at: 2019-01-21T02:59:16.693Z Reads: 251

```
Are you still restricted to a certain number of replies?  This thread needs to keep going.
```

---
## \#69 Posted by: shaman Posted at: 2019-01-21T03:16:53.718Z Reads: 248

```
[quote="dareno, post:68, topic:81344, full:true"]
Are you still restricted to a certain number of replies? This thread needs to keep going.
[/quote]

I think I'm ok now. I'm a trust level 1 which doesn't advertise any reply restrictions. Before, I was level 0 which does have that limit I ran into.
```

---
## \#70 Posted by: shaman Posted at: 2019-01-21T03:20:24.955Z Reads: 250

```
https://endless-sphere.com/forums/viewtopic.php?f=7&t=97699&start=50

I've posted about my current progress in my sphere thread (see link). Sort of anti-climactic at the moment but it's something...
```

---
## \#71 Posted by: dareno Posted at: 2019-01-21T03:21:28.175Z Reads: 247

```
Bookmarked for progress and keep up the damn fine work sir!
```

---
## \#72 Posted by: shaman Posted at: 2019-01-21T03:23:29.971Z Reads: 244

```
[quote="dareno, post:71, topic:81344, full:true"]
Bookmarked for progress and keep up the damn fine work sir!
[/quote]

I appreciate that and I'll continue to do my best!
```

---
## \#73 Posted by: b264 Posted at: 2019-01-21T09:58:00.732Z Reads: 256

```
[quote="shaman, post:51, topic:81344"]
So I have several people interested in testing my controller between here and the sphere. I do need these testers so that I get good data form several different use cases. The problem is sourcing the amount controllers needed for the testers. There’s no way that I can make multiples of these controllers by hand during my spare time. Some testers may be able to solder the boards up themselves but that leaves plenty of opportunity for human error (just like in my own prototype so far). I’m considering having a PCB assembly service make some of these for me but I don’t have the cash to front for that. [https://www.7pcb.com/ ](https://www.7pcb.com/) quoted me about $600 for 15 boards. I have a couple of questions for this community…

Do you guys think it would be successful to have a gofundme or patreon or something like that to help with these kinds of things? If not, what would be the alternatives?
[/quote]

If I could make some suggestions, for testers---

* only one or two in sunny California
* at least one in each hemisphere
* one in a hot, sunny place
* multiple in a cold, snowy place
* one in NYC specifically

That way you can really test the product
```

---
## \#74 Posted by: Andy87 Posted at: 2019-01-21T10:23:35.101Z Reads: 249

```
[quote="b264, post:73, topic:81344"]
multiple in a cold, snowy place
[/quote]

@shaman I guess I would be the right person for it (living in Russia) ;)
Also with bigger motors like 8085 I could make some tests (if they don´t break befor :sweat_smile:)

@b264 why more tester in cold conditions than in warm?
Isn´t the heat production the bigger problem and wouldn´t it make more sense the other way round?
```

---
## \#75 Posted by: b264 Posted at: 2019-01-21T10:28:58.814Z Reads: 243

```
Sure.  I was just throwing out some suggestions so there aren't 17 testers, all in SoCal, and then they don't actually work in the real world :rofl:
```

---
## \#76 Posted by: pat.speed Posted at: 2019-01-21T10:42:42.184Z Reads: 235

```
Def need some in San Francisco, they got some thiccc hills to test on. Does @Hummie live there?
```

---
## \#77 Posted by: Hummie Posted at: 2019-01-21T16:31:52.255Z Reads: 235

```
I do. could it be made a cm thinner with maybe 3 shorter caps instead of the two long?  Would fit a lot more boards.  If ur still looking for people to try I will!   Happy to solder it.
```

---
## \#78 Posted by: banjaxxed Posted at: 2019-01-21T17:02:45.758Z Reads: 236

```
It would be nice to see a community ESC based on the VESC6 design, @fedestanco did this but in a limited release. Great advances could come out of branches of community design 

This is a really nice offering to students etc looking for value builds
```

---
## \#79 Posted by: Indiangummy Posted at: 2019-01-21T17:05:54.323Z Reads: 245

```
But vesc 6 is not open scource right? How would you be able to get the schematics?
```

---
## \#80 Posted by: moon Posted at: 2019-01-21T17:06:30.214Z Reads: 252

```
The schematics and BOM are available online
```

---
## \#81 Posted by: banjaxxed Posted at: 2019-01-21T17:07:45.454Z Reads: 252

```
@stewie, @fedestanco both created their own designs based on a released schematic. Flipsky and probably a couple of other vendors have gone the same
```

---
## \#82 Posted by: shaman Posted at: 2019-01-21T17:41:43.566Z Reads: 229

```
[quote="Hummie, post:77, topic:81344, full:true"]
I do. could it be made a cm thinner with maybe 3 shorter caps instead of the two long? Would fit a lot more boards. If ur still looking for people to try I will! Happy to solder it.
[/quote]


I don't think I can cut 1cm from any dimension here. I'm already going to switch to 2 680uF caps instead of the taller 1000uF so that it fits in the hammond enclosure properly.
```

---
## \#83 Posted by: Hummie Posted at: 2019-01-21T17:47:53.083Z Reads: 219

```
But can’t the caps simply be laid sideways and longer not taller?  A different heatsink? At 45mm tall that’s an obstacle for a lot of people fitting it in their board.
```

---
## \#84 Posted by: shaman Posted at: 2019-01-21T17:51:36.698Z Reads: 220

```
L92mm x W45mm x H23mm(approx). It's only going to be about 23mm tall as it is. I have considered the ability to lay the caps down over the board but I don't like that for some reason. It's a weird OCD or something.
```

---
## \#85 Posted by: Hummie Posted at: 2019-01-21T17:52:52.406Z Reads: 227

```
23mm. Sorry I’m wasting your time thought it was fatter!  Sounds great! I wrote u on endless sphere. Hope we can make something go in the future together.  Hope to get u the money u need.
```

---
## \#86 Posted by: shaman Posted at: 2019-01-21T17:54:34.573Z Reads: 229

```
[quote="Hummie, post:85, topic:81344, full:true"]
23mm. Sorry I’m wasting your time thought it was fatter! Sounds great! I wrote u on endless sphere. Hope we can make something go in the future together. Hope to get u the money u need.
[/quote]

Now worries! PM sent on the sphere btw.
```

---
## \#87 Posted by: shaman Posted at: 2019-01-23T22:24:19.017Z Reads: 233

```
Project Update

I've got good news and bad news.

Good news:
I got the software loaded up. I was able to see real time temperature and stuff. 

Bad news:
No spinning motors yet. I have a weird situation surrounding the USB and ST link connection. The VESC tool only maintains a connection when both the ST link AND the USB cable are plugged in. Removing one or the other causes the VESC tool to lose connection. Don't know if it's a software/driver issue or a hardware issue. Probably the latter. I can still probably spin a motor tomorrow even under this condition. Will have to eventually resolve this issue though.

I want to verify that the USB 5V power does not actually connect to anything on the VESC right?
```

---
## \#88 Posted by: AlexBE Posted at: 2019-01-23T23:02:31.674Z Reads: 213

```
Sounds like a GND problem. Ie your USB ground is not connected or something similar.
```

---
## \#89 Posted by: b264 Posted at: 2019-01-23T23:03:29.766Z Reads: 215

```
Yes, it sounds like ground is coming from one connection and power coming from the other connection.

Try putting a 9V battery on the VESC power wires to keep it on
```

---
## \#90 Posted by: shaman Posted at: 2019-01-24T00:34:45.660Z Reads: 216

```
To clarify, power has been coming from a separate bench top power supply straight to the main DC power input. I will still verify if the USB is grounded tomorrow. I'll fix that if it is. If not, more debugging to follow.
```

---
## \#91 Posted by: shaman Posted at: 2019-01-24T13:42:10.629Z Reads: 215

```
So the ground seems ok after doing continuity checks. I may try a different computer with a clean install of the STM drivers, bootloader, and vesc tool. I have a spare STM32 if comes down to swapping that out. I may not make much progress until next week as I'll be out of town starting today.
```

---
## \#92 Posted by: shaman Posted at: 2019-01-28T14:43:09.109Z Reads: 225

```
Just seems like a good ol fashioned "turn it off and back on again" did the trick. Now I've issues with the current sense part of the system. 

I get a weird "ghost current" reading from the Real Time data. It shows motor current at 0.35A when everything is idle and no motor is connected. My power supply doesn't register this much current being drawn. I believe there's something up with the current sense portion of the system. Could be a bad reference voltage or solder bridge somewhere. Could also be the DRV. I'll be troubleshooting this today and on into the week if need be.
```

---
## \#93 Posted by: shaman Posted at: 2019-01-29T13:21:22.214Z Reads: 232

```
So I went through an elaborate debug to try and fix the "ghost current" issue. Swapped out both the DRV and STM32 without much improvement. I did discover the TRUE reason why I was having the USB/STlink issue. Simply leaving the STlink connected to the VESC even without being plugged into the computer hijacks the reset pin. Must remove STlink completely after loading bootloader. 

Nothing I did resolved the "ghost current" and minute amount of duty cycle percentage that was being displayed. I found out that this seems like normal behavior of an idle VESC after viewing the video from the link below and other screen shots of people's VESC real time data. Real time data at 1:18 in the video is the same as mine showing approx. 0.3A and 0.1% duty cycle. 

Can anyone else confirm that this normal behavior? 

https://www.youtube.com/watch?v=UmlLNGOSL6w
```

---
## \#94 Posted by: shaman Posted at: 2019-01-29T15:57:51.307Z Reads: 234

```
So I made a mistake on the schematics. I accidentally mixed up the phase and current sense signals. I have SENS1 to H1_VS, SENS2 to H2_VS, and SENS3 to H3_VS. I have SH1_A and SH1_B measuring H1 current and SH2_A/B measuring H3 current.

The correct schematics have SENS1 to H3_VS, SENS2 to H2_VS, and SENS3 to H1_VS along with the current sense opposite of mine. 

It bothers me that I didn't catch this with as many hours I spent staring at the schematics of both my controller and the official VESC 4.12. I don't think this is contributing do the "ghost current" readings but we'll see.

Regardless, I'll have to do either a hardware fix by doing PCB surgery to swap the signals paths around or modify the firmware to accept the hardware configuration as is. Just know that is solvable and not project killing. Either way, I'm fixing my schematics and PCB design so that they align with the original VESC 4.12. I don't want people to have to upload custom firmware for my controller if it's not necessary.
```

---
## \#95 Posted by: moon Posted at: 2019-01-29T16:00:26.483Z Reads: 218

```
I'm not replying much because I can't help with stuff like this but I am reading every response :grin:
```

---
## \#96 Posted by: shaman Posted at: 2019-01-29T16:01:36.376Z Reads: 219

```
[quote="moon, post:95, topic:81344"]
I’m not replying much because I can’t help with stuff like this but I am reading every response :grin:
[/quote]

No worries. I'm glad people are still interested enough to read!
```

---
## \#97 Posted by: Benjamin899 Posted at: 2019-01-29T16:07:18.330Z Reads: 212

```
second that
```

---
## \#98 Posted by: Andy87 Posted at: 2019-01-29T18:00:25.451Z Reads: 211

```
@moon is not the only one 😉
Please keep updating us. Even if we can’t help much it’s very interesting to follow your progress 👍
```

---
## \#99 Posted by: shaman Posted at: 2019-01-29T18:08:11.311Z Reads: 215

```
[quote="Andy87, post:98, topic:81344"]
@moon is not the only one :wink:
Please keep updating us. Even if we can’t help much it’s very interesting to follow your progress :+1:
[/quote]

No problem! Will do!
```

---
## \#100 Posted by: linsus Posted at: 2019-01-29T19:20:40.467Z Reads: 213

```
aaaaand this is why the review is done by someone else then the creator 9/10 times :D (but you know this ;) )
```

---
## \#101 Posted by: shaman Posted at: 2019-01-29T21:52:16.012Z Reads: 214

```
You got me there! :grin:
```

---
## \#102 Posted by: mynamesmatt Posted at: 2019-01-29T21:59:50.184Z Reads: 221

```
[quote="b264, post:73, topic:81344"]
one in a hot, sunny place
[/quote]

get me one down here in Sydney Australia! Tomorrows forecast is:
![Screenshot_20190130-085910_Google|690x262](upload://70NYoDjVinwnjn9c12WVFIxCQQN.jpeg)
it gets bloody hot here. dunno why my focboxs don't overheat lol
```

---
## \#103 Posted by: shaman Posted at: 2019-01-30T14:21:53.503Z Reads: 218

```
So there's a lot of .c and .h files associated with the VESC firmware and I'm too inexperienced with it all to try and find every little variable that I need to change to accommodate my hardware mistakes. I'm gunna try the PCB surgery route but I'll to wait until I'm back at the lab where I can use a dissection scope. These are tiny little traces and things would get sloppy without magnification.
```

---
## \#104 Posted by: Ackmaniac Posted at: 2019-01-30T14:32:28.264Z Reads: 217

```
I guess you have to change the hwconf\hw_410.h file and change

    #define ADC_IND_SENS1   2
    #define ADC_IND_SENS2   1
    #define ADC_IND_SENS3   0 

to

    #define ADC_IND_SENS1   0
    #define ADC_IND_SENS2   1
    #define ADC_IND_SENS3   2
```

---
## \#105 Posted by: rey8801 Posted at: 2019-01-30T14:40:16.480Z Reads: 205

```
@shaman same here. Super interested, but lacking of knowledge :sweat_smile:
You are not alone. We are all watching you! :laughing:
```

---
## \#106 Posted by: shaman Posted at: 2019-01-30T15:31:03.571Z Reads: 197

```
@Ackmaniac

Supposedly that's all I would have to do for FOC functionality. However, supposedly there are more things to adjust for BLDC operation and motor parameter detection.
```

---
## \#107 Posted by: Ackmaniac Posted at: 2019-01-30T16:56:03.552Z Reads: 194

```
If all your hardware is based on the 4.12 layout and that was the only difference then this change should be all you need. Just simply give it a try.
Or did you already use another DRV or anything else?
```

---
## \#108 Posted by: shaman Posted at: 2019-01-30T17:18:10.162Z Reads: 197

```
Nah it's the same DRV and such from 4.12. The reason I'm hesitant on the firmware is that I've read where there's more to it that just those values you have mentioned. The thread from the link below addresses my situation but just from a different 4.12 VESC variant. The original poster never followed up so idk if the issues were resolved. Also, I also have anxiety about screwing up the firmware and blowing up my controller. 

https://vesc-project.com/node/363
```

---
## \#109 Posted by: b264 Posted at: 2019-01-30T17:23:54.316Z Reads: 191

```
I'd also be worried that if yours is a VESC derivative on the market, most folks would assume it will run standard firmware and not need a recompilation with 3 changed variables, could cause operator-error situations....
```

---
## \#110 Posted by: shaman Posted at: 2019-01-30T17:27:53.338Z Reads: 200

```
[quote="b264, post:109, topic:81344, full:true"]
I’d also be worried that if yours is a VESC derivative on the market, most folks would assume it will run standard firmware and not need a recompilation with 3 changed variables, could cause operator-error situations…
[/quote]

This "mix up" of mine will absolutely be corrected in the PCB design and schematics. The controllers for testers will not have this issue and neither will the final release. Folks will be able to use the standard firmware for the 4.12 hardware once its all said and done.
```

---
## \#111 Posted by: ZachTetra Posted at: 2019-01-30T17:36:42.856Z Reads: 191

```
So aside from the asthetics and price tag, these will be the same as every other VESC derivatives?
```

---
## \#112 Posted by: moon Posted at: 2019-01-30T17:41:05.843Z Reads: 198

```
https://www.ebay.co.uk/itm/Aluminium-DieCast-POWDER-COATED-Hammond-STYLE-Enclosure-StompBox-ALL-SIZES/254082202609?hash=item3b287abbf1:m:mgJVN23iJyYN0-8AJ5EloeQ:rk:3:pf:0

This + engraving :ok_hand::ok_hand:
```

---
## \#113 Posted by: Ackmaniac Posted at: 2019-01-30T17:46:13.591Z Reads: 189

```
In your case it should be fine. Simply set like 3A for motor max and battery max to keep currents low if something goes wrong, And i hope you will switch in the future to DRV with higher voltage. I like the idea of a cheap high voltage VESC for ebikes which don't need crazy high amps.
```

---
## \#114 Posted by: b264 Posted at: 2019-01-30T17:59:49.974Z Reads: 195

```
[quote="ZachTetra, post:111, topic:81344, full:true"]
So aside from the asthetics and price tag, these will be the same as every other VESC derivatives?
[/quote]

This is a lot different from other ones.  It's not as small and easier to construct and far easier to attach heatsinks to.  If you can solder one DRV8302, you could handmake this entire thing.  And who knows if a vendor will sell the boards with the DRV and MCU presoldered
```

---
## \#115 Posted by: ZachTetra Posted at: 2019-01-30T18:06:13.152Z Reads: 192

```
I mean in terms of use...same ports same software same ability to run a motor?
```

---
## \#116 Posted by: Andy87 Posted at: 2019-01-30T18:08:37.296Z Reads: 191

```
Pro tip: it helps to read all comments in the thread 😉
```

---
## \#117 Posted by: shaman Posted at: 2019-01-30T18:19:18.789Z Reads: 190

```
I may take a crack at the firmware. Gotta set up an Ubuntu VM. Yes I will be utilizing the DRV8353R for the high voltage version. Up to 20s battery.
```

---
## \#118 Posted by: b264 Posted at: 2019-01-30T18:21:18.168Z Reads: 202

```
Virtualbox 5.2.24 has a bug and Ubuntu 18 does not work.  Use VirtualBox 5.2.22 and "Ubuntu Server" 18 -- then after it's installed, run

[quote]
sudo apt-get update
sudo apt-get upgrade
sudo apt-get dist-upgrade
sudo apt-get install ubuntu-desktop
sudo init 6
[/quote]

And you're good to go
```

---
## \#119 Posted by: shaman Posted at: 2019-01-30T18:21:54.390Z Reads: 191

```
Sweet. Thanks b264.
```

---
## \#120 Posted by: Ackmaniac Posted at: 2019-01-30T18:35:21.502Z Reads: 199

```
I just created the firmware file for you. check your PM's.
```

---
## \#121 Posted by: moon Posted at: 2019-01-30T21:16:51.463Z Reads: 194

```
@shaman

Found out that I have access to a reflow oven. That's good 😁
```

---
## \#122 Posted by: shaman Posted at: 2019-01-30T21:20:47.736Z Reads: 180

```
That makes soldering SMD quick and easy!
```

---
## \#123 Posted by: moon Posted at: 2019-01-30T21:27:24.071Z Reads: 180

```
Yeah can help once you get going
```

---
## \#124 Posted by: shaman Posted at: 2019-01-31T00:20:16.276Z Reads: 187

```
I got good news guys!

So I implemented the firmware alterations as suggested by @Ackmaniac plus a few more. I was able to do both FOC and BLDC calibrations and spin the motor with both methods! Still trying to figure out the sampling settings in the VESC Tool though. I wanna see those sinusoidal phase currents. 

Thanks @Ackmaniac for the compiled firmware!

Thanks @b264 for the Ubuntu set up instructions! I was able to adjust a couple of more things in the firmware in the VirtualBox.

So the next thing I'll do is get scope shots of the switch nodes. I need to see if there's any bad ringing and voltage spikes. Those spikes will kill the DRV if it's too intense.
```

---
## \#125 Posted by: b264 Posted at: 2019-01-31T00:28:46.701Z Reads: 178

```
[quote="shaman, post:124, topic:81344"]
So the next thing I’ll do is get scope shots of the switch nodes. I need to see if there’s any bad ringing and voltage spikes. Those spikes will kill the DRV if it’s too intense.
[/quote]

I'd absolutely love to see those on a scope with 42.0V power versus with 50.4V power

Under load and not under load if it's possible
```

---
## \#126 Posted by: shaman Posted at: 2019-01-31T00:37:36.942Z Reads: 177

```
Sure! But loaded tests may not be for another week or so. There's a bit of setup involved with the dyno and power supply that's gunna be used for all that.
```

---
## \#127 Posted by: shaman Posted at: 2019-01-31T15:42:38.168Z Reads: 191

```
So while we wait for me to make more progress, let's discuss preferred connectors for the battery, phase cables, throttle, and hall effect sensors. I will probably ship the test controllers with cables and connectors if enough people agree on the same thing.

For the battery connector I see XT60 or XT90 being commonly used with success. I'll most likely go with these unless someone suggests something better.

For phase cables, I've personally used the [MT60 connectors](https://hobbyking.com/en_us/mt60-3-pole-motor-esc-connector-set-12awg-male-female-2-set.html). They're like a triple connector version of the XT60. You can use up to 12awg wire with them. They look kinda cool and I can ship the other end of the connector as well to be attached to your motor phases. Would the community accept these or prefer something else like bullet connectors?

For the analog throttle and hall effect sensors I was thinking just some generic 3 pin and 5 pin connectors. This would most likely apply more to ebikes since analog throttles and sensored motors do not seem to be as common in the esk8 world.

Let me know what you guys think!
```

---
## \#128 Posted by: Indiangummy Posted at: 2019-01-31T16:11:13.803Z Reads: 179

```
For motors I would say 5.5 mm bullet connectors are the most common. If we wanted to use mt60 we would have to change the connectors on the motor. Not a big deal. For remote, a servo connector is most common.
```

---
## \#129 Posted by: J_Dizzle Posted at: 2019-01-31T16:11:22.036Z Reads: 174

```
For the phase wires 4mm bullet connectors would be good, because that is the connector on most motors sold on here like Torqueboards and bkb.
```

---
## \#130 Posted by: Andy87 Posted at: 2019-01-31T16:11:25.749Z Reads: 176

```
Xt60 and xt90 as main power are both perfect.
Personally i like xt90 more but people with less space will prefer xt60.
Most our outrunner motors come with 5.5mm bullet connectors, so for me that would be preferred.
Sonsor connectors are usually 2mm 6pin jst ph
```

---
## \#131 Posted by: Andy87 Posted at: 2019-01-31T16:13:02.794Z Reads: 184

```
Torque boards has 5.5mm too
https:///collections/featured-items/products/electric-skateboard-motor-6355-190kv

Bkb has 4mm
But 
Aps 5.5mm
Maytech and most rebranded maytechs 5.5mm
Too
```

---
## \#132 Posted by: Andy87 Posted at: 2019-01-31T16:20:30.274Z Reads: 188

```
@shaman lot of motors come with a 1.5 6pin jst zh for sensor wires, but most time this wires anyhow to short and people need an adapter cable which is sold here like this 
 https://eskating.eu/product/sensors-adapter-jst-2-0mm-6-pins/

If you have a look at other vesc designs it’s common to use 2mm jst for CAN port, hall sensor port, uart port and ppm port.

On the focbox the ppm cable was already soldered on the pcb with a connector for rc radio receiver.

![image|690x425](upload://5Wce9m9f9XjmSNWhx2hjAqGSjpy.jpeg)
```

---
## \#133 Posted by: moon Posted at: 2019-01-31T17:09:28.673Z Reads: 177

```
I don't know, why not leave them empty, without connectors
```

---
## \#134 Posted by: shaman Posted at: 2019-01-31T17:11:41.885Z Reads: 174

```
Its an option but I was wanting to make the controller as ready as possible for people.
```

---
## \#135 Posted by: mishrasubhransu Posted at: 2019-01-31T17:24:34.681Z Reads: 175

```
I use those connectors. They are awesome: strong and less mess.
```

---
## \#136 Posted by: moon Posted at: 2019-01-31T17:25:31.948Z Reads: 181

```
[quote="shaman, post:127, topic:81344"]
sensored motors do not seem to be as common in the esk8 world.
[/quote]

most motors are sensored :)
```

---
## \#137 Posted by: shaman Posted at: 2019-01-31T17:40:32.033Z Reads: 176

```
I stand corrected!
```

---
## \#138 Posted by: Ackmaniac Posted at: 2019-01-31T19:09:16.387Z Reads: 176

```
What are your plans? You want to make a business out of it or release all the design files and BOM so that people can buy the kit themself?
I thought you just do it for science so that everybody can build his cheap VESC himself afterwards. But when you talk about connectors then it sounds like you like to sell them.
```

---
## \#139 Posted by: mishrasubhransu Posted at: 2019-01-31T19:11:43.770Z Reads: 174

```
He might mean what connectors to use for the test batch.
```

---
## \#140 Posted by: shaman Posted at: 2019-01-31T19:17:12.431Z Reads: 190

```
[quote="Ackmaniac, post:138, topic:81344, full:true"]
What are your plans? You want to make a business out of it or release all the design files and BOM so that people can buy the kit themself?
I thought you just do it for science so that everybody can build his cheap VESC himself afterwards. But when you talk about connectors then it sounds like you like to sell them.
[/quote]

Yes of course I intend to release all the design files and BOM! The connector questions is primarily for the test controllers for the test volunteers. I want those set up nice for them. 

But now that you mention it, if I released the design as open source but still sold pre-made ones on the side, does that make me a bad person? I figure the option is there for those that want to DIY but why not sell some completely assembled controllers to those that just want instant gratification?
```

---
## \#141 Posted by: moon Posted at: 2019-01-31T19:19:41.455Z Reads: 189

```
[quote="shaman, post:140, topic:81344"]
But now that you mention it, if I released the design as open source but still sold pre-made ones on the side, does that make me a bad person? I figure the option is there for those that want to DIY but why not sell some completely assembled controllers to those that just want instant gratification?
[/quote]

That makes you a good person :ok_hand:

Some people don't have time to go through all of that hard work :slight_smile:

When there's an option to buy and an option to build everyone is happy
```

---
## \#142 Posted by: shaman Posted at: 2019-01-31T19:20:44.971Z Reads: 175

```
Thank you @moon!
```

---
## \#143 Posted by: Ackmaniac Posted at: 2019-01-31T19:23:42.493Z Reads: 173

```
To do both is totally fine. Even to only sell is totally fine. Only difference is that people who support the project mostly only like to support open community projects.

Maybe a really nice and cheap idea would be to sell the boards with the Chip, DRV and maybe USB connector presoldered and preprogrammed (small parts that are hard to solder but easy to do with a reflow oven) and all other parts are added as a kit that can be soldered then by everybody themself. 
This way it's a nice little project and you safe a lot of time when you don't need to place all the small components yourself.
```

---
## \#144 Posted by: shaman Posted at: 2019-01-31T19:26:56.782Z Reads: 172

```
I like the DIY kit idea! Cuts out most of the cost of assembly. I could even sell just the bare boards to more "advanced" DIYers since those tend to cost the most in low quantity.
```

---
## \#145 Posted by: Andy87 Posted at: 2019-01-31T19:27:56.675Z Reads: 169

```
I don’t have the tools and the skills to assemble one by my own.
I would be very happy if you sell some pre assembled 😌
```

---
## \#146 Posted by: Ackmaniac Posted at: 2019-01-31T19:30:07.015Z Reads: 174

```
if you finally have a 2 layer board they will be 50 cent each plus a bit shipping if you buy at JLCPCB.com even at low quantity.

Just make wide tracks that are not covered by silk so that they can be reinforced with more solder manually.
```

---
## \#147 Posted by: Hummie Posted at: 2019-01-31T19:32:21.922Z Reads: 171

```
When u do get it all figured out maybe make a website or something so we can get info better than trying to read long threads digging.
```

---
## \#148 Posted by: ZachTetra Posted at: 2019-01-31T19:32:28.658Z Reads: 171

```
How hard is it to make the mostfets externally mounted?  Leave holes where wires to them go so the ESC can be in a nice hard case and the hottest elements can be in an external heat sink on the  bottom of the board in a nice easy row?

I feel that would be good for some DIY cooling solutions
```

---
## \#149 Posted by: shaman Posted at: 2019-01-31T19:35:53.894Z Reads: 172

```
This is exactly what I've already done for my prototype I'm currently testing!
```

---
## \#150 Posted by: shaman Posted at: 2019-01-31T19:40:42.287Z Reads: 176

```
[quote="Hummie, post:147, topic:81344, full:true"]
When u do get it all figured out maybe make a website or something so we can get info better than trying to read long threads digging.
[/quote]

Sure! I'll also consolidate a lot of the information on my controller in the github repository.
```

---
## \#151 Posted by: shaman Posted at: 2019-01-31T19:44:40.039Z Reads: 179

```
[quote="Ackmaniac, post:146, topic:81344"]
if you finally have a 2 layer board they will be 50 cent each plus a bit shipping if you buy at [JLCPCB.com](http://JLCPCB.com) even at low quantity.

Just make wide tracks that are not covered by silk so that they can be reinforced with more solder manually.
[/quote]

One still has to buy 10 at a time that will total out to $17ish USD. Yes the cost per board is really cheap but you still gotta pay for all 10 and that's not very useful for someone that just wants to build a single controller. I could provide individual boards for much less than $17 USD for those that just want to build one or two.

yeah I totally went with the manual track beefing technique. Check out my thread on the endless sphere. It's got pics of my assembled board!
```

---
## \#152 Posted by: b264 Posted at: 2019-01-31T19:45:50.822Z Reads: 168

```
[quote="shaman, post:140, topic:81344"]
released the design as open source but still sold pre-made ones on the side
[/quote]

That's the best of all the options :slight_smile:
```

---
## \#153 Posted by: shaman Posted at: 2019-01-31T19:46:49.991Z Reads: 174

```
[quote="ZachTetra, post:148, topic:81344, full:true"]
How hard is it to make the mostfets externally mounted? Leave holes where wires to them go so the ESC can be in a nice hard case and the hottest elements can be in an external heat sink on the bottom of the board in a nice easy row?

I feel that would be good for some DIY cooling solutions
[/quote]

The plan is to already thermally couple the mosfet heatsink to the aluminum hammond enclosure from the inside. This will have very good heatsinking while maintaining a sealed enclosure.
```

---
## \#154 Posted by: b264 Posted at: 2019-01-31T19:47:02.646Z Reads: 182

```
[quote="Ackmaniac, post:143, topic:81344"]
Maybe a really nice and cheap idea would be to sell the boards with the Chip, DRV and maybe USB connector presoldered and preprogrammed (small parts that are hard to solder but easy to do with a reflow oven) and all other parts are added as a kit that can be soldered then by everybody themself.
This way it’s a nice little project and you safe a lot of time when you don’t need to place all the small components yourself.
[/quote]

Yes I agree, if you sell the board with MCU and DRV and USB presoldered it will be an instant success story.  And with bootloader already on the MCU
```

---
## \#155 Posted by: moon Posted at: 2019-01-31T19:47:30.110Z Reads: 171

```
Dont forget the last part :sweat_smile:
```

---
## \#156 Posted by: rey8801 Posted at: 2019-01-31T20:04:10.455Z Reads: 179

```
@shaman just a noob question. Probably being already covered but you clearly know what you are doing. What limit a vesc to the 12s or the 69V limit? Is it the DRV only or something else too? Because I do not se the point where everyone use the same DRV limited to 60V if thst is the bottle enck of the whole pcb. Is it due to the price of the higher voltage ones? Thx and sorry for the off topic... :grin:
```

---
## \#157 Posted by: janpom Posted at: 2019-01-31T20:43:06.692Z Reads: 185

```
The DIY kit sounds awesome! I have always wanted to assemble an ESC by myself. :smiley:
```

---
## \#158 Posted by: moon Posted at: 2019-01-31T20:48:54.596Z Reads: 193

```
![image|666x500](upload://xPjh8rgapEv1yoiSwzTGY9dx7eP.jpeg) 
![image|690x377](upload://p9XubBkr6IaLdKJVvkrG2Y7I8Tp.jpeg)
![image|690x164](upload://czWzuRCFzAenzxuiZZGAl666LBf.jpeg) 
![image|666x500](upload://qO20Bwj4px2UHgWywxZp8qHMaMp.jpeg) 

pics from es
```

---
## \#159 Posted by: shaman Posted at: 2019-01-31T22:02:49.133Z Reads: 189

```
[quote="rey8801, post:156, topic:81344"]
@shaman just a noob question. Probably being already covered but you clearly know what you are doing. What limit a vesc to the 12s or the 69V limit? Is it the DRV only or something else too? Because I do not se the point where everyone use the same DRV limited to 60V if thst is the bottle enck of the whole pcb. Is it due to the price of the higher voltage ones? Thx and sorry for the off topic… :grin:
[/quote]

Yes the 60V limit is due to the DRV8302 indeed. Its max operating voltage as stated by the datasheet is 60V. The DRV8301 used in the VESC 6 has the same limitation. The rest of the control circuitry in the VESC operates off of the 5V or 3.3V votlage rails. Until recently, this was the best TI could do for a "high" voltage motor driver. Now there is the new DRV8353 which can go up to 100V. That's the one I'm using for the high voltage VESC design.

Note that one can design out the DRV entirely and just use individual gate drivers for every set of 2 MOSFETs. A few designers are doing that right now for really high powered VESC based motor controllers.
```

---
## \#160 Posted by: rey8801 Posted at: 2019-01-31T22:09:21.172Z Reads: 183

```
Thanks, got it! Just to know, which is the price different between let's say DRV8302 to DRV8353? Because you BOM is really low, maybe is possible with the double to make a 100V one. I am not trying to change your plans, it's just out of curiosity.
```

---
## \#161 Posted by: shaman Posted at: 2019-01-31T22:15:20.697Z Reads: 177

```
The price difference is about $0.50 USD in the 1000 unit price. It won't cause the BOM to double in price by any means. Also don't forget that anyone can about 5 free sample of most ICs from TI simply by making an account on TI.com. From a DIY perspective, that keeps the BOM cheap!
```

---
## \#162 Posted by: shaman Posted at: 2019-01-31T22:20:09.388Z Reads: 185

```
[quote="b264, post:154, topic:81344"]
Yes I agree, if you sell the board with MCU and DRV and USB presoldered it will be an instant success story. And with bootloader already on the MCU
[/quote]

I'm seriously going to consider this approach. Maybe I can finally get an LLC going and start feeding the DIY community cool stuff. All open source of course!
```

---
## \#163 Posted by: moon Posted at: 2019-01-31T22:21:22.192Z Reads: 179

```
I want to make some cases or cnc heatsinks for this for sure :)

Theres not enough community projects here
```

---
## \#164 Posted by: rey8801 Posted at: 2019-01-31T22:21:53.126Z Reads: 178

```
:star_struck: Then I will patiently waiting for second generation "100Vesc"
```

---
## \#165 Posted by: shaman Posted at: 2019-01-31T22:24:57.968Z Reads: 178

```
Not to bring you down, but just a caveat. Yes 100V is the max but I wouldn't push it that high. Always leave room in the design for transients/spikes so you're not constantly riding the line between working and broken. I am advertising the high voltage design to operate up to 84V(20s).
```

---
## \#166 Posted by: rey8801 Posted at: 2019-01-31T22:25:48.513Z Reads: 175

```
Sure, I want it to have a reliable 12-14s max
```

---
## \#167 Posted by: b264 Posted at: 2019-01-31T22:38:35.595Z Reads: 182

```
[quote="shaman, post:165, topic:81344"]
Always leave room in the design for transients/spikes so you’re not constantly riding the line between working and broken.
[/quote]

Good luck with that :smirk:  everyone here wants to push it as far as they can.  I prefer to know the thing that holds my life in its hands is not operating at max voltage while feeding square waves into inductors....

I will only run the DRV8302 at 42V but mostly folks here push it to 50.4V and some even 54.6V
```

---
## \#168 Posted by: shaman Posted at: 2019-01-31T23:21:12.352Z Reads: 174

```
I'm sure I can come up with some fancy disclaimer. Something like...
"Do not FOC the Cheap FOCer outside of it's advertised FOCing limits. You risk damaging yourself, the controller and your ability to FOC any further."
```

---
## \#169 Posted by: Indiangummy Posted at: 2019-01-31T23:25:36.500Z Reads: 173

```
[quote="shaman, post:168, topic:81344"]
“Do not FOC the Cheap FOCer outside of it’s advertised FOCing limits. You risk damaging yourself, the controller and your ability to FOC any further.”
[/quote]

it think that wins the best caption of 2019.
```

---
## \#170 Posted by: shaman Posted at: 2019-02-01T11:29:56.245Z Reads: 174

```
[quote="b264, post:154, topic:81344"]
Yes I agree, if you sell the board with MCU and DRV and USB presoldered it will be an instant success story. And with bootloader already on the MCU
[/quote]

So I was thinking of switching to a vertical mounted mini USB port. These are through-hole components and should be easy to solder by hand. The orientation would also grant easier access to the USB port while the Cheap FOCer is in an enclosure like the hammond 1590b. The only downside is that LCSC is out of stock on those and idk for how long. I was hoping to be able to pitch a BOM to everyone that is 100% from LCSC.
```

---
## \#171 Posted by: shaman Posted at: 2019-02-01T15:19:38.831Z Reads: 169

```
That would be cool! Would you utilize the hammond enclosures or go with something else?
```

---
## \#172 Posted by: Andy87 Posted at: 2019-02-01T15:21:51.027Z Reads: 171

```
I‘m sure he will design something totally new 😜
@moon a dual heat sink case would be great 👍
```

---
## \#173 Posted by: moon Posted at: 2019-02-01T17:39:09.524Z Reads: 172

```
We can do both. But we can also have a custom heatsink...
```

---
## \#174 Posted by: deucesdown Posted at: 2019-02-03T16:22:30.561Z Reads: 177

```
[quote="Hummie, post:147, topic:81344, full:true"]
When u do get it all figured out maybe make a website or something so we can get info better than trying to read long threads digging.
[/quote]

Lol how dare you, of all people! ;)

[quote="b264, post:167, topic:81344"]
everyone here wants to push it as far as they can.
[/quote]

I believe 60vdc through the fingertips is where it starts to get very dangerous for humans. I'm pretty close to my personal limits with with 13-14s.
```

---
## \#175 Posted by: deucesdown Posted at: 2019-02-03T16:34:53.186Z Reads: 172

```
@shaman can I make 1 request? The canbus implementation on 4.xx hardware doesn't have adequate protection. If 2 vesc are connected, they must be powered on and off at the same time, and cannot be disconnected when they are on.

6.xx hardware, and I think the most recent version of FOCBOX has improved the canbus protections. It would be _great_ if you could cherrypick this improvement. Sorry, I'm not smart enough to have any specific details.

But this issue has fried many vescs. Personally, despite being aware of the issue, I had a xt60 disconnect on a vesc and lost 2 vesc (it's on my todo list to repair).
```

---
## \#176 Posted by: shaman Posted at: 2019-02-03T16:36:19.844Z Reads: 166

```
I got the 6.4 schematics in front of me right now. Let me see what going on with CAN stuff.
```

---
## \#177 Posted by: shaman Posted at: 2019-02-03T16:54:33.496Z Reads: 181

```
So the VESC 6.4 uses an automotive grade CAN transceiver. It can handle a lot more abuse from transients and such. The CAN transceiver from 4.12 is an older TI transceiver that is lower-class industrial grade.

There is a TI drop-in replacement I can use to replace the old transceiver. It's the TCAN1042-Q1. It's automotive grade as well and should be able to handle the abuse just fine. Note that this will have to be proven as a fix by conducting the procedures mentioned that would kill older VESCs.

I'll change the BOM to use the TCAN1042-Q1. I might be able to also add a spot for a TVS diode on the bus lines that would further help protect the system from spikes.
```

---
## \#178 Posted by: Hummie Posted at: 2019-02-03T17:34:43.970Z Reads: 175

```
[quote="deucesdown, post:175, topic:81344"]
But this issue has fried many vescs. Personally, despite being aware of the issue, I had a xt60 disconnect on a vesc and lost 2 vesc (it’s on my todo list to repair).
[/quote]

What’s the danger?!
```

---
## \#179 Posted by: deucesdown Posted at: 2019-02-03T17:44:21.690Z Reads: 181

```
[quote="Hummie, post:178, topic:81344"]
What’s the danger?!
[/quote]

I'm riding dual vesc 4.12, canbus connected. The xt60 to the battery slipped off on one vesc, and boom, hot canbus chips, no startup. Disconnected canbus, one vesc won't turn on, hot canbus chip. The other turns on with hot canbus chip, worked with split ppm, but stopped turning on a few days later.

the xt60 that slipped off was under zero tension, very surprised. Now I make sure the bananas are tight, or tape or zip tie them together...
```

---
## \#180 Posted by: shaman Posted at: 2019-02-03T18:35:32.654Z Reads: 176

```
You may be able to restore single motor function by removing the CAN transceiver from your broken VESCs. It could be that it's shorted on the inside and drawing too much current from the 3.3V regulator causing the STM to brownout.
```

---
## \#181 Posted by: deucesdown Posted at: 2019-02-03T18:45:28.285Z Reads: 179

```
Yah I have canbus chips in. Repair is on the long todo list. :slight_smile:
```

---
## \#182 Posted by: b264 Posted at: 2019-02-03T19:23:37.098Z Reads: 171

```
[quote="Hummie, post:178, topic:81344"]
What’s the danger?!
[/quote]

None -- if you run dual-independent with 2 receivers and no CANBUS and no "split PPM"
```

---
## \#183 Posted by: deucesdown Posted at: 2019-02-04T00:29:42.562Z Reads: 166

```
[quote="b264, post:182, topic:81344"]
run dual-independent with 2 receivers and no CANBUS and no “split PPM”
[/quote]

An example of things we're driven to for self-preservation, giving up remote configuration, telemetry, etc. :)
```

---
## \#184 Posted by: ZachTetra Posted at: 2019-02-04T00:32:10.970Z Reads: 165

```
How is using 2 different controllers any better than split ppm?
```

---
## \#185 Posted by: b264 Posted at: 2019-02-04T03:40:49.223Z Reads: 160

```
Because if one ESC fails, the other one still has brakes
```

---
## \#186 Posted by: tony74 Posted at: 2019-02-04T06:48:36.060Z Reads: 173

```
How about the ChESC?
```

---
## \#187 Posted by: Excess Posted at: 2019-02-04T07:15:04.830Z Reads: 175

```
Quote from deodand about the hardware change from focbox 1.6 to 1.7 that apparently mitigates the canbus issue. 

“we switched the CAN bus transceiver IC to an isolated one. Basically prevents the CAN transceiver from blowing things up unintentionally.”
```

---
## \#188 Posted by: shaman Posted at: 2019-02-04T13:37:16.226Z Reads: 177

```
An isolated CAN transceiver would be the most robust solution. There is an isolated version of the TCAN1042-Q1 called the ISO1042-Q1. I'm not sure if isolation is truly needed if the VESC 6 doesn't display negative qualities with CAN utilizing a non-isolated transceiver.
```

---
## \#189 Posted by: taz Posted at: 2019-02-04T14:18:23.285Z Reads: 177

```
Since I can't bail on my mountainboard due to the bindings I figured it would be a good solution.
So I tried deactivating traction control to see if I could live without it before making any changes.
Nope, impossible to ride an MTB on loose terrain without traction control, so CAN bus it is.
However I really like the redundancy of dual receivers for a commuting board.
```

---
## \#190 Posted by: Livid Posted at: 2019-02-04T14:34:28.041Z Reads: 172

```
60v is fine, just make sure you have good life insurance before you start playing. I put 240vac through my hand 10 years ago, still got the scars hehe
```

---
## \#191 Posted by: sayekim Posted at: 2019-02-04T15:37:13.037Z Reads: 171

```
Good life insurance doesn’t really help him now does it.
```

---
## \#192 Posted by: linsus Posted at: 2019-02-04T15:38:46.271Z Reads: 176

```
Bru, you never played super mario? Respawn try again.
```

---
## \#193 Posted by: deucesdown Posted at: 2019-02-04T15:39:12.708Z Reads: 190

```
Reposting this video. Love it! I'll stay under 60v :)

https://www.youtube.com/watch?v=PH28BId6BuM
```

---
## \#194 Posted by: shaman Posted at: 2019-02-04T19:30:27.943Z Reads: 193

```
![Cheap%20FOCer%20angled|690x404](upload://9P5bJhd7lccHltn0jlvPv4tRr65.jpeg) 

Here is an updated rendering with most of the changes and fixes so far put into place.

* Shorter 680uF caps to reduce overall height

* Vertical Mini USB for easier access and soldering

* Signal path fixes for Phase voltage and Current sense

* Widened holes for phase lines and battery cables

* Minor layout and routing improvements for the gate driver and gate traces
```

---
## \#195 Posted by: b264 Posted at: 2019-02-04T19:41:07.781Z Reads: 185

```
[quote="shaman, post:194, topic:81344"]
Widened holes for phase lines and battery cables
[/quote]

Do these hold 10AWG super-stranded?
```

---
## \#196 Posted by: b264 Posted at: 2019-02-04T19:42:10.591Z Reads: 187

```
After accidentally ripping off two USB jacks now, I have to ask --

What's the chance of using a through-hole USB jack?  Or is that one through-hole?
```

---
## \#197 Posted by: telnoi Posted at: 2019-02-04T19:58:41.332Z Reads: 184

```
That big a difference? Never tried it, so don't miss it.
```

---
## \#198 Posted by: shaman Posted at: 2019-02-04T20:01:45.811Z Reads: 189

```


[quote="b264, post:196, topic:81344, full:true"]
After accidentally ripping off two USB jacks now, I have to ask –

What’s the chance of using a through-hole USB jack? Or is that one through-hole?
[/quote]

The vertical Mini USB receptacle is indeed through-hole.

https://www.te.com/usa-en/product-1734753-1.html
```

---
## \#199 Posted by: shaman Posted at: 2019-02-04T20:04:12.416Z Reads: 188

```
[quote="b264, post:195, topic:81344"]
Do these hold 10AWG super-stranded?
[/quote]

It should. It might be close but the holes are 2.8mm in diameter and 10awg is approx. 2.6mm in diameter.
```

---
## \#200 Posted by: Pedrodemio Posted at: 2019-02-04T21:08:59.969Z Reads: 182

```
Are you sure of that? I can measure later, but the 12 AWG that I have in my hand is almost 3mm
```

---
## \#201 Posted by: moon Posted at: 2019-02-04T21:13:09.420Z Reads: 182

```
2.8mm 10awg. I have just measured it - the copper part
```

---
## \#202 Posted by: taz Posted at: 2019-02-04T21:14:19.333Z Reads: 180

```
Without traction control one wheel would spin on loose gravel etc and I would go nowhere.
Traction control greatly improved grip.
On tarmac though I don't think it is needed.
```

---
## \#203 Posted by: b264 Posted at: 2019-02-04T21:15:05.797Z Reads: 177

```
With two separate motors, even if one starts spinning, the other one still has power.  It's not like a differential in a car.
```

---
## \#204 Posted by: taz Posted at: 2019-02-04T21:16:21.231Z Reads: 178

```
Yes, however if one starts spinning then the other also loses traction on loose terrain.
```

---
## \#205 Posted by: b264 Posted at: 2019-02-04T21:19:30.328Z Reads: 174

```
That's likely due to the fact that the terrain under the other wheel is similar terrain, based on the proximity of the two wheels to each other.  It could be caused by a lower speed, which is a result of the other wheel spinning.  But it is not a direct result of the other wheel spinning.
```

---
## \#206 Posted by: taz Posted at: 2019-02-04T21:31:26.204Z Reads: 172

```
Direct or indirect is beside the point.
When one wheel starts spinning you rely on the other to propel you forward.
However on low traction situations one wheel simply is not enough and also starts spinning.
Traction control prevents the first wheel from breaking traction by lowering the current that goes to the motor that spins faster.
You don't have to take my word for it. Find a really steep gravel road and do tests with your mtb with and without traction control.
```

---
## \#207 Posted by: shaman Posted at: 2019-02-04T22:49:49.926Z Reads: 178

```
[quote="Pedrodemio, post:200, topic:81344, full:true"]
Are you sure of that? I can measure later, but the 12 AWG that I have in my hand is almost 3mm
[/quote]

[quote="moon, post:201, topic:81344, full:true"]
2.8mm 10awg. I have just measured it - the copper part
[/quote]

Looks like the diameter is going to vary based on type and probably manufacturer. I'll make the holes 3mm to try and compensate for variance
```

---
## \#208 Posted by: deucesdown Posted at: 2019-02-04T23:35:06.606Z Reads: 190

```
What's happening here, is this some alternate universe? AWG specifies the thickness of a cylindrical wire. It does not vary with respect to use for electrical wiring. As it specifies "thickness" of something cylindrical, it describes a circle, which can be specified by:
- diameter or radius
- circumference
- area

I'm trapped in 'murica units, but I believe the rest of the world uses cross sectional area (mm^2).

This wikipedia page has a table to convert awg to diameter and cross sectional area in both 'murica and SI units.

https://en.wikipedia.org/wiki/American_wire_gauge

10awg:
- diameter
  - 0.1019 inches
  - 2.588 mm
- area
  - 10.4 kcmil (wtf is this unit...)
  - 5.26 mm^2

(did I misunderstand the discussion and will feel stupid shortly?)
```

---
## \#209 Posted by: shaman Posted at: 2019-02-04T23:45:42.628Z Reads: 181

```
No you're statement is valid. That's why I said approx 2.6mm earlier for the same reasons due to the standard of what AWG is. But no manufacturing process is perfect and there will be variance. Also the stranded stuff probably fluffs out a bit which could throw off a measurement. Either way, 3mm should allow 10awg comfortably.
```

---
## \#210 Posted by: shaman Posted at: 2019-02-05T19:00:33.215Z Reads: 187

```
Did a bit of measurements and observation on the switch node ringing today.

So I tried 0.1uF 1206 100V ceramic cap. I measured all 3 switch nodes with a power supply voltage of 12V. The node closest to where power comes in on the rails peaks at 16V. The node furthest away peaks at 21V. Looks like I've got some inductance issues that increase the further you go. I may try various values of polypropylene caps to see if they improve the situation.

One of the contributing factors is the relatively low gate charge of the FETs I'm using. They're TI CSD18535KCS and they only have a typical total gate charge 63nC vs the 236nC of the FETs from the original 4.12 hardware. Increasing the series gate resistance should help. I will seek a balance between adding caps and increasing series gate resistance. 

For the PCB design, I think I need to go ahead an move the big ground track to underneath the big positive track. I've been advised to to this before and now I think I truly understand why. One will have to beef up those traces in a low profile fashion (like with the copper flat wire) since the exposed power track will sit right beneath the tabs of the FETs after I make this adjustment.
```

---
## \#211 Posted by: b264 Posted at: 2019-02-05T19:30:52.229Z Reads: 173

```
No, you aren't misunderstanding, but that is for one cylinder of solid wire.  When you have one thousand small cylinders (super-stranded) all summing to the same area as the big cylinder, the total wire size increases because it also now contains air as well as conductor.
```

---
## \#212 Posted by: ZachTetra Posted at: 2019-02-05T20:45:18.921Z Reads: 173

```
Just whipped out some 10 awg super stranded and some calipers...smallest hole I can easily get it in is 3.2mm

When tinned its closer to 4mm
```

---
## \#213 Posted by: shaman Posted at: 2019-02-05T22:45:26.708Z Reads: 174

```
[quote="ZachTetra, post:212, topic:81344, full:true"]
Just whipped out some 10 awg super stranded and some calipers…smallest hole I can easily get it in is 3.2mm

When tinned its closer to 4mm
[/quote]

Ok. Are all you guys measuring a freshly stripped piece of wire? Cause that's what's going to go through the hole in the PCB.
```

---
## \#214 Posted by: moon Posted at: 2019-02-05T22:49:45.309Z Reads: 183

```
![IMG_20190205_224813_HHT|375x500](upload://b4vlVGiv07xVbM0tkGqDS5hQiK2.jpeg)
```

---
## \#215 Posted by: ZachTetra Posted at: 2019-02-05T23:15:49.185Z Reads: 179

```
You can't pinch wire if it's hot with solder... measure it unsquished
```

---
## \#216 Posted by: Andy87 Posted at: 2019-02-06T11:06:24.965Z Reads: 177

```
But it is not pinched. Just twisted. All good, should be accurate measurement from @moon
```

---
## \#217 Posted by: moon Posted at: 2019-02-06T18:04:45.442Z Reads: 178

```
Yeah it's twisted.

And no one measures shit like what you just described
```

---
## \#218 Posted by: b264 Posted at: 2019-02-06T18:27:23.426Z Reads: 179

```
I just checked here and it's like 3.35mm

![20190206_122441|690x388](upload://e4mgHGKW32MrmJ78wpzmYmxf17m.jpeg) 

![20190206_122550|690x388](upload://1tTnatEeJjRJByvP851pOjPKjpe.jpeg)
```

---
## \#219 Posted by: shaman Posted at: 2019-02-08T03:55:50.651Z Reads: 176

```
OK guys. So I've been going hard on this ringing issue. I'm seeing a voltage spike of about 10V above the supply voltage for whatever the supply voltage may be. I've been successful in getting rid of the ringing after the spike but not the initial spike itself.

The next thing I intend to try is a RC snubber circuit placed on the switch nodes. There is a lot of material out there that shows how this helps and how to design it. Testing this out will be the next thing I do in the lab.

Note that I've improved the PCB design in Altium to attack this issue at its source. What I'm doing now is just putting band-aids on my current prototype so I can do some loaded testing without the thing frying. I'll repeat a lot of this analysis on the version that the testers receive so that I verify that issue will have indeed been fixed.

Also, I'll be out on vacation for the next 5 days so progress won't happen until I get back. Cheers!
```

---
## \#220 Posted by: mishrasubhransu Posted at: 2019-02-08T04:02:53.808Z Reads: 175

```
[quote="shaman, post:219, topic:81344"]
I’m seeing a voltage spike of about 10V above the supply voltage for whatever the supply voltage may be
[/quote]

When are you seeing this spike?
```

---
## \#221 Posted by: shaman Posted at: 2019-02-08T04:04:55.481Z Reads: 180

```
![image|294x171](upload://5l8E3ItT7lL9CLID2v2hHGluL6H.jpeg) 

Showing you guys an example of what I'm trying to get rid of. It's that spike at the upper left corner of that square. That's the MOSFET/DRV killer when you try run the VESC with voltages around 54V or so.
```

---
## \#222 Posted by: shaman Posted at: 2019-02-08T04:07:42.189Z Reads: 182

```
[quote="mishrasubhransu, post:220, topic:81344"]
When are you seeing this spike?
[/quote]

At the switch nodes(phases) on every rising edge. So this is happening at 15kHz on each phase when the FOC frequency is at 30kHz. The spike is also seen on the voltage supply.
```

---
## \#223 Posted by: b264 Posted at: 2019-02-08T04:09:13.390Z Reads: 175

```
@shaman If I could upvote your last three posts a thousand times, I'd have done it
```

---
## \#224 Posted by: shaman Posted at: 2019-02-08T04:10:09.038Z Reads: 174

```
[quote="b264, post:223, topic:81344, full:true"]
@shaman If I could upvote your last three posts a thousand times, I’d have done it
[/quote]

I appreciate that @b264 :slight_smile:
```

---
## \#225 Posted by: mmaner Posted at: 2019-02-08T04:26:01.376Z Reads: 170

```
That's interesting... Like a pill to give me a 45 point IQ bump is interesting. What I'm trying to say is FUCK YEAH!  Keep doing what ya doing.
```

---
## \#226 Posted by: shaman Posted at: 2019-02-08T04:27:17.317Z Reads: 176

```
[quote="mmaner, post:225, topic:81344, full:true"]
That’s interesting… Like a pill to give me a 45 point IQ bumps is interesting. What I’m trying to say is FUCK YEAH! Keep doing what ya doing.
[/quote]

Will do! :smile:
```

---
## \#227 Posted by: mishrasubhransu Posted at: 2019-02-08T05:32:44.087Z Reads: 177

```
Inductive spiking happens when a closed circuit(with an inductor) is suddenly opened. This is not what's happening right? You are seeing the spike at the start of a rising edge. Hmm.
```

---
## \#228 Posted by: AlexBE Posted at: 2019-02-08T07:45:29.889Z Reads: 178

```
I have probably mentioned this before, but how are you making this measurement? If you are using your scope probe with the GND clip attached, it will not work. You will just read the inductive coupling to the scope.
```

---
## \#229 Posted by: b264 Posted at: 2019-02-08T07:46:25.991Z Reads: 170

```
Wouldn't that show the opposite spikes, though?
```

---
## \#230 Posted by: AlexBE Posted at: 2019-02-08T07:49:44.848Z Reads: 175

```
I don't know exactly what you mean, and I don't know exactly what OP is measuring. My general word of warning regards trying to measure fast rising edges when there are high speed gates and big currents floating around. Everyone who has not worked with this kind of stuff before fails to make this measurement correctly and often end up chasing transients that don't exist for months.

Maybe you know, but is OP measuring Vgs of the FETs? Or maybe phase to ground? The fact that they mention that this spike is also on the power rail, tells me there is a very good chance it is not real.
```

---
## \#231 Posted by: Ackmaniac Posted at: 2019-02-08T07:53:32.491Z Reads: 170

```
And how to do it right?
```

---
## \#232 Posted by: AlexBE Posted at: 2019-02-08T07:56:23.318Z Reads: 166

```
extremely small probe loop area by either making custom scope probe leads and soldering them to the board, OR worst case using the spring tips instead of the alligator leads. Even the spring tips will be dodgy at these switching currents. Connect alligator GND to probe tip to see the induced currents to see how bad it is.

OP might have a really good measurement setup, worth checking though to not waste time chasing your tail.
```

---
## \#233 Posted by: shaman Posted at: 2019-02-08T12:18:57.290Z Reads: 177

```
[quote="AlexBE, post:232, topic:81344"]
OP might have a really good measurement setup, worth checking though to not waste time chasing your tail.
[/quote]

I'm using an active probe with low-noise, low-inductance measurement techniques. See figure 6 of [this document](https://e2echina.ti.com/cfs-file/__key/communityserver-discussions-components-files/24/8244.Ringing-Reduction-Techniques-for-NexFET-high-performance-mosfets.pdf)

[quote="AlexBE, post:230, topic:81344"]
The fact that they mention that this spike is also on the power rail, tells me there is a very good chance it is not real.
[/quote]
 
No sir. It's very real.

I encourage all who question this to read 
[this document](https://toshiba.semicon-storage.com/info/docget.jsp?did=59456) and the document I linked before. Parasitic induction **IS** responsible. This ringing is a common occurrence in any application involving H bridges such as DC/DC converters and motor controllers.
```

---
## \#234 Posted by: shaman Posted at: 2019-02-08T14:05:37.130Z Reads: 181

```
From the TI document:

A number of methods have been widely used to minimize the switch node ringing. These methods are listed as follows:
1. Careful PCB layout to minimize the parasitic loop inductance in circuit [1]. 
2. Gate resistor/ Bootstrap resistor to slow down the turn-on of the control FET.
3. RC snubber circuit to attenuate the ringing.
4. Common Source inductance to slow down the turn on of the control FET.

My current prototype has non-ideal layout of the high-current traces causing excessive parasitic inductance. This is what I get for using the cheap Chinese motor controllers as a reference for my layout...

I know there's a lot of EE concepts I'm throwing around. It's not trivial to understand and it takes a bit of reading to wrap you're head around it all. I'll be on
 vacation but I can do my best to answer questions anyone has about all of this.
```

---
## \#235 Posted by: Ackmaniac Posted at: 2019-02-08T15:15:09.748Z Reads: 183

```
Would be great if you can share the pcb layout or at least a image of the layout where you think the problem comes from.
```

---
## \#236 Posted by: shaman Posted at: 2019-02-08T15:44:20.564Z Reads: 190

```
![IMG_20190111_175620|666x500](upload://sHB89yZci9BAHzfdQwZmpeMldHk.jpeg) 

The bottom board is the underside. There you can see two large exposed traces that run parallel to each other with the switch nodes in between. The trace closest to the edge is positive and the other is negative. Having them spaced apart like this causes a large ground loop that causes parasitic inductance 

The new layout has the positive trace directly over the ground trace by the edge of the board. This reduces the loop area and therefore the parasitic inductance.

I can't provide screen shots of the PCB layers right now as I don't have my laptop with Altium with me right now.
```

---
## \#237 Posted by: shaman Posted at: 2019-02-15T03:30:58.277Z Reads: 188

```
https://www.electro-tech-online.com/threads/mosfet-vds-rating.128972/
http://www.tij.co.jp/jp/lit/ds/symlink/csd18535kcs.pdf

So I found a nice bit of information concerning how MOSFETs behave when they encounter voltage spikes above their rated max Vds. They essentially behave like a zener diode and clamp from drain to source. This event is called Avalanche. The MOSFET can handle the avalanche event for a small amount of time which is specified in the datasheet. Figure 11 in the datasheet I linked shows the avalanche characteristics of the FETs I'm using in my prototype.

The high voltage spike I'm seeing and that I've been battling only lasts for 100 nano-seconds. The avalanche rating suggests the MOSFET can handle this just fine even if the spike is 60V or above. I'm still seeking to squash this spike but it may not be a show stopper if I can't squash it completely.

I don't trust the DRV to tolerate 60V for any amount of time so I'm going to try an age old technique to try and protect it. A good old fashioned RC filter on the supply to the DRV should squash these fast spikes. This will involve a resistor in series with the power line to the DRV and will dissipate a small amount of power. Using a 4.7ohm resistor will cause only 23mW to be dissipated, assuming a supply current of 70mA, which is nothing compared to 250W+ being used by the motor.
```

---
## \#238 Posted by: mishrasubhransu Posted at: 2019-02-15T04:21:23.669Z Reads: 172

```
Do you see the spikes when you have a battery connected or just the lab supply. I believe battery will mitigate the effects.
```

---
## \#239 Posted by: shaman Posted at: 2019-02-15T15:03:15.814Z Reads: 167

```
I had the same thought too and switched to a battery a while back. Unfortunately it didn't make a difference.
```

---
## \#240 Posted by: shaman Posted at: 2019-02-15T15:04:37.256Z Reads: 189

```
![TEK0005|640x480](upload://t9zyhdSrJXrQBhaBUWSjSBBI4g8.jpeg) 
Ringing on furthest switch node

![TEK0007|640x480](upload://9YXDoSmerBNlZzxbphiMYhGPCby.jpeg) 
Ringing on furthest switch node after adding 4.7uF electrolytic cap by each FET's drain pin

![TEK0009|640x480](upload://sAZVS5Pu5dG2ns2JXzuKh91B6Xf.jpeg) 
Ringing on furthest switch node after adding 4.7uF electrolytic cap by each FET's drain pin and adding the RC snubber.
*the furthest switch node has the worst ringing and is the furthest away from where power and ground leads come in from the battery

Guys I have good news! I've managed to reduce the ringing/spikes to manageable levels. I've added 4.7uF electrolytic caps by each FET as well as an RC snubber to each switch node. Between those two things, I only have a 15.4V spike when supplying the controller with 13.8V. I'm using a 4.7nF WIMA polypropylene cap and a 4.1ohm resistor for the RC snubbers. 

I've added these extra caps and RC snubber to the PCB design for the future version. I suspect that capacitor value will not need to be as large since I'm pretty sure I've reduced the parasitic inductance in the layout/routing. Now I think I can move on to loaded testing!
```

---
## \#241 Posted by: b264 Posted at: 2019-02-15T20:26:50.256Z Reads: 171

```
This is amazing.

What does the spike measure at 50.4V supply voltage?
```

---
## \#242 Posted by: Benjamin899 Posted at: 2019-02-15T20:36:00.310Z Reads: 163

```
since you are so knowledgeable about this, why not make a controller for much higher voltages?
```

---
## \#243 Posted by: rey8801 Posted at: 2019-02-15T20:38:25.945Z Reads: 167

```
Based on what he said first the 4. 11 version then the 20s one! I am patiently waiting for the biffier one. So we can have a 12-13s reliable vesc
```

---
## \#244 Posted by: shaman Posted at: 2019-02-15T20:50:27.215Z Reads: 169

```
This is exactly what's happening. I've already started the schematic/layout of the high voltage version. It will have all of my lessons learned from the Cheap VESC development.
```

---
## \#245 Posted by: shaman Posted at: 2019-02-15T20:51:34.422Z Reads: 171

```
[quote="b264, post:241, topic:81344, full:true"]
This is amazing.

What does the spike measure at 50.4V supply voltage?
[/quote]

Don't know but I need to find out. This will be next week's problem :slight_smile:
```

---
## \#246 Posted by: shaman Posted at: 2019-02-15T20:55:21.236Z Reads: 173

```
[quote="shaman, post:1, topic:81344"]
Features of Future Versions (Calling them the High Voltage (HV) 6 and 12 FET versions)

* Implementing DRV8353 for higher voltage operation (I estimate at least 20s capable). Will need stable version of VESC 6 firmware/software for the 3 phase current sensing and stuff.
[/quote]

It's happening :slight_smile:
```

---
## \#247 Posted by: shaman Posted at: 2019-02-18T14:04:23.617Z Reads: 188

```
![TEK0013|640x480](upload://dDOVCDy5M5ySCf6hDfrFgtZq9v8.jpeg) 
Vsupply @ 50.4V

![TEK0014|640x480](upload://k4m49XXCzLuvO06Y8X4iP1HCYIG.jpeg) 
Vsupply @ 42v

Here you go! Running 50.4(12S) on my prototype doesn't exceed 60V but you still get a +6V spike. Now remember I expect the version I release to be better than this. The real test though will be on the dyno under load. I gotta see how high currents affect all of this.
```

---
## \#248 Posted by: rey8801 Posted at: 2019-02-18T14:23:45.810Z Reads: 178

```
That's fantastic! Well done.
If you want tester for 12s I can give it a try. Don't want it free. You could send a prototype to people that wants to try it out and stress it out and pass to the next one. I am making a new 12s4p board with DIY direct drive.
```

---
## \#249 Posted by: moon Posted at: 2019-02-18T14:31:40.438Z Reads: 183

```
Ill tag @b264 :slight_smile:
 
Even though he is probably watching the thread

Nice work, even though I don't know whats happening 1/2 the time
```

---
## \#250 Posted by: shaman Posted at: 2019-02-18T14:35:31.117Z Reads: 185

```
I do. Look for a PM once I'm ready to reach out to testers. FYI I'm looking at having the test controllers assembled for the testers. I'll divulge more details after it's all hashed out.
```

---
## \#251 Posted by: shaman Posted at: 2019-02-18T14:36:49.091Z Reads: 182

```
No worries! Also feel free to ask for clarification when you need it. That goes for everyone.
```

---
## \#252 Posted by: deucesdown Posted at: 2019-02-18T15:13:28.967Z Reads: 181

```
Can you sneak a tube screamer in the circuit? With true bypass? :)
```

---
## \#253 Posted by: shaman Posted at: 2019-02-18T15:20:05.034Z Reads: 188

```
Ha! I'll call it the Screaming FOCer!
```

---
## \#254 Posted by: b264 Posted at: 2019-02-18T18:49:55.605Z Reads: 189

```
[quote="shaman, post:247, topic:81344"]
Running 50.4(12S) on my prototype doesn’t exceed 60V but you still get a +6V spike. Now remember I expect the version I release to be better than this. The real test though will be on the dyno under load. I gotta see how high currents affect all of this.
[/quote]

This is exactly the kind of stuff we need.  Awesome!
```

---
## \#255 Posted by: shaman Posted at: 2019-02-18T19:33:01.187Z Reads: 192

```
![image|319x164](upload://jYKfRMnITUZtE85ZShPKdNwJhmA.png) 
**1: LCSC cart total**

![image|295x187](upload://iOQxs3IsNkOTSWdEMp8ZzpAuEbm.png) 
**2: JLCPCB cart total**

Here's an estimate of cost to make one of my VESCs. This is the BOM and PCB through LCSC/JLCPCB. You can combine the PCB and BOM orders into one shipment. When I'm done, there will be an LCSC specific BOM file on the Github that you can upload onto the site and auto-load a cart for my VESC BOM. It will be a similar process for JLCPCB and the gerbers for the PCB. Shipping costs may vary from country and I may add some things to the BOM between now and completion, but this is in the ballpark.

*This is the cost for making just **1** of my VESCs along with free samples from TI. The cost per VESC changes if/when you decide to make multiple
```

---
## \#256 Posted by: Andy87 Posted at: 2019-02-18T19:38:44.136Z Reads: 186

```
I have two 8085 motors I could test them out on.
Always ready for it!
Like @rey8801 i don’t want anything for free, just try to give you opportunities to test your work in real life conditions.
As i don’t have the knowledge to support you while developing this is the only thing I can offer.
So if you one day at this point, let us know and we glad to look what we can get out of your escs 😜
```

---
## \#257 Posted by: shaman Posted at: 2019-02-18T19:58:45.686Z Reads: 185

```
Cool! I have had quite a few volunteers to test my VESC. I have to go back and assess them all in chronological order so I can prioritize who I ask first. It's looking like I'll have about 15 assembled controllers for testing. I'll be sending PMs to those that have asked to help test once its time. I will have to ask you guys to help cover the costs of BOM, board, and assembly. I'll provide more details as we get closer to that stage. 

I really appreciate you and the others coming forward to help me gather test data. It gives me the opportunity to prepare my VESCs for real life applications!.
```

---
## \#258 Posted by: Mich21050 Posted at: 2019-02-18T20:00:10.258Z Reads: 178

```
I would also be willing to test it. I can assemble mine myself. I would only need the BOM and Gerbers.. :slight_smile:
```

---
## \#259 Posted by: shaman Posted at: 2019-02-18T20:02:02.773Z Reads: 180

```
Awesome! Hopefully I'll have the Github repository up and running by the time I'm ready to send out the test controllers. If not, I'll send the BOM and Gerbers to you and anyone else who wants to go this route.
```

---
## \#260 Posted by: shaman Posted at: 2019-02-18T20:07:30.464Z Reads: 179

```
One big detail I forgot to mention here. This is assuming you get free samples through TI.com. That's how the total is so low. The DRV, 3.3V LDO, and CAN transceiver and be acquired as free samples.
```

---
## \#261 Posted by: janpom Posted at: 2019-02-18T20:19:23.162Z Reads: 193

```
Me too! Pick me, pick me! 

![giphy|426x240](upload://g0HwbKBE5MRxvA3GIQBIVLFm53f.gif)
```

---
## \#262 Posted by: Mich21050 Posted at: 2019-02-18T20:20:22.090Z Reads: 187

```
I could solder one and if that works will I would be willing to solder a bunch.. Of course with @shaman 's permission.. :slight_smile:
```

---
## \#263 Posted by: shaman Posted at: 2019-02-18T20:28:36.135Z Reads: 188

```
Someone has already offered to assemble 15 controllers for me. Him and I have been discussing details. However, I won't stop you if you want to do more on your own.
```

---
## \#264 Posted by: shaman Posted at: 2019-02-18T20:46:43.787Z Reads: 190

```
Ha! I'll let you know :slight_smile:
```

---
## \#265 Posted by: shaman Posted at: 2019-02-20T14:53:27.101Z Reads: 199

```
Due to the amount of likes I got for the Cheap FOCer name, I'm gunna roll with that for my ESC. Keeps the VESC name owners happy. Keeps me happy with an original name. Keeps you guys happy with a name you liked.
```

---
## \#266 Posted by: LukePL Posted at: 2019-02-20T15:02:46.540Z Reads: 195

```
Hehehehe super cool. I would like to get one just for the name :D
```

---
## \#267 Posted by: lrdesigns Posted at: 2019-02-21T00:47:32.398Z Reads: 199

```
Great name! "He's a Cheap FOCer"

Can anyone find a cheaper version of these waterproof aluminum boxes? I found [this one](https://www.aliexpress.com/item/Aluminum-waterproof-electronics-cabinet-box-aluminium-amplifier-enclosure-DIY-aluminum-housing-project-junction-box-115-68/32906085955.html?spm=2114.search0104.3.69.5c5e19ea3cFRVw&ws_ab_test=searchweb0_0,searchweb201602_7_10065_10068_319_10059_10884_317_10887_10696_321_322_10084_453_10083_454_10103_10618_10307_537_536_10902,searchweb201603_61,ppcSwitch_0&algo_expid=c8141199-6597-4bed-98db-6762633108cf-11&algo_pvid=c8141199-6597-4bed-98db-6762633108cf) for about $20 delivered on aliexpress. 

![image|500x477](upload://4gFY6nxxVq84oGXqvFfkCAxcPtv.jpeg)
```

---
## \#268 Posted by: shaman Posted at: 2019-02-21T04:06:06.482Z Reads: 196

```
![image|500x500](upload://sDAdedmJtS59bcYsGQXbc5SDPs6.jpeg) 
https://www.digikey.com/product-detail/en/hammond-manufacturing/1590WB/HM586-ND/284783

These are the Hammond 1590WB. The "W" marks the IP65 waterproof version. The difference is that it has the gasket and o-rings. You can also just buy the regular 1590B and the gasket/o-rings separate.
```

---
## \#269 Posted by: shaman Posted at: 2019-02-27T18:01:35.081Z Reads: 192

```
Sorry I haven't posted in a while. I'm actively working on setting up the loaded testing with the dyno and such. This test will be conducted in a lab environment and I'm working with the lab manager on details. Testing is tentatively scheduled for Friday afternoon central time. I'll keep you guys on the thread in the loop as best as I can.
```

---
## \#270 Posted by: shaman Posted at: 2019-03-02T01:03:52.115Z Reads: 183

```
Unfortunately no testing today but I got the majority of the setup done. See the link below to my most recent post in the Endless Sphere. Couldn't post the content here due to a forum memory shortage. Going to try again Monday.

https://endless-sphere.com/forums/viewtopic.php?f=7&t=97699&p=1449031#p1449031
```

---
## \#271 Posted by: Andy87 Posted at: 2019-03-02T02:14:24.228Z Reads: 178

```
@shaman sorry if the question was asked before, but I don’t remember that it was,so...
What do you think is the max ERPM limit with the drv you use?
The old basic v4.12 hw was limited to 60000.
Which was already critical on 12s and motors with 200+kV.
```

---
## \#272 Posted by: shaman Posted at: 2019-03-02T02:16:53.023Z Reads: 178

```
It will be the same for this one and most likely anything that uses the STM32F405RGT6 along with the VESC firmware. The limit isn't due to the DRV, it's due to the processing speed of the microcontroller.
```

---
## \#273 Posted by: shaman Posted at: 2019-03-02T02:18:00.787Z Reads: 173

```
Thats for 4.12 hardware. The VESC 6 stuff is higher I think. My next gen controller may be able to go higher as well. We'll see.
```

---
## \#274 Posted by: Andy87 Posted at: 2019-03-02T02:20:30.215Z Reads: 175

```
I don’t know what is used in the focbox, but they tested till 100000 which is already better.
Also the vesc 6 design has a limit above that (140000 if I remember right 🤔)

There is no easy way to extend the erpm limit?
I personally don’t see an issue as I use 190kV or lower on 12s, but if your design allows to use up to 20s the kV of the motors would need to go drastically down to not fry the esc.
```

---
## \#275 Posted by: shaman Posted at: 2019-03-02T02:23:58.632Z Reads: 180

```
The 20s capable controller is the next controller I design, not the Cheap FOCer. That high of voltage is more useful in the large hub motors of eBikes anyway. Motors with around 40kV. I will start a new thread for my high voltage controller after the testing phase of the Cheap FOCer.
```

---
## \#276 Posted by: shaman Posted at: 2019-03-02T02:27:12.114Z Reads: 183

```
You can reterminate delta configured motors to a wye configuration. This divides your kV by 1.73. This pretty much forces you to run sensorless though as the hall effect sensors would only be good for the original delta configuration. Most outrunner phases are in delta configuration.
```

---
## \#277 Posted by: Andy87 Posted at: 2019-03-02T02:28:21.739Z Reads: 187

```
Alright, sounds good 👌
```

---
## \#278 Posted by: b264 Posted at: 2019-03-02T03:30:01.055Z Reads: 188

```
[quote="shaman, post:275, topic:81344, full:true"]
The 20s capable controller is the next controller I design, not the Cheap FOCer. That high of voltage is more useful in the large hub motors of eBikes anyway. Motors with around 40kV. I will start a new thread for my high voltage controller after the testing phase of the Cheap FOCer.
[/quote]

40kv at 20S on an esk8 would have so much torque it'd rip your shoes off.  Can't wait for that.
```

---
## \#279 Posted by: shaman Posted at: 2019-03-05T00:08:31.058Z Reads: 201

```
![image|624x351](upload://t9uvXvjE7JnbhVfulLaHxxTaOWC.png) 

I Motor = 20A

![image|624x351](upload://85Sa3W6Zh9yhsOIqC63s2c2T8WY.png) 

I Motor = 30A

![image|624x351](upload://dF2piyPyacRrdu0CrdYpXU0mTOj.png) 

I Motor = 43A

Completed some initial tests at 24V to 27V. The temperature to look at is T FET. The current to look at is **I Motor (Phase amps)**. This is the current that the MOSFETs pass to the motor and therefore cause the heating. The motor was ran at 18% duty cycle in BLDC control mode. Each current limit was tested for at least 3 minutes or until the MOSFET temperature stabilized.The conditions weren't ideal with the controller sitting in still-air with only a relatively small amount of aluminum for heat sinking. Real life conditions will most likely be much better when the controller is in a full aluminum enclosure with wind rushing past it as you ride down the road/sidewalk. Overall this gives me confidence that this controller can handle 40A to 50A continuous for a decent duration when placed in the mentioned ideal conditions. 

Understand that I am testing continuous current limits. This means that you can still deliver higher phase currents to your motor for a short duration such as for accelerating. 

I will do loaded tests at higher voltage levels later this week to see if this can handled the coveted 12s battery.

*Test conducted in 23C ambient temperature. Hotter ambient temps will decrease max continuous current handling capability
```

---
## \#280 Posted by: Andy87 Posted at: 2019-03-05T15:41:11.548Z Reads: 190

```
[quote="shaman, post:279, topic:81344"]
with wind rushing past it as you ride down the road/sidewalk
[/quote]

That’s not always the case when the esc is mounted in the underboard enclosure for example there is only very less air flow around it.
Besides this it non the less looks already pretty good and i‘m sure a proper heat sink will help a lot to get some more amps out of it.
👍
```

---
## \#281 Posted by: shaman Posted at: 2019-03-05T17:20:12.261Z Reads: 187

```
I would encourage users to mount this controller where it can be exposed to airflow. The hammond enclosures I've mentioned should be worthy to mount to the underside of a board. Maybe I'm missing something though.
```

---
## \#282 Posted by: moon Posted at: 2019-03-05T17:23:31.558Z Reads: 188

```
Yeah no one does that. All the current ESCs just have heatsinks.

well there might be a few people do it
```

---
## \#283 Posted by: banjaxxed Posted at: 2019-03-05T17:26:07.492Z Reads: 189

```
A cheap PC heatsink
```

---
## \#284 Posted by: shaman Posted at: 2019-03-05T17:31:08.535Z Reads: 195

```
https://www.electric-skateboard.builders/t/vesc-hw-4-12-temperature-comparison/23230

Seems like the benefits of airflow would be obvious. Someone has taken the time to prove that in the thread I linked. Application was an ebike though.
```

---
## \#285 Posted by: Andy87 Posted at: 2019-03-05T17:42:34.254Z Reads: 192

```
No doubt that airflow would be better and the box you mentioned or recommended would be easy to mount exposed.
I think for people who want to use it on a mtb the airflow is not the problem.
Buuut a lot of guys here store there esc inside if the enclosure.
I think for this it would be great if we ( maybe @moon ) can design a heatsink which could be mount in a cut out of the enclosure.
```

---
## \#286 Posted by: shaman Posted at: 2019-03-05T18:11:39.452Z Reads: 188

```
I see what you're talking about after googling eskate enclosures. Sure seems like the cut out idea would the way to make a heatsink work with the controller. I'm surprised eskate manufacturers/DIYers haven't adopted a more modular approach with the controller and battery being in separate enclosures.
```

---
## \#287 Posted by: rey8801 Posted at: 2019-03-05T18:18:02.592Z Reads: 186

```
They did. It's mostly for flexible decks to leave free space in the middle. Although everyone is trying to have the smallest and slimmest enclosure with the biggest battery possible. That's why the typical layout. I think the cut out with heat sink will work just fine.
```

---
## \#288 Posted by: shaman Posted at: 2019-03-05T18:31:20.674Z Reads: 196

```
Got it. Even though I'm designing this controller I need info like this to understand the eskate application. Thanks everyone for educating me on how this will most likely be mounted on a board. :slightly_smiling_face:
```

---
## \#289 Posted by: Andy87 Posted at: 2019-03-05T18:33:56.547Z Reads: 198

```
It very much depends on the board.
For example on my e-mtb I have the battery box in the middle and on both deck ends a case for my vescs 
![image|375x500](upload://yAuXuFOGOB1qpOnjazQnPXRN8G4.jpeg)
```

---
## \#290 Posted by: b264 Posted at: 2019-03-05T19:51:01.432Z Reads: 198

```
[quote="shaman, post:281, topic:81344"]
I would encourage users to mount this controller where it can be exposed to airflow.
[/quote]

"exposed to airflow" often means "exposed to saltwater spray" so keep that in mind.  Saltwater tends to eat everything it touches that's made of metal.
```

---
## \#291 Posted by: spei Posted at: 2019-03-05T20:06:51.755Z Reads: 190

```
How about making it water and air tight, with heatsinks exposed to air flow? At least thats what people do with with heatsinks for their controllers, not all people, but they do it.
```

---
## \#292 Posted by: shaman Posted at: 2019-03-05T20:46:42.851Z Reads: 195

```
I didn't consider that, but a coat of clear spray lacquer on something like that Hammond enclosure should help with corrosion. Something similar could be done to exposed heatsink fins. Maybe even anodizing them could help with corrosion.
```

---
## \#293 Posted by: shaman Posted at: 2019-03-05T20:54:03.981Z Reads: 202

```
![TEK0000|640x480](upload://pBpw6e7NhPdaFOUnjLo7wPdsJUS.jpeg) 
Vsupply = 50.4V, 
I Motor = 46A continuous


So I did a test at 50.4V with the motor under load. I picked up spikes of 61.6V under these conditions. Note that I could not use low-induction/low-noise measurement techniques as I did before for this test. I estimate at least 3V are attributed to the non-ideal measurement. Secondly, this is with the bad layout of my prototype. The tester's edition and beyond will have much better layout and probably lower spikes. I will test the newer version of the Cheap FOCer under the same conditions so a side-by-side comparison can be made.
```

---
## \#294 Posted by: b264 Posted at: 2019-03-05T23:11:32.421Z Reads: 192

```
Water tight never works.  Water always gets in eventually.  The secret is making it water-resistant like you said but also making it waterproof so once water gets in, it still works.
```

---
## \#295 Posted by: shaman Posted at: 2019-03-05T23:19:44.522Z Reads: 195

```
I see. Things like IP65 or better enclosure and conformal coating to the assembled PCB should help fight corrosion and moisture...for a while at least. Nothing will last forever though.
```

---
## \#296 Posted by: shaman Posted at: 2019-03-10T13:33:44.654Z Reads: 196

```
Hey guys here's an update on the project. The beta testers are finishing up their payments for their test controllers. Once that happens, I'll order the materials of the controllers and have them shipped to @Martinsp. 

@Martinsp has volunteered to be the assembler of the test controllers. He'll be shipping the controllers to the test volunteers once they are done.

In the mean time, I will be preparing the documentation i.e schematics, gerbers and BOM for my GitHub repository. Once uploaded, it will be dubbed open source and available to all.
```

---
## \#297 Posted by: shaman Posted at: 2019-03-12T23:35:18.941Z Reads: 191

```
BOM and PCBs have been ordered and/or shipped already! Wish us luck in everything making it to @Martinsp without any troubles. 

So this is my first time coordinating anything like this. I've done my best to account for expenses but there may be some surprise costs such as taxes, duties, or whatever other not-fun expenses that make it hard to send other humans some stuff. I'd like to offer you guys the option to pitch in any amount of help you wish to offer. Any amount will help me, the test volunteers, and Martin out in making sure this project follows through :slightly_smiling_face:

https://www.paypal.me/shamansystems?locale.x=en_US
```

---
## \#298 Posted by: shaman Posted at: 2019-03-24T23:23:26.759Z Reads: 186

```
Hey guys! Project update

@Martinsp now has most of the materials needed. The assembly process will begin this week and we will hopefully have the beta controllers in the mail to the beta testers soon. Stay tuned and wish us luck!
```

---
## \#299 Posted by: lrdesigns Posted at: 2019-03-25T00:58:13.456Z Reads: 189

```
Awesome, hope we get lots of photos of these prototypes.
```

---
## \#300 Posted by: Benjamin899 Posted at: 2019-03-25T01:38:27.185Z Reads: 188

```
keep it up
```

---
## \#301 Posted by: shaman Posted at: 2019-03-29T00:11:07.670Z Reads: 190

```
![Cheap%20FOCer%20in%20progress|666x500](upload://5eYX5ZQulAICddNwE2aNizL27LP.jpeg) 
![Cheap%20FOCer%20in%20progress2|666x500](upload://pCZhuvRngu6iWx9W7Z7Zal9ZjAv.jpeg) 

Hey guys Martin is working through the assembly process. Here some pics of a board with some of the SMD components placed.
```

---
## \#302 Posted by: skatardude10 Posted at: 2019-03-29T00:13:42.920Z Reads: 182

```
I like how you did the copper like that, I might give that a try.
```

---
## \#303 Posted by: shaman Posted at: 2019-03-29T00:15:09.468Z Reads: 183

```
Yeah @Martinsp had the awesome idea of just using single-core copper for trace beefing. It looks good!
```

---
## \#304 Posted by: skatardude10 Posted at: 2019-03-29T00:16:43.565Z Reads: 188

```
What kind of iron/power did you use for that? Did you just run the iron down them as the solder melted? How did you keep them in place without rolling off?
```

---
## \#305 Posted by: shaman Posted at: 2019-03-29T00:18:42.673Z Reads: 188

```
This is a question for @Martinsp. It looks as if he just used a ton of solder paste, wrapped the copper wires in regular solder wire, and flowed it accordingly. The tension of the solder in a liquid state keeps the wires in place.
```

---
## \#306 Posted by: skatardude10 Posted at: 2019-03-29T00:20:57.104Z Reads: 200

```
Nice. Thanks!
```

---
## \#307 Posted by: shaman Posted at: 2019-03-31T20:50:58.903Z Reads: 205

```
![image|666x500](upload://vFhbt4AxD574Q13t0ap5Lad74XL.jpeg)
@Martinsp has been working hard guys!  Next is functional testing, attaching the heatsink, and then applying the conformal coating.
```

---
## \#308 Posted by: shaman Posted at: 2019-04-02T16:10:32.553Z Reads: 197

```
Got some slightly bad news. Texas Instruments has changed how they do their sampling. You now have to have a business email and a few other qualifications before being able to get free samples. Kinda sucks for the hobbyists. The BOM will be more expensive for one-off boards now being that you can't practically get free samples anymore.
```

---
## \#309 Posted by: Benjamin899 Posted at: 2019-04-03T06:51:36.761Z Reads: 189

```
Are they offering it for schools/universities?
```

---
## \#310 Posted by: shaman Posted at: 2019-04-07T17:25:28.887Z Reads: 183

```
Idk. I'll have to look into it further
```

---
## \#311 Posted by: shaman Posted at: 2019-04-07T17:27:33.733Z Reads: 189

```
So I have good news and bad news.

Good news is that the controllers have been made and are functional in FOC and BLDC. Martin spun a 380kV motor with a 10s battery to test these controllers. No eRPM issues!

Bad news is that I messed up the CAN power rail on the PCB. My intent was to have a beefy automotive grade CAN transceiver to help with the issues people experience when using CAN with HW 4.12. I totally missed the fact that the new CAN transceiver needed 5V and not 3.3V. I didn’t make that adjustment in the PCB design :frowning_face: Martin is currently getting 3.3V CAN transceivers from Europe to put on the controllers so we can at least have functioning CAN for the beta test team

I fixed the PCB design now so that CAN device gets the 5V that it should. This is why I didn't want to release the design before feedback from the beta test experience.
```

---
## \#312 Posted by: Benjamin899 Posted at: 2019-04-07T18:38:17.285Z Reads: 188

```
my buddies at the lab like your idea and we are gonna build like 10 or so.
```

---
## \#313 Posted by: shaman Posted at: 2019-04-07T18:53:47.550Z Reads: 180

```
Cool! What do they like about it?
```

---
## \#314 Posted by: Benjamin899 Posted at: 2019-04-07T18:57:55.201Z Reads: 184

```
whats not to like. Not too expensive, bigger parts make it easier to solder and like you said the CAN improvment. They want to use it on small vehicles for transportation. But the most important thing, for science^^
Also they testet my board and are hooked.
```

---
## \#315 Posted by: TowerCrisis Posted at: 2019-04-07T19:02:16.679Z Reads: 181

```
Honestly I could seriously see this used in an educational setting.

- good pricing
- robust design
- user repairable (TA's and the like)
- headers, headers, headers. Standard pinouts are so beautiful.
- mini USB means it can be repeatedly setup.
```

---
## \#316 Posted by: brschaefer74 Posted at: 2019-04-07T19:04:11.957Z Reads: 174

```
What type of issues were seen with 4.12?
```

---
## \#317 Posted by: shaman Posted at: 2019-04-07T19:05:52.237Z Reads: 172

```
My wife actually has the same idea. We spoke about getting involved with education with my open source designs. Academia needs a lot of help relating theory to industry...
```

---
## \#318 Posted by: shaman Posted at: 2019-04-07T19:08:24.121Z Reads: 177

```
Issues with transients over the CAN bus when the bus lines were suddenly disconnected during operation. The transients could actually kill the MCU too.

 There are other qualities that are improved upon by the VESC 6 design that my new controllers are based on.
```

---
## \#319 Posted by: Benjamin899 Posted at: 2019-04-07T19:08:43.278Z Reads: 177

```
My thoughts exactly, we want to do a workshop.
```

---
## \#320 Posted by: brschaefer74 Posted at: 2019-04-07T19:10:28.163Z Reads: 185

```
Pretty sure that is what killed one of my first units.
```

---
## \#321 Posted by: shaman Posted at: 2019-04-07T19:14:12.799Z Reads: 192

```
The version of Cheap FOCer I release with have the CAN issue addressed and utilizes an automotive grade transceiver with high voltage bus tolerances. It should eliminate the issue
```

---
## \#322 Posted by: shaman Posted at: 2019-04-10T18:42:21.416Z Reads: 194

```
https://github.com/shamansystems/Cheap-FOCer

Ok. So I finally got the GitHub repository up. The schematics and silk screen on the PCB still need some cleaning up on my end but at least this is something. I'll be cleaning up the files and repository as we progress through the beta testing process.
```

---
## \#323 Posted by: doomy Posted at: 2019-04-11T06:21:58.058Z Reads: 192

```
wow thats so cool, thank you very much for your work. 

will order some pcb and assemble them asap.

cheers!
```

---
## \#324 Posted by: goldrabe Posted at: 2019-04-11T06:32:00.653Z Reads: 190

```
I did lurked on this thread and your achievements are impressive!\
One thing that always bugs me with all vesc derivatives I had are the standard jst connections for sensors, canbus, UART and PPM. They always are prone to coming loose due to vibrations e-skates are facing. I would love to see connectors with a locking mechanism like they are used in automotive applications like these.
![images%20(2)|350x350](upload://ncgrm85FrmRhpxi5f2FrxataLut.jpeg)
```

---
## \#325 Posted by: shaman Posted at: 2019-04-11T10:35:14.952Z Reads: 187

```
I still have to upload the BOM. Hopefully I can get that done today
```

---
## \#326 Posted by: shaman Posted at: 2019-04-11T10:41:04.994Z Reads: 185

```
This is something I've thought about for the new controllers I'm working on.
```

---
## \#327 Posted by: janpom Posted at: 2019-04-11T10:48:46.044Z Reads: 186

```
Hm, I never had a problem with a JST connector coming loose. I usually have hard time disconnecting them even when I want to. Takes a lot of wiggling. I can't imagine that they would come loose merely due to vibrations.

The nice thing about standard JST is that it's widely available and you can create custom cables easily. I wonder if that would still be possible with these locking connectors and whether you wouldn't have hard time finding exactly the ones that you need.

I guess it would still be possible to deliver the ESCs without any connectors at all and then everyone can solder the on their preferred ones since that's very easy to do.
```

---
## \#328 Posted by: goldrabe Posted at: 2019-04-11T11:05:22.907Z Reads: 185

```
I've had them come loose, there are better ones and loose ones. People here use hot glue, cable binders etc. to avoid this. In my case everything is attached to the deck and not placed in the enclosure, so gravitation doesn't help.\
I agree and see your point that those ones are not that easily available. I can solder basic stuff, but would rather avoid soldering on pcb's with my basic skillset and tools.
```

---
## \#329 Posted by: janpom Posted at: 2019-04-11T11:08:32.558Z Reads: 181

```
Just to be clear, are you talking about the mating connectors disconnecting or about the wires coming out of the connector? I never had a problem with the former. I do sometimes have problems with the latter, but as you say, hot glue helps.
```

---
## \#330 Posted by: goldrabe Posted at: 2019-04-11T11:18:41.235Z Reads: 186

```
I had both issues, recently a cable broke at the joint I made with hot glue between the wires and jst connector to prevent them from backing out.\
Anyway I don't want to over exaggerate this, it's just something what would give me more confidence.\
And this ESC is already great with standard jst connectors!

`
```

---
## \#331 Posted by: shaman Posted at: 2019-04-11T12:22:06.832Z Reads: 193

```
[quote="goldrabe, post:330, topic:81344"]
And this ESC is already great with standard jst connectors!
[/quote]

Sorry but the stock Cheap FOCer simply has standard pin headers for connectors. One can most likely replace these with different connectors as long as the pin spacing is the same
```

---
## \#332 Posted by: shaman Posted at: 2019-04-12T15:38:07.565Z Reads: 200

```
So it looks like universities qualify for free samples. This will be good for those that want to use this for educational purposes.

* Step 1 – Create or login to your myTI account using a corporate or university email domain. The TI store does not allow sample orders from a free email domain (e.g. @gmail, @yahoo, @qq, etc.)

* Step 2 – Click [here](https://www.ti.com/csc) for the samples program request form and selct "Create a new case"

* Step 3 – Select “Request access to TI’s sample program”

* Step 4 – Complete and submit the form with your corporate or universtiy myTI account

* Step 5 – You will be notified by email within 5 business days if you are approved for samples or if you need to purchase your devices from the [TI store](http://store.ti.com/)

TI's sample policy:

* All sample orders are shipped ground
* Sampling limits apply
* A company or universtiy email address is required to process your order
* Free email domains (e.g. @gmail, @yahoo, @qq, etc.) will not be accepted
```

---
## \#333 Posted by: Benjamin899 Posted at: 2019-04-12T21:08:42.698Z Reads: 187

```
awesome, thanks for the write up.
```

---
## \#334 Posted by: lazarus Posted at: 2019-04-14T17:57:00.219Z Reads: 187

```
Hey @shaman, I'm thinking of putting together a couple of these. Is the BOM uploaded already? Any design changes in the works I should wait for?
```

---
## \#335 Posted by: shaman Posted at: 2019-04-14T19:07:44.709Z Reads: 192

```
Ok I just uploaded the BOM specific for LCSC. By default it contains enough components for one build and you can upload it to LCSC via their BOM tool. After going through the BOM tool the cart should load up with the components. Note that LCSC is currently out of stock of the CAN transceiver and the DRV8302 . You will have to source the DRV from somewhere else.

Note that BOM has large quantities for the resistors and capacitors. This is because LCSC makes you order most of those at a minimum quantity of 50. I'll upload the traditional BOM soon that reflects exactly what each component is and how many you need.
```

---
## \#336 Posted by: lazarus Posted at: 2019-04-14T19:23:31.066Z Reads: 189

```
Awesome, thanks! I'll be getting a couple extra PCBs due to min order, if anyone else wants to give this a shot and form a small group (ideally SF bay area) PM me.
```

---
## \#337 Posted by: shaman Posted at: 2019-04-14T19:26:19.391Z Reads: 190

```
I uploaded the regular BOM. Note that I don't specify a part number for generic resistors and capacitors. There's no need. Just find some that have the specifications as listed in the BOM.
```

---
## \#338 Posted by: shaman Posted at: 2019-04-14T19:34:40.010Z Reads: 190

```
I don't have design changes planned unless something is discovered during the beta testing that requires a change. Feel free to let me know if you find discrepancies in the BOM or any other files. I'm the only reviewer for all of this so there's bound to be some small mistakes.
```

---
## \#339 Posted by: Blacksheep Posted at: 2019-04-17T05:39:09.226Z Reads: 185

```
Could I test one ?
```

---
## \#340 Posted by: shaman Posted at: 2019-04-17T12:30:50.407Z Reads: 190

```
Unfortunately those participating in the beta test have already been identified and have paid. However the Gerbers and schematic are on my GitHub repository if you would like to make one.
```

---
## \#341 Posted by: Blacksheep Posted at: 2019-04-17T13:08:58.217Z Reads: 187

```
I don’t have the skills for making one
```

---
## \#342 Posted by: shaman Posted at: 2019-04-17T13:56:58.343Z Reads: 181

```
Would you be interested in participating in a  "group buy" event? If there is enough interest in this, I may do a group buy for this controller. If anyone else is interested in this then let me know. Don't forget I have the newer model controllers I'm developing if you would rather hold out for those.
```

---
## \#343 Posted by: Blacksheep Posted at: 2019-04-17T14:16:13.502Z Reads: 178

```
Yes please I’m currently building a build just need controller
```

---
## \#344 Posted by: Benjamin899 Posted at: 2019-04-17T15:08:21.609Z Reads: 182

```
just created a sample order on TI, 3 components are from TI and the rest have to be sourced elsewhere right? Still new to this BOM thing^^
```

---
## \#345 Posted by: Mich21050 Posted at: 2019-04-17T15:12:57.780Z Reads: 184

```
Yes. Best would be lcsc since you can combine your order with jlcpcb. You can just upload the BOM from Github to lcsc and order all your parts. :slight_smile:\
You can just PM me if you need more help.
```

---
## \#346 Posted by: shaman Posted at: 2019-04-17T16:03:53.806Z Reads: 187

```


[quote="Mich21050, post:345, topic:81344"]
Best would be lcsc since you can combine your order with jlcpcb. You can just upload the BOM from Github to lcsc and order all your parts. :slight_smile:
[/quote]

This is correct. Note that the stock and minimum quantities for the parts on LCSC do change frequently. You very well may find that some parts are out of stock already and need to be subbed out. No worries, just find a replacemnt that has the same spec. A 0805 25V X7R 2.2uF ceramic cap is more or less the same from manufacturer to manufacturer.
```

---
## \#347 Posted by: Benjamin899 Posted at: 2019-04-17T16:12:46.698Z Reads: 184

```
dang i was declined by TI. welp gotta go buy it myself.
```

---
## \#348 Posted by: diedirk Posted at: 2019-04-17T18:06:24.001Z Reads: 187

```
I would be interested in an group buy for a diy kit.
```

---
## \#349 Posted by: shaman Posted at: 2019-04-17T18:18:37.141Z Reads: 194

```
A group buy would most likely be for completely assembled modules like the ones for the beta test team. Before I do this, I'll need to check with @Martinsp if he would be willing to assemble a group buy batch.

This wouldn't happen until after the beta testers get they're controllers and have had some time for testing.
```

---
## \#351 Posted by: shaman Posted at: 2019-04-22T19:37:10.432Z Reads: 188

```
FYI I've uploaded an Assembly pdf document on the GitHub. It helps in identifying which component goes where on the PCB.
```

---
## \#352 Posted by: shaman Posted at: 2019-04-26T14:10:36.709Z Reads: 190

```
Shipping the beta controllers has begun! 

Also, I've been cleaning up the schematic for the controller. Expect an update in the GitHub soon.
```

---
## \#353 Posted by: shaman Posted at: 2019-05-03T22:04:14.745Z Reads: 182

```
![image|690x388](upload://20PdhpQunAGN3LuCFBCQXFbpmdo.jpeg) 

The beta testers and I are starting to receive the beta controllers in the mail. I'll be testing one of mine in the lab next week to see if there are any improvements over the proto-FOCer. I'll be posting results here just as I've done in the past.
```

---
## \#354 Posted by: doomy Posted at: 2019-05-05T07:07:43.716Z Reads: 183

```
I really like your design shaman, cant wait for the high amp/volt version. Where did you get the thermal pads on the mosfets?
```

---
## \#355 Posted by: shaman Posted at: 2019-05-05T14:02:01.377Z Reads: 181

```
Thanks. I left it up to @Martinsp to acquire the thermal pads.  You can find them on aliexpress, amazon, or from electronics components distributors like Digikey.
```

---
## \#356 Posted by: shaman Posted at: 2019-05-10T14:15:17.189Z Reads: 177

```
![TEK0000|640x480](upload://g0I0cz34F3TlAesdqwYNi7EYz2k.jpeg)

Switch Node @Vsupply = 54V 

Ok so I fired up the beta version in the lab. @54V there was only a spike of 55.6V at no-load. This is much better than the prototype and is most likely due to the improved layout.

The owner of the dyno I was using before is currently using it for his own tests. I won't be able to use it for a while. However, I'm sure this version performs better under load as well when it comes to voltage spikes.

12s is only 50.4V max so there is even more headroom for that scenario. That being said, still be cautious using 12s. Some of the beta testers are using 12s and I'll have feedback from them on performance after they're done testing.
```

---
## \#357 Posted by: b264 Posted at: 2019-05-10T19:23:55.732Z Reads: 170

```
I don't recommend it, but FYI a very few folks do run ESCs at 13S / 54.6V
```

---
## \#358 Posted by: linsus Posted at: 2019-05-10T20:21:09.489Z Reads: 166

```
If you want to quantify the distortion or noise bit better try to solder a coaxial to test point of intrest. Normal probes are really shite.

You'll prob need a BNC to SMA adapter tho
```

---
## \#359 Posted by: shaman Posted at: 2019-05-10T20:23:10.441Z Reads: 169

```
Yeah. I did do low inductance measurements but soldering a connector directly to the board would be better
```

---
## \#360 Posted by: MD84 Posted at: 2019-05-11T04:44:36.167Z Reads: 171

```
Thank you for all of the hard work. I will plan on making a couple for my next build. I take pride in building as much as I can myself and this diy will let me assemble the esc. Great job!

Looking forward to the testing.
```

---
## \#361 Posted by: Prism Posted at: 2019-05-11T15:28:49.300Z Reads: 162

```
@shaman, have you thought about adding some sort of silicone or glue to the THT capacitors to help with vibration stress on the solder joints?
```

---
## \#362 Posted by: shaman Posted at: 2019-05-11T15:30:54.483Z Reads: 159

```
Yeah I almost forgot about that. I know that's good practice for professional electronics. I'll most likely do that before I actually put one of these controllers in a rig of some kind. Thanks for the reminder!
```

---
## \#363 Posted by: doomy Posted at: 2019-05-12T12:40:00.814Z Reads: 159

```
I'm running my FSESC 4.12 on 13s (BLDC Mode), even do a full charge to 54.6 now and then..
So far, about 7 months and 400km its running great..

Most of my ebikes run at 14s tough, too bad thats not possible..
```

---
## \#364 Posted by: AlexBE Posted at: 2019-05-13T01:35:24.659Z Reads: 152

```
You don't need a dyno if you have multiple ESCS, you use one ESC as the load, the other as the driver.
```

---
## \#365 Posted by: shaman Posted at: 2019-05-13T03:00:22.122Z Reads: 154

```
Interesting. I'm not sure that replicates the inductive load that a motor is though. Got any details on how to do this?
```

---
## \#366 Posted by: b264 Posted at: 2019-05-13T03:25:51.651Z Reads: 166

```
[quote="AlexBE, post:364, topic:81344, full:true"]
You don’t need a dyno if you have multiple ESCS, you use one ESC as the load, the other as the driver.
[/quote]

This is genius.

[quote="shaman, post:365, topic:81344"]
Got any details on how to do this?
[/quote]

Two remotes, one on throttle and one on brake?
```

---
## \#367 Posted by: TowerCrisis Posted at: 2019-05-13T03:42:24.940Z Reads: 162

```
That only works if you've got them hooked up to eachother (on a bench). Riding it with them fighting eachother slightly (or regening your "tested" side) won't give you good data since you have to account for rider weight as well.

You'd be better off doing tests whilst carrying various weights.

The right way to do this is to setup a stationary dyno, using a vesc, that you can manually set the regen wattage to. This way it's easy to simulate exact weights and inclines. Programming an arduino could do this easily since you can just input rider weight, incline, and speed, and it would set the regen wattage appropriately.
```

---
## \#368 Posted by: b264 Posted at: 2019-05-13T03:43:38.611Z Reads: 151

```
Can't you just connect the motors to each other with a belt?
```

---
## \#369 Posted by: TowerCrisis Posted at: 2019-05-13T03:46:21.763Z Reads: 161

```
Yeah see my ninja edit :grin:

My interpretation of the test explained above me was that you'd just be riding with additional resistance or something.


Realistically, you would need a bigger motor to handle the resistance, or a reduction. That way you can get better low end torque readings, as the back EMF for regen is really low at slow speeds.
```

---
## \#370 Posted by: AlexBE Posted at: 2019-05-13T05:05:33.551Z Reads: 166

```
Sorry, I should have been more clear. You still use two motors, just connected together with a belt. It's also useful to include a heavy flywheel for more accurate acceleration testing. The very cool thing this allows you to do is calculate your efficiency. I've had this setup on my bench many times.

It also allows you to run very high powers, but with a small battery as the battery only needs to supply the difference between input and output "battery" currents.
```

---
## \#371 Posted by: shaman Posted at: 2019-05-13T12:50:54.078Z Reads: 164

```
Ah I see now. I'll keep this in mind for the future. Unfortunately I only have one non-hub motor to work with at the moment. It would be nice to have my own test equipment instead of someone else's dyno.
```

---
## \#372 Posted by: shaman Posted at: 2019-05-13T13:11:18.780Z Reads: 159

```
FYI I cleaned up the schematic and re-uploaded it to the GitHub. Hopefully it's easier to read now.
```

---
## \#373 Posted by: spork Posted at: 2019-05-14T03:07:39.527Z Reads: 155

```
This looks like a really great project.  I'd really like to build one myself if that's an option.  And here's the part I feel really guilty about...  is there somewhere I can see a summary of the project - what's available, what are the design choices, etc. - without reading all 370 comments on this thread?

Thanks.
```

---
## \#374 Posted by: Andy87 Posted at: 2019-05-14T03:43:58.230Z Reads: 157

```
[quote="spork, post:373, topic:81344"]
370 comments
[/quote]

Come on... just 370 not 3700 😂 that’s easy peasy 10min read time max. You can do it 💪
```

---
## \#375 Posted by: shaman Posted at: 2019-05-14T10:45:15.036Z Reads: 157

```
I know your pain. The Cheap FOCer is in beta testing. Things are looking good. The GitHub repository has the files needed to make one yourself. Note that the beta version isn't perfect and will have corrections implemented before the v1.0 release. Feel free to PM me specific questions you have
```

---
## \#376 Posted by: louwii Posted at: 2019-05-20T07:37:47.050Z Reads: 145

```
Finally had time to go through this topic. Thanks a lot @shaman for all your work, and the community that's helping him. I love projects like this one, seeing people getting together to get shit done is awesome. :+1:

I'll be following this closely. I'm considering trying to assemble one by hand with a soldering iron, just for the challenge. Might just be stupid though, I don't know...
```

---
## \#377 Posted by: janpom Posted at: 2019-05-20T10:19:44.475Z Reads: 144

```
It's not stupid at all. I want to do that too. A proper DIY board deserves a DIY VESC. :smile: BTW, I'm in the Cheap FOCer beta testing team and have already test ridden my board with the FOCers installed. The results are very impressive so far.
```

---
## \#378 Posted by: shaman Posted at: 2019-05-20T13:41:20.821Z Reads: 143

```
[quote="louwii, post:376, topic:81344"]
I’m considering trying to assemble one by hand with a soldering iron, just for the challenge
[/quote]

This is totally doable with fine solder wire, solder wick, and plenty of flux. The hardest part will be the STM32 and the DRV of which both have 0.5mm pitch leads. That's where the solder wick comes in to soak up excess solder and eliminate solder bridges.
```

---
## \#379 Posted by: janpom Posted at: 2019-05-20T13:51:07.967Z Reads: 141

```
@shaman If one was to assemble the FOCer "by hand", is it possible to do some sanity checks as you progress? I mean, it kind of sucks if you spend 4 hours soldering all the components, then you try to turn it on and... it doesn't work... or worse, you get the famous magic smoke. Is it somehow possible to solder on only a few parts; check that it's done correctly; then solder on more parts, etc?
```

---
## \#380 Posted by: shaman Posted at: 2019-05-20T15:33:50.140Z Reads: 150

```
It's hard to do functional checks as you go. The best is to do visual checks as you go and give close attention to the 0.5mm pitch parts under a microscope or magnifying glass. All the other components are relatively easy. 

You can do continuity checks with a multi-meter before powering up to make sure things have continuity where they should and don't have it where they shouldn't. One check would be for continuity from Vsupply to Ground before powering up. This can identify that a short to ground exists before powering up. You can do the same for the 5V and 3.3V rails.

I would also use a current-limited power supply if possible for the first power on. You can limit it to 100mA since the controller should only be drawing around 40mA in standby. This would then limit current if there is a short somewhere and hopefully prevent catastrophic damage.

Have spare STM32s or DRVs handy just in case they get burned up.

I know its a little daunting to try and hand solder something like this for the first time. But once you do, the feeling of success is awesome!
```

---
## \#381 Posted by: bradarad Posted at: 2019-05-20T18:40:41.373Z Reads: 148

```
Decided to try to build one of these myself. Got the boards in last Friday. I tried to get free samples through TI as a student, but they turned me down. So now I'm waiting on a few more parts.
![IMG_20190520_123400|375x500](upload://fVYqNZ8nuQ2czyfux3Ckz89u6NK.jpeg)
```

---
## \#382 Posted by: shaman Posted at: 2019-05-20T18:46:00.258Z Reads: 142

```
Awesome! This is exactly what I designed this for. Good luck on your DIY adventure with this!
```

---
## \#383 Posted by: gmurad Posted at: 2019-05-20T18:51:08.072Z Reads: 141

```
If you do this you should make a video soldering it like you did with the DaveGA, that was really helpful for me who doesn't have much soldering experience.
```

---
## \#384 Posted by: bradarad Posted at: 2019-05-20T19:01:57.172Z Reads: 146

```
You did all the legwork and I am super thankful for that.

Did you say there is a problem with 5v somewhere? I have no problems cutting traces and adding jumper wires if needed.
```

---
## \#385 Posted by: bradarad Posted at: 2019-05-20T19:02:54.217Z Reads: 147

```
I might be able to post a soldering vid when I get all of the components in. It probably won't be for a couple of weeks.
```

---
## \#386 Posted by: diedirk Posted at: 2019-05-20T19:31:19.482Z Reads: 147

```
turned me down as well when I asked why they just closed the request :cry:
```

---
## \#387 Posted by: shaman Posted at: 2019-05-20T19:31:46.998Z Reads: 151

```
[quote="bradarad, post:384, topic:81344"]
Did you say there is a problem with 5v somewhere?
[/quote]

Yes. Pin 2 of SERVO header is not connected to 5V. I'm keeping a list of the issues with the Beta version on the GitHub page.
```

---
## \#388 Posted by: janpom Posted at: 2019-05-20T19:40:53.114Z Reads: 153

```
Thanks for putting your trust in me. :) This is a bit above my league though. I can make a video of me struggling to get it soldered. It would be very entertaining and people would learn a lot from my mistakes. :laughing:

Hopefully @bradarad will be able to make a more serious video. I'd be one of the first ones to watch it.
```

---
## \#389 Posted by: Andy87 Posted at: 2019-05-20T19:58:29.731Z Reads: 153

```
@janpom looking forward to your videos...imagine that kind of format 😌😜

 https://youtu.be/Tq-EpR-8R0w
```

---
## \#390 Posted by: district9prawn Posted at: 2019-05-21T02:03:35.909Z Reads: 153

```
On the vesc boards I've assembled my checklist before powering on involves:

Supply rail shorts to ground

Mosfet drain source shorts

Mosfet gate source shorts

Look for cold solder joints on the gate driver outputs.

Reason for the gate output check is that I've found a floating gate trace can result in false mosfet switching events. Which means shoot through fault.

On the a200s 18 fet boards I've been making I also check gate capacitance to make sure all mosfets are actually connected.

And of course for first power up use a current limited supply at low voltage, not battery.
```

---
## \#391 Posted by: Benjamin899 Posted at: 2019-05-21T11:35:23.672Z Reads: 142

```
Yeah TI turned me down too, i even just asked for drv. Fuck em, just gonna buy it elsewhere
```

---
## \#392 Posted by: b264 Posted at: 2019-05-21T15:41:27.979Z Reads: 143

```
You're cursing them because they're not in business to give you free shit?
```

---
## \#393 Posted by: spork Posted at: 2019-05-25T22:48:44.189Z Reads: 138

```
>>  I’m considering trying to assemble one by hand with a soldering iron

I would think the only tricky part would be soldering the pad on the bottom of the DRV (and maybe the MCU?).  Unless there's a hole through the board for that purpose.
```

---
## \#394 Posted by: spork Posted at: 2019-05-25T22:56:03.686Z Reads: 138

```
>>  just gonna buy it elsewhere

$6.08 with free 1-day shipping.  Can't be beat!

https://www.arrow.com/en/products/drv8302dca/texas-instruments
```

---
## \#395 Posted by: shaman Posted at: 2019-05-26T00:21:04.255Z Reads: 134

```
The DRV footprint on the PCB does have vias in the thermal pad. One can actually apply solder through the vias on the backside.
```

---
## \#396 Posted by: b264 Posted at: 2019-05-26T01:14:17.118Z Reads: 137

```
A large via under the DRV ground pad is such a good idea. @shaman any way to enlarge the hole on the next version?
```

---
## \#397 Posted by: shaman Posted at: 2019-05-26T01:58:09.777Z Reads: 136

```
Currently the pad has an array of 0.3mm vias. I can enlarge them to 0.4mm or 0.5mm no problem.
```

---
## \#398 Posted by: b264 Posted at: 2019-05-26T04:17:39.169Z Reads: 137

```
I was thinking more like 4.0mm.
```

---
## \#399 Posted by: louwii Posted at: 2019-05-27T01:02:23.503Z Reads: 131

```
Wait, that means the DRV is supposed to be soldered to the pad with the 3x5 vias? I thought this was only for cooling or something.
```

---
## \#400 Posted by: TowerCrisis Posted at: 2019-05-27T01:14:51.036Z Reads: 130

```
Pretty sure it's just good practice to use grounding pads when given them, even if it's not technically necessary due to redundant ground pins and manageable thermals.
```

---
## \#401 Posted by: louwii Posted at: 2019-05-27T01:34:33.195Z Reads: 128

```
Got it. I looked at pictures of a DRV, I had no idea chips could have a soldering pad under them. Looks like I learned something today.
```

---
## \#402 Posted by: shaman Posted at: 2019-05-27T13:02:30.439Z Reads: 126

```
So the multiple small vias are better for thermal management. Personally I didn't have an issue in getting solder to wick through vias from the backside. I used leaded solder (best tasting kind) and plenty of flux.
```

---
## \#403 Posted by: shaman Posted at: 2019-05-27T13:04:11.939Z Reads: 131

```
[quote="louwii, post:399, topic:81344"]
Wait, that means the DRV is supposed to be soldered to the pad with the 3x5 vias?
[/quote]

Yes. One must solder this pad. This is mandatory in order to keep the DRV cool during operation and provide a strong connection to ground.
```

---
## \#404 Posted by: louwii Posted at: 2019-05-28T23:55:08.193Z Reads: 128

```
Got it. It seems impossible to solder by hand as it is now though. Now I understand why @b264 was mentioning putting bigger vias there. Because right now this seems too small to make solder flow through them?

EDIT: just saw your post above. It is do-able then. Interesting. Now I'm even more curious to try.
```

---
## \#405 Posted by: b264 Posted at: 2019-05-29T00:37:42.046Z Reads: 129

```
I wonder why not make a via over *almost* the entire bottom pad.  If you need to remove heat from the pad, just flow solder over it.

At least then it's much easier to solder and desolder with rudimentary tools.
```

---
## \#406 Posted by: shaman Posted at: 2019-05-29T00:43:09.778Z Reads: 133

```
Well you're not wrong. Generally the technique of adding several small vias for thermal management is to facilitate easier reflowing in manufacturing. But being that this is for the DIY community, adding a large through hole pad underneath would most likely do the trick. I'll add this to the list of changes to be conducted for the full release of this controller. Keep up the good suggestions!
```

---
## \#407 Posted by: doomy Posted at: 2019-05-29T10:59:31.726Z Reads: 126

```
Just ordered all the parts to assemble 5  of those cheap FOCers!

Here is what i got:

https://www.aliexpress.com/item/5-PCS-LOT-STM32F405RGT6-32F405RGT6-LQFP64-NEW/32961183726.html?spm=a2g0s.9042311.0.0.df354c4dsblNwB

https://www.aliexpress.com/item/10PCS-lot-DRV8302-DRV8302DCAR-HTSSOP56-IC-Chip-New-Original/33022829247.html?spm=a2g0s.8937460.0.0.5b872e0et5Ob5O

5 PCBs in black from jlcpcb 2$

rest of the components from LCSC 58$ without shipping

That makes a little bit over 100$ for 5 pieces..
```

---
## \#409 Posted by: shaman Posted at: 2019-05-29T12:22:22.451Z Reads: 122

```
So FOCing cheap!
```

---
## \#410 Posted by: Benjamin899 Posted at: 2019-05-29T14:10:56.724Z Reads: 121

```
where is difference between the DRV8302DCA and DCAR?
```

---
## \#411 Posted by: Snehith Posted at: 2019-05-29T14:16:33.850Z Reads: 115

```
it's just some difference in reel packing i 
think
```

---
## \#412 Posted by: Benjamin899 Posted at: 2019-05-29T14:18:42.445Z Reads: 115

```
ok good to know.
```

---
## \#413 Posted by: doomy Posted at: 2019-05-30T05:57:25.280Z Reads: 115

```
Here is the LCSC BOM for 5 pieces (without DRV and STM chip):

I also had to switch the main smoothing capacitors(16x20) for 16x25mm ones because there were none available. It will probably not fit into a case anymore.

https://www.dropbox.com/s/69snb2ovnku5crm/LCSC_Exported_20190530_135126.xlsx?dl=0

Talking of cases, does anyone have a link for these hammond / ebike controller boxes?
```

---
## \#414 Posted by: shaman Posted at: 2019-05-30T11:41:23.796Z Reads: 114

```
The taller capacitors will make the controller too tall for the Hammond 1590b that I've mentioned before. However, it would still most likely fit in a Hammond 1590n1 enclosure. The generic version of that is the 125b which can be found on aliexpress.

https://www.aliexpress.com/item/32955592415.html?spm=2114.search0604.3.2.62344031WzxyWu&amp;ws_ab_test=searchweb0_0%2Csearchweb201602_6_10065_10130_10068_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_10618_10307_537_536_10059_10884_10887_321_322_10103%2Csearchweb201603_53%2CppcSwitch_0&amp;algo_expid=909c4b78-9735-4766-baa8-670c3214b1e7-0&amp;algo_pvid=909c4b78-9735-4766-baa8-670c3214b1e7
```

---
## \#415 Posted by: doomy Posted at: 2019-05-30T12:22:34.799Z Reads: 113

```
Cool thanks, i will probably change them for the 16x20mm caps once the controller is working and they are available again..

Is the board supposed to be attatched to the enclosure trough the top left and bottom right hole and the mosfet cooling pads? 

Il probably need some kind of spacers, right?
```

---
## \#416 Posted by: shaman Posted at: 2019-05-30T12:45:53.820Z Reads: 115

```
![image|666x500](upload://iGDmOTcQV35tbvJpILoViPmCQmh.jpeg) 

I've been meaning to show this for a while but I haven't had the time. The way I had in mind was to couple an aluminum bar to the MOSFETs and then attach that bar to the inner wall of the enclosure. One can simply drill some of the MOSFET mounting holes through the aluminum bar and the enclosure wall and just use longer screws to mount it all together. I hope that makes sense. I need actually do it and show pictures sometime soon...

The cables are intended to come out through the sides through cable glands like these.
![image|225x225](upload://eRMdAnjYmRy8PeazkLzyqU1DAK2.png)
```

---
## \#417 Posted by: shaman Posted at: 2019-05-30T12:51:14.283Z Reads: 113

```
Be sure to use a bit of thermal grease between the bar and the inner wall of the enclosure. The whole point is make the enclosure part of the heatsink for max cooling.
```

---
## \#418 Posted by: doomy Posted at: 2019-05-30T12:57:58.771Z Reads: 116

```
Looks good, and it will be watertight too if using some rubber washers on the outside screws..

Whats the thickness of the aluminium bar?

Is the bottom left hole next to the capacitor useable to attatch the esc?
```

---
## \#419 Posted by: shaman Posted at: 2019-05-30T13:12:27.295Z Reads: 122

```
![image|666x500](upload://Ss8kwaT1OyBKC4HgSLuFC3O2wl.jpeg) 

For good water resistance you will also need to get the gaskets and rubber O-rings that fit the 1590b enclosure. Rubber washers can be used on the outside screws as well.

The aluminum bar needs to be 6mm thick. It can be a bit thicker but not too much.

You can use that hole by the capacitor if you want but I don't think it's necessary if you mount it in the way I have said.
```

---
## \#420 Posted by: DjamboBuksne Posted at: 2019-05-30T14:49:20.080Z Reads: 113

```
Does somebody sell them?
```

---
## \#421 Posted by: shaman Posted at: 2019-05-30T15:00:51.413Z Reads: 110

```
Not yet. I'm most likely going to do a group buy for these after beta testing and after I apply changes to the design.
```

---
## \#422 Posted by: Benjamin899 Posted at: 2019-05-30T18:55:32.990Z Reads: 110

```
the changes are concering only the pcb atm, right? Basicly quality of life for soldering. Or did i get that wrong.
LoLz, all 16mm Caps are sold out
```

---
## \#423 Posted by: kalebludlow Posted at: 2019-05-30T20:25:10.908Z Reads: 107

```
Hey @shaman not sure if you've done it yet but you should make a thread for this over at forum.
```

---
## \#424 Posted by: shaman Posted at: 2019-05-30T21:53:48.553Z Reads: 104

```
Yep. Just minor changes to the PCB. Fixing the CAN transceiver power to be 5V, fixing the "SERVO" pin header to have 5V at pin 2, and putting a large through-hole pad underneath the DRV to allow easy soldering to the thermal pad with a standard soldering iron 

You guys may have to source the large caps from somewhere besides LCSC if they stay out of stock. They just need to be the same physical size, same capacitance, and be low-impedance
```

---
## \#425 Posted by: shaman Posted at: 2019-05-30T21:55:14.370Z Reads: 103

```
Yes I need to do that. I'll be looking for a way to do that gracefully. I'll be announcing what I do in those regards in this thread.
```

---
## \#426 Posted by: Benjamin899 Posted at: 2019-05-30T22:14:56.969Z Reads: 104

```
there are also other parts missing on lcsc, can we take similar products with the same values given in the bom? 
For example this item https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_220KR-2203-1_C139903.html instead of originally this https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_220KR-2203-1_C101567.html. 
Whats interesting is that most items have many similar products but the price range is huge.
```

---
## \#427 Posted by: shaman Posted at: 2019-05-30T23:09:55.841Z Reads: 104

```
For all the passive components, it doesn't matter. The replacements just need to have the same attributes. Yes there can be a significant price difference for some reason. However in my experience, a 1K, 0805, 1% resistor does not vary much from manufacturer to manufacturer. Same for ceramic caps.
```

---
## \#428 Posted by: doomy Posted at: 2019-05-31T10:32:09.621Z Reads: 94

```
Will the CAN module still work with 3.3V or do i have to cut the trace and solder a jumper wire?
```

---
## \#429 Posted by: shaman Posted at: 2019-05-31T12:13:53.156Z Reads: 97

```
When did you get the Gerbers from the GitHub? The current Gerber files have the CAN issue fixed and the CAN transceiver is powered from 5V
```

---
## \#430 Posted by: doomy Posted at: 2019-05-31T13:36:05.447Z Reads: 94

```
Ah thats good news. Downloaded them only 3 days ago (28. May). I did not know the changes were already implemented. Thanks!
```

---
## \#431 Posted by: shaman Posted at: 2019-05-31T14:02:30.075Z Reads: 94

```
Only the CAN issue has been fixed for the Gerbers in the GitHub. The rest will be fixed after I'm done receiving feedback from the beta testers
```

---
## \#432 Posted by: doomy Posted at: 2019-05-31T14:07:56.312Z Reads: 96

```
Suits me, the can bus is the most important. I wont use the servo port and if i would its an easy fix.

Do you have any updates on motor amp capabilities?
```

---
## \#433 Posted by: shaman Posted at: 2019-05-31T14:17:17.329Z Reads: 97

```
@janpom used a motor current limit of 60amps and the controller didn't get over 50C while putting it through some serious hills. That's just with an aluminum bar as a heatsink with no airflow.
```

---
## \#434 Posted by: janpom Posted at: 2019-05-31T14:33:22.953Z Reads: 116

```
That's right. Here's the Metr log from one of my test rides:
https://metr.at/r/4zLRS
```

---
## \#435 Posted by: shaman Posted at: 2019-05-31T17:45:06.383Z Reads: 114

```
Alright everyone. I've made a new thread in the esk8 news forum. Please redirect your attention over there if possible. The new thread is where I'll be posting updates, answering questions, and receiving suggestions. 

I am not actively deleting this thread on the esk8 builders forum. It will remain as a reference for all as long as it exists.

https://forum./t/cheap-focer-vesc-compatible-4-12-redesign/1510
```

---
## \#436 Posted by: ChristianT Posted at: 2019-07-12T14:12:29.538Z Reads: 65

```
only the bom of the vesc 6 are 60$-? from where did u get that number? 

(would appreciate an answer, thanks already ;))
```

---
## \#437 Posted by: moon Posted at: 2019-07-12T14:23:42.879Z Reads: 65

```
I got it from adding the value of the components..
```

---
## \#438 Posted by: shaman Posted at: 2019-12-02T00:11:39.302Z Reads: 28

```
https://forum./t/cheap-focer-2-open-source-low-cost-vesc-6-based-esc-prototyped-ordered-materials-for-test-batch/13631

Figured I'd just slip this in over here...
```

---
## \#439 Posted by: esk8me Posted at: 2019-12-02T02:00:39.431Z Reads: 28

```
Sent my money.. Hopefully this works out fine.
```

---
