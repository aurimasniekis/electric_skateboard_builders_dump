# 001 &#124; Jet Invasion Voyager-X &#124; Evolve trucks &#124; Dual 6355s 190kv &#124; Custom 10S4p 30Q &#124; Focbox

### Replies: 125 Views: 18789

## \#1 Posted by: egzplicit Posted at: 2017-11-04T18:22:16.298Z Reads: 838

```
Hi,

Time to post pictures from my first build. I entered the esk8 scene this summer when I bought a Boosted V2 Dual+, my first ever skateboard. While I was happy with the board, I quickly learned that 6 miles goes by very fast. Looked around to see what else does the market offer and quickly learned about Evolve and their products. Really enjoyed the double kingpin wide trucks, I was hooked after the first ride. However, I found their battery and specially the controller / remote to be very twitchy. Coming from the Boosted, it was miles behind.

With the above in mind, I started learning about DIY boards and what people are building. I'm a software engineer with some background in electronics so I thought it would be a nice project to try and build one for myself. Since I enjoyed the carving and feeling of the evolve trucks, I decided to go with them.

## Finished board (more pictures below)

<img src="/uploads/db1493/original/3X/7/1/713d8fc3ff13ccf3081104955884faabde38ec4f.jpg" width="690" height="460">

## Parts list

#### DB Longboards Freeride DT 38"
https://www.skatedeluxe.com/en/db-longboards-freeride-38-96-5cm-longboard-deck_p87193

#### Evolve Trucks & Motor mounts
https://www.evolveskateboardsuk.co.uk/collections/bamboo-gtx-at/products/gt-truck-front-or-rear

#### Racerstar 5065 140kv
https://www.banggood.com/Racerstar-5065-BR5065-140KV-6-12S-Brushless-Motor-With-Gear-For-Scooter-p-1110304.html

#### Custom 10s4p 12Ah battery pack using Samsung 30Q
https://eu.nkon.nl/samsung-inr-18650-30q-3000mah.html

#### Enertion @onloop FOCBOX
http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/

#### Enertion @onloop  Nano-X remote
http://www.enertionboards.com/electric-skateboard-parts/nano-x-enertion-2-4ghz-controller/

#### @esk8 Enclosure 
https://store7570530.ecwid.com/#!/Akku-Box-aus-ABS/p/77922661/category=15842017

#### @esk8 vedder anti spark switch
https://store7570530.ecwid.com/#!/Vedder-SparkProtectionSwitch-mit-Sicherung-new-Version-made-by-eSk8-de-kostenloser-Versand-Free-Shipping/p/59817445/category=15842017

#### @rpasichnyk Bluetooth module and metr app
https://metr.at/
 
Few notes about the build:

### Battery

This was very fun to build. Got myself an Arduino spot welder from https://malectrics.eu/product/diy-arduino-battery-spot-welder-prebuilt-kit-v3/ and a cheap 40A / 440CCA car battery. 30Q batteries arrived quickly from nkon.nl, all sitting nicely at 3.6v. I didn't have room for a Bestech 80A BMS so I decided to hook up a cheap one and bypass it. So far I did about 5 charging cycles (using a 42v 2A charger) and everything looks nice, charging stops at 4.21v per module and then cells drops at 4.2v. I'll keep monitoring the BMS behaviour but so far so good.

In terms of nickel strips, I used pure nickel strips @ 12mm wide and .15 thickness. I never found a reliable source for A rating (seller said 40A per nickel strip but in other places I found people saying it's a lot less). I ended up using 2 strips one on top of each other for the parallel modules and 4 strips for serial connections... and, for safety, a nice and thick copper wire that i soldered to the 2nd strip before spot welding it. I'm sure it's an overkill but better be safe than sorry. Everything was then covered in kapton tape. The BMS sits on top of the pack.

### Deck

This was a bit more difficult to find. It had to work with both 97s and AT wheels and it needs clearance for the motors behind it. I used Photoshop to overlay various decks and compare them with the original Evolve one. Found the DB Freeride 38" to be very similar in shape and not too flexible. Once I mounted the motors I found out it needed a bit of shaving so I removed about 5mm from the end to make sure it wasn't touching the motors when carving hard.

### FOCBOX & Nano-X

After finishing the build I tried BLDC in firmware 2.18, Hybrid mode. Initially I forgot to calibrate the nano-x remote (turn on, full throttle, full brake, then turn board on... I know, there's even a sticker that is saying this... thanks @Jinra for pointing this out). After doing everything right I found BLDC in hybrid was good, acceleration and braking very gradual and smooth right out of the box. However, I got FOCBOXes for a reason... upgraded the firmware to @Ackmaniac 3.100 and switched to FOC sensored. My god it's smooth: startup is even better now, no cogging no drama. Even while rolling backwards, it starts like my boosted does. There is almost no noise at all and after tweaking the acceleration curves a bit and playing with ramping times, it's now so good that I would compare the controller/remote with the boosted one: smooth, predictable and fun. The remote feels a bit cheap in hand, but apart from that it's great. I like thumb control so I never tried the Mini remote I had as a backup.

### Motors and settings

I had to switch the connectors since the Racerstars come with MT30 connectors and not bullet ones. The hall sensors connector is also smaller so I changed that as well.

In terms of settings, currently I'm using (per VESC):

Motor max: 40A
Motor min: -40A
Battery max: 30A
Battery min: -10A

Ackmaniac 3.100 in FOC sensored.

I could go higher on the battery but I found that's enough for now and I don't need more. Motors are rated at 34A so 36A is slightly over the spec. They don't seem to get hot at all (no temp sensor) so maybe it's worth pushing them a bit more in the future.

I did a few tests and top speed is 22mph on ABEC11 97s. I could have gone with 200kv motors but I don't really want more speed so I chose to limit myself to 22mph by picking these 140kv variants.

### Pictures

<img src="/uploads/db1493/original/3X/a/a/aa970e03032b18eaec162512bf41c056ffc67aeb.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/d/2/d281a47816769e9387e0f897182f3cfef9ee5e9c.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/b/4/b48e573798134b5b1ebb7398d88c80d52f721ac9.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/b/3/b347ac6ae8e82a26c491466f0c5a8c1f2048c1b1.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/b/6/b60494e45e628e6a5eaca7a16448b8c3f9339882.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/7/9/799411002ac124883a272c8ec844bb18843bf3f0.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/9/6/9600cf4975ea7f1195bbfda51e7ba77d600488de.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/2/d/2de8a029726596cc417b4d15d56b03b3c8a8add1.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/6/7/67ed372ec1ad3bd8368033871a5917a0edc47324.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/d/0/d0fb46192a3f40e4400b2f9c12efff18b91460ed.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/7/2/72f149314ad84e9bf0a77c579417017e2279e9f2.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/5/3/53a941b43e9ceae1c7f405cc920ce68f326bdc48.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/0/8/08dfedf492fca51b02c530164e9bbeb35100d2aa.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/3/d/3dccf98e63819cede25ea687ee902e0f4ebbce45.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/9/1/9145432d7728238a22c2bf5f53f81992708f5e7d.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/7/2/72c24fb7a2f61c80968909516449078157e32c69.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/2/1/21a1176ee22917591ae6586d60264a0ba8189aa5.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/b/4/b4ed3ec285abce09d926e4ce96ea036be970e849.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/9/8/988415235c8bf95a5d5ec571220e407aa80c0268.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/f/6/f6e3cfa150acca2d989cf0baf6fc6ae46cda05c5.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/f/c/fc5b16f06b11a5ceb27e2bdeece18f304100998a.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/7/1/713d8fc3ff13ccf3081104955884faabde38ec4f.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/d/5/d5a75451e537f74372992b2489f3663ccb68fe5b.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/0/9/09603b39aca1075304b0153868f29e7a198b13ed.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/1/4/14b21260ec6d9aa4b113a6bcb0af86c8b994dd2d.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/d/1/d1a24729be03e059c9b60ad6087e51c27693907a.jpg" width="690" height="460">
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2017-11-04T18:28:56.055Z Reads: 622

```
That is one beautiful build
```

---
## \#3 Posted by: Rinzler Posted at: 2017-11-04T18:47:52.320Z Reads: 616

```
Sweet build man, looks beautiful.
```

---
## \#4 Posted by: pixelsilva Posted at: 2017-11-04T20:24:26.984Z Reads: 603

```
Red light glow fantastic over red motors. What Gen are them mounts?
```

---
## \#5 Posted by: egzplicit Posted at: 2017-11-04T20:51:45.899Z Reads: 590

```
Thank you! Gen 3 mounts.
```

---
## \#6 Posted by: Quezacotl Posted at: 2017-11-04T20:55:56.385Z Reads: 567

```
Nice build.

