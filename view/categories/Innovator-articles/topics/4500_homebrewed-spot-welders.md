# Homebrewed spot welders

### Replies: 150 Views: 12889

## \#1 Posted by: monkey32 Posted at: 2016-06-10T02:54:57.230Z Reads: 653

```
I have come to the point where I feel my power sources are the weak link on my boards. I figure it is about time for an upgrade, I currently run 7s2p limited to 20amp which is more timid than the 10s lipo I ran earlierbut lipo chem makes me nervous  me in my inner city apt. so why not build my own 10-12 s pack??

Well cells are getting cheap, but typical spot welders are running near the cost of a pack to build, plus i want to understand how these work and control some variables which are not as precise with Sunkko welders - the most used alternative.

Reading about welders on and off I found two viable options
1- Whitepony has a home brewed version with a 2Farad Super Capasitor, copper bar switch, and car battery charger.
2. On instructables I found a Ardruino based Mofet driven pcb that is solder up and play using a car battery for power. 

I'm gonna build/ write up both and compare....you know, for science.

DIY is a lifestyle I'm finding - so much cooler to learn and understand how this and other tech work.

Anyway here is the start....


<img src="/uploads/db1493/original/2X/9/91d60fd454949e8c3b690484fb914162ffb25b53.jpg" width="674" height="500">
```

---
## \#2 Posted by: lox897 Posted at: 2016-06-10T04:21:14.532Z Reads: 592

```
I'm building the exact same Arduino Spot Welder. This is my first time soldering through-hole. Make sure you get the correct number display. The old BOM had the wrong display and it didn't work. Read the comments of the arduino spot welder and you will see the guy I am talking about who had the problem.
```

---
## \#3 Posted by: akira Posted at: 2016-06-10T05:44:18.113Z Reads: 587

```
Hi lox, 
I am also building the same spot welder. I found a mismatch between the numbers on the pcb and the bom. The small capacitor in parallel with the radial 1uF is 100pF in the BOM and 100nF on the pcb.
Is that the problem you re referring to or is it something else ?

Cheers
Akira
```

---
## \#4 Posted by: lox897 Posted at: 2016-06-10T05:54:01.806Z Reads: 548

```
No. I was referring to the common cathode display. I have never heard about a problem with the caps.
```

---
## \#5 Posted by: akira Posted at: 2016-06-10T07:49:47.137Z Reads: 537

```
Thanks for the warning, 
After checking, I used the corrected BOM.
```

---
## \#6 Posted by: lox897 Posted at: 2016-06-10T07:53:29.780Z Reads: 512

```
I've got the wrong display. I'll have to order one off of Ebay.
```

---
## \#7 Posted by: Krudte Posted at: 2016-06-10T10:54:13.718Z Reads: 512

```
Whould love to do the instructable one, do you or @lox897 have an extra pcb I could buy?
```

---
## \#8 Posted by: lox897 Posted at: 2016-06-10T12:14:31.221Z Reads: 513

```
Yeah. I have 9 more. $3.50 AUD + shipping. That is the money I have to charge because other wise I will lose money. Are you in the US?
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-06-10T13:21:31.832Z Reads: 489

```
i kind of love my Sunkko, but this thread is amazing. I'm excited to see people building thier own tools.
```

---
## \#10 Posted by: monkey32 Posted at: 2016-06-10T14:26:52.138Z Reads: 483

```
how much to ship to madrid spain??
```

---
## \#11 Posted by: Krudte Posted at: 2016-06-10T14:32:04.874Z Reads: 475

```
In Denmark, so shipping might be high....  Any idea what it would cost to ship?
```

---
## \#12 Posted by: monkey32 Posted at: 2016-06-10T17:02:15.860Z Reads: 460

```
I may just order 10 and sell them at cost plus shipping if there are enough euro peeps
```

---
## \#13 Posted by: lox897 Posted at: 2016-06-10T20:08:18.643Z Reads: 445

```
$2.75 for an envelope and $21.56 for a parcel.
```

---
## \#14 Posted by: lox897 Posted at: 2016-06-10T20:47:56.514Z Reads: 455

```
To ship to Madrid $2.75 for envelope and $21.48 for package. This is the cheapest price. It will take about 9 days to get to you.
```

---
## \#15 Posted by: lox897 Posted at: 2016-06-10T20:48:13.807Z Reads: 446

```
All prices in AUD.
```

---
## \#16 Posted by: lox897 Posted at: 2016-06-10T21:09:33.307Z Reads: 469

```
The people that made my PCBs couldn't do the vcut. Their machine wont accept pcbs that small or something. I am just going to score it with a stanley knife and then snap it to separate the two boards.
```

---
## \#17 Posted by: squad Posted at: 2016-06-10T23:49:06.510Z Reads: 491

```
What a coincidence, as a matter of fact, today I made most of my DIY spotwelder :smiley:
It's based on rewired microwave transformer, nothing fancy, I'll use bought timing circuit made for that application. Here are pics:

http://i.imgur.com/PIGhWDB.jpg
Inside of spotwelder, only part missing is timing circuitboard.

http://i.imgur.com/CHM7fGQ.jpg
I turned electrodes on a lathe

http://i.imgur.com/UV0kO1W.jpg
...and also custom connectors

http://i.imgur.com/wyrw9KO.jpg

http://i.imgur.com/upOgr48.jpg
```

---
## \#18 Posted by: Michaelinvegas Posted at: 2016-06-23T07:36:39.406Z Reads: 460

```
https://youtu.be/UU7QC5Uby6M
```

---
## \#19 Posted by: Maxid Posted at: 2016-06-23T08:09:09.444Z Reads: 460

```
who doesn't want to remove the insulation plus have all the current travel through so much of the battery :confused:
```

---
## \#20 Posted by: Michaelinvegas Posted at: 2016-06-23T08:51:23.182Z Reads: 456

```
Lol agreed lol
```

---
## \#21 Posted by: Michaelinvegas Posted at: 2016-06-23T08:54:11.169Z Reads: 448

```
https://youtu.be/Gk3vrKc4Y1w

