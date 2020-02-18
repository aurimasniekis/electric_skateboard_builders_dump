# V4.12 Direct VESC - OllinBoardCo

### Replies: 160 Views: 12687

## \#1 Posted by: chaka Posted at: 2016-11-15T15:16:12.888Z Reads: 703

```
I have received several request to modify V4.12 to use direct-fets. Time will tell what kind of increase in current handling the direct-fets will provide but this should provide some relief for those who are upset about the recent events in the open source community.

<img src="/uploads/db1493/original/3X/7/3/73965c56aa9aa81c795f3e864546c21084aea1d0.png" width="690" height="291">
[https://oshpark.com/shared_projects/6kWeFuuK](https://oshpark.com/shared_projects/6kWeFuuK)

These files are untested but we will build them out and run them through some trials in about a week. The plan is to encase this version of the VESC in a very low profile case and supply this for those who need something a little more compact than the upcoming V6.
```

---
## \#2 Posted by: Pantologist Posted at: 2016-11-15T15:27:18.201Z Reads: 602

```
Are the direct Fets the only modification compared to your regular updated BOM?
```

---
## \#3 Posted by: akira Posted at: 2016-11-15T15:29:24.061Z Reads: 594

```
I asked exactly the same question on another forum ;-)
And the very quick answer was ... YES.
Direct FET reference : http://eu.mouser.com/Search/ProductDetail.aspx?R=IRF7749L2TRPBFvirtualkey57370000virtualkey942-IRF7749L2TRPBF

Thanks Chaka !
```

---
## \#4 Posted by: chaka Posted at: 2016-11-15T15:32:03.148Z Reads: 568

```
Please wait till we have assembled and tested these files before ordering pcb's ;) They passed the sanity check but there is always a chance that something will need to be changed.
```

---
## \#5 Posted by: Michael319 Posted at: 2016-11-15T16:10:58.781Z Reads: 550

```
Does anyone have an ETA or an update on 6.0, I plan on building in around February, so I might need to go with a 4.12
```

---
## \#6 Posted by: chinzw Posted at: 2016-11-15T17:03:22.255Z Reads: 532

```
Great job! It's good to see people keeping open source going!
```

---
## \#7 Posted by: chaka Posted at: 2016-11-15T18:17:46.806Z Reads: 514

```
Version 6 is coming. Vedder is finishing the new Vesc-tool and should have something for everyone soon. I expect him to make some sort of announcement in the next few weeks.

Version 6 is much more than just switching to direct-fets and a new layout.  It will perform on a whole new level and requires some new components which will result in a higher production cost. Simply switching to direct-fets will result in a very small increase in price but adding heatsinks is a requirement. We are considering building these with several different heat sink packages, the most affordable will be what we offer now. Fully enclosed ultra slim options will also be available. 

If designed well, a dual drive will perform perfectly with the original v4.12 designed by Vedder and the extra expense of heat sinking and switching to direct-fets is not really needed. We really only see problems when using hub motors due to the huge amperage spikes and efficiencies we see on 1:1 gear ratios and single belt-drives with 2:1 gear ratios.

Adding heatsinks and direct-fets alone might not add much to the constant current handling of the vesc, you will need to provide some sort of active or passive cooling with vents and/or fans to see real gains.
```

---
## \#8 Posted by: Quinlanbrown Posted at: 2016-11-15T18:38:57.891Z Reads: 470

```
Will these new vesc have a higher A output also you'll should sell an option with no heat sink bc divers could bild there own if it's clear that it's needed, I build one in about an hour
```

---
## \#9 Posted by: Michael319 Posted at: 2016-11-16T13:57:24.306Z Reads: 452

```
Do you have an idea on pricing? Because u really don't want to spend over 200 on a single vesc.
```

---
## \#10 Posted by: chaka Posted at: 2016-11-17T14:43:06.991Z Reads: 443

```
Pricing will vary depending on the heat sink packages. We will probably have several options. 

We are also working on a high output model with 12 fets for ebikes and high performance RC applications. 

You may not want to pay more than $200 but you will quickly find that most high output 12s ESC packages are well over $200, some as high as $350.
```

---
## \#11 Posted by: Michael319 Posted at: 2016-11-17T14:55:56.284Z Reads: 427

```
That's the problem, I'm 18 and I'm not made of money lol. Will probably have to just stick with a 4.12
```

---
## \#12 Posted by: chaka Posted at: 2016-11-17T15:14:29.011Z Reads: 429

```
That is why I provide the PCB order links to our OshPark account. Get a few like minded friends together and build a few. Who knows it may help fund your inevitable Eboarding addiction someday! 

Be sure to wait till I test these first.
```

---
## \#13 Posted by: mishrasubhransu Posted at: 2016-11-17T21:07:55.707Z Reads: 424

```
So who's building the 12 fet model? It is based on VESC 6 or V4.12? Is it just a matter of putting the FET's in parallel?
```

---
## \#14 Posted by: chaka Posted at: 2016-12-07T18:12:58.623Z Reads: 426

```
@mishrasubhransu we will be working towards a 12 fet version soon. Currently we are testing the direct fet version we posted to our oshpark account. Did the first round of testing this morning and it is running beautifully! We will be installing it on a single motor build and running it through some trials in an enclosed system before moving it into full production. 

In short, the gerber files are working as they should, feel free to order and assemble! Be sure to add some sort of heat sink to the fets too ;)

<img src="/uploads/db1493/original/3X/c/c/cc3f1837923017507932b50795d7a490aac245ac.jpg" width="690" height="388">
```

---
## \#15 Posted by: chinzw Posted at: 2016-12-07T18:21:50.481Z Reads: 404

```
That's looking beautiful!
```

---
## \#16 Posted by: saul Posted at: 2016-12-07T20:26:34.105Z Reads: 400

```
[quote="chaka, post:14, topic:13104"]
In short, the gerber files are working as they should, feel free to order and assemble! Be sure to add some sort of heat sink to the fets too :wink:
[/quote]

Great to see you giving back to the open source community! 

I'm tempted to mod a toaster oven for some smd goodness! :sunglasses:
Not trying to make you reveal any production secrets but a timelapse of blank pcb -> finished VESC would be awesome!
```

---
## \#17 Posted by: chaka Posted at: 2016-12-07T21:08:55.135Z Reads: 387

```
There are few time laps videos on our Instagram.  We have always planned on creating a "how to" video but we never seem to have time. Never not building here in the shop.
```

---
## \#18 Posted by: saul Posted at: 2016-12-07T23:30:39.297Z Reads: 389