What worries me, you have a lot of room for parts to shake around and things can damage the cells when shaking there. Unless you have sturdy paddings there.

I have had a three of those cheap BMS-modules, and each one has failed easily. They tend to go poof while charging. Cannot handle even the slightest voltage offset. Might be that i am the unlucky one with all the bad modules though. :smiley:
```

---
## \#7 Posted by: mccloed Posted at: 2017-11-04T21:05:54.094Z Reads: 526

```
Nice Build! Really clean looking. I ,too, will warn you about that BMS. I used it for charge only and it killed some cells on two of my boards.
```

---
## \#8 Posted by: Jedi Posted at: 2017-11-05T02:15:47.692Z Reads: 511

```
Great pictures!
```

---
## \#9 Posted by: mrjonnyjones Posted at: 2017-11-05T10:05:08.892Z Reads: 509

```
Bravo dude, this is what an actual Evolve board should have been from day one!
```

---
## \#10 Posted by: MontPierre Posted at: 2017-11-05T11:02:34.279Z Reads: 516

```
Wow! Neat! Any chance you could link motor mounts? I looked at Evolve website but can only find mount plates ... 

Secondly - what is your hardware for fixing the enclosure? I see you have drilled through - are you having problems with nuts unscrewing due to vibrations?
```

---
## \#11 Posted by: BoostedBuilder Posted at: 2017-11-05T14:59:00.753Z Reads: 511

```
These are the mounts he is using:
https://evolveskateboardsusa.com/collections/gt-bamboo-parts/products/gt-motor-plate
```

---
## \#12 Posted by: briman05 Posted at: 2017-11-05T18:05:16.209Z Reads: 481

```
Minus the wheels, trucks and shape of the deck that is what I want my board to be. I’m looking at 200kv racerstar motors. What motor pulleys did you use the 15 tooth for the motors?
```

---
## \#13 Posted by: Insanity_Wins Posted at: 2017-11-06T17:42:17.740Z Reads: 469

```
How much did this build cost? And would you mind doing a tutorial video on how to build it?
Really want a board like this one
```

---
## \#14 Posted by: oct0f1sh Posted at: 2017-11-06T18:00:02.299Z Reads: 476

```
Hey what belts did you use? I'm using the same trucks and mounts but I didn't want to pay for the more expensive evolve belts.
```

---
## \#15 Posted by: Jebe Posted at: 2017-11-06T23:06:06.941Z Reads: 485

```
http://www.electric-skateboard.builders/t/rudolph-arbor-axis-gullwing-evolve-sidewinders-ollin-200kv-dual-motors-vescs-10s4p/11400/6?u=jebe

I had to offset the brackets to fit this onto my arbor and also onto the gen 2 evolve.

<img src="/uploads/db1493/original/3X/0/8/08ae49fb6dcc75e91f1341b90143d80ac1dff331.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/7/d/7d42f906d2d3ba6e9d17c8a207862cd4ba649ec6.jpg" width="281" height="500">

The arbor doesn't have too much flex - Am just over the sidewinders. Have an evolve for that. Have installed the sidewinders and Ollin 200kv's on an evolve gen 2 and will be trialling jacobs hubs motors on the arbor.
```

---
## \#16 Posted by: egzplicit Posted at: 2017-11-07T12:29:56.153Z Reads: 448

```
@ARetardedPillow @Rinzler   @Quezacotl @mccloed @Jedi @mrjonnyjones @MontPierre  thanks!
```

---
## \#17 Posted by: egzplicit Posted at: 2017-11-07T12:30:04.963Z Reads: 459

```
@Quezacotl that picture is misleading, I was just setting the software so nothing was properly mounted inside the enclosure. 

I agree about the BMS not being the best one. I've monitored all charges so far and charger goes green when cells are at 4.22v, they then settle to 4.2v. So far so good. I'm talking to Bestech in order to buy one of their smaller BMSes to be used bypassed. I have their HCX-D223V1 but it's too big to fit in this build. Once I get a smaller bms from them, i'll fit that. 

@MontPierre I drilled through yes. I got countersunk bolts from here http://www.ebay.co.uk/itm/M3-M4-M5-M6-M8-BLACK-SOCKET-COUNTERSUNK-HIGH-TENSILE-BOLT-ZINC-NYLOC-NUTS-WASHER/192077433917?ssPageName=STRK%3AMEBIDX%3AIT&var=491966486164&_trksid=p2057872.m2749.l2649 and they come with nyloc nuts so they don't unscrew under vibrations. Alternatively you can use thread lock. 

@briman05 I used these: https://www.banggood.com/Racerstar-Motor-Gear-Red-For-BRH5065-BRH5045-Brushless-Balancing-Scooter-Motor-p-1139957.html . Loctite and with grub screw.

@Insanity_Wins i have no video, sorry. I haven't calculated the price but it's around £1000 ish.

@oct0f1sh unfortunately I paid evolve for their belts. You can use HTD 5M 15mm ones but not sure about length, 265mm or 255mm i think. When these wear out I'll give HTD a go.

@Jebe yeah, I had to file down 5mm from the deck. I've got another one coming that is slight longer and i wanna give that one a go (Boosted is 42" so i kind of got used to a bigger deck). 38" and foot pockets feel nice but I would want a 40" deck so I'll see if this new one will work. The arbor looks sweet but you have to modify it to fit the motors... and I wanted drop through mount.
```

---
## \#18 Posted by: briman05 Posted at: 2017-11-07T14:02:34.303Z Reads: 431

```
coudl you give me the set screw size for the gear.  I'm sure I have one laying around my work.
```

---
## \#19 Posted by: egzplicit Posted at: 2017-11-07T14:55:29.921Z Reads: 441

```
It’s M3 (3mm) and I used a 8mm long one and filed it down by 1 or 2 mm. The hole on the pulley is wide and if your grub screw is pointy it won’t fill it properly. I tried just the grub screw (not filed) and I had a play after riding for 2km. It was holding it in place just fine but there was play. Second try I filed it down, loctite the pulley to the shaft then screw the grub screw in and used thread lock on it. 

Also make sure to not over tight it and f0ck the hex head otherwise it will be a pain to take it out. I had to cut one in order to remove it :frowning:

<img src="/uploads/db1493/original/3X/f/5/f5b4e5358381b5e6cc1c05b8055f96c761e3f220.jpeg" width="375" height="500">
```

---
## \#20 Posted by: Lionpuncher Posted at: 2017-11-07T17:41:49.966Z Reads: 432

```
 AWESOME build man. Looks great!
