# Help with charge only BMS wiring

### Replies: 72 Views: 11970

## \#1 Posted by: stuxtruth Posted at: 2016-07-05T23:07:54.890Z Reads: 685

```
Ok. So the instructions seem pretty straightforward for wiring this bad boy up. The problem is that I bought a 45A continuous BMS without thinking when I meant to buy the 60A. By all means... If you think the 45A is enough let me know. I'm running two sk3 270kv 6354 motors with 6s car ESC and a 6s4p lithium ion pack.

Basically I want to figure out how to wire this up for charging only so I can charge with laptop style charger. 

<img src="/uploads/db1493/original/2X/8/823116fe2d820530b21d973eb7d3ee8ee8e53aa1.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/9/91622c2b0290f6346391e7603ca91074c344f6fc.jpeg" width="375" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-05T23:11:34.198Z Reads: 623

```
You might be okay with the 45A continuous as the BMS allows for higher burst current, but I'd be more comfortable running a 45A BMS on a 10S setup. I don't think there's anyone here who knows 100% whether it'll work or if you'll get constant overcurrent problems because it depends on a lot of things such as your riding environment and weight. 

As for the diagram, it's pretty self explanatory, the battery positive (red wire) also goes to your charge port, and the BMS (P-) port goes to the charger negative.

Judging by the balance cable I'm assuming you have the positive lead (red) and 6 negative leads (blacks). The red lead should go to balance slot '6' and the rest will be paired to 5,4,3,2,1. The last black lead is a duplicate of the battery negative so you don't need that. The discharge negative (thicker black wire) goes to the BMS (B-).
```

---
## \#3 Posted by: mason Posted at: 2016-07-05T23:13:09.707Z Reads: 605

```
Off topic, but how long did this take to ship and did you buy it from their ebay store or their site? Thanks.
```

---
## \#4 Posted by: stuxtruth Posted at: 2016-07-05T23:13:43.126Z Reads: 588

```
 #2 on the instructions gave me the impression that the N- port would be used for charging only.
```

---
## \#6 Posted by: stuxtruth Posted at: 2016-07-05T23:14:40.932Z Reads: 575

```
I bought from their site and it took a friggin month.
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-05T23:15:57.389Z Reads: 564

```
Put a space before the # sign to avoid big text. I edited my comment with more instructions, check it out. I think it's saying don't use N- when you're charging/discharging from the same port (P-).

Also CHECK VOLTAGES BEFORE ATTACHING ANYTHING AND EVERYTHING. You can easily blow out your BMS.
```

---
## \#8 Posted by: mason Posted at: 2016-07-05T23:20:26.200Z Reads: 549

```
guess I won't be riding before summer ends :(
```

---
## \#9 Posted by: HTownBomber Posted at: 2016-07-05T23:41:41.691Z Reads: 549

```
I think you can probably run your board for a month or 2 without a BMS. Just be careful to err on the safe side with your charging, set your discharge voltage cut-off with the VESCs and maybe check the voltage of your cells every week or so to make sure they aren't too far apart.

I'm also waiting for a BMS from China. Through eBay.
```

---
## \#10 Posted by: mason Posted at: 2016-07-05T23:47:28.491Z Reads: 538

```
When did you order? Let me know when you get yours :)

I will probably ride without BMS if possible, but I am having an issue with one of my cells. It drops very quickly compared to others. I am hoping the BMS helps to keep this cell in balance, otherwise I will replace it.
```

---
## \#11 Posted by: Namasaki Posted at: 2016-07-06T01:01:53.017Z Reads: 536

```
I ran some tests recently with 6s and dual 6355 230kv motors. 16/36 gears and belt drive
185lb rider going up 10% grade at full throttle 
Real time measurements as follows:
37.38 peak amps 
863 peak watts
So, I would highly recommend that you connect the BMS for discharge as well as charge To get the full protection benefits that it will give to the battery. 
You probably won't go over 45a but if you do,
The BMS has over current protection so it will cut back and You could also put a 40amp inline fuse between the battery and the ESC for extra protection.
```