I posted this some place else...I guess I thought I posted here...

This seems a bit better
```

---
## \#22 Posted by: monkey32 Posted at: 2016-06-23T09:43:03.849Z Reads: 431

```
I'd grab 3 of those pcbs if you still got em. Pm me your info and price.
```

---
## \#23 Posted by: Nordle Posted at: 2016-06-23T10:07:58.265Z Reads: 427

```
[CD Welder](http://ledhacks.com/power/battery_tab_welder.htm) I like this, it's like your's but instead of the pcb just uses a big rectifier.
Do you think it will work well? From what I remember @whitepony is using something similar?
```

---
## \#24 Posted by: monkey32 Posted at: 2016-06-23T12:28:05.973Z Reads: 431

```
So still playing with some free time but hitting the pool today so just a few shots....

Sanded down copper rods for  electrodes so they have tips fine enough to fuse the nickle.

<img src="/uploads/db1493/original/2X/f/f2a87ee28f87637aa52a6e0e7a0d0abbccda762c.jpg" width="674" height="500">
```

---
## \#25 Posted by: akira Posted at: 2016-06-23T14:00:12.978Z Reads: 412

```
What diameter do you use for the copper rods ?
I have finished the instructable arduino version but I am still wondering how big I should go with the soldering tips ...
```

---
## \#26 Posted by: mason Posted at: 2016-06-23T14:12:24.109Z Reads: 401

```
this is extremely dangerous.
```

---
## \#27 Posted by: Nordle Posted at: 2016-06-23T14:35:50.906Z Reads: 395

```
or, how to blow up a car battery :D
```

---
## \#28 Posted by: akira Posted at: 2016-06-23T16:43:25.879Z Reads: 403

```
Can you elaborate on that ? Do you have arguments / bad experience with this setup ?
JP Spot welder (also a battery welder) is used by many people. I have not heard of such an accident.

I plan to put a 200A slow fuse is serie with the spot welder. 
What can possibly happen then ?
```

---
## \#29 Posted by: Karmannghiagirl Posted at: 2016-06-23T16:45:33.944Z Reads: 397

```
That's just shorting out the battery, which is not great. it also has no safety mechanisms so if something metal shorts the contacts and welds on, you're fucked.
```

---
## \#30 Posted by: akira Posted at: 2016-06-23T16:56:11.549Z Reads: 385

```
If I have a 200A fuse in serial, a short will just blow the fuse, I guess, right ?
I do not see the very high danger ... but I'd be happy to hear your view on this.
```

---
## \#31 Posted by: Karmannghiagirl Posted at: 2016-06-23T16:59:32.996Z Reads: 379

```
even with the fuse, you are shorting out a battery. thats how it makes the heat required to spot weld. but when you short out a battery it damages it. it might work for awhile but over time it will degrade and fail at some point, possibly in a dangerous way.  The spot welders that use transformers are going to be the best, but i would but capacitor based ones right behind them, and then battery ones if you have no other option.

90% of the time its going to be perfectly fine to use a battery one, but that 10% can be dangerous.
```

---
## \#32 Posted by: akira Posted at: 2016-06-23T17:11:36.535Z Reads: 392

```
I see, thanks for the explanations.
Well, I do not plan to use mine for more than a couple hundreds of batteries. 
That should do.

If I go for a larger amount, I'll probably consider building this one 
http://www.avdweb.nl/arduino/hardware-interfacing/spot-welder-controller.html
```

---
## \#33 Posted by: Michaelinvegas Posted at: 2016-06-23T18:40:53.034Z Reads: 385

```
Honestly ... It's good for a couple of spot welds....but not a true solution to replace the real thing
```

---
## \#34 Posted by: longhairedboy Posted at: 2016-06-23T18:53:49.541Z Reads: 406

```
[quote="akira, post:28, topic:4500"]
What can possibly happen then
[/quote]

never EVER ask that question out loud where lithium and extreme current is a factor. Skatan will show you "what could possibly happen then." DOOM. CHAOS. THE BURNING TIMES. 

Also i've seen them built with those huge car stereo supercaps and they seem to work well with those too. I do enjoy seeing this kind of thing done. Ultimately i ended up buying a sunkko but i was originally planning to build my own.  What kind of thickness can you weld with something like this?
```

---
## \#35 Posted by: squad Posted at: 2016-06-23T21:45:25.866Z Reads: 406

```
Today I finished my spot welder. Here are results, I'm pretty happy with it, and it was waaaay cheaper than cheapest option on aliexpress.

http://imgur.com/fkrbdq8

https://www.youtube.com/watch?v=brkA9j_55J0&feature=youtu.be
```

---
## \#36 Posted by: Michaelinvegas Posted at: 2016-06-23T22:49:01.352Z Reads: 399

```
I agree it's dangerous ...but a momentary switch can resolve the issue of the contacts welding accidentally to the piece you are welding
```

---
## \#37 Posted by: lox897 Posted at: 2016-06-24T00:39:14.243Z Reads: 389

```
The arduino spot welder has a foot switch. I am pretty confident that stops one of the electrodes welding unless you push the switch.
```

---
## \#38 Posted by: Karmannghiagirl Posted at: 2016-06-24T00:46:06.709Z Reads: 389

```
you would have to use a relay, but yea that would increase the safety factor by a lot.
```

---
## \#39 Posted by: Michaelinvegas Posted at: 2016-06-24T00:47:12.488Z Reads: 387

```
Oh and running a long line away from the battery lol like outside lol
```

---
## \#40 Posted by: emepror Posted at: 2016-06-25T01:54:09.193Z Reads: 413

```
I'm ordering all the parts needed for an arduino spot welder. Once I'm done, I can post a mouser order list and update once I build it. Going to be welding a 10S4P battery for my new board. I ordered the PCB's through Bay Area Circuits.
```

---
## \#41 Posted by: kovjanos Posted at: 2016-08-11T11:24:24.175Z Reads: 395

```
Hi,

I have 8 packs of:
  - PCB
  - Foot switch
  - Arduino
to build this: http://www.instructables.com/id/DIY-Arduino-Battery-Spot-Welder/?ALLSTEPS

PCB printed by PCBWay, latest design (13Jun2016), single piece to be cut.
Foot switch from kEK, 10 x 6 x 3.5 cm.
Arduino Nano v3 (ATMEGA328P-AU, CH340) in antistatic bag.

13 EUR + shipping from .HU 

Let me know if you are interested!

R, J.

<img src="/uploads/db1493/original/2X/8/891cbb57ff3c603c6fc3b0530109def2f7005f24.jpg" width="690" height="388">
```

---
## \#42 Posted by: Tarzan Posted at: 2016-08-11T11:47:18.314Z Reads: 371

```
@kovjanos 
Make a Pack with all necessary components and I'm in!
```

---
## \#43 Posted by: kovjanos Posted at: 2016-08-11T11:56:41.634Z Reads: 371

```
Hi @Tarzan,

I checked but:

* cable and battery terminal set are heavy, more than 2x heavier than the 3 components. In local stores they are cheaper plus you have to select the terminal based on the car battery you use.
* electronic components can be easily ordered in 1 pack with 1 click from .DE - and the price is almost the best: https://secure.reichelt.de/index.html?&ACTION=20&AWKID=1203408&PROVID=2084

R, J.
```

---
## \#44 Posted by: Maxid Posted at: 2016-08-11T11:57:08.231Z Reads: 358

```
there is a reichelt shopping card link - just order it yourself and you are good.
https://secure.reichelt.de/index.html?&ACTION=20&AWKID=1203408&PROVID=2084
(Ok you need to also buy cables and a car battery)

Edit: @kovjanos was 10 microseconds faster :smiley:
```

---
## \#45 Posted by: DeathCookies Posted at: 2016-08-11T12:18:32.677Z Reads: 353

```
[quote="kovjanos, post:43, topic:4500"]
plus you have to select the terminal based on the car battery you use.* electronic components can be easily ordered in 1 pack with 1 click from .DE - and the price is almost the best: https://secure.reichelt.de/index.html?&ACTION=20&AWKID=1203408&PROVID=2084
[/quote]

Your three parts + link from reichelt + (additionally) car battery = complete spotwelder?
The terminal must match the battery. Which/What terminal?
Does i am missing something?
```

---
## \#46 Posted by: Maxid Posted at: 2016-08-11T12:27:36.318Z Reads: 338

```
you also need cables and electrodes.
with the terminal I think he means something like this:
https://www.hornbach.de/shop/Presskabelschuh-16-x-10-5/4046168/artikel.html
which is for the connection to the battery
```

---
## \#47 Posted by: kovjanos Posted at: 2016-08-11T12:27:57.754Z Reads: 361

```
Hi @DeathCookies,

You will also need:

* some cables - thin for powering the board and connecting the foot switch and thick for welding.
* something to mount the thick cable to the battery, e.g. terminal set

E.g. 1m of 1G10 cable plus a pair of small terminal set that fits on my battery.

R, J.
<img src="/uploads/db1493/original/2X/9/908da9025b493e8c220a8f499ef4397261250b0a.jpg" width="690" height="388">
```

---
## \#48 Posted by: lox897 Posted at: 2016-08-11T12:42:16.541Z Reads: 333

```
What did you use for electrodes?
```

---
## \#49 Posted by: Maxid Posted at: 2016-08-11T12:47:01.434Z Reads: 329

```
I think they usually just use a piece of 10mm² solid copper wire and remove the insulation.
```

---
## \#50 Posted by: kovjanos Posted at: 2016-08-11T12:47:38.125Z Reads: 326

```
Similar size but solid copper wire. 
Just find a friendly guy in the shop and agree to pay extra 20cm of the welding wire but have the 20cm from the solid wire. This is good if minimal length to buy would be 1m... If you are lucky you will get it for free :) 