```

---
## \#21 Posted by: briman05 Posted at: 2017-11-07T19:05:52.565Z Reads: 417

```
I just looked up different set screws and there is one called a dog point set screw it has and extend flat piece that keeps everything aligned
```

---
## \#22 Posted by: egzplicit Posted at: 2017-11-08T09:16:20.851Z Reads: 425

```
Thanks for letting me know, dog point is what you want. I used these http://www.ebay.co.uk/itm/M3-M4-M5-M6-A2-Stainless-Cone-Point-Grub-Screws-Hex-Socket-Set-Screw-Din-914-/272342289921 and filed them down, I didn’t know dog point is a thing :slight_smile:
```

---
## \#23 Posted by: bullrider12 Posted at: 2017-11-08T11:34:17.380Z Reads: 423

```
Can you show me a detailed picture of your sensor wiring? :slight_smile:
```

---
## \#24 Posted by: egzplicit Posted at: 2017-11-09T22:34:58.214Z Reads: 432

```
<img src="/uploads/db1493/original/3X/a/8/a8b516a5b51f99aa90688a996670c02889d26b35.jpeg" width="667" height="500">

<img src="/uploads/db1493/original/3X/1/3/135706661a599d2b61b355147461511f2050ff4f.jpeg" width="666" height="500">
```

---
## \#25 Posted by: bullrider12 Posted at: 2017-11-09T22:38:01.888Z Reads: 409

```
Thanks a lot :slight_smile:
```

---
## \#26 Posted by: egzplicit Posted at: 2017-11-09T22:38:31.444Z Reads: 403

```
No worries. Added a 2nd picture where u can see all wires.
```

---
## \#27 Posted by: koralle Posted at: 2017-11-09T22:40:37.681Z Reads: 407

```
Can you please elaborate on your decision on these motors? How has your experience been? I just see so many motors for >100$. Are they a lot better`?
```

---
## \#28 Posted by: pixelsilva Posted at: 2017-11-09T22:44:38.964Z Reads: 415

```
Nope. The ones you mention resemble like an 8. The ones he is using are different. Take a closer look....

https://www.electric-skateboard.builders/uploads/db1493/original/3X/d/1/d1a24729be03e059c9b60ad6087e51c27693907a.jpg
```

---
## \#29 Posted by: egzplicit Posted at: 2017-11-09T22:56:25.798Z Reads: 406

```
Sorry I missed that question. Mounts are gen 3 evolve stock, @BoostedBuilder is right.
```

---
## \#30 Posted by: Toleg Posted at: 2017-11-10T00:47:45.967Z Reads: 402

```
this built is a blast... trying to do a similar one :slight_smile:
good job :slight_smile:
```

---
## \#31 Posted by: GrecoMan Posted at: 2017-11-10T00:49:50.396Z Reads: 403

```
oooo I'm already subbed to you on youtube... whens the video?
```

---
## \#32 Posted by: egzplicit Posted at: 2017-11-26T11:11:54.480Z Reads: 405

```
I'll make one at some point :) I need a rider so I can do the shooting.

Until then: 

https://j.gifs.com/AP6pXp.gif
```

---
## \#34 Posted by: egzplicit Posted at: 2017-12-17T16:04:24.738Z Reads: 392

```
New grip tape, vinyl wrap on the bottom and rubber seal:

<img src="/uploads/db1493/original/3X/5/9/5960c83a3c8934a342452829a3b14fdc492e44c1.jpeg" width="690" height="460">

<img src="/uploads/db1493/original/3X/8/e/8ea7b093cc9d63c611cf8c8d9f93191e3a8b5d38.jpeg" width="690" height="460">

And some 107s that I still haven’t tested due to bad weather:

<img src="/uploads/db1493/original/3X/5/1/519899209c120c41a8d870b31d2c8a26230c1d86.jpeg" width="690" height="460">

<img src="/uploads/db1493/original/3X/9/2/926f8be6059c013b46c78922bfe63c69ca3f9a2e.jpeg" width="690" height="460">
```

---
## \#35 Posted by: Sender Posted at: 2017-12-17T17:32:16.580Z Reads: 380

```
I look forward to hearing your preference of the pneumatic or those 107s!  Such a great build man
```

---
## \#36 Posted by: jdnicholson Posted at: 2017-12-17T23:34:03.864Z Reads: 373

```
@egzplicit Love the build!
How are you finding the racestar motors? Do they have enough power for you?
```

---
## \#37 Posted by: Sippahodge Posted at: 2017-12-18T01:14:00.360Z Reads: 364

```
Nice build, I'm using mostly the same stuff. What connector did you need to change the motor sensors too for the focbox?
```

---
## \#38 Posted by: navgor Posted at: 2017-12-18T02:29:53.597Z Reads: 365

```
Oh. My focbox's have the T where the H1 is. I was getting detection errors. Looks like they labeled my batch wrong! I have the same motors btw.
```

---
## \#39 Posted by: egzplicit Posted at: 2017-12-19T08:36:15.602Z Reads: 377

```
@Sender due to UK weather I think my first ride on 107s will be next year. Even when it doesn’t rain it’s constantly wet on the roads and AT does a much better job handling that compared to urethane. Sometimes it’s so slippery (at 1C) the rear wheels lock under really hard braking.

@jdnicholson I like these motors, with 140kv and FOC I get 20mph top speed on AT (15T/66T) and 22-23 on 97s (15T/32T). On 107s it should be slightly more at around 25-26mph but I still have to test that.

I increased motor max amp to 60A and there is plenty of torque, accelerated faster than an evolve in GT (did a drag race once) and Boosted. Overall I’m impressed giving the price of these motors. One motor has developed a ticking noise when not under load (with belt and wheel you can’t hear it but without you can slightly hear a tick tick) but Banggood was kind enough to already send a replacement. I haven’t changed it because it still works just fine but i have a 3rd one just in case. If you need more top speed maybe 200kv is a better option but some torque will be lost. However, overall these motors are great.

@Sippahodge I just cut the hall connector and soldered a jst 2.0mm to fit the focbox. 

@navgor yes some batches had the labels wrong, T is next to 5v and not GND.
```

---
## \#40 Posted by: treenutter Posted at: 2017-12-20T20:16:57.896Z Reads: 382

```
Great build thread @egzplicit ! What camera are you using for your photos? They are really sharp and vivid! Your build has a similar look to one I did years ago, before evolve had parts for sale and we were all using kid's nordic rollerblade wheels lol!

http://www.electric-skateboard.builders/t/the-village-build-s9-faultine-paris-195mm-sk3-6364-diyes-mount-8s-vesc-127mm-pneumatic-wheels/292
```

---
## \#41 Posted by: egzplicit Posted at: 2018-01-13T12:59:57.637Z Reads: 372

```
Thanks! I'm using a Sony A6500 and one external flash to take the pictures.
```

---
## \#42 Posted by: egzplicit Posted at: 2018-01-13T13:11:19.130Z Reads: 385