```
[quote="chaka, post:17, topic:13104"]
Never not building here in the shop.
[/quote]

I hope to have that problem someday soon! :upside_down:
```

---
## \#19 Posted by: racidon Posted at: 2016-12-08T04:09:07.633Z Reads: 405

```
Would you think these would hold up to e-MTB applications?
I've still yet to get my ESCs for my next board and would prefer VESC over other ESCs I just know that VESCs are not recommended for eMTB at the moment.

I've got all of it except mounting hardware and ESCs (+ BEC if I don't use the VESC)

Parts:
HolyPro Deck
8" wheels
12s7p (samsung cells)
Leopard 8072-10T 175KV (x4)

I'm leaning towards chain at the moment, as I want to take this board in the bush more than I will use it around town so it's going to be pushed to the limits :slight_smile:
```

---
## \#20 Posted by: jmasta Posted at: 2016-12-08T04:28:16.948Z Reads: 394

```
Looks promising! Thanks for all your hard work
```

---
## \#21 Posted by: chaka Posted at: 2016-12-08T05:10:33.822Z Reads: 374

```
@racidon Hard to give any real feedback before testing this in "real world conditions". Might be up to the task but I am leaning towards a 12 fet version for eMTB. 

@jmasta Thanks, but this wasn't too hard to do. KiCad is surprisingly easy to use. Thank Benjamin Vedder! 
http://vedder.se/2015/01/vesc-open-source-esc/
```

---
## \#22 Posted by: PXSS Posted at: 2016-12-08T11:10:43.849Z Reads: 369

```
Hey! I'm fairly new here. Can you add links to where we can buy the pcb and a bom if possible? Looking to buy and assemble myself. Hopefully doable under $120?

Thanks!
```

---
## \#23 Posted by: akira Posted at: 2016-12-08T12:30:30.432Z Reads: 370

```
Here is the PCB : 
https://oshpark.com/shared_projects
The BOM is mostly the same than the V4.12 there except for the MOSFETs :
https://github.com/vedderb/bldc-hardware

But you need VERY good SMD soldering skills and some serious equipement (hot air gun/reflow oven).
```

---
## \#24 Posted by: hexakopter Posted at: 2016-12-08T21:22:24.790Z Reads: 368

```
[quote="chaka, post:14, topic:13104"]
we will be working towards a 12 fet version soon
[/quote]
Just know that the DRV could most likely not handle that. It would be a too high gate charge from two IRF7749 in parallel. 
Also your current design looks like a waste of place just to maintain the dimensions of the HW 4.12 VESC. Because almost all the heat is transferred over the top and not the PCB, I don't see a problem placing them opposite.
```

---
## \#25 Posted by: chaka Posted at: 2016-12-08T21:37:11.143Z Reads: 356

```
Yeah, we have accounted for the gate charge. It should be fine but we wont know until we build it.

@PXSS I wouldn't try this unless you are fairly confident. It can get costly very quickly if you make mistakes. Plus you will need a hot air machine at the very least.
```

---
## \#26 Posted by: PXSS Posted at: 2016-12-08T22:23:47.792Z Reads: 345

```
Thanks for the warning! I am an aerospace engineer with fairly good soldering skills and tools. I got a soldering station and a full rework hot air station. 

It's just my first time getting my feet wet with electric longboards. ;-)
```

---
## \#27 Posted by: chaka Posted at: 2016-12-08T22:28:59.297Z Reads: 340

```
If you can hold off for a few days I will be updating the files on OshPark, going to expose the main power via so we can tin it with a bead of solder for better current handling. Might not be necessary but I have yet to run these very hard for an extended period.
```

---
## \#28 Posted by: Hummie Posted at: 2016-12-08T22:31:04.310Z Reads: 336

```
Maybe you don't know yet but what do u think the amp limits will be?
```

---
## \#29 Posted by: chaka Posted at: 2016-12-08T22:39:11.734Z Reads: 329

```
50 to 60 amps constant. Possibly more if you add a cooling fan. Really can't say until we get more bench testing done.
```

---
## \#30 Posted by: michaelcpg Posted at: 2016-12-08T22:52:09.450Z Reads: 325

```
Any chance of there being the possibility to upgrade your standard 4.12 VESCs to ones with direct FETs or do these require a different PCB layout?
```

---
## \#31 Posted by: chaka Posted at: 2016-12-08T23:02:03.413Z Reads: 324

```
Yeah it is a different layout but the good news for you is you have Ollin VESC's so they have value even if they are not working. :wink: You can sell them after you upgrade!

 Really the main goal for these is to provide more current handling for more extreme conditions and applications. If your current setup is working without hitting the overheat protection then you really don't need to upgrade.
```

---
## \#32 Posted by: michaelcpg Posted at: 2016-12-08T23:24:33.704Z Reads: 318

```
Haha no worries, thought that might be the case. 
My dual VESC's atm start to hit their overheating protection near the top of some of the gnarlier hills around my house but it's generally a non issue for 95% of my riding so probably not worth the upgrade for me at this stage :p
```

---
## \#33 Posted by: racidon Posted at: 2016-12-09T00:24:56.969Z Reads: 323

```
[quote="chaka, post:21, topic:13104, full:true"]
@racidon Hard to give any real feedback before testing this in "real world conditions". Might be up to the task but I am leaning towards a 12 fet version for eMTB. 

[/quote]
Let me know when you think it would be ready for real world testing I'd be keen to give it a go. I'm pretty confident that if you think it will work it likely will :)
```

---
## \#34 Posted by: chaka Posted at: 2016-12-15T15:56:07.641Z Reads: 323

```
Finished making some revisions last night and sent the files to OshPark for pcb fabrication.

  The power stage is now equal or better to what we see on version 6. I have also moved and added several capacitors to improve FOC performance and increase reliability. 

  We are also taking a more aggressive approach in designing the heatsink/case, double sided vs a single base.  Nearly double the thermal mass and surface area as V6 so we expect to handle more than 70 amps constant.

  We do not expect any problems with our latest revision so we will be moving this into production once we verify the changes.
```

---
## \#35 Posted by: Michael319 Posted at: 2016-12-15T16:09:08.038Z Reads: 313

```
Super exciting! Can't wait to pick one of these up!
```

---
## \#36 Posted by: Michael319 Posted at: 2016-12-15T16:15:15.232Z Reads: 312

```
Do you have anytime frame for pre ordering/delivery? I want to pick one up ASAP tbh
```

---
## \#37 Posted by: chaka Posted at: 2016-12-15T16:33:58.622Z Reads: 305

```
I should have some g-code for the aluminum case finished later this week. I will post photos and make an announcement regarding pre-orders and pricing as soon as we finish!
```