---
## \#12 Posted by: stuxtruth Posted at: 2016-07-06T01:23:47.181Z Reads: 501

```
Thanks for the info! Maybe I will go ahead and wire it up.
```

---
## \#13 Posted by: Namasaki Posted at: 2016-07-06T01:25:19.134Z Reads: 500

```
sure, try it with the inline fuse at first and if it never blows, then you got it!
```

---
## \#14 Posted by: Namasaki Posted at: 2016-07-06T01:27:05.125Z Reads: 497

```
Really, its just a good idea to have a fuse anyway incase you get a short in wiring or Esc.
```

---
## \#15 Posted by: Namasaki Posted at: 2016-07-06T01:29:20.994Z Reads: 505

```
Get an ATC/ATO fuse holder. There not too big and you can get 40a ATC fuses on Amazon or Ebay
ATC fuses are sealed  ATO fuses are not sealed
```

---
## \#16 Posted by: stuxtruth Posted at: 2016-07-07T00:40:29.387Z Reads: 508

```
Hey does this wiring look right to you guys?

<img src="/uploads/db1493/original/2X/4/4a70a9784094ca60b0824ccb2e9cf93e8c3ee74a.jpeg" width="375" height="500">
```

---
## \#17 Posted by: Jinra Posted at: 2016-07-07T00:51:28.569Z Reads: 510

```
You want the charge port connecting to the BMS otherwise you won't be balance charging, so make sure charger negative goes to P- on the BMS. You may also want an anti-spark switch/loop to avoid nasty sparks when connecting the battery.

As for the ESC's you'll want to wire them in parallel instead of series so have two cables from the BMS and battery positive go to each ESC. Make sure balance lead voltages are right!
```

---
## \#18 Posted by: stuxtruth Posted at: 2016-07-07T00:54:37.879Z Reads: 499

```
Holy smokes. I did it all wrong. Let me re draw this thing.
```

---
## \#19 Posted by: stuxtruth Posted at: 2016-07-07T01:02:37.492Z Reads: 501

```
<img src="/uploads/db1493/original/2X/e/eb94c8e93d597c46ead98928a6cd1aa3912ed57b.jpeg" width="375" height="500">

Like this?
```

---
## \#20 Posted by: Jinra Posted at: 2016-07-07T01:16:16.970Z Reads: 483

```
The other charge cable should be going to battery positive not the bms. Throw in an anti spark and you're set.
```

---
## \#21 Posted by: stuxtruth Posted at: 2016-07-07T01:19:06.654Z Reads: 488

```
Great thanks!
```

---
## \#22 Posted by: massy Posted at: 2016-07-07T11:39:30.681Z Reads: 475

```
Only difference to a "proper"  connection should be to parallely connect batteries to bms and esc.
```

---
## \#23 Posted by: stuxtruth Posted at: 2016-07-07T12:31:52.766Z Reads: 476

```
How would I do that?
```

---
## \#24 Posted by: Jinra Posted at: 2016-07-07T14:11:04.322Z Reads: 477

```
Your recent diagram is already parallel, you're good
```

---
## \#25 Posted by: RideTheIon Posted at: 2016-07-08T06:23:50.070Z Reads: 480

```
I ran into the same problem a year ago. I bought a BMS for charging and the discharge current limiting was only 30 A, which would have majorly crippled my board. My board is a mountainboard so it requires about twice the power of a skateboard to get it moving.

I had overthought the BMS and somehow assumed that the charging and current limiting function was in the same circuit. There not, they are semi-separate.
That what Namasaki meant by “So, I would highly recommend that you connect the BMS for discharge as well as charge”.

I assume your motors can take 2-3 kW per motor. My math says your BMS will limit your power to 1 kW. Your losing about 80% of your motors maximum power.

I'd personally put in at least a switch that would bypass the current limiting function. This way you can flip the switch and if it burns the fuse, then you know you are crippling your board.
Though you might be better off taking advice for the others on this board. I have only a 150 A circuit breaker between my ESC and battery. I fried a Flier ESC and at the same time that ruined my battery :( 
Now I have a pair of VESCs. If you trust your ESC you don’t need to protect your battery.
```