```
Decided to do some upgrades... the RacerStar are great motors for the price and do have good power but @okp did some great custom mounts for evolve trucks that allow you to fit 63mm motors so I just had to give them a go.

So a marriage between @okp UniK mounts and eskating.eu 6355s 190kv 3510W motors just happened:

![Photo 12-01-2018, 11 35 13|690x459](upload://fzRgk8TDXgw20qMyNJcgsFG4SRI.jpg)

![Photo 12-01-2018, 13 20 20|690x459](upload://nhmRCsrqFaVrRdJwFmCYdYcXiMh.jpg)

![Photo 12-01-2018, 15 06 30|690x459](upload://7SJK4yWiIXpiuI6zqq903Cf1wGz.jpg)

5.5mm bullet connectors on the FocBoxes:

![Photo 13-01-2018, 12 35 42|666x500](upload://uPgaPM8YGou4LQ5UgzouUUrywYh.jpg)


The original bullet connector solder job on the focboxes was pretty bad tbh, this is how it looked once I took one out:

![Photo 12-01-2018, 17 58 41|575x500](upload://aN2t1rIJribEWk2A7mnVsXyaaTV.jpg)

Wasn't impressed at all.

Anyhow, it's time to do some motor configuration and detection. I still won't be able to test the new setup due to needing longer belts so I'm currently waiting for a few that should be here next week.

I also got some 36T pulleys from @johnny_261, 15/32T was working fine on my old 140kv motors but for the new 190kv it's just too fast. Specially on 107s [the calculator](https://tinyurl.com/y6uvdxk3) shows 34mph... I really don't wanna try that. 

New specs with the upgraded motors should be:

Street setup with

* Abec 107s on 15/36T pulleys: 30mph top speed
* Street setup with Abec 97s on 15/36T pulleys: 27.5mph top speed
* AT setup with Evolve tyres on 15/66T pulleys: 27mph top speed

Time to do vesc settings now...
```

---
## \#43 Posted by: DavidBanner Posted at: 2018-01-13T13:14:31.281Z Reads: 359

```
Looking good!
```

---
## \#44 Posted by: briman05 Posted at: 2018-01-13T19:06:23.691Z Reads: 361

```
Upgrading already I saw this on the eskate page on Facebook
```

---
## \#45 Posted by: egzplicit Posted at: 2018-01-28T17:17:43.922Z Reads: 356

```
Quick speed test on the new 6355s motors with 107s ABEC 11 and 15/36t pulleys. 27mph reached around the 30 second mark.

https://www.youtube.com/watch?v=BhWgtjIJLUY
```

---
## \#46 Posted by: egzplicit Posted at: 2018-02-18T17:36:42.370Z Reads: 346

```
Did a quick video of the board:

https://www.youtube.com/watch?v=tBouSTJ93QY
```

---
## \#47 Posted by: Apolo Posted at: 2018-02-18T18:11:20.841Z Reads: 336

```
BRO YOU'RE TALENTED. 

The pictures were insane, that video too!
```

---
## \#48 Posted by: davidbonde Posted at: 2018-02-18T19:05:56.681Z Reads: 325

```
Cool - Thats not a quick video to make! Must have taken tiiiime to edit :stuck_out_tongue_winking_eye:
```

---
## \#49 Posted by: JonathanLau1983 Posted at: 2018-02-18T20:14:57.150Z Reads: 323

```
Awesome build! 
Pleasure meeting and riding with you and the guys/gals on Saturday. Thanks for letting me borrow your power bank for a bit, looks like my issue could be a motor phase wire break though not so much remote battery.
```

---
## \#50 Posted by: LAVAMAN Posted at: 2018-02-18T22:55:58.161Z Reads: 315

```
Really nice for a first build! Very clean. I am always impressed by the fabrication and building skills of the users of this forum.
```

---
## \#51 Posted by: Riako Posted at: 2018-02-19T09:41:01.450Z Reads: 317

```
Brrriiiiilliant clip ! So cool to watch. Well done :v: 
we all should make video presentation like for our board !
```

---
## \#52 Posted by: egzplicit Posted at: 2018-02-19T10:56:03.478Z Reads: 316

```
Thanks guys. @JonathanLau1983 glad you found the issue, better fix that before it fries the controller!
```

---
## \#53 Posted by: JonathanLau1983 Posted at: 2018-02-19T12:23:45.144Z Reads: 313

```
Had the motor apart last night and it seems fine, so I think it's the other end leading to the ESC. Fingers crossed I can get it done by Friday for Critical Mass.
```

---
## \#54 Posted by: Bjork3n Posted at: 2018-02-27T16:33:27.571Z Reads: 308

```
Whats the lenght on your enclosure? (never mind found it in your part list, shame on me)
How big enclosure could you fit on there? How long is the part where a enclosure can be fitted?
 
Will a 570mm enclosure fit?
```

---
## \#55 Posted by: Slipstriker98 Posted at: 2018-03-03T22:02:19.159Z Reads: 305

```
[quote="egzplicit, post:42, topic:37352"]
Abec 107s on 15/36T pulleys: 30mph top speed
[/quote]

What motor drive gear are you using? 15 teeth, could you tell me the width and where you got it from?
```

---
## \#56 Posted by: Esk8t.nz Posted at: 2018-03-04T09:15:24.761Z Reads: 292

```
Mint build.. will be following..
```

---
## \#57 Posted by: jdnicholson Posted at: 2018-03-13T02:07:26.145Z Reads: 298

```
@egzplicit I have put together a similar build using dual 6374 motors on the unik evolve mount. My street setup works well. However, the stock 360mm belt for the evolve AT setup won't fit, its too tight. The original evolve motor pulley is much smaller than the normal keyway pulley that I can see you are using as well. 

How are you running your AT setup? Did you have to but a longer belt? 

I was thinking I'd go up to a 365mm or 370mm belt but I cant find anyone that sells one.
```

---
## \#58 Posted by: egzplicit Posted at: 2018-03-13T12:32:43.858Z Reads: 288

```
These are the lengths you need:

15/32T = 265mm belt
15/36T = 280mm belt
15/66T = 375mm belt (this is for AT setup)

I think 370mm would also work but I used 375 with the motors almost all the way back and the tension is spot on. I got my belts from a UK supplier: http://www.bearingboys.co.uk/5M-Section-5mm-Pitch/3755M15-Timing-Belt-6091-p
```

---
## \#59 Posted by: egzplicit Posted at: 2018-03-13T12:35:36.177Z Reads: 283

```
[quote="Slipstriker98, post:55, topic:37352"]
What motor drive gear are you using? 15 teeth, could you tell me the width and where you got it from?
[/quote]

I use https://eskating.eu/product/custom-htd-5m-12-to-20-teeth-steel-motor-pulley-in-9121520-width/ custom steel pulleys with no overhang (otherwise the overhang touches the AT wheels). U can use ones with overhangs but not on AT wheels.
```

---
## \#60 Posted by: egzplicit Posted at: 2018-03-13T12:37:00.815Z Reads: 285

```
[quote="Bjork3n, post:54, topic:37352"]
Will a 570mm enclosure fit?
[/quote]

I don’t think so. I’m away on holiday and don’t have the board with me but 520-540 I think was the max. I can measure when I get back home.
```

---
## \#61 Posted by: Bjork3n Posted at: 2018-03-13T12:57:30.225Z Reads: 292

```
No worries, i eventually found the measurements! 
Using the same deck now, its awesome ;)
```

---
## \#62 Posted by: Bjork3n Posted at: 2018-03-16T19:25:52.463Z Reads: 283

```
Sorry posted in the wrong thread....now carry on
```

---
## \#63 Posted by: davidbonde Posted at: 2018-03-16T22:57:14.253Z Reads: 297

```
[quote="egzplicit, post:1, topic:37352"]
The hall sensors connector is also smaller so I changed that as well.
[/quote]


What did you change them to? I am about to install this motor with a focbox and would appreciate that help. The motor sensor comes with 5 wires and the focbox plug have room for 6. 

![IMG_6421|375x500](upload://b6q2nsBdxj348FOzapf6IDiQfov.JPG)
```

---
## \#64 Posted by: egzplicit Posted at: 2018-03-16T23:32:51.494Z Reads: 293

```
I got 6 pins plug from eBay and cut the original
one and extended the wires, see above: http://www.electric-skateboard.builders/t/first-build-db-freeride-dt-38-evolve-trucks-dual-racerstar-5065-140kw-custom-10s4p-30q-focbox/37352/24?u=egzplicit

The extra one is for motor temp, the racerstars don’t have a temp sensor so just skip it.
```