---
## \#38 Posted by: Pedrodemio Posted at: 2016-12-15T17:13:29.728Z Reads: 299

```
Would you sell without any heatsink? I will use a custom one that integrates with the design of the enclosure and board
```

---
## \#39 Posted by: racidon Posted at: 2016-12-16T03:45:29.520Z Reads: 298

```
More than 60amps? O.o    you think that will be emtb ready then? if I remember correctly my battery design (12s7p) really shouldn't operate higher than 60amps continuous anyway :)
```

---
## \#40 Posted by: saul Posted at: 2016-12-16T03:57:29.399Z Reads: 306

```
[quote="chaka, post:34, topic:13104"]
We do not expect any problems with our latest revision so we will be moving this into production once we verify the changes.
[/quote]

is this replacing the standard 4.12 or is this a high power version?
```

---
## \#41 Posted by: psychotiller Posted at: 2016-12-16T04:05:19.286Z Reads: 272

```
Just count me in for 2! :stuck_out_tongue_winking_eye:
```

---
## \#42 Posted by: WrinklyWink Posted at: 2016-12-18T08:47:00.918Z Reads: 279

```
I ordered a pair with heatsinks earlier this year.. I've never used them, that includes soldering, but I only cut off the heat shrinks. Can I exchange them?
```

---
## \#43 Posted by: Eboostin Posted at: 2017-01-10T03:30:30.654Z Reads: 284

```
Any updates? I saw them on your site. @chaka

Definitely interested! Also, what do you think the capability is withouth the heatsink? What are the dimension without a case?  

I'm getting short on space with my 10S4P.
```

---
## \#44 Posted by: chaka Posted at: 2017-01-12T15:54:51.597Z Reads: 277

```
They do well without heat sinks if you want to save money and space but you need heat sinks if you want to drive them hard.
```

---
## \#45 Posted by: Eboostin Posted at: 2017-01-12T16:16:35.531Z Reads: 268

```
My preference would be to run with heatsink just not sure if I can fit it with them.

Do you have anymore pics? What are the dimensions without the heatsink? Do these peform any better than the old layout when neither have heatsinks?
```

---
## \#46 Posted by: okp Posted at: 2017-01-12T16:21:13.555Z Reads: 270

```
is there some data evidence showing that the "original" VESC is getting in "bad shape" and your or other  vesc under steroids are outstanding its "performance"? Not sure I'm using the right words; but wondering if such tests were done to assess the benefits in a real case situation of someone who is riding; sort of a gap analysis ... but with real riding figures/live mode.
```

---
## \#47 Posted by: chaka Posted at: 2017-01-12T16:28:23.480Z Reads: 276

```
@Eboostin We will be releasing product photos soon. 

@unik We covered this already on your forum didn't we? I know I have covered the limitations of the original VESC extensively on this forum. The search function should give you the information you need.
```

---
## \#48 Posted by: okp Posted at: 2017-01-12T16:33:54.663Z Reads: 267

```
@chaka thanks a lot for the kind words :) I was much more asking about real life video riding evidence that may show that a VESC freezes or burn... vs yours ... that still survive and this is way better for the user than all the top notch experts that speak complex languages. But you are right, I'm sure I will find such video with the search button.
```

---
## \#49 Posted by: chaka Posted at: 2017-01-12T16:43:00.466Z Reads: 265

```
I am sure you will find the information you need. Frankly, I am surprised you were unaware that the original VESC will overheat if you push it hard. It is well known among seasoned builders.
```

---
## \#50 Posted by: okp Posted at: 2017-01-12T16:45:05.098Z Reads: 268

```
been quite busy last year on my project; some people are lucky enough to have a garage... I had a 3x3 meters square room to develop it !! seems I have to get up to speed on some topics. cheers!
```

---
## \#51 Posted by: jbruce Posted at: 2017-01-18T01:12:08.663Z Reads: 268

```
Any pictures or updates on production? @chaka
```

---
## \#52 Posted by: Michael319 Posted at: 2017-01-18T01:17:44.215Z Reads: 268

```
No pics available to the public yet, but pre orders should be shipped by the 30th
```

---
## \#53 Posted by: jbruce Posted at: 2017-01-18T02:17:12.234Z Reads: 272

```
lol @Michael319  that's why I asked chaka if he's got any. :wink:
```

---
## \#54 Posted by: Eboostin Posted at: 2017-02-01T01:02:56.799Z Reads: 266

```
Are these close to shipping out? @chaka
```

---
## \#55 Posted by: Michael319 Posted at: 2017-02-01T02:45:52.828Z Reads: 265

```
I'm wondering the same thing, @chaka told me mine would be shipped out 2 weeks ahead of the other orders, but still no word. One of their customer service reps sent me they still haven't finalized the design, they will let us know when they do. But I'm not sure she has accurate information.
```

---
## \#56 Posted by: Eboostin Posted at: 2017-02-01T03:10:37.309Z Reads: 278

```
I hope that's not the case. I paid with the expectation that they were completed and shipping out on or around the end of January. It's only the 31st so I get it but would hope to have it in hand in the next two weeks.
```

---
## \#57 Posted by: Michael319 Posted at: 2017-02-01T03:26:54.715Z Reads: 289

```
@Eboostin 
<img src="/uploads/db1493/original/3X/0/b/0b8c79c67e1d3af9049217e16f8c60490c2ba659.png" width="281" height="500"><img src="/uploads/db1493/original/3X/c/7/c7666cb4158f9454f01c0057f62a6a10559483bb.png" width="281" height="500">
```

---
## \#58 Posted by: Eboostin Posted at: 2017-02-01T03:56:01.847Z Reads: 277

```
Hmmm, well hopefully they are close. 

Ollin Has a solid reputation from what I've read and my one previous purchase so not worried, some updates would be nice though
```

---
## \#59 Posted by: Michael319 Posted at: 2017-02-01T04:04:13.628Z Reads: 274

```
That's how I feel, I still have the utmost respect for them. Haven't heard anything in over 2 weeks though.
```

---
## \#60 Posted by: Eboostin Posted at: 2017-02-04T04:16:53.101Z Reads: 277

```
Any updates? @chaka
```

---
## \#61 Posted by: Michael319 Posted at: 2017-02-04T14:18:38.837Z Reads: 266

```
Just heard from them, they will no longer be visiting the forum.
```

---
## \#62 Posted by: Eboostin Posted at: 2017-02-04T15:36:55.734Z Reads: 270

```
That's unfortunate :( I valued his posts.

Did he provide an update when you talked to them? @Michael319
```