R, J.
```

---
## \#51 Posted by: Tarzan Posted at: 2016-08-11T13:43:51.354Z Reads: 311

```
Awesome guys!
I ordered the parts from reichelt.de now I need your three parts.
Shipping to Germany is okay I hope :smiley:
PM me your Paypal and you have a customer.
```

---
## \#52 Posted by: DeathCookies Posted at: 2016-08-11T13:44:39.586Z Reads: 305

```
Lets buy together to save some shipping costs? i believe you live in hagen? I am from muenster so we could arrange something?
```

---
## \#53 Posted by: Tarzan Posted at: 2016-08-11T13:45:51.682Z Reads: 305

```
If we save some € of course!
Unfortunately I have ordered the parts from Reichelt 4 min ago. 5,50 € Shipping :frowning:
```

---
## \#54 Posted by: Maxid Posted at: 2016-08-11T13:53:08.207Z Reads: 302

```
Can't you cancel the order? Shouldn't be a problem so close to the time of order.
```

---
## \#55 Posted by: kovjanos Posted at: 2016-08-11T13:55:08.331Z Reads: 306

```
@DeathCookies and @Tarzan: should I pack 2 sets of the 3 components into one box? 
That would really save some EUR for you if you chose DPD or GLS but as a standard post parcel it would save only ~2EUR (~8 instead of 2x ~5) as one pack is ~160g and the limit is 250g but the two packs would fit only into the 500g limit...

R, J.
```

---
## \#56 Posted by: Tarzan Posted at: 2016-08-11T14:10:36.835Z Reads: 303

```
@Maxid
I wrote an email to Reichelt that I like to cancel my order.
We'll see how that turns out.
All in all the savings aren't that high and how do you plan to exchange the goods? Sending it in a package is more expensive and a drive by car as well!
@kovjanos
We'll buy two, but give us some time to figure out how we do it.
I'm not sure if it's worth it to pack it in one package.
```

---
## \#57 Posted by: DeathCookies Posted at: 2016-08-11T14:18:47.597Z Reads: 303

```
Well you are right. it does not matter because the shipping cost is only 5€ to germany.
(He have to check if it has insurance because he had bad experiences with it when the shipping company lost some parcels...)
It would only make a difference if we would ship it by dpd or ghs 18-22€. 