---
## \#65 Posted by: davidbonde Posted at: 2018-03-16T23:48:06.058Z Reads: 293

```
Thanks. I missed those pictures!
```

---
## \#66 Posted by: Idea Posted at: 2018-03-31T22:10:30.417Z Reads: 287

```
Nice build :)

What is your maximum range on the 10S4P battery pack?
```

---
## \#67 Posted by: egzplicit Posted at: 2018-03-31T22:48:51.315Z Reads: 282

```
Depends on wheels used. I recently switched to 6355s and haven’t done a full ride to 0% but with the old 5065s I did a 20 miles on ATs with 5% left and on paper should be close to 28-29 miles with 97s wheels.

I see about 23-25 Wh per mile with ATs (15/66t pulleys) and 16ish Wh per mile with 97s (15/32t). The bigger 107s are somewhere in between, at 17-19Wh/mile with 15/36t or 15/38t.

Once the weather improves in the UK, I’ll test the current 107s (15/38t) with the 6355s and see how much I get.
```

---
## \#68 Posted by: Idea Posted at: 2018-04-01T06:35:30.483Z Reads: 270

```
Thank you for the answer, that's enough for me ...

I have the same packet of batteries in my board but built with  LG HG2 and my range is much smaller, 19km on AT wheels, less than 12 miles :frowning:
```

---
## \#69 Posted by: egzplicit Posted at: 2018-04-01T08:57:08.667Z Reads: 274

```
Umm, that can’t be right. Hg2 are also 3A each and if u get 12 miles that’s 35-36Wh/mile. Something must not be right, even when I did acceleration tests after switching the motors (with lost of start - stop at full throttle) I didn’t use more than 28Wh/mile...

Maybe degraded cells or a bad one in one in the pack? If you have a BT module you could check real consumption and see if it’s actually using that much or if the pack is damaged..

What configuration for pulleys? And what motors?
```

---
## \#70 Posted by: Idea Posted at: 2018-04-01T21:47:12.687Z Reads: 273

```
My batteries are new, I bought them at www.fasttech.com so they are rather original.
The condition of all cells is also good, I controls them through BMS with the BT module.
I do not want to clutter up your topic so I do not include screenshots

The problem is rather the current consumption by the motors

My motors are SK3 6364 190kV (without sensors)
ESC - VESC 4.10
The gear ratio is 15/72

I do not have any experience with VESC yet, so maybe this is a configuration problem.

I am waiting for a special BT module for METR application, but maybe it will install a standard BT module beforehand to check the power consumption with another application
```

---
## \#71 Posted by: egzplicit Posted at: 2018-04-04T08:32:05.308Z Reads: 267

```
Yeah, your consumption seems rather high and I don’t think it should be like that. Riding style and terrain matters but on a flat surface I don’t think it should be higher than 28Wh/mile. I don’t have experience with eMTBs but on my 15/66t with 7” pneumatics on 6355s with 78kg rider and 10.5kg for the board I’ve never seen anything higher than 27-29Wh (during testing with lots of hard acceleration) and 25-26Wh during normal riding.

I would put the Metr module and app and record a session to get more details like real time amps and such. The 72t pulley might also cause this (depending on size of the wheels as well) but not sure...maybe losses in the cables, things getting hot, etc?
```

---
## \#72 Posted by: Idea Posted at: 2018-04-04T08:51:11.779Z Reads: 281

```
Thank you very much for your answer,

Maybe VESC does not like SK3 6364 motors? Without load, the motors take 5-6A (together)
![image|375x500](upload://uoJRBqA6fAWfic1XVmLgojDnv4Q.jpg)

or maybe my batteries have a fictional capacity :/

Today I will have a BT module from METR, so I will be able to take measurements :)

I builds another board using:
Samsung Q30
Racerstar motors 140kV
Focbox
And gearbox so I count on better range :D

![image|565x499](upload://t7AEi2D3kR94JMiQnEzK2MKmSWb.jpg)
![image|612x499](upload://2sa79raCu5ffbltGtzfxixIlpBA.jpg)

but that's another topic ...
```

---
## \#73 Posted by: Powadangaboards Posted at: 2018-04-04T09:32:02.731Z Reads: 260

```
Thats a topic i cant wait to find out more about :slight_smile:
```

---
## \#74 Posted by: egzplicit Posted at: 2018-04-04T09:53:04.196Z Reads: 266

```
[quote="Idea, post:72, topic:37352"]
Without load, the motors take 5-6A (together)
[/quote]

I’ll check on mine so we can compare. Currently have 15/38t with 107s but when I’ll switch to ATs will check amps at full throttle with no load. 

Yeah the BT module is really useful in debugging stuff, you will be able to check how many Wh and As are actually used by the motors and see if you have losses along cables and connectors or if battery is not performing as it should. As a bonus you can create a TCP/IP proxy and connect the PC vesc tool via a phone connected to the same network and via BT to the module. Really useful if you wanna make changes without physically using a USB cable (and taking enclosure off).

Oh that build looks very interesting, curious as well, can’t wait for the thread and some impressions. And noise levels :slight_smile:
```

---
## \#75 Posted by: riva_00 Posted at: 2018-04-04T15:52:16.814Z Reads: 260

```
Evolve has been interesting on it's youtube channel regarding weekly tips and such, recently they covered how riding in "fast" mode used way less amps that the "GT" mode, and that's how they do their longer distance runs (along with push starting).

Can both of you post your VESC setting please? I'll want to compare with mine for range in the future (15/66 - 150mm pneumatics, 2x 5065 motors)
```

---
## \#76 Posted by: Guacamoleface Posted at: 2018-04-04T16:00:02.107Z Reads: 249

```
I may have an erection right now. Just want you to know that, thoose that gearsystem looks juicy. That your own creation?
```

---
## \#77 Posted by: egzplicit Posted at: 2018-04-04T18:04:52.196Z Reads: 252

```
[quote="riva_00, post:75, topic:37352"]
Can both of you post your VESC setting please? I’ll want to compare with mine for range in the future (15/66 - 150mm pneumatics, 2x 5065 motors)
[/quote]

I'm currently running 60A motor max / 30A battery max (on each Focbox). 15/38t with 107s and 15/66t with 175mm Evolve pneumatics).
```

---
## \#78 Posted by: Meche Posted at: 2018-04-04T18:27:53.851Z Reads: 245

```
Where did you get that direct drive?
```

---
## \#79 Posted by: mikenyc Posted at: 2018-04-04T19:11:05.496Z Reads: 251

```
he makes them
```

---
## \#80 Posted by: Idea Posted at: 2018-04-04T21:01:58.485Z Reads: 255

```
@Guacamoleface
@Meche
Thanks :slight_smile:
This is my project, but it's a non-tested prototype
```

---
## \#81 Posted by: Redfire1 Posted at: 2018-04-14T04:52:48.825Z Reads: 265

```
@egzplicit hi morning I bought this motor in and this vesc but it only come with 5 wires,I see in your pic you did so adopting.what is the colour sequence,is that a 5 wire setup and did you leave the T out.please I need you help.I ordered a jst 6 connector to do the adoption.![image|230x500](upload://eQqJ1ifraMalnH6PbeHneNnQFkG.jpg)![image|230x500](upload://7L3hP7FUgUJjsTsJAxZcM7gKRWi.jpg)![image|375x500](upload://6zHInHfGpAJAB3kFuiMBdzzx81s.jpeg)
```

---
## \#82 Posted by: egzplicit Posted at: 2018-04-16T08:56:14.686Z Reads: 257