---
## \#26 Posted by: HTownBomber Posted at: 2016-07-15T01:32:30.489Z Reads: 427

```
Ordered June 27th, got it July 13th (yesterday).  Faster than my VESCs, that's for sure. 

Left the obligatory "A+++ SELLER!!! WOULD BUY AGAIN!!!1"
```

---
## \#27 Posted by: mason Posted at: 2016-07-15T01:36:26.139Z Reads: 414

```
I got mine today!
```

---
## \#28 Posted by: stuxtruth Posted at: 2016-07-15T01:37:28.492Z Reads: 406

```
From battery supports?
```

---
## \#29 Posted by: JuniorPotato93 Posted at: 2016-07-15T03:04:39.696Z Reads: 412

```
@Jinra I'm in the process of packing a pack as well, where would I put a on/off switch to cut off power to the board in this set up?
```

---
## \#30 Posted by: Jinra Posted at: 2016-07-15T03:17:36.539Z Reads: 408

```
some bms's come with an e switch so preferably there. If not, after the bms and before the voltmeter.
```

---
## \#31 Posted by: JuniorPotato93 Posted at: 2016-07-15T03:20:55.558Z Reads: 410

```
Thanks @Jinra   Once I have made some progress on this bad boy I'll be posting some pics
```

---
## \#32 Posted by: JuniorPotato93 Posted at: 2016-07-18T04:56:26.638Z Reads: 401

```
This may very well be a silly question but if i intend to use a BMS for charging but discharge through a bypass, will the e-switch on the BMS be rendered useless? I believe the answer is yes once I thought about it but I dont know much about how these things work just yet. If that is the case though, I will have to get a higher amp BMS (80 continuous discharge for 10s4p using Samsung 18650 25R) to be able to use the e-switch to turn off the board?
```

---
## \#33 Posted by: lox897 Posted at: 2016-07-18T05:25:44.220Z Reads: 379

```
@lowGuido can confirm BMS question. @JuniorPotato93 is your CAD design for the kegel available on thingiverse.
```

---
## \#34 Posted by: lowGuido Posted at: 2016-07-18T06:25:58.474Z Reads: 387

```
[quote="JuniorPotato93, post:32, topic:5626"]
This may very well be a silly question but if i intend to use a BMS for charging but discharge through a bypass, will the e-switch on the BMS be rendered useless?
[/quote]


True story.
```

---
## \#35 Posted by: JuniorPotato93 Posted at: 2016-07-18T11:00:11.566Z Reads: 374

```
The CAD will be available today. I made the Thingiverse account yesterday and so it wouldnt let me publish for 24 hours
```

---
## \#36 Posted by: JuniorPotato93 Posted at: 2016-07-18T22:02:26.882Z Reads: 359

```
@lox897 the CAD is available now
```

---
## \#37 Posted by: Eboostin Posted at: 2016-08-10T03:41:27.846Z Reads: 369

```
Why does it go from 7 wires to 6 wires on the BMS connector? @stuxtruth @Jinra  

Apologize if it's a simpleton question, still figuring out BMSs and whether or not I want to use one or use it for charging only.
```

---
## \#38 Posted by: Jinra Posted at: 2016-08-10T04:23:20.305Z Reads: 352

```
the 7th wire is effectly the pack main negative lead. "B-" on the diagram.
```

---
## \#39 Posted by: Eboostin Posted at: 2016-08-10T05:47:03.530Z Reads: 375

```
Ok, thank you!

Some of the BMSs I have looked at have a B- or B0 balance cable in addition to another spot on the board for B- which is why I was confused about dropping to 6 cables. The Evolve BMS is like this https://endless-sphere.com/forums/viewtopic.php?t=70435#p1064672 

I guess the one the @stuxtruth must not be set up that way.
```