The shipping cost in germany would be only 4€ (Hermes Päckchen).
```

---
## \#58 Posted by: DeathCookies Posted at: 2016-08-11T14:58:44.788Z Reads: 317

```
@Tarzan 8€ for registered mail and if we buy together it would be 11€

Calculation:
Together:
11€ to germany
5,50€ from reichelt
4€ to me
= 20,50 / 10,25 each

Alone:
8€ to germany
5,50 from reichelt
= 13,50 each

Well that would save 3,25€ :joy:
With that calculation i dont mind if we buy it together or not. But if somebody else wanna chime in it would make sense.
```

---
## \#59 Posted by: Tarzan Posted at: 2016-08-11T20:48:02.894Z Reads: 303

```
Maybe we wait for the weekend and the answer of reichelt.
So is somebody in Germany interested in a cheap spotwelder kit?
@whitepony @HH1 @E-Boarding @hexakopter  @flatsp0t to name some
I could add terminals, wires and mashined electrodes if you are interested.
```

---
## \#60 Posted by: whitepony Posted at: 2016-08-11T20:52:31.193Z Reads: 299

```
my stone age version works too well to swap it for something else, but I really like this arduino based spot welder. have fun fiddling it together :slight_smile:
```

---
## \#61 Posted by: Tarzan Posted at: 2016-08-11T20:59:43.486Z Reads: 273

```
Have thought about building a sotwelder like yours so many times, because it seems to work well.
This arduino one looks like a fun project and totally doable. The costs are okay and if I fuck up I can live with it 😄
```

---
## \#62 Posted by: Maxid Posted at: 2016-08-11T21:31:54.969Z Reads: 264

```
I already ordered the reichelt parts. They also have battery terminals for like 2,5€ :thumbsup:
```

---
## \#63 Posted by: Maxid Posted at: 2016-08-17T08:44:39.530Z Reads: 261

```
Do you still have a pack? I would need one sent to Germany.
```

---
## \#64 Posted by: lox897 Posted at: 2016-08-17T10:34:55.614Z Reads: 263

```
I'm soldering some of the components to the PCB this weekend. I will post some pics.
```

---
## \#65 Posted by: lox897 Posted at: 2016-08-20T08:55:56.306Z Reads: 260

```
@kovjanos How did you get the potentiometer in? Mine doesn't fit.
```

---
## \#66 Posted by: Okami Posted at: 2016-08-21T19:40:34.598Z Reads: 279

```
How much you spent on mosfets and other little parts?

I might join in, if you dont run out of pcb's that soon.. Although, I have my own 5v arduino nano, so I would only need the pcb and perhaps footswitch, if the switch  I found in a  microwave does not fit nicely.

---
Although I am still a bit unsure of the spot welder idea.. especially, because of the technique I found, where a small fuse wire is soldered directly onto to the cell, thus avoiding to excessively heat the cell or the cable to make a connection to the cell... 

Will see with time.. although my calculation was that diy spot welder's cost is close to 50 eur. Depends is it battery or transformer driven of course, but still.
```

---
## \#67 Posted by: lox897 Posted at: 2016-08-21T20:24:39.513Z Reads: 295

```
<img src="/uploads/db1493/original/2X/e/e63d409fa51ad1432df9f8cea3676cf0b694ab30.jpeg" width="499" height="499"><img src="/uploads/db1493/original/2X/d/dd90e627f50b45bede815b854ce794aac18a9138.jpeg" width="499" height="499">
Finished most of the soldering on the Arduino side. Need to get some aluminium sheet so I can start on MOSFETS.
```

---
## \#68 Posted by: kovjanos Posted at: 2016-08-23T08:23:21.475Z Reads: 285

```
What’s wrong with it?
I read somewhere (or on instructables?) that new pieces have a clip-type legs not only thick pass-through to secure it to the panels. Those legs are for removing twisting stress from connector legs… Just squeeze those flat clips a bit or apply some sandpaper on them..

R, J.
```

---
## \#69 Posted by: lox897 Posted at: 2016-08-23T08:27:38.270Z Reads: 274

```
The pins are rectangular now, not pin. I looked at the traces on the board and there are no traces to the side pins so I just carved out the pcb a bit. I think that is ok. Otherwise I have another PCB.
```

---
## \#71 Posted by: kovjanos Posted at: 2016-08-23T08:31:27.918Z Reads: 276

```
Yes, enlarging the holes would also help – just make sure you have enough surface to solder it to the PCB.
Those pins / clips are only to physically secure the potmeter to the panel and remove the twisting force from the normal pins.

R, J.
```

---
## \#72 Posted by: lox897 Posted at: 2016-08-23T08:40:41.004Z Reads: 269

```
Pictures of what? There is a video on how to make the spot welder. It isn't too hard.
```

---
## \#74 Posted by: lox897 Posted at: 2016-08-23T08:50:34.048Z Reads: 281

```
I will send a pic when I get home. 
<img src="/uploads/db1493/original/2X/f/f56dd759700ae627b6dcbf55c09842584385d910.jpeg" width="384" height="384">
See the big side pins? They don't fit in the circle on the pcb. Either sand the pins thinner or use an xacto knife to carve the circle out a bit bigger so the pins fit in. If you still need a pic, I will happily get one for you.
```

---
## \#75 Posted by: DeathCookies Posted at: 2016-08-23T08:52:09.691Z Reads: 271

```
nah, everything is alright :D i just did not find the time to assemble mine yet.... Thank you very much!
```

---
## \#76 Posted by: lox897 Posted at: 2016-08-23T08:54:48.259Z Reads: 273

```
No problem. If you need any other help just ask me. I will finish the PCB soon but won't be able to finish the rest until Christmas. Please show me some pics when it is done. Good luck!
```

---
## \#77 Posted by: kovjanos Posted at: 2016-08-23T09:05:37.475Z Reads: 279

```
Check out the diffs in size of the clip-legs - thick does not fit through the hole:
<img src="/uploads/db1493/original/2X/3/3db134168a47537452c24a7c50160a2a2101b655.png" width="284" height="220">
```

---
## \#78 Posted by: DeathCookies Posted at: 2016-08-23T09:33:03.974Z Reads: 270

```
You have bought the parts from the bom of reichelt?
```

---
## \#79 Posted by: sl33py Posted at: 2016-08-23T19:49:18.612Z Reads: 273

```
@kovjanos - thanks for making these available to everyone.  I'm going to PM you to grab one or two.  I'll get the parts list from Mouser vs reichelt.de.