```
The sequence doesn't matter as long as the GND and positive wires are in the right place. Just make sure those two are correct and skip the temperature pin as you said and you should be good. A vesc will detect the hall sensors and figure out the order on it's own, as long as the +/GND are correctly plugged.

Edited: if you wanna follow my exact sequence, have a look at this picture:

http://www.electric-skateboard.builders/uploads/db1493/original/3X/a/8/a8b516a5b51f99aa90688a996670c02889d26b35.jpeg
```

---
## \#83 Posted by: Redfire1 Posted at: 2018-04-16T09:33:50.921Z Reads: 255

```
Thanks,is it the same on vesc
```

---
## \#84 Posted by: Redfire1 Posted at: 2018-04-16T09:41:16.201Z Reads: 262

```
This is my vesc ![image|679x500](upload://xNEWmDFUhUPqgQ8BG5Tptwt9UgN.jpeg)
```

---
## \#85 Posted by: egzplicit Posted at: 2018-04-16T09:49:11.869Z Reads: 257

```
Usually it's the one next to the +5v. Your vesc is a maytech so I think it's this:

![pinout|511x500](upload://29enokzf9eaZ4OqjygQdTbbzGxT.png)

(From here: http://www.electric-skateboard.builders/t/maytech-sensor-schematic/22378/4 )

So just skip that one and make sure +/- are in the right place and you should be good.
```

---
## \#86 Posted by: Redfire1 Posted at: 2018-04-16T11:31:36.736Z Reads: 244

```
That’s the wire that came with my vesc can I check it with Volt meter.
```

---
## \#87 Posted by: egzplicit Posted at: 2018-04-16T11:44:20.521Z Reads: 258

```
Based on your image:

Green : 5V
Orange: Temperature
Yellow: H1
White: H2
Red: H3
Black: GND

So ignore the temp one and hook up the rest.

See image below: 

![image|668x500](upload://A2sFmAN3ocXFhdAzFPDOtRgx95b.jpeg)

(From @Jinra build)
```

---
## \#88 Posted by: briman05 Posted at: 2018-04-16T11:45:24.577Z Reads: 242

```
I would take out the temp wire so to make sure there is no issues.
```

---
## \#89 Posted by: Redfire1 Posted at: 2018-04-16T13:04:15.873Z Reads: 238

```
Thank you very much you a star
```

---
## \#90 Posted by: Redfire1 Posted at: 2018-04-16T13:05:57.695Z Reads: 251

```
On the motor red is + and black is - and other others don’t matter
```

---
## \#91 Posted by: egzplicit Posted at: 2018-05-01T13:49:46.388Z Reads: 260

```
A quick update: after seeing some images, I got a new Jet Invasion Series Voyager X deck to try it out. The current Freeride DT 38 is nice but with the micro drop it means I can't have a wide stance, my feet are touching the edge where the micro drop begins and it's slightly annoying. 

The new deck is 39" long, so just 1" more, but it doesn't have the micro drop and the nose at each end is a bit shorter. This means I can sit with my legs further apart. 

Since I like plain black on the underside of the deck, I decided to spray paint it:

Orginal:

![18|226x500](upload://a9Md4nLousJFqvBTYYJtjte3Aet.jpg)

Spray painted:

![paint1|271x500](upload://gi0AZIG6E46WUVZWyVJtvUorjDu.jpg)

![paint3|690x460](upload://gXRQL5CJyiVl3d1di0HM0OPBqwD.jpg)

![paint2|690x460](upload://sRDHSUF2R9mutoxkxlDpV4Ais66.jpg)


Bit busy this week but next one I'll move all the stuff on the new deck to give it a go.
```

---
## \#92 Posted by: egzplicit Posted at: 2018-05-08T08:29:36.865Z Reads: 247

```
New deck, same everything else. From a 6 mile test, the deck has slightly wider wheelbase helping with stability at high speeds (24mph and above) while allowing trucks to be a bit more loose for better carving. The raised edges are great, you feel planted on the deck. Slightly less flex, on rough roads with 107s you can tell the difference but it’s not much, maybe 5-8% more vibrations.

Went with a dual tone grip tape, vicious and some other smoother one, no red accents this time:

![image|689x460](upload://hWOknypqx7hXHXj09z9LSovIZU.jpeg)

![image|689x460](upload://aySkcLxfCB5koCbX2HDmlIq332p.jpeg)

![image|690x460](upload://9VHEQ7pJjLaQOSwCXbx4tP5GDzG.jpeg)

![image|690x460](upload://i9rqJPpyJFy8tW0pPqPrUYkrn01.jpeg)

![image|690x460](upload://4lKklqxpIyFNMmT3OAi5AlQN9qi.jpeg)

![image|690x460](upload://kcMtwG3te56B1QwuJZhzx7hJNxc.jpeg)
```

---
## \#93 Posted by: dg798 Posted at: 2018-05-08T17:07:02.055Z Reads: 221

```
Very nice and sleek and clean build @egzplicit
```

---
## \#94 Posted by: egzplicit Posted at: 2018-05-10T17:08:13.390Z Reads: 233

```
Testing AT wheels. The belts are making a whining noise, they are perfectly aligned so not sure what I can do to get rid of it. I assume the extra contact patch the belt is making with the big 66t pulleys is causing this.. on 38t/107s it’s dead silent but on 7” at with 66t the noise is way more pronounced. I kind of got used to having a perfectly silent board so if you guys have any suggestions to reduce the mechanical noise I’m all ears! 

![image|666x500](upload://q8pjmoFeeNmQ7RbbhK3eyEOl6Qg.jpeg)
```

---
## \#95 Posted by: mmaner Posted at: 2018-05-10T17:12:18.035Z Reads: 223

```
Make sure your belt tension isnt too high.  Yuu want to be able to push the belt down at least 1/4 inch without too much pressure.
```

---
## \#96 Posted by: egzplicit Posted at: 2018-05-10T17:27:42.611Z Reads: 227

```
Tried playing with the tension but didn’t make much difference. They are as tight as you say; tried loosen setup but didn’t notice less noise. I also don’t want them too loose to avoid belt skipping. It might be just a pulley + belt combination thing, it’s not horribly loud but compete to the almost dead silent 107s setup, it’s way more noisy. At least people hear me coming now :smile:
```

---
## \#97 Posted by: mmaner Posted at: 2018-05-10T17:36:18.683Z Reads: 220

```
post a video, let's figure out if its normal or not.
```

---
## \#98 Posted by: egzplicit Posted at: 2018-05-10T18:17:20.586Z Reads: 228

```
107s: https://youtu.be/BhWgtjIJLUY
ATs: https://youtu.be/xF-UpgHZ3ks

On video the 107 config sounds more pronounced than in real life however I think you can hear a difference. Again, maybe it’s just me used to the silence of the 107s...
```

---
## \#99 Posted by: mmaner Posted at: 2018-05-10T18:23:01.023Z Reads: 231

```
OK, so 1st thing...you ride goofy, stop that it's just unamerican :slight_smile:

Joke BTW.

I can hear the difference, but its absolutely normal.  I think what your hearing is a combination of motor noise and road noise from the numies that your not used to.  Try riding some new/smooth asphalt and you will see what I mean.
```

---
## \#100 Posted by: Redfire1 Posted at: 2018-06-15T16:54:34.067Z Reads: 207

```
Thank you very much
```

---
## \#101 Posted by: rusins Posted at: 2018-07-01T10:51:13.686Z Reads: 207

```
Really sick board! Am building my own now, with a lot of the same parts as you, and was wondering where you bought that cool griptape with the red triangles at both ends?
```