---
## \#63 Posted by: Michael319 Posted at: 2017-02-04T15:39:35.558Z Reads: 269

```
Yes, they were having small issues, so they fixed them and put in a new order, they should be arriving within a week or 2. I was told that I would have one in my hand in 2 weeks.
```

---
## \#64 Posted by: jbruce Posted at: 2017-02-20T22:03:13.507Z Reads: 267

```
By any chance have you gotten yours yet?
```

---
## \#65 Posted by: Pantologist Posted at: 2017-02-20T22:28:43.773Z Reads: 259

```
Pretty sure the first few batches went to FreeRide preorders. Preorders just started getting fulfilled so a bit longer.
```

---
## \#66 Posted by: jbruce Posted at: 2017-02-20T22:38:49.776Z Reads: 263

```
What's free ride? I pre ordered t the first day it came up on ollinboards.
```

---
## \#68 Posted by: jbruce Posted at: 2017-02-20T23:04:01.582Z Reads: 262

```
Nice!! Did you preorder it from ollin boards and did they send you a tracking number?
```

---
## \#69 Posted by: Michael319 Posted at: 2017-02-20T23:05:03.984Z Reads: 264

```
yes, I preordered it, but I had to contact them for my tracking number
```

---
## \#70 Posted by: jbruce Posted at: 2017-03-07T00:40:54.751Z Reads: 252

```
did you end up getting it? I've been trying to contact them for a week and they haven't responded to my email.
```

---
## \#71 Posted by: Michael319 Posted at: 2017-03-07T02:35:27.769Z Reads: 254

```
Try to contact them on Facebook, they're much more responsive there. And yes I did receive it.
```

---
## \#72 Posted by: Eboostin Posted at: 2017-03-07T02:40:18.249Z Reads: 261

```
Did you receive 2.0 or 2.1?
```

---
## \#73 Posted by: Michael319 Posted at: 2017-03-07T02:43:36.606Z Reads: 260

```
What is 2.1?
```

---
## \#74 Posted by: Eboostin Posted at: 2017-03-07T02:45:30.661Z Reads: 255

```
The new version. It's on their site now, shipping end of March
```

---
## \#75 Posted by: Michael319 Posted at: 2017-03-07T02:59:57.943Z Reads: 254

```
The hell is the difference?
```

---
## \#76 Posted by: Michael319 Posted at: 2017-03-07T03:10:18.864Z Reads: 260

```
Releasing a new product before some people even receive their pre order for the previous product is kind of ridiculous, hopefully they have some sort of upgrade like Carvon.

Especially if there is a flaw with 2.0
```

---
## \#77 Posted by: jbruce Posted at: 2017-03-07T03:10:35.958Z Reads: 252

```
From what ive heard from them, 2.0 is the same form factor as the old vesc, just with all the new updates, and the one used in thier freeride board. The 2.1 is the new form factor with the the heatsink attached. Which one did you get?
```

---
## \#79 Posted by: jbruce Posted at: 2017-03-07T03:13:01.200Z Reads: 259

```
So same form factor as normal vesc just with a heat sink? Are the capacitors in the normal place of is it one large one as the picture on thier website shows?
```

---
## \#80 Posted by: jbruce Posted at: 2017-03-07T03:15:57.552Z Reads: 259

```
Would you mind sending a picture if its no trouble?
```

---
## \#81 Posted by: Eboostin Posted at: 2017-03-07T04:26:16.984Z Reads: 267

```
I have no clue, I've been trying to get mine for months now and then I checked the site. It now says 2.1 instead of 2.0 and is no longer discounted. Idk what the difference is. 

Can you post pics of what you received? Kind of jealous you already have yours. I wanted to wrap up my boards at end of January when they were supposed to ship but I've been stuck waiting on them.
```

---
## \#82 Posted by: Michael319 Posted at: 2017-03-07T14:31:25.397Z Reads: 261

```
Looks exactly like the old one with an aluminum heatsink on it.
```

---
## \#83 Posted by: jbruce Posted at: 2017-03-07T17:22:17.982Z Reads: 264

```
ok i take back what i said earlier. i believe you have received a v1 of these which is all the same features as v2 and v2.1 just different form factor. from what i've heard from jeramiah is that v2 (the new form factor) had some problems with pcb routing so they had to get new ones made (v2.1) which are currently being fabricated and hopefully will be done soon. i don't believe anyone will be receving v2 as they had problems. also if you're in a rush and don't care about the new form factor and just want the features you can contact jeramiah and ask to receive a v1.
```

---
## \#84 Posted by: Eboostin Posted at: 2017-03-29T04:22:10.643Z Reads: 265

```
Has anyone heard back on their orders? They were supposed to start shipping on 3/22 and I have not been able to get a response back on the 4 VESCs that I ordered.
```

---
## \#85 Posted by: UserName0 Posted at: 2017-03-29T06:45:12.478Z Reads: 272

```
I just spotted a picture of one in the "no words just pictures thread".  disappointment there is no info on this been scouring google with a giant ace afro pick and I aint found shit.
```

---
## \#86 Posted by: smurf Posted at: 2017-03-29T06:49:42.843Z Reads: 273

```
https://www.instagram.com/p/BRbgkJ9j28G/
```

---
## \#87 Posted by: Eboostin Posted at: 2017-03-29T14:53:19.334Z Reads: 270

```
I don't think that is it.
```

---
## \#88 Posted by: Michael319 Posted at: 2017-03-29T15:11:48.288Z Reads: 269

```
It is. It's the same one I have
```

---
## \#89 Posted by: Eboostin Posted at: 2017-03-29T15:17:56.639Z Reads: 273

```
That's not 2.1. 2.1 has the capacitor as part of the board 

<img src="/uploads/db1493/original/3X/1/d/1d428b7b9bead6fd25fa961ff4fd2e5489add66b.JPG" width="690" height="492">
```

---
## \#90 Posted by: Kaly Posted at: 2017-03-29T15:26:59.198Z Reads: 269

```
The one on the previous picture is the V1.1 
For the V2.1 there is no timetable as of now, that I know of. 
You can email them and inquire about it :-)
```

---
## \#91 Posted by: Eboostin Posted at: 2017-03-29T15:27:48.139Z Reads: 270

```
How thick is the v1.1 you have? @Michael319
```

---
## \#92 Posted by: Kaly Posted at: 2017-03-29T15:42:50.913Z Reads: 270

```
The V1.1 on that pic is the thick version is 22 mm thick
```

---
## \#94 Posted by: Eboostin Posted at: 2017-04-13T17:20:30.869Z Reads: 267