Sounds like a fun project - do you have yours complete and working well?  Any issues or tips we need to know that have changed from the video?

Thanks!
```

---
## \#80 Posted by: lox897 Posted at: 2016-08-24T10:55:56.588Z Reads: 257

```
I bought them from Reichelt. Cost quite a bit for shipping from Germany to Australia but at least I knew I had the right parts.
```

---
## \#81 Posted by: lox897 Posted at: 2016-08-24T10:56:43.515Z Reads: 253

```
@sl33py read the comments on the instructable. A guy put a list for Mouser components.
```

---
## \#82 Posted by: sl33py Posted at: 2016-08-24T17:23:12.547Z Reads: 255

```
Thanks @lox897!  Perfect - that'll be a lot easier for me in the US.  I'm talking with @Kovjanos to confirm he has a kit or two for me before getting the components.
```

---
## \#83 Posted by: Tarzan Posted at: 2016-09-06T10:45:55.748Z Reads: 240

```
[quote="lox897, post:67, topic:4500"]
Finished most of the soldering on the Arduino side. Need to get some aluminium sheet so I can start on MOSFETS.
[/quote]

Hey Lox I have to ask you what you mean with aluminum sheet and what you have done with it?
I have started mine yesterday and actually the soldering is fun.
My joints look good to me and I'll post some pics when I'm done.
```

---
## \#84 Posted by: Maxid Posted at: 2016-09-06T11:03:15.581Z Reads: 259

```
[quote="Tarzan, post:83, topic:4500, full:true"]
Hey Lox I have to ask you what you mean with aluminum sheet and what you have done with it?
[/quote]

see that aluminium the mosfets sit on:
https://cdn.instructables.com/FQ5/S6OA/IRLQQN5S/FQ5S6OAIRLQQN5S.LARGE.jpg
he talks about it in the video
```

---
## \#85 Posted by: lox897 Posted at: 2016-09-06T11:04:11.817Z Reads: 254

```
On the MOSFET side of the board you should put aluminium on top of the silver rectangle so the mosfets are level. If you watch the video he shows how to do it. If you need the template for the aluminium, pm me.
```

---
## \#86 Posted by: lox897 Posted at: 2016-09-06T11:05:10.072Z Reads: 248

```
Is that your board Maxid? Or is that his?
```

---
## \#87 Posted by: Tarzan Posted at: 2016-09-06T11:08:15.372Z Reads: 246

```
It must be his.
Mine is far away from complete :smiley:
```

---
## \#88 Posted by: lox897 Posted at: 2016-09-06T11:09:05.087Z Reads: 240

```
I meant Maxid or the creator of the welder. Sorry for the misunderstanding.
```

---
## \#89 Posted by: Maxid Posted at: 2016-09-06T11:10:10.956Z Reads: 254

```
that is an image from the instructable website.
mine is wrapped in heatshrink - otherwise I would have posted an image of it
```

---
## \#90 Posted by: Tarzan Posted at: 2016-09-06T21:31:27.822Z Reads: 265

```
<img src="/uploads/db1493/original/3X/b/f/bf5259f5ff2b41449cc2dcfb6624c37bf391a5da.jpg" width="666" height="500">
I have done some work and thanks to @lox897 I understood the aluminum part.
Please note that I have no idea what I'm doing and if this thing works everybody is able to do that.
I have  three more questions.
First: What to do with the fets? I don't know if I have to cut some legs or not. 
Second: Do I have to scratch the traces from the pcb like the German dude in the video?
Third: Do I connect the main pcb (12V and, GND) direct to a battery with thin wire for continues supply? Or do I need an extra 12 Volt supply because of the current?
Thanks
```

---
## \#91 Posted by: lox897 Posted at: 2016-09-06T21:36:27.192Z Reads: 251

```
1st: You don't need to cut the legs.
2nd: No, he fixed that quickly although I see silver on my board connecting to the mosfet board so I am not sure. Hopefully someone can confirm.
3rd: You can connect the 12v to the big 12v battery or use a 3s lipo or wall power supply.
```

---
## \#92 Posted by: lox897 Posted at: 2016-09-06T21:42:40.201Z Reads: 253

```
<img src="/uploads/db1493/original/3X/0/7/074eddb766b12da6bcaa93ba90625854b7c560af.jpeg" width="666" height="500"> This image shows that the trace underneath is connected
```

---
## \#93 Posted by: Tarzan Posted at: 2016-09-06T21:48:46.319Z Reads: 259

```
Thanks!
1: <img src="/uploads/db1493/original/3X/8/4/848d5e1e311011ede8d61f0c825c0292391b2269.jpg" width="375" height="500">
I don't know how these fets work, so I have ask again to make sure.
Do you have a detailed picture?
2: I heard that too but in the video it looks live he scratched away a bridge witch is on my pcb as well.
<img src="/uploads/db1493/original/3X/b/c/bcad653b80e332bd27685c9181278409a84c9e9e.jpg" width="666" height="500">
@Maxid what have you done?
3: Thanks again!
```

---
## \#94 Posted by: Maxid Posted at: 2016-09-06T22:22:49.472Z Reads: 232

```
The pcb we got is a newer version so no need to scratch anything. Just solder everything as it is now and you should be fine. Also when testing don't be surprised that you need to hold the foot switch down for a second until the spark is actually delivered - i tried to only have contact as short as possible and thought it is not working :smiley:
```

---
## \#95 Posted by: lox897 Posted at: 2016-09-06T22:23:00.607Z Reads: 233

```
Could you post a pic of the traces you are talking about?