---
## \#102 Posted by: egzplicit Posted at: 2018-07-01T11:55:18.834Z Reads: 201

```
Thanks! I made my own, got a black and a red griptape then glued two plastic rulers at an angle and cut the grip tapes accordingly.
```

---
## \#103 Posted by: rusins Posted at: 2018-07-01T11:57:21.360Z Reads: 199

```
Wow! Really interesting! The result looks really good, so I might try that as well, but with a different design of course :smiley: Thanks!
```

---
## \#104 Posted by: Tomer Posted at: 2018-07-01T12:54:05.088Z Reads: 194

```
I really like the grip tapes!

Could you please share where did you get each one? I would love to have different toning to my grip tapes as well.
```

---
## \#105 Posted by: egzplicit Posted at: 2018-07-01T13:06:56.760Z Reads: 202

```
For the red one I got them from here:

https://www.ebay.co.uk/itm/Skateboard-Griptape-Every-Colour-9-x-33-Universal-Fit/332182362382?var=541215901916&hash=item4d579c990e:m:mer48b2Fvnlg_IURcsw0rtQ

It's 33" long but you only need a few inches for the front and tail. Then some normal grip tape in between. The new deck with black and gray grip tape uses some standard Jessup Griptape for the grey one and Vicious Griptape for black one.
```

---
## \#106 Posted by: Tomer Posted at: 2018-07-01T13:11:05.290Z Reads: 203

```
Thanks, although I meant to the Black and "Gray" color.

https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/1/e/1e7e060233b92f2576b167b10bd37df31214e41a_1_690x460.jpeg

Do you have any links for each one?
```

---
## \#107 Posted by: egzplicit Posted at: 2018-07-01T14:29:05.541Z Reads: 194

```
https://www.sickboards.nl/en/griptape/9861-jessup-griptape-10-per-10cm.html
https://www.sickboards.nl/en/griptape/919-vicious-griptape-per-10-cm.html

Vicious one seems to be out of stock.
```

---
## \#108 Posted by: 9imeisne Posted at: 2018-07-26T20:37:08.851Z Reads: 170

```
Hey! I am the seller of the boosted XR battery on ebay, wanted to find you on here and give us another way to communicate other than ebay. Do you follow the boosted board reddit too?
```

---
## \#109 Posted by: Slipstriker98 Posted at: 2018-07-26T20:48:37.119Z Reads: 166

```
I do not follow the Reddit
```

---
## \#110 Posted by: 9imeisne Posted at: 2018-07-26T21:03:49.970Z Reads: 167

```
Ah ok. I sent you a message on RC groups too! I am on vacation and wanted to accept your offer, but saw that there is an expiration on the offer.
```

---
## \#111 Posted by: Sinned800 Posted at: 2018-08-03T07:45:42.864Z Reads: 154

```
@egzplicit I thank you really much for your thread. 

YOUR BOARD IS A BLAST !

I thought along time to build a similar board and you gave me so many impressions and hints thats amazing. What goes around my head now are your actual costs. i love to build my own "evolve GTX" like yours with AT tires and stuff but i come to quite high costs around 1400€ . and a new gtx would be around 1800€ bucks here in germany. so yeah i know its always a discussion with pro and cons so. 

i would like to know was worth the money ? and on the bottom line what did you pay.:moneybag:
```

---
## \#112 Posted by: egzplicit Posted at: 2018-08-03T07:55:10.085Z Reads: 153

```
Happy that the thread helped.

It’s difficult to get an exact price for this build because I changed the deck once, then the motors and mounts (both changes well worth it).

Even if it would be the same as a new GTX, I would do it over again any time of the week. You can’t compare the specs, a diy with dual 6355s is much much more powerful, acceleration is crazy fast (I have mine tuned down a bit and it’s still way faster than an Evolve). The battery has almost no sag (until you reach the last 4-5 miles), the range is a true 27-30 miles depending on riding style and you know the battery won’t degrade as fast as theirs. 

I’ve put about 450miles on it without a single fault. It sounds and goes like it did at the beginning. It’s also much more silent than an Evolve, you can’t hear it until it reaches 15-18mph (both a good and bad thing, people won’t get out of your way if they can hear you coming).

Even if it goes wrong, building one means you know how they work and you can fix it in a day, no need to wait for servicing or shipping it to s repair service.

It’s really up to you but seeing all the issues around their boards, their weak batteries that never achieve their claimed range (just see how many packs are being replaced daily with 3rd party ones), remote and disconnects issues... I’m glad I never went the Evolve route. I started with a boosted v2 that I loved but this is just in a different league. The one thing Evolve did right is their double kingpin trucks, if you like carving a lot and never go in a straight line, these are for you.
```

---
## \#113 Posted by: Sinned800 Posted at: 2018-08-03T08:01:42.726Z Reads: 138

```
Thanks for your quick reply. ! i go for it then :sweat_smile: 

Did you have any trouble bypassing your bms ?
I would go for an Lipo Pack because i want to make a swappable battery but i as well want a bypassed bms just for charging.
```

---
## \#114 Posted by: egzplicit Posted at: 2018-08-03T08:19:56.090Z Reads: 142

```
No issues at all, just make sure you configure your cutoff start and end voltage correctly based on your battery pack and it’s all good.
```

---
## \#115 Posted by: DAddYE Posted at: 2018-08-03T08:53:42.819Z Reads: 146

```
How is the hill climbing with those motors? I was going to get the TB 6355, but I’d like something with less kv and more lightweight
```

---
## \#116 Posted by: Sinned800 Posted at: 2018-08-03T20:32:23.475Z Reads: 148

```
Hi @egzplicit one question again :slight_smile: which unikmount are you using ? They got two in the shop: could you link yours ? (I only ride the at set-up).
```

---
## \#117 Posted by: egzplicit Posted at: 2018-08-04T08:41:57.816Z Reads: 157

```
@DAddYE Do you mean TB 6355? When I switched from racerstars 5065 to maytech 6355s, the power went up a lot. The 6355s are much more beefy and have way more torque for the same amps compared to the racerstars. They are also not a lot bigger in weight/size and more efficient (my Wh/mile dropped and I get even better range).

@Sinned800 I’m still on the v1 version, this one:   https://www.unikboards.com/en/boutique/motor-mount-for-evolve/ . The v2 is basically a bit longer and has more room for adjusting the position of the motor and tension on the belts. The v1 is more restricted in motor adjustments and with a sealed maytech motor you might need to shave off the lip of the mount. I would recommend going for the improved v2 design from here: https://www.unikboards.com/en/boutique/core-serie-support-moteur-pour-truck-evolve-supercarve-street-et-at/ . The v2 works with all motor types without any modifications.
```

---
## \#118 Posted by: Redfire1 Posted at: 2018-09-24T07:24:40.304Z Reads: 146