```
The DirectVesc 2 has been postponed for the moment

They will be sending out the V1.1. It sounds pretty robust so excited to get it and get riding!
```

---
## \#95 Posted by: Randyc1 Posted at: 2017-04-21T15:02:54.165Z Reads: 264

```
Anyone have Dimentions of V1.1 in post 85 ??
```

---
## \#96 Posted by: Kaly Posted at: 2017-04-21T17:24:48.067Z Reads: 268

```
I'll post them when I get back home

aluminum heat-sink
65x38x23 without the cap bank

with cap bank 
110x38x23

dim mm
```

---
## \#97 Posted by: Randyc1 Posted at: 2017-04-23T13:30:35.669Z Reads: 259

```
Thanks Kaly !
```

---
## \#98 Posted by: Trizzly Posted at: 2017-04-29T11:58:28.771Z Reads: 248

```
I ordered a VESC 4.12 on 3/28 and haven't heard anything back after contacting them.
```

---
## \#99 Posted by: Pantologist Posted at: 2017-04-29T12:27:58.206Z Reads: 249

```
I think Jeremiah lost it... Seems to be a few incidents happening between him and his customers as stories appear on Facebook and Reddit. If he thinks you support Enertion at all, he will probably never ship to you...
```

---
## \#100 Posted by: Michael319 Posted at: 2017-04-29T15:20:31.580Z Reads: 245

```
That is definitely not true, he has a phone number you can call him at. It is for all of his customers: 650 761-1801
```

---
## \#101 Posted by: scrapheap Posted at: 2017-04-29T15:27:22.887Z Reads: 259

```
Don't think that's true about the Enertion statement. But it seems he is weeding out any customers that post any communications between themselves and his company on the net, canceling their orders, giving them a refund, and putting their names on a blacklist.

I think he bit off more than he can chew...too many projects. He's already working and developing three new boards...
```

---
## \#102 Posted by: Randyc1 Posted at: 2017-06-12T02:15:59.601Z Reads: 250

```
V1.1...They are actually less thick than 23mm<img src="/uploads/db1493/original/3X/d/e/de8d9d39aeb8af27d1f348361c0b1ef33b513175.jpg" width="690" height="388"> !,
Here is a photo next to a .75" ,19.6 mm piece of mdf .
```

---
## \#103 Posted by: mwkeefer Posted at: 2017-06-14T15:23:01.146Z Reads: 247

```

Wow tried to post the following alone:

ESC PORN, HELLA YEAH !!!

And got owned by some Java Script syntax evaluator which realized, doesn't seem like a sentence... so now flipping Bots are Posting Signs that weren't there before, lol

Seriously though, beautiful enclosures... Right??

-Mike
```

---
## \#104 Posted by: chaka Posted at: 2017-06-14T15:56:02.508Z Reads: 244

```
> Seriously though, beautiful enclosures... Right??

We think they look great for their purpose. They are thicker now, 23mm. We also have a fully enclosed version in development that out performs the VESC6 and it is under 2 inches wide.

https://www.instagram.com/p/BUU8teMDBxQ/?taken-by=ollinboardco
```

---
## \#105 Posted by: psychotiller Posted at: 2017-06-14T16:01:51.443Z Reads: 243

```
[quote="scrapheap, post:101, topic:13104"]
But it seems he is weeding out any customers that post any communications between themselves and his company on the net, canceling their orders, giving them a refund, and putting their names on a blacklist.
[/quote]

That's called getting "Jeremiah'd" haha! If it happens to you, you deserved it.
```

---
## \#106 Posted by: mwkeefer Posted at: 2017-06-14T16:11:14.968Z Reads: 238

```
Katch me outside, aight

Rotflmfao, sorry couldn't resist...

 They are straight up ESC porn  though aren't they I freaking love billet shit !!!

Mike

 Hey  seriously though I don't know anybody who's ever had a problem with him  or had their order canceled only was this one guy was like trash talking all over the place about how terrible this that  and the other thing and let's be serious  The guy was a dick,  used guy loosely because this was probably a 12 or 13-year-old ...

Oh wait, that wasn't you {swallows}.. ER um, lol

-Mike
```

---
## \#107 Posted by: scrapheap Posted at: 2017-06-14T16:32:14.404Z Reads: 228

```
There were a thread or two on Reddit about the whole canceling thing...I was surprised too since Jeremiah has been nothing but helpful to me and to others. But there's always that disgruntled customer that's going to make a fuss, so meh.

On another note...@chaka, any possible ETA on that new ESC? :D
```

---
## \#108 Posted by: mwkeefer Posted at: 2017-06-14T17:07:16.069Z Reads: 228

```
 Yeah there is always one I read on re-irritable obstinant customer that's the problem and for some reason I guy seems to think that they can just call somebody out like oh just drag them down like Wawa wow if they make the most noise though get the oil and all they get is "get the hell out of line sale canceled"
```

---
## \#109 Posted by: chaka Posted at: 2017-06-14T18:02:49.922Z Reads: 233

```
The new version is intended for use in electric surfboards with much higher power demands than electric skateboards. We will post some photos and specs in a week or two. Should be a good choice for single drives with hellishly tall gear ratios.
```

---
## \#110 Posted by: hexakopter Posted at: 2017-06-14T18:27:36.337Z Reads: 240

```
[quote="chaka, post:104, topic:13104"]
We also have a fully enclosed version in development that out performs the VESC6 and it is under 2 inches wide.
[/quote]


How do you know they outperform the VESC6 when yours isn't finished yet and you didn't test the VESC6?
This isn't meant as an accusation, but I am interested in what would it do better. Thanks.
```

---
## \#111 Posted by: chaka Posted at: 2017-06-14T18:38:26.210Z Reads: 247

```
This is based on max output, max constant current of our latest heatsink design. VESC6 still outperforms in regard to using very high KV motors and FOC operation due to the third current shunt resistor. You could also add more cooling to the VESC6 to improve high current performance. It really comes down to heat sink design at this point.
```

---
## \#112 Posted by: hexakopter Posted at: 2017-06-14T19:13:48.722Z Reads: 246

```
I think the best heatsink is quite useless when not using the airflow properly. You can see a video I did about that topic here: 
[https://www.youtube.com/watch?v=UwVQQ_LY5bc](https://www.youtube.com/watch?v=UwVQQ_LY5bc)
I think I will do another video comparing the HW4.12 to the HW6.4 as soon as possible.
So what do you mean with more cooling? To add a bigger piece of aluminium, so that it take some more time to heat that thing up without airflow, or a design that uses the airflow (when it is available) in a better way?
What type of MOSFET will you use? In my opinion a more important thing than just the heat sink design.
```