EDIT: Did you also make sure you put the components on with the right polarity? The resistor at the top left looks like it has the writing facing inwards, I think it is supposed to be outwards
```

---
## \#96 Posted by: Tarzan Posted at: 2016-09-07T08:46:11.452Z Reads: 247

```
@lox897 
Of course.
<img src="/uploads/db1493/original/3X/9/1/91d28a2e18a17b9445faf72e273b5c2d1772d463.jpeg" width="666" height="500">
But I think maxid left them and his is working. So should be good!

I checked the components for polarity, but I was unsure with the top left one. I don't know what it is and the legs had the same length so I thought that there is no polarity.
Do resistors have a polarity? I know capacitors, diodes und LEDs have a polarity.

EDIT: I checked and resistors don't have a polarity. Is the top left part a resistor in a different shape?
```

---
## \#97 Posted by: lox897 Posted at: 2016-09-07T09:07:06.389Z Reads: 229

```
Yeah those traces are fine. I think it is only the brown resistors that have polarity. Maybe switch it just in case.
```

---
## \#98 Posted by: Maxid Posted at: 2016-09-07T09:11:18.703Z Reads: 225

```
https://github.com/KaeptnBalu/Arduino_Spot_Welder/blob/master/Eagle%20Files/Mosfet.PCB_board.JPG 
There you can see that it is meant to be that way. The fets have three legs: one for the current to enter and one to leave and one gate to "switch" the fet's state (basically opening and closing the circuit to allow the current to flow). If you would scratch the marked positions you would cut the circuit and the current would have no way to flow to - so please don't do it. The guy was talking about something else in the video - we do not have this issue anymore. Also there are different types of capacitors: http://2.bp.blogspot.com/-e4Y8eklya-M/T5tsyCnhwxI/AAAAAAAAAHI/CzLyc6APv88/s1600/capacitor1.png the one you are talking about has no polarity so it does not matter what way you mount it. Hope this helps - if you have further questions let me know.
```

---
## \#99 Posted by: kovjanos Posted at: 2016-09-07T09:51:14.082Z Reads: 229

```
PCBs are fine, no need to cut/remove anything on them. (other than cut the single PCB into two pieces :) )

FYI: The old PCB - what is presented on youtube - had an issue: not only the leg on the side but also the middle leg was connected and had to be cut manually otherwise it shorted the gate. This issue was fixed in the PCB design long time ago and now nothing to be cut...