---
## \#40 Posted by: Genex Posted at: 2016-08-14T19:12:33.256Z Reads: 426

```


To bring this subject into light again...

I'd like to make a charge only BMS set up for my 6S2P setup with venom lipo's (slightly nicer zippys)  The single plug is going to be a must for me since I will be at college.  I want to use the BMS to ONLY CHARGE, not for discharging, so I would end up getting a less expensive BMS.

I made a circuit diagram that you will see below.  From what I can tell, this circuit is for both charging and discharging, which would require me to have a bms with a high discharge value so it won't limit my motor power. How would I go about making it for charging only, with a bypass so I can avoid the BMS current limit?

Also, I am planning on using one of these adapters to connect my two lipo packs into effectively a 6s pack so the BMS will see it as a 6s.  Would this work, or will I have to wire the balance connectors myself? [http://www.hobbyking.com/hobbyking/store/__9910__2_x_3S_gt_6S_Splitter_JST_XH_5pcs_bag_.html](http://www.hobbyking.com/hobbyking/store/__9910__2_x_3S_gt_6S_Splitter_JST_XH_5pcs_bag_.html)

And if I do have to wire it myself, is this diagram correct?

<img src="/uploads/db1493/original/2X/1/1f87e99866cd373f72ee2554866b32078ba1c87c.gif" width="365" height="500">

And finally here is the circuit diagram

<img src="/uploads/db1493/original/2X/0/055838ca30d11dae1af2b4f358164e11ac911afb.png" width="419" height="500">

Please check to make sure that diagram makes sense.  The bms I am planning on using is something along the line of this: [Ebay](http://www.ebay.com/itm/7s-Cells-24V-20A-W-Balancing-Li-ion-Lithium-18650-Battery-BMS-Protection-Board-/272315777944?hash=item3f67490398:g:y6gAAOSw4s9XkbJG)

It is cheap and probably has less than perfect build specs, but since it is (as planned) going to be for nothing other than balancing the cells while charging I do not see a problem.  If there is one, let me know and I will pick up the same bms that strux had.

EDIT-

I should mention I have had all of this figured out by now, just haven't updated this thread.

To run a Charge Only BMS you will need to follow the diagram above but run the negative from the esc/motor straight to the battery instead of to P-.  You will still attach the negative to B-, but not P-.  The charger does still attach to P- however.
```

---
## \#41 Posted by: jackw Posted at: 2016-09-02T10:14:45.684Z Reads: 456

```
I'm having some confusion too with the wiring of these BMS's.

I have ordered the 12s 60A BMS and am looking for pointers on the wiring.

This is the diagram that they provide:

<img src="/uploads/db1493/original/2X/6/65d7443e0ae741e1d89e4e9e9fa571e432b63cbf.JPG" width="690" height="385">

This is a quick diagram that I have set up as I understand it (Excuse the rushed-ness!).

<img src="/uploads/db1493/original/2X/2/2094476139b90c721d4eb45ce2f0ec8150c53642.jpg" width="375" height="500">
(I labeled it as 80A but I have ordered the 60A).

Is this correct? The balance cables took some mind bending but I think they're correctly wired. If I wanted to use the BMS as charge only (incase the 60A limit is too low for my setup) how would I modify this wiring?

Also, does the AWG of the wiring to the charge port need to be low gauge? Or does it only need to handle the charge current coming in through the charger?

Hope someone out there has used something similar!
```

---
## \#42 Posted by: mccloed Posted at: 2016-09-02T16:18:55.079Z Reads: 473

```
[quote="jackw, post:41, topic:5626"]
Is this correct? The balance cables took some mind bending but I think they're correctly wired. If I wanted to use the BMS as charge only (incase the 60A limit is too low for my setup) how would I modify this wiring? **See below for charge only** 

Also, does the AWG of the wiring to the charge port need to be low gauge? Or does it only need to handle the charge current coming in through the charger? **Just needs to handle the charge current from charger**
[/quote]
I have also corrected your diagram for the Amp limiting wiring.

<img src="/uploads/db1493/original/2X/b/b0d29e643f19c9d3e8921069cade470192c521c0.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/d/d202db1c8084d6cd73a322aa1c422b125dfd6abc.jpg" width="375" height="500">

You could wire it the way you have it, but the main negative and the last negative balance wire are on the same terminal on the battery.
```