---
## \#113 Posted by: chaka Posted at: 2017-06-14T19:36:53.243Z Reads: 244

```
Try to get your hands on the new VESC tool and run bench tests using the FOC open loop command. You will find that simply increasing the mass of the heat sink increases the max current handling significantly. There is a limit to this, a point where you need to start actively cooling to see more gains.

My design parameters do not allow for active cooling. Designing a component that can be attached to another surface is the goal here. A solid face transfers heat much better to an aluminum bulkhead to air or water much better than a fluted face.
```

---
## \#114 Posted by: Randyc1 Posted at: 2017-06-14T23:24:36.323Z Reads: 233

```
Is the 23mm version the same as the 19mm version i posted a pic of above ?

Do you know people or forum for E-surfboards Chaka? ... something i could be interested in building ?
```

---
## \#115 Posted by: PB1 Posted at: 2017-06-15T06:19:40.925Z Reads: 228

```
@Randyc1 the old Endless Sphere has a section on "electric watercraft" 
https://endless-sphere.com/forums/viewforum.php?f=39&sid=294552d1ecbabc4c57b2bde19b1f1346 
and one big thread about "electric surf board"
```

---
## \#116 Posted by: chaka Posted at: 2017-06-15T14:03:58.285Z Reads: 228

```
Internals are the same just a bit more aluminum. If you want the thicker enclosure let me know, I can send you one from our next batch on the CNC. 

Quite a few people are building water craft using the VESC.  Seems to be a rapidly growing sector with lots of fun design challenges to overcome.
```

---
## \#117 Posted by: Randyc1 Posted at: 2017-06-15T14:10:55.092Z Reads: 222

```
Thanks Chaka , but i think the ones i have will be more than enough for a Double motor correct ? ,..and are only 19mm thick
```

---
## \#118 Posted by: chaka Posted at: 2017-06-15T14:23:37.815Z Reads: 220

```
Yeah you will be fine on those.
```

---
## \#119 Posted by: trampa Posted at: 2017-06-15T14:53:54.740Z Reads: 237

```
You are quite right! Its about the flow of the cooling media. Giving the alloy more mass will only help for a short period of time, until your mass is hot. In that case it will also take a longer period of time until you cooled it down again. 
The positive effect you had in the first place could turn itself against you later. It really depends on the application (short power spikes VS. high continuous Amp drain).
So we didn't go to crazy about the pure mass of alloy since it will also ad weight to the product. You can still screw the VESC SIX to another heat sink with more surface area if you need more cooling. I personally think the VESC SIX is up to the task for many many applications. If it comes to the point where you need more power, a new design, specific for the application is probably the best way forward. You can't nail everything with one design. VESC 6 is the 5KW class. A 5-20KW hardware is something to thing about if you design e.g. nautical equipment. 

I hope we will see some funky designs in near future. It al helps to grow the project bigger.

Frank
```

---
## \#120 Posted by: chaka Posted at: 2017-06-15T15:30:45.326Z Reads: 229

```
One thing you have not considered is the heat sinking effect of having the phase wires submerged in water during testing and benchmarking. The constant current handling is much lower when the phase wires are exposed to air only. The VESC6 is still impressive but it doesn't really output that much power under normal operating conditions.
```

---
## \#121 Posted by: trampa Posted at: 2017-06-15T17:36:50.537Z Reads: 242

```
Benjamin took very long cables and these were also using bullets in the middle. Sure, there is an effect when you cool the cables but that is minor. The cables got so hot, you couldn't touch them. What really has an effect is a good thermal conductivity between the FETs and the heat sink. 
We tested that out.
If the cooling is good 80A continuous is achievable. That is more than enough for a single drive. But maybe we see water-cooling soon...

Frank
```

---
## \#122 Posted by: chaka Posted at: 2017-07-11T17:30:24.950Z Reads: 240

```
Another enclosure option for our Ollin ESC "based on version 4.12 VESC".  This enclosure expands the constant current handling beyond the capabilities of the VESC6.

This is still in development so the finish is a little rough. Might extend the peripherals with cables and seal each end for a more water proof design without any openings on top. Might even design a breakout board for panel mounting the usb. 

<img src="/uploads/db1493/original/3X/5/0/50760ac94b629262f37a1e028df5c0b998f20099.jpg" width="690" height="439">
```

---
## \#123 Posted by: Hummie Posted at: 2017-07-11T17:42:00.192Z Reads: 238

```
The copper cables between the motor and esc are a direct thermal path to the hottest parts and surely there's a lot of cooling potential.  If the motor wires were wide copper foil in a good stream of water or air I bet they could transfer a huge amount of heat away. Right between the two biggest heat producers
```

---
## \#124 Posted by: trampa Posted at: 2017-07-11T17:51:54.959Z Reads: 234

```
True, but unfortunately the cables are always covered in silicone or shrink tube.
The enclosure does a good job transferring the heat away.
If you want to push more amps, its best to go for more, or higher rated FETs.
In a couple of years we might see even better FETs. 
With these Direct FET designs you can push most motors we use to their limits already.
The power we get out of our equipment is already far beyond what average users can handle.

Frank
```

---
## \#125 Posted by: chaka Posted at: 2017-07-11T19:17:10.029Z Reads: 231

```
I suppose you are right, the original v4.12 is perfect for the average rider, but most of us are not average. :) Having a motor controller that dissipates heat more efficiently means lower average temps and longer life for electronics and the added current handling will keep a smile on the face of those who push the limits.
```

---
## \#126 Posted by: trampa Posted at: 2017-07-12T07:39:48.585Z Reads: 232

```
Even riding my boards hard, I barely see any temperatures that matter. I bet you experience the same.
We all know, that a correctly adjusted electrical system is keeping currents low and things cool.
12S in combination with nice gearing and a torque rich motor keeps stuff nice and cool anyway.
In my eyes you always need to think all components in parallel to get good results.
Heat means losses and we don't want that anyway. Cooling away losses is not the solution.
Who pushes 80A continuous on a skateboard? Usually that happens for a limited amount of time only.
The heat sinks of your design and the VESC SIX design swallow that quite well.
There are applications where you want 100-200A continuous, but that is a different ESC design then.
Horses for courses....

Frank
```

---
## \#127 Posted by: chaka Posted at: 2017-07-12T12:17:55.018Z Reads: 222

```
Not everyone uses the vesc at 12s. Believe it or not, there are riders using the VESC at voltage down to 6s. A single motor build at 6s will use around 60 - 80 amps during a good hill climb. You see, not everyone will have a perfectly balanced system. Losses within any system are a compromise and ideally there would be none. What I am concerned with is expanding the usefulness of the base model v4.12 and the v6 and increasing their operational life.
```