R, J.
```

---
## \#100 Posted by: Tarzan Posted at: 2016-09-07T21:42:55.982Z Reads: 245

```
Got some work done.
<img src="/uploads/db1493/original/3X/3/3/337a402a7c10ee0a2cce3d518822929c91c39b9e.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/b/d/bdd66082c3c0d43aa69ded45376f38099e8ea86c.jpeg" width="666" height="500">
The fat cables on the back were a pain, but I'm happy with the results.
```

---
## \#101 Posted by: Maxid Posted at: 2016-09-07T21:46:07.702Z Reads: 241

```
looks beautiful - mine was such a mess that I had to wrap it in heatshrink just so that I do not have to look at it ;)
```

---
## \#102 Posted by: Tarzan Posted at: 2016-09-07T21:50:26.777Z Reads: 238

```
😄 I know exactly what you mean.
Some of my projects turned out worse then expected, but for some reason I'm very passionated with this one.
I only have clear shrink so it has to look cool at least.
```

---
## \#103 Posted by: sl33py Posted at: 2016-09-08T00:03:21.581Z Reads: 225

```
anyone with this Arduino setup also use the TVS and Schottky diodes?  I just finished reading through the 24 pages on ES (from Riba's original JP welder) and this seems to be recommended by the gurus.

I'm going to mangle it, but basically there is an avalanche current for ~100 microseconds which is known to fry FETs.  They added two components - the Schottky and then TVS to minimize this and extend the life of the spot welder.  They are two small components and only $3-5ea.  I think i understand how to wire these in, so will give it a shot when i build mine.  I got a board (and a spare) so just waiting on components from Mouser.

I also went with the 1324 FETs as they were recommended as an upgrade.  A bit more $, but marginal additional cost.
```

---
## \#104 Posted by: lox897 Posted at: 2016-09-08T03:49:49.281Z Reads: 220

```
May I ask what wire you used?
```

---
## \#105 Posted by: akira Posted at: 2016-09-08T08:01:55.150Z Reads: 223

```
Do you have a link for this modification ?
```

---
## \#106 Posted by: DeathCookies Posted at: 2016-09-08T09:00:57.803Z Reads: 221

```
Lazy folk :smiley:
https://endless-sphere.com/forums/viewtopic.php?f=14&t=81400&start=550#p1218325
```

---
## \#107 Posted by: Tarzan Posted at: 2016-09-08T09:16:08.367Z Reads: 219

```
:D That is speaker wire with 2.5 mm^2 on each strand.
I combine four of them together to get 10 mm^2.
Why I used speaker wire? Good question!
I had it and it is quite flexible. It should do the job well and handling of the electrodes will be easy.

@sl33py No I haven't updated anything. I see that thread on ES the first time right know :slight_smile:
Looking forward for your build.
```

---
## \#108 Posted by: Tarzan Posted at: 2016-09-09T16:12:09.819Z Reads: 212

```
Damn mine isn't working. I think I destroyed one to some of the fets due to heat.
If I measure the resistance on the legs there shouldn't be a connection right?
Mine circuit shortened and the switch does nothing and the current flows the whole time.
The potentiometer works but the display does not show anything.
Do I have to program this tiny computer before? @Maxid 

@sl33py do you have a list with all necessary parts for the upgrade? Since I have to order new fets I could add them as well.
```

---
## \#109 Posted by: kovjanos Posted at: 2016-09-09T16:17:05.540Z Reads: 216

```
Yes, you have to program it. Here is the sketch: 
https://github.com/KaeptnBalu/Arduino_Spot_Welder/tree/master/arduino_spot_welder 

R, J.
```

---
## \#110 Posted by: Tarzan Posted at: 2016-09-09T16:20:16.396Z Reads: 215

```
Thank you for your help. @kovjanos 
Is there a recommendated tool to transfer the code? Or a YouTube tutorial 😄
I'm sorry but I'm really clueless.....
```

---
## \#111 Posted by: kovjanos Posted at: 2016-09-09T16:24:01.880Z Reads: 233

```
Download link:
https://www.arduino.cc/en/Main/Software

Make sure you have the USB driver for the CH340 chip (serial adapter). Win10 should have it, for Win7 and Win8 Google will help.

When you program it, select the Arduino Nano and then the new ATmega328 after you double checked that the right port is selected.

R, J.
```

---
## \#112 Posted by: laikiux Posted at: 2016-09-15T18:12:52.841Z Reads: 237

```
Some pics of my custom made spot welder:
<img src="/uploads/db1493/original/3X/0/8/08bf9d5c26abcd3e0a4fab276774b72f82033ed7.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/5/d/5debc8d71620455685b3131482a4d042bdace364.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/3/f/3f7c665da037bb887760bfe452b9eb1575a4000d.jpg" width="669" height="499">
```

---
## \#113 Posted by: TarzanHBK Posted at: 2016-09-15T21:21:17.492Z Reads: 234

```
do you still have one set available? sitting in germany :slight_smile:
```

---
## \#114 Posted by: kovjanos Posted at: 2016-10-03T08:27:53.685Z Reads: 203

```
I received another set of components, a few packs are available again!
```

---
## \#115 Posted by: Maxid Posted at: 2016-10-25T11:24:50.235Z Reads: 198

```
Tried mine today with nickel strips - it works in principal but even at 20ms it does not weld two strips together. They stick slightly but can be pulled apart easily. Any idea what I can do? Battery is a car battery with max discharge 700A
```

---
## \#116 Posted by: DeathCookies Posted at: 2016-10-25T11:27:17.559Z Reads: 205

```
How thick is the nickel strip? Maybe it is too thick?
```

---
## \#117 Posted by: 2-alex-2 Posted at: 2016-10-25T11:39:20.854Z Reads: 209

```
I have been using a car battery to do mine so far ok are you using a controller to restrict the flow. <img src="/uploads/db1493/original/3X/f/a/fa8fbce19bfc2b4323ca242c9e2956013083817b.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/4/247637f9ad116563b8fdb925089725cbe7aef441.JPG" width="375" height="500">
```

---
## \#118 Posted by: Maxid Posted at: 2016-10-25T11:46:58.327Z Reads: 204

```
I am using the arduino spot welder linked above. 

@DeathCookies thickness is 0.15mm. so pretty standard
```

---
## \#119 Posted by: 2-alex-2 Posted at: 2016-10-25T11:53:14.607Z Reads: 207

```
Ok may be something in the settings as similar setup to mine just I'm using a high amp push button switch. What do you copper probes look like nice point on them.
```

---
## \#120 Posted by: TarzanHBK Posted at: 2016-10-30T17:57:06.035Z Reads: 205

```
I started today with the arduino spotwelder and have 2 questions:

<img src="/uploads/db1493/original/3X/2/e/2eb4e2a109833d1f8eec98febf7b75a8912a7281.jpg" width="690" height="388">

1 - Why is there a connection when i´m supposed to cut the pcb there?`

2 - JP1 - 4 should i connect them on the 2 boards? Like JP1 goes to JP3 and JP2 goes to JP4? Or are they for something else?
```

---
## \#121 Posted by: kovjanos Posted at: 2016-10-31T16:12:52.503Z Reads: 199

```
Hi,

1 - That change was added by the author to let the PCB manufacturer accept it as a single PCB. You can cut it as printed on the board.

2 - From the instructables page:
> In the new Version you have to connect JP1 on the Arduino Board with JP1 on the Mosfet Board and JP2 on the Arduino Board with JP2 on the Mosfet Board. Use pin headers and sockets. These jumpers connect the ground of the two boards.

Unfortunately those are called JP1 and JP2 on the Mosfet Board and JP3 and JP4 on the Arduino Board...

R, J.
```

---
## \#122 Posted by: mountainboardlover69 Posted at: 2016-10-31T17:03:20.299Z Reads: 182

```
do u stil have on btw i am in nl
```

---
## \#123 Posted by: kovjanos Posted at: 2016-10-31T17:06:19.150Z Reads: 173

```
I could have a single PCB available but no more packs. I have to check it on Wednesday when I'm back to home...
```

---
## \#124 Posted by: mountainboardlover69 Posted at: 2016-10-31T17:07:11.787Z Reads: 178

```
wil u ever get more?
```

---
## \#125 Posted by: mountainboardlover69 Posted at: 2016-10-31T17:07:45.702Z Reads: 182

```
btw is ther any one i can sell the full woring ting from?
```

---
## \#126 Posted by: kovjanos Posted at: 2016-10-31T17:13:26.762Z Reads: 188

```
Maybe - not easy to source things getting closer to Xmas time...
```

---
## \#127 Posted by: TarzanHBK Posted at: 2016-11-01T22:18:13.020Z Reads: 185

```
great! Will do that, thx janos :slight_smile:
```

---
## \#128 Posted by: Maxid Posted at: 2016-11-08T11:59:28.574Z Reads: 191

```
@TarzanHBK @DeathCookies @Tarzan @kovjanos

While waiting for my new Mosfet drivers to arrive (I shorted mine :( ) I had the idea to get rid of the big foot switch and replace it with a switch at the fingertips.
Used a cheap microswitch like this one:
http://www.sf-ersatzteile.de/out/pictures/master/product/1/dsc_0038.jpg

and attached it to the electrode via double sided tape.
Allows for a much smaller total footprint of the spot welder - and is also cheaper and easier to get than the foot switch.

Just thought you might want to know for your builds.
```

---
## \#129 Posted by: TarzanHBK Posted at: 2016-11-08T12:04:08.784Z Reads: 188

```
Thx Daniel, i got @kovjanos set with a small footswich, which feels really good to work with.
I still have to finish my Spotwelder, then i will report back here about how good it works ;)
```

---
## \#130 Posted by: Tarzan Posted at: 2016-11-10T21:55:47.325Z Reads: 187

```
My fets shorted as well after five welds.
Are you building this bypass seen on endless sphere?
```

---
## \#131 Posted by: Maxid Posted at: 2016-11-11T20:29:39.007Z Reads: 193

```
I included the TVS diode but could not get it to work with the schottky. With the schottky everytime i applied a pulse the arduino would seemingly stop working (status LED did not turn off anymore, pulse time display stopped alternating between digits and no additional pulses could be fired). I removed the schottky and think that the TVS diode is at least better than nothing. Worked like a charm for my first custom 4S Liion battery. I replaced the NiCd battery in my electric drill - no more memory effect :D :tada:
```

---
## \#133 Posted by: Pedrodemio Posted at: 2016-11-13T13:50:10.048Z Reads: 182

```
Anyone tried using a LiPo battery instead of the car battery? I have 2 3S 5000mAh 35-70C that on paper should provide sufficient current with them in parallel
```

---
## \#134 Posted by: DeathCookies Posted at: 2016-11-13T18:04:40.010Z Reads: 178

```
I got told from the creator of the adruino spotwelder that you will need about 300A. It could be even less but he advises this number.
```

---
## \#135 Posted by: TarzanHBK Posted at: 2017-01-18T09:44:12.302Z Reads: 170

```
How thick is your Aluminium under your fets guys?
```

---
## \#136 Posted by: Maxid Posted at: 2017-01-18T11:47:25.842Z Reads: 164

```
I think I used like 4-6mm
```

---
## \#137 Posted by: Tarzan Posted at: 2017-01-18T11:56:26.367Z Reads: 163

```
Mine is only 3 mm
```

---
## \#138 Posted by: TarzanHBK Posted at: 2017-01-18T12:27:00.917Z Reads: 159

```
hmm i think i´ll up that to 4mm then..
```

---
## \#139 Posted by: TarzanHBK Posted at: 2017-04-13T11:19:35.415Z Reads: 152

```
how did you solve your problem with welds beeing too loose?
Having the same problem, tried it on a car battery, setting to 20 mS Puls, so FULLPOWA, but could still remove the 2 welded 0,15mm nickel strips by hand..
Does someone else has a solution for this?
Would be good to set puls to something like 10 mS and get good results, to have a bit more room for thicker things with up to 20 mS, instead I´m already having problems with 20 mS :frowning:
```

---
## \#140 Posted by: Pedrodemio Posted at: 2017-04-13T12:27:05.311Z Reads: 153

```
How big is your battery? And is it new? It seems to be low current
```

---
## \#141 Posted by: TarzanHBK Posted at: 2017-04-13T12:35:25.136Z Reads: 155

```
I tested it on two old 45Ah car batteries, first with one - too low, then with the other one connected in parallel to ensure more current - still too low (ok both are a bit old..)
So I hooked up two 3s 30C Lipos in parallel to test it with them - worked much better, but it´s still possible to get them apart  by hand. 
So I think i´ll try it with my current, fresh battery if that works better...
```

---
## \#142 Posted by: Maxid Posted at: 2017-04-13T13:05:23.695Z Reads: 152

```
My welds are solid at like 14ms. Putting pressure on the tips also gives me better results - I don't know how hard you have been pushing them down on the tabs. Maybe some of your mosfets are broken? First thing I would try is a fresh (and powerful) battery though. I used a brand new one when I did my packs.
```

---
## \#143 Posted by: TarzanHBK Posted at: 2017-04-13T13:09:01.468Z Reads: 149

```
so you had problems at first with 20mS, used a new battery and now it works with 14mS?
```

---
## \#144 Posted by: Maxid Posted at: 2017-04-13T13:13:58.363Z Reads: 146

```
As you can see in the thread I had to replace my Mosfet drivers and Mosfets and had no problem since. The first time I accidentally bridged some connections on the bottom next to the soldered wire with a bad soldering job.

Maybe you did the same?
```

---
## \#145 Posted by: TarzanHBK Posted at: 2017-04-13T13:22:12.972Z Reads: 152

```
Ah ok I see...
I look after them later today and try a new battery, if everything looks good.
Thx :slight_smile:
```

---
## \#146 Posted by: Maxid Posted at: 2017-04-13T18:41:29.439Z Reads: 150

```
So from looking at the picture you posted it looks like you got some nice welds. What made the difference?
```

---
## \#147 Posted by: TarzanHBK Posted at: 2017-04-14T09:31:06.922Z Reads: 159

```
Yep! Was the battery! Just went and bought a 95 Ah 710A big battery and everything works perfectly fine!
I'm welding with 11 mS now 👌
```

---
## \#148 Posted by: tonystark Posted at: 2017-05-12T23:29:42.153Z Reads: 149

```
what kind of wire are you using? i got some fat wire but it is very stiff and i cant pull it through the transformer
```

---
## \#149 Posted by: TarzanHBK Posted at: 2017-05-13T09:32:56.658Z Reads: 145

```
8awg. Works good, but gets warm after a few welds. So I'd take 2 8awg parallel.
```

---
## \#150 Posted by: TarzanHBK Posted at: 2017-08-30T13:45:02.844Z Reads: 120

```
just leave this here for other people to find:
Arduino Spotwelder from Käpt´n Balu:
https://malectrics.eu/
```

---
## \#151 Posted by: darkkevind Posted at: 2017-08-30T14:06:45.920Z Reads: 118

```
Or this..... (my welder)

https://youtu.be/o4NaDMoEHxU
```

---
## \#152 Posted by: Rinzler Posted at: 2017-11-02T22:17:58.163Z Reads: 102

```
@acido Maybe build your own? There are plenty of diy options out there. Some good info in this thread too.
```

---
## \#153 Posted by: moon Posted at: 2018-04-10T14:11:58.544Z Reads: 61

```
How did you spotwelder turn out @monkey32
```

---