---
## \#43 Posted by: Eboosted Posted at: 2017-01-27T06:37:56.027Z Reads: 417

```
[img]http://i.imgur.com/AdtkOc0.jpg[/img]
```

---
## \#44 Posted by: IsTalo Posted at: 2017-01-27T19:06:19.752Z Reads: 402

```
Hi, I wanna buy a BMS too, but tell me, 45A isn't low limit? Because a Skateboard can use more than 60A
```

---
## \#45 Posted by: Eboostin Posted at: 2017-01-28T01:42:36.663Z Reads: 378

```
Just curious, why did you go with two fuses?
```

---
## \#46 Posted by: Eboosted Posted at: 2017-01-28T02:43:00.556Z Reads: 371

```
I saw a wiring diagram, but after some advise I'll live it with no fuse.
```

---
## \#47 Posted by: Eboosted Posted at: 2017-01-28T02:44:24.103Z Reads: 361

```
Yes you need to use a 60A bms for a 10s3p and 80A for 10s4p, nevertheless there are a lot of people running 60A bms for a 10s4p on Samsung 25R with no issues whatsoever
```

---
## \#48 Posted by: IsTalo Posted at: 2017-01-28T10:41:12.066Z Reads: 360

```
But I'm using a 6s1p 6300mah 35c, witch Bms I have to buy?
```

---
## \#49 Posted by: Eboosted Posted at: 2017-01-28T17:23:57.260Z Reads: 352

```
This should be the one you need

http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html
```

---
## \#50 Posted by: IsTalo Posted at: 2017-01-28T22:26:01.520Z Reads: 345

```
Why? And Battery Supports do not ship To my Country! I saw some people using like 15A Bms with Sk3 Motors, How they do this?
```

---
## \#51 Posted by: willpark16 Posted at: 2017-01-29T02:43:57.614Z Reads: 346

```
Use it for charging only
```

---
## \#52 Posted by: IsTalo Posted at: 2017-01-29T08:29:02.773Z Reads: 339

```
Like Soldering the Vesc Cables in Charge Port of Bms??
```

---
## \#53 Posted by: lox897 Posted at: 2017-01-29T10:43:51.548Z Reads: 338

```
No. You only use the BMS to charge the battery, and connect the battery straight to the esc (with a switch in between)
```

---
## \#54 Posted by: IsTalo Posted at: 2017-01-29T12:30:17.254Z Reads: 339

```
<img src="/uploads/db1493/original/3X/6/d/6d5b2942ac83195d615644870d78c1cb9481dfc2.PNG" width="281" height="500"> 
Like this?
```

---
## \#55 Posted by: lox897 Posted at: 2017-01-29T19:38:10.120Z Reads: 326

```
It depends on the BMS. There are a few threads here on how to do it, search how to bypass bms
```

---
## \#56 Posted by: IsTalo Posted at: 2017-01-30T00:37:08.622Z Reads: 318

```
Man, Wait, I want a Bms just for charging, How do I connect the Bms with the Battery? Because I don't want to Burn My Bms
```

---
## \#57 Posted by: lox897 Posted at: 2017-01-30T01:44:09.455Z Reads: 316

```
What BMS do you have? You need to find a diagram on bypassing the bms
```

---
## \#58 Posted by: IsTalo Posted at: 2017-01-30T01:58:15.582Z Reads: 309

```
I don't have, this is why I'm making so many questions hahaha, Tell me, Witch one do you recommend? (WorldWide Shipping Please)
```

---
## \#59 Posted by: lox897 Posted at: 2017-01-30T04:11:30.593Z Reads: 300

```
Battery support or bestech
```

---
## \#60 Posted by: IsTalo Posted at: 2017-01-30T13:35:50.164Z Reads: 299