---
## \#128 Posted by: skslingo21 Posted at: 2017-07-14T05:33:01.122Z Reads: 218

```
Im building a tramp w/ 6364 2400w 136kv motors. 

I plan to run 2x  6s packs in a series for 12s.

I plan to use two Ollin v 1.1

What GUI does the ollin use for configuration?
How is it recommended to sync two Ollin's? (split throttle signal etc)
```

---
## \#129 Posted by: chaka Posted at: 2017-07-14T13:15:34.584Z Reads: 227

```
The Ollin ESC v1.1 is compatible with the VESC v4.XX firmware. You will need the v2.18 bldc-tool or the new vesc-tool for configuration. To split the throttle signal, easiest way is to use a canbus cable. You can also  use a Y-splitter servo style connector but you need to be sure you are only drawing power from one vesc.
```

---
## \#130 Posted by: chaka Posted at: 2017-07-14T18:00:31.401Z Reads: 228

```
Edit: I assumed too much :) read below.  The consensus seems to think it is best to use the canbus to keep the signal clean.

> I revisited this question of using a Y splitter and discovered something I should have realized a long time ago. We "should" be using another set of headers with its own resistor.  

> Here is a servo tester, notice the outputs at the bottom. Each set of headers has an isolated resistor connected to the PWM signal.  I have been using similar logic on the canbus port/s on our prototype VESC's, figures it is what we need when splitting a recievers signal. Interested in seeing the drawbacks since it is common to just use a y splitter and call it good.

<img src="/uploads/db1493/original/3X/0/c/0ca07d3481dd5ff13dedb3a6d919a0b5e87c60c3.jpg" width="525" height="500">
```

---
## \#131 Posted by: chinzw Posted at: 2017-07-14T18:31:39.381Z Reads: 220

```
@chaka why would you need a resistor for the PWM?
```

---
## \#132 Posted by: chaka Posted at: 2017-07-14T18:49:59.779Z Reads: 216

```
Next time I open up a gt2b receiver I will break it down and explain what at play and how it works. Seems to work either way so I am not sure it matters much.
```

---
## \#133 Posted by: FredSaberhagen Posted at: 2017-07-14T18:54:10.094Z Reads: 218

```
I may be wrong here but generally any time you see split resistors off a shared TX signal there are a couple common reasons:

470 ohm resistors as shown here will slow down the edges a little bit of the PWM signal resulting in less noise (although ~khz not a ton of energy, but concentrated frequency spectrum can be an issue depending on the harmonic)

more likely, the resistance there protects against a fault on the opposite side - meaning one failure wouldn't hang the entire PWM bus from the host side.

The PWM provider doesn't have real strong (low) output impedance and it doesn't know what you're hooking up to it out there in the world... SHOULD be a high input Z buffered stage at your RX side but... not everyone is a good PWM citizen haha
```

---
## \#134 Posted by: chaka Posted at: 2017-07-14T19:02:26.199Z Reads: 210

```
> more likely, the resistance there protects against a fault on the opposite side - meaning one failure wouldn't hang the entire PWM bus from the host side.

 Do you think it is a good enough reason to use something similar when splitting the signal on a receiver? The canbus has proven reliable so I don't think it matters much but some still prefer to split the signal.
```

---
## \#135 Posted by: Blasto Posted at: 2017-07-14T19:21:50.153Z Reads: 222

```
[quote="chaka, post:134, topic:13104"]
Do you think it is a good enough reason to use something similar when splitting the signal on a receiver?
[/quote]

There`s already a RC filter on the servo input of the vesc, 
<img src="/uploads/db1493/original/3X/2/c/2c92ca8100fd2b3c22c1b9ae2e000ac2458e2150.png" width="377" height="82">

Adding more resistance could expose the ppm signal to noise.

If the receiver had it`s own power supply, opto-isolating the PPM signal would be a good solution, but because it is the vesc that provides the power, opto-isolating the signal is useless.

I one way of making sure the vesc is "ppm Y split ready" is by putting a little schottsky diode (low fwd voltage drop) on the 5V. This will prevent the buck converters beating each other up... then again would need to be tested

<img src="/uploads/db1493/original/3X/0/2/02631d0364746fb55148d355ea0bc1b45df34546.png" width="628" height="173">
```

---
## \#136 Posted by: chaka Posted at: 2017-07-14T19:23:20.094Z Reads: 214

```
Yeah I was just looking at that. Still not sure why Benjamin has been warning people to not use a split signal. Or does his warning only concern the VESC 6?
```

---
## \#137 Posted by: Blasto Posted at: 2017-07-14T19:27:20.023Z Reads: 225

```
[quote="chaka, post:136, topic:13104"]
Still not sure why Benjamin has been warning people to not use a split signal.
[/quote]

You can do it, but if you do, HIGHLY recommended to cut the 5V and maybe even the GND from one of the vesc.

you do not want to put both 5V rails in parallel, if one of the rails is slightly higher than the other. One rail will short circuit in to the other, thus overworking it until a failure occurs.

another reason is that you ppm signal becomes weaker, again exposing the signal to noise

[quote="chaka, post:136, topic:13104"]
Or does his warning only concern the VESC 6?
[/quote]

this applies to 4.xx and 6.xx
```

---
## \#138 Posted by: chaka Posted at: 2017-07-14T19:33:57.788Z Reads: 219

```
Yes, that has always been my recommendation to those asking. I do prefer the canbus for the common values in telemetry anyway. Never had a problem with splitting the signal before the VESC but, like you said, they might have built in protections in the ESC's I was using.
```

---
## \#139 Posted by: skslingo21 Posted at: 2017-07-16T03:06:53.550Z Reads: 215

```
Wow, talk about getting the info I asked for, I'm surely in the right place. 

I will split the signal wire to both vesc's, but be sure not share any other terminals. 
I will use only one 5v 1 amp output on one vesc to power the wireless receiver. 

Thank you for your thorough replys!
```

---
## \#140 Posted by: skslingo21 Posted at: 2017-07-27T14:35:37.139Z Reads: 210

```
okay still pondering the canbus or pwm...
Using canbus, can you copy settings to the slave esc?(both motors are identical) Or must you set both individually anyhow?

also does the ollin vesc come precoated in conformal coating?
```

---
## \#141 Posted by: guyguy Posted at: 2017-07-27T14:44:12.764Z Reads: 219

```
I believe so:
https://www.instagram.com/p/BKb1defAMkJ/?taken-by=ollinboardco
```