```
Hi everyone @jerry9800 @Jebe @korryh @Quezacotl @BoostedBuilder @topcloud @rich @Eboosted @johnny_261  as some of you know my skateboard catches fire over the weekend while charging it and almost burn my house to the ground with the kids in it,but from my previous fire fighting training I put out the fire before the fire brigade get here just with a few burns to the fingers burnt clothes and shoe and smoke poison,we are ok.All most everything on my board is damage 2x Lipo ,2x Vesc,anti spark switch wheels,BMS.must of you guys I bought stuff from and give me advice to make my board,I know everyone know someone who knows someone,I don’t want to give up just yet I spend loads of money time and loads more in making this board and don’t want to give up just yet,so I am asking for help from my Eskateboard family,anyone you could donate anything so I can have a second chance of rebuilding it.I am so happy to be alive with my wife and 3 kids and my dog.I have learn my lesson not to leave anything charging without watching it.anything will be appreciated.may someone have some old parts they don’t need that work.
Recaldo Miller 
Oberlinstr 2 
33330 Gütersloh 
Germany NRW ![image|374x500](upload://uxGhpK2V16NcyXp3wMofkXlrDUt.jpeg) ![image|374x500](upload://dYEDZEtyXHHhiE6nsiHxExxUv7z.jpeg) ![image|374x500](upload://f8xOJMLXnORTfzYsJY91frwgrVI.jpeg) ![image|374x500](upload://cdF5GYkRQbw2xqOAQeLhlURuuRM.jpeg) ![image|375x500](upload://vfn1SIj7keGrToVm7PQMSPBHUEY.jpeg) ![image|375x500](upload://qmdWKH1kQ8AjeXK8rhe855CROM2.jpeg) ![image|375x500](upload://2gI56QrFNSkEYrjLpxOy6K6VMz5.jpeg) ![image|374x500](upload://gWYiVwtMhT0dQZ2jCTfRriMLU6K.jpeg) ![image|375x500](upload://6eZCC8CtFmZpDbFp4QHvNsT4dnP.jpeg) ![image|374x500](upload://sZAQaQYhg4mtUZCH8VFiX0N9o60.jpeg) ![image|374x500](upload://uVniGpazOg0Ioq4mBzZWz53KuV3.jpeg) ![image|374x500](upload://noG16KC1IrNWTFxg3wuNRE5j3K3.jpeg)
```

---
## \#119 Posted by: Redfire1 Posted at: 2018-09-24T07:26:33.072Z Reads: 140

```
Hi everyone  @Idea @DeathCookies @marcmt88 @b264 @egzplicit @JohnnyMeduse @chaka @Hummie @Quiles @Esk8board4life as some of you know my skateboard catches fire over the weekend while charging it and almost burn my house to the ground with the kids in it,but from my previous fire fighting training I put out the fire before the fire brigade get here just with a few burns to the fingers burnt clothes and shoe and smoke poison,we are ok.All most everything on my board is damage 2x Lipo ,2x Vesc,anti spark switch wheels,BMS.must of you guys I bought stuff from and give me advice to make my board,I know everyone know someone who knows someone,I don’t want to give up just yet I spend loads of money time and loads more in making this board and don’t want to give up just yet,so I am asking for help from my Eskateboard family,anyone you could donate anything so I can have a second chance of rebuilding it.I am so happy to be alive with my wife and 3 kids and my dog.I have learn my lesson not to leave anything charging without watching it.anything will be appreciated.may someone have some old parts they don’t need that work.
Recaldo Miller 
Oberlinstr 2 
33330 Gütersloh 
Germany NRW ![image|374x500](upload://uxGhpK2V16NcyXp3wMofkXlrDUt.jpeg) ![image|374x500](upload://dYEDZEtyXHHhiE6nsiHxExxUv7z.jpeg) ![image|374x500](upload://f8xOJMLXnORTfzYsJY91frwgrVI.jpeg) ![image|374x500](upload://cdF5GYkRQbw2xqOAQeLhlURuuRM.jpeg) ![image|375x500](upload://vfn1SIj7keGrToVm7PQMSPBHUEY.jpeg) ![image|375x500](upload://qmdWKH1kQ8AjeXK8rhe855CROM2.jpeg) ![image|375x500](upload://2gI56QrFNSkEYrjLpxOy6K6VMz5.jpeg) ![image|374x500](upload://gWYiVwtMhT0dQZ2jCTfRriMLU6K.jpeg) ![image|375x500](upload://6eZCC8CtFmZpDbFp4QHvNsT4dnP.jpeg) ![image|374x500](upload://sZAQaQYhg4mtUZCH8VFiX0N9o60.jpeg) ![image|374x500](upload://uVniGpazOg0Ioq4mBzZWz53KuV3.jpeg) ![image|374x500](upload://noG16KC1IrNWTFxg3wuNRE5j3K3.jpeg)
```

---
## \#120 Posted by: Redfire1 Posted at: 2018-09-24T07:27:26.786Z Reads: 140

```
Hi everyone @Mikenopolis @moon @briman05 @Jinra as some of you know my skateboard catches fire over the weekend while charging it and almost burn my house to the ground with the kids in it,but from my previous fire fighting training I put out the fire before the fire brigade get here just with a few burns to the fingers burnt clothes and shoe and smoke poison,we are ok.All most everything on my board is damage 2x Lipo ,2x Vesc,anti spark switch wheels,BMS.must of you guys I bought stuff from and give me advice to make my board,I know everyone know someone who knows someone,I don’t want to give up just yet I spend loads of money time and loads more in making this board and don’t want to give up just yet,so I am asking for help from my Eskateboard family,anyone you could donate anything so I can have a second chance of rebuilding it.I am so happy to be alive with my wife and 3 kids and my dog.I have learn my lesson not to leave anything charging without watching it.anything will be appreciated.may someone have some old parts they don’t need that work.
Recaldo Miller 
Oberlinstr 2 
33330 Gütersloh 
Germany NRW ![image|374x500](upload://uxGhpK2V16NcyXp3wMofkXlrDUt.jpeg) ![image|374x500](upload://dYEDZEtyXHHhiE6nsiHxExxUv7z.jpeg) ![image|374x500](upload://f8xOJMLXnORTfzYsJY91frwgrVI.jpeg) ![image|374x500](upload://cdF5GYkRQbw2xqOAQeLhlURuuRM.jpeg) ![image|375x500](upload://vfn1SIj7keGrToVm7PQMSPBHUEY.jpeg) ![image|375x500](upload://qmdWKH1kQ8AjeXK8rhe855CROM2.jpeg) ![image|375x500](upload://2gI56QrFNSkEYrjLpxOy6K6VMz5.jpeg) ![image|374x500](upload://gWYiVwtMhT0dQZ2jCTfRriMLU6K.jpeg) ![image|375x500](upload://6eZCC8CtFmZpDbFp4QHvNsT4dnP.jpeg) ![image|374x500](upload://sZAQaQYhg4mtUZCH8VFiX0N9o60.jpeg) ![image|374x500](upload://uVniGpazOg0Ioq4mBzZWz53KuV3.jpeg) ![image|374x500](upload://noG16KC1IrNWTFxg3wuNRE5j3K3.jpeg)
```

---
## \#121 Posted by: legend27 Posted at: 2018-09-24T14:07:53.040Z Reads: 121

```
What charger did you use?
The lipos might have been overcharged?

Im sorry to hear what happend. It could have been a lot worse. Wish you the best!
```

---
## \#122 Posted by: Redfire1 Posted at: 2018-09-24T15:27:57.211Z Reads: 123

```
I think it’s over charge I am sad it burn up but happy it did when it did because if it was late at night it could be worst,I used this charger in pic ![image|230x500](upload://e2zBclSn5yI5FvLYDi1hSq32fKn.jpeg)
```

---
## \#123 Posted by: Hummie Posted at: 2018-09-24T15:36:11.349Z Reads: 117

```
What bms were u using if u were using one?
```

---
## \#124 Posted by: Quiles Posted at: 2018-09-24T19:04:01.449Z Reads: 112

```
wow...can't believe...so sorry man. Pls send more info....before building another one, it's important to figure it out why.
```

---
## \#125 Posted by: Redfire1 Posted at: 2018-09-29T16:03:52.343Z Reads: 99

```
This one ![image|230x500](upload://nNFqdePa5ueH9QVRCvC1mWZ87wI.jpeg)
```

---
## \#126 Posted by: Redfire1 Posted at: 2018-09-29T16:04:14.584Z Reads: 98

```
I think the Lipo over charge
```

---