```
Man, can you explain to me how to buy in Bestech? Their site have no "Buy or Add to Cart" button
```

---
## \#61 Posted by: Namasaki Posted at: 2017-01-30T22:53:35.939Z Reads: 302

```
To Buy from Bestech:
Find the bms you want on their website then send an email to their sales dept asking to buy the bms.
They will contact you and setup the order through email. Their minimum order qty is 2.
```

---
## \#62 Posted by: IsTalo Posted at: 2017-01-30T22:58:31.152Z Reads: 278

```
So, okay, I think I'll divide the price with a friend
```

---
## \#63 Posted by: willpark16 Posted at: 2017-01-31T16:47:48.163Z Reads: 282

```
if you find a decent bms pm me and ill paypal u some money
```

---
## \#64 Posted by: Jammeslu Posted at: 2017-03-22T16:19:23.361Z Reads: 266

```
Hi, I'm on a 8s setup and wondering what bms to use. Will a 45A work or do I need to a 60A?
```

---
## \#65 Posted by: landonkun Posted at: 2017-03-22T22:37:51.038Z Reads: 263

```
It depends on what type of batteries you're using. 8S of what type of cells?
```

---
## \#66 Posted by: Jammeslu Posted at: 2017-03-22T22:38:41.746Z Reads: 262

```
Zippy lipo
```

---
## \#67 Posted by: landonkun Posted at: 2017-03-22T22:40:26.475Z Reads: 262

```
You're gonna have to be more specific. Is it an 8S2P? 3P? 4P? And what's the discharge rating of those? Zippy makes lots of different kinds of lipos.
```

---
## \#68 Posted by: Jammeslu Posted at: 2017-03-23T07:04:23.340Z Reads: 260

```
Sorry, 8s2p 5000mah esch 20C conected in series from Zippy
```

---
## \#69 Posted by: Tamatoa Posted at: 2017-05-06T19:32:04.984Z Reads: 254

```
Hi,

I was wondering if anyone could help me out regarding wiring a BMS for charge only. Please have a look at the picture and I would appreciate any input on if that is how it is supposed to be wired so that does charge only. I hope it is not too messy.

I am confused I bought this pack from China, together with another one with the same components but different cells (LG MG1) which stopped working when I gave a big acceleration. According to the seller I fried the BMS by pulling to much amps. The thing is, after reading posts on how to wire BMS for charge only it seems like they already did it so the BMS handles charge but not discharge. I tried to find the diagram for this BMS but using the reference number all I could find is a website in Chinese with just a picture of the BMS I am adding this picture as well just in case it might help.

<img src="/uploads/db1493/original/3X/a/3/a380b8d88c88fb5628f8d6c3c23dc92aa37c9410.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/6/8/68ae58500aebcc64562638ade44a336080620f12.jpg" width="600" height="418">
```

---
## \#70 Posted by: EvoHub Posted at: 2017-11-07T11:27:18.803Z Reads: 183

```
Hello everyone, do you think you guys could help me figure out how I'm suppose to connect the balance cables on to this BMS balance charger, it's for TWO 4s LiPo batteries = 8s <img src="/uploads/db1493/original/3X/d/f/df409a9bc0a6d9c0e499ba45aed79884acd95515.jpg" width="382" height="500">
```

---
## \#71 Posted by: Falcon87407 Posted at: 2018-06-11T18:23:00.593Z Reads: 117

```
I can't seem to find a good wiring diagram for the below BMS.  It has the B- P- and Ch-.  The Ch- confuses me on charge only wiring.  Any thoughts/Suggestions?

https://www.amazon.com/gp/product/B074WZL5NF/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
```

---
## \#72 Posted by: filipandre95 Posted at: 2018-06-13T19:07:48.500Z Reads: 106

```
Ch- goes to "-" on the charger
```

---
## \#73 Posted by: Falcon87407 Posted at: 2018-06-13T23:11:34.838Z Reads: 104

```
Yea, I figured it out. Also good thing to note, you don't use P-
```

---