---
## \#142 Posted by: chaka Posted at: 2017-07-27T14:45:32.389Z Reads: 218

```
The canbus is the way to go if you don't want to worry about which wires to cut. I always save my settings and load them onto the slave VESC. Be sure to list the master as 0 and the slave as 1.  Let us know if you need any help or have trouble finding the bldc-tool software. Our VESC is also compatible with the new VESC-Tool from Ben Vedder so you can use that once it is released to the public.

Your VESC does come with a conformal coating. If you need to do any soldering the coating does not need to be removed. It actually helps and acts similar to flux.
```

---
## \#143 Posted by: scepterr Posted at: 2017-08-15T08:35:49.115Z Reads: 208

```
@chaka
Hey is the PCB file up somewhere?
```

---
## \#144 Posted by: evoheyax Posted at: 2017-08-15T15:17:52.538Z Reads: 201

```
@scepterr  https://oshpark.com/profiles/Chaka
```

---
## \#145 Posted by: akira Posted at: 2017-08-15T15:30:48.435Z Reads: 200

```
The is the regular SMD FET, right ?
No the direct FET version.
```

---
## \#146 Posted by: evoheyax Posted at: 2017-08-15T15:37:20.999Z Reads: 204

```
[quote="akira, post:145, topic:13104"]
No the direct FET version.
[/quote]

I'm assuming so. @chaka can you confirm this?
```

---
## \#147 Posted by: akira Posted at: 2017-08-15T16:51:25.306Z Reads: 193

```
I am just saying this because I had the impression that @scepterr was lookign for the DirectFET version.
```

---
## \#148 Posted by: scepterr Posted at: 2017-08-15T16:52:44.493Z Reads: 196

```
Yeah the file on oshpark is the old version
```

---
## \#149 Posted by: chaka Posted at: 2017-08-15T16:55:34.377Z Reads: 193

```
You might want to wait for the version 6 reference design from Vedder. @Trampa should be able to give you an ETA on that.
```

---
## \#150 Posted by: scepterr Posted at: 2017-08-15T16:59:10.916Z Reads: 193

```
I'll do those too, need a cheap, but better than old  fet option for now 😉
I'll send a free PCB to anybody that can get me the file. :slight_smile:
I'm about a day away from just modifying the original to directfet myself, so if you're a file hoarder now is your chance lol
```

---
## \#151 Posted by: skslingo21 Posted at: 2017-09-01T06:34:22.449Z Reads: 186

```
Thanks, after some playing around, Ive got everything dialed in. 

Its priceless having a differential in the rear as im off-road about half my rides.

**These OLLIN VESCS are MACHINES.** :grin:
I have them sandwiched in foam in a 206 drybox, with active air cooling, and some hot glue to prevent any shorts against the heatsinks. 
Just rebuilt the housing after over 100miles on/offroad. 
Everything was intact! 
My housing is not ideal as there are some stresses on the wires/solder pads
<img src="/uploads/db1493/original/3X/b/8/b80b5f43ec7b4cbdf32b38326763d2f6c13321cf.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/e/0e88f0484aad2391e9e3d181b968e86e2eb8be50.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/d/4/d452da9b4a743c7c61a21ebcfdd6b5d37a3cd863.jpg" width="666" height="500">
Though the solder pads are still intact and seem to be surviving the abuse, thanks to the ultra-flexible stranded wire. 

My next housing for these VESCS will be five star, as they deserve nothing less.
```

---
## \#152 Posted by: skslingo21 Posted at: 2017-09-01T07:23:52.770Z Reads: 190

```
Glamour shot before installation ~105 miles ago. :heart_eyes:

<img src="/uploads/db1493/original/3X/5/2/52ac1d3ea67e6e7717ba3240931f0c38153db7a0.jpg" width="666" height="500">
```

---
## \#153 Posted by: nw-esk8 Posted at: 2017-09-13T19:03:07.153Z Reads: 184

```
Does anyone have any info on what continuous current these updated VESCs are rated at?  I have tried asking around a number of times, but I haven't had any luck getting a response.
```

---
## \#154 Posted by: skslingo21 Posted at: 2017-09-15T04:45:08.143Z Reads: 175

```
Here is a link to the same VESC's I own, WITHOUT the super swank heatsink. :hugging:
It is listed here as 50A constant current...
 Although this sale does not include any additional heatsink. 
http://www.ollinboardcompany.com/product/vedder-s-speed-controller
```

---
## \#155 Posted by: Michael319 Posted at: 2017-09-16T22:11:22.009Z Reads: 171

```
Don't you have the Direct VESC?
```

---
## \#156 Posted by: SpeedyGonzales Posted at: 2018-03-04T23:20:00.027Z Reads: 135

```
Why is this thread dead?
All Direct VESCs sold out.
Is this the end of the world?
```

---
## \#157 Posted by: Michael319 Posted at: 2018-03-04T23:29:07.914Z Reads: 138

```
I believe OllinBoardCo is no longer going to be selling DIY parts. Or at least they're are slowing down for now. Might be bad info tho,
```

---
## \#158 Posted by: SpeedyGonzales Posted at: 2018-03-06T04:55:50.569Z Reads: 130

```
Too low profit margin I guess.
```

---
## \#159 Posted by: scrapheap Posted at: 2018-03-06T05:10:09.248Z Reads: 131

```
More likely, they are pooling all their resources into completes for now. They ARE still a small shop with limited space and are trying to do everything they can in-house, so their ability to make things in huge quantities doesn't really exist presently.

They will probably come back to selling DIY parts, if either one of two things happen: their complete esk8  sales slow down OR they expand.

Though...they still sell SOME DIY parts...but priority is still for their completes.
```

---
## \#160 Posted by: Randyc1 Posted at: 2018-06-03T04:40:40.262Z Reads: 108

```
Is the v1.1 good for 12S and FOC ?![20180529_012014|690x388](upload://gN8xDcIIdROSyxRf7knK3uFVDPg.jpg)
```

---
## \#161 Posted by: willpark16 Posted at: 2018-06-03T04:53:48.789Z Reads: 106

```
Yes but Chaka doesn’t sell them anymore
```

---
## \#162 Posted by: Silvio Posted at: 2018-06-25T15:30:48.049Z Reads: 74

```
Hi @chaka
 I was wondering if it's still possible to get your version of VESC 4.12 with direct fet? 
I'd like to order one on OSH Park but the link is dead. 
I'm running some test on heat transfert and your design just looks fantastic! 
Thanks
```

---
## \#163 Posted by: moon Posted at: 2018-06-25T15:37:38.536Z Reads: 68

```
He is no longer on the forum
```

---
