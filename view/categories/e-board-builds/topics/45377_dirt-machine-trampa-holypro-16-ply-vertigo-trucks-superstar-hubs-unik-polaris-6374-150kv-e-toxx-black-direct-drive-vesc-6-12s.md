# DIRT MACHINE &#124; Trampa Holypro 16 ply &#124; Vertigo trucks &#124; Superstar hubs &#124; Unik Polaris 6374 150kv &#124; E-toxx black direct drive &#124; Vesc 6 &#124; 12s

### Replies: 839 Views: 26549

## \#1 Posted by: rich Posted at: 2018-02-02T19:29:00.240Z Reads: 1273

```
First of all I want to thank all forum members for the big inspiration and great support, I love this place! 

This is my third build and I’m an esk8 addict. 2 years ago I started with the intention to build a cheap longboard but ended up with 3 builds so far.. 

**The evolution of the MountainFOCer** (now called dirt machine)

I built version 1 of the MountainFOCer last summer and actually are working on V2.  I describe here what I’ve done so far plus what I’ve changed and why. Also about real life experiences with the setups and more. For V2 there will be updates from time to time, so stay tuned.

V1 setup:
trampa holypro deck 16ply | vertigo trucks
136kv 6364 sensored trampa motors
trampa urban mounts
dual esk8 4.12 controller
DIY enclosure
10s 10Ah Turnigy Graphene Lipo
bypassed 10s BMS for charging
8” trampa treads (hard compound) on superstar hubs
14T / 66T pulleys
anti-spark switch with fuse

Range: max. 23 km / 14 miles
Length of cables from battery to capacitors: 28 cm / 11 inch
Length of phase and sensor wires: about 85 cm / 33.5 inch


![20170816_162010|690x388](upload://qo1us49mZsozNmWYylGaYwWB7tX.jpg)

![20170731_155853|690x388](upload://gxnZPriYYe9vrCF5Bpf5zSajvTb.jpg)

![20170713_202428|690x388](upload://dRupvtoqCtnClj4iF00Vaj68crg.jpg)

![20170715_195936|690x388](upload://7LSYloqvL3xaEF0ynRBdy1wDUSn.jpg)

![20170713_194347|690x388](upload://1jlAYrp1zosslPYhsmdFLRWE9Wi.jpg)


**But now some general details about this build and V1:**

First thing I did is to get rid of all bling bling parts because I don’t like it shiny, it must be black. I went to a local shop for black anodizing and love the result. 

![20170327_034216|690x388](upload://bQkFotUFY6nC2ZZU88hGN24y4yS.jpg)

![20170330_151806|690x388](upload://lv8jbdAwXCCd48uhulGRvBgMJUO.jpg)

The Trampa motors also got a special treatment with carbon foil, black bolts and black metal mesh against debris.

![20170708_021533|690x388](upload://2U55KrPtWwRcCcF4xBe4I6L65he.jpg)

The urban mounts are sturdy and the grub screws keep tight. I like the look more than the pro mount but the disadvantage of an open belt system is that all that debris enters the drive system. I damaged some belts so far due to stones between belt and pulleys or by hitting the ground with belt/wheel pulley. 

I tried idler pulleys on the slack line and it worked well but the tiny M4 bolts get loose and bend quickly, changed to M5 bolts but am not happy with the durability so I dismounted it. The motor mount is long enough (axle to axle distance) for most cases, but on hard braking the belt can skip, I like to have the belts quite loose. 

![20170711_011538|690x388](upload://zl4XASh018T6l8cb8bhImMjPY2d.jpg)

The enclosure was bent from an 0.5mm steel sheet and was a lot of work but it did the job. Bottom and top are 4mm plywood. I would use 0.8mm -1.2mm aluminium sheet  if I would do it again. The goal was to have battery and Vescs in one box in the middle of the deck which I like more than the look of 2 boxes. In the end I changed my mind because it was impossible to swap or change batteries with this setup.

Outside I put carbon foil and inside some pieces of foil I had to insulate the metal.

![20170709_011326|690x388](upload://vnnKZJGCK5fgo006jtzhGndODb8.jpg)

![20170709_011344|690x388](upload://71ypnFoAbxRnoyAse02ftM4sg4Y.jpg)

![20170712_221112|690x388](upload://ny1zch0MvxswsrEQP9wJlOyWrdg.jpg)

![20170713_190249|690x388](upload://cF0U5zIsA2cYw3ZjNFLuBPVihho.jpg)

A short story about my vesc disaster. I started with 2x flier V4.12 but the hall sensor ports were not working so I switched to 2x Maytech V4.12. I realized that BLDC hybrid mode didn’t help with cogging at all, just a better control at low speed, that’s it, but feels like unsensored. After many different trials I knew FOC would be the only solution in my case. Bad that Maytech don’t run in FOC that’s why I ordered 2x esk8 4.12 controllerand finally it performed as I wanted, smooth startup without any cogging! Well, because I work on 2 builds (the Urban FOCer is not finished yet), I needed another 2 vescs for use in FOC, so I ordered 2x esk8 controller 1.1. 

That should be enough vescs for a long time and I was totally broke. 2 weeks later my MTB didn’t run anymore and I was sure that I fried the vescs.  That’s why I begged Frank to sell me 2x VESC 6 for a discounted price, what he fortunately did. 2 days later I realized that a solder joint of a phase wire was disconnected (couldn’t see it through the wire mesh) so all good, after resoldering everything was working again. Because of VESC 6 I sold all V4.12’s I had, only kept the esk8 1.1 controller for the Urban FOCer.

![20171016_213643|690x388](upload://g1TTf0w00x68OQcheHZC2tXk4ov.jpg)

I started with 10s 10Ah Turnigy Graphenes (6s+4s in series) with bypassed BMS for charging only in combination with a 42V Li-ion 3A charger. Placed in a Lipo safe bag with some foam and wrapped in fabric tape.

Everything was working well until the day I forgot to switch off the board after a full discharge, 28 hours later the cell voltage was 0.887V. One more reason for V2 and upgrade to 12s..

![20170709_011134|690x388](upload://4c8a0OXmwER1pnfMtzZ4gypz21z.jpg)

As remote I have the steez but had some problems with scary dropouts in the beginning. The receiver was too close to the metal and after reposition the issue was gone.

![20180202_201023|690x388](upload://xVK33iBBNUhqgDUXaFekHZ4vQX7.jpg)

I use motorcycle 5g adhesive lead weights against valve/wheel wobble and it works really nice , big up @whitepony AFAIK the first who tried this technique on MTB hubs. It is a big difference. After 600km some weights are missing, in the future I’ll take pictures of all wheels so I know where to add missing weights without balancing again.

![20180202_200901|690x388](upload://nXFf6wBUjtyiHm99i36Yf7r4xm8.jpg)

First I used the 15T pulleys but after a couple times of reassembling the grub screws were stripped and got stuck. Thread locker on the grub screws was not enough, it came loose very often because of the play of key and keyway. I ended up with using a special non-permanent thread locker for shafts for the new 14T pulleys. I put plenty of it on the motor shaft and key and since a few hundred kilometers it holds up very well. It’s ridiculously cheap, both thread lockers are from hobbyking. 

EDIT: This HK thread lockers are too strong, it needed heat to remove the pulleys, I switched to the genuine Loctite.

![20170826_135405|690x388](upload://iEhDMujO8mDk0K7mT2Oed0rSmH6.jpg)

I use the 8” trampa treads in hard compound. Because of more tear on the rear tires I swapped the rear and front tires after 300km (186 miles) and had another 300km. In future I’ll wait until the rear tires are worn out, then replace the 2 and the next time all 4 and so on, less work.

What really sucks is a puncture, I had 5 within 600 km (373 miles). The tires had no visible damage and there were no stones inside the tire, no idea why this happened. I fixed the tubes with bicycle repair kit and they last so far.

![20171106_153743|690x388](upload://zW5IXgXcysoIqTuzxypC9S5kvSJ.jpg)

I love the fact that I can ride without taking care of the battery and electronics, for MTB top mounting is a must IMO, it's ugly but rocks! Here you see what happened to my nice Trampa sticker and why I enjoy top mounting

![20171024_180037|690x388](upload://hHXKuYvP35MJyubG60rXCFaMDDG.jpg)

One Video tells more than 1000 words and pictures, so I uploaded this video for comparison of bldc and FOC mode. In the beginning you can see the annoying performance at startup with hybrid BLDC. Sorry for the length of this video, better skip sometimes :wink:

https://www.youtube.com/watch?v=ptlHqK7kqCA


Meanwhile I’m working on the second (and hopefully last) version of the MountainFOCer and will post some more details soon.

Changes in V2:
dual VESC 6
E-Toxx direct drive
separate DIY  box for electronics at the tail of the deck
12s bestech BMS for discharge/charge
12s 8Ah Lipo (+ 12s5p 15,6Ah Li-ion)
Peli case for swappable Batteries
direct fet anti-spark switch
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2018-02-02T19:42:34.852Z Reads: 877

```
Yeah it's time to get serious! 
I like you enclosures and the Motors :sunglasses:
And you should really think about opening a museum for all the VESCs :smile: 
Curious to see which color you choose for the direct drive :D
```

---
## \#3 Posted by: rich Posted at: 2018-02-02T19:54:01.062Z Reads: 892

```
[quote="Der6FingerJo, post:2, topic:45377"]
And you should really think about opening a museum for all the VESCs :smile:
[/quote]


Hehe. I sold most of them but I have this picture for the museum (but one was sold already when I took this pic)

[quote="Der6FingerJo, post:2, topic:45377"]
Curious to see which color you choose for the direct drive :smiley:
[/quote]

Guess which?

https://www.e-toxx-shop.com/trampa/direct-drive/black-direct-drive/#cc-m-product-9936130870

Shipped one vertigo hanger to @nowind for machining. Can't wait to receive these beauties :heart_eyes:
```

---
## \#4 Posted by: rich Posted at: 2018-02-13T20:31:49.262Z Reads: 801

```
Received the direct drive today and am happy, it’s f****** sexy! 
@Nowind = Nodirt = Noproblem 

![20180213_185433|690x388](upload://oA0hENQkqyFhWfdzBlVlPN22Se8.jpg)

Also there is some progress on v2 of the MountainFOCer
Hexagon news, no comment……..

![20180210_005739|690x388](upload://fiaZAR0mKoAazKIkJA0EVLROnSa.jpg)

some hours later... 

![20180210_211226|690x388](upload://6FuTVQ5GpE5OO0hnrsN9YnF4qig.jpg)

FInished my first 12s battery “brick” with bestech BMS for discharge/charge with 2x 6s 8Ah 15C Turnigy Graphenes. Furthermore I want to build a 12s5p Li-ion 15,6Ah with VTC6 cells within the next weeks/months for more range and easy swapping.

![20180123_213409|690x388](upload://CqE6DI2IKtgOgzXUrvg22siKSi.jpg)

![20180123_224245|690x388](upload://dMK3wbv3C3er5jGnWKBS7j2c42r.jpg)

Some ABS for protection

![20180213_202450|690x388](upload://107GShyKrZGHDZdkB2kmR5kGvss.jpg)

For now I’m going with a PeliCase 1150 bolted to the deck with some rubber washers for both batteries but I don’t like the bulky look at all. I think I need to change that but that’s not first priority now, I need to ride first

![20180203_170124|690x388](upload://pGMDBcsFEjaB5zpuBbxfU8YATzY.jpg)
![20171204_144005|690x388](upload://oT54yng26SzfqBTz7fxTk13mjxL.jpg)

I’m a bit jealous when I see all you guys with 3D printers.
I have to do it old school style and bent an aluminium sheet for the enclosure. The Vescs are bolted directly to the aluminium enclosure so it should help with heat dissipation. I tried it with a cardboard model first.

![20171121_140552|690x388](upload://wI6QpYVDmA9zll6zBTaD6HpVkmQ.jpg)

![20171121_141135|690x388](upload://p5qOu93sUxWKesud3sQnZbspcWO.jpg)

![20171121_154640|690x388](upload://4bS0YbTzvl6FjUSJjou5o56wTcZ.jpg)

![20171121_232301|690x388](upload://fVMtk2Q4wP1C63skNBgQLJJCrZj.jpg)


Added 3x M4 threaded inserts for the enclosure.

![20180108_191533|690x388](upload://1WRZakjwto7WqJgqeB5jPWOa0SA.jpg)

![20171230_223326|690x388](upload://1iGyHVtm4FvfSNAQvw6U9E487M3.jpg)

Glued all open edges, added  some insulation and carbon foil.

![20180109_005356|690x388](upload://xRf8CGoS7Hr4qRkwDotqHm2g4Ai.jpg)


It is really tight inside with 2x VESC6, 1x @goldenHusky Direct FET Antispark with LED switch, 1x HM-10 bluetooth module, the huuuuge steez receiver (I had to remove one port on PCB) and all the cables. No more space left, hope the receiver works properly at that given position.

![20180211_215101|690x388](upload://4ukDqtQxZODI1gLuAIdqEPu0k67.jpg)

![20180212_105306|690x388](upload://wQHcUnpXlJwHDjeVkqJzPcNDesE.jpg)

I'll add a silicone gasket between the aluminium and the ABS cover for splash proofing. When I finally know the length and arrangement of the phase- and sensorwires I want to seal the cable feedthrough with silicone, too.

![20180213_194453|690x388](upload://gl7JuHBmuwTUAHNYUq6YcoixTFv.jpg)

![20180213_194540|690x388](upload://A2UMhgUzYIcG9PcoGYM5p2gxTje.jpg)

That's it for now, hope to ride again soon, it is 4 months ago...
```

---
## \#5 Posted by: rich Posted at: 2018-02-15T17:49:32.820Z Reads: 692

```
Today was my first test run with 12s and VESC6 :metal:
I kept the belt drive because I wanted to feel the difference compared to 10s and V4.12 with the same drivetrain first before I mount the Direct Drive.

![20180215_165645|690x388](upload://1TPVWBVobjwPYcdiw6stN1iqaBV.jpg)

I use the @Ackmaniac App “VESC Monitor” which worked flawlessly. Last summer it didn’t with new FW but now it’s perfect (well, I would prefer a dark theme). 

![Screenshot_20180215-171540|281x500](upload://b60K7dkHMtfM7oIiIQDqB5JV8CV.jpg)

To be honest, I thought there is more difference in power delivery when using VESC6 but there is still a difference. On start up it’s the same but when hitting full throttle later it feels like I get more or faster power. Everytime hitting full throttle I had between 70A-98A motor current and max. 59A battery current. I was not nice to my MTB but when I came home the temperature of the Vescs was 17.5 degrees (and 29 max), I like the aluminium housing and also the fact to have reliable 12S FOC.

These are my settings in VESC-Tool for each Vesc (with 2400W 136kv motors)
Motor max: 50A
Motor regen: -25A
Batt max: 50A
Batt regen: -15A


I get a top speed of about 44 km/h with this 14/66T setup, but counted with a wheel diameter of 190mm, none of my tyres are real “200mm”.

I removed the dampas on the front truck and kept the yellow dampas on the rear truck. It’s really nice to ride, feels good.  I’ll see how it’s gonna be in heavy offroad conditions if it’s too loose but carving or u-turns are much easier now.

Next thing is to switch to direct drive. Unfortunately it’s a bit cold outside, can’t wait for spring time!
```

---
## \#6 Posted by: Der6FingerJo Posted at: 2018-02-15T19:16:22.775Z Reads: 635

```
I like what i'm seeing! 
Already suspected that there isn't that much a difference in the feel between 4.12 and 6, but 6 should of course be more reliable in 12 FOC which is also nice when riding. Less worries and all.

Also curious about the tires though i don't have high hopes for them :sweat_smile:

I might try removing the in the front as well, sound promising. I don't like jumping around everytime i want to make a somewhat tight turn.
```

---
## \#7 Posted by: rich Posted at: 2018-02-15T19:31:03.279Z Reads: 634

```
[quote="Der6FingerJo, post:6, topic:45377"]
Also curious about the tires though i don’t have high hopes for them :sweat_smile:
[/quote]

Yeah these cheap ones probably won't last long but I felt not much difference during riding, only the sound. They are thin and very soft compared to the genuine ones.

[quote="Der6FingerJo, post:6, topic:45377"]
i want to make a somewhat tight turn.
[/quote]

The ultimate turn you could get without springs :joy:
```

---
## \#8 Posted by: Der6FingerJo Posted at: 2018-02-15T19:35:45.890Z Reads: 617

```


[quote="rich, post:7, topic:45377"]
i want to make a somewhat tight turn.

The ultimate turn you could get without springs :joy:
[/quote]
Maybe when i'm planning the next roundabout-only tour :laughing:
```

---
## \#9 Posted by: rich Posted at: 2018-02-27T14:13:58.312Z Reads: 632

```
I couldn’t find a replacement shaft for the trampa motors and don’t want to cut the original ones so I decided to get new motors and maybe sell the trampa’s including drivetrain.

Received my (frozen) parcel from Unikboards today, really nice guys and good service Ben and @okp!

![20180227_135148|690x388](upload://xj0BfcNqLyO1LRGTM2YFeawfvWU.jpg)

They fit soooo nice, it’s like one unity  :heart_eyes:.

![20180227_135710|690x388](upload://yw72ITImteJJGduFvtQpI2ZZlo2.jpg)

I have to rename this build because with sealed drivetrain and motors it’s more a dirt machine than a MountainFOCer, also there are not too much mountains in my close area :laughing:. I hope the motors don't get too hot in summer (BTW today it's -11 degrees, can't wait for spring)

The weakest part right now is the vesc enclosure because it’s not waterproof yet, especially the upper shell, I have to change that.
```

---
## \#10 Posted by: rich Posted at: 2018-03-13T19:58:18.829Z Reads: 628

```
It seems like the snow is gone and I want to ride :stuck_out_tongue_winking_eye:
Mounted the direct drive, looks so sick and can’t wait to ride the machine.

![20180309_191130|690x388](upload://wtSDG71u1x9GzrAzc7SmRcZu47L.jpg)

![20180310_122710|690x388](upload://A6NSoYVSvLM6cKDxoC7Y08hXKNG.jpg)

Unfortunately my vesc enclosure is too wide for this drivetrain so right now I’m working on a new one made of 2mm ABS, so much nicer to work with. I’m no boss in thermoforming that’s why I bend it with a heat gun at 250 degrees, easy. The new enclosure will be much better than my old one, also better sealing and stress relief on the wires so they can’t move inside the enclosure


![20180311_040554|690x388](upload://o1txvlkN3EZIImw0LpxSAvt0pmv.jpg)

![20180311_041308|690x388](upload://sZkea3KlhHnpWjhRYHDXscJH0zv.jpg)

![20180312_223204|690x388](upload://6epva5kJ58XIkIuibS5YGc6P6hk.jpg)


Glued the edges and added some plastic angles for reinforcement of the structure and drilled 19 holes which is so easy with ABS, would love to drill more :laughing:, aluminium was a pain.
Now it’s time to bend the upper lid and resolder almost all connections.

![20180313_195108|690x388](upload://qi1C1EwMJJXg1wVw8M04hTQki35.jpg)
```

---
## \#11 Posted by: rich Posted at: 2018-03-19T13:31:20.861Z Reads: 604

```
Finished the enclosure, had to enlarge the inner height from 30 to 35mm to fit all parts, maybe I need to make a new upper lid but fore sure not now :laughing: . Between both shells I use a thick flexible foam sealant, forgot to take pics. The LED switch for the antispark was too big that's why I use a different waterproof switch and an additional red LED as rear light plus this way I can't forget to switch my board off again :wink:

![20180315_015705|690x388](upload://oIbdbuBw6j5AFHOaByLEw7yNc3Z.jpg)

![20180317_173236|690x388](upload://vB4RYU2Dkoscs7pc5wSSy3F8p4p.jpg)

![20180317_233018|690x388](upload://ep11PhQUwzgwVMMdirGBUQBoPqh.jpg)

![20180317_232737|690x388](upload://xhhnKapi4kmp5UowbvMWq2TN6qM.jpg)

I had to remove the wire mesh on the phase wires but am happy with the nice cable grommets, the wires can't move which is perfect and it's almost waterproof.

Unfortunately some snow an frostiness is back but I have the feeling I can't resist to test it anyhow. I'm too excited to feel the new drivetrain and motors :grin:
```

---
## \#12 Posted by: Acido Posted at: 2018-03-19T18:24:04.008Z Reads: 563

```
I like what you did with the box for vescs!
```

---
## \#13 Posted by: rich Posted at: 2018-03-19T20:55:34.241Z Reads: 592

```
Thanks @Acido, it wasn't easy to fit everything inside and the enclosure isn't perfect but hey, it's custom made. I couldn't find a box with nice dimensions, the one from UK is only 8,9cm in width. Mine is inside 12cm x 14,5cm x 3,5cm.

I had my first test ride today but unfortunately only for 2-3km because one spring retainer of the front truck broke, i think it happened because I crashed into a tree but I'm not sure.

![20180319_164404|690x388](upload://ktStxbctplMwdavljmn0aTHgZZC.jpg)

![20180319_214025|690x388](upload://e1ldGvijlOuiyOfL4G8yGAvsUUn.jpg)

But what I can say from this short ride is that I'm quite happy with my new parts. 
@okp these motors are powerful and good looking, I like them. 
@Nowind the direct drive is genius and the free coasting epic in comparison to belt drive. Maybe it's only in my head but It feels like the MTB rolls better with attached drivetrain and motors than without :laughing:. 
The only downside is the noise, my dirt machine sounds like a machine now.
But the advantage of the noise is that 100% of the people turn around even when I'm far away and hear I'm no joker and step to the side. I've never had this experience with belt drive and FOC that's why I thought about using a bicycle bell but that's the past.

![20180319_164741|690x388](upload://4jj7BzoX1cbHENpn2LrXO590atV.jpg)

![20180319_164722|690x388](upload://yKe01pgaegjCq04jY4g2pnBafg1.jpg)


It is so great that I can lean the board against a wall without fixing it :sunglasses:

![20180319_170748|281x500](upload://gyuc031m4w6MQlncEWoAvE1Fh9r.jpg)


Here a short part of my very first test ride with telemetry data. The quality is bad, the goal was to monitor the data. The video starts with a speed wobble at 44km/h (I think I'll use my dampas again on the front truck, too spongy) and ends with a crash. I forgot the first rule: Always check the terrain BEFORE you ride there

https://youtu.be/WIdTK5-xKyg
```

---
## \#14 Posted by: Acido Posted at: 2018-03-19T20:59:44.854Z Reads: 547

```
That should not happen
```

---
## \#15 Posted by: rich Posted at: 2018-03-19T21:22:44.972Z Reads: 565

```
Also that should not happen after 600km :face_with_raised_eyebrow:

![20180310_031233|690x388](upload://m7Es6Agaf8szCIktIFZ5YoJIOhq.jpg)

Í need even more spare parts than this, this are my spare boxes, it's ridicolous

![20180319_220821|690x388](upload://7l6hx512A6rRmMHQXsjG7sXEInZ.jpg)


I have 1mm, 1.5mm and 2.5mm bushings but no 2mm. I had to disassemble my urban carver to get some 2mm bushings, need to order some.

Today was another reason why I have all kind of spare parts. Imagine I have no spring retainer at home, then I would have to wait 1-2 weeks without riding. It happened to me 2 years ago in summer that my remote was broke and I couldn't ride for several days before I found an ugly massive remote on ebay. Then I had to wait for an additional proper remote to arrive. Of course I have a spare remote. The worst case for any esk8-er is a board which is not running.
```

---
## \#16 Posted by: telnoi Posted at: 2018-03-19T21:36:14.963Z Reads: 533

```
What's up with the different sized bushings anyway? Haven't looked deeply into it yet, but it appears there are different sizes for the same trucks depending on tolerances?

Direct drive indeed does sound loud. Don't want to attract any unnecessary attention from hunters/police, as both tend to be assholes in Hessen... The former being awfully afraid of me spooking their game. Sticking with belts, though the maintenance free direct drive does sound like a dream.
```

---
## \#17 Posted by: rich Posted at: 2018-03-19T22:05:32.971Z Reads: 553

```
[quote="telnoi, post:16, topic:45377"]
What’s up with the different sized bushings anyway? Haven’t looked deeply into it yet, but it appears there are different sizes for the same trucks depending on tolerances?
[/quote]

Hangers and baseplates have tolerances that's why there are different bushings, only the thickness of the base differs. For example standard size of bushings seems 2mm. If I would use my spare hanger I would need different bushings, sounds complicated :laughing:, easier to explain with pictures:

First you measure the outside of the hanger without bushings

![20180319_224617|690x388](upload://qi2LsO8Xa66v2gziXVG59CN9QMG.jpg)

Then you measure the inside of the hanger

![20180319_224723|690x388](upload://k4SNnotBsqmSbucRkH9vtR9MqvR.jpg)

As you can see in my case there is 4mm difference so 2x2mm bushings fit perfect.
There are also bushings on the baseplate but the size does'nt matter, usually they are 2.5mm and black. The 2mm bushings are grey.

[quote="telnoi, post:16, topic:45377"]
Direct drive indeed does sound loud. Don’t want to attract any unnecessary attention from hunters/police, as both tend to be assholes in Hessen
[/quote]

Where I ride there is no police, I wouldn't use it in public places and try to avoid streets and pavements. Do you mean hunters because there are animals which sound like a direct drive :rofl: or because they want to catch you? I would say "catch me if you can"
```

---
## \#18 Posted by: telnoi Posted at: 2018-03-20T06:14:09.887Z Reads: 519

```
Thanks for explaining. Time to order some replacement parts. 

Regarding hunters, they would complain about disturbing nature. They themselves drive around in jeeps. At my current skill level, they still keep up with me.
```

---
## \#19 Posted by: Acido Posted at: 2018-03-20T06:25:57.796Z Reads: 517

```
Run them overwhey they get out of the jeeps
Problem solved ;)
```

---
## \#20 Posted by: telnoi Posted at: 2018-03-20T07:37:56.605Z Reads: 541

```
That's a good idea :stuck_out_tongue:
Building a second board for my wife, which should be a bit louder and safe. I think direct drive is the right thing for her. 

It took me some time to get used to the drag and instant slow down of belts when you let go of gas. The sudden jolt would throw her off for sure.

We will both go on a MTB course (for me personally, learning how to brake/slide). Hopefully, I'll feel as Conformable as this guy at some point. Those pussy ass hunters in their jeeps would not be an issue :stuck_out_tongue: 

https://youtu.be/tVf_e6p7Nxg?t=2m10s
```

---
## \#21 Posted by: Der6FingerJo Posted at: 2018-03-20T08:31:42.413Z Reads: 511

```
[quote="telnoi, post:20, topic:45377"]
Those pussy ass hunters in their jeeps would not be an issue :stuck_out_tongue:
[/quote]

Here in Sachsen Anhalt all the Hunters i encountered were friendly and interested, not sure whats wrong in Hessen :smile:

I think a slightly louder drive is better for everyone involved.
```

---
## \#22 Posted by: telnoi Posted at: 2018-03-20T08:33:30.671Z Reads: 493

```
They are overly protective of their hunting grounds around here (must be related to the amount of cash they own... all rich people with stupidly expensive 4x4s)  and even stop mountain bikers and tell them they are not allowed.
```

---
## \#23 Posted by: DanSkates Posted at: 2018-03-20T11:48:41.635Z Reads: 474

```
LOVING watching this build!  Can't wait to see some more vids when the weather warms up for you :sunny::crazy_face:
```

---
## \#24 Posted by: rich Posted at: 2018-03-20T14:04:38.976Z Reads: 521

```
[quote="telnoi, post:20, topic:45377"]
Building a second board for my wife
[/quote]


I like that you share this hobby, that's great  :grin:
I wish I had someone to join my rides

Great video, definitely not my skill level :laughing:

[quote="Der6FingerJo, post:21, topic:45377"]
slightly louder drive
[/quote]

:joy:
I think I have to do a comparison video filmed with the same mobile and settings as I did with belt drive and FOC.

[quote="telnoi, post:22, topic:45377"]
They are overly protective of their hunting grounds around here
[/quote]

I also had an experience with a hunter, i was landkiting and he came to drive me off, took pictures of the licence plate of my car and said he gonna sue me, never happened.

With an E-MTB you are almost hidden but with a kite like 20-30m up in the skye everybody within a radius of some kilometers recognize you. Almost every single time someone came and said it's forbidden here, go away. That's one reason why I decided to switch to an electric mountainboard and this was one of the best decisions in my life :sunglasses:

[quote="DanSkates, post:23, topic:45377"]
LOVING watching this build!  Can’t wait to see some more vids when the weather warms up for you :sunny::crazy_face:
[/quote]

Thank you, really appreciate it!
Would love to go for a ride with you and try your kickers but unfortunately you are almost exactly on the other side of this planet :wink:

I need a action cam but can't afford a gopro, I've heard the apeman a80 is not bad but the battery sucks (like 20 minutes runtime only). Or do you know a good and cheap (I should know this is not possible :rofl:) cam?

Another hint:
I'm now a big fan of O-Rings (or rubber washers) on bolts. I use them on the bolts for the electronics enclosure. The future will tell but on my first ride nothing came loose. 
The last time wihout O-Rings the box was loose after the first ride and i had to use thread locker. It seems like it's working without thread locker when I use these O-Rings, I'll see.

![20180320_135737|690x388](upload://tUbMSpjtK9SIcT4UzYbmNHS6vXJ.jpg)

I love the idea of @trampa using O-Rings between spacer and bearing against rattling but the O-Rings are too small in my opinion. First you need a woman with long nails to slide it on the axle and if you need to take the wheel off (which I did 5 times in the fields when I had a flat) then one bearing, the spacer and the O-Ring flies away, not nice in grass. Now I always carry a small white blanket in my backpack :laughing: for such situations because once I had to search 10-15 min an O-Ring in deep grass. When I had the puncture it was before dusk but after changing the tube it was dark and I realized the O-Ring is missing.

Anyhow, the Trampa O-Ring for 12mm axle has an inside diameter of 10mm that's why you have to stretch it to get it on the axle. Actually I'm using different O-Rings on my MTB which are really easy to slide on the axle. They have an inside diameter of 11.8mm and fit perfectly. They are 2.1mm thick, the original ones are 2mm but I don't recognize any difference.

![o-ring|250x180](upload://jEu8QVpcBFCrSaeYTSzUU8zBHSk.jpg)
```

---
## \#25 Posted by: rich Posted at: 2018-03-20T20:16:23.895Z Reads: 488

```

I had my second ride for about 20km and it's so freaking great, it's time to get dirty. With belt drive I would have a hard time now with cleaning up everything :laughing:

![20180320_172053|690x388](upload://jb8VJztimKSOlJZyWisSXIJfon0.jpg)

![20180320_173238|690x388](upload://ahNQ1OCSz7XJWoexte48J6PjKqK.jpg)


Inspired by Nowind I use my snowboard goggles and like it very much. Also the fact that people can't see where I am watching is genious. Also in case I have to flee from police and they catch me I could say "I didn't see you". I think I'll buy a similar one but for summer. Now I remember all the insects in my eyes last year.

![20180320_172352|375x500](upload://tuv5aJsxCJFsfC0EXnX2gRusktV.jpg)

For the very first time I used a selfie stick to catch some footage and have to say this is scary and dangerous 
No idea how you all manage this. If you missed it in the video, at 01:50 i almost crashed because I checked the angle of the mobile instead of watching the ground. At 08:00 you see how I deal with puddles. Also I have to work on my filming skills

https://youtu.be/-sdVYlZm-1U

On both rides all bolts of one wheel hub adapter which is connected to the wheel spur gear came loose. @Nowind any idea? As you recommend I used very little amount of thread locker on this bolts but strange that only one side gets loose. I have a feeling it is because of hub/spoke/bearing wobble. Amongst my 12 superstar hubs only 1 is true, the other 11 wobble. For the direct drive I use the perfect hub plus the almost perfect one. Maybe I need to remove the O-Rings and mount the wheels more loose with a bit rattling. Or should I use more thread locker?
```

---
## \#26 Posted by: benjammin Posted at: 2018-03-20T22:43:40.414Z Reads: 446

```
Nice save at ~ 2 min in! Looked like you were going down for a second 👍
```

---
## \#27 Posted by: rich Posted at: 2018-03-20T23:55:11.027Z Reads: 445

```
I was really lucky, what you can't see on the video is that there are bushes and small trees on both sides on the narrow path. I have no idea how I managed to make the last curve, the brown thing is a massive bush followed by trees.

I ordered an action cam to shoot some better footage (hopefully not of crashes :laughing:). The new edition of the A80 seems to have better batteries so I give it a try, also I like 120FPS in HD.
```

---
## \#28 Posted by: benjammin Posted at: 2018-03-21T00:09:21.010Z Reads: 421

```
I've had some close calls as well. Seems like hitting the throttle kinda helps pull out of it. Worst fall had was pre-motors, just going downhill. Carving too hard on gravel and iced out. Sucks falling with the bindings!
```

---
## \#29 Posted by: rich Posted at: 2018-03-21T00:21:04.420Z Reads: 434

```
[quote="benjammin, post:28, topic:45377"]
Sucks falling with the bindings!
[/quote]

So true :rofl:
Do you use heelstraps?
I think I'll mount mine again, they could save my feet from braking when falling at higher speed. I used them only once, they felt very well in the bmx track but at slow speed when turning or on a steep hill everytime I lost the balance I tumbled down like a stone forward or backwards and felt like a idiot. But maybe this is the price for more safety, in this case I need ass padding :joy:.
```

---
## \#30 Posted by: benjammin Posted at: 2018-03-21T00:28:07.029Z Reads: 407

```
Yeah, I use straps. Feel less likely to fall with 'em, more likely to hurt myself if I do though :sweat_smile:
```

---
## \#31 Posted by: rich Posted at: 2018-03-21T00:36:50.642Z Reads: 422

```
:joy:
OK, hope it's not too painful because sometimes I have the feeling it is good when I can fall away from the board. Once I had an ice out on loose gravel like you, suddenly I was standing in mud puddles in my socks only, my shoes remained in the bindings :laughing:, that was a weird experience.

BTW I just realized I have another puncture :tired_face:
What is the strongest tube in this world? I'm tired of all the balloons.....
```

---
## \#32 Posted by: benjammin Posted at: 2018-03-21T00:45:32.106Z Reads: 414

```
Lol yeah seen some vids of people avoiding some nasty falls by slipping out of their bindings at last minute.

Sucks about the flat. Are you using trampa tires (alpha lite or whatever)? Kept getting flats with those things. Little goat head thorns and whatnot. Went through some bark and came out with both front tires flat. So far I like the Evolve street tires the best. Dk about their knobbies though.
```

---
## \#33 Posted by: rich Posted at: 2018-03-21T01:01:37.983Z Reads: 423

```
Actually I'm using thin 8" "wheelchair tires",j wanted to test them because they are half of the price but I don't trust them. It's quite hard to spend 70€ for 4 tires every 600km.

I use the CST tubes which trampa sells. This is my 6th flat within 625km. I need to buy more bicycle repair kits or try out the innova tubes.

[quote="benjammin, post:32, topic:45377"]
So far I like the Evolve street tires the best.
[/quote]

I have them, too. Yes they seem very thick and durable but maybe not the best in offroad conditions but definitely would help against flats.

[quote="benjammin, post:32, topic:45377"]
Went through some bark and came out with both front tires flat.
[/quote]
:roll_eyes:
I think I stop complaining and start to carry 2 replacement tubes in my backpack additional to my workshop.
```

---
## \#34 Posted by: benjammin Posted at: 2018-03-21T01:25:03.982Z Reads: 390

```
Green slime stuff seems to help. Saw a thread recently where someone mentioned using an alternative that worked better. Can't remember what it was called though. Have to dig around.

Had a blowout recently from riding on bald tires. Fkn covered in green slime. Had it all the way up my back :rofl:
```

---
## \#35 Posted by: DanSkates Posted at: 2018-03-21T04:26:07.462Z Reads: 420

```
Hey top tip with the o-rings!  I used those rubber gromet things on my ultrabox when I was using it before - got a nice new dual CNC case for my FOCBOXs now and have just glued some thick rubber to the underside and velcro'd it to my board!!!  So far so good and I've landed pretty hard off the kickers and it hasn't moved.  Funny thing actually waytching some of my landings off the bigger kicker in slow-mo the board nearly always bottoms out and the way it all contorts is terrifying - I can't believe I haven't smashed or cracked any of my parts yet either!  I tell you what the the bottom of my board has some serious battle scars from dirt tracks though.

Did you buy the action cam already?  For what it's worth I'm using the Thieye t5e which you can grab here: https://www.gearbest.com/action-cameras/pp_575345.html

It's performed pretty well so far and for the money you can't complain!

Dude, back to kickers - I'd bloody love to ride with you too.  Or anyone for that matter!!!  It's bloody lonely carrying that bloody thing around and riding around like a loner.  Hard to push yourself too without the encouragement of someone else riding with you.  I'm actually from the UK orirgnally so next time I'm home to visit the fam I'll try and look you up!

Anyways, at work at the mo but looking forward to your next vid.  Hoping there's a fair bit of swearing in this one too! :smile:
```

---
## \#36 Posted by: Nowind Posted at: 2018-03-21T04:28:27.299Z Reads: 402

```
@rich
If they come loose add more Loctide... the hint with the aware of too much was only after seeing people adding a ton of locker and turning out the coils... 

Really nice build Richard, super clean. Great
```

---
## \#37 Posted by: telnoi Posted at: 2018-03-21T05:46:03.753Z Reads: 424

```
The diyeboard 8" tires lasted a bit longer (about double what you mentioned) /never had a flat, but they are hard and stiff. Most likely a different /cheaper composition, but who cares.

Haven't checked if they fit my trampa hubs yet.


It's got tears, bulged...but no flat :sweat_smile:

![2b2437ac2c406cfe68bd81e54b03b30e349906e0_1_375x500|375x500](upload://wiVpGZDzXAahSadRk2nnlb4W0Hf.jpg)
```

---
## \#38 Posted by: DanSkates Posted at: 2018-03-21T11:55:58.472Z Reads: 414

```
Holy shit that's insane!  They look ready to pop! :sweat_smile:
```

---
## \#39 Posted by: rich Posted at: 2018-03-21T12:49:33.969Z Reads: 441

```
@telnoi this is an epic picture of a tyre :rofl: they must wobble as hell, but I like the fact that you never had flats.

This is how my old trampa treads look compared to a new one, i thought when I see the structure of the tyre it's time to swap before they blow up.

![20180208_201548|690x388](upload://zyfuv16YTwtWZkerfqawgTLebAP.jpg)

[quote="benjammin, post:34, topic:45377"]
Saw a thread recently where someone mentioned using an alternative that worked better.
[/quote]

Saw that, too. Looks interesting and I'll try something like that.

[quote="DanSkates, post:35, topic:45377"]
got a nice new dual CNC case for my FOCBOXs now and have just glued some thick rubber to the underside and velcro’d it to my board!!!
[/quote]

Hope you get rid of the heat problems with this case, should help.
Nice to hear the velcro holds up, I also wanted to velcro everything but had no balls in the end and mounted threaded inserts :laughing: it feels much safer for me.

The cam you linked looks good, I already ordered an Apeman A80 but if it's bad I can send it back and order ThiEYE :stuck_out_tongue_winking_eye: . I think compared to my mobile any action cam looks great,hehe.. 

[quote="DanSkates, post:35, topic:45377"]
looking forward to your next vid.  Hoping there’s a fair bit of swearing in this one too! :smile:
[/quote]

:joy: I'm sure that's the case

[quote="Nowind, post:36, topic:45377"]
Really nice build Richard, super clean. Great
[/quote]

Thank you :blush:
I'm really happy with the build beside the bulky case but I like the fact that I can jump on it and swap batteries inside the bolted case, for now it's ok.
Man, the direct drive is really major league :hugs:! Yesterday i rode different paths and through small bushes without any problems. With the belt drive I had to stop regularly to remove all the branches, leaves and rubbish (and couldn't ride through a bush). With this drive I feel 100% unstoppable, great!

Ok, i'll try more thread locker, it was more homeopathic.

Do you personally use spacers and O-Rings or not? In your tutorial video you mount the wheels whithout, that looks easy but with O-Rings it's hard to tell when to stop tightening, on the front truck it's easy.
```

---
## \#40 Posted by: rich Posted at: 2018-03-21T16:29:15.206Z Reads: 434

```
I got mail from china today because last year it was always so dangerous in the dark, used this customized working lamp before:

![20170725_160912|690x388](upload://wmELfgBR0oMqAMGH2moVcB3vcof.jpg)

![20171129_154216|690x388](upload://tfd6R1pdj4595oCpxSU4LcT9VMU.jpg)

But now I need some serious light and found it. It's full metal, no plastic at all.

![20180321_171153|690x388](upload://iJ9otWEkuPwg5pIapULn9BlcTHR.jpg)

![20180321_170921|690x388](upload://clQsYOGnU9aHIUP1kZK0CEvIWzO.jpg)

![20180321_170807|690x388](upload://4Fm6HIvLfeVmuwMlTTrKYJFLL6t.jpg)

Jesus that is bright as hell :rofl:, exactly what I wanted, each lamp is 18W/12V/1.5A
```

---
## \#41 Posted by: Nowind Posted at: 2018-03-22T05:41:23.911Z Reads: 423

```
[quote="rich, post:39, topic:45377"]
Thank you :blush:

I’m really happy with the build beside the bulky case but I like the fact that I can jump on it and swap batteries inside the bolted case, for now it’s ok.

Man, the direct drive is really major league :hugs:! Yesterday i rode different paths and through small bushes without any problems. With the belt drive I had to stop regularly to remove all the branches, leaves and rubbish (and couldn’t ride through a bush). With this drive I feel 100% unstoppable, great!

Ok, i’ll try more thread locker, it was more homeopathic.

Do you personally use spacers and O-Rings or not? In your tutorial video you mount the wheels whithout, that looks easy but with O-Rings it’s hard to tell when to stop tightening, on the front truck it’s easy.
[/quote]


homeopathic thread locker :joy::rofl::joy:

I dont use O-Rings between the Bearings, i normaly just tight the axle nut until the wheel start to block and going a 1/8 backwards... done

For me it was a similar expierence during my first winter seasion with the Direct Drive... fallen leaves and tons of mud was not longer a kind of a problem...

only exposed wires could be problematic by riding through a bush IMO,
 @notger mad some bad expierences
```

---
## \#42 Posted by: rich Posted at: 2018-03-22T09:21:25.831Z Reads: 401

```
Thanks for info, I have to hail the DD again because when I wanted to add thread locker I realized there were 3 bolts missing, only 2 left! What a crazy bulletproof drivetrain where you don't even feel something is missing before the last bolt is gone :laughing:! I guess this is because of the wheel support bearing :grin: 

Have to buy some stainless steel bolts and looking forward to ride again on weekend.

[quote="Nowind, post:41, topic:45377"]
only exposed wires could be problematic by riding through a bush IMO,

@notger mad some bad expierences
[/quote]

Haha, I've read that, too.  If it's not a massive branch my wires should hold, the stress-relief due to the cable feed-through is perfect, only had to remove the wire mesh. BTW I'm not a bush rider, it happend for accident but I like the fact that I can do it.

WIll test without O-Rings and Spacers next time. I'm also thinking about buying 18,2mm spacers and file them down to 17,8mm to make them fit without O-Rings, I like spacer (when they fit).

Sorry, one more question :wink:
How do your metal bushings hold so far?
I'm scared of the plastic ones, even when installing the hanger I scratched  and almost ruined the new ones, they won't remain long.
```

---
## \#43 Posted by: Nowind Posted at: 2018-03-22T09:42:59.424Z Reads: 379

```
Hehe
Yap in the end 3 screws are still one more then you really need .... used one of mine weeks this way just for hardcore testing the parts.... the complete drive is bulletproof... i destroyed one housing and two customer a gear / one with too much play one too less after motor comes loose ... some people pulled out helicoils thats why i warning from too much Loctide... nothing else i know from ... by over 50units not Bad and you can be sure i dont play with my stuff i work :sunglasses: its oversized in a good way... 

Dont get me wrong i use spacers... just no o-rings

You can have some bushings... free for testing... i saw your measuring with 2mm flange thickness... schoud fit in

Let me know what screws you need and i send with the bushings..

Cheers
```

---
## \#44 Posted by: rich Posted at: 2018-03-22T09:55:59.262Z Reads: 381

```
[quote="Nowind, post:43, topic:45377"]
You can have some bushings… free for testing
[/quote]

:heart_eyes::hugs:
Wow, that's awesome Jenso! PM you later, have to work soon...

[quote="Nowind, post:43, topic:45377"]
Dont get me wrong i use spacers… just no o-rings
[/quote]

I forgot you must have correct spacers from the past. Trampa doesn't sell 17.8mm spacer (for Superstars) anymore, only 16.5mm with O-Ring (or 18.2mm for hypa). I have 17.8mm spacers for urban carver but not for 12mm axle.
```

---
## \#45 Posted by: Der6FingerJo Posted at: 2018-03-22T10:41:08.691Z Reads: 355

```
[quote="Nowind, post:43, topic:45377"]
Yap in the end 3 screws are still one more then you really need … used one of mine weeks this way just for hardcore testing the parts… the complete drive is bulletproof…
[/quote]

Damnit Jens you are tempting me, my 3d printed mounts begin come loose even with 4 set screws and enough loctite.
If i don't get it working reliably until Hassloch i might get a Etoxx DD too :D
```

---
## \#46 Posted by: telnoi Posted at: 2018-03-22T11:43:15.363Z Reads: 347

```
colleague of mine has a kick ass 3d printer...tried to print the drive for me, but ended up having a thermal runaway. This is a universal sign...I bought a direct drive.
It will be loud, it will be reliable, it will be good, it will hopefully hold up to my abuse.

No more fucking around with semi-serious attempts. Life's on the line after all.
```

---
## \#47 Posted by: Der6FingerJo Posted at: 2018-03-22T11:48:48.112Z Reads: 349

```
Yeah you're right. But right now i already got so far and have still a few ideas left, so i definitely want to do this right. I never had a total failure until no, just some parts that got wobbly or began to show signs of cracks etc.

My last 100% Infill PETG Motor mount, printed with a higher temperature and less air cooling looks very promisung. A lot better Layer Bonding and no problems for ~40km now, can't wait to get back on my board to test it a bit more. 

The original gear i printed also shows no signs of wear, just the other gear that had problems while printing.
```

---
## \#48 Posted by: telnoi Posted at: 2018-03-22T12:16:00.988Z Reads: 343

```
Your drive is a whole lote safer than mine. In the case of a planetary gear approach, the motor spur wheel has a relatively large space to move around and wobble without blocking the entire drive train, thus causing the driver to crash. With a regular direct drive, there is less space within the enclose. I'm sure your drive will work out.
```

---
## \#49 Posted by: rich Posted at: 2018-03-22T13:27:00.057Z Reads: 381

```
[quote="Nowind, post:43, topic:45377"]
Yap in the end 3 screws are still one more then you really need … used one of mine weeks this way just for hardcore testing the parts
[/quote]

I'm really impressed that you do tests like this :smiley:

I was riding with **2** loose almost lost screws instead of 5, didn't recognize it.
```

---
## \#50 Posted by: lazerusrm Posted at: 2018-03-22T17:32:32.700Z Reads: 396

```
just found this thread! I don't have pics but I built something similar with jens direct drive, except with 80mm 6kw 170kv motors and 12s 16000mah pack and vesc6. 

your board looks dope!I have also been mountain riding in the snow and stuff.. oh it's so much fun! exept... my wife is in surgery after a broken arm after falling off her electric longboard... wear gear! and make your wife wear more!!
I'll attach and old pic with roxxys and a test 12s pack (8000mah)!

![20180223_130929|375x500](upload://kAC4z6v3yvC5piRqqDnPPUgjXDR.jpg)

![20180319_201324|374x500](upload://eDJkHUhUGuj42AeHV8FrWsknq6u.jpg)
```

---
## \#51 Posted by: rich Posted at: 2018-03-22T19:52:55.407Z Reads: 392

```
Thanks @lazerusrm! 
First pic looks great! Must be powerful with these massive motors :grin: :drooling_face:
Second pic, well :sleepy:, wish your wife fast recovery!

This is my "budget" gear for MTB, cost about 100€ all together (except the rabbit), but need some upgrades.

![20180322_204312|690x388](upload://fRob3Yp7oZcdWmpqKXw4DvbTPBR.jpg)

I've mounted my heelstraps again so I'll need asspadding :laughing:
And something for the shoulders and breast. My spine should be protected from my backpack, it is soft plus I want to add a sheet of ABS or wood inside for more protection. I still feel like a jedi fighter. 
Kevlar shirt and trousers would be perfect but all this stuff is so expensive.

But it is very important to wear the gear, when I look at all the scratches on my gear I know these could be scars! Once (with a different helmet) I was landkiting on concrete and I fell backwards, with full energy I hit the ground with the head, didn't know it can happen that fast. I just stood up and sayed such sentence like the guy from the YouTube video "I love helmets" :joy:
```

---
## \#52 Posted by: Der6FingerJo Posted at: 2018-03-22T20:09:24.664Z Reads: 361

```
:heart_eyes: 
I knew something was missing from my esk8 experience!
I need a bunny too :smile:
```

---
## \#53 Posted by: rich Posted at: 2018-03-22T20:15:22.359Z Reads: 359

```
:joy:
The rabbit is very soft but no perfect protection because it would move all the time.
Safety gear should stay always at the same place during riding
```

---
## \#54 Posted by: trancejunkiexxl Posted at: 2018-03-22T20:16:37.913Z Reads: 355

```
watch your gear, mine loves to chew on stuff
```

---
## \#55 Posted by: rich Posted at: 2018-03-22T20:30:37.941Z Reads: 354

```
Haha... I know!
Mine would eat the whole gear within a few days :laughing:
Gnawers are evil and conscience-proof! My rabbit has no cage (only a litter box) that's why almost every single day my flat is getting bigger by loosing some material.
```

---
## \#56 Posted by: trancejunkiexxl Posted at: 2018-03-22T20:51:55.529Z Reads: 334

```
mine 2 free roam of house, has a little box its pretty dope setup
```

---
## \#57 Posted by: routevoom Posted at: 2018-03-24T15:05:16.410Z Reads: 334

```
Hi,
I saw some pictures of your earlier builds... Are those Urban Carver motor mounts from Trampa that you where using on the Trampa MTB?
```

---
## \#58 Posted by: GrecoMan Posted at: 2018-03-24T17:55:28.581Z Reads: 333

```
i’ve always wanted a bunny
```

---
## \#59 Posted by: rich Posted at: 2018-03-24T19:42:42.506Z Reads: 387

```
Yes @routevoom they are, I like them more than the half-closed pro mounts…..

[quote="GrecoMan, post:58, topic:45377, full:true"]
i’ve always wanted a bunny
[/quote]

You need 2 otherwise they are lonely, unfortunately the bunny wife of my rabbit died some months ago :sleepy:

Discovered some interesting telemetry data from my 20.8km  ride today.

![Screenshot_20180324-170630|281x500](upload://nbD3a4d9TeNtFKi3ljzQ8u8m76x.jpg)

Jesus, my top speed on concrete was 49 km/h, that’s my personal record. This is calculated with 190mm wheel diameter (not 200mm like the tyre manufacture claims). @Ackmaniac, any idea why the GPS speed is not working? GPS on the mobile was enabled and also “save GPS position” in the app. Is there something I forgot? 

Interesting that I was faster than the unweighted calculated top speed, maybe it was a small decline.

![DirtMachine-Calculation|645x500](upload://4r1SDTVqWJ3LqtUnKAbsX3Vk9qm.jpg)

Also the vescs got some fever, 37.8 degrees :laughing: (outside temperature was 9)

I took my new action cam for a park ride, this is the unedited footage. I can’t decide what’s the best cam position for “one take” rides. 

What do you guys prefer? I use 3 different cam positions in this video, first from the front, then from the back and then close to the ground with the front wheels only. Or better some footage from the side? Hard to decide, need some help.

https://youtu.be/VqrFHNr99LM

Does someone has a hint for me how to deal with heel straps properly? @benjammin?
I still don’t like them. Today I lost my balance in front of 20 kids and fell down like an idiot, it was so embarrassing. It mostly happens at tight turns at slow speed like at 06:30 in the video above. I enjoyed the rest of my ride without heel straps.

I did some jumping on the bmx-track and recognized a very loud and strange impact noise while landing, I guess it has something to do with my pelicase but I have to check it, didn’t like it at all.

Also the feeling in the air differs very much to my previous version, the balance is different, almost crashed several times :laughing:
```

---
## \#60 Posted by: benjammin Posted at: 2018-03-24T20:42:37.188Z Reads: 355

```
Nice video 👍

Yeah idk about the heel straps, just kinda whatever you feel comfortable with. I'm used to being locked into my board from snow and wakeboarding. I've taken a few falls at lows speeds like that too though. Once awhile back at a red light. Bunch of cars. Sure everyone was laughing their asses off :sweat_smile:

I've also noticed my top speed is always higher, according to my app, than what's shown on the calculator. I've had to plug in an efficiency of 110% to get it to match up. I've been using the other calculator though: http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html?m=1
```

---
## \#61 Posted by: rich Posted at: 2018-03-24T20:51:38.139Z Reads: 321

```
Haha funny, I'm getting exactly the same results as at esk8.it, seems equal.

@benjammin did you set 200mm as wheel diameter in your app? If yes this would be the reason why it shows higher speeds, none of my wheels are 200mm, rather 190mm.
```

---
## \#62 Posted by: AndyBigD Posted at: 2018-03-24T21:08:49.686Z Reads: 331

```
[quote="rich, post:59, topic:45377"]
I did some jumping on the bmx-track and recognized a very loud and strange impact noise while landing, I guess it has something to do with my pelicase but I have to check it, didn’t like it at all.
[/quote]

If you get a loud metallic knock on landing jumps its always worth checking the kingpin bushes in your trucks, they could've worn through?...
```

---
## \#63 Posted by: benjammin Posted at: 2018-03-24T21:13:00.261Z Reads: 320

```
No, I didn't notice an option for wheel diameter in the app. I'll have to look and see.

You do mean the speed app, not the calculator right?
```

---
## \#64 Posted by: rich Posted at: 2018-03-24T21:21:25.988Z Reads: 340

```
It is not a metallic knock that's why I don't think it's the truck, drivetain or the motors. I guess I have to record the noise next time but there were too much people today and maybe it's not the best idea to jump with a selfie stick in the front hand, but I have to for science :laughing:

My bushings are still fine, replaced them a couple days ago, but they will crack again, getting some metal bushings from @Nowind soon :blush: 

[quote="benjammin, post:63, topic:45377"]
You do mean the speed app, not the calculator right?
[/quote]

Yes, do you use an esk8 app or a gps speed app?
```

---
## \#65 Posted by: benjammin Posted at: 2018-03-24T21:28:51.531Z Reads: 315

```
It's just a freebie gps app on my phone (no option for wheel diameter). Tried it in my car though and it seems to be pretty accurate.
```

---
## \#66 Posted by: rich Posted at: 2018-03-24T21:34:19.608Z Reads: 305

```
Ah ok then forget what I said.
Maybe your motors have a higher efficiency than 85% :grin: or you measure when going dowhill only :wink:.
```

---
## \#67 Posted by: DanSkates Posted at: 2018-03-25T00:31:02.729Z Reads: 336

```
DUUUUUUDE!! Loving the new camera work! The first two angles - front and back worked best but the mix is what really kicks ass. You’re riding looks pro now too!!! Really love that’s there’s a few more people getting out there and recording now. I feel like we’re really exploring the possibilities of this sport and crafting its future.

Ref heelstraps @benjammin has a similar background to me and I prefer to be locked in. I actually feel more at risk if my feet or just 1 foot can come out. Like you guys though I still have falls from them - you just get better at jumping slightly and correcting to avoid tipping on to yo ass!!  

One thing I did notice tho is that you wear your heelstraps really low on your boots. I wear mine up above my heel on my achilles and feel more connected to the board that way. When they’re actually on your heel I feel like they’re tripping me up if that makes sense? Give it a go, sometimes a slight adjustment can make all the difference. As well you might find that your foot angle also changes when you have your heelstraps in so possibly changing the angle of your toe straps to compensate (choosing a different bolt setting) will change the feel of the ride too.  Just my thoughts 😁

Loving your work though dude!!

Are they the 150kv sealed UNIK motors btw?? My SK3s are shite and I gotta ride sensored man!! Would you recommend them? They certainly ride smoothly in your board!!
```

---
## \#68 Posted by: Duffman Posted at: 2018-03-25T10:20:56.402Z Reads: 336

```
The dirty little secret to keep balance with heel straps is: jumping!

Because if you are too slow to keep balance by steering you automatically try to keep balance by further tilting the board. If your center of gravity is more off than the width of your wheelbase you sit on your ass.

So, if you are slow and loose balance, just jump up and place the board under your center of gravity again and you are fine. It's not easy to tell your brain to jump if you are about to fall, but it works...

The higher you keep your heel straps while riding the more force you can apply to the board on heelside turns. That enables you to setup your trucks stiffer and keeps you safer from speed wobbles.
```

---
## \#69 Posted by: rich Posted at: 2018-03-25T11:58:21.851Z Reads: 357

```
Thanks for your kind words :blush:

[quote="DanSkates, post:67, topic:45377"]
front and back worked best but the mix is what really kicks ass.
[/quote]

You’re right it’s probably the mix of different angles otherwise it gets boring. I have to shoot more footage and edit later but I’m afraid this has no end. But then I have to remember a sentence which a teacher at film academy told a friend of mine: “You never finish editing, you just stop it”, how true.

[quote="DanSkates, post:67, topic:45377"]
I actually feel more at risk if my feet or just 1 foot can come out.
[/quote]

This is also my biggest fear why I want to use them, also I like the fact that I can do 180s on standstill, I can’t do it without heel straps. Almost every crash ends with one foot or both outside the bindings. Fortunately I never crashed at high speed but I know this will happen one day.

I think I have to grease my ratchets, all 4 ratchets are so hard to open, they always get stuck. It’s not as easy to open as a snowboard binding, it took me about 2 minutes to open one heel strap, that’s really annoying.

But normally I never touch my bindings because they are in perfect position (at least without heel straps :laughing:). In the beginning my bindings were too loose that’s why I cranked them down until I got numb feet. This video helped me a lot finding the proper binding position:

https://www.youtube.com/watch?v=ObNSURYIj9E

For now this is the actual position of my heel straps, got the hint from @Der6FingerJo  

![20180325_101902|690x388](upload://rUtcxlLJAdNhCjzq4ADHHXi8VU4.jpg)

[quote="DanSkates, post:67, topic:45377"]
One thing I did notice tho is that you wear your heelstraps really low on your boots. I wear mine up above my heel on my achilles and feel more connected to the board that way. When they’re actually on your heel I feel like they’re tripping me up if that makes sense?
[/quote]

As you say it that totally makes sense, didn't think about it :grin:
Also a slight adjustment of the binding could do the trick. My main problem are my loose skater shoes, need some proper ones, maybe with ankle support. If I would position the straps at my achilles now they would touch my socks only :joy:.

[quote="DanSkates, post:67, topic:45377"]
Just my thoughts :grin:
[/quote]

I like your thoughts :wink:

[quote="Duffman, post:68, topic:45377"]
The dirty little secret to keep balance with heel straps is: jumping!

Because if you are too slow to keep balance by steering you automatically try to keep balance by further tilting the board. If your center of gravity is more off than the width of your wheelbase you sit on your ass.
[/quote]

Wow, thanks for sharing your dirty little secret :sunglasses:
That makes me hope again, I would never ever think of jumping against falling. Definitely gonna try that, unfortunately I'm at work but I guess tomorrow I'll test it. @DanSkates I just realized you mentioned the jumping, too but @Duffman explained it so well that even people like me can understand it :joy:

The whole gravity thing reminds me of proper steering, when I don't think about it I don't steer with my hip, only by lean, also I have to bend my knees more on tight turns to get better balance.

This is an interesting article about steering a mountainboard:

http://www.mountainboarding.uk.com/learning-the-basics-of-mountainboarding/steering/

[quote="DanSkates, post:67, topic:45377"]
Are they the 150kv sealed UNIK motors btw?? My SK3s are shite and I gotta ride sensored man!! Would you recommend them? They certainly ride smoothly in your board!!
[/quote]

Yes, these are sealed Maytech motors. Unik sells them with 150kv, Overion with 130kv and there are 190kv versions out there, too. Maytech sells them with 170kv. They are powerful and have temperature sensor. The only thing they have a quite high cogging torque (resistance when spinning) which results in funny noises from the gears when you push it very slow. The APS or Trampa motors have way less resistance when spinning, but that's just theory. In pratice these Unik motors are the most powerful motors I've ever had :sunglasses: but I have no direct comparison to another 6374 motor, only 6355 and 6364.

[quote="DanSkates, post:67, topic:45377"]
My SK3s are shite and I gotta ride sensored man!
[/quote]

unsensored? :weary:
Do you run them in FOC? What about cogging, jittering?
```

---
## \#70 Posted by: DanSkates Posted at: 2018-03-25T12:24:14.131Z Reads: 332

```
Love your detailed replies man - and love that you take advice on board so well.  At the end of the day we're all on this wild journey together and it's so good we have a place like this to share information.


[quote="rich, post:69, topic:45377"]
My main problem are my loose skater shoes, need some proper ones, maybe with ankle support.
[/quote]

Yeah this makes a HUGE difference to the feel you get from the bindings.  I rode in skate shoes but as soon as I got heel straps had to move to booties!  I can recommend the Vans Sk8 Hi Pro as they're lightweight but have the right level of padding and support.  I've seen a few other guys riding in Supra Muska's - they look pretty good too.  Or you could do a @Nowind and buy a pair of Burton motos!  @Duffman - what footwear you rocking btw?    

One last thing on bindings.  I LOVE my Trampa, but HATED the toe straps.  The heelstraps are great, but the toes straps sucked for me.  If you wanna explore the option I cannot recommend these comfy beauties highly enough:

https://www.munroboards.com.au/wp-content/uploads/2016/10/mbs-f5-bindings-ratchets-i.jpg

MBS F5.  They do heels to match but I found the combo of these on your toes and the trampa heels works really nicely.  Think a lot of the other guys are rocking these too.

[quote="rich, post:69, topic:45377"]
unsensored? :weary:

Do you run them in FOC? What about cogging, jittering?
[/quote]

YEAH.  I really gotta sort this out - It's a bit miserable I have to say!  So I'm running them in FOC which gives me smooth start up if I'm on a straight or slight downslope, but give me any sort of gradient and I'm hoping around like the easter bunny trying to get going again!!!  :rofl::sweat_smile::sob:  It's tragic really.  I'm on the hunt for the perfect motors currently so will have a look into your other suggestions too.
```

---
## \#71 Posted by: DanSkates Posted at: 2018-03-25T12:32:42.113Z Reads: 295

```
[quote="rich, post:69, topic:45377"]
This is an interesting article about steering a mountainboard:
[/quote]

Hey just watched this - really interesting comments on having loose bindings and pointing your toes in.  Wouldn't have thought you could jump the board with the straps undone!!  Though...I'd like to see him do that with with an extra 10lbs batteries and motors on the board!  :wink:
```

---
## \#72 Posted by: Acido Posted at: 2018-03-25T13:21:47.198Z Reads: 280

```
Cool rabbit, heres mine!
[29513469_1518914438235929_1216827407_o|281x500](upload://uPCsiO3uAhqvXKUc4MmVatijUbz.jpg)

Rabbits are the best
```

---
## \#73 Posted by: rich Posted at: 2018-03-25T13:44:58.655Z Reads: 303

```
I love sharing knowledge, it helps everyone to improve...
Thanks, I'll buy some new shoes soon.

[quote="DanSkates, post:70, topic:45377"]
Or you could do a @Nowind and buy a pair of Burton motos!
[/quote]

Well, probably the best ankle support ever :joy:

[quote="DanSkates, post:70, topic:45377"]
MBS F5.  They do heels to match but I found the combo of these on your toes and the trampa heels works really nicely.  Think a lot of the other guys are rocking these too.
[/quote]

They really look convenient compared to Trampa's "instep" straps (wouldn't call them toe straps). I think I can't resist, started to search for availability in europe :rofl:, nice hint!

[quote="DanSkates, post:70, topic:45377"]
but give me any sort of gradient and I’m hoping around like the easter bunny trying to get going again!!!  :rofl::sweat_smile::sob:
[/quote]

Haha, unfortunately I know what you mean, I really enjoy having 100% cogging free motors in FOC. It's so nice to roll backward on a hill and just accelerate again whenever you want, I feel unstoppable :sunglasses: 

[quote="Acido, post:72, topic:45377"]
Cool rabbit, heres mine!
[/quote]

Hehe, unfortunately I see no pic....
```

---
## \#74 Posted by: Acido Posted at: 2018-03-25T13:51:45.518Z Reads: 307

```
![IMG-20171217-WA0008|281x500](upload://iuYgzRYV3YghmHenRrDziDPQJhw.jpg)
```

---
## \#75 Posted by: Duffman Posted at: 2018-03-25T14:16:32.290Z Reads: 306

```
If I got you right, you keep your bindings locked in position and open your heel straps to get on and off your board. I do it the opposite way: I set my heelstraps to my desired position once and open my bindings to step on the board.

I'm also running mbs f5 bindings, which are indeed very comfortable and can be opened in less than a second. Combined with the older mbs fx 2 heel straps which have no ratched but just slim and light cam locks this is a decent combination. Somewhen I will also try trampa bindings because I'm looking for some wider -> higher heel straps...

@DanSkates: Seriously, you can't switch to sensored motors. You need this kind of handicap to stay on the same level as we are... Else you would just fly away! But if you ignore my words and upgrade anyway get yourself a pair of aps6384 sensored motors. This shoud give you perfect startup in any situation and an extra portion punch on high currents due to the lower resistance. The highernthe kv of the motors the more power you can get from them in real life. Calculate your kv based on a top speed that is 15-20kmh higher than the maximum speed that you want to ride. This way you wont feel any impact of voltage sag if your battery gets drained and still have full punch even if you ride at your maximum (desired) speed.

In the winter and in the dirt I ride some random winter boots and rest of the year I ride in sneekers. They give better feeling for the board and if I bail reallly hard they stay on the board and I sit besides it in socks.
```

---
## \#76 Posted by: rich Posted at: 2018-03-25T18:17:50.007Z Reads: 299

```
[quote="Duffman, post:75, topic:45377"]
If I got you right, you keep your bindings locked in position and open your heel straps to get on and off your board. I do it the opposite way: I set my heelstraps to my desired position once and open my bindings to step on the board.
[/quote]

Now it makes sense to me why you route your power wires on the heel straps :laughing:
Definitely gonna try both ways to see what's best for me.,thanks for info.

Really enjoying to watch your videos and builds, customization to the fullest :+1:

[quote="Duffman, post:75, topic:45377"]
I’m also running mbs f5 bindings
[/quote]

Ok one more reason to try them...

[quote="Duffman, post:75, topic:45377"]
@DanSkates: Seriously, you can’t switch to sensored motors. You need this kind of handicap to stay on the same level as we are…
[/quote]

:joy::rofl::laughing:

I think @Duffman tinkers with the idea to buy some sensored 6384, that's why @DanSkates must buy some sensored 80mm Motors to win the battle :grin:   

@Acido,haha what a sweet rabbit, looks very fluffy :heart_eyes:
```

---
## \#77 Posted by: Acido Posted at: 2018-03-25T18:21:21.319Z Reads: 259

```
The fucker today made a hole in my speaker...
Tomorrow shes getting castrated...
```

---
## \#78 Posted by: rich Posted at: 2018-03-25T18:22:25.073Z Reads: 278

```
[quote="Acido, post:77, topic:45377"]
Tomorrow shes getting castrated…
[/quote]


But that won't save your second speaker :wink:
```

---
## \#79 Posted by: Acido Posted at: 2018-03-25T18:23:54.321Z Reads: 278

```
Its just the cover, I can fix that
It calmed down my second rabbit, hes now low key and just sleeps behind the thrash lol he a male tho
Hopefully the result will be the same
hormones n shit probably
```

---
## \#80 Posted by: rich Posted at: 2018-03-25T18:30:18.413Z Reads: 274

```
Maybe this is the first and only thread where you see pics and discussions about rabbits :joy:
```

---
## \#81 Posted by: Acido Posted at: 2018-03-25T18:30:47.943Z Reads: 254

```
Probably... hahah
```

---
## \#82 Posted by: rich Posted at: 2018-03-25T20:11:20.793Z Reads: 270

```
[quote="Duffman, post:75, topic:45377"]
I ride in sneekers. They give better feeling for the board and if I bail reallly hard they stay on the board and I sit besides it in socks.
[/quote]


:joy:
Forgot to quote that, it's too funny.
It know the feeling standing in wet mud with socks only watching my shoes still inside the binding.
```

---
## \#83 Posted by: Nowind Posted at: 2018-03-26T03:39:40.096Z Reads: 277

```
[quote="rich, post:73, topic:45377"]
Or you could do a @Nowind and buy a pair of Burton motos!

Well, probably the best ankle support ever :joy:
[/quote]


Well in the end i have to say that the Burton Moto is to restrictive for me.
In the beginning it was nice, loved this locked in feeling and the massive Support.
But if you compare with my Supra Mids it is just too stiff .... dont get the right feeling in the longtherm... for a Winter / Snow / Mud Tour they are great but for my regular driving i prefer other
```

---
## \#84 Posted by: Sender Posted at: 2018-03-26T07:16:43.002Z Reads: 267

```
[quote="Acido, post:77, topic:45377"]
Tomorrow shes getting castrated
[/quote]

No "she" can ever be castrated... just sayin'
```

---
## \#85 Posted by: DanSkates Posted at: 2018-03-26T08:51:58.912Z Reads: 285

```
[quote="Duffman, post:75, topic:45377"]
@DanSkates: Seriously, you can’t switch to sensored motors. You need this kind of handicap to stay on the same level as we are… Else you would just fly away!
[/quote]

:rofl::rofl::rofl:

Too funny!!!  

It really is a handicap too!  If we were racing and I fell at the base of a jump I'm screwed!!!  I'd literally have to turn around and take a run up!!  It's that bad!  

In other news, I've really neglected my settings since I blew up my last FOCBOX, and I've had to match the new FOCBOX to the working one that was on that board but the only problem is with that FOCBOX that the USB port broke off :cold_sweat:  So I haven't been able to change the settings on it for a while so I've just matched what I think the saved settings were but its running like a dog at the moment.  Anyways, a BT module turned up a few days ago so I'm going to add that and see if I can connect to my computer that way and set them both up again properly.

Out of interest what are you guys @rich, @Duffman, @Nowind, @Acido running your battery max and motor max at?   I have mine at 80, 80 and the motors make a weird squeeling sound when I try to push them too hard from stand still at the mo.  It's strange - almost like I'm putting too much power into them to even cog!!!  Some times they cog, sometimes they squeel and if I'm on a the flats I role away smooth.  I'll try and record it so you see what I mean...but I think I'm maybe asking too much of them.  Obviuously they need replacing but I have a ride this weds and it would be good to get them to be as good as they can be.
```

---
## \#86 Posted by: telnoi Posted at: 2018-03-26T09:07:47.149Z Reads: 252

```
You're having some bad luck with your gear.
I personally run 80 motor amps/unsensored on SK3 149 KV. They squeel unloaded & no wheels attached at full RPM/did not do this at the beginning, so I guess the bearings need to be replaced at some point. No ill effect otherwise though.
```

---
## \#87 Posted by: DanSkates Posted at: 2018-03-26T09:08:03.463Z Reads: 262

```
[quote="Duffman, post:75, topic:45377"]
if I bail reallly hard they stay on the board and I sit besides it in socks.
[/quote]

This literally made me piss myself laughing!!!
```

---
## \#88 Posted by: DanSkates Posted at: 2018-03-26T09:10:31.042Z Reads: 269

```
Ah shit - seriously?  That's intersting...I couldn't work out if it was the FOCBOXs squeeling to start off with but I defo think it's the motors.  Yeah...I have to say I enjoy the riding part way more than the building!!!  :sweat_smile:
```

---
## \#89 Posted by: rich Posted at: 2018-03-26T09:20:34.505Z Reads: 282

```
My settings on each vesc are quite unspectacular:

![settings|266x45](upload://cTPVCurUfpZx5jau3CVUzDkYjfg.PNG)

In reality I also discharge  amost the full amount of the settings above.
My Battery max is set to 100A because of BMS and 8Ah 15C Graphenes.

What confuses me are the max motor amps when looking at spec sheets. APS states 80A no matter how big or small the motors are (beside 80mm) :laughing:. When looking at the specs of my motors, maytecch says 3550W max = 60A max :roll_eyes:? On a different sheet they say it's rated for 60A and motor max is 65A. That's why I set it to 65A to be on the safe side.

In no way someone can top the vesc settings of @Nowind  :rofl:
I think this makes his day when he see my 65A motor max setting.
```

---
## \#90 Posted by: telnoi Posted at: 2018-03-26T09:25:45.429Z Reads: 261

```
Your issue is a bit weird though. Obviously, bearing noise would only become apparent when the wheels are actually rotating. You're saying it makes that sound when the motor isn't even cogging yet/thus no rotation.
```

---
## \#91 Posted by: DanSkates Posted at: 2018-03-26T09:26:40.581Z Reads: 257

```
Interesting - but you still have heaps of torque and a decent top end so you gotta be doing something right??  :wink:  I might try and tame my setings to see if it resolves the issue in the short term.
```

---
## \#92 Posted by: DanSkates Posted at: 2018-03-26T09:28:08.538Z Reads: 259

```
Yeah I know right?  Hold up - I'll cut a bit of footage where it does it and load it up...They literally freeze and make this high pitched, almost computerised squeel.  They rool perfectly and I've never had it once they're moving just when they're under too much load.

Sorry to hijack your thread @rich - let me know if you want this splitting...
```

---
## \#93 Posted by: telnoi Posted at: 2018-03-26T09:29:12.884Z Reads: 246

```
:D there should be a general trampa/e-toxx build thread.
Sorry @rich
```

---
## \#94 Posted by: Acido Posted at: 2018-03-26T09:32:57.702Z Reads: 241

```
Sterilised then
```

---
## \#95 Posted by: rich Posted at: 2018-03-26T09:37:22.885Z Reads: 272

```
[quote="DanSkates, post:85, topic:45377"]
the only problem is with that FOCBOX that the USB port broke off :cold_sweat:  So I haven’t been able to change the settings on it for a while
[/quote]

Don't remember it, do you use CAN-bus? Then it's no problem to change settings.
Which usb port broke? Master or slave?

[quote="DanSkates, post:92, topic:45377"]
Sorry to hijack your thread @rich - let me know if you want this splitting…
[/quote]

[quote="telnoi, post:93, topic:45377"]
Sorry @rich
[/quote]

Don't worry, this way it's less struggle for me to find interesting content :laughing:

BTW @telnoi if you have a pic of the ascending slope you usually ride, then I want to see it :wink:
```

---
## \#96 Posted by: telnoi Posted at: 2018-03-26T09:40:52.461Z Reads: 262

```
Once the Trampa is up and running, I'll record the ride with my gopro.
I'm not getting on that Diyeboard MTB again.
```

---
## \#97 Posted by: telnoi Posted at: 2018-03-26T09:49:33.646Z Reads: 279

```
That's where I loose 1V. The rest of the 12 km trip is a mixture of up/down hill, where the last bit is 2 km downhill.

![hill|690x454](upload://kPnaR3Oa72NP9AqsBqiU6WUpzMS.jpg)
```

---
## \#98 Posted by: DanSkates Posted at: 2018-03-26T10:34:27.879Z Reads: 294

```
This should be good for a laugh!!!  :sweat_smile:

So here's some footage I just quickly hacked together.  You can hear the squeel right at the start and then again half way through.

I've left some footage either end for all you guys running sensored so you can see the 'real' first world problems of someone running unsensored - I'm literally trapped by that patch of mulch - oh the indignity :rofl:  

https://youtu.be/PgjFZw8tQ08

Thanks @rich for letting me share in your thread!  Like you said - this is a good thread to keep all this good info on anyways and will hopefully help someone else some day.

[quote="rich, post:95, topic:45377"]
Don’t remember it, do you use CAN-bus? Then it’s no problem to change settings.

Which usb port broke? Master or slave?
[/quote]

Oh...I blew both CANBUS trancievers to had to remove them!  So I'm having to run split PPM cable.  I wonder if that makes a big difference too?  Do you find it much better with the traction control?
```

---
## \#99 Posted by: telnoi Posted at: 2018-03-26T10:43:05.557Z Reads: 289

```
no, those are not your bearings...
Sounds like coil whine...could be your motor windings or if it is not coming from the motors, a component with coils if the vesc even has those.

![coil|375x500](upload://5IYLgBp9twnAfcdStWjfR817Dhx.jpg)

you need 4x4 :P
```

---
## \#100 Posted by: DanSkates Posted at: 2018-03-26T10:49:25.210Z Reads: 279

```
Coil whine?  Holy shit.  The only whine I'm happy with is 'red wine'!
```

---
## \#101 Posted by: telnoi Posted at: 2018-03-26T10:52:48.648Z Reads: 265

```
it attracts dogs & rodents from miles away...be weary of that.
```

---
## \#102 Posted by: rich Posted at: 2018-03-26T11:20:15.942Z Reads: 286

```
[quote="DanSkates, post:98, topic:45377"]
I’m literally trapped by that patch of mulch - oh the indignity :rofl:
[/quote]


First, the title of the video makes me laugh really hard :joy:
And on top of that, it's uncensored unsensored drama!

I think I have to shoot a reply video showing sensored mulch startups :wink:

I guess when your wheels spin like in the video they suck a lot of ampere!
Once during riding my wheels lost traction in deep wet mud and spinned like yours, The battery discharge raised from smooth 35A to about 80-90A within this time.

Would love to ride in this skate park and the mulch right now

[quote="DanSkates, post:98, topic:45377"]
Oh…I blew both CANBUS trancievers to had to remove them!  So I’m having to run split PPM cable.  I wonder if that makes a big difference too?  Do you find it much better with the traction control?
[/quote]

Oh, no that's bad.
I've tried with and without traction control,  felt no difference but maybe I wasn't in the proper environment for really testing it. But I never had wheelspins like you, only this one time in mud.

But let's talk about first world sensored problems, yes, even they are existing in hybrid bldc mode :rofl:

https://www.youtube.com/watch?v=RFA9374i2pk

This video reminds me of my first impression of the first version of my build after spending a lot of money and time. I thought: What is this? Really great when riding but I'm afraid to stop because I can't start anymore. Sensored motors in FOC run like a dream, but maybe to smooth for people who like raw power. I have a lot of power but it's still smooth. One day I'll have a look about change settings like acceleration curve or ramping time but for now it feels good.
```

---
## \#103 Posted by: DanSkates Posted at: 2018-03-26T11:38:44.951Z Reads: 282

```
Hahahaha glad I managed to give you a laugh!!  I'd love to see the reply vid! :smile:

I'll get the BT module added and see what's really going on in there - I reckon you're right.  Maybe they're just squeeling because they're in pain!  :crazy_face:

[quote="rich, post:102, topic:45377"]
Would love to ride in this skate park and the mulch right now
[/quote]

Ditto dude - it's lonely here in SA with noone to ride with!  The skate park wasn't really big enough for mountainboards but still good fun.  I'm actually looking to head over to the Shed skatepark in melbourne in the next couple of months as I've connected with Dylan Warren (Mountainboard God for MBS) and he's keen to feel the power of one of these things!  I can't wait to see what he can do on my board!  I'm totally gonna sort out all the problms I have before I fly a board out there and the bloody thing blows up or kills him!  I'll be sure to film it too - that skatepark has a foam pit and everything!

[quote="rich, post:102, topic:45377"]
But let’s talk about first world sensored problems, yes, even they are existing in hybrid bldc mode :rofl:
[/quote]

That's completely how my board behaves!  Bloody embarrasing!  I gotta head over to sensored asap.
```

---
## \#104 Posted by: scrapheap Posted at: 2018-03-26T11:54:13.798Z Reads: 270

```
Gentlemen, I think the word you might be looking for is spaded O.o...
```

---
## \#105 Posted by: Duffman Posted at: 2018-03-26T12:14:43.546Z Reads: 279

```
Hey guys, I'm running quite conservative 100A / 100A settings on my vesc 4.11 right now, after I burned a motor in summer on 120A / 120A.

This was just a quick test with blocked motor:
https://youtu.be/VUQ_XAvSJqc
```

---
## \#106 Posted by: DanSkates Posted at: 2018-03-26T13:43:01.460Z Reads: 270

```
WOW - that's insane!  So what's your upgrade to make the 4.11 perform like that?  Steriods?  Viagra?!! :face_with_raised_eyebrow::sweat_smile:  If you can make that VESC perform like that then what's the advantage of higher spec VESCS?  Are you running FOC too? I need to revisit some of your old posts I think!  I've read them so many times but everytime I do they seem to make more sense :wink:  

We need a  @duffman and @nowind collaboration thread on how to build the most insane eMTB!
```

---
## \#107 Posted by: rich Posted at: 2018-03-26T17:12:21.100Z Reads: 278

```
Just came back from a wicked ride session.

@DanSkates  I recorded videos of startups on any terrains including mulch which will make you cry and order sensored motors :rofl:
I have so much material that I have to edit it (quick and dirty), was on bmx-track, did slides (at least tried)...... and captured some funny fails including standing on the ground with one sock only.

Thank you so much for the hint with the wrong position of heel straps. This time I used them on a higher position and quite loose, was much much better and I enjoyed it. 

@Duffman also the jumping instead of falling works well :+1:
I lost one half heel strap but found it again. My ride was over after 17km and my second puncture within 3 rides. Now I need to buy more bicycle repair kits.

![20180326_175406|690x388](upload://gGGUNImwVbwsai2ORAWJ0zbS9cY.jpg)

EDIT: bought more than that :grin:
I'm tired of punctures, will try some new stuff. 
Did also some research about kevlar stripes which would be good between tube and tyre but mostly I find kevlar for fire artists, don't think it's cut resistant.

![20180326_195406|690x388](upload://nfpOR5YzA0CXUE749HjFG2k5g3o.jpg)
```

---
## \#108 Posted by: Duffman Posted at: 2018-03-26T19:20:05.854Z Reads: 268

```
Go sensored or go home!!!

@rich Glad to hear that you start enjoying your heelstraps. Give them a few more rides and you can't ride without them anymore.

@DanSkates I'm running BLDC to get the most out of my VESCs and I avoid running FOC on 4.x hardware...
But as you are already running FOC you could also switch to an AS5047 setup, which is technically even better than hall sensors and cheaper as you can keep your motors. The problem in your case is that you would have to reconfigure your VESCs...
```

---
## \#109 Posted by: Ackmaniac Posted at: 2018-03-26T20:36:26.580Z Reads: 265

```
When you fix the CANBUS you can setup the VESC with the broken USB via CAN.
And i had problems with unsensored motors at startup as well when they make this high frequency sound.
What helped in my case was to raise the swithing frequency to 30 kHz (which i do at all my motors). 
And i also increased the Observer Gain At Minimum Duty which helped the most in my case. But every motor is different.
![image|690x158](upload://kI4VK34kg62H1yUHLNVq4H0d1Um.png)
```

---
## \#110 Posted by: DanSkates Posted at: 2018-03-26T21:04:34.497Z Reads: 266

```
[quote="Duffman, post:108, topic:45377"]
switch to an AS5047
[/quote]

Ooooohhh yeah I remember when @nowind documented doing this with your support!  I'll do some research on past builds to see if I can figure this out - great idea - I totally forgot about this.

[quote="Duffman, post:108, topic:45377"]
The problem in your case is that you would have to reconfigure your VESCs…
[/quote]

I'll get these sorted - there's a couple of local shops that I'm sure could fix this if - if not I'll buy a hot air station and do it myself.  It's long overdue!

Thanks @Ackmaniac - once the VESCs are configureable again I'll test these tweaks too!  amazing that they fixed the squeeling motors!   Thanks for jumping in here too - your support is always appreciated.

@rich - can't wait to see the videos dude!!!!  Sorry you keep getting punctures - it appears my achilles heel is my motors and yours is your tyres.  Thorns are like you kryptonite!!! :sweat_smile:
```

---
## \#111 Posted by: rich Posted at: 2018-03-28T23:04:59.358Z Reads: 264

```
Finally I managed to upload at least one video, there are some problems with audio but I can’t open the project anymore, that must be fate. Need to fix the problems before I edit the rest. 
@DanSkates I didn’t forget the reply video, coming soon! :wink: 

https://youtu.be/TTUdD-7KH4s
```

---
## \#112 Posted by: DanSkates Posted at: 2018-03-28T23:36:35.271Z Reads: 257

```
Duuuuuude!  That's such a sick edit - i loved it!!  The baby music with the bikes had me pissing myself!!  And the section with your missing heelstrap - very funny dude!  Can't say enough good things about this.  Also, sweet riding dude!  Sitting at my desk at work deperate to get out to the BMX park now.  Can't wait to ride this easter weekend!

Looking forward to the next video to man - looks fun!
```

---
## \#113 Posted by: rich Posted at: 2018-03-29T00:02:38.356Z Reads: 251

```
Hehe, glad you like it! The editing was not really planned before, it just happened. But now I have some funny ideas for a different BMX track when I find some time.
```

---
## \#114 Posted by: benjammin Posted at: 2018-03-29T01:37:51.990Z Reads: 248

```
😂 that was hella funny with the music change with the bikes! Nice vid 👍 I gotta get some pads and start hitting the bike tracks. Looks like a blast!
```

---
## \#115 Posted by: rich Posted at: 2018-03-29T10:52:39.591Z Reads: 261

```
[quote="benjammin, post:114, topic:45377"]
I gotta get some pads and start hitting the bike tracks.
[/quote]


Does that mean you don't wear any pads right now? :crazy_face:
I really like my ellbow and forearm protectors, they saved me from some nasty cuts when falling in the BMX track from video above. 

![20180329_124036|690x388](upload://mBlld0ZoHVhgTD0xlRDfTGG8Us1.jpg)

Stones are evil! When I was a kid I was falling with my BMX without protectors, you could see my kneecap and gravel everywhere underneath the skin on different spots. Well, after surgery it took some weeks to recover. I prefer protectors more than hospitals these days.
```

---
## \#116 Posted by: rich Posted at: 2018-03-29T13:03:34.253Z Reads: 265

```
After some detailed research of spots in my hometown I found some awesome places, the second one is not my league yet but maybe one day. But they have a trial ramp with foam blocks, I want to try that :sunglasses:

https://www.youtube.com/watch?v=xpajNZI7Ghk

https://www.youtube.com/watch?v=U9eU76j-SZE
```

---
## \#117 Posted by: benjammin Posted at: 2018-03-29T17:11:16.610Z Reads: 256

```
I've just been wearing a fullface and wrist guards.
```

---
## \#118 Posted by: DanSkates Posted at: 2018-03-30T01:40:51.302Z Reads: 257

```
Wow! So these spots are local? Sick! I’d love to try the jump with the soft landing.
```

---
## \#119 Posted by: Cobber Posted at: 2018-03-30T02:52:38.046Z Reads: 272

```
Dan with your motor/battery max the same as your battery voltage drops your board will feel as though it is dying...

I was talking to Decky about it in this thread over here. Essentially setting a higher motor amps will _**help**_ compensate the above. Although using Ack's watt control or similar is the only way to get a linear delivery.

http://www.electric-skateboard.builders/t/pushing-the-limits-of-motor-amps/49277/9?u=cobber
```

---
## \#120 Posted by: Cobber Posted at: 2018-03-30T03:15:48.158Z Reads: 263

```
Hi Ack, I've read a few times to increase switching frequency of brushless motors, now my understanding of controllers and motors is limited... so
Is a side effect of increased switching frequency more losses (heat) in the controller at higher rpm and less ripple voltage at low rpm?
```

---
## \#121 Posted by: rich Posted at: 2018-03-30T13:05:16.580Z Reads: 274

```
The second spot with the ramps I can reach within only 10-15 minutes. Guess I wear my brown trousers so nobody can see that I'm scared to death. But need to practice on smaller ramps first and then with foam blocks before I feel comfortable to do it.

Uploaded this video for demonstration of smooth startups on any terrain with sensored FOC.

https://youtu.be/HUcIlua5FjI

BTW this is how I service my MTB, it's a stand for speakers up to 40kg, this way I have access from all sides. Often I use it for storage, too. Looks good and saves space. 

![20180330_123228|690x388](upload://uaZgt1cu6CLsKN1vYbQbhQ58KNd.jpg)

Fixed some tubes and wanted to replace the punctured tube. First I recognized the slice in the tube instead of a mini hole. Then I found the reason, look at this scar tyre :laughing:

![20180330_132210|690x388](upload://59YDr87wLQmF69QOPrSDJPhw6XP.jpg)

It happened when I went full throttle uphill a steep path with gravel and stones. Once one wheel lost traction and spinned very fast. I guess there was a sharp stone or something, crazy
```

---
## \#122 Posted by: rich Posted at: 2018-04-04T13:10:16.358Z Reads: 274

```
My board is out of order because one motor spur gear came loose after 100km. The problem is that the key wiggles  a little bit inside the keyway of the motor shaft and 1 grub screw only can't withstand the force. Now I soaked it in thread locker and hope it will last. If not I need to file a flat spot or glue the gears which I want to avoid.

![20180403_171756|690x388](upload://d2JxZNTQAamF4fTOzDiW7PB5VjZ.jpg)

I wish the grub screw would be 1mm closer to the gears, then I wouldn't have to dismount the motor, I'm lazy :laughing:

![20180403_182803|690x388](upload://umgL7wGhFIL9SFhkWx8ePcN9oBD.jpg)

I'm using Innotec total power grease for the gears. The description says it's thin like oil when applying and becomes a grease after some time. I used a lot but there is almost nothing on the gears and what's strange that the grease is sticky. I have no experience with grease but I didn't expect it sticky. I think I have to use a lot more of this grease, too.

My other problem is is this:

![20180404_134818|690x388](upload://iqfLPRnwaCXvbnbkeJhTS9beH3l.jpg)

![20180404_134923|690x388](upload://1IHP4sCIL5UXFXLjzSP2negUxVr.jpg)

And this is after 100km only, need to protect the drivetrain and used 1mm thick self-adhesive full rubber, that should help, we'll see. 

![20180404_141948|690x388](upload://dJJgLGYtYL0wVtw5OOMauhdzluk.jpg)

![20180404_142536|690x388](upload://r3SZfq7jtU2wAZJLBa90R6Wstay.jpg)

Beside this small problems I really enjoy the spur gears and don't miss my dirty belts :wink:
Tomorrow I'm ready to ride again...
```

---
## \#123 Posted by: DanSkates Posted at: 2018-04-04T14:16:45.526Z Reads: 268

```
I have had the same thing happen to me recently buddy!  RED LOCTITE!  

http://henkeladhesivesna.com/blog/media_uploads/Loctite%20Threadlockers.png

Once the 263 sets the only way you get the gear off again is with a blowtorch!!  Honestly I had to remove one recently and I could only get it off with a blowtorch!  I know @nowind recommends just loctiting the shit out of these parts too to ensure they don't move!  I forgot to add this when I adjusted the motor pulley a few weeks back and it came loose after 10 jumps or so.  Put the red back on again and the mother ain't going nowhere!

I like your hack with the rubber protector - I'm totally gonna try this too and mine a getting a bit gnarley underneath and I wanna start hitting rails but currently even catching it on a curb makes me wince.

Can't advise on grease - I'd love to know some good options here too as the one I'm using feels a little thin.
```

---
## \#124 Posted by: rich Posted at: 2018-04-04T18:31:16.552Z Reads: 260

```
Good hint with the red loctite,  this is my last option. Did you need any special tools to remove the gear after using the blowtorch?

[quote="DanSkates, post:123, topic:45377"]
Can’t advise on grease - I’d love to know some good options here too as the one I’m using feels a little thin.
[/quote]

Maybe I'll try white lithium grease next time, seems much thicker but could be a mess.
```

---
## \#125 Posted by: telnoi Posted at: 2018-04-05T19:27:17.606Z Reads: 254

```
Any idea what you are hitting?
```

---
## \#126 Posted by: ArnhemAnt Posted at: 2018-04-05T21:57:58.759Z Reads: 261

```
[quote="DanSkates, post:123, topic:45377"]
Can’t advise on grease - I’d love to know some good options here too as the one I’m using feels a little thin.
[/quote]


I contacted a commercial company here in Australia. They sell massive quantities of lubricants to mining companies, etc. I explained the situation with the direct drive units and they highly recommended a product called Becham PAL 1 grease. I was fortunate enough to order a small quantity (100g) from them.
Hope this helps.
```

---
## \#127 Posted by: rich Posted at: 2018-04-06T03:24:10.208Z Reads: 254

```
[quote="telnoi, post:125, topic:45377, full:true"]
Any idea what you are hitting?
[/quote]


Yes I can remember every single time, the sound is heartbreaking :weary:
50% was because of hitting curbs, I always try to pass them straight but sometimes it happens when riding  a little bit diagonal. The remaining 50% are mostly stones laying on paths or in the grass. The ground clearance is about 35mm. But the drivetrain seems bulletproof, no matter how hard you hit it. With belt drive that happened, too (seldom because of more gound clearance) but the result was either a damage of pulley teeth or a broken belt. 

[quote="ArnhemAnt, post:126, topic:45377"]
they highly recommended a product called Becham PAL 1 grease
[/quote]

Wow, thanks for the tip, did some research and this stuff seems high tech, great! Also I like the fact that it shall absorb some noise. There is only one thing I'm worried about, the shops where it's available state "price on request", that must be some expensive shit :laughing: 

Please let us know when you've tested that grease!
```

---
## \#128 Posted by: Mobutusan Posted at: 2018-04-06T06:43:11.684Z Reads: 256

```
How about something like a gear oil for car differentials? Not nearly as thick as grease, but should keep the gears nicely coated and bathed at all times. 

https://www.amazon.com/Red-Line-57904-Synthetic-Oil/dp/B000CPCBF0
```

---
## \#129 Posted by: telnoi Posted at: 2018-04-06T06:48:36.323Z Reads: 250

```
Was hoping it would be just curbs :smile:
Got a decision to make. Got a 20mm belt drive with tensioner and a direct drive. Offroad pretty much consists of rocks sticking out from the ground at different angles mixed with sand.
```

---
## \#130 Posted by: ArnhemAnt Posted at: 2018-04-06T08:04:51.585Z Reads: 247

```
[quote="rich, post:127, topic:45377"]
There is only one thing I’m worried about, the shops where it’s available state “price on request”, that must be some expensive shit :laughing:

Please let us know when you’ve tested that grease!
[/quote]


Not that expensive at all. I think I paid about $20.00 for the 100g container and there is a LOT there.
I'll be sure to let you know how it goes once I get the board together, but from just looking, and feeling this stuff, I think it will be perfect. It has a great consistency and I'm pretty sure it's going to stick like shit to a blanket on those gears.
```

---
## \#131 Posted by: rich Posted at: 2018-04-06T11:56:05.398Z Reads: 253

```
[quote="Mobutusan, post:128, topic:45377"]
How about something like a gear oil for car differentials?
[/quote]

That could work if it's acid free. 
But next time I want to try a thick grease like white lithium, it's cheap and also recommended for spur gears. I think with a thick grease there is less friction on the gears and a little bit less noise but I'm no engineer, just my thoughts. Only downside is that I have to open the gearbox to add that grease, the grease which I actually use can be added through the greasing access point.

[quote="telnoi, post:129, topic:45377"]
Got a decision to make. Got a 20mm belt drive with tensioner and a direct drive. Offroad pretty much consists of rocks sticking out from the ground at different angles mixed with sand.
[/quote]

On normal paths you can avoid bigger stones because you see them, in deep grass it's different. Some of the scars on my drive are from a dirt park where are massive stones on bumpy terrain, hard to avoid.

With belt-drive I hit some stones in this dirt park, too but as mentioned I hit the stones with belt and wheel pulley. I prefer to hit these stones with the sturdy DD housing. IMO the direct drive is the winner and you could add some protection before using it to prevent any damage.

I don't like cleaning but I love to clean this drivetrain :laughing:
Had it fully covered with mud already, it's sealed so no problem at all. And nothing can enter, with belt drive I had regularly to remove things like leaves, sticks, high grass and so on. Now when I hear a scraping noise it's just something which got stuck in the holes of my hangers.

The only reason to use belt drive would be the noise if this is important for you.

[quote="ArnhemAnt, post:130, topic:45377"]
I’m pretty sure it’s going to stick like shit to a blanket on those gears.
[/quote]

That sounds promising :joy: 
Good luck with your build!
```

---
## \#132 Posted by: telnoi Posted at: 2018-04-06T16:54:24.660Z Reads: 224

```
Yeah, I can't avoid that crap here. The path that can be driven is about twice as wide as the mtb. Will choose ground clearance for now. I'll double check the clearance around  certain areas and may change things out or complete a second board for cruising.
```

---
## \#133 Posted by: DanSkates Posted at: 2018-04-07T22:53:13.932Z Reads: 231

```
[quote="ArnhemAnt, post:126, topic:45377"]
Becham PAL 1 grease
[/quote]

Hey @ArnhemAnt - just been on there website - there's ALOT of options! :smile:

Which one did you go with?  Looks like they have some incredible grease!
```

---
## \#134 Posted by: ArnhemAnt Posted at: 2018-04-08T01:11:13.676Z Reads: 234

```
Dude - send me your postal address and I'll shoot some of this stuff down to you.
```

---
## \#135 Posted by: DanSkates Posted at: 2018-04-08T05:33:01.550Z Reads: 242

```
Legend - thanks buddy.  I'll pm you now...
```

---
## \#136 Posted by: rich Posted at: 2018-04-08T12:42:47.570Z Reads: 261

```
The rubber protectors were not really useful, after one ride 3 of 4 protectors are damaged :smirk: The brown colour is dust sticking on the glue.

![20180407_195653|690x388](upload://vymrEtnMnJmFAbWSHw3wQfx73dz.jpg)

But I had a wicked ride session today. Inspired by @DanSkates I'm developing my freestyle skills and made my first 180's :sunglasses: Took some footage from there and from skate park. Need to edit it but for now some stills:

![Grass_06|690x387](upload://c84f2Lzy3KpEFYFB40TFQBWBI9j.jpg)

![Grass_07|690x389](upload://2HgPGrIVvpHh2oG1yGcAeWRFV6a.jpg)

![Skatepark_01|690x387](upload://vHaoaEdH5PhbcmiOvfa78cY0bG1.jpg)

![Skatepark_06|690x387](upload://ijeWdnw2rEKLYnLNhba2nqUEfUn.jpg)

![Skatepark_03|690x386](upload://Yu8n5GjCSlNl5nsyp29TAS1aRO.jpg)

In the end I was in dirt park and had some painful falls, but no footage recorded. I definitely need ass padding.
```

---
## \#137 Posted by: telnoi Posted at: 2018-04-08T15:45:38.140Z Reads: 241

```
Almost nothing sticks to it I noticed today.
Best solution I can think of is to create a bumper pad with the exact curvature of the drive that locks onto the axle.
```

---
## \#138 Posted by: Mobutusan Posted at: 2018-04-08T15:52:43.900Z Reads: 251

```
Cool shots! Even though I can't figure out how you got into the air on those first two jump pics. Invisible ramp? :crazy_face:

And for your DD sealing, this liquid/paste gasket maker might be the ticket. Just paint a light coating on the mating surfaces of the case halves, bolt it together, and let it dry. 

https://www.amazon.com/gp/aw/d/B0002UEN1U/ref=mp_s_a_1_1?ie=UTF8&qid=1523202850&sr=8-1&pi=AC_SX236_SY340_QL65&keywords=permatex+ultra+black

Or you could get some gasket sheet material and cut out custom gaskets. That might actually be better if you have to take the gear box apart later. I don't know what material might work best, but you could get a pack like this and experiment for cheap.

https://www.amazon.com/dp/B000CNKUGO/ref=cm_sw_r_other_apa_8NJYAbQSWTH87
```

---
## \#139 Posted by: rich Posted at: 2018-04-08T16:26:37.337Z Reads: 253

```
[quote="telnoi, post:137, topic:45377"]
Almost nothing sticks to it I noticed today.
[/quote]


Yeah that's really great :metal:

[quote="telnoi, post:137, topic:45377"]
Best solution I can think of is to create a bumper pad with the exact curvature of the drive that locks onto the axle.
[/quote]

Probably the best solution, also best for the DD, it must be rigid but would take to much space eventually.
But in my case the housing is strong as on day 1 and I hit it hard sometimes. It happened several times that I landed on one DD housing when trying to ollie up a sidewalk with too low speed. This drivetrain is bulletproof, no doubt. It makes me ride and jump like never before, e.g. didn't ollie with belt drive before :laughing:.

[quote="Mobutusan, post:138, topic:45377"]
Cool shots! Even though I can’t figure out how you got into the air on those first two jump pics. Invisible ramp? :crazy_face:
[/quote]

:rofl: 
You are right, it's an invisible ramp. The lower path before is concrete and the steep ramp is dirt/grass and about 50-60cm high. The landing is grass with some dog shit, it's in the city. Here I am standing in front of the ramp.

![Grass_09|690x388](upload://vo6d0tE0ujtbGO89oaZ6JjAonDx.jpg)

[quote="Mobutusan, post:138, topic:45377"]
That might actually be better if you have to take the gear box apart later.
[/quote]

Thanks for the links, maybe I'll need them later but right now there isn't much dust inside the gear box, just a little bit on the edges of the gear box but not on the gears. If I see more dust in the future I'll check them out.
```

---
## \#140 Posted by: telnoi Posted at: 2018-04-08T16:46:47.299Z Reads: 241

```
Ah well, fuck cosmetics. Got direct drive installed now. If you haven't driven it before you don't know what you are missing, but the feeling of letting go of gas and still feeling the momentum instead of being on belt resistance brake is really something.
```

---
## \#141 Posted by: rich Posted at: 2018-04-08T17:03:00.823Z Reads: 235

```
Agreed, the free coasting is beyond words....
```

---
## \#142 Posted by: rich Posted at: 2018-04-09T20:00:03.165Z Reads: 253

```
I have new victims due to my jumping, both new bushings on the rear hanger are broken after roughly 150-170km :roll_eyes:. Fortunately @Nowind sent me metal bushings, hope to receive them soon so I can ride again.

After my falls in dirt park yesterday I "designed" an ass,back, hip and rip protector made of insulating mat for free :rofl:. It is very hot underneath and not comfortable but today I was lucky to wear it because after a jump I lost balance and fell on my ass and back quite hard. BTW need a professional solution for this.

![20180409_175340|690x388](upload://totkT64jTCZYkMEtVReywLwnXqL.jpg)

Recorded some jumps before I recognized the broken bushings, video coming soon!

![Dirt_3|690x387](upload://b4ZUcoJXkrskmJxAiAVE6qouFhe.jpg)

![Dirt_4|690x387](upload://qKX0g00mwIJQWk937YBCRQUHy3o.jpg)

![Skate_1|690x388](upload://uV9XpHVKYjXfqCZNVYPXoxjw1nw.jpg)
```

---
## \#143 Posted by: okp Posted at: 2018-04-09T20:25:12.825Z Reads: 240

```
sick ! you do really well keep the balance in the air.  Impressive!
```

---
## \#144 Posted by: rich Posted at: 2018-04-09T20:35:14.442Z Reads: 242

```
Thanks, bro!
The difficult part is not the balance in the air, it's more finding and keeping the balance after landing :laughing:. But I'm still a beginner in freestyle and need to learn a lot :wink: Right now I feel every single part of my body. Normally I don't crash when riding but when jumping it's part of the game as rookie.
```

---
## \#145 Posted by: DanSkates Posted at: 2018-04-10T04:50:51.213Z Reads: 248

```
THAT NOSE GRAB IS THE SICKEST THING I'VE EVER SEEEEEEEEEEN!!!  Dude - dope!!!  I need to practice that :smiling_imp:  and again - you seem to be doing them without a kicker?  WTF?  :joy:

Loving these photos!  Are those stills from your action cam?  Are you shotting in 4k?  What's your frame rate?  

I'm getting seriously excited by your riding dude.  YESS!!!  

Everytime time I see your posts I just wanna get out there and ride!

Yeah as for ass pads I'm gonna pull the trigger on the Hillbilly pads.  I constantly fall on my coccyx and it hurts like hell!!  

Keep up the good work bro!
```

---
## \#146 Posted by: rich Posted at: 2018-04-10T12:42:30.265Z Reads: 261

```
[quote="DanSkates, post:145, topic:45377"]
THAT NOSE GRAB IS THE SICKEST THING I’VE EVER SEEEEEEEEEEN!!!  Dude - dope!!!  I need to practice that :smiling_imp:  and again - you seem to be doing them without a kicker?  WTF?  :joy:
[/quote]

That thing is the sickest fake nose grab I've ever posted :joy::joy::joy:
I wanted to grab the deck but had really bad balance in the air so rotated my arms to avoid a crash. At home when watching the footage I recognized it looks like a nose grab :rofl:

Well, this is the hidden truth:
On the dirt ramp of the table I push the deck down and then lift it for jumping and normally bend both knees but in this case my balance was too much backward and I made it even worse with bending the front knee only. So I aborted the grab and tried to move the body mass to the front. As you can see I didn't make it. When your ass is above the rear wheels it's not a good sign :laughing:. What you don't see on the pic is that I fell backward down the hill on the other side, there is hard dirt and stones. It was the fifth and last jump I've recorded. After that I prefered to behave like a normal adult on the remaining ride and left the park.

Also the landing zone of this table would be on the right edge of the pic, need more speed and cojones.

![Jumpfail|690x388](upload://kX9piCYbx6Hu3YFKOSHARXCPIOL.jpg)

Let's see if I can do a real nose grab, gonna try that :sunglasses:

BTW, the stills are taken from the footage of the action cam, recorded in full HD 30fps. My laptop is old and doesn't like 60fps or more. The jumps would also look much better in slow motion but for now I record 30fps. I would have a program for fluid slow motions, too but my laptop says no. First world problems :roll_eyes:

I shoot with 170 degrees angle and it is sick when looking at the pic above. When I do the "nose grab" I'm small, and when landing I'm much bigger. I'm just a little bit closer to the cam, that's really weird.

[quote="DanSkates, post:145, topic:45377"]
Everytime time I see your posts I just wanna get out there and ride!
[/quote]

Same here :metal:

My next step is to ride a real kicker, never tried that before but the gap is scary, need to find one without or in skate park (or find someone with a portable kicker). Jumping on a double is something that is far away from now.
```

---
## \#147 Posted by: DanSkates Posted at: 2018-04-10T12:54:59.039Z Reads: 249

```
I love your honesty dude!  Fact is - a lot of shots in skate mags, snowboard mags, surf mags etc give the impression of the perfect trick when in actual fact the landing isn't always there.  I think the path to us sculpting the future of this sport is honesty, sharing and learning....together!  

And...in the spirit of sharing I went on a group ride a few weeks back and I've been trying to edit the footage for ages now but like you my computer hates me and it takes FOREVER to render anything!  Anyways, having spent the last 5 hours or so uploading it to youtube it's at 97% so I'll upload it to my thread very shortly.  It's mostly just plain riding with a couple of small jumps, but the best bit is in the first 30 seconds when I land right on my ass!  :joy:  So it should make for some light entertainment! :smile:

There's also a kind of review of a Bajaboard during my first run on it which I have to say I really loved!  In hindsight though I prefer my Trampa and once I have the cogging issue sorted it'll be better for sure!

I'll be sure to tag you in a mo when I upload it! :rofl:
```

---
## \#148 Posted by: hornet90 Posted at: 2018-04-10T13:01:30.131Z Reads: 234

```
Just on the grease we did a lot of testing here in work and we found food safe white grease to be more silppy 
than brown and high end red and lasted longer .......
```

---
## \#149 Posted by: TarzanHBK Posted at: 2018-04-10T13:27:44.756Z Reads: 233

```
Look at my profile pic from snowboarding. Same here :smiley: My brother took an awesome shot and i concentrated more on the camera than on the landing. So after that pic, i ate some bushes :monkey:
```

---
## \#150 Posted by: rich Posted at: 2018-04-10T13:41:46.355Z Reads: 233

```
In the end it is the pic which counts :sunglasses: (but a pic eating the bush would be funny, too)
The camera makes me pushing the boundaries, the result is either a nice video or a fail. I wouldn't hide the fails because I enjoy watching them even when it's me and I also can learn from it.
```

---
## \#151 Posted by: rich Posted at: 2018-04-12T12:40:41.169Z Reads: 252

```
This is my new video with edited footage from the latest jumping and ride sessions, hope you enjoy it!
I really like the action cam because it pushes me to do something new like my first 180's here, can't wait to try 360's (or showcase the fails). Almost every ride I try to improve my skills just a little bit, also with the help and hints of you guys! It's really a big motivation for me.

I'm glad if I can inspire others like others inspire(d) me.

For example, last year I wanted to build the second version of my longboard, ordered many parts already but then I saw the urban/street carver builds of @Kaly and @whitepony and fell in love. This was the end of my longboard project and I sold all parts to build an urban carver, too. 
Same for MTB, I had a bad wood MTB which I wanted to electrify but after seeing all this nice Trampa builds here I knew this is exactly what I want, wood MTB with velcro straps sold :metal:. This is the beauty of DIY and this forum, you can read 10 build threads, get the knowledge and combine the best ideas for your own board.

BTW @Nowind YOU are fucking legend (ok, helicals, too) and a big inspiration for all of us, love your builds, threads, videos, products......

https://youtu.be/e52hsv-BzGY
```

---
## \#152 Posted by: Silverline Posted at: 2018-04-12T19:32:03.732Z Reads: 241

```
I see you are using yellow dampers in you front/rear springs ... Is it okay to carve still ? Is it to prevent speed wobbles ?  What is your weight, if i may ask :-) ?
Nice video btw.
```

---
## \#153 Posted by: rich Posted at: 2018-04-12T22:24:46.947Z Reads: 233

```
If you ride on streets and with lower speed no dampas are fine for carving but offroad it feels better with dampas. Once I rode without dampas but it is too spongy for offroad. Also I've removed the front dampas once but got a scary speed wobble on concrete at 39km/h (24mph). With yellow dampas I've never had a speed wobble up to 49km/h (30mph) and it feels good with a bit spring pre-tension. My weight is about 74kg (11.6stones).
```

---
## \#154 Posted by: DanSkates Posted at: 2018-04-13T09:43:17.423Z Reads: 228

```
DUUUUUUUDE!! 🤙🏻

EPIC riding and super well edited video man! 

Loved the skate park section too! And the part where you lose your shoe 😂🤣😂 I think you and @Duffman need a losing shoes compilation! I have one of those too from pre-electric days - I’ll share it with you 😂
```

---
## \#155 Posted by: rich Posted at: 2018-04-13T10:58:03.509Z Reads: 251

```
Thanks bro!

Still trying to improve riding and editing skills :laughing:
Skate park is scary because of the concrete, it's not a good place to fall (guess why I know). I like the landing in soft grass most but it's hard to find natural kickers, the one in the video is nice but the approach is not long enough to get the speed for trying 360's, which is one of my next ambitions.  

Because of the broken bushings I had to dismount the enclosure and rear hanger but got a chance to take a pic of my magic gasket :sunglasses:


It is HSF foam sealant tape 600 and I love this stuff. There are many different sizes available. I chose 1cm width and for 1-4mm gaps. Compressed it is 1mm but after some minutes it's 10mm and is very fluffy. When it's 60% compressed it's almost waterproof (but 100% splash proof) and for temperatures up to 80 degrees. On my upper lid I have a gap of about 8mm on two holes and it's still splash proof but not perfect. The enclosure was several times covered in wet mud, dust and debris. Inside it is 100% clean, not even dust. 


![20180413_120132|690x388](upload://9QXR3ON6X8ecuOL9EOSe39evo7B.jpg)

For demonstration, the middle one I pressed down with one finger to 1mm (no force needed), after some minutes it's 10mm again. This stuff is also perfect for cable feed-throughs. Just one square hole, all the cables side by side with a little bit distance and this sealant tape from 2 sides. The tape automatically fills all gaps.

![20180413_120607|690x388](upload://jVurRdoZhbZdaGUMcczYhZSQVyb.jpg)

I ordered mine in a german shop, they also have neoprene foam tapes and mats in different sizes.
https://www.fugendichtband24.de/HSF-Fugendichtband-600-1-4mm-13m-Rolle-grau-oder-schwarz-diverse-Breiten.htm
```

---
## \#156 Posted by: DanSkates Posted at: 2018-04-13T12:55:24.936Z Reads: 241

```
Wow that stuff is awesome! Great choice! I’ll look into that for my eSk8.

I just tried to make a few changes to my board and rounded off an Allen key so took out the trusty dremel to cut off the end but forgot to tighten the bit and nearly shot myself when the end flew off!! 😳. Remind me not to work on my board when I’m tired and have had several beers and half a bottle of wine!! 😂. Think I’ll buy a new Allen key and work on it tomorrow!!
```

---
## \#157 Posted by: rich Posted at: 2018-04-13T13:04:41.151Z Reads: 234

```
Lucky you, don't drink and work :wink:
I've tried that once, wanted to take a hub apart and forgot that there is still air in the tube.
```

---
## \#158 Posted by: DanSkates Posted at: 2018-04-13T13:06:12.378Z Reads: 243

```
Hahaha!! Yep I did the exact same thing the first time I took my drive system apart. Come to think of it I had probably been drinking then as well 😁
```

---
## \#159 Posted by: rich Posted at: 2018-04-13T19:08:39.624Z Reads: 253

```
Today I had a 10km ride on concrete and grass and got 2 flats, WTF, I'm so done with this bullshit :face_with_symbols_over_mouth::rage::face_with_symbols_over_mouth: 

![20180413_190635|690x388](upload://3wRk503W1Vh0PZIwl79oCOxaRRZ.jpg)

I'd have this green slime but also always this sentence in my head:

[quote="benjammin, post:34, topic:45377"]
Had a blowout recently from riding on bald tires. Fkn covered in green slime. Had it all the way up my back :rofl:
[/quote]

This is not something I wanna experience. 
Today I went to the riding spot by public transport, as always the people look at me like I'm an alien with my MTB. But imagine I would be covered in green slime additionally :nauseated_face: :laughing: This is the worst case without a car.

I'm still searching for some proper tire liners between tire and tube to prevent flats. The ones for bicycle are not wide enough but if I don't find proper ones I'll try it with an overlap.

But I also have some good news :grinning:
Today I bought this used armoured vest for 35€ (43usd), think that's a pretty good deal and I'm ready for some more action (my tubes not).

![20180413_202533|690x388](upload://sqORvUKx5on7wdZ7WFway9dEU04.jpg)

![20180413_202808|690x388](upload://rHRHUz33KLUNpCn84ErkPer5fya.jpg)
```

---
## \#160 Posted by: Der6FingerJo Posted at: 2018-04-13T19:14:26.873Z Reads: 244

```
Ahh the fucking tubes, time to 3d print the tires as well :grin:
```

---
## \#161 Posted by: rich Posted at: 2018-04-13T19:18:53.457Z Reads: 240

```
[quote="Der6FingerJo, post:160, topic:45377"]
fucking tubes
[/quote]


Did you just wrote fucking? 
You are so motherfucking right :rofl:
```

---
## \#162 Posted by: Der6FingerJo Posted at: 2018-04-13T19:19:34.109Z Reads: 237

```
Shit, the fucking tubes might be something else :rofl:
```

---
## \#163 Posted by: Duffman Posted at: 2018-04-13T19:26:31.874Z Reads: 247

```
Hey guys, just fill your fucking tubes with green slime... :grin:

This stuff really works and in 99,9% of all cases you only have a small hole in your tube which gets closed by this stuff before you notice it. How often did you have an exploded tube that could splash you with slime??
```

---
## \#164 Posted by: benjammin Posted at: 2018-04-13T19:35:16.715Z Reads: 250

```
![IMG_0804|666x500](upload://20ISMhXPi0Nak0Hv1NboD7AC3yV.JPG)
```

---
## \#165 Posted by: rich Posted at: 2018-04-13T19:48:39.942Z Reads: 248

```
Fuck, yeah! :metal:

[quote="Duffman, post:163, topic:45377"]
How often did you have an exploded tube that could splash you with slime??
[/quote]

That's a valid point :joy:  

Maybe I have to try it and avoid bald tires not like @benjammin, btw nice shoes hehe...  

My slime bottle is for 2 bicycle tubes, is it too much (or less) for 4x 8" tubes?
```

---
## \#166 Posted by: benjammin Posted at: 2018-04-13T19:56:18.961Z Reads: 240

```
I use one bottle for all four tires. Yeah, I won't ride on bald tires anymore. Never had a blowout like that before. Really loud, scared the shit out of me :laughing:
```

---
## \#167 Posted by: rich Posted at: 2018-04-14T15:05:10.127Z Reads: 252

```
[quote="Duffman, post:163, topic:45377"]
just fill your fucking tubes with green slime… :grin:
[/quote]

Advice taken :sunglasses:

![20180414_155156|690x388](upload://w32tjM5SxK8d6NqKnJ7bKPtJxXd.jpg)

Had some troubles with the last tube because I added to much at once, some slime bubbled on the hubs, better to add it in some steps with taking off the bottle in between. This is what I did on the first tubes to check the amount of remaining slime in the bottle according to my marks.

I just remember when I sliced one tire and tube a couple of rides ago. I hope this won't happen again otherwise I'm also a member of the "covered in green slime" club AFAIK there is only one member yet :wink:
```

---
## \#168 Posted by: ArnhemAnt Posted at: 2018-04-14T22:14:50.332Z Reads: 245

```
Been loving watching the progress of this thread - awesome work dude.

This 'green stuff' has my interest. Got any links to where I can find it? 
Yeah, I'm a lazy bastard and couldn't be bothered trolling through the net to locate the stuff myself.........
```

---
## \#169 Posted by: mmaner Posted at: 2018-04-14T23:49:46.361Z Reads: 239

```
Oregon SL11 Slime Tire Sealant 16Oz https://www.amazon.com/dp/B0086OE6P2/ref=cm_sw_r_cp_apa_joP0Ab52B71PR
```

---
## \#170 Posted by: ArnhemAnt Posted at: 2018-04-15T01:06:59.793Z Reads: 239

```
Thank you, kind sir.
```

---
## \#171 Posted by: rich Posted at: 2018-04-15T08:52:12.270Z Reads: 249

```
[quote="ArnhemAnt, post:168, topic:45377"]
Been loving watching the progress of this thread - awesome work dude.
[/quote]


Thanks dude :blush:!
My aim of this thread was always exchange of information and hints additional to the building part. About real life experience, problems and solutions. I really enjoy all this continuing discussions with you guys (btw where are the ladies?)..

Without this forum I would never know this green slime!
Thanks for the link @mmaner , love the fact that this forum has members all around the globe so while I'm sleeping you answer some questions, that's great :sunglasses:!
I bought my tire sealant in a local building supplies store (bicycle section).

Just take care that the tire sealant is for TUBES because there are also tire sealants for tubeless tires which are different but both sealants are sold as "tire sealant". And buy a tool for opening the valve. My plastic tool which was attached to the bottle broke on the 4th valve, but opening and closing the valve is simple.

Yesterday I had a very funny ride with my new body armour and the knowledge of puncture free tubes. I really abused the tires with the intention to get some flats or broken tire. Nothing happened, I think this stuff works :laughing:

I love this Armour, it is even more comfortable than my cheap ellbow pads alone. I think I'll wear it on every ride now, I feel safer and ready for some more action.

What I need are new gloves. I have Sector9 longboard sliding gloves (with some holes), unfortunately I can't attach the pucks because of the remote, maybe I try it with the left puck only because from falling I have a swollen heel of hand and with every fall it's getting worse. Does someone know some good gloves with padding on the inside?
```

---
## \#172 Posted by: benjammin Posted at: 2018-04-15T09:29:26.843Z Reads: 246

```
![IMG_0978|500x500](upload://7ghONZ6jXKuR8K8mMpLAabcDkjn.JPG)
```

---
## \#173 Posted by: ArnhemAnt Posted at: 2018-04-15T09:32:21.047Z Reads: 244

```
[quote="rich, post:171, topic:45377"]
Without this forum I would never know this green slime!
[/quote]

[quote="rich, post:171, topic:45377"]
love the fact that this forum has members all around the globe so while I’m sleeping you answer some questions, that’s great
[/quote]

Great points. I've learnt so much from this forum, and the members, and I have also 'met' some great blokes.
Without this forum, I'd still have an additional $3500.00 in my bank account.............
```

---
## \#174 Posted by: michaelcpg Posted at: 2018-04-15T09:54:34.409Z Reads: 236

```
>  I’d still have an additional $3500.00 in my bank account

Amateur.... :p
```

---
## \#175 Posted by: telnoi Posted at: 2018-04-15T09:56:19.785Z Reads: 226

```
Did those drive/hub screws of yours stay put this time? Any issues Removing them after you applied more loctite? Almost my whole drive came undone yesterday, including my motor spur/loctite 603 :sweat_smile:
```

---
## \#176 Posted by: rich Posted at: 2018-04-15T11:08:16.719Z Reads: 238

```
Looks good and the protectors inside are exactly there where I have pain, the problem ist that I couldn't hold my steez remote plus I need protection for my fingers, too. The holes in my gloves are on the finger tips only and are results from falling.

[quote="telnoi, post:175, topic:45377"]
Did those drive/hub screws of yours stay put this time?
[/quote]

Well......... no :joy:
After applying more thread locker it hold for about 2-3 rides on one side.  but as mentioned I think it is because of wobbly hubs. Right now I have to tighten the bolts each 10km, when I'm jumping each 3-5km. But actually there is almost no thread locker on the bolts because I dismounted them once, also I want to open the drivetrain soon to apply some white lithium grease for testing. After that I'll apply more thread locker on the bolts. But first I need proper 17.8mm spacers, I want to get rid of the o-rings

The bolts of the other gear holds very well with just a little bit thread locker, I'm sure the problem is my hub.

[quote="telnoi, post:175, topic:45377"]
Almost my whole drive came undone yesterday
[/quote]

Also the grub screws of the housing? Because mine hold very well and take hardcore abuse...
```

---
## \#177 Posted by: telnoi Posted at: 2018-04-15T12:10:23.922Z Reads: 225

```
[quote="rich, post:176, topic:45377"]
Also the grub screws of the housing? Because mine hold very well and take hardcore abuse…
[/quote]

Housing stays put and won't budge. Only the hub screws and spur gear. Looks like balanced tires/hubs are important. I actually checked all 4 wheels to determine the best fit. Loctite 603 may have had issues with the motor temperature... I hope not.
```

---
## \#178 Posted by: rich Posted at: 2018-04-15T12:33:35.807Z Reads: 226

```
Ah, alright. 
I don't know but all my hubs (except one) are (a bit) wobbly and I have 12 :stuck_out_tongue_winking_eye:. But also the spokes are not true and the bearings are dancing in about 50% of the spokes. It's lottery, definitely not something what I've expected when buying Trampa stuff...... I thought it's perfect.

Could it be that you put too less Loctite 603 on it? I thought that stuff is strong as hell.
```

---
## \#179 Posted by: telnoi Posted at: 2018-04-15T12:47:12.655Z Reads: 220

```
Don't know, will find out. Degreased everything & drenched both the axis and spur gear this time around. Leaving it to cure while I'm on a business trip/3 days should be enough.

Regarding the wheels. Yah, also expected near perfect balance.
```

---
## \#180 Posted by: Acido Posted at: 2018-04-15T12:52:02.743Z Reads: 219

```
kevlar is used to make bulletproof vests
```

---
## \#181 Posted by: rich Posted at: 2018-04-15T13:30:03.244Z Reads: 212

```
Yeah I hope my problems are solved with the tire sealant, time will tell. If not I'll take another look at (kevlar) tire liners.
```

---
## \#182 Posted by: benjammin Posted at: 2018-04-15T20:25:22.584Z Reads: 227

```
Gloves can be worn underneath the wrist guards (got a pair I use when it's cold with the trigger finger removed). Works fine with GT2B, but yeah grip looks different with the steez remote.
```

---
## \#183 Posted by: rich Posted at: 2018-04-15T22:41:35.942Z Reads: 245

```
Never thought about that :laughing:
BTW I hate wrist guards but I can see the advantages. I have some cheap never used, did I mention that I can't stand wrist guards? They are tight with bicycle gloves but the remote is not too far away from the normal position, a bit weird but it could work. I should give it a try. Maybe if one day my whole body is padded and armored, I'll start enjoy falling.

![20180416_000655|690x388](upload://gumj6pyB3kobscplJr65Jpi6hpw.jpg)
```

---
## \#184 Posted by: ArnhemAnt Posted at: 2018-04-16T00:02:28.011Z Reads: 238

```
For me, wrist guards are just as important as a helmet. As a teenager, whilst skateboarding, I broke both my wrists. Since that time, I always wear wrist guards when I am on a board.
```

---
## \#185 Posted by: rich Posted at: 2018-04-16T00:32:19.262Z Reads: 236

```
I think i have to transform my feelings about wrist guards into love. Broken wrists are evil! 

I've never used helmets in the past but started last year. Now I can't ride without anymore. I just realized how lucky bastard I was that I never had an accident. Also I don't feel comfortable without knee and ellbow pads anymore. The more protectors the more I enjoy riding :grin:
```

---
## \#186 Posted by: Cobber Posted at: 2018-04-16T00:46:28.454Z Reads: 237

```
[quote="rich, post:178, topic:45377"]
and the bearings are dancing in about 50% of the spokes. It’s lottery, definitely not something what I’ve expected when buying Trampa stuff…
[/quote]

Yeah I have some like that, I used some plumbers (teflon) tape to get a good press fit, not sure if it put them out of balance as I also use ceramic balance beads?

I have a extra set of brand new trampa wheels if anyone wants to buy em :rofl: ?
```

---
## \#187 Posted by: rich Posted at: 2018-04-16T01:13:41.254Z Reads: 225

```
Good hint with the tape! I don't think the balance is worse than with wiggeling bearings.

[quote="Cobber, post:186, topic:45377"]
I have a extra set of brand new trampa wheels if anyone wants to buy em :rofl: ?
[/quote]

including tape? :joy:
```

---
## \#188 Posted by: Deckoz Posted at: 2018-04-16T01:15:38.459Z Reads: 222

```
[quote="rich, post:185, topic:45377"]
The more protectors the more I enjoy riding :grin:
[/quote]

Man in an armor suite.

Makes riding fun.. not a nightmare, and worried about every move.

Also... I agree about the wrist guards..I won't wear them normally as I prefer slide gloves...but I picked up a pair for off-roading.
```

---
## \#189 Posted by: Cobber Posted at: 2018-04-16T01:22:20.020Z Reads: 215

```
yeah including tape if you like :smiley:

you don't need much, stretch it on & only once around ;)
I pressed them in with my drill press and a socket suited to the outer race.
```

---
## \#190 Posted by: benjammin Posted at: 2018-04-16T01:22:32.714Z Reads: 222

```
I won't ride without a helmet and wrist guards. I should really be using knee pads too, at the very least. Got some here I was using for awhile, but they're so shitty (for paintball I think) feels like they wouldn't stay in place if I were to fall. Gotta get some new stuff as soon as I have some more cash to throw on it.
```

---
## \#191 Posted by: rich Posted at: 2018-04-16T01:52:53.981Z Reads: 233

```
[quote="Deckoz, post:188, topic:45377"]
Makes riding fun… not a nightmare, and worried about every move
[/quote]


True, more and more I understand your love wih protectors....

Also  I'm trying to improve my jumping and sliding skills, in reality that means falling all the time :laughing: Fortunately I never fell at higher speed but most likely the day will come and then I want to be prepared best, too.

[quote="Cobber, post:189, topic:45377"]
yeah including tape if you like :smiley:
[/quote]

I have a spare set, too I'm just asking for others :grin:

[quote="benjammin, post:190, topic:45377"]
but they’re so shitty (for paintball I think) feels like they wouldn’t stay in place if I were to fall. Gotta get some new stuff as soon as I have some more cash to throw on it.
[/quote]

maybe better this than nothing :wink:
I bought my knee and shinbone protectors at a local motorbike store (Moto Cross). They were cheap, are not very comfortable but saved my knees and shins a couple of times so far. One day I'll get better ones but for now they work and my wallet is happy..
```

---
## \#192 Posted by: benjammin Posted at: 2018-04-16T02:34:43.567Z Reads: 216

```
[quote="rich, post:191, topic:45377"]
maybe better this than nothing :wink:
[/quote]

Yeah, you're probably right. Set a better example at least. Been riding way too fast to not be geared up.

Damn speed is addicting 😅
```

---
## \#193 Posted by: Deckoz Posted at: 2018-04-16T03:02:39.424Z Reads: 228

```
[quote="rich, post:191, topic:45377"]
jumping and sliding skills, in reality that means falling all the time
[/quote]

This is gonna be mostly a new world for me.. I've kiteboard on water, but having the feel strapped in completely is going to be new..and something I will have to feel out.

Also sliding,.on pneumatics on dirt..I'm sure some will transfer... But with straps it's going to be different for sure.

I ordered a
- Bell MX-9 helmet, but likely return for a Super 3R
- Leatt Knee & Shin guards
- Leatt 5.5 Body Protector
- TSG Force Wrist guards
- CG Work Gloves, I grabbed some of these in suede/back of leather, style gloves. As back of the hide does better with dirt.
A couple ripstop jerseys and MTB shorts/pants.

Little more coverage then my street gear... But shins, ribs and forearms are alot more likely to skinning. Lol
```

---
## \#194 Posted by: Nowind Posted at: 2018-04-16T12:27:06.734Z Reads: 230

```
You guys know the MBS Hillbilly ?
Integrated wristguard and nice leather.
Short fingers... kind of taste 

https://shop.elektro-skateboard.de/schutzausruestung/437/mbs-hillbilly-wrist-guard-gloves-half-finger?c=5
```

---
## \#195 Posted by: DanSkates Posted at: 2018-04-16T12:46:58.438Z Reads: 233

```
Godamn these are great @Nowind!!  I've shredded my fox gloves so need some more.  Probably time I got some wrist guards too - like @rich I think I've been lucky up till now!

I just realised that 'Hillbilly' make those awesome impact shorts too!  Think Hillbilly and MBS must have collaborated on a few things:

https://static1.squarespace.com/static/581378e659cc68fbc0f3b838/5899d21c1b10e35238fa89b9/5899d230b3db2bf74c185497/1486475825719/MBS+Hillbilly+Banner+png.png?format=300w

https://www.mbs.com/gear
```

---
## \#196 Posted by: DanSkates Posted at: 2018-04-16T12:48:56.051Z Reads: 225

```
[quote="Deckoz, post:193, topic:45377"]
This is gonna be mostly a new world for me… I’ve kiteboard on water, but having the feel strapped in completely is going to be new…and something I will have to feel out.
[/quote]

You'll love it dude!!  If anything being totally commited is way safer.

LOVE you armour shopping list!!  That is some beautiful gear there dude!
```

---
## \#197 Posted by: DanSkates Posted at: 2018-04-16T12:51:26.161Z Reads: 216

```
[quote="Duffman, post:163, topic:45377"]
Hey guys, just fill your fucking tubes with green slime… :grin:
[/quote]

Looks like I'm gonna be joining the green slime club too!!!  This thread is so fucking funny!  You guys!  Funniest shit I've EVER read!!  :joy:
```

---
## \#198 Posted by: rich Posted at: 2018-04-16T12:59:20.966Z Reads: 232

```
[quote="benjammin, post:192, topic:45377"]
Damn speed is addicting :sweat_smile:
[/quote]

So true!

[quote="Deckoz, post:193, topic:45377"]
Also sliding,.on pneumatics on dirt…I’m sure some will transfer… But with straps it’s going to be different for sure.
[/quote]

I can't really slide/drift with a longboard but with bindings and pneumatics it's a lot of fun. But it's different depending on terrain.

Your list of gear sounds as good as your list of board parts, love it!

Btw I managed to graze the tiny spot of skin between back protector and trousers last time in dirt park :roll_eyes:

[quote="Nowind, post:194, topic:45377"]
You guys know the MBS Hillbilly ?
[/quote]

Looks very nice and it's goat leather :goat:
Seems that they are easy to get them on!

[quote="DanSkates, post:197, topic:45377"]
I’m gonna be joining the green slime club too!!!
[/quote]

GSC! It's a fucking great club......
```

---
## \#199 Posted by: Deckoz Posted at: 2018-04-16T13:33:31.200Z Reads: 224

```
[quote="rich, post:198, topic:45377"]
Btw I managed to graze the tiny spot of skin between back protector and trousers last time in dirt park
[/quote]

That stinks man.. but that's why I wear a spine protector with the hllbilly hip pads..so my mid section is double coverage.

Also talking about the Hillbilly gloves.... Hillbilly used to make a MTBoard glove that was full finger leather with wrist guards, called "Heavy Dooty", unfortunately they are discontinued...so I opted for leather work gloves meant to be in the dirt. Vs traditional hide leather with slide pucks...

I need full finger coverage as I use my fingertips for my job so.....

[quote="rich, post:198, topic:45377"]
Your list of gear sounds as good as your list of board parts, love it!
[/quote]

Thanks man. I'm on the boat of skate everyday, even if I go down..or I try to skate everyday. Yea I mean I might skate 10 or 20 minutes more without the pads as I'm cooler(temp wise not looks wise)... But I won't push myself to get better as hard... And progress would be a standstill of fear of injury. 

[quote="DanSkates, post:196, topic:45377"]
You’ll love it dude!!  If anything being totally commited is way safer.
[/quote]

Hesitation is what leads to injury. I've done almost every board sport at one point. And there is one thing for certain... Commitment is success. I'm gonna ride the trampa on some bmx tracks non powered for a bit while I build the battery...
```

---
## \#200 Posted by: DanSkates Posted at: 2018-04-16T13:38:21.416Z Reads: 213

```
[quote="Deckoz, post:199, topic:45377"]
Hesitation is what leads to injury. I’ve done almost every board sport at one point. And there is one thing for certain… Commitment is success. I’m gonna ride the trampa on some bmx tracks non powered for a bit while I build the battery…
[/quote]

This is exactly what I did!  I have some vids that I've never got round to editing which I put up for amusement at some point!
```

---
## \#201 Posted by: Deckoz Posted at: 2018-04-16T14:08:57.532Z Reads: 222

```
To follow up these are the gloves I ordered...

![image|682x500](upload://ymFoCyt7onYyeB79Cxk33zQ2wlh.jpg)

https://www.amazon.com/Mechanix-Wear-Leather-M-Pact-Gloves/dp/B01EOWA1FI

because... suede/back of hide doesn't look like shit after one time in the dirt ;) plus the palms are D30 backed...
```

---
## \#202 Posted by: Cobber Posted at: 2018-04-16T14:43:34.990Z Reads: 216

```
get on some aftermarket insoles...

change your life!

i'm on these, well from my local, be somewhere close to you can get the same...

https://www.ocdskateshop.com.au/shop/safety/insoles/footprint-king-foam-jaws-mushroom-hi-insoles.html

change yo world!
```

---
## \#203 Posted by: rich Posted at: 2018-04-16T16:44:23.809Z Reads: 217

```
[quote="Deckoz, post:199, topic:45377"]
But I won’t push myself to get better as hard… And progress would be a standstill of fear of injury.
[/quote]

[quote="Deckoz, post:199, topic:45377"]
Hesitation is what leads to injury
[/quote]

Wise words....

[quote="Deckoz, post:201, topic:45377"]
plus the palms are D30 backed…
[/quote]

D30, that's the material of the video with the guys and the shovel @DanSkates posted in his thread, or? :rofl: Nice!

[quote="Cobber, post:202, topic:45377"]
get on some aftermarket insoles…
[/quote]

Good hint, when I build my spare battery probably I'll need them because of longer range.

Meanwhile I love the heelstraps but my feet always move forward so I have to reposition my feet or tighten the heelstraps all the time. Like after 3 jumps my feet move no matter how tight I have the bindings. BTW the brackets are in good position, that means no space in between feet and brackets.
Anyone has an idea what I'm doing wrong?
```

---
## \#204 Posted by: Deckoz Posted at: 2018-04-16T16:56:11.931Z Reads: 203

```
[quote="rich, post:203, topic:45377"]
D30, that’s the material
[/quote]

Yea man, g-form pads, and my spine protectors are d30... It's a form of viscous elastic polymer dough.. soft and pliable to mold to your body..and hardens on impact. Good stuff.

Loaded pushing cushion is also d30... Makes riding almost not noticable since it cushions your feet and hardens perfectly for every vibration
```

---
## \#205 Posted by: Deckoz Posted at: 2018-04-16T17:13:45.459Z Reads: 190

```
[quote="rich, post:203, topic:45377"]
what I’m doing wrong
[/quote]

You still have griptape under your feet right? Are you using a super coarse like vicious?
```

---
## \#206 Posted by: rich Posted at: 2018-04-16T18:20:55.690Z Reads: 200

```
I'm an idiot :laughing:

I couldn't understand what's wrong with the bindings but never thought about griptape. Well, I use a fine griptape because I thought it's easier to step in the bindings :joy:

Thanks for the tip, definitely I have to change it to vicious or jessup or similar super coarse griptape. I put so much love in cutting out the hexagons but this time no more hexagons....
```

---
## \#207 Posted by: Cobber Posted at: 2018-04-17T03:33:42.433Z Reads: 202

```
I won't use anything but vicious or lokton on a longboard, the lokton is bit grippier but more prone to flaking and I don't get as nice a cut around the board edge.
```

---
## \#208 Posted by: Nowind Posted at: 2018-04-18T10:16:37.249Z Reads: 206

```
[quote="DanSkates, post:195, topic:45377"]
I just realised that ‘Hillbilly’ make those awesome impact shorts too!  Think Hillbilly and MBS must have collaborated on a few things:
[/quote]

Yeah i saw the crashpants ... looking great... actually happy with my Dainese ones... but next will be the Hillbilly

@rich
The goat leather is super nice ... määääähhhh😁
```

---
## \#209 Posted by: rich Posted at: 2018-04-18T10:27:09.202Z Reads: 209

```
Määäääh bro!
They look so good and I would love to order them, the only problem is that all the goats were too small so not enough Määäääääh on the finger tips :unamused:

Ordered a dirty cheap crashpant from china yesterday :grin: better than nothing.
```

---
## \#210 Posted by: telnoi Posted at: 2018-04-18T11:53:12.786Z Reads: 213

```
![image|500x500](upload://szduE7AJgug6V0lRT6tfbi7wj8C.jpg)
need this, combined with some armor... :sweat_smile:
```

---
## \#211 Posted by: rich Posted at: 2018-04-18T12:06:39.135Z Reads: 209

```
What is that? :laughing:
```

---
## \#212 Posted by: ArnhemAnt Posted at: 2018-04-18T12:13:36.525Z Reads: 205

```
[quote="rich, post:211, topic:45377"]
What is that? :laughing:
[/quote]


Looks like a bionic skateboard knee that enables you to leap small buildings in a single ollie.
```

---
## \#213 Posted by: telnoi Posted at: 2018-04-18T12:14:35.511Z Reads: 201

```
that would prevent some nasty rotating in ways the knee should never be bent. Imagine the board spinning like a crashing car, whilst your body has less momentum...
```

---
## \#214 Posted by: rich Posted at: 2018-04-18T12:26:18.964Z Reads: 211

```
[quote="ArnhemAnt, post:212, topic:45377"]
Looks like a bionic skateboard knee that enables you to leap small buildings in a single ollie.
[/quote]

:rofl:

[quote="telnoi, post:213, topic:45377"]
that would prevent some nasty rotating in ways the knee should never be bent.
[/quote]

Loooks interesting except the hole, it's more against twisting, or does it affect the ability of bending the knees at some point?
```

---
## \#215 Posted by: telnoi Posted at: 2018-04-18T12:33:21.335Z Reads: 200

```
shouldn't, that's what I used for snowboarding in the past.
```

---
## \#216 Posted by: scrapheap Posted at: 2018-04-18T15:09:17.658Z Reads: 208

```
There's also MX knee braces. They have hard protectors over the knee caps...but they cost quite a pretty penny.
```

---
## \#217 Posted by: rich Posted at: 2018-04-18T19:34:34.398Z Reads: 222

```
I couldn't ride the last days because of work but the next days I (would) have time to ride. So today after work I wanted to go for a short pre-ride and this happened, one side crooked and damaged:

![20180418_191719|690x388](upload://dsMk7E8RR0OOV8hGaqzbFheDQtB.jpg)

![20180418_191732|690x388](upload://hVYsaE6wv10y4nsLsJk4f0XfD4L.jpg)

I lost my balance on the yellow ramp that's why I steered the board in the worst direction and crashed backward in the concrete obstacle. Furthermore it was the worst way to hit it because one wheel was beside the obstacle that's why I crashed with both motors and one housing only :face_with_symbols_over_mouth:  


![20180418_192101|690x388](upload://ebRYUOcjffzph0ShnLbyaoDQRVF.jpg)

After disassembling the whole drivetrain it looks like it survived but I'm not sure yet if the hanger or mounting plate is alright, I'll see it tomorrow when I tighten the grub screws again if there is a problem.

But for sure I killed at least 1 motor, it's totally locked and crushed. R.I.P.
The other motor has scars from the crash but seems to spin alright, will check it further before I  order new motor(s). WTF!
```

---
## \#218 Posted by: Nowind Posted at: 2018-04-18T20:29:59.420Z Reads: 217

```
And people call ME the destroyer :joy:

This will be interresting what takes the most damage ....
Here your Base/HAnger looks bad IMO : 

![7db2a8289109676c5d77e336c93e43a1d92546bb_1_690x388|690x388](upload://la3qoA9Byxyw6oe9s9I3AsoXJhB.jpg)

Not seen a bent Motormount till this day so maybe you are the first....... or it doesnt bent just out of angle from the impact.....

Contact me for help ANYTIME
```

---
## \#219 Posted by: rich Posted at: 2018-04-18T21:11:55.763Z Reads: 223

```
[quote="Nowind, post:218, topic:45377"]
And people call ME the destroyer :joy:
[/quote]


I guess I watched too much of your videos and got inspired :rofl:

[quote="Nowind, post:218, topic:45377"]
Here your Base/HAnger looks bad IMO
[/quote]

Jesus, I didn't recognize that!
After further inspection it looks like the hanger is bend and the baseplate as well.

[quote="Nowind, post:218, topic:45377"]
This will be interresting what takes the most damage …
[/quote]

It looks like everything is fucked up except your drivetrain :sunglasses: 
After loosening the grub screws and tighten them again it looks straight but have to check further.

![20180418_225132|281x500](upload://7WD43U1JvazKCvtHSO88tj4QJbj.jpg)

[quote="Nowind, post:218, topic:45377"]
Contact me for help ANYTIME
[/quote]

Thanks bro, will contact you tomorrow.
```

---
## \#220 Posted by: ArnhemAnt Posted at: 2018-04-18T22:30:48.013Z Reads: 216

```
[quote="rich, post:219, topic:45377"]
It looks like everything is fucked up except your drivetrain :sunglasses:
[/quote]


Yet another reason why I am so glad I put a E-Toxx drive system on my board. They not only look sexy as fuck, but they are tough as nails too.

Sorry to read about your crash @rich. I hope you are back up and running as quickly, and cost effectively as possible. My days just won't be the same while I wait for you to get everything back together again so you can keep posting in this thread.
```

---
## \#221 Posted by: Der6FingerJo Posted at: 2018-04-19T07:18:37.939Z Reads: 204

```
How fast were you going against that concrete block? Could not have been more than 20km/h i think? Probably less. Takes a massive amount of force to bend a whole fucking hanger i think :open_mouth:
```

---
## \#222 Posted by: telnoi Posted at: 2018-04-19T07:29:25.926Z Reads: 204

```
That sucks...good thing the drive train is ok (most expensive part). Hope you get on the road again soon.
I wonder if the infinity trucks can take more of a beating, being solid.
```

---
## \#223 Posted by: rich Posted at: 2018-04-19T08:14:26.609Z Reads: 219

```
[quote="Der6FingerJo, post:221, topic:45377"]
How fast were you going against that concrete block?
[/quote]


Maybe 10km/h (6mph), hard to say. I tried to brake but for some reason it didn't or time was too little. 

[quote="Der6FingerJo, post:221, topic:45377"]
Takes a massive amount of force to bend a whole fucking hanger i think :open_mouth:
[/quote]

And imagine the sound crushing motors in this concrete wall, this was one of the worst sounds I've ever heard.

![20180419_092837|690x388](upload://4172cVq8yRzdCz0aA5swyoUzZB2.jpg)

Right now the morning sun is shining while I disassemble half of the build instead of going for some rides, this is weird and feels like a nightmare.

![20180419_092544|690x388](upload://e0MK5MQwLD2Mwb3VMqNchDWkc3R.jpg)


[quote="telnoi, post:222, topic:45377"]
Hope you get on the road again soon.

I wonder if the infinity trucks can take more of a beating, being solid.
[/quote]

Thanks man!
I guess I order an machined Infinity hanger today, it has no holes so it must be stronger but it is heavier and not as sexy as the vertigo.
```

---
## \#224 Posted by: rich Posted at: 2018-04-19T08:29:56.835Z Reads: 214

```
[quote="ArnhemAnt, post:220, topic:45377"]
Sorry to read about your crash @rich. I hope you are back up and running as quickly, and cost effectively as possible. My days just won’t be the same while I wait for you to get everything back together again so you can keep posting in this thread.
[/quote]


Thanks for your kind words :blush:

Maybe I should start a new thread about my urban carver build which I try to finish since 14 months :joy: I want this build as daily commuter but need to finish building first, neverending story :roll_eyes:
```

---
## \#225 Posted by: telnoi Posted at: 2018-04-20T12:59:40.670Z Reads: 205

```
how are those motors performing in the spring heat by the way? My SK3 are heating up nicely now (would estimate around 50 degree C) during a hill climb. Do you have open motors you can compare them to?
```

---
## \#226 Posted by: rich Posted at: 2018-04-20T21:20:45.504Z Reads: 218

```
Can tell you exact temperature next week when my board is running again. The last rides I didn't use the phone app so I don't know the temperatures of motors and vescs. The motor has a temperature sensor so I should get some valid data.

Last year in midsummer I used open motors on this build with V4.12 and outside temperature of 35 degree C and after maybe 30 minutes I hit some temperature limits and got less power, after cooling down for 2-3 minutes it was fine again. I'm used to ride until my battery is empty without taking brakes :grin:. Unfortunately the Ackmaniac app wasn't working on new FW last year so I don't know if the motors or the vescs hit the temperature limit (the motors had temperature sensors, too).

I'm also very curious how the sealed motors will perform in midsummer and if I get heat problems. The opened motors got also hot during longer hill climbing.

Next thing:

I want to thank @okp and @Nowind for the express handling of my problem :sunglasses:! Them shipped motor and a machined Infinity Hanger today so I can ride again probably end of next week :pray: Fortunately I have a spare baseplate at home.

I just realized that all parts of my build including MTB are from UK, Germany and France, this is really perfect for quick replacement within Europe, never thought about that before but this is a massive advantage.

Got this metal bushing beauties from @Nowind, they feel very sturdy and fit perfectly, I'm sure they will survive some abuse :grin: . Thanks a million bro!

![20180420_215703|690x388](upload://lhH5nN64MElbQLFwijEd20cvJMD.jpg)
```

---
## \#227 Posted by: Deckoz Posted at: 2018-04-20T21:44:39.568Z Reads: 210

```
Nice. I asked him about those bushings. You'll have to tell me how you like them :smiley:
```

---
## \#228 Posted by: rich Posted at: 2018-04-20T21:57:53.808Z Reads: 209

```
For sure, gonna let you know my impressions next week after my first ride. I'll use  them on another build, too. I'm afraid I got the whole stock :face_with_hand_over_mouth:
```

---
## \#229 Posted by: Deckoz Posted at: 2018-04-20T21:59:33.275Z Reads: 211

```
Lol oh...that might be why haha
```

---
## \#230 Posted by: rich Posted at: 2018-04-20T22:55:05.087Z Reads: 213

```
After watching this video of @amecces I'm a bit concerned about my bolted Pelicase, it could crack one day. I think the best solution would be a segmented enclosure with 2 or 3 parts for jumping.

![Deck1|622x302](upload://cp03mVnG6OLTtkkysrc1zjFmRH1.jpg)

![Deck2|690x355](upload://cjY53fDL0bolSvvUnFoIUHyJ6X4.PNG)


https://youtu.be/i39RkWcM1VI
```

---
## \#231 Posted by: Deckoz Posted at: 2018-04-20T23:12:35.267Z Reads: 210

```
:slight_smile: segmented enclosure ;) now your talking.
```

---
## \#232 Posted by: DanSkates Posted at: 2018-04-20T23:18:51.495Z Reads: 203

```
Couldn’t agree more buddy!! I’d love to see something like the guys have been building below their decks above the deck! You’d want good cushioning under the batteries too though to protect the cells from impact. I’ve been thinking about this a lot too recently :thinking:
```

---
## \#233 Posted by: DanSkates Posted at: 2018-04-20T23:38:26.332Z Reads: 198

```
It’s be great to incorporate a BMS too for charging!
```

---
## \#234 Posted by: Deckoz Posted at: 2018-04-20T23:48:25.748Z Reads: 204

```
Eboosted and I we're talking about doing like 3 segments. 

The front and back segmented being lower and holding 18 cells each, with the front one slightly taller to hold the bms/voltage display if you wanted it. Charge port ect. And then the middle being double the height to hold 36 cells. To try to keep it evenly weighted and relatively low and sleek to fit between the bindings. 12s6p total
```

---
## \#235 Posted by: rich Posted at: 2018-04-21T00:20:42.489Z Reads: 220

```
This sounds like the perfect solution, definitely interested, too!
I would prefer to have BMS in the back segment but I guess it's mountable in both directions. Fiberglass should be the strongest solution.

Last year I did some testings with thermoforming, wanted to do a segmented ABS enclosure for Urban carver deck, but after some fails I gave up. Maybe I give it another try but this fiberglass thing seems promising.

For those who want to try vacuum thermoforming I can tell you how not to do it :laughing:

The mold was too much square-edged, should be more rounded.

![20170602_222742|690x388](upload://qgHhroZZ61bstH3US0Fsot80Mm.jpg)

I tried it with a DIY oven with a burner, an electric grill plus heatgun, it didn't work so I split the mold in two halfs and used the oven in my kitchen.

![20170601_225702|690x388](upload://joeUZDsgB76qzvpA6kWPdUjEkTI.jpg)

The second problem was to get that ABS between the gaps, it would be a lot easier with bigger gaps. 

![20170609_151852|690x388](upload://puclK7FCMxwJN9fJs5McG16oOJO.jpg)

I made a new frame and tried it with aluminium crossbars which worked but only with 1mm ABS and that's not sturdy enough. I got tired of it and had no more energy to make new molds/frames..

![20170614_154024|690x388](upload://qb1tTFmm8DrTarqLTVcsiDlCcY5.jpg)
```

---
## \#236 Posted by: amecces Posted at: 2018-04-21T01:42:46.627Z Reads: 212

```
I use only Velcro to fix the batteries (2x4s), that weighs nothing and is firm when jumping
```

---
## \#237 Posted by: Cobber Posted at: 2018-04-21T01:51:37.752Z Reads: 210

```
@DanSkates @ArnhemAnt @Deckoz

@rich got the last set of bronze bushings :( from @Nowind
I (we, Dan & Ant) spent too long waiting for the rest of my kit and missed out.
Hopefully enough people will show interest in a set to get JensoBro to tool up & make some more before too long :pray:

& Velcro lipos for the :checkered_flag:
```

---
## \#238 Posted by: ArnhemAnt Posted at: 2018-04-21T02:17:11.163Z Reads: 217

```
Yeap - I figured that @rich got greedy (LOL). All good. Happy to wait. Keen to hear the feedback from @rich on how the bushings perform.

I'm also very, very interested in the concept of a flexible enclosure above the deck as mentioned above by @Deckoz. Sounds like an awesome idea. I've only just got my enclosure from @Eboosted and haven't even got the battery pack built, but I do see the downside with the batteries being under the deck, particularly for off-road use, which is all mine will be doing.
I've got that sick feeling in the pit of my stomach as I can already feel a second, and possibly third build coming up.........
```

---
## \#239 Posted by: Eboosted Posted at: 2018-04-21T02:20:26.763Z Reads: 209

```
We need an antidote, this is a desease and we are all infected
```

---
## \#240 Posted by: rich Posted at: 2018-04-21T08:55:56.990Z Reads: 223

```
[quote="amecces, post:236, topic:45377, full:true"]
I use only Velcro to fix the batteries (2x4s), that weighs nothing and is firm when jumping
[/quote]

I bought different velcro's, too but my mind doesn't trust them but I think it's just in my head :grin: 


[quote="Cobber, post:237, topic:45377"]
@rich got the last set of bronze bushings :frowning:
[/quote]

[quote="ArnhemAnt, post:238, topic:45377"]
Yeap - I figured that @rich got greedy
[/quote]

:laughing::joy::sunglasses::kissing_heart:

This is the first time I'm happy that we live so far away from each other because I have the feeling you would like to visit and beat me up :rofl:

And sorry @Nowind, I think the picture put some pressure on you :wink: 


[quote="ArnhemAnt, post:238, topic:45377"]
I’ve only just got my enclosure from @Eboosted and haven’t even got the battery pack built, but I do see the downside with the batteries being under the deck, particularly for off-road use, which is all mine will be doing.
[/quote]

With the urban carver deck you have more ground clearance than with HolyPro so it should work if there are no big stones on your bush tracks, also the enclosure seems sturdy enough to take some hits. BTW would love to see a pic of the environment you gonna ride. 

One downside of an enclosure under the deck is that you can't swap batteries to get more range and maybe end somewhere in the bush with empty battery :smile:  If you need more stability you could upgrade your front truck with the wide hanger.

[quote="ArnhemAnt, post:238, topic:45377"]
I’ve got that sick feeling in the pit of my stomach as I can already feel a second, and possibly third build coming up…
[/quote]

Welcome to the club!

[quote="Eboosted, post:239, topic:45377, full:true"]
We need an antidote, this is a desease and we are all infected
[/quote]

My antidote is lack of money :laughing:
For all of you with enough money I don't see any chance of healing, you could try spiritual healing or quit your well-paid job to get rid of this disease......
```

---
## \#241 Posted by: ducktaperules Posted at: 2018-04-21T09:24:24.174Z Reads: 186

```
i agree with all of this. making enclosures like this is hard. since trying i have a shittone of respect for people that make good enclosures.
```

---
## \#242 Posted by: rich Posted at: 2018-04-21T09:35:41.513Z Reads: 192

```
Same here, It is even hard to make a shitty enclosure :laughing: 
Also my respect for those who are in the game!
```

---
## \#243 Posted by: ArnhemAnt Posted at: 2018-04-21T09:41:51.453Z Reads: 218

```
[quote="rich, post:240, topic:45377"]
BTW would love to see a pic of the environment you gonna ride.
[/quote]


I don't have a lot of pictures, but I do have lots of video.
This clip is of me riding my WR450 along some of the tracks. It's pretty long, and boring, but you'll get an idea of the terrain.
https://www.youtube.com/watch?v=DALNHk4NdeA&t=6s


Here's some aerial footage I got with one of my smaller UAV's. This location is not too far from 'home' and I think would be LOTs of fun with a E-MTB.
https://www.youtube.com/watch?v=f30g5Ljkl2g

Good point about the additional clearance with the Urban Carver - I had forgotten about that.

Oh, and @Eboosted, it's people like you that are contributing to our 'disease'. Stop making sexy stuff and we won't be compelled to buy it.
```

---
## \#244 Posted by: rich Posted at: 2018-04-21T10:04:28.337Z Reads: 204

```
Sick, I had no idea it looks like this!
I think the sealed direct drive is best especially in this environment, you won't get any troubles.

Man, the second video is really great looks like the perfect playground :heart_eyes:

I wish it would be closer for me than a 22 hours flight...
```

---
## \#245 Posted by: ArnhemAnt Posted at: 2018-04-21T10:11:29.984Z Reads: 204

```
Thanks man. Yep, I took some time choosing the drive unit and I have absolutely no regrets with what I have. @Nowind makes some really sexy stuff and that drive unit is perfect for where I am. Maybe a helical gear upgrade one day down the track....

If you ever get the inclination to make the 22hr flight over here, you are more than welcome to see part of my playground. There are plenty of other locations that are just as good as this one. Anyway, I sense a 'thread derail' here, so I'm best to stop.
```

---
## \#246 Posted by: DanSkates Posted at: 2018-04-21T10:15:40.583Z Reads: 201

```
Absolutely stunning area you live @ArnhemAnt!  There's some pretty hefty looking jumps there!  Love the epic crash at the end too! :crazy_face:

@rich if you did ever fancy the flight you could come visit my place in SA too and then on to @cobber on Kangeroo Island! ;-)
```

---
## \#247 Posted by: rich Posted at: 2018-04-22T12:06:00.229Z Reads: 220

```
Thanks for your invitations @ArnhemAnt and @DanSkates :sunglasses:  
I hope I will make it one day....  and if you ever come to europe you know who to call :wink:

Meanwhile I made some modifications on my board.
First I made some custom bearing spacers to say good bye o-rings :clap:
I filed down the 18,2mm spacers until they fit perfectly, each spacer is different in length and between 17,2 and 17,7mm. That was really hard work doing by hand.

![20180421_150049|690x388](upload://ijRgU06GUzt0WE41qwCP8wLWFqu.jpg)

After I finished all spacers I realized once again only one wheel is perfect. The bearings in almost all other spokes have a bit play. On the front wheels I can (must) accept it but the rear wheels should be perfect because of the drivetrain. Wanted to change one spoke in one rear hub but can't find a better one :roll_eyes:


![20180422_120228|690x388](upload://ejPcFEdMbtf59YUJr0SW2vrVFac.jpg)

The bolts of the hub adapter for wheel gear of the perfect hub never come loose, only the bolts of the hub where 1 bearing has a bit play come loose. One day I have to order more spokes.....

Then I changed the bushings on the front truck and made an aluminium spacer which should help against bending of the hanger or in worst case keep the bushings in place if they should ever brake which I doubt.

![20180422_130123|690x388](upload://643SnQRSS8WdQUM9bMoejP8Y0bc.jpg)

Put some grease on all moving parts especially because metal is rubbing on metal.

![20180422_130938|690x388](upload://nloJmNcXvGS9W58eiVKcCdXeg60.jpg)

Fits nice without rattling :sunglasses:

![20180422_131827|690x388](upload://3Q1xX64YDPo7yROr1brAiHWrMJw.jpg)
```

---
## \#248 Posted by: DanSkates Posted at: 2018-04-22T12:15:46.531Z Reads: 215

```
Beautiful work mate!!!  I have to say I've been super lazy not sorting out the play in my bearings - I'll get on that next week for sure.  Great tips!  I reckon we need to start an 'eMTB hacks' page up with all these little nuggets of gold as the tend to get lost between our various threads.

As soon as I'm back in Europe I'm coming with my board to pay yo a visit for sure!  :sunglasses:
```

---
## \#249 Posted by: rich Posted at: 2018-04-22T12:52:42.723Z Reads: 218

```
If I would have a running board now I would prefer riding and not filing spacers like a freak. This is perfect work for winter or rainy days or never. 

[quote="DanSkates, post:248, topic:45377"]
I have to say I’ve been super lazy not sorting out the play in my bearings - I’ll get on that next week for sure.
[/quote]

If you don't have troubles with the play then I'm sure there are more important things in life existing :joy:

![play|690x460](upload://uXwgyyMm1VNuiViKiphlSKLiGnM.jpg)



What I did during building was to take 8 hubs apart and combined the best parts.
```

---
## \#250 Posted by: DanSkates Posted at: 2018-04-22T13:00:46.487Z Reads: 212

```
HAHAHA! Best meme yet! 

No my bearings shift back and forth like a motherfucker. They’re pretty bad - I gotta get on that! 

Btw...I’ve reset the S.K.A.T.E trick for when you’re up and running again! 😉
```

---
## \#251 Posted by: ArnhemAnt Posted at: 2018-04-22T21:07:47.275Z Reads: 211

```
[quote="rich, post:247, topic:45377"]
First I made some custom bearing spacers to say good bye o-rings
[/quote]


Now I'm puzzled. I don't have any 'O' rings. Were these supposed to come with the trucks?
```

---
## \#252 Posted by: rich Posted at: 2018-04-22T22:29:24.802Z Reads: 214

```
The rubber o-rings are used between bearing spacer and bearing but there are different options....

![20180422_233715|690x388](upload://A9GfEmyYfyx8h4XauAQiZ19uoah.jpg)

The space between the 2 bearings on superstar hubs is about 17,3-17,9mm, due to tolerances of the hubs, spokes and bearings. If you have 16,5mm bearing spacers you should use 2mm o-rings to fill the gap.
The spacer on bottom of the pic is the former 17,8mm spacer but Trampa changed to 16,5mm spacer and o-rings last year (the spacer is still available for mini vertigo axle but not for 12mm).

The gaps on my superstar hubs for urban carver are between 17,8 and 17,9mm so I'll use the 17,8mm spacer plus kaptontape or similar to reach 17,9mm.

For my custom spacers I took the 18,2mm spacer which are used on Hypa hubs and on all ATB hangers and filed them down to desired length.

Confused now? :crazy_face:

But you know what, just measure the length of your spacers and if they are 16,5mm I can send you some o-rings by mail, I have some spares...

And if you have no time to wait maybe you can find them locally in a plumber store, for mini vertigo ID=8mm and for 12mm axle it's ID=10mm and 2mm width.

In theory I like the o-rings because they prevent rattling (which I really don't like) but in pratice it's hard to say when to stop tightening the axle nut and when you tighten it too much the o-ring gets squeezed and bigger in diameter, killed some o-rings because of this so far. And when you take off the wheel from the axle the o-ring flies away, nice in deep grass. But with my green slime I hope I won't have to take off the wheels that often.
```

---
## \#253 Posted by: ArnhemAnt Posted at: 2018-04-23T08:50:14.078Z Reads: 202

```
[quote="rich, post:252, topic:45377"]
Confused now?
[/quote]


Absolutely. 
I'm lost. I ordered the Urban Carver with the Mini trucks. There were no 'O' rings with them. When I ordered the gear drive from @Nowind, he sent me a machined hanger (which is wider than the mini). So, I have front trucks that are Mini's and rear trucks (to accommodate dual gear drive units) which are 'standard' or wider than the front. Neither of these have 'O' rings.
I think I'm going to have to go back and pull everything apart just to check spacers, tolerances, etc so I can work out a plan of attack.
From what I understand, the superstar hubs and spokes are certainly not an item that is consistent in their machining and tolerances, and this, in turn, leads to 'patches' like using 'O' rings or different sized spacers - frustrating.
```

---
## \#254 Posted by: Kug3lis Posted at: 2018-04-23T09:39:07.759Z Reads: 199

```
Wait rubber goes inside? :D
```

---
## \#255 Posted by: rich Posted at: 2018-04-23T11:36:40.506Z Reads: 217

```
I guess you use ID=12mm bearings on all wheels and additional bearing conversion spacer (to 9,525mm) on the mini hanger, right? 

http://www.trampaboards.com/9525mm-axle-bearing-conversion-spacers--c-950.html

That means you don't have spacer between the bearings for the wheels on the machined hanger because when you ordered the urban carver you had only ID=9,525mm spacers which don't fit on 12mm axle. Is that correct?

Just take one of the front wheels and measure the length of the spacer between the bearings, if it's 16,5mm you should use o-rings or longer spacer. On the rear wheels you actually have no spacer if I'm correct.

Hope you are not more confused than before :laughing:

It's possible to ride without spacers but the bearings wouldn't like it. As I mentioned the o-rings are not a bad idea to fill the gap, better than a gap but in a perfect world you can crank down the axle nut without squeezing the bearings or getting any resistance when rotating because of a perfect length spacer, this is what I did :sunglasses:

[quote="ArnhemAnt, post:253, topic:45377"]
From what I understand, the superstar hubs and spokes are certainly not an item that is consistent in their machining and tolerances, and this, in turn, leads to ‘patches’ like using ‘O’ rings or different sized spacers - frustrating.
[/quote]

True, but it's still the sexiest hub IMO :wink:
I had several skate- and longboards in my life and all spacers of the bearings were to short, i have a trauma from rattling noises. Only once I had a perfect spacer/bearing/wheel combination on my Bustin Mission with the 70mm stock wheels, I could smash the board on the ground without any noise or ride harsh terrain in silence, that was great. Then I bought orangatang kegel wheels and the rattling was back again :roll_eyes: 

As you can see I have a personal problem with rattling noises that's why custom spacers.



[quote="Kug3lis, post:254, topic:45377"]
Wait rubber goes inside? :smiley:
[/quote]

Yes if you have 16,5mm spacer :grin:

This is how I mount the wheels with o-rings, first I add the inner bearing and slide the wheel on the axle, then the 16,5mm spacer.

![20180423_114713|690x388](upload://uMmw87VLX5A2Fja4ASuuaalr9Jn.jpg)

Then I squeeze the o-ring on the axle and slide it with help of finger nails or a tool.

![20180423_114826|690x388](upload://lAqQ4zaIXTZqQoewIvXDQwM8mB8.jpg)

![20180423_115014|690x388](upload://8N2aCoQ84uu0yEr1Z6wiFaNGEfw.jpg)

Then add the second bearing, done. 

![20180423_115232|690x388](upload://w3oXoO7FSZwI1Gf2ZwgzPTTUABl.jpg)


:clap:
Yessssssss!
I just solved the problem with the wiggeling bearing during writing this post.
I inserted the bearing in the spoke and wiggeled the bearing in all directions to see where the play is, often it's only on 2 sides. Then I marked the positions on the spoke and added stripes of kapton tape (which is 0,04mm) on 2 sides of the bearing there where the play is. 

Now the play is gone and the bearing ist still easy to slide in (only in the correct position according to mark on spokes), I could add another stripe to make it pressfit if neccessary but I'm quite happy now :blush:

![20180423_131121|690x388](upload://p1ji791ag4w2lgRgCJksHdeQ8eV.jpg)

![20180423_131821|690x388](upload://jGyGmqeFGSVYqXWuesS4Yb6E0Fz.jpg)
```

---
## \#256 Posted by: banjaxxed Posted at: 2018-04-23T11:43:25.235Z Reads: 200

```
It's like Slimer from Ghostbusters yakked on your sneaker.

Does the slime have a balancing effect as well? 

Tyre changeers hate the slime although that would be in tubeless tyres, I think I know why now
```

---
## \#257 Posted by: rich Posted at: 2018-04-23T11:59:49.646Z Reads: 200

```
[quote="banjaxxed, post:256, topic:45377"]
Does the slime have a balancing effect as well?
[/quote]


Definitely, maybe not 100% but I lost the counter balance weights on one hub and when spinning fast there is almost no vibration with slime like with counter weights :sunglasses:

But it needs some turns until the green slime is evenly spreaded, on first turn the balance is horrible :laughing:
```

---
## \#258 Posted by: benjammin Posted at: 2018-04-23T14:54:19.756Z Reads: 197

```
Yeah I agree, I haven't noticed any wheel wobbles with slime.
```

---
## \#259 Posted by: rich Posted at: 2018-04-23T15:41:44.841Z Reads: 212

```
Thanks to the hints of @Nowind and @Deckoz I found the HillBilly full finger goat glove in UK, määäääh!

![hb|690x396](upload://fg5EOnvFSCJrTIjz5xb5ahPrVrw.PNG)

Also ordered the MBS F5 binding for comparison, thanks @DanSkates and  @Duffman, I'm really curious!  

![f5|690x312](upload://5kzUZyO6cur9UOO8NwSJPZPhG3f.jpg)

Finally ordered vicious griptape @Cobber :hugs:
```

---
## \#260 Posted by: Deckoz Posted at: 2018-04-23T15:42:36.362Z Reads: 201

```
Dude Link for the full fingers.


:D
```

---
## \#261 Posted by: rich Posted at: 2018-04-23T15:43:02.086Z Reads: 198

```
https://www.atbshop.co.uk/protection-and-safety/hillbilly-full-finger-wrist-guard-gloves
```

---
## \#262 Posted by: Deckoz Posted at: 2018-04-23T15:45:43.125Z Reads: 198

```
Yesssssss 

Thanks man. Haha I was ready to rock wrists under gloves, but this looks alot better. At least I got a new set of work gloves  for the garden. Haha.

PS these are the Heavy Dooty Baahd Azz gloves I thought were discontinued :D
```

---
## \#263 Posted by: rich Posted at: 2018-04-23T15:47:55.392Z Reads: 192

```
I found this gloves cheaper in US, too but can't find the link anymore, think it was ebay
```

---
## \#264 Posted by: AndyBigD Posted at: 2018-04-23T20:18:54.693Z Reads: 195

```
Can get em cheaper than that in UK;
https://www.powerkiteshop.com/accessories/hillbillywristguards.htm
£30! Just bought a pair the other day.
Great shop for tyres too, T1s & T3s @ £40 a set. Bought a total of 2 sets from here now.
And free UK shipping too!!!
```

---
## \#265 Posted by: AndyBigD Posted at: 2018-04-23T20:21:02.391Z Reads: 194

```
P.s. I also just moved over from Trampa bindings to the F5s. Hand down the most comfortable I've ever felt on my mountainboard!
```

---
## \#266 Posted by: rich Posted at: 2018-04-23T22:11:49.432Z Reads: 196

```
Very nice shop man!
They even have free shipping within europe above 60£ :crazy_face:
I paid 26£ more at the other shop.......damn!
```

---
## \#267 Posted by: ArnhemAnt Posted at: 2018-04-23T22:55:53.867Z Reads: 215

```
[quote="rich, post:255, topic:45377"]
I guess you use ID=12mm bearings on all wheels and additional bearing conversion spacer (to 9,525mm) on the mini hanger, right?
[/quote]


Yes, that is right.

[quote="rich, post:255, topic:45377"]
That means you don’t have spacer between the bearings for the wheels on the machined hanger because when you ordered the urban carver you had only ID=9,525mm spacers which don’t fit on 12mm axle. Is that correct?
[/quote]

Correct.

The Mini hanger is on the front of my board. It has the bearing conversion spacers, which I guess means that no additional spacers are required with these, yet, there still is a gap inside the hub, between each bearing.

The rear hanger, with the gear drive system (from @Nowind)  has a 12mm axle. There are no spacers between the bearings on the rear hanger. There were some small, 10mm spacers with the gear drive kit, but I figured that these go between the hub adapter and the hub so that the rear bearing does not fall into the gap.

![P4241103|624x416](upload://uXoIleLxqV73xX3UIOg5RjldQxz.JPG)
With 10mm spacer.

![P4241102|624x416](upload://ucd0VR0rd5N16a3koCRolNo7R1b.JPG)
Without 10mm spacer.

Maybe I am best to order some spacers and 'O' rings from Trampa? Yet another small, insignificant order that will incur a large postage cost.........
Although, from what I understand, the Superstar hubs have a 'spoke support spacer' which basically works like the bearing spacers. If I was cautious about not over tightening the nuts, maybe I can get away with just using the existing spoke support spacer??
```

---
## \#268 Posted by: Nowind Posted at: 2018-04-24T05:55:40.634Z Reads: 202

```
[quote="ArnhemAnt, post:267, topic:45377"]
There were some small, 10mm spacers with the gear drive kit, but I figured that these go between the hub adapter and the hub so that the rear bearing does not fall into the gap.
[/quote]


Thats right Dude!
```

---
## \#269 Posted by: DanSkates Posted at: 2018-04-24T11:46:34.037Z Reads: 201

```
Livid!!! :joy:  I have to say though that the ATBshop has some wicked stuff!!  Everytime I see it written ATB i really feel like we should be calling these boards e-ATB to get away from the whole e-mountainbike (e-MTB) thing.   AT some point we've all just gotta decide to publish stuff written that way i reckon.  They are at their very core 'all terrain boards' and not mountainboards.  You really don't need a mountain for a motorsied board - that's why we motorised them!! :smile:

That aside...I NEED ME SOME OF THOSE GLOVES!!!
```

---
## \#270 Posted by: AndyBigD Posted at: 2018-04-24T12:38:05.081Z Reads: 189

```
Totally agree! I was just saying the very same the other day; https://www.electric-skateboard.builders/t/emtb-progression/52442/7?u=andybigd
Lets start the movement!
We build e-ATBs here not e-MTBs!
```

---
## \#271 Posted by: DanSkates Posted at: 2018-04-24T12:48:53.009Z Reads: 193

```
Dude - I'm in!!!  I'll reply on your other thread properly to give it some more visibility too...
```

---
## \#272 Posted by: DanSkates Posted at: 2018-04-24T12:59:53.859Z Reads: 201

```
I'll post the same thing here I just posted on the [eMTB Progression](https://www.electric-skateboard.builders/t/emtb-progression/52442) too to increase visibility - especially as @rich's thread already contains such an amazing array of facts and information :

https://www.electric-skateboard.builders/t/semantics-emtb-is-it-a-board-or-a-bike/21887/27

Reading back through that thread I’d say that most people agree eATB or e-ATB is the most apt naming convention for these boards. It’s kinda already agreed upon anyway by the fact that mountainboarders have already been using ATB to get away from the MTB sport.

From here on in I’ll only refer to my board as eATB (or e-ATB?) and hopefully others will start to accept that term too :slight_smile:
```

---
## \#273 Posted by: DanSkates Posted at: 2018-04-24T13:03:22.600Z Reads: 199

```
eMTB:

![43|690x462](upload://4w6OzdkV0OnLjFMu6CNd3Gbx9jp.png)

eATB:

![43|690x488](upload://nSHscaxLPCCo1GdOVqIYnHwrX7B.png)

I'm pretty sure we can topple the tissue banks for their top spot!  :smile:
```

---
## \#274 Posted by: DanSkates Posted at: 2018-04-24T13:08:42.543Z Reads: 188

```
It would be pretty intersting to see how quickly we can fill up the google top searches if we spam the use of e-ATB.  Obviously we're all trapped in our own filter bubbles so searches would vary but would be interesting to see none-the-less.  Think I prefer 'e-ATB' over 'eATB' as it looks a lot less like EAT and makes the distinction clearer whilst still retaining the fact that it's an ATB.
```

---
## \#275 Posted by: AndyBigD Posted at: 2018-04-24T13:12:36.223Z Reads: 186

```
[quote="DanSkates, post:273, topic:45377"]
I’m pretty sure we can topple the tissue banks for their top spot!  :smile:
[/quote]

:rofl::rofl::rofl:
```

---
## \#276 Posted by: rich Posted at: 2018-04-24T16:03:41.973Z Reads: 203

```
[quote="ArnhemAnt, post:267, topic:45377"]
The Mini hanger is on the front of my board. It has the bearing conversion spacers, which I guess means that no additional spacers are required with these, yet, there still is a gap inside the hub, between each bearing.
[/quote]


The bearing conversion spacers just reduce the inner diameter of the bearing from 12mm to 9,525mm for the mini hanger, but this has nothing to do with the bearing support spacer in between the bearings.

There are 2 possible ways to fill the gap between the bearings on MINI truck (**9,525mm axle**):

1. With [16,5mm bearing support spacer](http://www.trampaboards.com/bearing-support-spacer-used-with-8mm-oring-on-9525mm-axles-9525-x-13525-x-165mm--lathed--p-13996.html) and ID=8mm [o-ring](http://www.trampaboards.com/rubber-orings-p-23970.html)

2. or with [17,8mm bearing support spacer](http://www.trampaboards.com/bearing-support-spacer-fits-superstar-hubs-onto-9525-axles---9525mm-x-1355mm-x-178mm--cnc-p-12174.html) without o-ring

For the rear wheels on **12mm axle** you need:

1. [16,5mm bearing support spacer](http://www.trampaboards.com/bearing-support-spacer-used-with-10mm-oring-on-12mm-axles--12-x-16-x-165mm--lathed--p-12670.html) and ID=10mm [o-ring](http://www.trampaboards.com/rubber-orings-p-23970.html)

2. Or you file down some [18,2mm spacers](http://www.trampaboards.com/bearing-support-spacer--hypa-hubs-on-12mm-axles--12-x-16-x-182mm--hypa-p-436.html) to desired length.

If it's just about 2 spacers and 4 o-rings I can send them to you by mail. If you want to order some more spare parts I would highly recommend to get at least some parts which can save you from long waiting time without riding in case you need it.


http://www.trampaboards.com/king-pin-bushings-2mm-base-for-spring-trucks-p-437.html
The difference between the four bushings is the thickness of the base. The different base sizes are 1mm, 1.5mm, 2mm and 2.5mm. Check which one you need before ordering, especially the 4 bushings on the 2 hangers usually need replacement from time to time, rear hanger more often.

http://www.trampaboards.com/spring-retainer--specially-designed-to-work-in-harmony-with-the-dampa--spring-p-467.html

I just recommend this because one of my spring retainers broke already.

Maybe I find more important things for this list and gonna edit this post, or someone else got an idea.

Also a good idea is spare tires maybe tubes (or green slime) and spare bearings.

[quote="DanSkates, post:272, topic:45377"]
From here on in I’ll only refer to my board as eATB (or e-ATB?) and hopefully others will start to accept that term too :slight_smile:
[/quote]

 I would suggest eATB (I know you already changed your youtube titles to e-ATB)
google for "e-ATB" pictures and you know why :stuck_out_tongue_winking_eye: A lot of all terrain bikes out there :joy:

But anyway, e-ATB looks better than eATB
```

---
## \#277 Posted by: ArnhemAnt Posted at: 2018-04-24T17:19:06.950Z Reads: 182

```
@rich what about the fact that the spoke spacers should act as bearing supports? Or do I still really need the other types you have recommended?
Thanks also for the parts recommendations.

@DanSkates, without getting too caught up in semantics, what about MATB? Motorised All Terrain Board.
```

---
## \#278 Posted by: rich Posted at: 2018-04-24T17:37:47.556Z Reads: 198

```
[quote="ArnhemAnt, post:277, topic:45377"]
@rich what about the fact that the spoke spacers should act as bearing supports?
[/quote]

the main problem is that too much parts are called spacers :joy:
I'm not sure what do you mean with "spoke spacer", do you mean the plastic spacer between the spokes? These are for stability of the whole hub.

The frame of the bearing gets supported and hold by the spoke itself but the inner ring amongst the balls needs support, too. The bearing support spacer sits on the axle between both bearings and bricks the gap. Without spacer you would harm your bearings if you overtighten the axle nut and the spacer is needed for axial forces as well, e.g. when carving or sliding. If you only ride straight it could work without :wink:

Don't hesitate to ask again if something is not clear, it's hard for me sometimes to explain things in english
```

---
## \#279 Posted by: ArnhemAnt Posted at: 2018-04-24T21:58:02.331Z Reads: 188

```
Perfectly explained. I'll get another order underway with Trampa...........
```

---
## \#280 Posted by: DanSkates Posted at: 2018-04-24T22:39:40.041Z Reads: 183

```
Damn I like that too!! How the hell do we choose? I’m happy to go with the flow. If only there was a manufacturer of electric mountainboards to help choose @trampa 😂

Oh wait...best not make that suggestion in case he trademarks it!! 🤣

Totally kidding Frank! 😉

...well kinda! 😂
```

---
## \#281 Posted by: DanSkates Posted at: 2018-04-24T22:41:10.032Z Reads: 174

```
Jeez I forget that English isn’t your first language - it’s better than mine!! I really need to get my head around this my board sounds very ‘clunky’ and it can’t be good for it!
```

---
## \#282 Posted by: Deckoz Posted at: 2018-04-24T23:18:08.881Z Reads: 204

```
So there's two races on a bearing.

The inner race, which rests against the axle, it is the smallest circumference ring of the bearing. If you place this onto an axle with space between them, the inner races of the two wheel bearings end up pinched when installed in a wheel without spacers after tightening.  So a metal sleeve of the same diameter of the inner race is put between the two inner races of both wheel bearings. The distance between the inner race edges on standard skate wheels is 10mm. The distance on a superstar is 17.8mm.

Here is an example of bearing spacers on an axle supporting the inner race. The bronze is the inner race support spacer, this is inside of the wheel, where you cannot see
![9a05b751b3da7122119b9c4bfcfc74887c7c973f_1_299x500|299x500](upload://n4Hq9apVguyZeginRGkI3BQTNJl.jpeg)

Then there is the outer race. This race is supported by the bearing slot in the wheel or hub. On trampa superstars there is a "plastic hub support spacer" while clamping doesn't happen here too much, the plastic spacer is to keep the spokes from flexing in, and misalligning the outer race, from the inner race... 

Hope that makes sense...
```

---
## \#283 Posted by: rich Posted at: 2018-04-24T23:47:37.199Z Reads: 203

```
[quote="DanSkates, post:281, topic:45377"]
Jeez I forget that English isn’t your first language - it’s better than mine!!
[/quote]


Well.... shame on you! :joy:
I'm really thankful @Deckoz explained it in real english and much better than me, thanks bro!

Example for the same thing (while i try to explain, Deckoz knows the vocabulary):

[quote="Deckoz, post:282, topic:45377"]
The inner race
[/quote]
[quote="rich, post:278, topic:45377"]
the inner ring amongst the balls
[/quote]
:laughing:

[quote="Deckoz, post:282, topic:45377"]
outer race
[/quote]

[quote="rich, post:278, topic:45377"]
The frame of the bearing
[/quote]
:joy:
This is too funny!

I have another hint for you guys, some weeks ago I bought Hex Plus screwdrivers from Wera especially for mounting esk8 stuff. This was one of the best investments ever! It feels so much better than standard allen keys which you can throw away after tightening 2 grub screws. With this tools the head of the screws will last much longer and won't get stripped like with standard allen keys. These babys I also carry in my backpack when riding, seems that they'll have a long and happy life :heart_eyes:

![20180425_011819|690x388](upload://6CQndGbecDjtICBZmHHCq0lj6qQ.jpg)
```

---
## \#284 Posted by: Deckoz Posted at: 2018-04-24T23:58:31.229Z Reads: 195

```
Lol.i understood yours perfectly fine man.  Both are right. Because technically it is a ring. And the race(groove where the ball rolls) is a part of that ring. Just two different ways of saying the same thing broski :) as, the ring/housing/race are all the same assembly or piece :slight_smile:
```

---
## \#285 Posted by: rich Posted at: 2018-04-25T00:09:15.580Z Reads: 193

```
If you visit a piercing studio and ask for "inner ring amongst the balls" I guess you'll get something completely different  :crazy_face:
```

---
## \#286 Posted by: ArnhemAnt Posted at: 2018-04-25T00:18:34.478Z Reads: 192

```
[quote="rich, post:285, topic:45377, full:true"]
If you visit a piercing studio and ask for “inner ring amongst the balls” I guess you’ll get something completely different
[/quote]


I sincerely hope you're not speaking from experience.
```

---
## \#287 Posted by: rich Posted at: 2018-04-25T00:24:29.168Z Reads: 186

```
I have about 50 inner rings amongst the balls and additional some rusty.
For 12mm. 9,525 and 8mm axle :laughing:
```

---
## \#288 Posted by: lrdesigns Posted at: 2018-04-25T04:14:49.748Z Reads: 200

```
[quote="rich, post:283, topic:45377"]
Hex Plus screwdrivers from Wera
[/quote]

If anyone wants the regular style, these really are the best you can get and will save some badly worn hex bolts. $35.usd

https://www.amazon.com/Wera-05073593001-Multicolor-Metric-Blacklaser/dp/B07BNJQ8XM/ref=sr_1_1?ie=UTF8&qid=1524625426&sr=8-1&keywords=wera+hex+plus
```

---
## \#289 Posted by: ArnhemAnt Posted at: 2018-04-25T04:51:59.021Z Reads: 198

```
I gotta say, if there is only one thread to read on this forum, it has got to be THIS ONE. So much info on just about every aspect of e-ATB's out there. Huge thanks to @rich for starting it, and also to all who have contributed along the way.

Lovin' this forum.
```

---
## \#290 Posted by: Der6FingerJo Posted at: 2018-04-25T05:54:03.820Z Reads: 190

```
Don't forget the excellent shitposting about fucking tubes and ball rings :smiley:

But seriously, very nice collection of information about all the small things one could easily forget about :smile:
```

---
## \#291 Posted by: ArnhemAnt Posted at: 2018-04-25T06:02:24.234Z Reads: 196

```
[quote="Der6FingerJo, post:290, topic:45377"]
Don’t forget the excellent shitposting about fucking tubes and ball rings
[/quote]


Yeap. I was trying to forget about the chatter regarding rusty balls and inner rings - sounds more like a slogan for the 'blue oyster bar' than terms used for e-ATB's.
```

---
## \#292 Posted by: telnoi Posted at: 2018-04-25T06:13:58.726Z Reads: 187

```
Also a flat tire...hopped on, noticed some unusual resistance :sweat_smile:
Have some ordinary white goo in it now...hope it holds.

Will see if the diyeboard tires fit once the rear tires are worn down. They might not be of a good composition as Trampa states, but they are made of a harder material and lasted more than 1000 km with a tire pressure of 7.5
```

---
## \#293 Posted by: Cobber Posted at: 2018-04-25T06:16:27.926Z Reads: 203

```
For hex keys I like the T-handles the best, nice balance and with the extra leverage and momentum they have you can give them a spin and screw in/out long bolts quickly. (or T-bar Allen key, what ever you want to call it)

![image|500x500](upload://i9mCgbKNd7uls3ULWmaTRctkSaR.jpg)
```

---
## \#294 Posted by: trampa Posted at: 2018-04-25T10:08:57.577Z Reads: 189

```
The spokes can still flex a bit, which is important! No flex, would make them brake and bend. In consequence the gap between the bearings is not always the same, depending on inflation pressure. This is why we feed in a rubber O-ring, allowing to adjust the bearing spacers width by carefully tightening the wheel nut down. 

Main purpose of a bearing spacer: clamping down the inner bearing race, preventing them from spinning.
Axial loads will not be picked by that spacer, since the bearings can still slide in the outer bearing housing.
```

---
## \#295 Posted by: ArnhemAnt Posted at: 2018-04-25T10:55:12.840Z Reads: 176

```
Frank, thank you for clarifying this.
```

---
## \#296 Posted by: rich Posted at: 2018-04-25T13:20:42.158Z Reads: 204

```
[quote="ArnhemAnt, post:289, topic:45377"]
I gotta say, if there is only one thread to read on this forum, it has got to be THIS ONE. So much info on just about every aspect of e-ATB’s out there. Huge thanks to @rich for starting it, and also to all who have contributed along the way.
[/quote]

Thank you so much dude but this thread (and this forum) would be nothing without all of you! You are great!


[quote="Der6FingerJo, post:290, topic:45377"]
Don’t forget the excellent shitposting about fucking tubes and ball rings :smiley:
[/quote]

True, I wonder what's next :laughing:

[quote="telnoi, post:292, topic:45377"]
Have some ordinary white goo in it now
[/quote]

What is white goo?
I had sticky goo underneath my griptape btw

[quote="trampa, post:294, topic:45377"]
In consequence the gap between the bearings is not always the same, depending on inflation pressure.
[/quote]

That's a good point.
Lucky that mine are matched to inflated tubes at 40psi :sunglasses:
If something brakes I could switch back to o-rings.

btw do you still sell 17.8mm spacer for 12mm axle because I can't find them in your shop, I guess this bearing support spacers were used before you switched to o-rings.

[quote="Cobber, post:293, topic:45377"]
For hex keys I like the T-handles the best, nice balance and with the extra leverage and momentum they have you can give them a spin and screw in/out long bolts quickly.
[/quote]

Looks great, too. This tiny ball seems fragile but I'm sure I'm wrong. With this ball you can screw the bolt from different angles or for which reason is it there?
```

---
## \#297 Posted by: trampa Posted at: 2018-04-25T13:36:57.758Z Reads: 181

```
I'm sure we still have some flying around.
```

---
## \#298 Posted by: Dyspro Posted at: 2018-04-25T14:33:45.149Z Reads: 180

```
for naming conventions you could probably also go with mATB, motorized instead of electronic.
```

---
## \#299 Posted by: telnoi Posted at: 2018-04-25T15:55:37.237Z Reads: 186

```
[quote="rich, post:296, topic:45377"]
What is white goo?

I had sticky goo underneath my griptape btw
[/quote]

The foam stuff in a pressurized can. 

Goo under your griptape?
```

---
## \#300 Posted by: rich Posted at: 2018-04-25T16:41:14.800Z Reads: 182

```
[quote="telnoi, post:299, topic:45377"]
Goo under your griptape?
[/quote]

:rofl:
I've read a thread with a title like"how to remove sticky goo from deck after removing griptape". It sounds so funny that's why I used this word.
```

---
## \#301 Posted by: Cobber Posted at: 2018-04-25T19:54:15.222Z Reads: 190

```
[quote="rich, post:296, topic:45377"]
Looks great, too. This tiny ball seems fragile but I’m sure I’m wrong. With this ball you can screw the bolt from different angles or for which reason is it there?
[/quote]

I'm yet to break one off (or round one), the smaller sizes don't have one & the width (+length) of the T-handle varies with the size and strength of the key.
```

---
## \#302 Posted by: rich Posted at: 2018-04-25T23:50:04.202Z Reads: 193

```
Jeeeesus, this Vicious is a super rough monster griptape, my feet won't slip anymore for sure :laughing: 
Maybe it's difficult to step in the bindings because of the murder grip .....

The difference looks unreal

![vicious|690x388](upload://rpxd0iQKcOZ4hpYx730JnF7rjn2.jpg)
```

---
## \#303 Posted by: Deckoz Posted at: 2018-04-25T23:53:01.442Z Reads: 191

```
Hahahaha welcome to the vicious club lol
```

---
## \#304 Posted by: TarzanHBK Posted at: 2018-04-26T08:31:51.339Z Reads: 189

```
no sitting on that board again (or buttboarding) with Vicious - it will rip yo ass off :smiley:
```

---
## \#305 Posted by: ArnhemAnt Posted at: 2018-04-26T10:19:59.083Z Reads: 199

```
[quote="TarzanHBK, post:304, topic:45377"]
no sitting on that board again (or buttboarding) with Vicious - it will rip yo ass off :smiley:
[/quote]


I reckon I'll be okay. I just received my Hillbilly Hip Pants. Just tried them on and I feel like Superman ready for a serious ass wacking.
```

---
## \#306 Posted by: rich Posted at: 2018-04-27T14:49:28.508Z Reads: 203

```
[quote="TarzanHBK, post:304, topic:45377"]
no sitting on that board again (or buttboarding) with Vicious - it will rip yo ass off :smiley:
[/quote]

Please show me a picture sitting on a mountainboard :rofl:

Finally got some parcels so I'm ready to ride again very soon.

![20180426_161042|690x388](upload://35vkM8MbWH4nU3asf2CBwmIp8vk.jpg)

![20180427_163507|690x388](upload://whXNghI8TyJeLUIvSxgvOdD4w4j.jpg)

Will update this thread later with some more info, had some unexpected troubles...
```

---
## \#307 Posted by: ArnhemAnt Posted at: 2018-04-27T19:56:05.273Z Reads: 196

```
[quote="rich, post:306, topic:45377"]
Will update this thread later with some more info, had some unexpected troubles…
[/quote]


Hope everything is okay, and that things aren't too serious.
```

---
## \#308 Posted by: rich Posted at: 2018-04-27T23:06:54.385Z Reads: 201

```
[quote="ArnhemAnt, post:307, topic:45377"]
Hope everything is okay, and that things aren’t too serious.
[/quote]

:rofl:
Thanks man, if it's serious is a matter of opinion, I have problems with the new hanger :laughing: 

![20180425_140127|690x388](upload://gtnluUYRUNVFezbZRIvGzOaIPEX.jpg)

The outer width is only 49mm, it's not possible to bridge the gap even with the thickest bushings available :weary: My other hangers are about 51.7mm and fit with 2mm bushings (my baseplates are 55.7mm).

Because I want to ride (no, I must ride) I decided to fix my broken vertigo hanger for now, will change later to a new hanger (hope to get it replaced).

On the left side the bent hanger from skate park and on the right side a 51.7mm hanger as goal for bending.

![20180426_184607|690x388](upload://9M5NtQUDryw1YQPER7ueHGBO2gd.jpg)

With help of the bolt and the long nut I bent the hanger step by step with a wrench. After the M6 bolt was done I switched to M8 bolt to apply even more force to bend the hanger more because otherwise it would be too small after removing the nut. I've expected the hanger or bolt to crack but nothing happened :crazy_face:

![20180426_214539|690x388](upload://wxpDVb1w6Kp4wK3EbrMdCYDNUia.jpg)

Now the hanger is 51.4mm and ready again.
Made a spacer for inside the hanger so it can't bend again :metal:

![20180426_235048|690x388](upload://f8HY5wsEWg5J7rFiiu8w0bioPHM.jpg)

![20180427_222424|690x388](upload://dWGoZ2W5QN11I6ZATsvmfenG1mK.jpg)

The key of the motor spur gear had some play on the shaft of the motor, I guess that's also the reason why one gear came loose once. Added 0.24mm self-adhesive insulating paper just on the part where it sits inside the keyway of the shaft, the play is gone :grin:  

![20180427_015804|690x388](upload://5gs26cpvvq1gHJ4aaVtcePhSX1V.jpg)
![20180427_015812|690x388](upload://8fh4HjzjsWUBczavFWMjVgSXiy1.jpg)

I also use washers on the shaft for 2 reasons, it's easy to mount the gear again and again (e.g. if it comes loose) at the same position as before and they also prevent any possible movement of the can. I had one motor where the slot on the shaft was too big and the circlip had play sideways. After a while the can had play, too. After bridging the gap between circlip and motor pulley with washers the play of the can was gone.

Finished mounting the direct drive, need to fix and connect the rest before I can go for a ride tomorrow :drooling_face:

Check out this sexy @Duffman spacers :heart_eyes: 

![20180427_235643|690x388](upload://sUdR1WMs7aIDETrbfMcqlVkOQS7.jpg)

https://www.e-toxx-shop.com/trampa/spacer-frontruck/
```

---
## \#309 Posted by: DanSkates Posted at: 2018-04-28T01:07:43.016Z Reads: 192

```
HUBBA HUBBA :heart_eyes:  E-TOXX +DUFFMAN

Loving the improv to get back out riding.  This is part of my problem I've never actually had all the right things at the right time to make my board perfect so It's constantly a work in progress.  But, for me, overcoming challenges and rebuilding things is all part of the journey ;-)  

How do the new straps feel btw?  I'm pretty sure you will piss your pants when you see how comfortable they are :sweat_smile:
```

---
## \#310 Posted by: rich Posted at: 2018-04-28T01:34:00.770Z Reads: 201

```
[quote="DanSkates, post:309, topic:45377"]
How do the new straps feel btw?  I’m pretty sure you will piss your pants when you see how comfortable they are :sweat_smile:
[/quote]

I haven't mounted them yet but am glad that I read your warning and will prepare a diaper.

I wanted to make it ready for ride before mounting the F5 bindings otherwise I have the bindings mounted but can't ride because it looks like this right now

![20180428_031450|690x388](upload://AngpFeCG3hbE1rbV1wYWupcvEN.jpg)

Also I'm working slowly, it's 3:30 a.m. here :crazy_face:
Think I'll sleep and finish tomorrow (today)

[quote="DanSkates, post:309, topic:45377"]
This is part of my problem I’ve never actually had all the right things at the right time to make my board perfect
[/quote]

Almost every esk8 builder could say that :laughing:
```

---
## \#311 Posted by: DanSkates Posted at: 2018-04-28T02:09:40.748Z Reads: 200

```
DUDE you're an animal!!!  Get some sleep! :rofl:  Looking forward to seeing you up and riding again.
<div style="position: absolute; width: 100%; height: 100%; left: 0px; top: 0px;"></div><div style="position: absolute; left: 50%; top: 50%;"><a id="tumblr_lightbox_right_link" href="#" style="cursor: default;"><img id="tumblr_lightbox_right_image" src="//assets.tumblr.com/images/x.gif" style="border-radius: 3px; box-shadow: rgb(0, 0, 0) 0px 4px 30px; border-width: 0px; position: absolute; display: none;"></a><a id="tumblr_lightbox_center_link" href="#" style="cursor: default;"><img id="tumblr_lightbox_center_image" src="https://78.media.tumblr.com/237bbcbd5ea275f65c3a6e6955977a5e/tumblr_o73h5wsRi81slu2yco1_500.gif" style="border-radius: 3px; box-shadow: rgb(0, 0, 0) 0px 4px 30px; border-width: 0px; position: absolute; z-index: 2147483647; display: inline-block; width: 485px; height: 399px; left: -242.5px; top: -199.5px; background-color: transparent;"></a><a id="tumblr_lightbox_left_link" href="#" style="cursor: default;"><img id="tumblr_lightbox_left_image" src="//assets.tumblr.com/images/x.gif" style="border-radius: 3px; box-shadow: rgb(0, 0, 0) 0px 4px 30px; border-width: 0px; position: absolute; display: none;"></a><div id="tumblr_lightbox_caption" style="position: absolute; text-align: center; font-style: normal; font-variant: normal; font-weight: bold; font-stretch: normal; font-size: 17px; line-height: normal; font-family: HelveticaNeue, Helvetica, Arial, sans-serif; color: rgb(255, 255, 255); padding-top: 20px; text-shadow: rgb(0, 0, 0) 0px 4px 30px; display: none; text-rendering: optimizeLegibility;"></div></div></div>
```

---
## \#312 Posted by: ArnhemAnt Posted at: 2018-04-28T10:27:09.904Z Reads: 199

```
[quote="DanSkates, post:311, topic:45377"]
DUDE you’re an animal!!!
[/quote]


And an inspiration. Well done on the work to get things back up and running again @rich. I never would have thought of doing that with the hanger. I think, instead, I would have just hit it with a hammer.
```

---
## \#313 Posted by: rich Posted at: 2018-04-28T19:06:53.269Z Reads: 208

```
Thanks bro's, this thread is also an inspiration for me :sunglasses:

Wow, had almost forgotten the feeling riding the dirt machine (and how loud it is) :laughing:
Feeling alive again and found new paths today in the city

![rebirth_2|690x388](upload://n4Nn5FeccZPF3ft3WYD8ZsJEmv9.jpg)

![rebirth_1|690x388](upload://y5ge3KzqAR4K01bqabxZSa7VJrv.jpg)

This time I wasn't lazy and added wire mesh :grin:

![rebirth_3|690x388](upload://eov5A44D2phaTk9uuPPec7UoZ8D.jpg)

The new bindings feel very good and after some time you forget about them. My back foot hurted but I think the strap was too tight, Compared to Trampa you have much more freedom and movement in the MBS bindings and it's fluffy. What I don't like is all the plastic instead of aluminium, e.g. when I open the heelstrap the whole bracket bends a lot. I hope it won't break, saw a video on youtube where someone did a backflip in skate park and on landing the binding broke :rofl:

Here a comparison of the bindings, the toes have more freedom with MBS but I don't know yet if that's good or bad. On backside turns you are more locked to the board with Trampa bindings. 

Without heelstraps the MBS give more support and it's also possile to jump. It's helpful that both sides of the strap can be adjusted in length.

![bindings|690x388](upload://prqwescq4DE5ryq25JV6Gz5WVgR.jpg)

Had the app running and got some telemetry data. Outside temperature was 26 degrees C, the vescs and motors reached about 60 degrees maximum, I was riding 20km. That looks good and means that in summer with 36 degrees outside temperature it will be about 70-75 degrees. If the vesc get too hot I can change the upper lid to get some airflow inside the enclosure if necessary.

These Hillbilly wrist guard gloves feel good and provide proper safety. The only thing the velcro straps are very short in comparison to the size of the glove. I have Large but would like the Velcro straps of XLarge. The velcro is strong, I hope it will stay good otherwise it would affect the wrist guard function.

![20180428_205504|690x388](upload://ukWOXeQnsJDAYMLRsjDhiyrowox.jpg)

I feel much safer with this heavy doodies made in U.S of A. and finally love wrist guards, won't wear normal gloves anymore. Have to get used to the different position of the remote.

![20180428_205521|690x388](upload://sSvtRenOc48GDnsAI38S89C3oTf.jpg)

My only problem right now is the nasty and stinky dog shit on both rear wheels :face_with_raised_eyebrow:
```

---
## \#314 Posted by: Der6FingerJo Posted at: 2018-04-28T19:14:31.867Z Reads: 197

```
[quote="rich, post:313, topic:45377"]
My only problem right now is the nasty and stinky dog shit on both rear wheels :face_with_raised_eyebrow:
[/quote]

Finally someone else with that problem, was afraid i'm the only one to whom that happens constantly :smiley:
Do a burnout in tall wet grass with a bit of pressure on the wheels, gets most of the shit right off :laughing:

Anyways, great you're riding again :sunglasses:
```

---
## \#315 Posted by: telnoi Posted at: 2018-04-28T19:14:42.651Z Reads: 186

```
Awesome seeing you on the road again. What tires are you rocking there?
```

---
## \#316 Posted by: rich Posted at: 2018-04-28T19:53:08.109Z Reads: 209

```
[quote="Der6FingerJo, post:314, topic:45377"]
Do a burnout in tall wet grass with a bit of pressure on the wheels, gets most of the shit right off :laughing:
[/quote]

This is exactly how i got the shit on, but it wasn't wet (or if then it was dog piss). Have the board in bathroom now to let the shit dry.

Is it allowed for dogs shitting in germany btw? :rofl:
I'm not joking, here in vienna dogs are of course allowed to shit but the owner has to grab it with a plastic bag otherwise you have to pay up to 90€ fine.

![Gackerl|690x486](upload://6gt96DOVFPr9fmOOUXjLWGsDV7y.jpg) 

"Take a bag for the shit", these signs are everywhere.

So that means I have my tires covered with illegal dog shit, shall I call police...... better not I have an illegal board.

[quote="telnoi, post:315, topic:45377"]
What tires are you rocking there?
[/quote]

Rubena V38 Diamond ordered from czech republic, one tire was 8.50€ plus shipping but I don't really recommend them. They are very thin and made for wheelchairs and only up to 20 km/h and lower pressure. They sound strange on concrete while carving and I don't trust them. The only advanage is that I really don't care about these tires and sometimes ride like there is no tomorrow. I will use them until they brake (or loose the profile to have a comparison of range). My Trampa Treads lastet about 600km, with the grey tires I have about maybe 250km or more and don't see much wear (but changed both rear tires already)

For all of you who don't listen to me :rofl:, here you could order but I won't :
http://www.delfi.cz/en/eshop/reha-programme/tyres-and-tubes/tyres/pneumatic/for-electric-wheelchairs/8/plast-rubena-200-x-50-v38-diamond-seda-241.html
The shipping was expensive and they wrapped the totally squeezed tires in plastic foil only, no parcel!!! This was the most stupid "parcel" I've ever received in my whole life.

I am on a mission to find good durable cheap tires, the Rubena was my first try.

Want to try the MBS T3 next. Also have some new Trampa Treads at home but want to keep them as spare. It's really hard to afford Trampa tires for me, 80 Pounds for 4 tires incl. shipping is too much IMO. For the same money I get 8 T3 tires with free shipping. BTW does someone has experience with T3 tires?
```

---
## \#317 Posted by: Der6FingerJo Posted at: 2018-04-28T20:12:50.856Z Reads: 206

```
[quote="rich, post:316, topic:45377"]
Is it allowed for dogs shitting in germany btw? :rofl:

I’m not joking, here in vienna dogs are of course allowed to shit but the owner has to grab it with a plastic bag otherwise you have to pay up to 90€ fine.
[/quote]

No we train them from a young age to just not shit of course :rofl:
But seriously, i'm mostly riding in way more rural areas than Vienna, so while it technically isn't allowed no one really gives a shit. Well, no one but the dogs :smiley:

[quote="rich, post:316, topic:45377"]
So that means I have my tires covered with illegal dog shit, shall I call police… better not I have an illegal board.
[/quote]

Maybe get a baby stroller and mount the tires there and then go to the police :D
```

---
## \#318 Posted by: rich Posted at: 2018-04-28T22:38:03.419Z Reads: 205

```
[quote="Der6FingerJo, post:317, topic:45377"]
no one really gives a shit Well, no one but the dogs :smiley:
[/quote]

:rofl:

[quote="Der6FingerJo, post:317, topic:45377"]
Maybe get a baby stroller and mount the tires there and then go to the police :smiley:
[/quote]

I love that idea, but motorized of course :laughing:
You talk about **ATB** = **A**ll **T**errain **B**aby stroller
I'm talking about **E-ATB**  = **E**lectric **A**ll **T**errain **B**aby stroller
Ask @DanSkates or @AndyBigD, they have E-ATB's :wink:  

I managed to record and upload the first trick of the [S.K.A.T.E. Challenge](https://www.electric-skateboard.builders/t/s-k-a-t-e-challenge-upload-your-trick-vids/52423) today

https://youtu.be/kGa8ZBwZANk
```

---
## \#319 Posted by: DanSkates Posted at: 2018-04-28T22:56:01.044Z Reads: 198

```
https://i.ytimg.com/vi/QstoNAnyNH0/maxresdefault.jpg
```

---
## \#320 Posted by: rich Posted at: 2018-04-28T22:59:52.296Z Reads: 198

```
:rofl::joy:
Great but I thought you have the All Terrain version
```

---
## \#321 Posted by: DanSkates Posted at: 2018-04-28T23:01:53.905Z Reads: 204

```
How I imagine Batman might enginner his electric baby stroller!

http://www.ohgizmo.com/wp-content/uploads/2015/02/Batmobile-baby-stroller1.jpg
```

---
## \#322 Posted by: rich Posted at: 2018-04-28T23:06:13.586Z Reads: 202

```
Tssssss, no ground clearance, I thought this **ATB** could be interesting to convert in e-ATB

![babystroller|666x500](upload://l6nWDkFUsvFpiN2HkSEG6afMFVM.jpg)
```

---
## \#323 Posted by: ArnhemAnt Posted at: 2018-04-28T23:06:38.140Z Reads: 195

```
[quote="rich, post:313, topic:45377"]
My only problem right now is the nasty and stinky dog shit on both rear wheels :face_with_raised_eyebrow:
[/quote]


I don't have to deal with stinky dog shit where I've been riding, but, I do have to deal with stinky buffalo shit.
```

---
## \#324 Posted by: rich Posted at: 2018-04-28T23:09:02.893Z Reads: 190

```
[quote="ArnhemAnt, post:323, topic:45377"]
stinky buffalo shit
[/quote]


Would love to smell that stinky buffalo shit one day, I'm tired of dog shit
```

---
## \#325 Posted by: ArnhemAnt Posted at: 2018-04-28T23:10:47.459Z Reads: 189

```
Never heard anyone ever say that they'd love to smell buffalo shit before!

I can package some up and send it over. Maybe just place it on the track over there somewhere and practice riding through it, so that when you come over here, you'll have it nailed.
```

---
## \#326 Posted by: AndyBigD Posted at: 2018-04-28T23:11:53.293Z Reads: 195

```
I'm gonna have to build one of them!!! Or a trailer for my eATB 😜 I've been debating with the wife how safe it would be to go for a ride on the eATB with my 10 month old in a carrier on my chest... Hmmmmm.......
```

---
## \#327 Posted by: DanSkates Posted at: 2018-04-28T23:19:20.846Z Reads: 200

```
I'm pretty sure I can tie all of this together in one meme:

https://pics.me.me/what-did-the-buffalo-say-to-his-son-when-he-22894204.png
```

---
## \#328 Posted by: rich Posted at: 2018-04-29T07:53:20.046Z Reads: 197

```
Please don't send me buffalo shit, I prefer to avoid any shit, just talking about some diversion :laughing:

[quote="AndyBigD, post:326, topic:45377"]
Or a trailer for my eATB :stuck_out_tongue_winking_eye:
[/quote]

Haha, that must be fun...

@DanSkates What's the difference between an bison and a buffalo? you can't wash your hands in a Buffalo.
```

---
## \#329 Posted by: Der6FingerJo Posted at: 2018-04-29T09:24:19.602Z Reads: 196

```
[quote="rich, post:328, topic:45377"]
Please don’t send me buffalo shit, I prefer to avoid any shit, just talking about some diversion :laughing:
[/quote]

Hana, back again at Shitposting (sorry) :rofl:
```

---
## \#330 Posted by: rich Posted at: 2018-04-29T22:49:02.283Z Reads: 202

```
I have some updates about the metal bushings.

@Nowind told me "Try to break them" and I have got it made today, they lasted 30km :rofl:  

![20180430_003033|690x388](upload://eqXZ77V7HC8XC632ER2c6EOUO41.jpg)

I did a jumping session in dirt park trying to increase my airtime (which I did), after some time there were strange noises coming from the rear truck and the hanger had massive play.

The metal bushings are very sturdy and I thought they will last forever. Maybe they are perfect for normal riding but definitely not for jumping. It seems that the plastic bushings have a little bit flex that's why they last longer.

Crazy shit but this was real life hardcore testing :metal:
```

---
## \#331 Posted by: DanSkates Posted at: 2018-04-30T04:24:43.900Z Reads: 191

```
WHOA!!  And I thought I knew how to destroy stuff!  Hahaha...back to plan A then!  

Well done for destroying these before he made another load for us guys in Oz - @Cobber, @ArnhemAnt - I think we dodged a bullet here! :sweat_smile:

Do you have spare plastics to get you back on the road dude?
```

---
## \#332 Posted by: ArnhemAnt Posted at: 2018-04-30T06:37:30.199Z Reads: 192

```
I wonder if there will ever be an alternative made with something like the material used in car stabiliser bar bushings? You can use rubber, but there is also another type that I think is made with urethane?
```

---
## \#333 Posted by: rich Posted at: 2018-04-30T09:52:34.562Z Reads: 195

```
[quote="DanSkates, post:331, topic:45377"]
Do you have spare plastics to get you back on the road dude?
[/quote]


Some used for now but I have to order new before I kill my next bushings :laughing:
On the front truck I'll keep the metal bushings, want to know how long they last.

[quote="ArnhemAnt, post:332, topic:45377"]
You can use rubber, but there is also another type that I think is made with urethane?
[/quote]

I think that rubber or urethane wouldn't work because it's too too soft and flexy, there is massive strain on these bushings.

I thought about this polycarbonate and nylon material which @Der6FingerJo is using for his 3D printed gears. That could take impacts I guess. Yo bro, would love to test some of these bushings if you ever try to print them :blush:
```

---
## \#334 Posted by: Der6FingerJo Posted at: 2018-04-30T10:21:18.046Z Reads: 190

```
Sure, i'll send some as soon as i printed and tested them for a bit. Unfortunately it's as always - not enough time to test everything i want so it will probably be until my bushings are bad until i try for myself.

But if you want to be a super early prototype tester we could arrange something. 
Just need the exact measurements, would be a bummer to print a lot of pieces that just don't fit in the end.
```

---
## \#335 Posted by: Kug3lis Posted at: 2018-04-30T10:21:24.366Z Reads: 189

```
There are people who uses those boards for commute and there are people who destroys shit out of them :D
```

---
## \#336 Posted by: DanSkates Posted at: 2018-04-30T10:56:42.091Z Reads: 204

```
Ok...digging up your earlier post I defo gotta do this!  I gotta the rattles and have destroyed another wheel pulley so need to tighten things up.

I'm a bit confused by the measurements of these things though:

![01|690x331](upload://qgLyvMWAHGVAXk8vA9m8scS3iaj.jpg)

I'm trying to get as close as dammit to the ones Trampa sell (in Oz), but the sizing doesn't make sense.  They say it's 10mm ID and 12mm OD and 2mm thickness (CS).  Wouldn't this make the o-ring 14mm OD (10mm+2mm+2mm)?  Or is the 2mm thickness (1mm+1mm) combined for the 12mm OD?

I've found some locally which are the same ID (10mm), but a slightly thinner CS at 1.5mm thickness so total of 13mm OD.  Would these work?  Is it important that they're a wider OD to extend past the thickness of the spacer?

[![13|485x185](upload://5hgaob1sjfmMlFjCCyBXH60c7ge.png)](https://www.ludowiciseals.com.au/search?ProductSearch=o%20rings&PageProduct=1&PageSizeProduct=24)



Or i can go with this one which is 9.25mm ID,  12.7mm OD, 1.78mm CS:

https://docs-apac.rs-online.com/webdocs/14fd/0900766b814fdeb4.pdf

RS ship quick so this would be my preference - I'll have them in a couple of days.

@ArnhemAnt kindly offered to send me a few out but as I'm sure I'll loose a shit load of these things I thought I'd stock up.  I'd prefer to stock up on the right product though!!

I'm sure I'm over thinking this!! :smile:
```

---
## \#337 Posted by: rich Posted at: 2018-04-30T14:13:00.881Z Reads: 211

```
[quote="Der6FingerJo, post:334, topic:45377"]
Sure, i’ll send some as soon as i printed and tested them for a bit. Unfortunately it’s as always - not enough time to test everything i want so it will probably be until my bushings are bad until i try for myself.
[/quote]


You are wrong :rofl:
If you print it and I test it first then you can change some details (in case I break it) and have perfect bushings for yourself when you'll need them :wink:

[quote="Kug3lis, post:335, topic:45377"]
There are people who uses those boards for commute and there are people who destroys shit out of them :smiley:
[/quote]

No way I could use this board for commuting, too big, too heavy, this is a dirt machine made for abuse.

I remember when I saw some videos of @Nowind 1-2 years ago and couldn't understand why this guy treats his board as if he wants to kill it and doesn't care about anything, or showing burnouts and drifts as if tires would be for free :laughing:

Today I fully understand why he rides that hard, because it's soooooo much fun when you just don't care about to brake something, I'm loving it.

Everything can be replaced and if you have spare parts it's not that bad. Othe people go skiing or snowboarding and pay 40-60€ for a day ticket. I could kill 4 tires or a hanger for that money and had probably an epic ride. Also it happens seldom that something brakes.

[quote="DanSkates, post:336, topic:45377"]
Ok…digging up your earlier post I defo gotta do this!  I gotta the rattles
[/quote]

Which length are your spacers? 16,5mm?

[quote="DanSkates, post:336, topic:45377"]
Wouldn’t this make the o-ring 14mm OD (10mm+2mm+2mm)?  Or is the 2mm thickness (1mm+1mm) combined for the 12mm OD?
[/quote]

You are right, I measured the Trampa 10mm o-ring, it's 14mm outside diameter.

[quote="DanSkates, post:336, topic:45377"]
I’ve found some locally which are the same ID (10mm), but a slightly thinner CS at 1.5mm thickness so total of 13mm OD.  Would these work?
[/quote]

Better than nothing but 14mm would be better. The inner ring amongst the balls has ID=12mm and OD=16mm, the o-ring should give support within this area. So a 14mm OD o-ring can extend to 16mm without rubbing on the shield of the bearing when squeezed. Exactly this happened when I tried ID=12mm and OD=16mm o-rings, 10mm ID iand OD 14mm is perfect. I would not use these 12.7mm or 13mm OD o-rings.

A little hint for those who change their bushings or dismount the hanger. Check your inner baseplate.
I realized that on one bushing on the baseplate is sticking out a bit, last time I filed it a bit down but not enough (was in a hurry) you can see it on this pic how it looked after my first filing.

![20180430_123557|690x388](upload://g75JV9bIyriw04rS5A61gNQyvFF.jpg)

That leads to problems when inserting the hanger and the bushing of the hanger will get damaged like the left one in the picture

![20180430_123112|690x388](upload://ucByyT3noMElOkq3Ff45l36bDFC.jpg)

Sanded down the bushing until it was flush with the hanger, problem solved.

![20180430_125745|690x388](upload://zy2XWHwtZX36uS05nysJMp41uPS.jpg)

Finally I added Vicious grip tape to the deck and am curious if that stops my feet from moving, guess yes. Will find out later :grin: too lazy to cut out the holes and also I want 100% grip that's why I left it like that

![20180430_160440|690x388](upload://gRTzCEo28Cb38eeiZeNszgbmjdu.jpg)

My next aim is to get rid of the big case and give velcro a try for easy battery swapping. But want to finish my daily commuter first.
```

---
## \#338 Posted by: Der6FingerJo Posted at: 2018-04-30T16:14:26.881Z Reads: 200

```
[quote="rich, post:337, topic:45377"]
You are wrong :rofl:

If you print it and I test it first then you can change some details (in case I break it) and have perfect bushings for yourself when you’ll need them :wink:
[/quote]

Yeah no problem but it would be nice to know which version of the Bushings to print. Like 1.5, 2, 2.5mm and so on. Rapid prototyping is only fun if you don't have to ship it to Austria each time for test fitting :laughing:
```

---
## \#339 Posted by: telnoi Posted at: 2018-04-30T17:31:32.971Z Reads: 200

```
Highly recommended as part of the nowind repair kit :rofl:
More loctite fixed screws getting loose, but as Jens mentions in his video tutorial, you will pull out the threaded insets if you decide to do maintenance. Fixed two today. Sure beats loosing screws and having a wobbly drive train as a result. 

![1525109394268869329955098919441|666x500](upload://jU28UuNPEoWD024wRZpcd5lLyf3.jpg)
```

---
## \#340 Posted by: rich Posted at: 2018-04-30T17:43:02.902Z Reads: 194

```
[quote="telnoi, post:339, topic:45377"]
nowind repair kit :rofl:
[/quote]

:joy::laughing:

I pray that i don't need a Nowind repair kit :pray:
But it's clever to have some spare coils
```

---
## \#341 Posted by: DanSkates Posted at: 2018-05-01T03:11:27.775Z Reads: 196

```
Thanks as always for the advice bro 😊 I thought the Trampa description had to be wrong for those so glad I checked. Coincidently I just popped into Autobarn to get a new headlight bulb and they had a case of different sized o-rings and some digital calipers soi could choose exactly what I needed! And they had the exact size so I’m good! I paid for the convenience but now I can order in a batch of cheaper ones whilst I get up and riding again! 

[quote="rich, post:337, topic:45377"]
Which length are your spacers? 16,5mm?
[/quote]

I need to check this out but I’ll need to do some filing as you did for sure! Bye bye finger prints 😂

The Vicious looks awesome! You can probably take your heelstraps off now!! 🤪
```

---
## \#342 Posted by: Keevaan Posted at: 2018-05-01T03:17:36.160Z Reads: 190

```
What is the measurement between bindings??? Thanks
```

---
## \#343 Posted by: rich Posted at: 2018-05-01T11:27:00.567Z Reads: 201

```
[quote="Der6FingerJo, post:338, topic:45377"]
Yeah no problem but it would be nice to know which version of the Bushings to print.
[/quote]

I was joking but if you take it serious I'm serious, too :grin: PM you...

[quote="DanSkates, post:341, topic:45377"]
The Vicious looks awesome! You can probably take your heelstraps off now!! :crazy_face:
[/quote]

Had a short ride yesterday and love the grip, much better :sunglasses:
I'm curious if I slip when jumping or not, hope to find out tomorrow. 

I'm confused, did you ever had o-rings before? If not then you don't have 16.5mm spacers and o-rings won't help you :joy:

[quote="Keevaan, post:342, topic:45377"]
What is the measurement between bindings???
[/quote]

Hard to say, it depends on the position of the brackets of the bindings. In my case there is about 25.5cm (10 inch) space between the brackets on the deck, 24cm would be safe, 22cm totally safe for enclosures. Between the bindings is more space but the brackets limit it.
```

---
## \#344 Posted by: DanSkates Posted at: 2018-05-01T14:09:50.927Z Reads: 197

```
[quote="rich, post:343, topic:45377"]
I’m confused, did you ever had o-rings before? If not then you don’t have 16.5mm spacers and o-rings won’t help you :joy:
[/quote]

No I never had them - but the spacers are slightly too big so the bearing doesn't fit perfectly on one side - I'm sure it's supposed too.  Also, like you the bearings don't have a tight fit.  I figured by sanding the spacers down and then using an o-ring would give me a tighter fit and the dampening of the o-ring would help with vibrations right?
```

---
## \#345 Posted by: rich Posted at: 2018-05-01T15:33:18.310Z Reads: 195

```
Ah OK, I would just file them down until they fit. If you want to go with o-rings I can send you 16.5mm spacers and o-rings by mail.

AFAIK these o-rings are only existing because of tolerances in production of hub parts and against rattling, if the spacers are too small (or in your case too big). I don't see any advantage beside this 2 reasons.
```

---
## \#346 Posted by: rich Posted at: 2018-05-02T14:21:04.630Z Reads: 205

```
I have to say I like the bindings, give you more freedom, too

![N_01i|690x387](upload://yAj4w06C4chnmi0iBAHuYTqD4pF.jpg)

This still is from my "Nollie" video for S.K.A.T.E Challenge. As you can see I always place my weight above the rear wheels, that's no nollie but I like it :grin: Finally I did real nollies to earn my letter in the end, video coming in some hours...
```

---
## \#347 Posted by: rich Posted at: 2018-05-02T21:39:08.255Z Reads: 210

```
This video contains nollie trials only in chronological order at different places :joy:
I wouldn't say I can do proper nollies but maybe sometimes  :wink:

https://youtu.be/3Zy8Ytu32Rk


This video recording is also very interesting for me to see the progress in dirt park.

3-4 weeks ago I couldn't even reach the middle of the table when jumping. Take the small hill behind me on the table as reference for comparison.

![dirtL1|690x387](upload://eRT9abAdpyD3wDRSv8vFRAY92pW.jpg)


Now I land with my rear wheels only on the table, soon I can jump above :pray: 

![dirtL2|690x387](upload://ijs2G0cw3hktqdj868aqg1BYCzl.jpg)
```

---
## \#348 Posted by: ArnhemAnt Posted at: 2018-05-02T21:47:04.337Z Reads: 193

```
Lovin' this thread and also the progress you are making man. Keep it up and keep us posted.
```

---
## \#349 Posted by: rich Posted at: 2018-05-02T21:54:24.146Z Reads: 192

```
Thanks bro!
I just realized the amazing progress of all trees in the background within a few weeks :laughing:
```

---
## \#350 Posted by: Keevaan Posted at: 2018-05-02T21:54:28.900Z Reads: 192

```
Thanks, 
Also do you have a picture of your battery with the case open?
```

---
## \#351 Posted by: ArnhemAnt Posted at: 2018-05-02T21:59:53.492Z Reads: 195

```
[quote="rich, post:349, topic:45377"]
I just realized the amazing progress of all trees in the background within a few weeks
[/quote]

Shit yeah. I did,t even notice that. wow.
```

---
## \#352 Posted by: rich Posted at: 2018-05-02T22:42:59.236Z Reads: 212

```
I use the PELI Case 1150 (Inside: 21.6 x 15.2 x 9.5 cm, outside: 24 x 19.8 x 10.9 cm)
there is also the smaller 1120 case available (Inside: 18.9 x 12.6 x 8.5 cm, outside: 21.4 x 17.2 x 9.8 cm)

but the inside measurements are made from the top, on the bottom there is about 0.7 cm less on length and width.

The case is too big for my 12s 8Ah lipo but I wanted to build a 12s5p, too. When you use cell holders then 12s5p or 10s6p is the maximum for the 1150 case.

This is how it looks now, but there is also 1cm foam below the lipo, well protected I guess, maybe too much.

![peli1|690x388](upload://2WhiCd4c68zzoPdlIHE7my5eEwC.jpg)

![peli2|690x388](upload://pUm5U7RvZJPMACG50vjfccVOsUT.jpg)


Here you see more pics of the case and battery in an [earlier post](https://www.electric-skateboard.builders/t/dirt-machine-trampa-holypro-16-ply-vertigo-trucks-superstar-hubs-unik-polaris-6374-150kv-e-toxx-black-direct-drive-vesc-6-12s/45377/4?u=rich).
```

---
## \#353 Posted by: Keevaan Posted at: 2018-05-02T22:50:05.511Z Reads: 206

```
I'm looking at building a 12s5p.  I did some math and seems as if the 60 cells won't fit in the 1150 with cell holders unless I stack them? How do recommend I arrange them to fit in the 1150?
```

---
## \#354 Posted by: rich Posted at: 2018-05-02T23:14:01.917Z Reads: 211

```
The best way is a block with 10x6 cells which is 20x12cm. You can even place a BMS on the side, easy.

![20180503_010019|690x388](upload://rOGeqEgB07neMUKixfxeeMFw8mv.jpg)

![20180503_011232|690x388](upload://t4ic5QnazXgd4pH0BYTzq7aYsmL.jpg)
```

---
## \#355 Posted by: Keevaan Posted at: 2018-05-02T23:30:42.149Z Reads: 205

```
![15253037561902520728126257787719|375x500](upload://jpWLBo3KqEDfEKwqNmOzj8P0ODL.jpg)
Great minds think alike, I was thinking of putting the BMS on the top because there should be about 2.5 cm between the top of the cells and the lid of the case.
```

---
## \#356 Posted by: rich Posted at: 2018-05-02T23:36:31.763Z Reads: 195

```
Yeah on top is easier, the bottom of the case has about 21x14.5 cm.
```

---
## \#357 Posted by: Nemesis Posted at: 2018-05-03T00:28:20.566Z Reads: 199

```
You could put the selfie stick over your shoulder now and then with the cam pointing forward to get a third person gaming style view, though it may take a few test runs to master the shot without seeing what you recording.
```

---
## \#358 Posted by: Keevaan Posted at: 2018-05-03T00:45:39.388Z Reads: 202

```
Well my cells are on their way hopefully this pack will be done in the next few weeks
```

---
## \#359 Posted by: rich Posted at: 2018-05-03T18:55:14.905Z Reads: 212

```
[quote="Nemesis, post:357, topic:45377"]
You could put the selfie stick over your shoulder now and then with the cam pointing forward to get a third person gaming style view
[/quote]

Definitely gonna try that :+1:
Maybe I find a way to attach it on the shoulder or stick it to the helmet one day to have the hands free.

Had a muddy ride today, that's why I call it Dirt Machine :laughing:

![DirtMachine_m1|690x388](upload://4ahgFFdqd3eDVnDdebW22Q9MjWD.jpg)

Also I'm very thankful for the hint with this glove/wrist guard. No more pain since I wear it. This is how they look after I've used them 3 times. No wonder that my palms were always hurting when I see the scars on the palm protectors, wicked!

![gloves|690x388](upload://xlLMTwnZx4LSe0LDkdrplEn318y.jpg)

When I finally get my crash pants then I'm fully protected, can't protect more :grin:
I never thought that but the more protectors I wear the more fun is riding for me. Last year I tried to avoid any situations where I could fall, this year I search and enjoy this situations :rofl:.
```

---
## \#360 Posted by: FredrikHems Posted at: 2018-05-03T18:59:26.798Z Reads: 199

```
Wow, that looks slippery :stuck_out_tongue_closed_eyes:

How does a 2WD board perform in these conditions? Is 4WD a must?
```

---
## \#361 Posted by: rich Posted at: 2018-05-03T19:16:58.178Z Reads: 197

```
Fortunately these muddy spots were only partially but I got stuck, the mud drags a lot. It's only slippery when doing turns. But I didn't try to ride in this conditions only but in general I like 2WD because I can drift/slide.

I think a 4WD would be very nice when climbing crazy steep hills or in real mountains, not only because of the better traction but mainly because of 4 motors, btw never tried 4WD.
```

---
## \#362 Posted by: telnoi Posted at: 2018-05-04T20:09:20.434Z Reads: 208

```
[quote="rich, post:316, topic:45377"]
For the same money I get 8 T3 tires with free shipping
[/quote]

Blew a hole in my trampa tires today. They are done after about 400 km. Temporarily installed the diyeboard 8" tires of my old board, but they are super hard in comparison and severely out of balance. Also getting some mbs tires.
```

---
## \#363 Posted by: rich Posted at: 2018-05-04T20:27:40.255Z Reads: 205

```
Shit, with a big bang?
Did you order T1 or T3 tires? T1 seems better for offroad but the T3 has much more rubber.
```

---
## \#364 Posted by: telnoi Posted at: 2018-05-06T13:14:06.550Z Reads: 209

```
Sounded allot like a rock hitting the dd. Sadly, it wasn't :sweat_smile:

T3 (seems to be the only tire offered x4 at a ~ 50 euro price range). The diyeboard 8" pattern is almost identical to T3 and noticed today that it actually handles loose sand allot better than trampa treads. It stays on course instead of loosing traction when carving.
```

---
## \#365 Posted by: rich Posted at: 2018-05-09T18:15:08.502Z Reads: 213

```
[quote="telnoi, post:362, topic:45377"]
Blew a hole in my trampa tires today
[/quote]

Blew a hole in my rubena tire today

![Bang1|690x388](upload://lQjWDjmGcPbPVIv3ICwZUmhcpFC.jpg)

![Bang3|690x388](upload://jOkLNJ5FUmbiYAZCNvgGqx3zVxO.jpg)

That was scary, rode about 35km/h when a massive wobble started followed by a big bang. I looked back and saw my tire squirting green slime during breaking. Fortunately my back wasn't covered like @benjammin when this happened to him :laughing:. My arms are hurting, it was a loooooong way back home.
```

---
## \#366 Posted by: telnoi Posted at: 2018-05-09T18:17:38.127Z Reads: 206

```
Who are you gonna call
![32-AM|540x405](upload://2tv8pxt58I3MWn6RYqrx4CaGHAr.png)
```

---
## \#367 Posted by: Der6FingerJo Posted at: 2018-05-09T20:04:41.005Z Reads: 199

```
[quote="rich, post:365, topic:45377"]
My arms are hurting, it was a loooooong way back home.
[/quote]

Dude I know that! Recently I had to carry the board only half an hour and my arm hurt the next day.
```

---
## \#368 Posted by: Kug3lis Posted at: 2018-05-09T20:30:09.897Z Reads: 195

```
Carry a tools to change front wheel with back one so you could pull the board ;) Did so many times :D
```

---
## \#369 Posted by: JonathanLau1983 Posted at: 2018-05-09T21:53:11.151Z Reads: 195

```
And maybe  a length of rope or strapping to wrap round the front trucks so you can tow it with the strap over the shoulder.
```

---
## \#370 Posted by: DanSkates Posted at: 2018-05-09T21:56:23.451Z Reads: 193

```
Dude! Your board bleeds like an alien! 

That seriously sucks. I’m clearly not riding hard enough!
```

---
## \#371 Posted by: Kug3lis Posted at: 2018-05-09T21:56:33.631Z Reads: 200

```
I always carry tool to remove motor from gear drive in case something happens with motor so at least I could ride on single motor :)
```

---
## \#372 Posted by: Kug3lis Posted at: 2018-05-09T22:56:17.156Z Reads: 203

```
Also I just about to change my tires because of usage... Too many burnouts this weekend :D

https://youtu.be/fM0FzuIhyQg
```

---
## \#373 Posted by: rich Posted at: 2018-05-09T23:25:44.136Z Reads: 210

```
[quote="Der6FingerJo, post:367, topic:45377"]
Recently I had to carry the board only half an hour and my arm hurt the next day
[/quote]


It was about half an hour for me as well but I wouldn't call it "only" :laughing:

[quote="Kug3lis, post:368, topic:45377"]
Carry a tools to change front wheel with back one so you could pull the board :wink: Did so many times :smiley:
[/quote]

I was pulling it but with the front wheels on the ground. So you don't use alien liquid? Highly recommended :grin:

I always carried my whole workshop, 2 tubes and 1 tire in my backpack for replacement in the field but since I filled that tire sealant in the tubes I had no more flats which is like a dream and I left the backpack at home.

[quote="JonathanLau1983, post:369, topic:45377, full:true"]
And maybe  a length of rope or strapping to wrap round the front trucks so you can tow it with the strap over the shoulder.
[/quote]

Sounds like a part of a survival kit for mountainboarders :joy:

[quote="DanSkates, post:370, topic:45377"]
Dude! Your board bleeds like an alien!
[/quote]

Yeah, didn't know if I shall call ghostbusters or MIB, the alien blood is still out there.

[quote="DanSkates, post:370, topic:45377"]
I’m clearly not riding hard enough!
[/quote]

I think it's my fault, the tires are rated for max. 35psi and I usually inflated the tubes to 40psi and 2 days ago I decided to feel the difference and increased to 45-50psi. I guess that was too much for this thin tires. There must have been a huge bubble in the fabric of the tire because it wobbled like hell before bursting. Glad to had that bubble because I applied almost full brake immediately, that was really weird.

[quote="Kug3lis, post:372, topic:45377"]
Also I just about to change my tires because of usage… Too many burnouts this weekend :smiley:
[/quote]

Great video, you have a very powerful RC car, how do you steer?  :rofl:
```

---
## \#374 Posted by: Kug3lis Posted at: 2018-05-09T23:27:54.487Z Reads: 204

```
On asphalt it even does donuts if I control the throttle :D
```

---
## \#375 Posted by: rich Posted at: 2018-05-09T23:34:19.945Z Reads: 209

```
If it does donuts with you standing on it you win a letter in the [S.K.A.T.E. Challenge](https://www.electric-skateboard.builders/t/s-k-a-t-e-challenge-upload-your-trick-vids/52423) :wink:

https://youtu.be/v4JwV8mlNag
```

---
## \#376 Posted by: Kug3lis Posted at: 2018-05-09T23:36:01.372Z Reads: 204

```
It does solo :D London crew saw it :D
```

---
## \#377 Posted by: banjaxxed Posted at: 2018-05-10T16:54:57.993Z Reads: 198

```
Why not carry a spare tire/tube? Could even be strapped to the deck..maybe even underneath like a car
```

---
## \#378 Posted by: telnoi Posted at: 2018-05-10T19:01:49.824Z Reads: 193

```
Installed banana flavored T3 today. They are rated for max 60 psi (all others for ~35, mbs vine for 80). They are a bit more out of balance compared to trampa treads. Reseating the tires helped resolve the worst. Maybe green soap (applied to hubs) helps when installing them.
```

---
## \#379 Posted by: rich Posted at: 2018-05-10T19:17:08.154Z Reads: 209

```
Today I carried 1 spare tube and tire and all tools but after filling it with green slime again I feel safe on short 20km rides and enjoy riding without backpack.

Switched to trampa treads and can't believe the difference, totally forgot the feeling when I used them before. They have much better traction than the rubena tires and feel really good but are unfortunately expensive. The wheelchair tires were much more comfortable, they acted as suspension because of the thin rubber, the treads at 50psi feel like wood wheels :joy:


![Treads|690x388](upload://AfWoWhlVMpTqWYJSj93bSC3HeSs.jpg)


Also removed the broken metal bushings of the front hanger which was not that easy.

![bushings|690x253](upload://bOhfqo0uvtYLHp7FP4uAwVkq9PO.jpg)


[quote="telnoi, post:378, topic:45377"]
Installed banana flavored T3 today.
[/quote]

Picture please :grin:
```

---
## \#380 Posted by: telnoi Posted at: 2018-05-11T13:17:38.633Z Reads: 209

```
[quote="rich, post:379, topic:45377"]
Picture please
[/quote]
Never mind the shrink wrap. Planning on replacing the motors. 

![15260445949075039092510122251026|666x500](upload://fSU292CsQrhwXkcvADQ8Qn8FYBf.jpg)
```

---
## \#381 Posted by: telnoi Posted at: 2018-05-11T19:47:08.272Z Reads: 204

```
And I will be another advocate for full body protection. Crashed today and body slammed into sharp stones. Big cap in my elbow/stitched , slashes across my upper body, side bruised up and there is a bit of skin missing there.

This has not deterred me though, just another lesson learned. And Thank God for my full face helmet.
```

---
## \#382 Posted by: rich Posted at: 2018-05-11T20:47:09.749Z Reads: 206

```
Shit, hope it heals quick man. 
Full body protection makes sense especially for MTB.
```

---
## \#383 Posted by: telnoi Posted at: 2018-05-13T11:15:25.853Z Reads: 203

```
Thx.What gear do you have and has any of it shifted after a crash?
```

---
## \#384 Posted by: rich Posted at: 2018-05-13T19:06:19.053Z Reads: 211

```
I had MX elbow and forearm protectors from nofear which never shifted. I switched to used O'Neal armored vest but one elbow protector shifted a bit on a sideward crash but in general it seems safe.

I use this knee and shin protectors (not very comfy but very sturdy)

https://www.louis.de/artikel/super-shield-ne-23k-knieprotektor-paar/20019224?filter_article_number=20019224&list=3c97773fd609b221a4a10ecf4123da70

and this helmet

https://www.amazon.de/axant-Line-Helmet-mountainbike-downhill/dp/B00K0L2K0M/ref=cm_cr_arp_d_product_top?ie=UTF8

and the Hillbilly heavy doodie gloves with integrated wrist guards

https://www.atbshop.co.uk/protection-and-safety/hillbilly-full-finger-wrist-guard-gloves

Also waiting for a crash pant from china.
```

---
## \#385 Posted by: rich Posted at: 2018-05-14T01:26:26.399Z Reads: 214

```
Oh lord, my front bushings broke again and also the rear ones need to be replaced very soon. I guess these bushings were made for riding not for jumping, no idea how I can solve this problem. 

![bush|690x388](upload://BdhgiiGeSV7mxkfgUnc9Rn81wo.jpg)

Last week I had some fun on a bmx track outside the town until I got banned. The problem is that it is non-public, the owner is an association and the chairman came and started yelling at me I shall fuck off. 
   
At least I recorded enough footage for a video :laughing:

It's edited but unfortunately I have audio problems which need to be solved before I can upload it, for now some stills:

![bmxV1|690x388](upload://2RZmEDbfL5UPQSGybnCIIB03803.jpg)

![bmxV2|690x388](upload://ahWbAp2bXoqs97kbyDqmVyCUL86.jpg)

![bmxV3|690x388](upload://pKGCkdZYb4wO0zIlM4OX95POHdt.jpg)

![bmxV4|690x388](upload://zrlgIfwaHP9eO3Ig07LxSNnoySq.jpg)
```

---
## \#386 Posted by: rich Posted at: 2018-05-14T18:57:10.423Z Reads: 210

```
Have a new victim :weary:

Was on bmx track and after some jumping there was suddenly resistance in one motor. Disconnected the phase wires from vesc but no difference, it seems like 2 phase wires are touching inside the motor. Never opened a motor, guess it's time for my very first time :face_with_raised_eyebrow:

![fu|690x388](upload://tKWCfnua6j7huF3q7h4dnJOB9Xh.jpg)
```

---
## \#387 Posted by: Ackmaniac Posted at: 2018-05-14T19:11:14.802Z Reads: 208

```
That track looks like fun. Where is that?
```

---
## \#388 Posted by: rich Posted at: 2018-05-14T19:33:47.484Z Reads: 202

```
It's near vienna, austria.
So if you ever visit my town we can go for an illegal ride, outlaw style :sunglasses:
```

---
## \#389 Posted by: Ackmaniac Posted at: 2018-05-14T19:38:27.325Z Reads: 195

```
Close by I also have a bike track. But by far not as nice as yours. But I should give it a try.
```

---
## \#390 Posted by: Der6FingerJo Posted at: 2018-05-14T20:10:18.030Z Reads: 205

```
[quote="rich, post:386, topic:45377"]
Was on bmx track and after some jumping there was suddenly resistance in one motor. Disconnected the phase wires from vesc but no difference, it seems like 2 phase wires are touching inside the motor. Never opened a motor, guess it’s time for my very first time :face_with_raised_eyebrow:
[/quote]

Noooooooo :frowning:

Very unfortunate, any particularly hard jumps before? I'm always putting this off, but we should probably fix the wires near the motor so they don't vibrate as much inside.
```

---
## \#391 Posted by: telnoi Posted at: 2018-05-14T21:00:08.930Z Reads: 198

```
Jumping appears to be the one weakness to break them all.
```

---
## \#392 Posted by: DavidC Posted at: 2018-05-14T21:14:09.493Z Reads: 207

```
Your new friend's named Sugru :smile:

![IMG_0454_S|375x500](upload://4qHroKh6DIwr0zG64fs5imCgE0l.jpg)
```

---
## \#393 Posted by: okp Posted at: 2018-05-15T06:09:06.696Z Reads: 198

```
hey bro, the riding photos on the BMX track are just awesome. I can imagine how much fun it was to ride this BMX track !!!
```

---
## \#394 Posted by: trampa Posted at: 2018-05-15T10:53:44.351Z Reads: 200

```
Your bushings probably brake because you tightened down the kingpin. The kingpin should be tightened to the point where any play is eliminated, but not any further.

Frank
```

---
## \#395 Posted by: Mobutusan Posted at: 2018-05-16T00:57:07.965Z Reads: 197

```
One solution might be to try MBS Matrix II trucks. Can you get your hands on a set of those? I'd be really interested to see if those can stand up to your abuse.
```

---
## \#396 Posted by: telnoi Posted at: 2018-05-16T04:31:47.982Z Reads: 197

```
Not compatible with direct drive.
```

---
## \#397 Posted by: DavidC Posted at: 2018-05-16T06:09:00.929Z Reads: 203

```
Actually there was a version of the direct drive for the Matrix2, the only problem was with the "6374"-sk3 on it, that were a bit too long :

![K800_P1010721|666x500](upload://hCiSUKFJlnaYYfT6RnGY8QHmYbD.JPG)

![K800_P1010749|666x500](upload://y1Fg7d5axg6h9UfvAjTMwWbllX0.JPG)

However correctly sized 6374 or 6364-sk3 may be ok.
```

---
## \#398 Posted by: ArnhemAnt Posted at: 2018-05-16T08:11:11.260Z Reads: 199

```
That looks like the SS Mini drive system.
```

---
## \#399 Posted by: rich Posted at: 2018-05-16T09:25:20.740Z Reads: 218

```
Thanks for your replies guys :blush:

I'm back from my 24 hours depression :laughing:

Searchd in 2 local shops but couldn't find a proper plier for the circlip to open the motor, that sucks.

[quote="Ackmaniac, post:389, topic:45377, full:true"]
Close by I also have a bike track. But by far not as nice as yours. But I should give it a try.
[/quote]

Definitely give it a try, it is so much fun. Almost every ride I spend some time at BMX track or dirt park, they are close-by but since I crushed one motor and hanger I avoid the skate park.

[quote="Der6FingerJo, post:390, topic:45377"]
Very unfortunate, any particularly hard jumps before?
[/quote]

Not really because this was not dirt park, just normal jumping. But what I did before was coasting backwards for 5-10 minutes but I don't think there's a relation.

[quote="Der6FingerJo, post:390, topic:45377"]
we should probably fix the wires near the motor so they don’t vibrate as much inside.
[/quote]

That's a good idea!
I'm curious what happened inside the motor, will see later but need this special plier first.
When I touch 2 phase wires the resistance is much higher, maybe there's just a tiny connection inside, or it's the bearings but I don't think so after this short time.

[quote="telnoi, post:391, topic:45377, full:true"]
Jumping appears to be the one weakness to break them all.
[/quote]

I think In general it's not the best for the parts.
My front hanger has play and also the rear hanger, 2 weeks ago it was OK. When I accelerate on rough terrain the rear hanger rattles. There is no visible gap but maybe I need to switch to bigger bushings, guess I have to order the complete trampa stock of bushings.

[quote="DavidC, post:392, topic:45377"]
Your new friend’s named Sugru :smile:
[/quote]

I have 7 black friends waiting for release :joy:
Your solution for the wires looks great, how did you achieve this smooth surface? Slightly wet fingers?

[quote="okp, post:393, topic:45377"]
I can imagine how much fun it was to ride this BMX track !!!
[/quote]

I love BMX tracks, are there any good in Paris?
There's one thing you did already and I have to try, riding stairs :laughing:

[quote="Mobutusan, post:395, topic:45377, full:true"]
One solution might be to try MBS Matrix II trucks. Can you get your hands on a set of those? I’d be really interested to see if those can stand up to your abuse.
[/quote]

Also thought about that and would love to try them but unfortunately as @telnoi mentioned there is actually no direct drive available. Furthermore my nick name is "rich" because of my name Richard and not because of the size of my wallet, the wallet is very thin :laughing: 

[quote="DavidC, post:397, topic:45377"]
there was a version of the direct drive for the Matrix2
[/quote]

I saw that, too but it's discontinued. If it's just about to swap the motor plates on DD I would think about it.

[quote="ArnhemAnt, post:398, topic:45377, full:true"]
That looks like the SS Mini drive system.
[/quote]

Ha, you are right! I think that was without wheel gear support bearing and these drives (including trampa mini hanger) are discontinued, am I right @Nowind? 

[quote="trampa, post:394, topic:45377"]
Your bushings probably brake because you tightened down the kingpin. The kingpin should be tightened to the point where any play is eliminated, but not any further.
[/quote]

Thanks for the hint, normally I tighten the kingpin nut only to the point where it touches the baseplate, no further tightening. The bushings which broke were used (need to order new ones soon) and when riding only they last much longer (at least 600km) and without any jumping maybe 1000km. But the higher I jump the sooner i kill bushings & more.


Yesterday I've uploaded the video of the BMX track on YouTube but are very pissed because of the video quality. I can't figure out what's the problem. I export in mp4 H.264 and the quality is good but after upload on youtube it looks awful, very poor quality, artefacts, blurring. I put so much work in this video and can't accept how it looks right now, especially when riding.

Just as example here the same still, once taken from the mp4 before upload and once from YouTube, both in HD 1080p, WTF, if someone has an idea what's wrong please tell me...

![1|690x388](upload://qLNcAY7EE69SE7Pc1Z9xlhoNeSW.jpg)
![1YT|690x387](upload://s0uLK4c12E6PvFeoiXHkg0qXbYk.jpg)
```

---
## \#400 Posted by: rich Posted at: 2018-05-16T09:26:06.299Z Reads: 213

```
Forgot to post the video :laughing:
This is the 30fps version, also uploaded it in 60fps. Personally I can't watch this video otherwise I get aggressions but you get an idea what it looks like. I try to upload a proper version ASAP and erase the earlier versions. 

https://youtu.be/S_Sc-r1jzFU
```

---
## \#401 Posted by: Manu39 Posted at: 2018-05-16T09:55:59.669Z Reads: 203

```
Very Nice vidéo,
```

---
## \#402 Posted by: Nowind Posted at: 2018-05-16T13:00:17.074Z Reads: 204

```
Yeah Dude
NiiiiceVideo
Badass Track
Sick riding
Great soundtrack
And the oskar goes to @rich

Cheers
```

---
## \#403 Posted by: TarzanHBK Posted at: 2018-05-16T14:52:54.848Z Reads: 207

```
Youtube takes a bit of time to have the full quality rendered. You only see bad quality in the first hour or so.
Do you like the current version quality wise now?

If not let me know your export software and settings and i´m gonna help you out bro ;)
```

---
## \#404 Posted by: rich Posted at: 2018-05-16T17:03:05.300Z Reads: 218

```
[quote="Nowind, post:402, topic:45377"]
And the oskar goes to @rich
[/quote]


Thanks bro, I am blessed! This is my first oscar!
Do you send it by mail?

[quote="TarzanHBK, post:403, topic:45377"]
Do you like the current version quality wise now?

If not let me know your export software and settings and i´m gonna help you out bro :wink:
[/quote]

The quality didn't change and I uploaded it yesterday. 
BTW all my videos look bad on YouTube but this one is the worst :laughing:
Thanks man for your help, will PM you :blush:

OK finally I found a shop which is selling pliers for the circlip and could open the motor. Everything looks fine to me but no way to check the cables because I would have to disassemble further, no idea how this would work, this is my first time opening a motor. The bearings seem fine.

![Motor1|690x388](upload://kSPIyv1eY1CeQVnEl6cLyFgrlL4.jpg)

So I decided to open the crushed motor as well to compare´the look of the cables and the bearings. It took some time because of stucked crushed magnet parts from the can, the shaft is also bent.

![Motor2|690x388](upload://z0ZurrcVyayeA1aorwvZv1nGSwH.jpg)

After comparing I had no idea what could be wrong and what I could do. Later I had a touch of genius, the motor part of the crushed motor looks good beside some small scratches. I took the can of the new motor combined with the old motor part and it works, already passed motor and sensor detection :grin::rofl::sunglasses:

Did you ever had or heard about such behaviour of this motor @okp?
The resistance when spinning is about double or three times as normal so when you spin it by hand it instantly stops. During free coasting the motor acts like a small brake that's how I recognized it. Also it got warmer than the other. But when I touch 2 phase wires there is really heavy resistance so I don't think it's an internal short.
```

---
## \#405 Posted by: okp Posted at: 2018-05-16T20:04:34.092Z Reads: 209

```
no but in any doubt shoot me via email the photos and I'll send you a replacement motor anytime.
```

---
## \#406 Posted by: rich Posted at: 2018-05-25T00:12:50.735Z Reads: 215

```
It's time for some updates....

Fortunately the motor works as expected so I'm back in the dirt :sunglasses:

Received the crashpants with thick foam, need no more belt on my trouser :laughing:

![crashpants|690x388](upload://fmoltu2oGWqZI16NbASGN2HUYuQ.jpg)

I was thinking about how to get faster power from the vesc, the motor max is at 65A (as the max rating) and I don't want to increase it so I need to change some other settings but I wanna stay on the safe side. What I tried is to decrease the PPM ramping time to 0.1 second.  It's not much difference to 0.3s but I like it, next time I'll try 0.01s.

![ppmRamping|327x53](upload://3Ol6sSGyAPHBSfNp1Ms3xMjLEQW.PNG)


Look at my rear tire compared to my front tire, I used them for a couple of days only :weary:

![tires|690x388](upload://gedCmExTyPeL0xhpScegztDBxFv.jpg)  

I know at least one reason why they wear down so fast.
I watched some videos of @Nowind and he inspired me to slide on loose gravel, that looked so much fun and it is for real :rofl:

https://youtu.be/IRf17kTNcwg
```

---
## \#407 Posted by: ArnhemAnt Posted at: 2018-05-27T01:13:18.861Z Reads: 209

```
Nice edit man - loved it.
```

---
## \#408 Posted by: Nowind Posted at: 2018-05-27T08:56:23.155Z Reads: 209

```
Great Video again Dude.
Loving the Music too.

Oh my eyes get wet (-;
I know how much fun it is to wear down tires this way...

Keep on drifting

"Stellst dich quer, siehste mehr"
:sunglasses:
```

---
## \#409 Posted by: DanSkates Posted at: 2018-05-27T09:06:23.766Z Reads: 213

```
😂😂😂🤙🏻

Love it bro!! You be slaying dat gravel homie!! 

Props!
```

---
## \#410 Posted by: rich Posted at: 2018-05-27T23:21:40.468Z Reads: 215

```
Thanks bro's @ArnhemAnt @Nowind @DanSkates! :blush:

Maybe it's better to slide on grass or mulch to save the tires :joy:

I swapped the front and rear tires today, it's so easy with this direct drive, much better than any belt drive. Unfortunately my front hubs wobble that's why I had to disassemble all hubs to swap the tires :confounded:. I did count the time to see how fast I can do it. Well I did a stupid mistake and forgot to release the air before, BANG, the hub and the tire popped like popcorn. I couldn't believe how big the tube is when it's inflated to 50psi, crazy!

![20180527_153347|690x388](upload://3TeUxV3rNx6v0CPo8wYtNqVaZJS.jpg)

The swapping took about 1 hour including cleaning the hubs. I recogized some dry material inside all hubs, that must be tire sealant and means I had at least 4 flats already without any consequences, I love this green slime.

My steez remote was very spooky today (need ghost busters). 2 times it locked the throttle at 50% and when I slightly attached the brake there was 100% brake, very tricky to keep balance with locked rear wheels. And last time I fell down and managed to go full throttle and lock the cruise control, fortunately I was able to lift the board wih my legs. Also almost every ride I loose connection 1-2 times, that can be dangerous.
```

---
## \#411 Posted by: TarzanHBK Posted at: 2018-05-28T07:58:25.874Z Reads: 209

```
[quote="rich, post:410, topic:45377"]
My steez remote
[/quote]
Throw that shitty thing away and use a propper 2.4ghz remote like the gt2b or the mini.
These things can cost a bone or two too fast!
```

---
## \#412 Posted by: rich Posted at: 2018-05-28T10:31:31.556Z Reads: 211

```
[quote="TarzanHBK, post:411, topic:45377"]
Throw that shitty thing away
[/quote]


:joy:
I've paid about 200€ for 2 of them, way too much to throw away... (but of course better than injuries)


I also had connection problems with the steez in my old enclosure but after changing the position of the receiver it worked flawlessly. Right now my receiver is above the power leads which is bad, maybe I could try to shield the receiver.

[quote="TarzanHBK, post:411, topic:45377"]
use a propper 2.4ghz remote like the gt2b or the mini
[/quote]

Used a GT2E but the receiver died after 2-3 weeks and it's too big IMO.
Do you mean the mini remote with finger or thumb throttle?

I have another problem but I think it has nothing to do with the remote. When I stand still and there is a small decline I slightly roll even when appplying 100% brake, that's very annoying especially when waiting to cross streets with heavy traffic, I always have to turn the board 90 degrees to avoid rolling, any ideas?
```

---
## \#413 Posted by: DeathCookies Posted at: 2018-05-28T10:36:38.364Z Reads: 197

```
[quote="rich, post:412, topic:45377"]
Used a GT2E but the receiver died after 2-3 weeks and it’s too big IMO.
[/quote]

I have a gt2e without any problems since two year. I also Moded it to become smaller and didnt even destroy anything
```

---
## \#414 Posted by: telnoi Posted at: 2018-05-28T10:45:48.853Z Reads: 191

```
also a happy gt2E user/ 1.5 years. Was using two separate receivers first, but they appear to be reliable enough. Split ppm now.
```

---
## \#415 Posted by: TarzanHBK Posted at: 2018-05-28T10:52:49.853Z Reads: 202

```
[quote="rich, post:412, topic:45377"]
Used a GT2E but the receiver died after 2-3 weeks and it’s too big IMO
[/quote]
There are pretty reliable, i think you just found a bad one :smiley: Mod it with something like the Sparkle or Mad Monkey etc.

[quote="rich, post:412, topic:45377"]
I have another problem but I think it has nothing to do with the remote. When I stand still and there is a small decline I slightly roll even when appplying 100% brake, that’s very annoying especially when waiting to cross streets with heavy traffic, I always have to turn the board 90 degrees to avoid rolling, any ideas?
[/quote]

Even with 100% brake, there is always a mini bit of rolling involved when there is a decline with vesc (my Max6 has this too). I don´t think there is a ESC out there which is able to really block a wheel 100%
```

---
## \#416 Posted by: rich Posted at: 2018-05-28T11:44:25.247Z Reads: 202

```
Ha, this is the GT2 clique, right @DeathCookies @telnoi and @TarzanHBK?
Glad to hear it works for you!

[quote="TarzanHBK, post:415, topic:45377"]
Mod it with something like the Sparkle or Mad Monkey etc.
[/quote]

Maybe in winter if my problems continue...   
Actually I try to finish my urban carver commuter which I started to build in february 2017 :joy:

[quote="TarzanHBK, post:415, topic:45377"]
Even with 100% brake, there is always a mini bit of rolling involved when there is a decline with vesc (my Max6 has this too). I don´t think there is a ESC out there which is able to really block a wheel 100%
[/quote]

Good to know so I have to live with this first world problem.
```

---
## \#417 Posted by: telnoi Posted at: 2018-05-29T08:41:29.602Z Reads: 210

```
hell yeah. It's big and clunky and I had to search for the batteries all over the place after I crashed..it actually helped me to distract myself from the hole in my arm. 
Speaking of which, have the following items in my basket. Only thing I dislike is the lack of shoulder pads...

 ![upgrade3|639x500](upload://ijajbTA6nNif56YDI5HRFLrJCMy.jpg)![upgrade2|639x500](upload://61wonYyCxbzzl78agUtEUUikTkm.jpg)![upgrade1|639x500](upload://r8UUqV6CxyCM5ccazNa10w86VBS.jpg)
```

---
## \#418 Posted by: Rookrider Posted at: 2018-05-29T13:56:17.792Z Reads: 193

```
I have the mallet IXS knee pads for mountain biking and I love them really comfortable and easy to walk in and wear for long periods of time. So I would recommend those. 

As for the second picture of those knee pads, I would not recommend those as they are quite awkward to wear and there is a little bit inside that rubbed on my knee also the connecting piece of plastic between the knee and shin guard broke very quickly so they get a thumbs down from me.

Leat is a good brand I have their neck brace and it is comfortable I don't know about their body amour. 

I would personally recommend Bliss body armour as this is very flexible and comfortable as each plate is soft but hardens on impact. Depending on how big you are I have an XS bliss body armour jacket which I could sell you it was an old one of mine which is now too small
```

---
## \#419 Posted by: telnoi Posted at: 2018-05-29T14:18:20.641Z Reads: 196

```
first picture are elbow guards :slight_smile:
Good to know the knee guards I listed break easily. I'll choose the mallet instead.

I'd need an XL body armour, otherwise I would consider your offer.
```

---
## \#420 Posted by: Rookrider Posted at: 2018-05-29T14:19:57.929Z Reads: 196

```
I would go all mallets and bliss for body armour and you will be safe as anything
```

---
## \#421 Posted by: rich Posted at: 2018-05-30T19:15:04.147Z Reads: 208

```
I see a lot of safety gear without plastic hard shells and wonder how they look after sliding on loose gravel? I can't imagine they survive when I look at all scratches on my plastic shells.

I have broken bushings on the rear hanger again :joy: 
Ordered a lot of replacement parts from trampa yesterday, hope the shipping is faster than the common 1 week.

Unfortunately I have new annoying problems since 1-2 rides, after 10-15 minutes the "hybrid" motor gets sizzling hot (really untouchable, over 85°C) while the other is just warm (about 50-60°C).

So when I accelerate, at about 50% speed there is a hard cut off (100°C) on one motor which leads to very strange "speed wobbles" of the rear truck, the same for braking. When I keep on riding the power is like zero even with full throttle maybe max. 5-10 km/h, the "cold motor" on the master vesc should deliver more power when the second motor has cut off, this is very strange.

A small hope is to change the bearings of the motor (because the can wobbles a bit) and hope I can solve the problem but it also wobbled before without overheating, no idea what's wrong, damn...

I'm also thinking about how to attach my 12V front light for night rides. I bought a step down converter but don't like to add more wires and drain the main battery so I'll use a 3s1p Li-ion (VTC5) with BMS in an enclosure plus mounted light as separate unit with velcro (hope it holds). And yes,  I solder Li-ion :grin:

![20180530_104156|690x388](upload://cFKDhKW9SSRJ32GyhlM5vBV9cMD.jpg)
```

---
## \#422 Posted by: Kug3lis Posted at: 2018-05-30T19:22:36.981Z Reads: 204

```
Get real Velcro brand velcro I have now packs witch I can't tear of without using any tools :D
```

---
## \#423 Posted by: rich Posted at: 2018-05-30T19:29:06.752Z Reads: 204

```
I'll try 3M dual lock or the wide one from hobbyking.
```

---
## \#424 Posted by: Kug3lis Posted at: 2018-05-30T19:31:06.645Z Reads: 206

```
I got this for like 5-10 pound just 1m I think

![image|500x500](upload://iXyfg8UllzvRjp47ozuK4f0J1gg.jpg)
```

---
## \#425 Posted by: rich Posted at: 2018-05-31T19:30:28.386Z Reads: 200

```
Switched to new Maytech remote just to see if this causes the heat problem, who knows. After changing the rear bushings I had a nice ride for 4 minutes until the overtemp protection kicked in. The motor is hot like lava, could boil water quickly, the other motor is not even warm after 4 minutes. I'm really desperate, no idea what's going on and can't afford new motors right now.

No more riding, no more jumping :disappointed_relieved:
```

---
## \#426 Posted by: Mobutusan Posted at: 2018-05-31T20:10:18.234Z Reads: 189

```
Have you switched wires to confirm that it's definitely the motor that's the issue? And if so, swap the motors to eliminate the drivetrain as the issue? You didn't tweak the drive gear housing or anything when you crashed?

And be careful with that dual lock stuff. The static holding power is good, but it doesn't deal with vibrations nearly as well as Velcro.
```

---
## \#427 Posted by: rich Posted at: 2018-05-31T20:39:40.215Z Reads: 203

```
I haven't switched wires or vescs yet (because I didn't change anything on my whole setup before), I think it's the motor but I should try this option, too.

[quote="Mobutusan, post:426, topic:45377"]
You didn’t tweak the drive gear housing or anything when you crashed?
[/quote]

Hehe, yes I did but that's a different story.

I try to explain it quick, it's a bit complicated :laughing::
There is Motor A, B & C. Motor A & B was my first setup then I crashed and killed Motor A. Fortunately @okp sent me Motor C to replace Motor A. 14 days ago Motor B broke (acting as a brake, resistance when spinning but not shorted). After that I combined the can and shaft from Motor B with the motor part of Motor A (from the crash). The can has a slight wobble on the motor part (I guess the bearings should be replaced) but it worked without problems for some rides but suddenly it is cooking within a few minutes. Because there were no heat problems in the beginning I don't think the bearings are the problem but I can try to change them.

Confused now? :crazy_face:

[quote="Mobutusan, post:426, topic:45377"]
And be careful with that dual lock stuff. The static holding power is good, but it doesn’t deal with vibrations nearly as well as Velcro.
[/quote]

Thanks for the hint, then I use velcro.
```

---
## \#428 Posted by: telnoi Posted at: 2018-05-31T20:55:17.102Z Reads: 194

```
[quote="rich, post:421, topic:45377"]
I see a lot of safety gear without plastic hard shells and wonder how they look after sliding on loose gravel? I can’t imagine they survive when I look at all scratches on my plastic shells.
[/quote]

At this point I'd rather have a hole in my armor than my arm, legs, torso. Recovery time is predicted to be another month.

Get your point though, but for some reason my clothing including flimsy t-shirt is almost fine, while the flesh underneath was torn apart and scarred. Fabric can apparently take a fair amount or abuse.
```

---
## \#429 Posted by: rich Posted at: 2018-06-04T22:16:58.735Z Reads: 185

```
@okp  saved my ass again and is sending me a replacement motor :heart_eyes:
I'm really super happy with the shop and service, amazing!

https://www.unikboards.com/

Just another example:
When I ordered my motors and bindings from Unikboards it was a Sunday. 
On the same day I got an e-mail asking me if it's correct because I ordered 2 motors and only 1 sensor adapter cable or if I need 2. I was stunned and impressed, very smart plus on a weekend!   

In general I can only recommend to support and buy from reliable shops which is win-win for all.
```

---
## \#430 Posted by: banjaxxed Posted at: 2018-06-05T10:51:10.446Z Reads: 185

```
Sort out your remote dude, it sounds like it's planning to kill you...maybe you have a loose wire? :face_with_monocle::joy:
```

---
## \#431 Posted by: rich Posted at: 2018-06-05T13:17:03.894Z Reads: 209

```
[quote="banjaxxed, post:430, topic:45377"]
:face_with_monocle:
[/quote]


:rofl: 

I did :face_with_monocle: but nothing loose. I changed the position of the receiver a bit, that could help.

But meanwhile I think it's not a connection problem, wanted to change the frequency that's why I read the manual again. I found a very scary function which is exactly the whole issue! The steez remote has a thumb throttle with integrated cruise control fuction. When you push the throttle down you lock the actual speed.

**Warning for Steez remote users:**
When you push the thumb throttle down while coasting (throttle in middle position) the remote enters pairing mode and you loose any control! After pressing the thumb throttle again the connection is back.

I mostly loose connection when jumping on bmx tracks, now all makes sense. Because while jumping and landing I dont accelerate and it's not hard to push down the thumb control unintentionally on landing. But now I know that a simple click brings back the control which is great compared to shutting the remote off and on which takes at least 8-10 seconds.

I really like the steez, also have the new Maytech but the control is completely different, needs throttle and brake curve adjustments, the steez not. But the throttle on the new one is much better protected when falling and it's smaller and cheaper, only thing I miss is the leash for the wrist.

![133117|690x388](upload://2zPScP8Y0lquFvlw7b0zBlhCozn.jpg)

@Nowind sent me new toys (also big up @Duffman) to play, I'm a big child :laughing:
A swiss army knife aka Bull Bars and some drive guards.

The bull bars are supposed as motor protectors, but are also nice on the front truck as protected camera holder (no tilting on turns!!!) or for massive offroad lights or as a handle or as motor protection plus pulling a trailer, or you could mount a bad ass rear light, too ..........

Definitely this Bull Bars would have saved my motor from crushing when I hit the wall backwards in skate park. 

![192549|690x388](upload://o3p1hHYdxuFqXBPy61uZGygY9UY.jpg)

![BullBars|690x388](upload://ttDVIIwqKIdj3Jjq4FzqBi4Uuqs.jpg)

These drive guards are well printed, they hold without screws :laughing:

![174455|690x388](upload://cizMQVrebN1bv6ILJ7M0ZIOgUVC.jpg)

Before mounting I have to buy shorter screws or if I'm lazy use some washers.

![175007|690x388](upload://2f0DzNETdngk8JY46CQUN51loHY.jpg)

I guess I'll touch stones or curbs more often because of less ground clearance but the drive is well protected. Looking forward to see what impacts they can take.
```

---
## \#432 Posted by: JonathanLau1983 Posted at: 2018-06-05T15:03:38.892Z Reads: 194

```
What are the drive guards printed in? TPU would be a good idea, it'll absorb the impact and I think it'll be more durable than hard plastics.
```

---
## \#433 Posted by: Duffman Posted at: 2018-06-05T15:06:00.607Z Reads: 192

```
Glad you like it! Your crashes, smashes, fails and scratches were the reason to build these things.

The DriveGuards you got are from the first material testing prototype runs and made of PETG. The series DriveGuards are printed in TPU and hopefully indestructible. Check out how well they hold up and everytime you kill them, you get the next stronger evolution step until everything is bulletproof. :sunglasses:
```

---
## \#434 Posted by: rich Posted at: 2018-06-05T15:18:45.340Z Reads: 193

```
:joy::joy::rofl:
Thanks, feel honored bro :blush:

[quote="Duffman, post:433, topic:45377"]
Check out how well they hold up and everytime you kill them, you get the next stronger evolution step until everything is bulletproof. :sunglasses:
[/quote]

Hehe great offer man! Let you know if I kill them and also if not :stuck_out_tongue_winking_eye:
```

---
## \#435 Posted by: telnoi Posted at: 2018-06-06T09:34:46.719Z Reads: 199

```
Any chance of getting the file for printing? I've already destroyed/bent a DD side panel and will be avoiding certain terrain because the direct drive does not have enough ground clearance (for where I ride anyway).


I would modify it and extend it to cover the full length of the drive. The weakest part is actually the Side panel. The rest is cosmetic damage so far.

![side%20panel|666x500](upload://pXNTroSMfUhKBju7Q5C3If5uJc8.jpg)
```

---
## \#436 Posted by: rich Posted at: 2018-06-06T10:28:18.104Z Reads: 200

```
Man that really sucks! :roll_eyes:
Any idea why this happened exactly? Looks like sabotage :sweat_smile:.
```

---
## \#437 Posted by: telnoi Posted at: 2018-06-06T10:30:38.595Z Reads: 200

```
Just a stone in the wrong place at the wrong time. It must have been wedged in between the wheel and the direct drive. All I heard was a dull clunk like I hear it so often (you can tell by the cratered POM enclosure).

What you typically find here are stones that come from mines (blast rubble, sharp edged). These are used to strengthen the roads for forest/wood cutting heavy machinery.
```

---
## \#438 Posted by: Der6FingerJo Posted at: 2018-06-06T13:04:56.325Z Reads: 192

```
Just to contribute some findings - the gears of my inner gear drive are printed from Taulman Alloy 910 and they have pretty much the same ground cleareance as the gearbox of the DD so they already hit a lot of stuff like curbs from sidewalks or just bigger stones. So far the material holds up great, there is no (permanent) deformation or visible scratches on the surface. If for some reason TPU doesn't hold up in the long run i think some kind of Taulman Nylon blend would be the way to go.
```

---
## \#439 Posted by: neverpush Posted at: 2018-06-06T17:34:57.420Z Reads: 189

```
Same. @Nowind, can we get the .stl for the guard?
```

---
## \#440 Posted by: rich Posted at: 2018-06-15T21:27:54.351Z Reads: 192

```
Since about 2 weeks I couldn't ride my board but looking forward to ride again probably next weekend thanks to @okp, you rock bro! Actually my board looks like this:

![003505|690x388](upload://6fTzW6hbLsBvYKBEnZ9P85UNXgx.jpg)

Meanwhile I had some time to buy high top shoes, I always have troubles with moving heelstraps with normal skate shoes. Also maybe I can jump higher with this Batman shoes :rofl: They were drty cheap on sale, it was so funny in the shop, they had these shoes only in adults sizes. Nobody except me was interested but almost all little kids passing by were screaming "Baaatmaaaan shoooes!". 

![204252|690x388](upload://a8E9Z6VhplfTFrWkAI0kuzF4w7H.jpg)
```

---
## \#441 Posted by: ArnhemAnt Posted at: 2018-06-15T22:17:08.571Z Reads: 190

```
"Quick Robin.......to the dirt machine"
```

---
## \#442 Posted by: rich Posted at: 2018-06-15T22:44:42.272Z Reads: 200

```
There is no place for Robin on the Batmobile :laughing:

![hehe|690x414](upload://cODyLL0YPx7PeLanwOlFjRyuS9u.jpg)

BTW this picture is from the "Batmobile Joyride Experience Australia".
Batman has full body protection which is great for but the helmet seems not safe.
```

---
## \#443 Posted by: telnoi Posted at: 2018-07-16T07:08:15.447Z Reads: 185

```
These tires (MBS T3) don't last much longer. Grip is a bit worse (more drifting in loose sand and stones).
Switching back to regular profile at least.
```

---
## \#444 Posted by: rich Posted at: 2018-07-16T09:03:38.206Z Reads: 198

```
It’s time for an update, the last weeks I had very little time to work on the board but I am back with some improvements and ready to ride again.

I sold my complete Trampa belt drivetrain with motors from V1 of this build, that’s why I could order some parts I had on my list (a long list but lack of money). Finally I have some MBS heelstraps, jesus they are huge and thick, very curious how they’ll perform, looks promising.

![021054|690x388](upload://loKEvJpP6ZzIKfqG7knoEYtsOvm.jpg)

Got 2 new shiny Unik motors and thought about how to improve the cable management. To eliminate any stress on the wires I extended and routed them different this time. Good side effect is a better compact looking and no more alien cables as usual.

![181945|690x388](upload://4Argzv4VUgAZ87zv8WnK9GCIRjI.jpg)

![225050|690x388](upload://3vAXG2gJr3IDiwY22N9Jk2C6UVT.jpg)

For the gears I’ve always used “Total Power Grease” which is a spray grease from Innotec. This time I wanted to try out something different, lithium-graphit grease. The gears are quite silent now and feel smooth but I guess this gonna change after riding.

![014804|690x388](upload://1fSTWdbyUMGuz5x5SNqxte7m8By.jpg)

I didn’t find a proper solution yet to handle the play of bearings in the superstar spokes. I killed my last bearings pretty fast I guess because of this fact. After 1000km you can see the contact areas inside the spoke, mostly it’s only on 2 sides where the color is gone. This is really annoying, used kapton tape to bridge the gaps, it’s better but not good at all.

![224449|690x388](upload://g6LIuohs14zGq864xF9mL26X3VW.jpg)

![224943|690x388](upload://v7mYxHgN9FuAhpz9nExTGGKZSlL.jpg)

Also mounted the drive guards, let’s see how they like impacts, gonna add the bull bars soon after black anodizing.

![003751|690x388](upload://a8fyyOkwBZKSD9VUzh54XlqKAL7.jpg)

There’s one strange thing happening with the tire sealant (aka green slime). After releasing the air of the tubes due to tire change it seems like in 1-2 tubes the sealant got hard and the wheels are imbalanced because the former fluid can’t spread and acts as an additional weight. @benjammin and @Duffman did you get similar problems after changing tires? 

[quote="telnoi, post:443, topic:45377"]
These tires (MBS T3) don’t last much longer
[/quote]

Interesting, do you also ride on concrete or 100% offroad?
I’ve ordered a set of T3, too plus 6 MBS Vine tires, they seem to have more rubber. I’ll report back when I hold them in my hands and also after riding.

Now I'm going for my first ride after a break of 6 weeks :grin: and I have holiday, perfect combination.
```

---
## \#445 Posted by: telnoi Posted at: 2018-07-16T09:08:43.736Z Reads: 187

```
The majority is off-road, but I have a feeling carving on concrete kills them harder.

[quote="rich, post:444, topic:45377"]
6 MBS Vine tires
[/quote]

Where did you order the vines? PM if you want to protect your source :stuck_out_tongue:
Supposedly, the vines are made of harder rubber, which should result in them lasting longer.
```

---
## \#446 Posted by: rich Posted at: 2018-07-16T09:17:40.111Z Reads: 179

```
Yeah carving on concrete is a tire killer but also sliding :stuck_out_tongue_winking_eye:

I've ordered the tires at mbseurope.com but after 2 days they wrote me they are out of stock until end of august, was a mistake on the homepage. Got refunded and ordered the vine tires [here](https://www.coronation-industries.de/shop/de/felgen-komplettrader/11845-mbs-vine-reifen-mountainboards-tyres.html) in germany. There is a second homepage of the same company with less products but also vine tires and [4x T3 for 45€](https://www.coronation-industries.de/shop/de/felgen-komplettrader/11845-mbs-vine-reifen-mountainboards-tyres.html)
```

---
## \#447 Posted by: telnoi Posted at: 2018-07-16T09:19:46.032Z Reads: 183

```
[quote="rich, post:446, topic:45377"]
Got refunded and ordered the vine tires [here](https://www.coronation-industries.de/shop/de/felgen-komplettrader/11845-mbs-vine-reifen-mountainboards-tyres.html) in germany
[/quote]

Thanks for the link. Been eyeballing these today, but looking at the site reviews (coronation) their stock indication is often incorrect :frowning:

Did you get a shipping notification already?
```

---
## \#448 Posted by: Kug3lis Posted at: 2018-07-16T09:40:47.971Z Reads: 176

```
You can try green loctite for glueing bearings into rims, it's made for it ;) Maybe will help for you. We also fixed our wheel hubs so now the bearing place is more accurate which leads into tighter bearing fit which requires bit pushing with rubber mallet :)
```

---
## \#449 Posted by: rich Posted at: 2018-07-16T09:50:12.176Z Reads: 177

```
[quote="telnoi, post:447, topic:45377"]
Did you get a shipping notification already?
[/quote]

Don't set my nerves on edge..... NO :laughing:
Just wrote them an e-mail, ordered 5 days ago. 6 days ago I asked them if they have 6 tires in stock and they said yes, it was the other homepage but that shouldn't make any difference.

[quote="Kug3lis, post:448, topic:45377"]
You can try green loctite for glueing bearings into rims
[/quote]

Good hint, does it need heat to remove?
I'm not sure if I like to glue bearings :wink:
```

---
## \#450 Posted by: Kug3lis Posted at: 2018-07-16T09:52:35.387Z Reads: 174

```
Yes, they need heat to remove, but green one is made for glueing bearings, and etc things into bit wider holes for cheaper manufacture :)

P.S. I am talking not about thread locking one, but retaining one :)

http://www.loctite.co.uk/retaining-9171.htm
```

---
## \#451 Posted by: telnoi Posted at: 2018-07-16T09:53:27.154Z Reads: 177

```
[quote="rich, post:449, topic:45377"]
Don’t set my nerves on edge… NO :laughing:
Just wrote them an e-mail, ordered 5 days ago. 6 days ago I asked them if they have 6 tires in stock and they said yes, it was the other homepage but that shouldn’t make any difference
[/quote]

Ugh, ok..hate it when that happens. This shit is my daily transportation and frustration venting equipment.
I should start stocking tires.
```

---
## \#452 Posted by: Kug3lis Posted at: 2018-07-16T09:54:23.856Z Reads: 168

```
Haha I know the feel, imagine my case ordered focbox waited 3 weeks no board to ride, UK public transport, get focbox which is defective now wait another 2 weeks for new one...
```

---
## \#453 Posted by: rich Posted at: 2018-07-16T09:59:09.839Z Reads: 175

```
[quote="Kug3lis, post:450, topic:45377"]
retaining one :slight_smile:
[/quote]

Seems promising but I guess the rubber shields of the bearings won't survive a blow torch when removing :rofl:

[quote="telnoi, post:451, topic:45377"]
I should start stocking tires
[/quote]

That's why I bought 10 :laughing: (hopefully I get them).
```

---
## \#454 Posted by: telnoi Posted at: 2018-07-16T10:00:49.979Z Reads: 183

```
[quote="Kug3lis, post:452, topic:45377, full:true"]
Haha I know the feel, imagine my case ordered focbox waited 3 weeks no board to ride, UK public transport, get focbox which is defective now wait another 2 weeks for new one…
[/quote]

Let's hope your DRVless esc will fix that stuff 4ever.

[quote="rich, post:453, topic:45377"]
That’s why I bought 10
[/quote]

Still testing different brands. Until I've found my match, it's 4 at a time :slight_smile:
Honestly, the chinese diyeboard tires weren't half bad from a mileage point of view. Seriously hard plastic, but they lasted.
```

---
## \#455 Posted by: Kug3lis Posted at: 2018-07-16T10:06:01.696Z Reads: 176

```
Oh boy you don't know how much I want that stuff to be finally on my board :D


@rich you don't need to blow bearing directly, just aluminum on the sides :)
```

---
## \#456 Posted by: rich Posted at: 2018-07-16T10:26:18.853Z Reads: 184

```
[quote="telnoi, post:454, topic:45377"]
Still testing different brands. Until I’ve found my match, it’s 4 at a time :slight_smile:
[/quote]


Doing the same, where is the everlasting tire out there? I seek I search I still can't find. But I prefer to have 6 tires. Instead of swapping front and rear tires after 50% (if you catch it right) I change the rear tires after they are worn out. The next time all 4 tires are worn out, that's why I like 6 tires.

[quote="Kug3lis, post:455, topic:45377"]
you don’t need to blow bearing directly, just aluminum on the sides :slight_smile:
[/quote]

Ah thanks, good to know.

Now my battery is charged, I'm geared up and ready to ride in the urban jungle :metal:
```

---
## \#457 Posted by: DeathCookies Posted at: 2018-07-16T12:06:30.399Z Reads: 172

```
We should produce or own pneumies!
It cant be to hard because a motorcycle or car tire will last much much longer... 

It is just that the Big players want to make some Cash...
```

---
## \#458 Posted by: rich Posted at: 2018-07-16T12:43:16.565Z Reads: 170

```
Just  came back from my 20km ride, almost forgot how great it is :sunglasses:

I like the MBS heelstraps, like the bindings they are comfy and barely noticeable. Due to their size they give good support even when they slip down, good investment.

I did monitor the realtime data, motors got 60°C and Vescs 51°C. The new motors have about 5 km/h less top speed, guess the first batch had more kv than advertised.

[quote="DeathCookies, post:457, topic:45377"]
a motorcycle or car tire will last much much longer…
[/quote]

True, imagine you drive with the car on vacation a couple of hundred kilometers to your destination. To drive back you need to buy new tires. After you reached home you need to buy new tires to get to work. If your distance to work is 50km you need to buy new tires at least four times a month. Nobody would drive a car ift it would be like that :joy:. We are poor mountainboarders.
```

---
## \#459 Posted by: telnoi Posted at: 2018-07-16T12:58:48.573Z Reads: 166

```
Those soft rubber tires are a business model for sure. The boards themselves last relatively long and any moving parts of trucks are cheap. Not much profit there except for the initial sell. 

[quote="rich, post:458, topic:45377"]
I did monitor the realtime data, motors got 60°C and Vescs 51°C.
[/quote]

Any hill climbs? My SK3 need replacing, wondering if I should go sealed or not.
```

---
## \#460 Posted by: Duffman Posted at: 2018-07-16T17:55:58.122Z Reads: 174

```
As far as I can tell the green slime is water based. Just try to drip some water in your tube and try to dissolve or thinn it.

I would also simply glue the bearings into the hubs. If you have to replace the bearings because they are broken then it does not matter if you burn them with a blowtorch and smash them out...
```

---
## \#461 Posted by: benjammin Posted at: 2018-07-17T00:25:19.667Z Reads: 176

```
No I've never seen the green slime harden like that, weird 🤔
```

---
## \#462 Posted by: rich Posted at: 2018-07-17T01:12:37.539Z Reads: 204

```
Hmmm just found out that the MBS vine tires are the same as Trampa's mudplugger, both seems to be made by Innova. 2 ply soft rubber, tssssss...

Beside the soft rubber I think the main problem is that MTB tires usually have about 2mm treads only, imagine a tire with 8-10mm :heart_eyes: 

If the treads on your car tires have 2mm left you need to replace them, for MTB it's called a new tire :thinking:

[quote="telnoi, post:459, topic:45377"]
Any hill climbs? My SK3 need replacing, wondering if I should go sealed or not.
[/quote]

Not really hill climbing but gonna test that and monitor as well. I guess a sealed motor runs a bit hotter. Did you ever had stones inside your motors?

[quote="Duffman, post:460, topic:45377"]
Just try to drip some water in your tube and try to dissolve or thinn it.
[/quote]

Good idea, gonna try it with one tube at least but before I'll deflate the tubes for further inspection. My tires need to be replaced very soon anyway. Maybe squeezing helps, too.

First feedback according the drive guards, they survived and work :grin:, recognized one hit, the other contacts I didn't recognize but there are grooves in both of them.

![023148|690x388](upload://5dzAtPbrIFeROA6eEBXonmyTwpW.jpg)

[quote="Duffman, post:460, topic:45377"]
If you have to replace the bearings because they are broken then it does not matter if you burn them with a blowtorch and smash them out…
[/quote]

Preach.... 
True words bro!

As you can see on the pic kapton tape is not the best method :joy:

![131554|690x388](upload://ztvNyxhTjTMHV9cOxc5NRTDtDAB.jpg)

[quote="benjammin, post:461, topic:45377"]
No I’ve never seen the green slime harden like that, weird :thinking:
[/quote]

Yeah that's really weird, it's stuck around the valve.
```

---
## \#463 Posted by: Duffman Posted at: 2018-07-17T03:32:38.764Z Reads: 192

```
If wear is your main concern just switch to these tires:[Mefo Ice Slider](https://shop.elektro-skateboard.de/eigenbau-tuning/rollen-reifen-felgen/444/mefo-ice-slider-dirt-runner-reifen-11x4-5-5) :rofl:
```

---
## \#464 Posted by: mmaner Posted at: 2018-07-17T04:00:12.004Z Reads: 194

```
Good God those are huge 😀
```

---
## \#465 Posted by: telnoi Posted at: 2018-07-17T05:16:26.506Z Reads: 208

```
[quote="rich, post:462, topic:45377"]
Hmmm just found out that the MBS vine tires are the same as Trampa’s mudplugger, both seems to be made by Innova. 2 ply soft rubber, tssssss…
[/quote]

And they appear to be identical to the tires that came with my first dirt cheap MTB. They lasted around 800 km. 

![15082621680|500x500](upload://3xXN3O1eUF6nU83mbR6hiO2z28i.jpg)

![200x50-8-Electric-mountainboard-Aluminium-Alloy-Pneumatic|500x500](upload://cCOQAlAc9EP7PLFuXrVzF1cNIM3.jpg)

[quote="rich, post:462, topic:45377"]
Not really hill climbing but gonna test that and monitor as well. I guess a sealed motor runs a bit hotter. Did you ever had stones inside your motors?
[/quote]

Let me know. I'll hold off my purchase untill then. It's either these or the APS 6384. Never had issues with stones, just mud and sand.
```

---
## \#466 Posted by: Okami Posted at: 2018-07-17T06:14:22.471Z Reads: 201

```
If im correct 9inch primo strikers have 4 ply. But im not at conputer to check that out. 

https://www.atbshop.co.uk/mountainboard-accessories/primo-striker-tyres

Though u would need a wide rim for them and I think the regular hypa / superstars cannot fit them.

Just a food for thought to these who shred tires more than it should :smiley: 

Maybe @Riako has some intel on 9inch strikers as i havent really used up mine, going only lightly with my board..

Though they are big so only wide trucks are recommended otherwise they give a wheel bite to the feet.
```

---
## \#467 Posted by: telnoi Posted at: 2018-07-17T08:56:26.330Z Reads: 205

```
https://www.alibaba.com/product-detail/8-inch-mountain-bike-tire-rubber_60471579252.html?spm=a2700.7724838.2017115.427.22555aefJzeV35

and here they are...just the min order is a bit...much.
There appear to be a fair number of rebrands for this tyre. Should be possible to find a good/better deal compared to Trampa/MBS.

https://www.monsterscooterparts.com/kick-scooter-parts/kick-categories/kick-scooter-tires/200x50-8-x2-tire-for-the-razor-phase-two-rds-dirt-scooters-multiple-choices.html

For now I ordered another T3 set from Evolve Germany. Ordered yesterday, arrived today.
```

---
## \#468 Posted by: rich Posted at: 2018-07-17T20:27:18.019Z Reads: 204

```
[quote="Duffman, post:463, topic:45377"]
If wear is your main concern just switch to these tires:[Mefo Ice Slider ](https://shop.elektro-skateboard.de/eigenbau-tuning/rollen-reifen-felgen/444/mefo-ice-slider-dirt-runner-reifen-11x4-5-5) :rofl:
[/quote]

Haha, well.... :joy:

[quote="telnoi, post:465, topic:45377"]
And they appear to be identical to the tires that came with my first dirt cheap MTB. They lasted around 800 km.
[/quote]

Rebranding everywhere :thinking: but 800km sounds good.

[quote="telnoi, post:467, topic:45377"]
and here they are…just the min order is a bit…much.
[/quote]

We could divide the tires, 250 for each of us :laughing:

[quote="Okami, post:466, topic:45377"]
If im correct 9inch primo strikers have 4 ply.
[/quote]

The Trampa Treads have 4ply as well but the height of the profile is too less IMO. And as you mentioned 9" tires would need different hubs as well which are not compatible with the gear drive.

[quote="telnoi, post:467, topic:45377"]
Ordered yesterday, arrived today.
[/quote]

I'm jealous!
I've ordered 7 days ago from coronation-sports.de, powerkiteshop.com and atbshop.co.uk.

Coronation didn't ship my parcel up to now and no notification, nothing, don't answer e-mail. I called them twice today and they say they have to look what's the problem and call me back very soon..... That's many hours ago. Very bad shop, I need these tires so much, my actual tires have 0.3mm profile left only. 

I've got a shipment notification of powerkiteshop today so at least they ship it after 7 days.

Best experience I have wit ATBshop, got the parcel last week already. One thing I want to mention because I had problems with my Hillbilly gloves. I claimed them and had to send several pics, later they told me that Hillbilly refused to replace them. 2 weeks and some e-mails later the shop owner had mercy and send me a free new pair, this is some good customer service!

![150910|690x388](upload://fbbne7KWgzWCNqUXIeCg4wQ4tEZ.jpg)
```

---
## \#469 Posted by: FredrikHems Posted at: 2018-07-17T21:53:35.431Z Reads: 199

```
What about trying something like these wheels? https://m.ebay.com/itm/3-50-4-10-4-Inch-Wheel-Rim-Tyre-Tire-49cc-Mini-Quad-Dirt-Bike-ATV-Buggy/281275675540?hash=item417d563394%3Ag%3ADfcAAOxy4fVTEJbF&_nkw=10»+mini+atv+wheel&_from=R40&rt=nc 
I know duffman used them, and he said he had gone thru 2 sets in 5 months or so (i think). While it may not be alot, it seems like the Trampa ones last even shorter... 
i dont know, just shooting out a thought here. :grinning:  
Their about 10” and abit wider too, so they should help with traction i guess :grinning:
```

---
## \#470 Posted by: Duffman Posted at: 2018-07-18T03:46:24.122Z Reads: 194

```
Simply forget those tires!!! These were the most crappy tires I've ever had. They stink like a chemical factory and I'm not sure if they are even made of rubber...

The second worst tires I had were the trampa treads: they wear down very fast and had way less grip than the mbs t3 tires I used before.

Right now I'm running t3 in the front and on the back vine tire / mud plugger or whatever the real chinese manufacturer calls them...
```

---
## \#471 Posted by: FredrikHems Posted at: 2018-07-18T07:07:34.324Z Reads: 187

```
Oh, Okay. I had no idea they were that crap
```

---
## \#472 Posted by: rich Posted at: 2018-07-18T08:09:37.214Z Reads: 199

```
Thanks for the link but I need 8" and as Duffman wrote

[quote="Duffman, post:470, topic:45377"]
They stink like a chemical factory and I’m not sure if they are even made of rubber…
[/quote]

:joy::rofl: that's too funny
Probably they are made from a factory specialized in tires for barrows.

I've never weigh my board but now I did: 15.5kg (34.2 lbs) , wow,  thought it's less but now I know why it's hard to carry.

Haha @Duffman @Nowind  I just wanted to check the drive guards after my second ride and one is gone :rofl: only a small piece is left around the screw. Recognized a harder hit but not that I've lost it.

![095506|690x388](upload://74LmxRhn7VqKDUxdWTDmYB2Hwok.jpg)
```

---
## \#473 Posted by: Duffman Posted at: 2018-07-18T12:39:37.905Z Reads: 195

```
So its time for the next round: TPU
```

---
## \#474 Posted by: rich Posted at: 2018-07-18T13:12:38.727Z Reads: 191

```
Thanks bro, PM'd you :+1:
```

---
## \#475 Posted by: Riako Posted at: 2018-07-18T15:43:20.552Z Reads: 198

```
Sorry, I'm late guys ^^
About Primo Stricker 9" (I also got the 8" but not used so much actually).
This 4 wheels always on the DarthVapor setup run since before 2015 ... Don't know really when 2014... 2013...
Got more than 1000 and 1000km I think, never flat :blush: never ever !! (now I say that I have to be careful but since my 1st ride with them in 2015 it's always a pleasure to ride !)
On big grass, under the rain be careful with the trigger they slip easily.
I ride low-pressure always at 2bar...
Rear tires start to become slim/slick more and more, but it takes time. I carve but not extremely. If Withepony rides them, maybe they probably won't pass a year of use :smile:  
I like those for all road use (road, dirt and some offroad), got the 8" setup soon on an other build...
```

---
## \#476 Posted by: michaelcpg Posted at: 2018-07-19T03:41:51.546Z Reads: 191

```
Interesting to hear. I'm using the soft Trampa Treads with my first build and I've also found that they wear pretty quickly, although I don't yet have any experience with any other tires. Was thinking about eventually replacing them with the hard Trampa Treads but I'm guessing there's better options out there...

Anyone have any recommendations for 8" tires that would mostly be used on road but are still suitable for dirt tracks on the weekends etc? 
Are there any 9" tires out there that fit on Trampa Superstar hubs?
```

---
## \#477 Posted by: telnoi Posted at: 2018-07-19T15:30:23.441Z Reads: 188

```
[quote="michaelcpg, post:476, topic:45377"]
Are there any 9" tires out there that fit on Trampa Superstar hubs?
[/quote]

No, but there should be :P
@trampa
```

---
## \#478 Posted by: trampa Posted at: 2018-07-19T17:49:18.450Z Reads: 178

```
There are no 9" that fit 8" hubs.
```

---
## \#479 Posted by: rich Posted at: 2018-07-20T16:01:46.699Z Reads: 212

```
[quote="Riako, post:475, topic:45377"]
1000km I think, never flat :blush: never ever !!
[/quote]

1000km sounds great but no flat even better! I had at least 8 flats within the first 800km :face_with_raised_eyebrow:

[quote="michaelcpg, post:476, topic:45377"]
Was thinking about eventually replacing them with the hard Trampa Treads
[/quote]

I had 2 sets of Treads in hard compound, first lasted about 600km (with perfectly timed swap of front and rear tires), the second looks like this after 300km (swapped too late and did some slides) :joy:

![141421|690x388](upload://8oQd2f9nXaXOqwenBzX8ZCwz3S4.jpg)


I was too scared to ride them today, fortunately I got this right now :sunglasses:

![20180720_162553|690x388](upload://1AtNgVxYYRJEmy7UIdSvvcFkuhK.jpg)

Interesting, on pictures the Vine tires look like they would have deeper profile than T3's and are more solid. Both tires have a tread depth of about 3mm, the Trampa Treads and Rubena tires had about 2.2mm. The T3 tires have more solid structure, it's not easy to squeeze them but the Vine tires are more soft and easy to squeeze but will be more comfortable to ride than T3's, gonna start with the Vine's and see.

![20180720_162600|690x388](upload://bmjZDhQhMmWC41jK3vecqDd6JmO.jpg)

[quote="michaelcpg, post:476, topic:45377"]
Anyone have any recommendations for 8" tires that would mostly be used on road but are still suitable for dirt tracks
[/quote]

If it's hard packed dirt and not really hardcore offroad you could use road tires, they also should last longer. If you are in EU and want some cheap road tires you could check this out: 
Model O200K 1 tire 6,20€ :laughing:, 1 tire including inner tube 8,31€ :joy:

![ZABI_O200K|547x500](upload://6hnIUFJcwAjGtbdBAz2Wddme64U.jpg)
https://www.zabi-rollen.de/de/angebot/47/reifen/

I know that @Idea use(d) them on MTB and I think @whitepony also ordered them once, would be interesting how long they lasted with hard carving :crazy_face:
```

---
## \#480 Posted by: No-Rules Posted at: 2018-07-20T16:34:57.686Z Reads: 206

```
I will receive those soon and I will give you a return on their longevity
![pneu-trottinette-200x50|500x500](upload://kn5n6t3XLDXWpWkkXeqtyU3LDxv.jpg)
```

---
## \#481 Posted by: rich Posted at: 2018-07-21T17:35:10.560Z Reads: 208

```
Which tires are those?

I bought new premium inner tubes because my old ones are all (multiple) fixed with bicycle repair stuff which is not flexible. The rubber of the new tubes is thicker and the material around the valve is stronger, also the valve is longer which is great for inflating but maybe not best for offroad, let's see.

![203812|690x388](upload://tcME5qyFwdfsKPaQNbjm07DjeHO.jpg)

Of course filled with the obligatory tire sealant, this tubes won't need bicycle repair kit because they are flat proof now.

![005343|690x388](upload://nvJiuyirjtVEsDMEX6fZFR2GJcs.jpg)

I had my first ride with the MBS Vine tires and are really surprised about their performance, I'm a bit disappointed. On concrete they run very smooth with good grip and normal offroad is also OK if you don't make (tighter) turns but e.g. on loose gravel they are slippery on turns, I had a lot of almost crashes because they started sliding where the Trampa Treads had good grip like on BMX track, weird.

I guess it's the kind of the continious middle profile which makes it more an "All Terrain" tire than a real MTB tire. No idea why it's called massive offroad tire or mudplugger in the descriptions. 

![190703|690x388](upload://1WUyof3mtaKB8MGjlHm2gEZgtlO.jpg)

I'm curious how the T3 tires are in comparison on loose gravel but I'm afraid there is not much diffference.
```

---
## \#482 Posted by: Duffman Posted at: 2018-07-21T22:18:42.892Z Reads: 199

```
The lateral stability is always a problem of the tires with a solid running surface.

![IMG_20180624_194500_HDR|690x388](upload://3cXSqRHdYEAj0PXlRh44h8Th0Ia.jpg)

I used a hacksaw to add a diamond pattern to the middle running area and I'm quite statisfied with the improved curve stability.
```

---
## \#483 Posted by: rich Posted at: 2018-07-22T05:45:06.332Z Reads: 205

```
Siiiick dude :sunglasses:, what a crazy DIY lifehack, can't believe you sliced them, must be weird doing that. Let's call it DDP (Duffman Diamond Pattern). Do you feel a difference between the bigger and smaller DDP's?

Did you ever try T3 tires? It looks like they could have better offroad traction when compared to Vine. 

![075319|690x388](upload://va8CteG3qvkfQC4dKtvMMkRjBjn.jpg)
```

---
## \#484 Posted by: Duffman Posted at: 2018-07-22T17:16:45.347Z Reads: 192

```
I'm running t3 in the front and vine in the back. Both of them with DDP. 

In my picture above are mbs vine with DDP on the left, trampa mudplugger in the middle and mbs t3 with DDP on the right.
```

---
## \#485 Posted by: rich Posted at: 2018-07-22T19:20:21.331Z Reads: 188

```
Oh my bad, was so focused on the DDP's and didn't recognize the T3.
I have 2 questions: Why don't you just use tires with offroad pattern? And second how the hell you manage to slice/saw not too deep? It's a bit like playing with fire :laughing:.
```

---
## \#486 Posted by: Duffman Posted at: 2018-07-23T05:40:57.922Z Reads: 192

```
Are there any 'real' offroad tires for 8" hubs? All tires I know have either a flat running surface in the middle or a very flat pattern.

Playing with fire is the right description. Simply don't cut too deep ;-)
```

---
## \#487 Posted by: rich Posted at: 2018-07-24T19:24:27.099Z Reads: 198

```
With "real" offroad tires I mean tires without any middle surface, only knobby. For example real mountainbike tires usually have no middle surface and if so it's a hybrid or cross country tire.

BTW I found out today that mudpluggers get stucked in mud :joy:

![200918|690x388](upload://mnzCPhKHTHPcnKPymuD22Ei9Jlh.jpg)
```

---
## \#488 Posted by: FredrikHems Posted at: 2018-07-24T19:52:19.751Z Reads: 201

```
Time to upgrade to bigger diameter ones? :sweat_smile::sunglasses:
```

---
## \#489 Posted by: Narnash Posted at: 2018-07-24T21:25:29.978Z Reads: 205

```
https://shop.elektro-skateboard.de/media/image/0e/2f/65/mefo_ice-slider.jpg
@rich time for an upgrade
```

---
## \#490 Posted by: telnoi Posted at: 2018-07-25T04:46:51.373Z Reads: 195

```
[quote="rich, post:487, topic:45377"]
mudpluggers
[/quote]

Tire gets plugged with mud to form a super efficient smooth surface. If you go fast enough, it will get flung into your face, taking away the fear factor (just floor it, don't see anything).
```

---
## \#491 Posted by: amecces Posted at: 2018-07-25T06:19:20.524Z Reads: 197

```
https://www.berghspecialproducts.de/reifen-und-zubehoer/rollstuhl-decken-schwarz/L.BU.0802.Z1

Just for offroad! On Street they will be down within minutes
```

---
## \#492 Posted by: Nowind Posted at: 2018-07-26T13:26:29.287Z Reads: 209

```
[quote="trampa, post:478, topic:45377, full:true"]
There are no 9" that fit 8" hubs.
[/quote]


Strange 
Running 9inch Striker Wheels on Flame Cryptics Hubs for long time, same for varios 8inch Tires on same Hub.
Works great. Even with sickest motors and Vesc settings

https://www.rideflame.de/shop/felgen/

![K800_P1020732|666x500](upload://qWpg9lHgiE1PHf3xAce3pz7fsCn.JPG)

![K800_P1020737|666x500](upload://vyqX90evnnCDtyXnuE6btYLWPvS.JPG)
```

---
## \#493 Posted by: Duffman Posted at: 2018-07-26T16:53:24.566Z Reads: 205

```
I even regrooved THESE with a special DDP pattern to gain more lateral stability:
![IMG_20180726_183859|281x500](upload://h4nPRjGbpuigWMzILNhdfENp2eM.jpg)
![IMG_20180726_184157|690x388](upload://gBU4dRuBffVb5iZhXn2Syj9vEpt.jpg)
```

---
## \#494 Posted by: rich Posted at: 2018-07-26T19:18:24.649Z Reads: 204

```
[quote="Nowind, post:492, topic:45377"]
Running 9inch Striker Wheels on Flame Cryptics Hubs
[/quote]


Good 2 know :sunglasses:

Is the bolt pattern the same as a specific Trampa or MBS hub?

@Duffman that's sick. Also this monster build is one of the craziest builds ever bro! Common, the motors look like a joke beside this bad ass wheels :rofl:

Today was a funny day including 65km of riding. I woke up at 5 am (which is way too early) and decided to go for a peaceful morning sun ride which was a  great idea, have to do that again.

![062204|690x388](upload://ofLEkwF7O4w4Oo0y7miy4bYNeGB.jpg)

Later I rode on a narrow sidewalk and after a curve suddenly it looked liked that, almost crashed, crazy shit!

![122021|690x388](upload://15rvlJShVDEaAuEPJPPgG5THyX3.jpg)

![122034|690x388](upload://xRzdohdYLtj90EUt6NEnKUg3bIh.jpg)

In the end it started raining when I was still 10km away from home and I decided to ignore it, after a while the remote started to have strange behaviour, bouncy and hard acceleration and braking, sometimes braking without touching the throttle but I made it home (was a challenge) and it seems to work again as usual. 

Conclusion of the day, I definitely need more range because 3 times charging for 65km sucks, I want to explore new paths and areas and not ride in circles all the time, weird first world problems :laughing:
```

---
## \#495 Posted by: telnoi Posted at: 2018-07-26T19:42:47.237Z Reads: 201

```
[quote="rich, post:494, topic:45377"]
Is the bolt pattern the same as a specific Trampa or MBS hub?
[/quote]
middle one, sadly no...at least not compatible with sstar.
http://www.e-toxx.com/wp-content/uploads/2016/08/K800_SuperstarCrypticHypa.jpg
```

---
## \#496 Posted by: Nowind Posted at: 2018-07-26T19:58:43.326Z Reads: 202

```
thanks @telnoi for the picture
@rich yeah unfortunally not compatible
i got hubadapters for the Flame Hub but the problem was always the axle length
(Supertars are very narrow in the area where i mount the hubadapter compared to others)
But i can tell you that maybe in near future there will be a solution for this

Also the "FiveStar" from MBS works with 8 and 9inch (-;
But same like above.

Cheers
```

---
## \#497 Posted by: rich Posted at: 2018-07-27T22:09:04.865Z Reads: 207

```
It's always like christmas when receiving a parcel from E-Toxx (and the next is on the way) :santa:

![143243|690x388](upload://tzWkfX2tE3hwh1Qo4DS22gwqCHn.jpg)

The bull bars are for 12V 18W offroad light with 3s1p Li-ion and charge port on the front truck. It's easy and quick to mount, it's just 2 bolts so I can carry it in the backpack or attach it at home if necessary.

The new TPU driveguards are magical
![144709|690x388](upload://pyXKAl0gSh9RQTxlXcNrT2IY1dU.jpg)

and flexy
![144745|690x388](upload://zm5yDLLkYENJzDCpXU6KvK7avcZ.jpg)

I've mounted them today and had one of the most wicked rides ever at a construction area below the highway. I did try my best to destroy the driveguards with many and massive stones. It is always the most fun when you ride like there is no tomorrow and today there was no tomorrow. In the end I thought I damaged the driveguards and housings for sure because when riding there was not this usual random single hit. No it was: "Pock, pock, kleng, tock, tack, pock, tong, klack" and so on all the time. For sure I had at least 200-300 impacts today.

![201431|690x388](upload://696G9slGDBZv0XVTY9LwX7a4EA0.jpg)

![201911|690x388](upload://2hx208KhRcTS4nOWFEETzyelluc.jpg)

![203011|690x388](upload://azpC4SgnirXcvcCf57wvsaKqwWx.jpg)

After cleaning everything I was scared to check how it is looking but then..... WTF just some grooves on the driveguards and one small damage but nothing else after this massive attack :laughing:

![230601|690x388](upload://wPuncnz9XnjsgKWq5ZfTKGzCdnf.jpg)

@Nowind @Duffman  these new flexy driveguards take most impacts like a king, well done! :clap:  Next test is the curb test.

The other damages from today are some deeper scratches on one motor from a crash but that's aesthetical only. And I can't turn off the volmeter and the backlight is dead as well since my ride in the rain yesterday.

Yeah and my bushings are almost done again, the hangers start rattling especially the rear one when accelerating offroad, that's the sign for a change. I started to save some telemetry data of my rides so I'll know exactly how long tires or bushings lasted.  

That's it for now, I wish you all a great esk8 time!
```

---
## \#498 Posted by: telnoi Posted at: 2018-07-28T18:05:12.806Z Reads: 205

```
Full coverage for me after bending the inner plate. Some measurements left to take (yes, I can print overhangs like that - no, I won't make the file available. E-Toxx sells the Duffman version depicted above - https://www.e-toxx-shop.com/trampa/direct-drive/drive-guards-tpu/#cc-m-product-10002765770).
![49|509x499](upload://1wZFaAdCZ4Aw96brq7oTOpHsUJQ.jpg)
```

---
## \#499 Posted by: rich Posted at: 2018-07-28T19:56:08.607Z Reads: 188

```
Looks interesting, too. Do you print them with a flexible material like TPU?
```

---
## \#500 Posted by: telnoi Posted at: 2018-07-29T04:13:38.795Z Reads: 199

```
[quote="rich, post:499, topic:45377"]
TPU
[/quote]

Yes. It's the only material that won't split apart or break, especially if you print it at higher than normal temperatures (layers melt together really nicely).
```

---
## \#501 Posted by: rich Posted at: 2018-08-01T20:26:11.649Z Reads: 209

```
More e-toxxication, elastomere dampers :heart_eyes:

![203645|690x388](upload://jozhIAPLLukiEAad3wFFl12WeS3.jpg)

Can't wait to test them, unfortunately I have to wait until tomorrow because of Loctite. They were a bit tricky to mount because the bolt and nut of the baseplate are very close (no problem to mount on carve baseplate). 

![204625|690x388](upload://zalz47Cs3M2Dxzq28LTie3qU542.jpg)

I replaced the front bolts to flat head and mounted them upside down. 

![133724|690x388](upload://7ZUqrCXVJTAGxKbUk9aXafuBZv5.jpg)

On the front truck it works perfectly, on the rear truck the bolts are a bit closer to the dampers (couldn't rotate the dampers freely), that's why I had to mount both dampers first to the deck, then the 2 baseplate bolts and then the hanger. With some sweat (32°C inside) it worked with 2 clamps to get the hanger in the right position.

Seems like I'm the original bushing killer, didn't last long :face_with_raised_eyebrow:

![bushing|690x388](upload://nabBiU2PNPmD0aGIYnwMuwFs52x.jpg)

I've had a weird experience this week, made the mistake to make a turn with too much lean on a path with big cobblestones and started skidding like a car, left-right-left-right. Fortunately I didn't crash and could stop the movement.
```

---
## \#502 Posted by: DeathCookies Posted at: 2018-08-01T21:00:54.809Z Reads: 198

```
Dude... Is there even a bushing you cannot destroy? :D
```

---
## \#503 Posted by: rich Posted at: 2018-08-04T21:18:47.663Z Reads: 207

```
@DeathCookies  No :laughing:

Well I didn’t find the root of the problem and it’s really getting worse! After replacement and 20km riding one brand new bushing looks like that

![20kmBushing|690x388](upload://hivGrEQWn9PhXzIHag4KhevCnTy.jpg)

Seems like the bushing was turning inside the hole of the hanger and got sanded down. I found out that this one hole is a bit bigger than the others. Fortunately I have bushings which I normally have to sand down because they are too big but fit perfect in this hole. To fill the gap I used DIY washers 



But after 10km the whole truck started to rattle again and sound broke. Now it’s not a problem outside of the bushing, it’s sanded down inside, WTF no idea what’s wrong, I can’t replace bushings after every ride, that’s stupid.
```

---
## \#504 Posted by: rich Posted at: 2018-08-04T22:06:16.374Z Reads: 206

```
Shot this video showing the behaviour of the elastomere dampers at different speeds and terrains. The original video with music is locked (copyright) so this version is with pure esk8 sound. Enjoy!

https://youtu.be/S1ezP3P8HSg
```

---
## \#505 Posted by: janpom Posted at: 2018-08-05T09:30:46.066Z Reads: 197

```
Batman shoes! :laughing:
```

---
## \#506 Posted by: rich Posted at: 2018-08-05T09:48:59.235Z Reads: 196

```
Haha, fortunately I don't hear this anymore since I've painted the logo black with edding. Good reminder for feedback, I like the improved stability with HiTop shoes and also the smooth leather is easy to clean. The only thing missing are some soft insoles, it's quite hard.
```

---
## \#507 Posted by: rich Posted at: 2018-08-10T11:17:27.056Z Reads: 207

```
Spent the last days at Lake Constance in switzerland and germany without board so I can't wait to ride again.

![113035|690x388](upload://dP0iwCOiXaS9TmmHMgyIkUa0Eys.jpg)

Replaced the kingpin which was a little bit bent and trying to fix my bushing problem. I have various bushings at home (I’m afraid I need to order more soon) and they differ a bit in ID and OD which means either the bushing sits loose or the kingpin has play, try to find out what’s better. 

I guess it’s better with play on the kingpin but then the truck sounds very broke and the hanger moves and it's getting worse when riding. When the kingpin in the hanger sits a bit  loose (can rotate) the bushing gets damaged ultra quick.

Or I glue the bushings on the hanger but don’t know which glue I should use which is easy to remove but still strong. I have to find a solution as I eat bushings for breakfast right now.

But before deciding what to do I would love to hear a explanation from @trampa how the movement on the spring trucks should work. Which part should move (rotate) and which should stay on place?

* Kingpin
* Bushings on the hanger



On the baseplate the bushings are very tight so I think they can’t rotate.
Thanks in advance!

![VertigoTruck|690x358](upload://lcZK4CuQJruSluZ7RsmhHiZ1AJo.jpg)



Hmm... after 160 km (100 miles) the rear tires show definitely more wear, let's see how long they last.

![120411|690x388](upload://4gYzVwLdegwSGHFDWF2n5wLXWYg.jpg)
```

---
## \#508 Posted by: telnoi Posted at: 2018-08-10T12:55:16.573Z Reads: 206

```
[quote="rich, post:507, topic:45377"]
Hmm… after 160 km (100 miles) the rear tires show definitely more wear, let’s see how long they last.
[/quote]

Getting sick of these tires. My freshly installed T3 lasted maybe 2 weeks before the middle profile was almost gone.

That's roughly 180 km.

group buy? I'm sure the min order quantity can be negotiated...

https://www.alibaba.com/product-detail/200-x-50-pneumatic-tyre-for_60381511644.html?spm=a2700.7724838.2017115.166.3e8a4d3743pAG0
```

---
## \#509 Posted by: rich Posted at: 2018-08-10T13:36:28.015Z Reads: 206

```
Nice find, motivated me to do some research for this tires on aliexpress.....
I would say back to the roots telnoi :laughing:

https://de.aliexpress.com/item/Reifen-und-Schlauch-200X50-Volle-R-der-Gr-e-8X2-Reifen-f-r-Elektrische-Roller-Rad/32876980889.html

32€ for 4 tires including free shipping!
But you have to order 2 at once twice, otherwise the shipping is not free. I just paid 2 and then ordered 2 again it worked flawlessly and no problems with customs, too :sunglasses:.

Do you swap front and rear tires after 50% of riding?
```

---
## \#510 Posted by: Mobutusan Posted at: 2018-08-10T15:03:55.264Z Reads: 201

```
That sucks about the bushings. Any idea what material they are made of? Maybe a material with high compression strength and low friction like Delrin or HDPE could work? Hopefully, @marcmt88 can chime in on the Delrin suggestion.
```

---
## \#511 Posted by: telnoi Posted at: 2018-08-10T15:26:08.116Z Reads: 201

```
Awesome, yah..honestly considering buying more directly from there. It seems many suppliers are more than willing to offer good prices for the stuff we need.

PS. Really interesting how much marketing plays a role in selling these products.
A: give it an obscure name to hide the origins of the product
B: give it a cool description (Electronic scooter tires? Doesn't sound good..these are the ultimate offroad tires)
C: profit

Regarding the bushings. If you send me some measurements I could try printing a special pair with a certain material.It's TPU based, but with a very high shore value.
```

---
## \#512 Posted by: Kug3lis Posted at: 2018-08-10T15:47:26.746Z Reads: 193

```
Hmm, this is interesting I just replaced hanger with bushings after 3.5k miles and my bushings looked pretty much no different from new apart of several scratches. Maybe your hanger and baseplate holes are bad?

P.S. I am riding on streets mostly and jumping a lot because of red/blue dampas
```

---
## \#513 Posted by: rich Posted at: 2018-08-10T20:23:47.699Z Reads: 210

```
Thanks for your replies :grin:

[quote="Mobutusan, post:510, topic:45377"]
Any idea what material they are made of?
[/quote]

No idea what the trampa bushings are made of

[quote="Mobutusan, post:510, topic:45377"]
Delrin or HDPE
[/quote]

Unfortunately I have zero knowledge about 3d printing and the materials but sounds interesting.

[quote="telnoi, post:511, topic:45377"]
honestly considering buying more directly from there
[/quote]

If the price is nice I'm in but I guess it's more than 8€/tire in the end. You have to pay shipping costs and if it's TNT or similar courier you have to pay tax plus some fees. I ordered stuff from Maytech directly and had to pay shipping plus paypal fee plus tax plus fees and in the end it was way more expensive than in europe.

[quote="telnoi, post:511, topic:45377"]
A: give it an obscure name to hide the origins of the product
B: give it a cool description (Electronic scooter tires? Doesn’t sound good…these are the ultimate offroad tires)
C: profit
[/quote]

:rofl: You got it

[quote="telnoi, post:511, topic:45377"]
Regarding the bushings. If you send me some measurements I could try printing a special pair with a certain material.It’s TPU based, but with a very high shore value.
[/quote]

Wow thank you very much for this offer :hugs:
The only thing I wonder is if TPU has too much friction compared to hard plastic when it's rubbing on rotation (on kingpin and baseplate). But I'm sure TPU would be perfect against cracking.

Would love to test a pair ( but I use 2.5mm and 3mm base). No idea how much TPU can be compressed but 1 hole is 10.04mm, the other 10.15mm. The inner diameter is 8mm.

@Eboosted made a file but I don't know if it's tested.

https://www.thingiverse.com/thing:2392543 

But before you spend any time on this I want to test my actual solution, also I'm thinking of changing the hanger and then the measurements would be different.

Because after a 20km ride today the new bushings are still fine which is a great improvement. I changed the bushings on the baseplate (kingpin had play) and added layers of kapton tape on the bushings on the hanger until they couldn't rotate anymore. I can't say how long they last but I was jumping in dirt park and bmx track and roughest terrain only today and no weird noise yet, only a little play like on the front hanger. I'll see after the next ride(s) what's going on.


[quote="Kug3lis, post:512, topic:45377"]
Maybe your hanger and baseplate holes are bad?
[/quote]

I think the main problem is my hanger, some weeks ago 2x2mm bushings were fine, now it's 1.5mm more so it's bent inside also 1 hole is bigger, guess I abuse the trucks too much.

[quote="Kug3lis, post:512, topic:45377"]
I am riding on streets mostly and jumping a lot
[/quote]

If you tired of jumping and want more longboard feeling you have to try these :sunglasses:

https://www.e-toxx-shop.com/trampa/elastomere-damper/
```

---
## \#514 Posted by: Kug3lis Posted at: 2018-08-10T20:28:09.326Z Reads: 188

```
I had my orange ones but it wasnt same feeling as hard dampas at 70kmh :D
```

---
## \#515 Posted by: rich Posted at: 2018-08-10T20:30:50.911Z Reads: 184

```
[quote="Kug3lis, post:514, topic:45377"]
70kmh
[/quote]

That's suicide :crazy_face:
```

---
## \#516 Posted by: Kug3lis Posted at: 2018-08-10T20:37:57.725Z Reads: 189

```
It's just city highways :D That's why I switched to full hard dampas and bindings, it's just pleasure to speed through cars and race them on red lights and see drivers faces at next stop light :D

At top speed I don't even feel slight wobble or etc if not bindings I could dance on the deck I guess :D
```

---
## \#517 Posted by: rich Posted at: 2018-08-10T21:20:54.551Z Reads: 204

```
I hope you wear good protectors @Kug3lis  :wink:

Forgot to mention that today was my first time jumping in dirt park after weeks and the very first time with MBS heelstraps. Wow what a difference, they kept me locked no matter what I did even after 180's. With Trampa heelstraps I had to readjust them after 1-3 jumps or one 180. With MBS zero readjusting, great!. They also slide down but you are still locked and not half-locked because they are bigger.

I really like the elastomere dampers and still didn't try them with pre-tension because I enjoy the carving and tight turns so much. Crazy how this small things effect the ride experience so much. The only thing because it's more sensitive is that when jumping you need good balance when landing. Today I left the track several times because of imbalance on landing, but quite funny. It'll take some more rides to get 100% used to the different behaviour but then it's unbeatable. I make u-turns on so many places which was impossible with springs.
```

---
## \#518 Posted by: Kug3lis Posted at: 2018-08-10T21:31:31.947Z Reads: 214

```
I sport Icon Variant (BattleScar) helmet, and if  am going crazy I put on some other protections, but normally on commute I am just with helmet, I am not doing crazy stuff which would require bailing out or etc... I speed only if I see possibility and etc ;)

Thinking of getting this to go with Mark 48 project :D as its more street board

![image|500x500](upload://gAEARmYtCa70KGtdrpl3mPwOVSQ.jpg)
```

---
## \#519 Posted by: telnoi Posted at: 2018-08-14T17:05:43.125Z Reads: 198

```
Upgraded my 149 kv to 12s, top speed around 50 km/h now. Scary enough today after I blew another fucking tire. The MBS T3 are absolutely horrid. Probably the shortest run time out of all tires I tried so far (200 km before end of life).  Once the wiggly line is no longer visible you can basically throw them away as a regular small stone can press through the rubber and puncture the inner tire. 

Funnily, I am back on my "clever" branded tires that look identical to the Trampa vine, also 80PS. They have lasted over 1800 km, though I am certain my driving style changed since they were last used.
```

---
## \#520 Posted by: rich Posted at: 2018-08-14T22:31:41.720Z Reads: 197

```
200km is really bad range. I don't feel motivated to try out my T3's :laughing:

Wanted to go for a ride but a motor gear was loose so no ride today.
```

---
## \#521 Posted by: rich Posted at: 2018-08-24T11:36:20.634Z Reads: 209

```
14 days after ordering I received the cheap tires from aliexpress today.

![115203|690x388](upload://8kpdUNdhOzqZBGpKpeCuKHTh2Vf.jpg)

Looks equal to MBS Vine but they are made of different more rigid nylon material which has less grip and is heavier. Could be that this tire is flatproof :laughing:

Seems like they are the same tires which you already used in the past @telnoi so 50% price and at least 200% range. Could be that the riding experience is more uncomfortable with this hard tires. I remember when I switched from soft Rubena tires to Trampa Treads (hard compound), it felt like wood wheels compared to the thin tires. But these chinese ones from Aliexpress are heavy duty ultra mega hard compound :crazy_face:

https://youtu.be/XDoZyiLUXBY
```

---
## \#522 Posted by: Okami Posted at: 2018-08-24T13:17:39.563Z Reads: 205

```
Compound / material difference is quite drastic..

I guess I wouldnt trust for more than 50km, if heavy burnouts were planned for these Vine tires..

They look like a joke in comparison.. material looks so thin :open_mouth:
```

---
## \#523 Posted by: rich Posted at: 2018-08-24T14:25:47.484Z Reads: 213

```
[quote="Okami, post:522, topic:45377"]
They look like a joke in comparison… material looks so thin :open_mouth:
[/quote]

The MBS Vine last since 350km and still have 50% rubber left on the rear tires, front tires have more rubber..

But let me lift the joke to the next level!
You think the Vine tires are thin? No man, my Rubena tires are thin. If you can hold you tires like that it's definitely soft compound  :laughing:

![20180824_155224|690x388](upload://ybHHPP9sqlLfCuWVjkXV7wNean7.jpg)![20180824_155300|690x388](upload://jCmzKVYS4gX1n9S6bTnLfwubdfQ.jpg)

But these were the most comfortable tires I've ever had because of the weakness they acted like a suspension. But bad offroad traction and one exploded.
```

---
## \#524 Posted by: telnoi Posted at: 2018-08-24T21:36:58.864Z Reads: 212

```
Haha, that's just an awesome comparison. Yes, these are most certainly the same tires that came with my China board.

A harder compound is of course going to be less comfortable and will have less grip, but I will gladly endure it for higher durability.
```

---
## \#525 Posted by: chrisLawrence Posted at: 2018-08-26T14:06:44.121Z Reads: 211

```
I bought some red ones from a local scooter shop and they are holding up well so far after 60km.
They feel more solid. You can see them on the back:
https://youtu.be/gu0B8gp_BBo
```

---
## \#526 Posted by: rich Posted at: 2018-08-26T14:27:02.747Z Reads: 202

```
Nice video :grin:
We mountainboarders are poor people. It's a tragedy to be happy when a tire still looks good after 60km :rofl:
```

---
## \#527 Posted by: Gaza65 Posted at: 2018-09-05T04:41:48.957Z Reads: 198

```
Pic and how much?
Regards garry wagener
```

---
## \#528 Posted by: rich Posted at: 2018-09-18T11:31:18.194Z Reads: 207

```
Time for some updates

Disassembled and degreased a drivetrain and did some inspections. After about 1000 kilometers (620 miles) the gears still look quite good. @Nowind estimates at least 2000 km and I'm sure the gears can take another 1000km and more than that. BTW using black grease on black gears was not the best idea.

![231935eR|690x388](upload://c7EcZkHw8r114EJmHlGxfiGtj1.jpeg) 

![205231|690x388](upload://lQVd5d46FlXAhGUvzjg2PaPgv3p.jpeg)

There are a few very small damages at the edges but that could be my fault. I had to re-mount the gears several times and therefore adjust the backlash. The wheel gear has a support bearing but it can happen when spinning (fast) by hand that the gear gets aslope and the edges have to take the force. I guess this is what happened.

![205459he|690x388](upload://3jXKCMuNXi0noQGq7NpFe0xJTer.jpeg) 

But nothing to worry. In the future I&rsquo;ll attach the hub to the wheel gear before adjusting the backlash. This way the gear stays straight when spinning by hand and it&rsquo;s also perfect to check the hub/bearings if there is any wobble. Almost all hubs wobble but it&rsquo;s best to choose the most true hubs for the gears.

As mentioned my vertigo hanger is totally bent (guess from jumping) and eats bushings at breakfast. Listen to this sound :laughing:

https://youtu.be/MZ6mkF8Cgsg


![110640h|690x224](upload://8oeK5DCwkZuum2B84fZLdIqV1f6.jpeg)

Time for a new baseplate and the Infinity hanger. 
I filled the gap between bushing and hanger with sugru, hope that helps a bit as support.

![124816|690x388](upload://lAiCwXIn6MnTtIjyAQYhA6Emkz2.jpg) 

![124045|690x388](upload://bZcm9cedVnqSQvzFXznG2JoFK1p.jpeg) 

Time for some epic changes, soon I send the DIRT MACHINE into silence :heart_eyes::heart_eyes::heart_eyes::heart_eyes::sunglasses:

![232838|690x388](upload://e2mZWae8EDEOBXVseIcbNsoTcZP.jpeg) 
![232810e|690x312](upload://gAQkSG0iT8j21VJwb9VDQAmuxha.jpeg) 

I'm so excited and can't wait to hear it, ah I mean not hear it. Holy @Duffman @Nowind shit!  

Need to prepare the motors for axial load first and also thinking about using Loctite 641 retaining compound for the wheel bearings and motor gear but it&rsquo;s hard to find.

Some more esk8 porn comparing straight cut and helicals.

![232504e|690x309](upload://vVkxSnjvjr5eXItmdQdcNxWJpq9.jpeg) 
![231935e|690x329](upload://hzRTUKPE46fpgJkswN2HRSgRrRK.jpeg) 
![232322e|690x297](upload://wdaNyuk08g5HV0wnNDwzmUeKhes.jpeg)
```

---
## \#529 Posted by: DanSkates Posted at: 2018-09-18T11:56:47.379Z Reads: 187

```
Duuuuuuuuuuuuuude!!! This makes me super happy!! I can’t wait to not hear your board 🤫

I’ve been offline quite a bit the last few months and my boards are all around the workshop in parts but I’m defo keen to resurrect them soon.

Keep up the awesome work bro - so good to see an update from you 😍
```

---
## \#530 Posted by: TowerCrisis Posted at: 2018-09-18T12:33:29.706Z Reads: 186

```
Is there a reason you're not using nylon or another material for the wheel gear? Also, is this 20dp?
```

---
## \#531 Posted by: rich Posted at: 2018-09-18T12:59:36.592Z Reads: 197

```
Thanks bro, looking forward to silent ghost rides :grin: 
I plan to make a direct comparison video of both gears with equal setup (same motors, same camera).

I know how time consuming this building is.... Just a quick fix, you think it's a 10 minutes job and 3 hours later you are done (like me soldering some wires yesterday). I have no wife or kids and even then everything takes forever.


It's getting dark earlier and I need some serious lights. Yesterday I tested my 18W 12V lights for the very first time. It is awesome and so bright, pefect for absolute darkness. I have a flood and a spot version but I prefer the spot version, it shines about 50-100 meters (150-300 feet) :laughing: best visibility within 20-30 meters. But very annoying for other people, looks like a small motorcycle is appearing.

Made a 3s1p with VTC5 cells and BMS for powering this light. Planning to mount everything to a bull bar. I have to experiment with height before I decide about final enclosure for the battery and on/off switches. Gonna add a second weak light when there are people around and 1-2 lasers as well.

![144218h|690x388](upload://5P8XD1Mueq97qTkCQBqoiKhU67N.jpeg) 

Here the link for the light, it's metal not plastic but I don't know how it handles heavy vibrations yet: https://www.aliexpress.com/item/1Pcs-2Pcs-18w-DRL-LED-Spot-Flood-Work-Light-Worklight-9-32V-4WD-12-volt-led/32835112621.html

[quote="TowerCrisis, post:530, topic:45377, full:true"]
Is there a reason you’re not using nylon or another material for the wheel gear? Also, is this 20dp?
[/quote]

No idea, @Duffman or @Nowind should know, these are helicals from E-Toxx.
```

---
## \#532 Posted by: janpom Posted at: 2018-09-18T13:10:51.230Z Reads: 189

```
[quote="rich, post:531, topic:45377"]
Just a quick fix, you think it’s a 10 minutes job and 3 hours later you are done (like me soldering some wires yesterday).
[/quote]

Hehe. I know that oh so well. Plus, I do have wife and kids. Fortunately, I'm just taking some longish time off work. Otherwise, I don't know when I would ever find the time to finish my build. :smile:
```

---
## \#533 Posted by: telnoi Posted at: 2018-09-18T14:04:20.287Z Reads: 186

```
How will you prepare the motors for an axial load?
I think I will go helical too after the current gears are done for. My wife bought an e-mtb (mountain bike) and complains about the noise I make :stuck_out_tongue:

PS. I just stick a light to my helmet using a gopro mount. Nothing beats being able to see the direction you are actually looking, though it looks stupid as hell.
```

---
## \#534 Posted by: rich Posted at: 2018-09-18T16:18:53.828Z Reads: 194

```
[quote="telnoi, post:533, topic:45377"]
How will you prepare the motors for an axial load?
[/quote]

It's not much to do, first step is to use socket head screws with Loctite instead of the tiny grub screws which hold the shaft to the can. This way you can crank them down much harder…… well unfortunately on my motors are M3 grub screws and this was just a test fitting. Lesson of the day, do not overtighten

![015319e|690x388](upload://r7H26Em0psU7av8jJLxawemKFdh.jpeg) 


Second thing is to remove the circlip and add washers between motor and the gear so there is no gap. It's best to glue the gear with Loctite 648 or like in my case keyway with grubscrew (blue loctite) plus on the opposite side on the shaft some 648 or 641 retaining compound.

Loctite 648 is high strength and 641 medium strength (and easier to remove). I wanted to use 641 as well for the wheel bearings but I'm so confused. Locally Loctite 641 costs 65€ for 50ml, on ebay the same for 13€ from greece or estonia (with long delivery time). On amazon germany 10ml is 20€. There are many different bottle designs then there is Loctite imported from china. Is there fake Loctite existing? WTF I need this stuff right now!

[quote="telnoi, post:533, topic:45377"]
I just stick a light to my helmet using a gopro mount
[/quote]

Also good idea plus people (or security cams) don't see your face :+1:
```

---
## \#535 Posted by: telnoi Posted at: 2018-09-19T07:16:42.373Z Reads: 186

```
Thanks for the explanation. How have your motors been holding up by the way?

[quote="rich, post:534, topic:45377"]
Is there fake Loctite existing? WTF
[/quote]

For sure.

[quote="rich, post:528, topic:45377"]
In the future I’ll attach the hub to the wheel gear before adjusting the backlash.
[/quote]

That's how I aligned everything from the start + I had a feeling the gears would not be accurately aligned if you just drop the gear onto the shaft as indicated by Jens in his video tutorial. The attachment to the hub alone will most likely offset it due to potential manufacturing inaccuracies etc. Part of the wheel is plastic after all. The partial dependency on the wheel hub for alignment is probably the only negative thing of this gear drive compared to say the Kaly drive (gear bearing not pressed against axle, wobble of wheel hub transfers to gear directly).

Adding loctite to that bearing seems like a good idea. Got a feeling it shifts around a bit/generates noise.
```

---
## \#536 Posted by: rich Posted at: 2018-09-19T12:45:44.050Z Reads: 189

```
[quote="telnoi, post:535, topic:45377"]
How have your motors been holding up by the way?
[/quote]

Let's say I had some bad luck so far. I really like the motors and they are powerful but not everlasting at least for me. One problem is that the cables can move inside the motor if you move them outside which leads to internal shorts that's why it's important to decrease the strain to 0% and route them on the hanger (or fix it with sugru on the motor). I am really happy with the customer service of Unikboards because I got replacements very fast. 

The sealed can is very nice and nothing can enter, on the other side the motors definitely run hotter compared to open motors. It's like everything in life, nothing is perfect and you can't have it all.

Just for demonstration, here you can see why the cables move (there is no protection beside one heat shrink tube for all which I removed for the pic) 

![003922|690x388](upload://73fh0dpSSKmfMbZRPnWo1KDfTp5.jpg) 

Compared to an APS motor where each wire is protected and can't move inside motor. BTW APS motors are very loud in FOC.

![221441|690x388](upload://8Q2uDnujSMGfhAgPbcO8DPN1h6l.jpg) 

[quote="telnoi, post:535, topic:45377"]
Adding loctite to that bearing seems like a good idea
[/quote]

Sounds good but how you remove the bearing when replacing? Blow torch? :rofl:

Damn I had a nasty crash yesterday evening with my carver where I destroyed the front truck and hurt myself so I'm not sure yet when I can ride again.

![212430h|690x388](upload://hitf9ltJDW0gWNhqvKcDvGYmodc.jpeg) ![203720h|690x388](upload://xoL4koIo1lNapdZGOBcI16bq7dp.jpeg)
```

---
## \#537 Posted by: telnoi Posted at: 2018-09-21T12:38:25.225Z Reads: 181

```
Thanks for the motor feedback.

[quote="rich, post:536, topic:45377"]
Sounds good but how you remove the bearing when replacing? Blow torch? :rofl:
[/quote]

Did they require replacing before the gear started cracking? 
Ordered some stainless steel replacement bearings now (for everything), my wheels have some unwanted movement after around 3800 km.
```

---
## \#538 Posted by: rich Posted at: 2018-09-21T13:04:53.710Z Reads: 178

```
The bearings are fine but my wheel bearings are always done after a few hundred kilometers. I changed the bearings 3-4 times already and now after 350km they start sound bad again, clicking and grinding noises. I'm sure this is because of the massive play inside the spokes that's why I want to try retaining compound. 

My dream is to have rattle free wheels with longer lasting bearings.....
```

---
## \#539 Posted by: ArnhemAnt Posted at: 2018-09-21T21:20:35.911Z Reads: 171

```
[quote="rich, post:538, topic:45377"]
My dream is to have rattle free wheels with longer lasting bearings…
[/quote]

From what I understand, the only way to achieve this is to switch over to MBS??
```

---
## \#540 Posted by: rich Posted at: 2018-09-21T22:08:14.553Z Reads: 172

```
From what I've read MBS have a too tight fit :laughing:

I can't switch hubs because of the drivetrains but I guess retaining compound will solve the problem. I'll do it for science
```

---
## \#541 Posted by: telnoi Posted at: 2018-09-29T16:09:16.458Z Reads: 179

```
[quote="rich, post:538, topic:45377"]
The bearings are fine but my wheel bearings are always done after a few hundred kilometers. I changed the bearings 3-4 times already and now after 350km they start sound bad again, clicking and grinding noises. I’m sure this is because of the massive play inside the spokes that’s why I want to try retaining compound.
[/quote]

Replaced all bearings today and they were equally messed up, including the gear bearings. The gears outlive the bearings in my case, so I won't be fixating them with glue.

Regarding skid pads, finally had the time to print them. Should have added them from the start. Turns the gear drive trampa back into all terrain instead of street/minor off-road capabilities. No more need for 9 inch wheels.
```

---
## \#542 Posted by: rich Posted at: 2018-09-29T18:14:55.523Z Reads: 185

```
My gear bearings are still fine after 1000km. The problem is that the wheel bearings don't fully touch the hub, therefore they wiggle. Also all the forces get mainly transmitted through 2 areas and not the whole bearing seat as you can see in the picture

![224449|690x388](upload://g6LIuohs14zGq864xF9mL26X3VW.jpg) 

That's why I'll try Loctite 641 which is made for this purpose. It's medium strength and should be not too difficult to remove, don't know but look here

![641|573x248](upload://zPCGyGdSCd50mGLGEqeODZLLu5v.png) 


Loctite 638 is high strength and I'll use a little bit on the helical motor gear opposite to the keyway. 

![638|575x287](upload://q1yGqww0Js4wkAocoD3ploZKvlN.png) 

[quote="telnoi, post:541, topic:45377"]
Regarding skid pads, finally had the time to print them
[/quote]

Already mounted? pics? :grin:
```

---
## \#543 Posted by: rich Posted at: 2018-10-02T11:22:48.329Z Reads: 190

```
Unfortunately the progress is very slow because my shoulder starts hurting when I lift or build something. Anyway the show must go on, finally mounted the motor plates on the Infinity hanger, added sugru and prepared a new baseplate.

![152253h|690x388](upload://47OgM1B3i70a4xqOEJEUld21aip.jpeg) 
![152540h|690x388](upload://5JWYXYQtPZmoTqi9WYGpnobpvzk.jpeg) 

But then the disaster started, for the helicals I wanted to remove the grub screws of the motors and replace with socket head ones. They didn't move at all and both are stripped now (of one motor). On the spare bell I could remove them without resistance. Like always: 1 step forward, 2 steps back :face_with_raised_eyebrow:
```

---
## \#544 Posted by: rich Posted at: 2018-10-04T20:50:30.640Z Reads: 187

```
I had to make a decision about the motors because I can't use the Unik motors with stripped grub screws for Helicals so they can rest and have to wait for another project. The grub screws are still tightened just stripped.

I decided to use my emergency motors which arrived from Hong Kong a couple of days ago, Turnigy SK8 149kv. They are huge, the motor length is 89mm (without the nipple 80.5mm) and weigh 0.986kg.

![141403h|690x388](upload://itpR3AWVp79vULFrjfb3WJwcNMT.jpeg) 
![142233h|690x388](upload://hZafWemqiGLkHME4X3zJMOHUX9Z.jpeg) 


Shaft is 38.5mm :astonished:


![153521h|690x388](upload://uyp0coatzPKxzkF5MFD0iNlSRO7.jpeg) 

It's time to make some noise

![172841h|690x388](upload://f0D9Vo82M5Bi9p4UoeYMzitksCq.jpeg) 
![195843h|690x388](upload://cA1Y1wnUBccUrat030AU8r6mWiv.jpeg) 
![195954h|690x388](upload://zfBXNVuNaSpsKKHZuSii2JUQQUf.jpeg) 
![210936h|690x388](upload://iXxLjVG0wpbAtKDrZ7TyAyAsYkO.jpeg) 

Picked up my fresh black anodized bull bars today :star_struck:

![202238h|690x388](upload://1G9y2A7saRd9xZc1XkBr6iz95QR.jpeg) 

Then I was shocked because the bull bar touched the motors when holding by hand but after mounting it looks I'm lucky.

![192845h|690x388](upload://x1JV0XC6thJdwl5RmVbsQtKr5Lh.jpeg) 
![193350h|690x388](upload://uYQbeuQCY96shmMChsNEWIr1Yy3.jpeg) 

My plan was to mount the cables with zip ties to the bull bar (left and right at the hanger) before routing them to the top. I have to rethink it, the big motors are so close plus the edges of the channels are like razor blades.

![193742h|690x388](upload://pEvXZzczxjhBqkwZdeFajSIybbh.jpeg)
```

---
## \#545 Posted by: ArnhemAnt Posted at: 2018-10-05T00:37:33.912Z Reads: 181

```
Man, that is a very tight fit between the motors and bull bars. You sure they won't rub once you riding?
```

---
## \#546 Posted by: Andy87 Posted at: 2018-10-05T05:05:55.361Z Reads: 181

```
What if you add two washers between your hanger and the pull bar. Could give some more space for the motors than.
```

---
## \#547 Posted by: rich Posted at: 2018-10-05T09:08:00.656Z Reads: 181

```
[quote="ArnhemAnt, post:545, topic:45377"]
You sure they won’t rub once you riding?
[/quote]


I'll tell you once I'm riding :laughing:

It looks a bit closer in the pics because they were shot more fom top and not from the side. When the motors are in the final position I'll triple check all distances, no doubt.

[quote="Andy87, post:546, topic:45377"]
What if you add two washers
[/quote]

Good idea for the worst case :grin:
```

---
## \#548 Posted by: Silverline Posted at: 2018-10-05T09:51:49.709Z Reads: 189

```
I had to cut the collar in length, i guess you did the same thing ?
https://cdn-global-hk.hobbyking.com/media/catalog/product/cache/1/image/660x415/17f82f742ffe127f42dca9de82fb58b1/1/8/188909-189049_2_10.jpg

Do you happen to know, where to get new ones ? They are kind of special, and only 0.5mm thick...

Looking forward to hear, what you think about sk8 :-)
```

---
## \#549 Posted by: rich Posted at: 2018-10-05T11:21:49.390Z Reads: 195

```
Yes, didn't know first how to cut it straight. In the end I slided it on a 8mm aluminium tube and cut both tubes.

![145324h|690x388](upload://bGH5bVI5klyDFm47OwrbUHZ7tm6.jpeg) 
![150452h|690x388](upload://pENbiFn5KHguoPir0y0NEmgP0KB.jpeg) 

It's not perfect and I need  a 0.2mm washer which I don't have yet.

[quote="Silverline, post:548, topic:45377"]
Do you happen to know, where to get new ones ? They are kind of special, and only 0.5mm thick…
[/quote]

Thanks for reminding me to buy those. Trampa sells them in 6.5mm length, so it sticks out 0.5mm.

http://www.trampaboards.com/8-x-10-x-65mm-brass-shim-spacer--slips-on-the-motor-axle-to-align-motor-pulley-p-25938.html

I think with the side loads of the helicals it's better to use 100% flat and accurate spacers. I wanted to do it quick and dirty by cutting the original one but in the end it should be perfect not almost.

Furthermore I ordered kingpins and the following washers which are great for any motor

http://www.trampaboards.com/8-x-10-x-05mm-brass-shim-spacer--positions-motor-pulley-in-perfect-position-p-25937.html

http://www.trampaboards.com/8-x-14-x-02mm-precision-shim-washer-marine-grade-stainless-steel-used-to-take-up-any-tolerance-when-mounting-to-motor-to-the-motor-shaft--p-13026.html

http://www.trampaboards.com/8-x-14-x-05mm-precision-shim-washer-marine-grade-stainless-steel-used-to-take-up-any-tolerance-when-mounting-to-motor-to-the-motor-shaft-p-13025.html

http://www.trampaboards.com/10-x-16-x-02mm-precision-shim-washer-marine-grade-stainless-steel-used-to-take-up-any-tolerance--p-25764.html
```

---
## \#550 Posted by: Silverline Posted at: 2018-10-05T13:16:26.188Z Reads: 170

```
Thanks for the awesome links. 

I used my cordless drill, and hold my hacksaw against the collar , while it was turning around. Perfect cut :slightly_smiling_face:
```

---
## \#551 Posted by: rich Posted at: 2018-10-05T15:03:20.930Z Reads: 167

```
Damn, much better solution, next time I'll do it like that :+1:
```

---
## \#552 Posted by: Silverline Posted at: 2018-10-05T16:09:00.289Z Reads: 183

```
Regarding this : http://www.trampaboards.com/8-x-10-x-65mm-brass-shim-spacer--slips-on-the-motor-axle-to-align-motor-pulley-p-25938.html

The text on the pictures says 8 x 10 x 6.5mm, but in the text under the picture, it says 12 x 15 x 1 mm :rofl:

I believe its 8 x 10 x 6.5mm.... But do you think this will fit ? Because the ones that comes with the motor is 8 x 9mm....
```

---
## \#553 Posted by: rich Posted at: 2018-10-05T16:40:21.715Z Reads: 192

```
[quote="Silverline, post:552, topic:45377"]
The text on the pictures says 8 x 10 x 6.5mm, but in the text under the picture, it says 12 x 15 x 1 mm :rofl:
[/quote]

I know they write OD 10mm but it's not.
Forget the text, maybe it says stainless steel, too.
There are products where I find 4 different sizes for the same product. On Trampa page many things are mixed up. I got used to it and waiting for my surprise parcel.

[quote="Silverline, post:552, topic:45377"]
I believe its 8 x 10 x 6.5mm…
[/quote]

I had Trampa motors which look very similar to SK8 using the same brass tube as Turnigy  just shorter so it must be the same. 

My theory is that the chinese factory (probably SunRay) which produces Trampa motors (and SK 3) took the same design for the new SK8 motors. The can is different but the rest looks equal, even the shaft is 38.5mm on both motors and Turnigy even cloned the Trampa motor axle support bearing housing, the only reason for this ultra long shaft. Also they sound equal when spinning. IMO the same just different, Trampa says their motors are hand-wound, don't know about SK8.
```

---
## \#554 Posted by: Silverline Posted at: 2018-10-05T17:16:25.549Z Reads: 182

```
Wow this is very very good info, thanks......

I will order those brassers then.... thanks again
```

---
## \#555 Posted by: telnoi Posted at: 2018-10-09T09:07:04.166Z Reads: 190

```
[quote="rich, post:521, topic:45377"]
14 days after ordering I received the cheap tires from aliexpress today.

[![115203|690x388](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/3/a/3a5fee54609be1a01eaf8358e4f4d8afde062aed_1_690x388.jpg)
115203.jpg3264x1836 317 KB
](https://www.electric-skateboard.builders/uploads/db1493/original/3X/3/a/3a5fee54609be1a01eaf8358e4f4d8afde062aed.jpg)

Looks equal to MBS Vine but they are made of different more rigid nylon material which has less grip and is heavier. Could be that this tire is flatproof :laughing:
[/quote]

I also received mine today. They are identical to the awesome long-lasting tires that were on my old mountain board/exact same brand (clever). The pressure rating has been changed to 60 instead of 80. I safely inflated these to 70 in the past, but if they are punctured the inner lining will unravel and the tire will begin to bulge. This won't happen if you stay around 50. Also makes for a more comfy ride (you can go lower on pressure compared to other tires due to the stiffness of these things, also increases grip).

There is no center ridge left on mine now...after 2500 km. :rofl:

[quote="rich, post:542, topic:45377"]
Already mounted? pics?
[/quote]

Soon. Needs some changes. Fit is not precise/downside of not having the cad files, seems my diameter measurement for the enclosure was off by a few mm.
```

---
## \#556 Posted by: rich Posted at: 2018-10-11T18:17:45.609Z Reads: 191

```
Good info about the tires, will mount them in a couple of weeks...

[quote="telnoi, post:555, topic:45377"]
if they are punctured the inner lining will unravel and the tire will begin to bulge
[/quote]

I remember when you posted this picture :rofl: 

![2b2437ac2c406cfe68bd81e54b03b30e349906e0_1_375x500|375x500](upload://wiVpGZDzXAahSadRk2nnlb4W0Hf.jpg) 

Finally I know the date when I gonna ride my "new" board after a very long break, it's on saturday :sunglasses:

Damn I'm sooooo curious about the helicals and also the motors, it's like christmas.

Received the 6.5mm brass tubes and spacers for the motors.

![191758|690x388](upload://oYFu4VGsNM6ipnIaiulHiuo9BSF.jpeg) 
![192431|690x388](upload://7QNcdJ6lV51bEwjqwBaFjeIs9GB.jpeg) 

It's very close but nothing is rubbing

![193012|690x388](upload://h5h58TFeDhOo6H2ufZRVBbo3d3p.jpeg) 

I ordered all kind of screws for 30€ but the Unikmotors had M3 grub screws so I had no M4x6mm for the SK8's. I use 10mm socket head bolts instead and because there is only one I glued them to the shaft and thread with Loctite 638, that should hold :wink:

![112257h|690x388](upload://kTS5RgmBoiwGHfC6Ccvte8UdsG6.jpeg) 

I would call this the point of no return

![000842|690x388](upload://7l9lXnwmbqw4fyJWkPwulcqZ8m3.jpeg) 

48 hours cure :face_with_raised_eyebrow:

![185341|690x388](upload://32U7b6iA67qjjBKIGJyhcY9aQRL.jpeg) 

Added  phase wires and heat shrinked all connectors, next step is soldering the other connectors and sensor wires and add wire mesh

![190335|690x388](upload://aM8Vg1OqOhEOIjWGzU1M6GTwqgp.jpeg) 

Unlike most others (I guess) I love how the cables come out of the motor, perfect for routing on the hanger and no more cable loops, unexpected surprise. 

Because of the length of the motors the cables are mounted very very close to the motors which is tricky. To achieve absolute no movement in the wires I made a construction which holds the cables in place, more pics gonna follow soon.

![200920|690x388](upload://bpC69TAOLGtKGYCy42bqf8BmVxz.jpeg)

And yeah I used some foil on the motors, the blue and silver hurts my eyes on a dark setup :laughing:
```

---
## \#557 Posted by: ArnhemAnt Posted at: 2018-10-11T20:51:59.642Z Reads: 190

```
[quote="rich, post:556, topic:45377"]
Finally I know the date when I gonna ride my “new” board after a very long break, it’s on saturday
[/quote]


Nice one bro. Bring on Saturday and hope you have a safe ride on the new beast. Loving the updates you have done and can't wait to see more pics when it all comes together.

My board is currently out of action - dropped a cell in the battery pack, so I'm having the pack rebuilt. The downtime has allowed me to make a few minor tweaks to help kill the waiting time.
```

---
## \#558 Posted by: rich Posted at: 2018-10-13T13:47:25.472Z Reads: 191

```
Today is the day of rebirth, ready to ride :sunglasses:

Finished everything at 5am and fell asleep, totally forgot to charge the battery but shouldn&rsquo;t take too long from now.

Why this soldering takes always so long, just 18 wires :thinking:

![030948|690x388](upload://9HRUzZKgxMkifJ0OGTXmP4JvsHC.jpeg) 

Also fixed some other things. I lost one bolt holding the Pelicase so I also could inspect the battery and damn it&rsquo;s a bit swollen not as bad as my old puffed Graphenes but nothing I&rsquo;ve expected after 1000km. But I have no idea when I should stop using this pack. It is wrapped in gaffa tape which is not flexible at all so the forces must be huge to stretch it.

![202824|690x388](upload://5FJK1AoxdHk1TvSIxmg5vEN9eQy.jpeg) 

I use tire sealant inside my tubes against flats which works great but unfortunately it&rsquo;s absolutely impossible to counter balance the wheels with this stuff. So I cut the valve including the enforced rubber of one tube for science to measure the weight, it&rsquo;s 16-17gr so about 4x5gr balance weights opposite to the valve and the valve wobble is gone.

![152801|690x388](upload://oEPPpeyQ7pl3sdtJAsPMKebBdnE.jpeg) 

The MBS Vine tires are quite unbalanced that&rsquo;s why I had to add or shift the counter balance weights by try and error. I took an extra hanger (holding/laying in the hand) and changed the weights until the wobble and vibrations were gone.

It&rsquo;s quite tight inside the rear enclosure but I could close it, all good.

![134620|690x388](upload://tQ6PQ7xjzLj9DwfLZFOSMd6JRWl.jpeg) 

Because of my heavy abuse before using the drive guards I have some signs of usage on the drivetrain :laughing:

This is e.g. from ollie up a sidewalk with too low speed and land on the drivetrain(s) only on the curb, this happens more often than I like. Also sometimes I land with full weight on one drivetrain and also once I slided some meters with one drivetrain  on a cobblestone curb before crashing. I can't kill this drivetrain

![141506|690x388](upload://w1XnY7Dt9pXhkc2zxREajTUIvHS.jpeg) 

But I recognized that due to the abuse on some spots material at the edges stick out a bit on the motor plate and the POM housing.

![141432hE|690x388](upload://yXHkJzY3wxxpI511YMD3yrMLRMa.jpeg) 
![213849|690x388](upload://hPGzYcy7g1q9m5X8Nulgy1sbFvt.jpeg) 

For the aluminium I used a fine file and for the housing sand paper. Now everything is like new again and solid sealed with the straight edges (no gaps).

![140552|690x388](upload://yXQPsvap8uOuhLPjc89l52PKXTm.jpeg) 

Damn I like the clean look

![152417|690x388](upload://sWMN0YkzORHgues5dypo3c39dug.jpeg) 

Wait, where are the cables? :laughing:

![152547|690x388](upload://1PuGFtxcZ9RclUh3PYZiYpodtB2.jpeg) 

Zip ties with shrink tube for better grip and protection mounted to the bull bar. The Infinity hanger has no holes like Vertigo so another reasoin for the bull bar.

![152454|690x388](upload://58PC3JipkxErR2CTCoZZ7nVL6w6.jpeg) 




Hehe, my battery is full and I need to go for a ride soon, I'll let you know about my first impressions

[quote="ArnhemAnt, post:557, topic:45377"]
My board is currently out of action - dropped a cell in the battery pack
[/quote]

Damn bro, hope you can ride again very soon :pray:.
```

---
## \#559 Posted by: Silverline Posted at: 2018-10-13T13:57:19.640Z Reads: 183

```
Damn.... that is one sexy ass you got there :sunglasses::heart_eyes:
```

---
## \#560 Posted by: Riako Posted at: 2018-10-13T14:34:37.919Z Reads: 187

```
Wow bro ! This is some good level up finish details !!! :P So clean !!
Fall in love with your ass too :smile:
 
:v: Enjoy !!

PS : how did you complete the streaks of the sk8 ?! :face_with_monocle:
```

---
## \#561 Posted by: telnoi Posted at: 2018-10-13T14:58:35.429Z Reads: 190

```
[quote="rich, post:556, topic:45377"]
I remember when you posted this picture
[/quote]

Big fat thorn. 
Some more fun pics. 
This is how far you can run them down. Probably still has a few rides left in it. This is 3500 km. 

![IMG_20181013_165430|375x500](upload://1WWT6SZArUhCxShLzVuTAe2oXIv.jpeg)

VS this T3. Already a flat and it always happens when the center tiny indented ridge is almost gone. This is 300 km. 

![IMG_20181013_165444|375x500](upload://vMHl920vIvTFifXL79nASiJRVD6.jpeg)
```

---
## \#562 Posted by: Riako Posted at: 2018-10-13T15:03:09.927Z Reads: 179

```
Dam ... that goes fast ... esk8 with air tire will coast almost as petrol commute this way :smile:
We need a real brand sharing his formula on this little size tire ! (Hope one of them is reading this !)
```

---
## \#563 Posted by: telnoi Posted at: 2018-10-13T17:29:46.831Z Reads: 175

```
I laugh at those Porsche (Cayenne) drivers around here. They've got it easy. 

MTB for daily commuting is in fact more expensive than a car for me...but it's also allot more fun and cars make me fat. Previously it was belts and pulleys and tires. With the Jens drive that has been reduced to just tires and the occasional gear change (estimate once every 1.5 years). Ah, yes...and lipo packs are done after one year.
```

---
## \#564 Posted by: rich Posted at: 2018-10-13T19:49:02.128Z Reads: 190

```
I am back from my journey and wow the helicals are great and I hear things that I've never heard before, like how the tires sound when rolling on different terrains or my front bushings :smile:

[quote="Silverline, post:559, topic:45377"]
that is one sexy ass you got there :sunglasses::heart_eyes:
[/quote]

[quote="Riako, post:560, topic:45377"]
Fall in love with your ass too :smile:
[/quote]

Haha glad you like the ass so I'm sure you like the dirty ass too

![172708|690x388](upload://kC4zdAUFyXFNYmPQGWalLKb4uj.jpeg) 

I had a lot of fun for 10km until I sliced a tire and got a flat in the middle of nowhere. It took a while to get home, thought with tire sealant it's flat proof

I have to ride more to judge about the motors but I think they are good. I realized that I need more throttle to get the same punch as before but they are still powerful. Need to ride on places which I know better and also uphill. The app said I've used 150A motor max :grin:

Here raw footage of my ride which ends with wipe outs and the flat. I started to give a lot of throttle (short impulses) in tight curves for short drifting but you don't hear it so you may think why is this dude falling.

Silent madness 
https://www.youtube.com/watch?v=aSr2WLeUODM
```

---
## \#565 Posted by: Silverline Posted at: 2018-10-13T20:08:59.336Z Reads: 178

```
Yes like i also noticed. They do feel more linear , and not so punchy from stand still , like other motors may do. But i do think, in the end, that they perform greate.
They have a good wh/km(or miles) i think it's because they have curved magnets. 

With all those rocks you have on the road, i can understand why you have a flat tire 😊
```

---
## \#566 Posted by: rich Posted at: 2018-10-13T21:05:42.201Z Reads: 190

```
[quote="Riako, post:560, topic:45377"]
how did you complete the streaks of the sk8 ?! :face_with_monocle:
[/quote]

What do you mean with streaks?

[quote="telnoi, post:561, topic:45377"]
This is how far you can run them down. Probably still has a few rides left in it
[/quote]

Damn, better not try to use these again :stuck_out_tongue_winking_eye:

[quote="Silverline, post:565, topic:45377"]
They do feel more linear
[/quote]

yeah good description

[quote="Silverline, post:565, topic:45377"]
With all those rocks you have on the road, i can understand why you have a flat tire :blush:
[/quote]

Haha true but this is the first flat since I use tire sealant which normally prevents flats (and works like a charm).

I love the self locking threaded inserts on the helicals so I can go for a night ride after changing the tube. I've inspected the tire but I can't find any damage so I try it with a new tube and spare wheel in backpack.

Haha this drive guard looked different when it was originally mounted :thinking:

![191349|690x388](upload://zTiFfgLDFMNmo6KwhJ3CknXsnEj.jpeg)
```

---
## \#567 Posted by: Riako Posted at: 2018-10-13T21:34:12.267Z Reads: 189

```
[quote="rich, post:564, topic:45377"]
Silent madness
[/quote]
:star_struck: insaaaaane !!!
And wow, what a ride, this is a hard dust shredding !! With a lot of fun ... but maybe not at the end ^^
[quote="rich, post:566, topic:45377"]
What do you mean with streaks?
[/quote]

Sorry bad google translate apparently ^^
a picture is worth a thousand words :blush: : 
![Capturecan|690x393](upload://tchUcZHt8YfiuS0q3Dwg3xQELNH.jpeg)
```

---
## \#568 Posted by: rich Posted at: 2018-10-13T21:46:49.500Z Reads: 183

```
Ah no the word streak makes sense :laughing:

I just put foil there without any modifications. I guess the gooves (sorry the streaks) are made for cooling. I have to watch the motor temperature, maybe I have to remove the foil in summer.
```

---
## \#569 Posted by: ArnhemAnt Posted at: 2018-10-13T21:58:02.335Z Reads: 174

```
Awesome to see you back on the board man. Again, your documentation of what you are doing at each stage, with pics, is an absolute asset to this forum and members, like me really appreciate the time and effort that you put into your posts.
I can't believe just how quiet the board is now with the helical gears. One day, when I have enough 'spare' money, I will upgrade, but for now I'll stick with the standard gears on my drives.
```

---
## \#570 Posted by: rich Posted at: 2018-10-13T22:49:35.156Z Reads: 192

```
Thanks for your kind words mate , that means a lot for me :blush:

I like sharing knowledge, also I've learnt many things from members like you e.g. that riding barefoot is an option :wink:

[quote="ArnhemAnt, post:569, topic:45377"]
but for now I’ll stick with the standard gears on my drives
[/quote]

yeah I like both gears, the only difference is the sound. With the straight cut gears it sounds like a machine which is also nice. With helicals it's still a machine but doesn't sound like one, more like an e-bike :laughing:

I live in the city and going for a night ride now without disturbing the neighbours. Changed the tube and also prepared a spare wheel. The bearings I have to put seperately because the fall of when moving the wheel. Mounted a bicycle rear light to the bull bar

![003005|690x388](upload://lwif9bhMofS3TvseV1NaOKAB65A.jpeg) 
![234550|690x388](upload://rcaozTP1iN53y564DMs8qX9sprX.jpeg)
```

---
## \#571 Posted by: rich Posted at: 2018-10-14T00:44:31.054Z Reads: 190

```
This night ride was a lot of fun but maybe I should rather sleep at night because I trampinated my front hanger :face_with_raised_eyebrow:

![022632|690x388](upload://hfaZzur4qmByFQxEXbW7tt9OHkq.jpeg) 

I didn't see the snag in the grass and shaved the hanger a bit, also hit it with the rear hanger but no damage there. But it shouldn't be a problem, it's more aesthetic.
```

---
## \#572 Posted by: ArnhemAnt Posted at: 2018-10-14T01:15:57.837Z Reads: 185

```
Woah - what sort of snag did you hit? Looks like a solid rock to do that sort of damage.
```

---
## \#573 Posted by: telnoi Posted at: 2018-10-14T13:22:03.275Z Reads: 190

```
Let's see what Jens will come up with. Tpu truck sleeve.

Stranded. Waiting for taxi aka wife. Get a keyway if you can people. 
![IMG_20181014_152311|690x343](upload://zr177iVxvoKemJyO60SQKddLkDM.jpeg)
```

---
## \#574 Posted by: rich Posted at: 2018-10-14T15:12:37.401Z Reads: 190

```
[quote="ArnhemAnt, post:572, topic:45377"]
Woah - what sort of snag did you hit?
[/quote]

Evil austrian wood :laughing:

[quote="telnoi, post:573, topic:45377"]
Tpu truck sleeve
[/quote]

:rofl:

[quote="telnoi, post:573, topic:45377"]
Stranded. Waiting for taxi aka wife. Get a keyway if you can people.
[/quote]

Damn when I stranded yesterday I had neither a taxi aka wife nor a real taxi. Also nobody wants to carry a dusty board and guy.

Do you use blue Loctite only on grub screw? I don't like keyways anymore, lack of precision everytime
```

---
## \#575 Posted by: telnoi Posted at: 2018-10-14T16:20:52.665Z Reads: 188

```
[quote="rich, post:574, topic:45377"]
Do you use blue Loctite only on grub screw
[/quote]

Only loctite 601, no key no grub.
Degreased everything with a variety of different products, roughed up the motor axis + gear on the inside and stuck it all together again with 601. The other side was treated in a  similar way after it broke loose and has held up. The gear that broke loose today was not degreased/not roughed up when I first installed it. Lesson learned.
```

---
## \#576 Posted by: Pedrodemio Posted at: 2018-10-14T16:42:06.139Z Reads: 179

```
That’s the best combo I tried so far, Loctite and keyway, easy to remove and no rattling
```

---
## \#577 Posted by: rich Posted at: 2018-10-14T17:49:43.548Z Reads: 193

```
I had my third ride today and felt like a ghost. It's so quiet that nobody turn around and even dogs don't bark at me. I am thinking about to carry a bicycle bell to get some attention :laughing: or a bluetooth speaker.

I love this gears :smiling_face_with_three_hearts: and also with the new motors it feels like a new board. Also had a session at BMX course today and did some jumps, everything survived.

@Nowind I didn't know the bull bars are so versatile. I wanted to protect the motors when crashing in something backward again (hopefully not). Yesterday I made a too big step and the bull bar saved the motor from my foot. Today I used the vacuum cleaner and heard a loud impact, the bull bars are great!

![170245h|690x388](upload://fsjzv35ofDVymwJk7n15uYF6N4r.jpeg) 


[quote="telnoi, post:575, topic:45377"]
The gear that broke loose today was not degreased/not roughed up when I first installed it.
[/quote]

Roughed up? 
I didn't, only degreased everything, hope it holds :pray:

[quote="Pedrodemio, post:576, topic:45377"]
Loctite and keyway, easy to remove and no rattling
[/quote]

All the motors I had/have (except 1) had a too wide keyway on the shaft (or on the pulley) so the key rattles and if the grub screw is on the opposite side on the rounded shaft it lasts not long. I added kapton tape to get a tight fit which worked but not forever. If key and keyways are one unity it's perfect. I thought about to glue the key to the keyway of the shaft but ended up with Loctite 638 only.
```

---
## \#578 Posted by: Pedrodemio Posted at: 2018-10-14T21:11:01.271Z Reads: 181

```
Nice save from the vacuum, the damage would be catastrophic!

About the key, I have a hard time trusting just the loctite, even more when it gets to decide if I can brake or not
```

---
## \#579 Posted by: rich Posted at: 2018-10-25T22:10:57.034Z Reads: 188

```
Time for some updates, good and bad news.

Meanwhile I was jumping in dirt park and on bmx course and riding different terrains and hills. The motors don't get hot and I got used to them. Also did hill climbing tests where I climbed insane 21-25°. But starting from standstill is not possible, only wheelspin. On this incline the motor max was only 90A and batt max. 45A.

![181716|690x388](upload://f34U00HVxdHvF8evr7aCIvx0kdP.jpeg) ![181908|690x388](upload://yu4hsUVGiUnJvZUZWWVq9JhalSI.jpeg) 

Now the bad news, one motor sounds bad after about 80-100km only! Unfortunately I know this sound and also know that I have 2-5 rides left until it's useless. What a shame! I ordered the motors from Hobbyking in Hong Kong and also cut the shafts so I don't know if there is any warranty. Need to contact them.

Tomorrow I go for a ride and check the sound afterwards, now it sounds like that:

https://youtu.be/1QkKpFBX7ec
```

---
## \#580 Posted by: Pedrodemio Posted at: 2018-10-25T23:16:44.172Z Reads: 186

```
Do you know what's broken? If it's bearing you can just put high quality ones, I did that in every motor I've owned so far since even the ones that are supposed to be genuine NSK/SKF/Nachi goes bad way too soon

And the noise was very similar to that
```

---
## \#581 Posted by: rich Posted at: 2018-10-26T00:08:29.718Z Reads: 185

```
[quote="Pedrodemio, post:580, topic:45377"]
And the noise was very similar to that
[/quote]

Interesting, for me it sounds like something is rubbing on the can or stator. When I had this problem with a different motor it sounded like that and after a couple of rides 10 times louder plus resistance.

But the real esk8 nightmare I have with my other build, much worse. Both builds have motor problems right now, it's so disappointing :disappointed_relieved:.
```

---
## \#582 Posted by: Pedrodemio Posted at: 2018-10-26T01:51:48.448Z Reads: 182

```
Best thing is to open them up and take a look, spin each bearing with fingers or inserting a screw drive to take the place of the shaft

Could also be loose magnets
```

---
## \#583 Posted by: rich Posted at: 2018-10-26T16:58:06.816Z Reads: 182

```
I'm afraid I have to open it but the motivation is not too big because I glued the gears :face_with_raised_eyebrow:

Had a ride today without problems but didn't check if the noise changed afterwards.
```

---
## \#584 Posted by: telnoi Posted at: 2018-11-03T18:59:02.359Z Reads: 187

```
Hmm, is this what destroyed your bushings? My old hanger was straight. The new one does not fit at a 90 degree angle with the baseplate/bushings.

PS. This is an entirely new truck, no mixed old & new parts.

![IMG_20181103_194417|375x500](upload://3FaLp0R65TQ34q9je748B7mdHbI.jpeg)
```

---
## \#585 Posted by: Andy87 Posted at: 2018-11-03T20:46:06.900Z Reads: 184

```
🤔 that makes me to check my trucks too when i‘m back home... 
looks not how it should be. Did you already ask frank about it?
```

---
## \#586 Posted by: telnoi Posted at: 2018-11-03T20:47:12.344Z Reads: 183

```
Sent Ted a message.

The holes in the hanger are drilled at different heights, enough to even decrease the angle of hanger compared to the deck or baseplate.
```

---
## \#587 Posted by: rich Posted at: 2018-11-03T21:05:06.165Z Reads: 189

```
[quote="telnoi, post:584, topic:45377"]
Hmm, is this what destroyed your bushings?
[/quote]

No it was the hole of the hanger, not the angle. With the new hanger which looks similar to yours I ride since 140km without problems. The angle is not 90° on the hanger but the hole for bushing and kingpin is straight and in line with the other hole. That's why the baseplate of your bushing looks crooked.

That's mine:

![124816|690x388](upload://lAiCwXIn6MnTtIjyAQYhA6Emkz2.jpg) 

for safety filled with sugru, don't know if it makes a difference

![124045|690x388](upload://bZcm9cedVnqSQvzFXznG2JoFK1p.jpeg) 

But my hanger was too much bent, that's why I need to use the biggest 3mm bushings plus a 1mm metal washer to fill the gap. Trampa has no 4mm bushings :face_with_raised_eyebrow:

Meanwhile I'm an expert in bushings, they have manufacturing tolerances. Best are 3mm bushings and 2.5mm. 2mm are OK but 1.5mm bushings are my enemies. They are too big outside and inside (diameter) therefore the kingpin has play and rattles inside the bushing.

[quote="telnoi, post:586, topic:45377"]
enough to even decrease the angle of hanger compared to the deck or baseplate.
[/quote]

Like my hanger :joy:
Is it a machined hanger or original? Because I didn't get replacement because of modifications. But good luck!

Meanwhile I had some rides and the motor sounds worse, I can hear it while riding now. I am trying to claim it but have no big hope because of the modifications. 

https://youtu.be/5tmVmGV5z3Y
```

---
## \#588 Posted by: telnoi Posted at: 2018-11-03T21:22:08.144Z Reads: 188

```
[quote="rich, post:587, topic:45377"]
No it was the hole of the hanger, not the angle. With the new hanger which looks similar to yours I ride since 140km without problems. The angle is not 90° on the hanger but the hole for bushing and kingpin is straight and in line with the other hole. That’s why the baseplate of your bushing looks crooked.

That’s mine:

[/quote]

Ok, that's different. If the holes are drilled in one go (thus at least the hanger bushings are always in line with the kingpin), the misalignment is going to be less of an issue. I have a benchmark though. My old bushings are still perfect after roughly 2000 km. It would suck incredibly badly if I end up changing them every odd sub 500 km mark.

[quote="rich, post:587, topic:45377"]
Like my hanger :joy:
Is it a machined hanger or original? Because I didn’t get replacement because of modifications. But good luck!
[/quote]

These are original/unaltered & never installed, straight out of the box that said ''battery tray.''
Replacement for the trampled front truck.

And these motor issues. Just frustrating man. I had high hopes for the SK8, seeing how the SK3 did so incredibly well.
```

---
## \#589 Posted by: rich Posted at: 2018-11-03T21:40:53.818Z Reads: 186

```
[quote="telnoi, post:588, topic:45377"]
My old bushings are still perfect after roughly 2000 km
[/quote]

unbelievable :smiling_face_with_three_hearts:
I am happy with 500km

[quote="telnoi, post:588, topic:45377"]
Replacement for the trampled front truck.
[/quote]

:rofl:
And you got a trampled hanger (hopefully paid by Trampler).

I forgot to write about my most weird esk8 experience ever which I recently had. It was getting dark and I kept on riding with a tiny light, not really enough to see anything. I was riding on gravel paths between trees and bushes quite slow. Nobody is walking there in the dark, only bicycles sometimes. However I heard strange music from far away like in a ghost movie. This music was coming closer and closer but there are no houses, only bushes and trees. Kinda scary, then I saw a person on the path. When I passed by I knew what it was, a woman playing a bagpipe in the dark WTF :joy: I had to laugh for a couple of minutes, that was a magic moment, crazy doodling woman.

Maybe her neighbours called the police several times already and now the only way to play the bagpipe is in dark nature. So funny.
```

---
## \#590 Posted by: ArnhemAnt Posted at: 2018-11-03T22:05:12.512Z Reads: 166

```
That didn't happen on the night of Halloween did it??
```

---
## \#591 Posted by: telnoi Posted at: 2018-11-05T08:47:06.985Z Reads: 176

```
[quote="rich, post:589, topic:45377"]
And you got a trampled hanger (hopefully paid by Trampler).
[/quote]

Frank replied on Sunday stating that the misaligned should not be cause for concern. The hanger can be replaced if it turns out to be an issue down the road. 

Can't fault their support.
```

---
## \#592 Posted by: rich Posted at: 2018-11-07T21:23:25.398Z Reads: 181

```
Skate parks are much more fun strapped to a mountainboard!
Last time with the Urban Burro I crashed and cracked the deck here at night.

https://youtu.be/JZM61Kdjc6s
```

---
## \#593 Posted by: janpom Posted at: 2018-11-07T22:10:07.734Z Reads: 182

```
Nice riding and cool vid! Looks like great fun.
```

---
## \#594 Posted by: rich Posted at: 2018-11-08T19:53:09.040Z Reads: 191

```
Wanted to go for a ride but couldn't switch the remote on so I had to disassemble it

![150219|690x388](upload://b2OBnNdtbNsKs0R9Jmm9to1W78I.jpeg) 

First of all I've expected some gold dust inside because it's so expensive but nothing. Now I know why I have to charge this remote all the time, Look at this tiny 200mAh cell compared to my little finger. It was additionally secured with 2 zip ties but 1 was broke 

![150131|690x388](upload://qvr7IKJG1j2a3FX9kqYSUiWbg4j.jpeg)  

I saw the problem of this stupid construction, the on/off button gets bend inwards and therefore no contact to the plastic button when pushing.

![150349e|690x388](upload://pCwbPTqNW6X9iFDnRAJDsouEi3c.jpeg) 

I bent it almost back and tested if it's working and yeeees it did so my plan was to bridge the gap behind against movement. Then I decided to bend it just a little bit more to get 90° like it was before and..... ZING, it broke off, damn!

![152654|690x388](upload://evadbuSrQYq6nIal3m2Y63Yv1on.jpeg) 

Fortunately the solder pads on the PCB are still fine. With a cable I can switch the remote on and off. So now I have to solder a momentary switch or maybe use this one but not on the PCB. I don't know why Maytech designed it this way, maybe because they thought they can sell more when they break.

My MBS Vine tires are done, almost no profile left on the rear ones

![160125|690x388](upload://nXDNZ2v6cP3uBxaNH2CGxnzwgFj.jpeg) 

Front tires look better but a bit sliced

![160357|690x388](upload://yszfhO9bOwLrqOIWKEv0sJHYYML.jpeg) 

Anyway this are the longest lasting tires so far. 
550km (342 miles) without swapping front and rear tires including heavy abuse like sliding or hardcore carving. Really not bad for MTB tires. Maybe they would hold up to 1000km with normal riding.
```

---
## \#595 Posted by: ArnhemAnt Posted at: 2018-11-08T20:43:56.065Z Reads: 181

```
Once again man, thanks for documenting all the things you are doing. Glad you got the remote working again - what a PITA. 
Stats on those tyres sound pretty good. I'm still on my Innova Mudplugger tyres, but haven't ridden anything close to your distances and I'm still getting used to the board so I'm certainly not riding 'hard', yet!

In the video you posted above, what setup were you running with the dampers on that board? You look to have a pretty good turning circle. I currently have the yellow dampers (front and rear) and have the adjuster screws flush with the top of the deck, but I my turning circle doesn't seem to be as tight as your turns.
Also, I only have the bindings, but no heel straps. I chose not to get heel straps at the moment so that I could still bail out of the board if things got a little 'hairy'. I'm actually considering taking the bindings off, but not sure if that's a good idea or not.
```

---
## \#596 Posted by: rich Posted at: 2018-11-09T00:06:34.059Z Reads: 186

```
The remote is not really working yet but yeah you're right, at least I can switch it on with a cable :laughing:

So we are using the same tires, mudplugger and vine are equal. As far as I remember you are riding some bush tracks, right? How does your board handle these? I'm curious because when the terrain gets too soft/deep I often get stuck and can't move on that's why I avoid very loose dirt. But I've never tried riding on sand.

[quote="ArnhemAnt, post:595, topic:45377"]
You look to have a pretty good turning circle.
[/quote]

I love it :sunglasses:
I don't use springs but this:

https://www.e-toxx-shop.com/trampa/elastomere-damper/

[quote="ArnhemAnt, post:595, topic:45377"]
I chose not to get heel straps at the moment so that I could still bail out of the board if things got a little ‘hairy’
[/quote]

Please never try to bail out when using bindings. I don't know if it's possible to get both feet out at the same time and furthermore instantly in an emergency situation. I think rather not. Then the chance is quite high that you twist a knee.

Heel straps are perfect for jumping but not necessary for riding. But I like the fact that I'm locked to the board and meanwhile I don't feel safe without. 

Riding on streets without bindings works but I wouldn't do it for all terrain/off road.
```

---
## \#597 Posted by: ArnhemAnt Posted at: 2018-11-09T03:55:36.049Z Reads: 183

```
[quote="rich, post:596, topic:45377"]
As far as I remember you are riding some bush tracks, right? How does your board handle these?
[/quote]


So far, I've had no issues with these tyres. I have ridden in loose gravel, grass, dirt, but not sand. I think they would spin and get stuck in sand, although, if I was going to try riding in sand, I'd do the same as I do with a vehicle and lower the tyre pressures. The other issue with my board is that if you hit the throttle to hard, the wheels will spin and that could be an issue with sand as well.

[quote="rich, post:596, topic:45377"]
I don’t use springs but this:
[/quote]

Thought you might be using those dampers from @Nowind. They seem like a way better option, but my cash-flow is pretty tight right now, so I'm going to have to keep with what I have until funds get batter.

[quote="rich, post:596, topic:45377"]
Please never try to bail out when using bindings
[/quote]

I've bailed out a few times, but only at lower speeds. So far so good, but I do understand what you are saying - it's always in the back of my mind that I could twist and ankle or knee in the process.

[quote="rich, post:596, topic:45377"]
Riding on streets without bindings works but I wouldn’t do it for all terrain/off road.
[/quote]

Fair point. I guess I should just stick with the bindings and just try to get used to them. Maybe I'll get a set of heel straps in the near future and take a shot at being locked into the board. 
My battery is under the deck so it doesn't lend itself to jumping, etc but I guess the heel straps have other advantages too.
```

---
## \#598 Posted by: Andy87 Posted at: 2018-11-09T04:56:07.763Z Reads: 168

```
Didn’t you also order the AliExpress version of those wheels a while ago?
If yes, are you planning to hook them up after this set?
I have a set of those Ali wheels and they still look good after round about 200km.

I have the same issue on sand. If sand is too soft I just sink too fast and wheels get stuck.
Idk how Baja boards manage that. I mean I have seen a promo video a while ago how they drive on the beach without problems and the wheels they use look very slim too.

@ArnhemAnt i came from no bindings on my street carve to bindings on my holypro and as I didn’t have had so much skating experience before it took me some time to get into it.
Now i‘m happy to have bindings as I have more control over the board. You can just turn with more pressure or tose the front around if you need to get around corners.
For now I drive without heel straps and I think as long as you don’t plan to do jumps it’s working good. As @rich once said (or it was in a video he linked) press your feeds to the out or inside of the bindings. That should give you a better sit in the bindings too.
```

---
## \#599 Posted by: ArnhemAnt Posted at: 2018-11-09T05:24:40.803Z Reads: 159

```
[quote="Andy87, post:598, topic:45377"]
For now I drive without heel straps and I think as long as you don’t plan to do jumps it’s working good.
[/quote]


Thanks @Andy87 - At this stage, that's pretty much my thoughts as well. I do not intend to jump with this current setup and the bindings do give me the feeling that I am "attached" to the board. I just have to spend more time riding it so that I get to feel more comfortable with it.
```

---
## \#600 Posted by: rich Posted at: 2018-11-09T20:28:30.455Z Reads: 189

```
[quote="ArnhemAnt, post:597, topic:45377"]
Maybe I’ll get a set of heel straps in the near future and take a shot at being locked into the board.
[/quote]

If then I recommend MBS heelstraps. Trampa are too small and shift all the time. For example when jumping in dirt park I had to reposition them always after 3 jumps. MBS shift, too but they are bigger that's why it's no problem and needs zero repositioning. MBS foot straps are like a cloud especially when riding barefoot :wink:

But again for riding you don't need heel straps and it's easier to get on and off the board but I prefer them for falling (with proper protectors). Funny that I had several injuries within 3 weeks riding my Trampa carver without bindings on concrete and almost no injury within the last 15 months riding strapped to the MTB. But I guess it's more thanks to my full body armor.

[quote="Andy87, post:598, topic:45377"]
@rich once said (or it was in a video he linked) press your feeds to the out or inside of the bindings. That should give you a better sit in the bindings too.
[/quote]

That's from an interesting Youtube video about bindings, so I post it again. After I watched this video I corrected the distance of the brackets of the bindings and it was much better. I don't like duck stance and pefer to stand 0° or maybe 15° on the front foot. That's why I have the brackets on the most inside position which lock my feet perfectly. In the beginning the foot straps were too loose.

https://www.youtube.com/watch?v=ObNSURYIj9E

[quote="Andy87, post:598, topic:45377"]
Didn’t you also order the AliExpress version of those wheels a while ago?
If yes, are you planning to hook them up after this set?
[/quote]

I have some tires at home including the Aliexpress ones (left side) :laughing:

![122117|690x388](upload://mdfBG70Xpcy10l0eExw5bEGB7FM.jpeg) 

But I switch to the last 2 Vine tires I have. I ordered 6 because the plan was to replace only the rear ones and they should be worn out at the same time as the front tires. I want to find out for science. Next time I'll mount the tires from Aliexpress.

Meanwhile I disassembled both rear wheels and found funny stuff in the tires like thorns which punctured the tubes. Both tubes and tires had several wet spots where the tire sealant worked like a king, I love this stuff!

I managed to fix the steez remote with the broken buttons. 
I don't need the B button so I soldered silicone 26AWG wires between the PCB and momentary push button and glued it to the enclosure, works like a charm. Maybe I'll replace the tiny battery with something bigger one day.


![161916|690x388](upload://utintAAIO1ahoFnUC7TlVVdk8rL.jpeg) 

![164322|690x388](upload://1IpKBK4wpMVMN2Dv8tItvTEg54F.jpeg) 

![164858|690x388](upload://74Fxihnehyq60YlTaptsiEFZSqi.jpeg) 

![165515|690x388](upload://jzfh1dk1TBtON9freKDsLW0aCbH.jpeg) 

![165752|690x388](upload://pFxH9yZTF0IEjJTby3M2rkKhOS2.jpeg)
```

---
## \#601 Posted by: telnoi Posted at: 2018-11-09T21:06:42.967Z Reads: 183

```
[quote="rich, post:600, topic:45377"]
Meanwhile I disassembled both rear wheels and found funny stuff in the tires like thorns which punctured the tubes
[/quote]

Got two punctures due to crap getting in via the big hole for the air valve. Tires themselves were never punctured. Sugru that shit for added security.
```

---
## \#602 Posted by: rich Posted at: 2018-11-09T21:41:10.229Z Reads: 186

```
Great idea with the sugru, never thought about that. I have at least 2 thorns or something else sticking through the tire which punctured the tubes but it's not visible from outside.

A couple of days ago I had the idea to mount the camera to the bull bar very close to the ground and machined some ABS sheets.

![143600|690x388](upload://4KicaEe9hMRGorpB2UKUx9sfWbK.jpeg) 

![094200|690x388](upload://otiRbj4m8jGk8RmtJefTtL8pcS3.jpeg) 

Finally mounted

![153107|690x388](upload://mkTiDAITd4u9kTWEda1Uk4qrU1m.jpeg) 

![153124|690x388](upload://uI0q24Il7zavTox83iIOKRL1u1M.jpeg) 

I did a test ride but it rattled and I'm not sure yet why but after the ride I realized the threaded insert got out the plastic and I can't push it back.

![055103|690x388](upload://fHNFKrlJlJZ616uMd7rtWJLbCsV.jpeg) 

 I also shoot at bmx course but the video is shaky. I hit some objects and damaged the case for the camera so I have to buy a new case. And the camera should be mounted higher :laughing:
```

---
## \#603 Posted by: ArnhemAnt Posted at: 2018-11-09T22:21:38.950Z Reads: 178

```
[quote="rich, post:600, topic:45377"]
In the beginning the foot straps were too loose.
[/quote]

Thanks for posting that video - a very good resource, and after watching it, I now know that my foot straps are too loose. The problem I have is that the brackets are already on the far inside positions. The foot straps were pre-installed on the board when I purchased it and I don't really want to drill more holes. Maybe they were fitted to the deck to allow for people wearing boots?
```

---
## \#604 Posted by: rich Posted at: 2018-11-09T22:53:10.662Z Reads: 177

```
[quote="ArnhemAnt, post:603, topic:45377"]
Maybe they were fitted to the deck to allow for people wearing boots?
[/quote]

:rofl:
I totally forgot about that, barefoot straps should have the brackets more inside. Maybe you can machine some aluminium plates with 4 holes to move the brackets more inside without drilling new holes. On the other side the brackets could hurt if you touch them. You could stick some high dense foam on them.
```

---
## \#605 Posted by: Tamatoa Posted at: 2018-11-09T23:06:10.427Z Reads: 168

```
Would it not be safer to mount the camera on top? I’d be worried it’d get ripped off.
```

---
## \#606 Posted by: Pedrodemio Posted at: 2018-11-10T02:37:18.010Z Reads: 171

```
I was going to say that, if you managed to break a deck, destroy a truck and probably more things that I can’t remember, that camera has no idea what it will have to face 😅
```

---
## \#607 Posted by: Tamatoa Posted at: 2018-11-10T05:50:20.894Z Reads: 167

```
Right?!!! My thought exactly,
```

---
## \#608 Posted by: rich Posted at: 2018-11-10T11:51:34.620Z Reads: 185

```
[quote="Pedrodemio, post:606, topic:45377"]
that camera has no idea what it will have to face :sweat_smile:
[/quote]

It faced it already and didn't like it :laughing:
I'll upload a short part of the video so you see and hear the abuse.

[quote="Tamatoa, post:605, topic:45377, full:true"]
Would it not be safer to mount the camera on top? I’d be worried it’d get ripped off.
[/quote]

Yes next time for sure it was a bad idea, I quote myself:

[quote="rich, post:602, topic:45377"]
I hit some objects and damaged the case for the camera so I have to buy a new case. And the camera should be mounted higher :laughing:
[/quote]

The plastic in the middle of where the lens is has a damage, you can see that in the video of skate park. In general the case is scratched everywhere because I like low angles. I'm sure I'll find cheap replacements on Aliexpress. 

As I wrote this i realized this part in front of the lens is mounted with screws and can be replaced, great! That should be cheaper than replacing the whole case. 

![124005|690x388](upload://8F2kjZFcUfbYP6iXNCwFGMZ0pox.jpeg)
```

---
## \#609 Posted by: DANGERDAD Posted at: 2018-12-26T15:40:38.997Z Reads: 165

```
I had two magnets come loose in a chinese board. Caused an esc failure by loading it up with to much current draw. Managed to get motor and esc replaced thank goodness
```

---
## \#610 Posted by: tardyparty7 Posted at: 2018-12-26T15:44:55.591Z Reads: 168

```
if i missed it sorry, but where did you buy the gear drive from?
```

---
## \#611 Posted by: Andy87 Posted at: 2018-12-26T16:21:09.009Z Reads: 161

```
@nowind  https://www.e-toxx-shop.com/
```

---
## \#612 Posted by: rich Posted at: 2018-12-26T17:34:37.819Z Reads: 171

```
Like @Andy87 said from E-Toxx, it's the 1:5 drive with helicals, very silent. Straight cut gears scream so you can hear the power and also people hear you and dogs bark at you :laughing:. Both are top-notch but I prefer the helicals for ghost mode, also the SK8 motors are quite silent in FOC.

BTW the one motor still sounds bad and has a very little play sideways but like @telnoi I just ignore it and keep on riding as long as possible.  

It was very cold the last 2 weeks so no riding but today we had sunny 5°C and it stopped raining so it was time to get dirty.

![164950h|690x388](upload://xURijsDEq9Qjgt6pGuAVoFu5Usd.jpeg) 

![165223h|690x388](upload://rVFGkNs9XeU5jmD1KQDCLaNB3HK.jpeg) 

![165935h|690x388](upload://mdCx1o5aQ0UyY0NnV8YOEJwG4wO.jpeg) 

The great thing with a sealed drivetrain is the cleaning part, just a bit water and some minutes later...

![174520h|690x388](upload://hz0hXZNnJMQs3EGCLVLglikqpos.jpeg) 

Today I've tried doing wheelies´, hurtful experience especially on concrete. It looks so easy but it ain't.
```

---
## \#613 Posted by: Andy87 Posted at: 2018-12-26T17:38:29.185Z Reads: 162

```
What a transformation 😂
Pimp my esk8 in only 5min 😜

And yes I totally agree, wheelies look easier than they are☝️

Did you change anything in your throttle curve to have more start up torque or you just run standard settings?
```

---
## \#614 Posted by: rich Posted at: 2018-12-26T18:12:41.569Z Reads: 158

```
No changements in throttle curve, I think you would need the raw power of a car ESC to lift the front properly anyway. All the videos with wheelies which I know were not running with vescs.

I just gave a bit more throttle but more tried to get in position by pushing down and then lifting the front foot and lean backwards like on a bicycle. My goal would be to find the balance with the body instead of increasing throttle but maybe I'm just too old :joy:
```

---
## \#615 Posted by: ArnhemAnt Posted at: 2018-12-26T20:16:36.143Z Reads: 164

```
[quote="rich, post:614, topic:45377"]
maybe I’m just too old
[/quote]


I'm with you on that one bro. I'm at a time in my life when I want to keep all my wheels in contact with the ground, whether its on my motorbikes, mountain boards, etc. There have been a few times on my mountainboard where I accelerate a little loo fast and I can feel the front wheels starting to lose traction. That was enough for me.
I guess if you really wanted to do wheelies, then it would make more sense to do these while the board is moving, rather than from a standing start.
```

---
## \#616 Posted by: garseng Posted at: 2018-12-26T21:35:16.203Z Reads: 154

```
your sunny is 5 degree mate? please come to Malaysia :slight_smile:
```

---
## \#617 Posted by: taz Posted at: 2018-12-26T22:41:56.158Z Reads: 160

```
I am going to ride to work on my board tomorrow since it will be a sunny 1C in the morning  and I live in Athens - Greece :smiley: 

![13|690x388](upload://oEUdR1w90oRQEwHposmyWjsIBCS.png)
```

---
## \#618 Posted by: Eboostin Posted at: 2018-12-26T23:25:03.725Z Reads: 156

```
What kind of wrap did you use on the motors? It looks thicker than regular vinyl wrap but looks great!
```

---
## \#619 Posted by: rich Posted at: 2018-12-27T00:22:47.519Z Reads: 167

```
[quote="ArnhemAnt, post:615, topic:45377"]
I guess if you really wanted to do wheelies, then it would make more sense to do these while the board is moving
[/quote]

That's what I did (or at least tried) and why it hurted more :laughing:, thanks to protectors no graze. 

I'm never too old to do stupid things but falling felt much better 20 years ago without hurting bones afterwards. My shoulder sometimes still hurts from the crash in skate park 3,5 months ago. That's what I meant with "too old" but anyway I want to jump bigger and higher in 2019 and hopefully do my first 360 :grin:

[quote="garseng, post:616, topic:45377"]
please come to Malaysia :slight_smile:
[/quote]

Checked the forecast, 31°C sounds really good but it's raining and thunderstorm bro. 

[quote="taz, post:617, topic:45377"]
sunny 1C in the morning
[/quote]

Brrrrrrrr..... didn't expect it to be colder in greece than in austria, tomorrow here it is up to 9°C.

[quote="Eboostin, post:618, topic:45377, full:true"]
What kind of wrap did you use on the motors? It looks thicker than regular vinyl wrap but looks great!
[/quote]

Yes, it is vinyl indeed but a little bit thicker than standard wrap but not much. It is carbon foil by d-c-fix for about 10€ per roll. I used it on other motors and enclosures, too and it holds.
```

---
## \#620 Posted by: garseng Posted at: 2018-12-27T00:39:12.875Z Reads: 154

```
[quote="rich, post:619, topic:45377"]
31°C sounds really good but it’s raining and thunderstorm bro
[/quote]


shower after shredding is nice sometime..lol
```

---
## \#621 Posted by: rich Posted at: 2018-12-27T01:25:41.351Z Reads: 160

```
What I forgot to mention is the poor range of my battery when riding in cold temperatures. The last 2 rides (at -1°C and 5°C) I had only 12km range instead of 20km (with 12s 8Ah lipo), that's a huge difference.
```

---
## \#622 Posted by: Andy87 Posted at: 2018-12-27T05:06:04.800Z Reads: 160

```
That’s really interesting.
I didn’t  notice any big range difference and the last rides where with -6 degree outside.
```

---
## \#623 Posted by: Trdolan03 Posted at: 2018-12-27T05:08:04.347Z Reads: 159

```
@rich what’s your setup? At 8C with my 12s 20ah pack I was only getting 19km on flat pavement
```

---
## \#624 Posted by: ArnhemAnt Posted at: 2018-12-27T06:38:22.190Z Reads: 156

```
Yeap. I just came back from a ride in the rain and it was awesome.
```

---
## \#625 Posted by: pjotr47 Posted at: 2018-12-27T08:51:36.845Z Reads: 155

```
The range difference is normal. You have the biggest range around 20 degrees. If you go around the 0 degree, you range would be around -30%,-40%. 

This is all this is all temporary and does not damage the battery. When the temperature rises, it will disappear again
```

---
## \#626 Posted by: Andy87 Posted at: 2018-12-27T09:31:15.893Z Reads: 161

```
I think it was more a statement and information for us than a question why that happend ;)
I wonder why my range isn´t significantly less even with -6 degree outside.
One other thing is, that the capacity will become less if the battery is at 0 or similar, but my batteries never get that cold.
I start from home with room temperature, let´s say 25degree.
After some minutes of use, the batteries start to get slightly warm.
I would say they nerver get below 10degree.
Maybe the reason why my range doesn´t change too much is the fact that I anyhow can drive max 45min till the battery is empty and i need to get a new set from the warm home place? :thinking:
Need to infestigate a bit more this winter. Maybe i should also install my temp sensor close to the battery to get some more exact information.
```

---
## \#627 Posted by: rich Posted at: 2018-12-27T15:46:31.688Z Reads: 170

```
[quote="Trdolan03, post:623, topic:45377, full:true"]
@rich what’s your setup? At 8C with my 12s 20ah pack I was only getting 19km on flat pavement
[/quote]

19km? With pneumatics or gummies? Seems like you can win a medal in poor range, damn.

I use 6374 149kv SK8 motors (but had the same range with Trampa and Maytech motors, too) with Vesc6 [motor 80A | brake -40A | batt current max 50A | batt current max regen -15A each Vesc], 1:5 gearing and 12s Graphene 15C 8Ah lipo.

[quote="pjotr47, post:625, topic:45377"]
If you go around the 0 degree, you range would be around -30%,-40%.
[/quote]

Yeah unfortunately it's -40% with my lipo. I wonder if there is a difference between lipo and li-ion at cold temperatures. I can imagine it's even worse with Li-ion because of the metal but no idea.

[quote="Andy87, post:626, topic:45377"]
I wonder why my range isn´t significantly less even with -6 degree outside.
[/quote]

Don't worry be happy :grin:
I wonder what's your range in real russian winter like -15°C or -20°C, you'll find out if you don't freeze to death.
```

---
## \#628 Posted by: Andy87 Posted at: 2018-12-27T15:52:27.197Z Reads: 162

```
[quote="rich, post:627, topic:45377"]
real russian winter like -15°C or -20°C,
[/quote]

February is usually the most cold month here.
-20 till -30. hope till this time my new motor cans are delivered and I can drive again and find it out.
```

---
## \#629 Posted by: rich Posted at: 2019-02-22T18:23:45.622Z Reads: 161

```
I had my first couple of rides in 2019 within the last week and it was great, can't wait for spring to come!
The E-MTBoard fever is back in full effect, I reay missed it.

One thing I learned last year, always have spare parts if you want to continue riding. 
Beside all mechanical spare parts which I already had I bought a third SK8 motor for quick replacement when I need it. I hope to ride this season without breaks and anytime I want.  

I want to do new things and break boundaries this year and first thing was to jump off ramps in skate park sideways which I never did before because I was too scared. It's not really difficult but you have to jump off active and earlier than on a straight edge. On the first 2 attempts I touched the edge with the deck because I jumped off to late but then I got it and shot this short video without licking the concrete. 

https://youtu.be/TKaj-uHQEzc

I'm planning to ride some MTB Trails and doing more crazy stuff soon. Also I want more airtime but trying to increase it very slowly because it's really dangerous when it's not within the skill level (guess why I know). Small steps...
```

---
## \#630 Posted by: topcloud Posted at: 2019-02-22T18:28:46.701Z Reads: 163

```
![image|480x270](upload://wmiTprAQc4NxnFA6G0UJhEdkPhV.jpeg)
```

---
## \#631 Posted by: Andy87 Posted at: 2019-02-22T19:49:49.457Z Reads: 166

```
Waiting patiently for some more of you videos in 2019!
Let’s rock it 😌
```

---
## \#632 Posted by: rich Posted at: 2019-02-25T18:57:21.899Z Reads: 166

```
Today I had the worst and most scary crash so far with the dirt machine.
I was riding on BMX track but in Round 3 everything went wrong. I was riding faster to make bigger jumps and just when approaching a kicker the board went 100% throttle. I lost balance and made a quarter backflip in the air and landed on my shoulder and arm first, then the hip got compressed into dirt and stones. That was really painful and I thought I'm done. I was able to stand up and ride back home very slowly. I'm not 100% sure but I think nothing is broken. The crash pant saved my hip and the full body armor probably my shoulder, let's see. Crazy thing is the graze below my elbow despite wearing protectors.

![160611_v|690x388](upload://bwKeBJtNDUMwp0v3fXnx7EhoM1q.jpeg) 

What the hell was going on? I never had this issues with the steez remote so far and I don't think it was unintended throttle by myself. It was instant 100% throttle, really scary. BTW it was fully charged.

I'll change the ppm wires first. On my first esk8 I had similar problems with a GT2E remote/receiver. Randomly 100% throttle while riding, only stoppable by applying brakes, crazy shit. The ppm cables were quite heavy bent after the connector. I swapped them and everything good again. 

Stay safe and wear protectors!
```

---
## \#633 Posted by: janpom Posted at: 2019-02-25T19:02:41.903Z Reads: 162

```
Board going full throttle by itself is my greatest fear when riding. One of the reasons I have the max speed limited to ~35kph on the VESC. 

Glad that nothing worse happened. The bruise is pretty crazy considering you wore your protective gear.
```

---
## \#634 Posted by: Andy87 Posted at: 2019-02-25T19:05:57.623Z Reads: 156

```
Damn it! Get well soon!
Good to hear not more happened!
```

---
## \#635 Posted by: rich Posted at: 2019-02-25T19:56:14.501Z Reads: 164

```
Thanks guys!

[quote="janpom, post:633, topic:45377"]
The bruise is pretty crazy considering you wore your protective gear.
[/quote]

True, I wore long sleeve, then protection vest plus a jacket. And my backpack has a hole now :unamused:. My hip is a bit swollen but no problem.

I checked the wires and they look good, not too much bent. 

I forgot that this full throttle thing already happened twice. Once while hitting the ground after a small crash and once while riding a tiny berm in dirt park. In both cases I could lift the board in the air to prevent catching speed.

The problem is the cruise control function of the remote which gets activated by pushing the thumb throttle down. It should keep the speed but often the speed increases very quick. It happens sometimes that I press the throttle down unintentionally like on landing after a jump. In zero position it enters pairing mode and no more control. I can deal with that since I know just to push the throttle down again to get control back.

On BMX track the full throttle happened while compressing the deck down before take off. Maybe my thumb made a weird movement including locking high speed. It happend so quick but made me rotatng backward while flying forward, not a good feeling.
```

---
## \#636 Posted by: okp Posted at: 2019-02-25T20:00:41.918Z Reads: 150

```
Be well mate ! Our games will anyway end up badly one day or the other !!!
```

---
## \#637 Posted by: Andy87 Posted at: 2019-02-26T15:32:12.120Z Reads: 153

```
Just came to my head, 
Any chance that the remote was on low battery?
Usually it should just drop out in this case, but who knows.
Did you check your fail safe settings too?
```

---
## \#638 Posted by: Pedrodemio Posted at: 2019-02-26T16:18:45.884Z Reads: 153

```
Glad you good

I had this problem once with cruise control, the button got stuck pressed and I had to bail, turned that off as soon as I got home
```

---
## \#639 Posted by: rich Posted at: 2019-02-26T21:08:35.191Z Reads: 163

```
[quote="Andy87, post:637, topic:45377"]
Any chance that the remote was on low battery?
[/quote]

Very good idea but since I know how weird my remote can act on low battery I charge it after every single ride, it's always fully charged. I want to install a bigger battery because it lasts only 40-50km (200 mAh).

[quote="Andy87, post:637, topic:45377"]
Did you check your fail safe settings too?
[/quote]

Yes and just checked it again, it's working like it should be. 
I also never had drop outs with this remote that's why I trust it, a remote with drop outs is deadly.

I'm holding it like that, not really comfortable but I got used to it. Of course the goat leather on my thuimb is not the best for sensitive control but I love this gloves, saved me so many times (also look at the curbs on palm protectors).

![202718_eh|531x500](upload://3Sedrm25dLgeG8GpOS84ULPjcej.jpeg) 

The main problem is that I need the thumb to hold the remote, therefore it can happen that I push it down on rough terrain or jumping unintended. That never happened on flat terrain.

[quote="Pedrodemio, post:638, topic:45377"]
I had this problem once with cruise control, the button got stuck pressed and I had to bail, turned that off as soon as I got home
[/quote]

Which remote? 
By turning off do you mean in the software (Ackmaniac)?

I would like to have a switch on the remote to turn the push function of the throttle on and off but that seems difficult. I don't know which connection it is and furthermore all is directly soldered to PCB.

![164322e|690x350](upload://yJubYGbbIrhXLs7ZkdGTUlrn22W.jpeg) 

I still have no idea how this accident happened and it was to quick to react. I had many falls but normally you see where you are falling so you can react. Flying in the air and don't know where is up and down is scary. All you can do is waiting for impact, that's it. I remember that I lifted my head to avoid any impact, that's why my neck and shoulder hurts. 

I just realized that this was the first real life test for the bull bars because the rear took the impact. Everything survived.

![205637h|690x388](upload://ApgeOUmFUik5MEzNIKoTGfn9n2W.jpeg) 

I have to hail once again @Nowind and also @Duffman :partying_face:
I love every single E-Toxx part which made my board a better one, piece by piece. It totally changed my riding style and I really can't destroy this drivetrain. Randomly I hit/slide curbs with the housing after a failed ollie or jump. Often it takes really bad hits where I think OK now I destroyed it or it's shifted but this never happened. 

And the helicals are epic. It's so funny when people don't hear you approaching from behind and are scared when I say "excuse me" just behind their heads. I need a bicycle bell on the finger or better a horn. Or speakers with a barking dog :laughing:
```

---
## \#640 Posted by: Pedrodemio Posted at: 2019-02-26T21:51:05.343Z Reads: 159

```
Mine is a custom Arduino based using a Wii nunchuck, how do you activate the cruise in this one?
```

---
## \#641 Posted by: rich Posted at: 2019-02-26T22:23:26.869Z Reads: 158

```
By pushing the thumb throttle down, it has a built in switch.
```

---
## \#642 Posted by: Pedrodemio Posted at: 2019-02-26T22:35:15.361Z Reads: 162

```
Apart from the 3 pins of each potentiometer (blue pieces) and the 4 on each corner holding the whole joystick down, the 2 or 4 remaining should be for the cruise

Unfortunately they could be routed on the top of the PCB making more difficult to trace it
```

---
## \#643 Posted by: rich Posted at: 2019-02-27T21:00:07.005Z Reads: 165

```
You motivated me to open the remote again and searching for the switch connection and finally I found the tiny switch itself for cruise control and how it works.

![190500_he|690x388](upload://42ebwBD8AvO3mk3a0mvVJWGpxhb.jpeg) 

No way to solve it electronically so I thought I could add a mechanical blockade that the white lever can't touch the switch. I took a toothpick and filed it a bit until it fitted into the gap.

![191919h|690x388](upload://v3vc6kEXLZGRN2Wn4RnT3bMTDMe.jpeg) 

Some magic glue and done! The toothpick is strong enough even when I push down hard.

![195408h|690x388](upload://oJhBIa9lunLoQNOIlAklzJW8G1V.jpeg) 

Finally the cruise control function is locked and no more unintended activation possible :ok_hand:. 
If I ever have to pair the remote it's easy to remove the toothpick.
```

---
## \#644 Posted by: Pedrodemio Posted at: 2019-02-27T21:20:49.733Z Reads: 160

```
Ok solution :grin:

If you manage to cut the 4 black dots the button will open and them you can remove everything from inside
```

---
## \#645 Posted by: rich Posted at: 2019-02-27T21:26:14.077Z Reads: 162

```
Thanks for the hint but I think I leave it like that because I need this switch for pairing with receiver and removing the toothpick is easy if I ever need it.
```

---
## \#646 Posted by: garseng Posted at: 2019-03-05T07:00:18.416Z Reads: 157

```
mind I'm asking, what is the version of the vesc6 fw are you using? is it the latest one?
```

---
## \#647 Posted by: rich Posted at: 2019-03-05T09:43:55.004Z Reads: 163

```
I'm still on FW3.38 (Vesc-Tool 0-94) :shushing_face:

I would love to get rid of the low braking/release problem in FOC but I don't know if cogging is the better solution. I'm waiting for more feedback and until my balls get bigger.

My shoulder still hurts but is good enough for riding without falling :wink:. I had 2 rides yesterday and recognized that my Lipo degraded badly. In winter I thought it's just the low temperature but it was 18°C and my range is max. 14km instead of 20km (12s 8Ah). Damn that's way too less range. I need to start my 12s6p asap, only problem is money like always.
```

---
## \#648 Posted by: taz Posted at: 2019-03-05T09:56:40.147Z Reads: 153

```
You need to start on your 12S7P or better yet 12S8P :sunglasses:
```

---
## \#649 Posted by: rich Posted at: 2019-03-05T10:27:45.461Z Reads: 158

```
I would love endless range :sunglasses: but there is no more space left in the Pelicase to go bigger. Also my board is not light weight so the bigger the heavier and 12s6p already adds about 1.5kg. 

I'm waiting until fishpaper and heatshrink is back in stock at Nkon and then order 30Q's, too. I would prefer to spot weld the battery but have no spot welder. Maybe I buy one with a friend together but it's expensive just for 1-2 batteries. Second choice would be soldering (with cell level fuse) where I have all materials at home. I already soldered a 10s4p with flat copper braid without problems but have no long term experience with this pack e.g. if it degrades after some time. Spot welding is definitely better.
```

---
## \#650 Posted by: taz Posted at: 2019-03-05T10:39:20.790Z Reads: 154

```
Lack of space is a legitimate problem.
The malectrics costs 130€ so not that expensive.
If you want I can lend you mine after I finish a couple of batteries I need to make for my Tayto and a friend's Evolve.
```

---
## \#651 Posted by: rich Posted at: 2019-03-05T10:54:06.364Z Reads: 155

```
Wow thanks for the offer :smiling_face_with_three_hearts: in worst case I PM you.

I have to take a closer look to the malectrics, seems fine. I was thinking about boss level and a friend about kweld. The malectrics also has seperate electrodes to hold with both hands, is this a problem in real life? I can imagine it's easier if you have one hand free e.g. to hold the nickel strip.
```

---
## \#652 Posted by: taz Posted at: 2019-03-05T10:59:31.231Z Reads: 158

```
Quite the opposite.
With 2 electrodes it is easier to put equal pressure to both as well as reach difficult places.
I found it very easy to use when I made my Trampa battery

https://www.electric-skateboard.builders/t/12s7p-battery-for-trampa-help-me-with-the-build/72900/35?u=taz
```

---
## \#653 Posted by: Andy87 Posted at: 2019-03-05T11:37:59.391Z Reads: 155

```
I have a sunkko spot welder as well and ready to lend you for the time you need.
Not sure about how much shipping that thing would be, but... just in case, let me know.
```

---
## \#654 Posted by: rich Posted at: 2019-03-05T20:23:06.891Z Reads: 157

```
Thanks a lot, really appreciate it!
I'm afraid shipping a huge parcel back and forth is too expensive and risky :laughing:. But I'll let you know in case. 

Didn't expect this kind of support from you and also @taz and am stirred :clap:
```

---
## \#655 Posted by: Nowind Posted at: 2019-03-06T14:54:59.845Z Reads: 156

```
Bro got one sunko laying around too...


Many options 😃
```

---
## \#656 Posted by: rich Posted at: 2019-03-06T21:48:02.682Z Reads: 162

```
Haha great :smiling_face_with_three_hearts: welcome to the spot welder battle, many thanks bro!

I had a ride today with a bit hardcore uphill action (want to know the limits), motors reached 70°C and Vescs 50°C. Outside temperature was 15°C so I'm a bit afraid of summer.

The last rides I recognized a loose rattling sound from the rear truck on all terrain. I checked all screws and everything else but couldn't find the root. Today I started to beat and knock on all kind of parts until I found the issue. It's the bad motor, it got worse, sounds like something is loose but it still runs without problems, weird.

https://youtu.be/pgZqvbuUqsM
```

---
## \#657 Posted by: telnoi Posted at: 2019-03-07T06:19:15.269Z Reads: 158

```
Just read what happened, speedy recovery.
Those basterd stones are my mortal enemies (causes a shitload of damage when falling) . Only thing I don't have yet is crash pants. Good reminder to buy one of these. 

Regarding your dead pack, were these graphenes?
```

---
## \#658 Posted by: rich Posted at: 2019-03-07T10:21:26.151Z Reads: 163

```
Thanks, fortunately I can ride again because the "bad" right shoulder is quite safe when falling (riding regular). 

It wasn't a pleasure to wear the crash pants in the beginning but after a short while I got used to it and now I feel naked and not safe without. Highly recommended but in summer hot AF :laughing:

[quote="telnoi, post:657, topic:45377"]
were these graphenes?
[/quote]

Yes but they are still graphenes, just a little puffed and with less capacity. Below the nominal voltage the voltage decreases very fast, last year it was much slower. I guess the main problem is that I'm using 15C graphenes, this is my second puffed pack within 2 years. 

I recognized green slime on the heel strap from my ride yesterday

![003205h|690x388](upload://ntxl1rI2mE933S9fHTKYth5RBPV.jpeg) 

I looked at my shoes and saw no signs of tire sealant, then I looked at my trousers :rofl:

![002844h|690x388](upload://md0Sr5Mt98YC3t7JwxLPdOQXf7b.jpeg) 

Damn it! Even on the hoodie and helmet but it's dry already, hope it's removable.

Strange thing is that I can't see any damage on the tire and it's still fully inflated. There must be a thin cut somewhere.
```

---
## \#659 Posted by: PatRocks Posted at: 2019-03-11T02:17:00.313Z Reads: 158

```
Lol, this thread has been SO entertaining!! I've been laughing out loud while reading. People looking at me funny 🤣
```

---
## \#660 Posted by: telnoi Posted at: 2019-03-11T06:19:53.007Z Reads: 151

```
[quote="rich, post:658, topic:45377"]
. I guess the main problem is that I’m using 15C graphenes
[/quote]

Would be interesting. I almost fear that with the amount of riding we do throughout the entire year, not a single pack survives for more than 1.5 season. Same with my drone packs, all dead within a year no matter the C rating.
```

---
## \#661 Posted by: rich Posted at: 2019-03-11T14:22:20.261Z Reads: 154

```
I have no experience with high C rated packs but I thought they should last longer beside the advantage of less voltage sag. They are too expensive for short usage IMO. Would be interesting to hear some more feedback from users from high C rated packs how long they last.
 
BTW I don't have problems with too much sag with 15C 8Ah, usually it's about 1V, on full throttle 3V. But I guess 15C is the reason why they puff and loose capacity that fast.
```

---
## \#662 Posted by: telnoi Posted at: 2019-03-11T16:18:36.918Z Reads: 154

```
[quote="rich, post:661, topic:45377"]
on full throttle 3V
[/quote]

That is still double compared to the voltage sag I see at 60C/12Ah.
As long as the combined output rating is not surpassed and the packs stay cool, the higher C rating should not lead to a substantially higher lifetime. As soon as they start puffing or become hot, you have already surpassed the limit. 

The Graphene packs do deal with depletion better (riding till 3.4V is possible, where 30C packs for example start cooking and should be limited to 3.7V minimum).
```

---
## \#663 Posted by: rich Posted at: 2019-03-15T17:06:54.404Z Reads: 150

```
Had some fun in the narrow single trail at dirt park. It is very difficult to ride because it's tiny and has tight curves, not mountainboard friendly. Slightly leaving the trail means 99% chance of falling which happens quite often :laughing:

https://youtu.be/Fcqdf5844EM
```

---
## \#664 Posted by: taz Posted at: 2019-03-15T19:03:13.195Z Reads: 152

```
Great video.

Do you know how much you board weighs?
```

---
## \#665 Posted by: Andy87 Posted at: 2019-03-15T19:05:19.860Z Reads: 151

```
[quote="rich, post:663, topic:45377"]
99% chance of falling
[/quote]
For this your fail part was pretty short compared to the rest 😜
```

---
## \#666 Posted by: rich Posted at: 2019-03-15T22:56:05.287Z Reads: 149

```
[quote="taz, post:664, topic:45377"]
Do you know how much you board weighs?
[/quote]

Actually 15.8kg (35lbs)

[quote="Andy87, post:665, topic:45377"]
For this your fail part was pretty short compared to the rest :stuck_out_tongue_winking_eye:
[/quote]

Haha true but it was a short session without testing the limits. The tricky parts are the curves/birms with stones and holes on the sides. Also in the grass are big stones, bricks and wood. But normally falling doesn't hurt at that low speed.
```

---
## \#667 Posted by: Pedrodemio Posted at: 2019-03-16T22:57:09.542Z Reads: 150

```
That second fall is the best :grinning:
```

---
## \#668 Posted by: amecces Posted at: 2019-03-20T17:08:08.254Z Reads: 149

```
https://www.elektro-skateboard.de/forums/topic/6859-dirt-track-meisterschaft-2019/
```

---
## \#669 Posted by: rich Posted at: 2019-04-02T21:22:44.687Z Reads: 148

```
Had a hardcore ride and destroyed 3 tires and bent the metal plate of the gear box :metal:.

But it was a lot of fun shredding stones and crazy inclines up to 40 degrees (83%). Fortunately I shot some video scenes there so I have evidence :grin:.

![still_02|690x388](upload://eGHAwEneNgW9g6bErJ1w9jPCCfp.jpeg) 

The wall of fear

![still_00|690x388](upload://vB6v8IwYPuXJ01GhVj2Op80blHB.jpeg) 

Unfortunately I've chosen the wrong angles so in the video exactly the same 40° wall looks like kindergarden

![still_08|690x388](upload://iJz9FOKUUIV5tO4REk70bsMWjgt.jpeg) 

It is so freaking steep and there are some more walls to climb

![still_05|690x388](upload://dQMXpQ4cFFHSrJVw0ZN6PVrToWh.jpeg) 

How to slice your tires...

![still_03|690x388](upload://xOgWGIEZ9pawVNTzQMMDDMy9ex5.jpeg) 

I would love to shoot more with better angles but I think it's enough damage for now.

![151608h|690x388](upload://p3bGbb5FV9JxoHKhIFMlEWihqsW.jpeg) 

![201518h|690x388](upload://pTwF5t1DnFPiZkY3P1Z2ZVJJdo.jpeg) 

Both rear tires have several slices like this 

![152859eh|690x388](upload://kupHQ9YtN5tD40BRjcLYOUZMYst.jpeg) 

and the front tire/tube.... well :joy:

![160459h|690x388](upload://oB8mzBd6Hx38zOhW9eD1ITiHAEO.jpeg) 

 ![coneheads1|665x375](upload://9a2egiD3g83HPXj4nc4DjB7hAVr.jpeg) 

Furthermore the motor shifted down, the backlash was gone and there was a noise. In the beginning I thought it's the faulty motor but after a while it sounded like straight gears and I started to carry it home. I degreased the drive train and it seems like there is no damage at all :ok_hand:

I was riding without backlash and sand in the gears, Jesus :laughing:

![135610h|690x388](upload://tfPRDzRqI7fcfmQxwq0DPhgZyRR.jpeg) 

Applied much more Loctite this time so it shouldn't move again. It's getting too late to make noise so I finish this tomorrow but it's still 80% done.

![220543h|690x388](upload://j07BAn3UxQ4uPtJinKjlSYaiGDH.jpeg) 

I guess it's time for the cheap aliexpress tires if I find enough tubes.
```

---
## \#670 Posted by: spei Posted at: 2019-04-02T22:06:20.968Z Reads: 145

```
1. https://www.ebay.de/itm/Pannenschutzband-Zefal-Z-Liner-lila-Enduro-DH-Breite-50mm-2x135g/391877231398?epid=2000406688&amp;amp;hash=item5b3db40326:g:5scAAOSwNvRbUim5 
2. https://www.ebay.de/itm/Slime-Innenschlauch-Versiegelung-237ml-Flasche/112336540050?hash=item1a27c79192:g:6i0AAOSwEFZZfE97 

Lil bit help for flat tyres, Its ment for bikes, but who cares. When applying in 6,5-9&quot; tyre. make a lot of cuts in tape along the sites to the center of tape, so you dont get curves, and then use some heavy duty tape to fix it with tyre so the tube wont get caught in between and get slice down. Then u can put on tyre with the tube on the rim and apply slime inside tube. Just remember to change tubes and apply new slime every year just in case.
```

---
## \#671 Posted by: rich Posted at: 2019-04-02T22:25:42.677Z Reads: 146

```
Thanks for the links. I've never tried tire liner but seems interesting.

I use tire sealant in all tubes already :grin:

![005343|690x388](upload://nvJiuyirjtVEsDMEX6fZFR2GJcs.jpg) 

That doesn't help all the time

![Bang3e|690x388](upload://cLmks0VmvxIsjASd8t8thvV9Uoc.jpg) 

Without tire sealant I always had flats, it was gone with the green slime but after some months they started to lose air regularly.
```

---
## \#672 Posted by: Pedrodemio Posted at: 2019-04-02T22:28:19.602Z Reads: 143

```
I think is time to change your title to Everythingnator 

Looking forward to this video
```

---
## \#673 Posted by: spei Posted at: 2019-04-02T22:35:40.372Z Reads: 141

```
I was doing lot of forest biking when I was younger, healthier and more handsom, so before I found out 'anti-puncture tape' what I did, was applying old tubes between tyre and new tube, but that stuff was meh. This shit is srsly doing its job. Just maka sure u fix it to tyre with tape. It can slice your tube. And slime helps with small cuts and holes. When u blow up tyre nothing can help(except lots of grass, gravel steel legs and concrete ass xD)
```

---
## \#674 Posted by: DEEIF Posted at: 2019-04-03T03:31:02.202Z Reads: 139

```
What exactly is your setup now? 😂
```

---
## \#675 Posted by: Andy87 Posted at: 2019-04-03T04:53:00.543Z Reads: 141

```
👍

I break a lot of shit as well and sometimes it makes me kind of thinking it’s a sign that esk8ing is not for me...but than I read your stories and how much you destroy and understand i‘m kind a lucky how less broke on me 😂👌

Looking forward to the video!
```

---
## \#676 Posted by: rich Posted at: 2019-04-03T10:04:56.782Z Reads: 142

```
I'm not afraid because it's DIY so a lot of things are fixable without high costs. Imagine we would ride commercial boards, that would suck and we could never ride because of external repairs :laughing:

I hate it when I destroy things but love to ride that this can happen, that's the best! It's really funny when I remember watching videos of @Nowind and thought what the hell is he doing. Why he is treating his board like his enemy, why he grinds the truck on the rail again, whaaat burn outs and that sliding must be very bad for the tires and so on.

Now I understand why :grin:

For comparison of some costs, last winter I went snowboading. A day ticket costs 43.50€ plus 20€ food and travelling costs so 80-100€ for a single day. For the same amount of money I could kill at least 8 tires or 1 motor and personally I enjoy it more to pay for destroyed parts than paying for a stupid day ticket. 

[quote="spei, post:673, topic:45377"]
Just maka sure u fix it to tyre with tape. It can slice your tube
[/quote]

Is it that sharp? Or because of the cuts on the sides you did? I would be afraid what happens when the tape stops sticking after a while :thinking:

[quote="DEEIF, post:674, topic:45377"]
What exactly is your setup now? :joy:
[/quote]

Not sure if this is a serious question :laughing: but same setup as before, just need new tires.
```

---
## \#677 Posted by: Andy87 Posted at: 2019-04-03T10:13:03.634Z Reads: 138

```
[quote="rich, post:676, topic:45377"]
last winter I went snowboading. A day ticket costs 43.50€ plus 20€ food and travelling costs so 80-100€ for a single day. For the same amount of money I could kill at least 8 tires or 1 motor
[/quote]

that´s a nice point of view :ok_hand::joy:

but to be fair, I hope to get way much more days on my esk8 than on the snowboard. Buying a "day ticket" for every weekend I´m out on my esk8 would be pretty exensive as well.

[quote="rich, post:676, topic:45377"]
I remember watching videos of @Nowind and thought what the hell is he doing.
[/quote]
:rofl: my thoughts as well when I just started with all that here.
I was crying to see the tires wearing down on the burn outs and asked myself, why...just why... isn´t that just expensive???

now I understand that way better... have a box of spare wheels at home and don´t mind to swap them all out during one season.
```

---
## \#678 Posted by: spei Posted at: 2019-04-03T10:40:47.325Z Reads: 134

```
[quote="rich, post:676, topic:45377"]
Is it that sharp? Or because of the cuts on the sides you did? I would be afraid what happens when the tape stops sticking after a while :thinking:
[/quote]

I made the cuts because its for bike applications and when I applied it in small tyres it was all curvy along sites. Than I applied [heavy duty tape](https://www.amazon.com/3M-Extra-Heavy-Duty-Duct/dp/B00H95LREW) so it wont move inside and just in case for peace in mind. It will stick forever, because u will have inflated inner tube so it will be pushed to tyre even more.
```

---
## \#679 Posted by: Pedrodemio Posted at: 2019-04-03T15:12:14.243Z Reads: 131

```
Hey @rich I had some ideas for a future board on my mind

How wide is your battery box, or even better, what’s the dimensions between the edges of the bindings on the center of the board?
```

---
## \#680 Posted by: rich Posted at: 2019-04-03T20:29:32.083Z Reads: 145

```
[quote="Andy87, post:677, topic:45377"]
Buying a “day ticket” for every weekend I´m out on my esk8 would be pretty exensive as well.
[/quote]

Haha yeah that would suck! But this thought also helps me to justify the overall costs.

[quote="spei, post:678, topic:45377"]
It will stick forever, because u will have inflated inner tube
[/quote]

Legit argument :ok_hand:

[quote="Pedrodemio, post:679, topic:45377"]
what’s the dimensions between the edges of the bindings on the center of the board?
[/quote]

Well in my case about 25cm (almost 10") with the brackets more inward. If they are mounted outward then 22cm.

![210442|690x388](upload://i73Nw53VR2mKHP7PaklGYX7GLRa.jpeg) 

Also keep in mind that in case of heel straps you maybe need a liitle more space so I would not exceed 22-23cm.
```

---
## \#681 Posted by: Pedrodemio Posted at: 2019-04-03T20:44:11.436Z Reads: 142

```
Thanks, my estimate from the diagrams for the deck were pretty close
```

---
## \#682 Posted by: banjaxxed Posted at: 2019-04-03T23:14:11.534Z Reads: 144

```
If ever there was a gear drive that needed a TPU bash guard it’s those poor fellas
```

---
## \#683 Posted by: rich Posted at: 2019-04-04T19:16:42.375Z Reads: 148

```
[quote="banjaxxed, post:682, topic:45377"]
TPU bash guard
[/quote]

Good reminder to mount them again. I had a problem with 2 threads which hold the drive guards, they are gone.

![151821eh|690x422](upload://jdMBINB5FpFE1jLutDzymsWjEcF.jpeg) 

It's my fault, the first times I used not enough Loctite on the screws and they came loose and took the impacts, I've also lost several bolts.

I replaced the 30mm bolts of the housing with 40mm so they stick out.

![002812|690x388](upload://5N8PTOcx9fXTJyMa8oXsG6G8w9A.jpeg) 

Then mounted the drive guards with slim nuts and plenty Loctite.

![004252|690x388](upload://y4cVEHKEUdiruP4F25jcWiA6rzx.jpeg) 

That should hold now, my only fear is if I ever bend the end of the bolts I can't unscrew them :laughing:

Yesterday late in the night I decided to open the second drivetrain for inspection.

The debris is just on the side and sticks to the grease. No dust on the gears, also the sealing ring was not perfectly aligned. But I didn't open the housings for 6 months so not bad at all when cleaning twice a year.

![013739h|690x388](upload://pfkbit9uEJxuZA6qR362PXS7VlX.jpeg) 

Degreased and reassembled everything, mounted the second drive guard and then fell asleep.

![031739h|690x388](upload://lt5pMUNbF7vMcglzn3H4bFfUNlV.jpeg) 

Today I replaced all tires and wanted to check a tube with several slime filled punctures if it's airtight. Well  it was not, after inflating it squirted the slime on me, ceiling, wall, carpet, curtain, monitor.... what a mess.

![170455|690x388](upload://wjyosg26F2rg7S2Awl7JA06Vo0u.jpeg)   

On the ceilings it's already dry, didn't see it before.


![205148h|690x388](upload://sKZSsIJw1Zz5qGSBTHfkg1RtSx7.jpeg) 

Damn but shit happens so I continued to reassemble with fresh tires and not so fresh tubes. 

![180216h|690x388](upload://rBnmZr0cfPN2xi6XkXtLOW0QUe3.jpeg) 

![180234h|690x388](upload://yyvIBKzD4mkD8jgWAFRHWvFDVTz.jpeg) 

All looked so fresh and clean until I went for a ride :grin:

![191850h|690x388](upload://zzR9tlUBlO9uFTVOjPe3vLOizED.jpeg) 

The new chinese tires are quite rough compared to the thinner MBS rubber compound but hey, they roll.... I forgot to check battery level so I had a walk of shame back home.

Mission completed, the next days I have to work but looking forward to more rides soon.
```

---
## \#684 Posted by: Andy87 Posted at: 2019-04-04T19:37:04.851Z Reads: 140

```
[quote="rich, post:683, topic:45377"]
The new chinese tires are quite rough compared to the thinner MBS rubber compound
[/quote]

Give them some miles go drive them in. Should get softer after some rides.
```

---
## \#685 Posted by: Pedrodemio Posted at: 2019-04-04T19:44:55.875Z Reads: 139

```
This last picture twisted my brain, at first it appeared that you had broken the deck in half :sweat_smile:
```

---
## \#686 Posted by: rich Posted at: 2019-04-04T19:54:36.423Z Reads: 137

```
True, I hope so.

[quote="Pedrodemio, post:685, topic:45377"]
at first it appeared that you had broken the deck in half :sweat_smile:
[/quote]

Now I can see it, too :joy:
```

---
## \#687 Posted by: DEEIF Posted at: 2019-04-07T05:14:31.784Z Reads: 133

```
What remote do you use?
```

---
## \#688 Posted by: rich Posted at: 2019-04-07T16:13:28.818Z Reads: 135

```
I'm using Steez remotes (Maytech MTSKR1512), they are expensive but the connection is very reliable. I had no luck with the new small Maytech remote (MTSKR1712) and think I won't use the winning remote because of reading bad things about it.
```

---
## \#689 Posted by: rich Posted at: 2019-04-08T14:26:36.856Z Reads: 137

```
Finally I could finish the video so here we go :grin:

https://youtu.be/STgSGXFGxmo
```

---
## \#690 Posted by: pjotr47 Posted at: 2019-04-08T14:46:28.958Z Reads: 139

```
Awesome video! I like to see what risks you take. 

What protection do you have?
```

---
## \#691 Posted by: rich Posted at: 2019-04-08T15:45:15.072Z Reads: 140

```
Thanks bro! Without protectors I wouldn't ride like this and there is always foam between my ass and the ground so usually it doesn't hurt :laughing:.

I made some pictures... btw who is that guy laying in my living room?

![165601|690x388](upload://9sYaZRliC16nCk7IlHBRjd4Ypuu.jpeg) 

![165846|690x388](upload://9Pi7gcYFivNxqSoW0L1HwasvcWf.jpeg) 

one more :joy:

![Protectors_1|562x500](upload://7JLewEdMRecaZxhsThe3e0VA5p5.jpeg) 

From head to toe:

* Axant MTB helmet (65€ amazon) 

* O'Neal Underdog MotoX vest with hard plastic shells (bought it used for 25€)

* HillBilly wrist guard full finger gloves (35€)

* CrashPants from china (on ebay 13€ | chinese XXL = european M)

* MotoX Knee-and shim protectors (25€ Louis)

* Batman Hitop shoes (on sale for 20€ because nobody wanted to buy them :joy:) 

So everything together including shoes is 183€ which is not bad. 

I always wear all protectors above which is sizzling hot in summer but I prefer sweating instead of ragged wounds.
```

---
## \#692 Posted by: pjotr47 Posted at: 2019-04-08T16:00:06.534Z Reads: 126

```
Many thanks for this list and pictures. I am going to take a look this evening what protection I also can use. 
I have a nice bike park 20km from my house. 
 And just sold my enclosure under my trampa and will go topmount  :slight_smile:
```

---
## \#693 Posted by: taz Posted at: 2019-04-08T16:11:32.843Z Reads: 127

```
[quote="rich, post:691, topic:45377"]
CrashPants from china (on ebay 13€ | chinese XXL = european M)
[/quote]

Ordered!!! lol
```

---
## \#694 Posted by: Sn4pz Posted at: 2019-04-08T16:20:57.449Z Reads: 130

```
[quote="rich, post:691, topic:45377"]
CrashPants from china (on ebay 13€ | chinese XXL = european M)
[/quote]

All the XXL are sold out... you think a US medium would qualify for XXXL? :rofl:
```

---
## \#695 Posted by: taz Posted at: 2019-04-08T16:24:17.000Z Reads: 137

```
I got the last one.
They have a size chart available on the listing.

https://i.ebayimg.com/00/s/ODAwWDgwMA==/z/nZsAAOSwPAxaH855/$_57.JPG?set_id=8800005007?size=76328&height=520&width=780&hash=351d543f3699728ee1f33dc2dbe884ca
```

---
## \#696 Posted by: taz Posted at: 2019-04-08T16:26:43.533Z Reads: 135

```
Here are the same pants but more expensive.

https://www.ebay.com/itm/Adult-Children-Roller-Skating-Crash-Pants-Hip-Bum-Saver-Impact-Padded-Shorts/183583900918?hash=item2abe7404f6:m:m1mcnPuvlkm-Hn_NiU7NNjw
```

---
## \#697 Posted by: Sn4pz Posted at: 2019-04-08T16:27:09.526Z Reads: 133

```
[quote="taz, post:695, topic:45377"]
I got the last one. They have a size chart available on the listing.

![](https://i.ebayimg.com/00/s/ODAwWDgwMA==/z/nZsAAOSwPAxaH855/%24_57.JPG?set_id=8800005007?size=76328&amp;height=520&amp;width=780&amp;hash=351d543f3699728ee1f33dc2dbe884ca)
[/quote]

Great, I found a listing with *maybe* the same item with 'speed shipping'
https://www.ebay.com/itm/Adult-Children-Roller-Skating-Crash-Pants-Hip-Bum-Saver-Impact-Padded-Shorts/183583900918?hash=item2abe7404f6:m:m1mcnPuvlkm-Hn_NiU7NNjw

E: beat me to it :sob:
```

---
## \#698 Posted by: taz Posted at: 2019-04-08T16:31:29.597Z Reads: 127

```
![](https://memegenerator.net/img/instances/57513702/my-google-fu-is-strong-you-have-much-to-learn.jpg)
```

---
## \#699 Posted by: Sn4pz Posted at: 2019-04-08T16:33:35.370Z Reads: 127

```
Much better formatting the second time :rofl: 

I'm just a slow creature :joy:
```

---
## \#700 Posted by: rich Posted at: 2019-04-08T18:03:46.603Z Reads: 132

```
Just came back from an evening ride :sunglasses:

[quote="pjotr47, post:692, topic:45377"]
will go topmount :slight_smile:
[/quote]

Nice! It's best when you can scratch the bottom of the deck without worries.

[quote="Sn4pz, post:694, topic:45377"]
you think a US medium would qualify for XXXL? :rofl:
[/quote]

Maybe :joy::rofl:

But joking aside, the 2XL is between M and L. Great that there is a 3XL available, should be between L and XL. But the material is stretchy anyway. The first times when wearing the stitching/seam is scratching/itchy but then it's gone.

[quote="taz, post:695, topic:45377"]
I got the last one
[/quote]

:laughing::ok_hand:
```

---
## \#701 Posted by: legend27 Posted at: 2019-04-08T20:47:04.626Z Reads: 128

```
[quote="rich, post:691, topic:45377"]
CrashPants from china (on ebay 13€ | chinese XXL = european M)
[/quote]

Ordered :slight_smile:

Thanks a lot!
```

---
## \#702 Posted by: rich Posted at: 2019-04-13T15:25:04.458Z Reads: 136

```
Had some troubles with my charge port, there was poor (loose) contact. It got very hot and the charge cable as well, I mean really hot. I soldered a new connector to the charger because the old (in the middle of the pic) melted and the outer plastic ring expanded. Meanwhile ghetto charged with adapters, I have to change the charge port as well but am not sure yet if I keep the Pelicase. 

![190247e|690x388](upload://43h8W5OanT9rHdUL8hPLDaPRw2x.jpeg) 

For the 12s6p I have different options. The easiest way is to make one brick which would fit into the Pelicase. The most beautiful way would be 3x4s segments side by side. But the spotwelding gets complicated and I would need to make a segmented enclosure (not a master in enclosures), also waterproofing is difficult.

Also I was thinking about Sanyo NCR20700B cells which wouldn't fit in the Pelicase and have more voltage sag but crazy range. 1101Wh (4.5kg) with 12s6p compared to 777Wh (3.6kg) with 18650. Haven't decided yet. 18650 would be VTC6 or 30Q.

However if I use a wider enclosure I have to mount the MBS heelstraps the other way.

This is how the heelstraps should be mounted (as in manual), ratchets and long ladder straps towards the middle ofhe board.

![220016h|690x388](upload://i6yGAjBZb1VsjHUagUykO2Pw8Vl.jpeg) 

It works great but the ratchets need space when closing/opening, bad for a wide enclosure.

![210843h|690x388](upload://JB1LsS1poyKuUFiIqQ5utO9GAc.jpeg)  

First problem is that the ladders are outside on the long strap and inside on the short one, furthermore it looks a bit different (checked it too late). I tried the ratchet on the short strap (could be flipped).

![220157h|690x388](upload://vrOXI8QUVMvgxvueghP2TVgJFwK.jpeg) 

Bad thing is that it is impossible to remove the heelstrap anymore because of this "barbed hooks" 

![134705e|690x388](upload://i3i8Ny7gmC3yx6NqiRICaoMxkIB.jpeg) 

I had to dremel them away...

Finished the first heelstrap but it was better before, it is not centered anymore because the short ladder strap is too short when the ratchet is outside. Damn but I really wanted to ride so I wanted to finish the second heelstrap to test it in real life, just the last ladder strap and SNAAAAP! :sob:

![181225h|690x388](upload://smWM3fut8yPicsoulKS0ihZeNyj.jpeg) 

![183004h|690x388](upload://8xZJpN68uQBCV1bYnQ4CGQTfOxh.jpeg) 

Shit!
```

---
## \#703 Posted by: Mobutusan Posted at: 2019-04-13T19:16:48.866Z Reads: 129

```
Dude, that sucks. Did you buy those new from @MBS? Maybe they can send you a replacement ratchet or strap. I don't use my heel straps very often yet, but I was under the impression that you set the heel strap position and leave it static, then use the toe strap to get in and out of the bindings and adjust the tightness. Obviously, that won't work with a busted ratchet but seems like you wouldn't need the clearance so much for the heel ratchet since it doesn't change very often.
```

---
## \#704 Posted by: rich Posted at: 2019-04-13T19:57:58.941Z Reads: 131

```
I bought them last July from ATBShop in UK, this was the second time I ever touched this ratchet. You need a lot of force to close them (plus keep the other hand on the ladder strap), maybe would be better made of metal :thinking:

[quote="Mobutusan, post:703, topic:45377"]
I was under the impression that you set the heel strap position and leave it static, then use the toe strap to get in and out of the bindings and adjust the tightness.
[/quote]

I know many do it like that but I prefer to have the toe straps static and open/close the heelstraps only. Furthermore I route the wires on the rear binding.

[quote="Mobutusan, post:703, topic:45377"]
busted ratchet
[/quote]

The broken ratchet is the small one, the big metal ratchet for opening/closing is fine.
```

---
## \#705 Posted by: Pedrodemio Posted at: 2019-04-13T20:27:47.005Z Reads: 127

```
I'm having the same nightmare with the charge plugs, melted a lot of them, I can't find anywhere a quality P4 male plug, all of them are cheap made and can't handle the current

I've given up on them and moved up to GX12 or GX16, I would suggest doing the same, them you can charge way faster without worrying
```

---
## \#706 Posted by: pjotr47 Posted at: 2019-04-13T21:45:24.457Z Reads: 124

```
I read 12s6p.... What enclosure do you have? I am going to fit a 12s7p with a 100A smart bms inside a peli 1150 case :see_no_evil: thinking of charging with a 15A charger or more. 

Btw: for your charge port problem. Use a xlr plug :slight_smile:
```

---
## \#707 Posted by: rich Posted at: 2019-04-14T06:19:36.732Z Reads: 131

```
[quote="Pedrodemio, post:705, topic:45377"]
I’m having the same nightmare with the charge plugs, melted a lot of them
[/quote]

At how many amps do you charge?
I charge at 4A but recently ordered a 8A charger with 5.5x2.1mm plug :joy: for science, wanna see how hot it becomes. I plan to change the charge plugs and ports to bigger ones but not sure which one.

[quote="Pedrodemio, post:705, topic:45377"]
GX12 or GX16
[/quote]

I did some research and everything I found was rated for 5A only. Also these connectors were not made for electricity.

[quote="pjotr47, post:706, topic:45377"]
Use a xlr plug :slight_smile:
[/quote]

Huuuuuuuge :pensive:
Do you know the amp rating for these? Generally would be interesting to know ratings for different charge connectors.

Maybe I do it DIY with XT30, nice size....

[quote="pjotr47, post:706, topic:45377"]
I read 12s6p… What enclosure do you have?
[/quote]

Pelicase 1150 but I want to get rid of it. 12s7p is possible but not with BMS on the side, on the top I have not enough space because of voltmeter.

Furthermore it's 12s6p mainly because of the weight, would love to have more range but not more weight. I made a decision and will go with a 18650 brick of VTC6 which cost only about 30€ more than 30Q right now.

The Pelicase weights 0.8kg, so 3.5kg in total with my actual 8Ah lipo and BMS. I need to save weight so I'll make an enclosure made of 2mm ABS to keep the total weight at around 4kg for 18Ah compared to 3.5kg for 8Ah which is a quite crazy difference in range.

Ironically the new DIY box should be even smaller in width than the Pelicase so no need to flip the heelstraps and I broke the ratchet for nothing, damn.

[quote="pjotr47, post:706, topic:45377"]
15A charger
[/quote]

:stuck_out_tongue_closed_eyes::crazy_face:
```

---
## \#708 Posted by: Pedrodemio Posted at: 2019-04-14T14:25:36.335Z Reads: 126

```
5A, good luck with 8A 😄 keep a fire extinguisher close

I see a lot of chargers coming with the GX series, true, they are 5A each pin, but you can get the 4 pin version and use two pins in parallel
```

---
## \#709 Posted by: rich Posted at: 2019-04-14T15:01:09.110Z Reads: 130

```
[quote="Pedrodemio, post:708, topic:45377"]
good luck with 8A :smile: keep a fire extinguisher close
[/quote]

Is this close enough? :joy:

![163313|690x388](upload://eBuiMphXUoxO3P3ub9sO5gwc9kN.jpeg) 

Hmmm just realized the extinguisher expired in 2009 :laughing: I'm getting old and should buy a new one.

[quote="Pedrodemio, post:708, topic:45377"]
but you can get the 4 pin version and use two pins in parallel
[/quote]

That's pretty damn clever bro and sounds like the perfect solution :smiling_face_with_three_hearts:. I never thought about that but start searching for 4pin GX12 right now.

https://www.aliexpress.com/item/2PCS-set-GX12-2-3-4-5-6-7-Pin-Male-Female-12mm-L88-93-Circular/32956363924.html?spm=2114.search0104.3.8.1bd978a5qSowdc&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10068_10547_319_317_10548_10696_10084_453_10083_454_10618_10304_10307_10820_10821_537_10302_536_10059_10884_10887_321_322_10103,searchweb201603_90,ppcSwitch_0&algo_expid=0ab432a1-58e4-4fd8-95b9-0c56cb2d428c-1&algo_pvid=0ab432a1-58e4-4fd8-95b9-0c56cb2d428c

Maybe the rubber cap is better because with the metal one a short is possible

https://www.aliexpress.com/item/2pcs-Dust-Cover-for-GX12-12mm-Aviation-Plug-Connector-Waterproof-Rubber-Metal-Cap/32833367491.html?spm=2114.search0104.3.66.1bd978a5qSowdc&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10068_10547_319_317_10548_10696_10084_453_10083_454_10618_10304_10307_10820_10821_537_10302_536_10059_10884_10887_321_322_10103,searchweb201603_90,ppcSwitch_0&algo_expid=0ab432a1-58e4-4fd8-95b9-0c56cb2d428c-9&algo_pvid=0ab432a1-58e4-4fd8-95b9-0c56cb2d428c

I have to dig further, there are thousands of different combos available but this is a perfect solution, thanks a lot!

@pjotr47 needs a 6-pin for 15A :smile:
```

---
## \#710 Posted by: Andy87 Posted at: 2019-04-14T15:35:43.353Z Reads: 124

```
[quote="rich, post:709, topic:45377"]
needs a 6-pin for 15A
[/quote]

Or just use a xt60 with panel mount and 3D print or silicon form your own waterproof cover. Easy thing, no troubles.
```

---
## \#711 Posted by: Pedrodemio Posted at: 2019-04-14T15:57:25.116Z Reads: 125

```
Since they are cheap I bought a bunch, GX12 and GX16 in 2, 4 and 6 pins, and rubber caps for both

I plan to use the GX12 6 pin for sensor wires
```

---
## \#712 Posted by: pjotr47 Posted at: 2019-04-14T19:48:06.874Z Reads: 138

```
[quote="rich, post:707, topic:45377"]
I charge at 4A but recently ordered a 8A charger with 5.5x2.1mm plug :joy: for science, wanna see how hot it becomes.
[/quote]

Lol 8A with a jack. The max amp is around 5A for such a connector.

[quote="rich, post:707, topic:45377"]
Huuuuuuuge :pensive: Do you know the amp rating for these? Generally would be interesting to know ratings for different charge connectors.

Maybe I do it DIY with XT30, nice size…
[/quote]

That's what she said :stuck_out_tongue:... a xlr port is not the smallest but it is nice if you have room. I think they can do around 10A max.

xt30 is indeed a nice size.

[quote="rich, post:707, topic:45377"]
Pelicase 1150 but I want to get rid of it. 12s7p is possible but not with BMS on the side, on the top I have not enough space because of voltmeter.
[/quote]

Oh, a 12s7p is a very nice fit in that peli 1150 case. I have finished today my 12s7p with a 60A bypassed smart bms. 100A in mail :) 

![image|281x500](upload://vmmC2atPG3W86oo6DMk6JxNAubR.jpeg) ![image|281x500](upload://29rk4KdgeFo1iDRprfdFLKGr8nI.jpeg) 

If you want I can check out the weight for that pack incl enclosure.

[quote="rich, post:707, topic:45377"]
:stuck_out_tongue_closed_eyes::crazy_face:
[/quote]
15A charger crazy? I was even thinking of a 30A adjustable (voltage and current) charger. But that would break my bank...

[quote="rich, post:709, topic:45377"]
Hmmm just realized the extinguisher expired in 2009 :laughing: I’m getting old and should buy a new one.
[/quote]
Yeah please buy a new one :rofl: 
I tried once 
to put out a fire with an expired fire extinguisher. So that thing did nothing at all. Fortunately I got out on time. I had a headache and a blue tongue for 4 days.


[quote="rich, post:709, topic:45377"]
@pjotr47 needs a 6-pin for 15A :smile:
[/quote]

Lol, I am just waiting on [this](https://www.aliexpress.com/item/1Set-WP20-4Pin-Waterproof-Chassis-Panel-Mount-Aviation-Plug-Cable-Connector-Plug-Socket-30A-500V/32764198104.html?spm=a2g0o.cart.99999999.297.56073c00VoBgQk) socket.

It is 4pin and can do 30A with no problem.
![image|511x500](upload://zMaMs8mpkjgWOZZ9o3leZIfclcv.jpeg)
```

---
## \#713 Posted by: taz Posted at: 2019-04-14T19:55:38.458Z Reads: 130

```
I have been thinking about a 8A charger.
So far I am leaning towards a XT30 or similar charge port. I find the XLR type ports unnecessarily big and complicated.

I can always make an XT30 to barrel plug adapter to use my other chargers.
```

---
## \#714 Posted by: spei Posted at: 2019-04-14T19:59:04.016Z Reads: 126

```
Apparently there is [DC 5.5x2.1 that is rated for 10A](https://www.aliexpress.com/item/5pcs-10A-5-5-mm-x-2-1mm-DC-Power-Jack-Socket-Female-Panel-Mount-Connector/32881008067.html?spm=2114.search0104.3.1.15214487sIGdn8&ws_ab_test=searchweb0_0,searchweb201602_5_10065_10068_10843_319_10059_10884_317_10887_10696_321_322_453_10084_454_10083_10103_10618_10304_10307_10820_10301_10821_537_536,searchweb201603_90,ppcSwitch_0&algo_expid=4e941172-8cf9-460d-a1f6-43e3a80a2043-0&algo_pvid=4e941172-8cf9-460d-a1f6-43e3a80a2043&transAbTest=ae803_4)
```

---
## \#715 Posted by: pjotr47 Posted at: 2019-04-14T19:59:26.355Z Reads: 126

```
A xlr port complicated? It is just solder 2 wires and you are ready to go... The thing is that a xlr port is easy to mount. a XT 30 not
```

---
## \#716 Posted by: pjotr47 Posted at: 2019-04-14T20:01:12.091Z Reads: 122

```
I have a bunch of them at home. I always use them in the packs I sell. Those are from the manufacturer rated for 5-6A max. This is just a Aliexpress seller who placed 10A on it.
```

---
## \#717 Posted by: spei Posted at: 2019-04-14T20:02:47.004Z Reads: 123

```
[quote="pjotr47, post:716, topic:45377"]
Those are from the manufacturer rated for 5-6A max
[/quote]

Noted, That is a good thing to know!
```

---
## \#718 Posted by: taz Posted at: 2019-04-14T20:09:52.316Z Reads: 121

```
I was referring to the fact that in order to get 30A on an XLR  connector you would have to use a 6pin version and even then the nominal current rating would be 22.5A.
```

---
## \#719 Posted by: Pedrodemio Posted at: 2019-04-14T20:30:38.407Z Reads: 128

```
The main problem is the male one 

The connection between the pin and the tab and between the barrel and the negative is just press fit, shouldn't call that since it's very loose, as you use the degrades and heats it even more until it melts away

![image|690x392](upload://9Z4tXWzZkmfEZsGnPSAfEOBWP6t.jpeg)
```

---
## \#720 Posted by: spei Posted at: 2019-04-14T21:06:45.543Z Reads: 127

```
@pjotr47 @Pedrodemio So what would be your recommendation for the 5A+ With the possibility to seal port from dust and mostly the water.
```

---
## \#721 Posted by: MBS Posted at: 2019-04-14T22:07:19.360Z Reads: 129

```
Bummer!  If you want the ratchets on the outside you need to unscrew the entire Heel strap assembly (including ladder straos) from the F5 bindings and flip the entire assembly.  That's because the two different types of ladder straps are NOT compatible with the two different types of buckles (ratchet buckle vs. cam buckle).  The ratchet buckle only works with the ratchet ladder strap (teeth on outside of strap), and the cam buckle only works with the cam ladder strap (teeth on underside).  In addition to the slight width different, the actual thickness of the straps is different (the reason that cam buckle broke).    Unfortunately, unlike the ratch buckle, that cam buckle can't be replaces with our replacing the whole strap.  But if you can find the position you want using the other foot, then you can probably lock that broken cam lock down permanently.   Good luck!
```

---
## \#722 Posted by: Pedrodemio Posted at: 2019-04-14T22:33:07.898Z Reads: 127

```
My bet is on the GX series with a rubber cover

And on the inside of the enclosure completely cover it with epoxi
```

---
## \#723 Posted by: rich Posted at: 2019-04-15T12:11:07.569Z Reads: 132

```
[quote="MBS, post:721, topic:45377"]
you can probably lock that broken cam lock down permanently
[/quote]

It took some minutes and several pliers but I could close it. I'm afraid this won't work a second time.

![132823h|690x388](upload://ztibfAVK4sBTN6mYbTt5xgqGSZI.jpeg) 

I just walked home (walk of shame) after a pre-work ride (empty battery) and the heelstrap holds. But my puffed lipo is getting warm and the voltage drops from 3.6V to 3.2V within a blink of an eye, that sucks. Can't wait for the new battery.

According the charge plug, gonna use 4pin GX12 and won't charge with 8A with the old charge port.

[quote="pjotr47, post:716, topic:45377"]
This is just a Aliexpress seller who placed 10A on it
[/quote]

The seller of my charge ports states 12A :rofl:

BTW the 12s7p looks good and has a nice fit :+1:, I plan do build it similar. Did you use 25x0.2mm or 0.15mm strips? I think I go with 25x0.2mm single layer.
```

---
## \#724 Posted by: pjotr47 Posted at: 2019-04-15T19:52:50.997Z Reads: 130

```
Yeps 25mm x 0.2 :slight_smile:

I use also a smart bms and it is awesome   ![image|281x499](upload://g5GkqzzNlVAIuqVYkj39FZWTl9F.png)
```

---
## \#725 Posted by: rich Posted at: 2019-04-16T22:52:09.678Z Reads: 129

```
Today I had a nice sesson at dirt park trying to improve jumping skills and airtime. There is a table which I never could jump over, now I need 10-20cm more and it's accomplished. That's why I started to remove all stones to be able to accelerate more to clear the table but it needs more treatment. I did this with full body armor and helmet and was sweating like a pig. Tomorrow I buy a shovel and broom to finish the work, hopefully I can jump over the table soon.

Also I was jumping a small double with about 1m gap, I never jump gaps because you know... that can hurt badly! Despite pissing in my pants I jumped it 4 times and succeeded 3 times :smile:

I contacted ATBShop regarding the broken cam buckle and hope I can get a replacement.

[quote="MBS, post:721, topic:45377"]
the actual thickness of the straps is different (the reason that cam buckle broke)
[/quote]

After reading your post the second time I realized that I didn't read this sentence properly before.

The cam buckle broke while opening on the original cam ladder strap. I only tried on the other binding if the ratched buckle works with a flipped cam ladder strap. 

After riding 2 times with "wrong" mounted heelstraps (ratchet buckles outside like Trampa) I must say I don't like it, it is quite a difference and I need to switch to the correct mounting with ratchet buckles inside which is much better, there is a reason why MBS have the ratchet buckles inside.. Unfortunately I can't switch right now because of the broken cam buckle. Sorry for writing buckle 10 times :laughing:

Hopefully soon like this again...
![172633h|690x388](upload://kBZVHigrllkDf87zJz736ibtFBo.jpeg)
```

---
## \#726 Posted by: MBS Posted at: 2019-04-16T23:25:07.250Z Reads: 124

```
Noted regarding the cam lever breaking while opening it on the original strap (factory spec).  In that case it'd be covered by warranty.  I just saw the straps swapped and assumed that was the cause.  Rad build by the way...
```

---
## \#727 Posted by: rich Posted at: 2019-04-16T23:47:58.130Z Reads: 130

```
I think I had the thumb on the tip of the buckle only (because of needed force) that means maximum stress for the buckle. From now on I gonna put the force spreaded to avoid that it happens again.

[quote="MBS, post:726, topic:45377"]
Rad build by the way…
[/quote]

Thanks a lot :blush:

I love the F5 bindings and heelstraps, they fit so nice, are very comfy and the heelstraps are perfect size. I don't have to adjust them. Smaller heelstraps need adjusting after 1-3 jumps because they move down. (MBS heelstraps also move down a little bit but it makes no difference because of the size)

I am thinking about a build for jumping only, maybe I'll try a stiffer MBS deck for better control. If I had the money I would buy the new Matrix II with metal baseplates straight away but I'm afraid I have to wait some time for financial healing.
```

---
## \#728 Posted by: rich Posted at: 2019-04-18T12:32:48.420Z Reads: 131

```
WTF I did it and now I can jump over the table without touching the platform, what a great feeling :smile:

![414|690x388](upload://j8ETxwbcP8hnBlp3d0geQEXh3kW.jpeg) 

But let's start from the beginning, I bought a shovel and (shitty) broom to end this rocky mess

![115935h|690x388](upload://9w6OAORgs43Zgs1z3hXCQeEGrJX.jpeg) 

![121756h|690x388](upload://q2tVNLkGgSSIZRpZHid51kOrToM.jpeg) 

![115827h|690x388](upload://eNcar0yPpggLchlSDb14UH8HMWt.jpeg) 

![120342h|690x388](upload://zxwwp9OX7BY0gjPu9S0D0DRUlEd.jpeg) 

After hard work it looks like a dream

![120944h|690x388](upload://2V1gBM8znXv7D8DcptZuaUaJHB3.jpeg) 

First step done so it was time to repair and (re-)shape some kickers

![123102h|690x388](upload://dhe6JaFEF94SfhAju4XJqiBTXxo.jpeg) 

After enough digging I desperately needed some water of the lake, it's a 5 minutes ride to get there.

![125132h|690x388](upload://tTIPetRXAWC1ypNXXOpVKzTOnB9.jpeg) 

Waaater, niceness

![131629h|690x388](upload://yTf8CzE5UQ2QOTfoazkIVIWIQYo.jpeg) 

![131612h|690x388](upload://hn4d4LxTRfjDqj6r2d80v41bq3n.jpeg) 

After fixing there are now 4 different kickers to choose

![133715h|690x388](upload://mnYmxY35heBCvTN2WwkOqdfZ0qn.jpeg) 

After 2-3 hours curing it was time to test it, I was afraid it is too loose for riding it but the kicker kept the shape nicely.

I've never jumped it before because it was too dangerous, now it's just great. Next time I have to re-shape the landing area.

![247|690x388](upload://64zOTZIgUsOxbVU2IYi1kOGLp41.jpeg) 

Then there was this little kicker which was full of plants which I removed and then brought the shape back to life.

![133251h|690x388](upload://jg4Z63MIdQwIohNbxE9M632Y98H.jpeg) 

I always thought only stupid people would try this kicker with a gap and a small step up. But why should I fix this kicker without jumping it? :thinking:

![133303h|690x388](upload://hPsdNlxtNjPEYa71x39bUakolQd.jpeg) 

Well I jumped it 3 times, the first 2 times I crashed but then it worked :laughing: It is so sick! I have to make it more wide and safe for MTB.

I have the biggest respect for shapers and builders because now I know how much work it really is. I was digging and brooming for 5 hours to achieve some improvements. It is hard work but the feeling afterwards is priceless when you ride the smooth fresh course with a grin in your face.

![956|690x388](upload://motfK9gN7LTdKnj8HB9lN7WdieL.jpeg)

I need a bigger broom and more tools for different treatings and removing bigger stones.

I did record some footage but unfortunately the battery was empty before doing sick and higher jumps. The camera started recording but shut down after 1 minute because of low battery. That happened 4 times until I realized it, so I have only a test jump on camera on this takes. I need to record everything again :face_with_raised_eyebrow:

Have a nice day!
```

---
## \#729 Posted by: Andy87 Posted at: 2019-04-18T12:53:20.896Z Reads: 123

```
looks like you always have the dirt park for your own :sweat_smile: seems to be a great time there!
```

---
## \#730 Posted by: taz Posted at: 2019-04-18T13:08:20.663Z Reads: 126

```
[quote="rich, post:728, topic:45377"]
![414.jpg](https://www.electric-skateboard.builders/uploads/db1493/original/3X/8/6/8623e653787d4a3652b73afe1f4961c511120d46.jpeg)
[/quote]

How do I like this post multiple times ???
```

---
## \#731 Posted by: Andy87 Posted at: 2019-04-18T13:09:16.974Z Reads: 122

```
i liked your post to like @rich post a second time... should work like this!
```

---
## \#732 Posted by: taz Posted at: 2019-04-18T13:10:25.515Z Reads: 122

```
Well, I also liked it in the pictures thread but only 2 likes are not enough for that pic.
```

---
## \#733 Posted by: Andy87 Posted at: 2019-04-18T13:12:08.816Z Reads: 127

```
definitly! just imagine the video would record as well... 

good motivation for the summer, for me for sure.
```

---
## \#734 Posted by: rich Posted at: 2019-04-18T13:34:10.859Z Reads: 134

```
[quote="Andy87, post:729, topic:45377"]
looks like you always have the dirt park for your own :sweat_smile:
[/quote]

Yeah often but not every time

![135|690x388](upload://3cZTx1LAKVpOZIibFVsZiQT2ScI.jpeg) 

I met a 13-year old talented kid, we were jumping in a train :ok_hand: and played the game S.K.A.T.E. It was the same day him and me succeeded to jump over the table.

![404|690x388](upload://4DHv9aWkXA7tLybKPeGKAPoM5Pj.jpeg) 

[quote="taz, post:730, topic:45377"]
How do I like this post multiple times ???
[/quote]

Haha thanks bro, you want more pics? Here we go

This is a step up which I can jump over since 2 weeks

![650|690x388](upload://yEYa64nqkjiWLWNKUs44PgCvYSW.jpeg) 

![825|690x388](upload://muIizhFG8KwEn2VMRb01LZNZxBB.jpeg) 

![163|690x388](upload://dnLkPeWlzk02G2hSbZMWSOQAfJe.jpeg) 

[quote="Andy87, post:733, topic:45377"]
just imagine the video would record as well…
[/quote]

All pics are screen shots of 60fps video footage before the battery was too low for the higher/better jumps :wink:.

I don't know but since the "Nollie challenge" of @DanSkates I always jump like this even when I don't want to, also it feels better to jump with style :laughing:

![720|690x388](upload://rKqb4SThJd7DRj3rq88Z4IigYJ2.jpeg)
```

---
## \#735 Posted by: pjotr47 Posted at: 2019-04-18T13:50:43.540Z Reads: 124

```
Bruh I wish I had such a nice track at my town
```

---
## \#736 Posted by: Okami Posted at: 2019-04-18T14:38:22.075Z Reads: 133

```
Yeh that picture with big air / jump is awesome.. 

Could almost save it and use as screen wallpaper.

 Too bad it is not me who does the jump :smiley: otherwise ppl would later ask is it me and would have to say I just took it from internet :smiley:  

I guess part of riding now is to train for the Paris esk8 cup? :slight_smile: 

At least I guess that will be a blast for everyone who can attend it and go with their boards
```

---
## \#737 Posted by: rich Posted at: 2019-04-21T20:22:20.912Z Reads: 136

```
[quote="pjotr47, post:735, topic:45377, full:true"]
Bruh I wish I had such a nice track at my town
[/quote]

Yeah I'm really lucky because it's only a 4 minutes ride from home to dirt park :sunglasses:

Unfortunately it's never in a good shape because nobody maintain this park, that's why I started to do it. After rain there are big holes and other problems which needs to get fixed. I was not that often there in the past.

If you think it's a great park you have to see how it looked some years ago before I was riding there :face_with_raised_eyebrow:

![Dirtpark_2012|690x379](upload://8g5RiEhFRvZRA3DeQqRjFoXj43s.jpeg) 

It's still great but dirt needs more maintainance and is not that smooth as wood kickers which I've never tried so far.

[quote="Okami, post:736, topic:45377"]
Could almost save it and use as screen wallpaper.

Too bad it is not me who does the jump :smiley: otherwise ppl would later ask is it me and would have to say I just took it from internet :smiley:
[/quote]

Hey there is no face visible so it could be you :+1: 

I found time to visit the dirt park again to pratice and shot more video footage. I think I have to go there one more time before editing the video. 

New day, new broom. Can you imagine how people look at me when riding with a broom (or last time with shovel and broom)? :laughing:

![175309h|690x388](upload://kmciXbEcAkRn0oRkaE0cCJCudp4.jpeg) 

This time I jumped a lot with backside grabs to have at least a second jumping style.

![820|690x388](upload://iqFnmPkvnob2PPjLiKNQCPPMakn.jpeg) 

![616|690x388](upload://5adKU01ONmdCelV1w6pV71x28HF.jpeg) 

![494|690x388](upload://bvPoVI7SMtUXHpuvdJw8TpddJP.jpeg) 

This kicker with a step up I've only tried once in the past and it hurted a lot after crashing but it was time to face the fear. At least I didn't crash and I can reach the platform but not the landing area yet. I need more speed but it's difficult to reach it because there is a small table before.

![802|690x388](upload://s9avisAdQ0zy5uVBhdrJ2FpUb1N.jpeg) 

This was my highest jump ever and I thought I gonna die but could land it safely. I was overshooting and flying to the skye because of too much speed. 

![450|690x388](upload://nAsErURr2FddfirikXQ6wxSjeNb.jpeg) 

I also get some kind of wobble on the front truck when riding faster to jump higher, had some almost crashes. The whole board starts swinging left and right and it's hard to keep it in straight direction. The problem only happens when riding down the steep "starting hill", it is very bumpy and aslope in different directions. After adding pre-tension on the elastomere dampers it was better, need to test more next time.

My second SK8 motor starts to make bad noises, too. I'm afraid I have to change both motors in the near future. On bumpy terrain they are very loud like there is something loose.
```

---
## \#738 Posted by: taz Posted at: 2019-04-21T20:26:24.371Z Reads: 124

```
Richard, I think I speak on behalf of most of us when I say that you are taking this eMTB thing on another level.
```

---
## \#739 Posted by: pjotr47 Posted at: 2019-04-21T20:34:24.657Z Reads: 132

```
[quote="rich, post:737, topic:45377"]
Yeah I’m really lucky because it’s only a 4 minutes ride from home to dirt park :sunglasses:
[/quote]

You make me jealous... only 4 minutes? The closest bike park (maybe the only one in 60km around me) is 25km from me with my board. With the car it is 35km and look like this :/ ![image|500x500](upload://8Qs4r2ZWSBccQ5eaGR2rtKccVVY.jpeg) 

[quote="rich, post:737, topic:45377"]
Unfortunately it’s never in a good shape because nobody maintain this park,
[/quote]
I think that applies to many bike parks.


I fully agree with @taz ....


 all those EMTB boys want to have such a dope track in their town :stuck_out_tongue:
```

---
## \#740 Posted by: MBS Posted at: 2019-04-21T23:47:34.731Z Reads: 123

```
That's so sick!
```

---
## \#741 Posted by: rich Posted at: 2019-04-22T00:16:28.853Z Reads: 131

```
[quote="taz, post:738, topic:45377, full:true"]
Richard, I think I speak on behalf of most of us when I say that you are taking this eMTB thing on another level.
[/quote]


Thank you so much, feeling honored :blush:

But compared to other "real" MTB-freestyler (non-electric) it's not really that rad even when it feels like that :laughing:

My dream is to jump bigger kickers but I'm not ready yet at least not without jumping in a foam pit before. 

[quote="pjotr47, post:739, topic:45377"]
You make me jealous… only 4 minutes?
[/quote]

Yes but prepare yourself for following...... :joy:

This skate park is 1 minute away from my flat (full throttle 25 seconds)

![958|690x388](upload://bQEAMUlEm0GjnR6gDZ5M2Qpe0eB.jpeg) 

To reach this BMX track it takes 5 minutes

![596|690x388](upload://e80bBpy20k8tgfmr7IskEtwQ2SS.jpeg) 

This skate park/pump track is a 10 minutes ride

![873|690x388](upload://1kU3cFzWS8sWwEClp8itSVm982P.jpeg) 

This BMX course is a 15 minutes ride (but I got banned, it's a private association which accept bicycles only) but gonna ride there again. Catch me if you can.

![bmx1|690x316](upload://4fd1PQ1TQPbdzZZfJntzF0VCNZI.jpeg) 
![bmxV2|690x388](upload://pePXEubIAmSAoU92QkgTkHG0cuP.jpeg) 

Because I wrote "foam pit", I totally forgot the sick Dirtgarden which I could reach within 15-20 minutes. I feel motivated to finally go there and see it in reality. They have fresh foam in their pit since 1 month so no reason to hide (the old looked disgusting). 

![10868214_1565505003661950_2709507757711792940_n|690x412](upload://6TNHKIv6Vu3BwvFYBu6Q9FPHCl7.jpeg)

![1_0|666x500](upload://yEY7s5RpxCM5E6YiQsIIvIbGaxN.jpeg) 

![1511285_1444679539077831_2144088371_n|407x500](upload://gnW4Bdbe8owI29uySzKgWQPaB8z.jpeg) 

Sick shit kicker on the left side, foam pit on the right side

![dg1|690x344](upload://oXoowbPaYRxDLmDnzvhq1bT0N7c.jpeg) 

WTF! :open_mouth:

![dg2|690x344](upload://e8Dz7waZ4uK5RgG3sAGa7ZpkRIw.jpeg) 


Posted this video last year already but this year it's definitely time to stop watching and start riding at dirtgarden.

https://youtu.be/U9eU76j-SZE



[quote="pjotr47, post:739, topic:45377"]
all those EMTB boys want to have such a dope track in their town :stuck_out_tongue:
[/quote]

Group ride (jump ride) in Vienna? :wink: I'm there...

[quote="MBS, post:740, topic:45377, full:true"]
That’s so sick!
[/quote]

Thanks a lot Joel :hugs:
```

---
## \#742 Posted by: taz Posted at: 2019-04-22T04:48:33.667Z Reads: 126

```
[quote="rich, post:741, topic:45377"]
But compared to other “real” MTB-freestyler (non-electric) it’s not really that rad even when it feels like that :laughing:
[/quote]

I get what you are saying and I have the utmost respect for these guys.

However jumping with a 15-20kg weight strapped to your feet , is a whole different ballgame and deserves its own respect.
```

---
## \#743 Posted by: rich Posted at: 2019-04-27T18:59:52.284Z Reads: 132

```
When the noise of your trucks remind you of your grandmother's doors it's definitely time to change the bushings :laughing:

https://youtu.be/Fq05V5bFdRc

Unfortunately one motor is quite loose and the play of the can/shaft sideways got worse so I'm afraid keep riding could harm the gears so it's time for a break :disappointed_relieved:. I'm trying to claim both motors at HK, wish me luck (because they are modified there is officially no warranty). 

At the right time I got my VTC6 cells for the 12s6p, still waiting for fishpaper from china (hopefully not forever).

![165110h|690x388](upload://pR4sxmLFuPTjiBOSHBreZjGOYSV.jpeg) 

Also ordered 4 Samsung 40T for a friend so I could compare them. Very good cells, better than any 18650 when looking at discharge curves. Unfortunately quite expensive, guess next year more affordable.

![165410h|690x388](upload://3XKndvP6J0wdffyAAgkCeNGzwQe.jpeg) 
![165454h|690x388](upload://y6PAirFQTVUap28VYjVxXQJU3yQ.jpeg) 
![165717he2|690x388](upload://yfsrPtRKoiEjHfqtERCTAXnWDkw.jpeg) 
![170035h|690x388](upload://cV2hLUzG48jNdzBXTvaQCU0YDNl.jpeg)
```

---
## \#744 Posted by: Andy87 Posted at: 2019-04-27T19:07:53.206Z Reads: 127

```
The end of the video 😂👌

How you decided about spot welder? You will go with the kweld?
```

---
## \#745 Posted by: rich Posted at: 2019-04-27T19:19:32.871Z Reads: 133

```
[quote="Andy87, post:744, topic:45377"]
You will go with the kweld?
[/quote]

Yes it's not mine but I can borrow it. I've infected some people with the esk8 virus in my town :grin:

![225912h|690x388](upload://49x8IWP9QVYoLRmLwBtM7Ws5Mj9.jpeg) 
![225459h|690x388](upload://lu789y2RebdgRfi08vbv0B11tWR.jpeg) 
![230027h|690x388](upload://xUeirpJojMtrB3IjONPLCUIN0pv.jpeg) 

Looks great only the nano-tech lipo is missing yet, hopefully he buys it soon :crossed_fingers:.
```

---
## \#746 Posted by: Andy87 Posted at: 2019-04-27T19:25:07.727Z Reads: 127

```
Looks pretty good. I looked the last days about the kweld as well, but unfortunately it’s not possible to get it delivered to Russia.
```

---
## \#747 Posted by: rich Posted at: 2019-04-27T19:29:42.752Z Reads: 128

```
If it helps I could order it and send it to you but in this case there is VAT added (within EU). The kweld is quite expensive and the prices on the homepage are without VAT so add 19% for total price. Just let me know.
```

---
## \#748 Posted by: Andy87 Posted at: 2019-04-27T19:40:20.710Z Reads: 128

```
Thx for the offer! I was talking one guy from the kweld company if there is a way to enable shipping to Russia. The problem is that he use an impulse module which can be used to build bombs, that’s why it’s restricted to import to Russia 🙄 I don’t understand why I than can order a sunkko or malectrics welder but better don’t risk any troubles. Might try my luck with the malectrics than. Should be fine too and a bit cheaper as well.
```

---
## \#749 Posted by: rich Posted at: 2019-04-29T21:48:09.274Z Reads: 135

```
[quote="Andy87, post:748, topic:45377"]
The problem is that he use an impulse module which can be used to build bombs
[/quote]

OK now we know what the guy was doing before building the spot welder :joy:

Little progress on the 12s6p, glued the parallel cells first with CA. Normally it sticks like hell but for some reason this time not, no idea why it is flexible afterwards, maybe they changed the material of the heat shrink.

![013020h|690x388](upload://x5rh6hHqQWZIQpHyGZQztQwCBng.jpeg) 

Second step was to make the final bonding with sikaflex. Good thing is that because of the CA I could glue both sides of the cells at once without waiting 24 hours in between.

![224118h|690x388](upload://fJ4bh0X408vcg4Kgo0NwNH8WR1Q.jpeg) 

Still waiting for fishpaper :face_with_raised_eyebrow:
```

---
## \#750 Posted by: DEEIF Posted at: 2019-04-29T23:03:57.232Z Reads: 130

```
How much range are you expecting?! Also what should the weight of the battery be?
```

---
## \#751 Posted by: rich Posted at: 2019-04-30T00:41:14.620Z Reads: 134

```
Before my 8Ah lipos degraded I had 20km (12.4 miles) range so I expect at least 40km (25 miles) with the 18Ah li-ion.

According the weight, the 72 cells are about 3.5kg (7.7lbs) so I guess with glue, wires and BMS max. 4kg (8.8lbs).

For comparison, the 8Ah Graphenes with BMS and Pelicase 1150 weight 3.5kg (7.7lbs)

![123127h|690x388](upload://zaubfY2iUNyCyG8dDRCB3Rd8JXS.jpeg) 

Because I want as less weight as possible I get rid of the Pelicase which weights over 0.8kg (1.8lbs). Hope I can bend a light one out of 2mm ABS sheet similar to the vesc enclosure. This way I can double my range without adding much weight. At least that's the plan in theory.
```

---
## \#752 Posted by: DEEIF Posted at: 2019-04-30T02:26:26.896Z Reads: 131

```
Nice! 12s(6?)p of VTC 6 should be nice!
```

---
## \#753 Posted by: Andy87 Posted at: 2019-04-30T04:34:02.275Z Reads: 138

```
[quote="rich, post:751, topic:45377"]
8Ah lipos degraded I had 20km
[/quote]

I probably need to lose some weight 😂 i just can dream about that range. 14-18km out of 10Ah lipos is pretty much all I get.
```

---
## \#754 Posted by: slick Posted at: 2019-05-01T07:24:58.408Z Reads: 135

```
Gotta give it to you. Thats dedication right there. :grin:
```

---
## \#755 Posted by: taz Posted at: 2019-05-02T09:50:56.861Z Reads: 129

```
The pants just arrived. You can't beat them for the price but at 2XL they are a bit big for me. I should have gone for XL. Their size chart is definitely not correct, at least in my case.
```

---
## \#756 Posted by: Andy87 Posted at: 2019-05-02T10:50:11.474Z Reads: 124

```
More lamp for you than! 👌
```

---
## \#757 Posted by: rich Posted at: 2019-05-02T19:49:22.332Z Reads: 132

```
[quote="Andy87, post:753, topic:45377"]
i just can dream about that range. 14-18km out of 10Ah lipos is pretty much all I get.
[/quote]

The range I'm talking about is on flat terrain, 40% concrete, 40% gravel and 20% dirt and grass. Furthermore I discharge from 4.2V to 3.2V-3.5V.

[quote="slick, post:754, topic:45377"]
Thats dedication right there. :grin:
[/quote]

Thanks :grin:
[quote="taz, post:755, topic:45377"]
they are a bit big for me
[/quote]
Damn but at least better than too small :wink:

The glued parallel cells are still a bit flexible but I think when I glue all together that's gone. Meanwhile I think about how to route and connect all the wires.

![014839h|690x388](upload://h7ykUoh2Lk6xAcihfB11hS2MTvd.jpeg) 

![20190501_184357h|690x388](upload://lnM2URToh721DiJt83Y78rCNZFH.jpeg) 

It's crazy when you compare the size of the 8Ah lipo (with BMS) and the 18Ah li-ion pack.

![182340h|690x388](upload://ss4IBuws1caC2rOyHntqbM4zKtg.jpeg) 

![182419h|690x388](upload://arN49Xy5USje2lknJVLy0Y45CaP.jpeg) 

The 8Ah lipo is about 2.45kg without BMS

![184122h|690x388](upload://siOhTnru09613FoKlzaRVquF1K4.jpeg) 

12s 5Ah 30C Zippy's :grin:

![184221h|690x388](upload://1lcTd1K2AO2ibrxrI4y35OI301f.jpeg)
```

---
## \#758 Posted by: pjotr47 Posted at: 2019-05-02T20:08:28.085Z Reads: 127

```
No fishpaper between the groups? :disappointed_relieved:
```

---
## \#759 Posted by: pjotr47 Posted at: 2019-05-02T20:10:35.755Z Reads: 132

```
I am just ready with a 12s7p for a customer inside a peli 1150 case. I have used fishpaper between each group.


![image|281x500](upload://rFmE6HTpexCUQzWvVm9IaNBccOn.jpeg)
![image|375x500](upload://l4db6YTOkniJarTVMkYfxzSqy7V.jpeg)  ![image|375x500](upload://6eKT9fyATTNF8MTi2YE6ombSSx8.jpeg)
```

---
## \#760 Posted by: rich Posted at: 2019-05-02T21:04:26.750Z Reads: 133

```
The pack looks good and nice fit :+1:

[quote="pjotr47, post:758, topic:45377"]
No fishpaper between the groups? :disappointed_relieved:
[/quote]

It doesn't matter on a 1s72p :joy:

![005308h|690x388](upload://4gizKiXrKnL4xWXlbWema4qlHnp.jpeg) 

The reason why I didn't glue them is is because I'm still waiting for fishpaper from china so all good :laughing:.

Also still editing the video from dirt park, should be online this week...
```

---
## \#761 Posted by: rich Posted at: 2019-05-04T21:20:02.361Z Reads: 132

```
Arrived home after work and checked my mailbox...

Fiiiiiishpaper :hugs:

![230718h|690x388](upload://6urWRBFBJejK9uzUFWSTKqNU0TI.jpeg) 


Another thing, for those who wonder why I always wear the same trousers here why

![155522h|690x388](upload://c2AYaLzcisiJJtx399VEQ92K6QF.jpeg) 

Seems it needs more treatment than washing this time :laughing:
```

---
## \#762 Posted by: Andy87 Posted at: 2019-05-05T03:53:22.888Z Reads: 132

```
Nothing what duck tape can’t fix 😌😂
```

---
## \#763 Posted by: rich Posted at: 2019-05-05T17:55:29.307Z Reads: 135

```
Thanks for the hint so I don't need to stitch :joy:

The video is finally finished and uploaded :grin:. It starts with the jump where I cleared the table for the first time and leads to footage of day 2 in dirt park. Hope you enjoy it....


https://youtu.be/A_YSeWyBZHA


I only had 3 fails (at the end of the video) which is quite impressing for myself. But I had a good feeling this day otherwise I wouldn't risk anything. There are days I'm not in the mood or able to jump so I just don't jump or if I try to then I quit because I know I would only hurt myself. Riding is also fun on such days. So the tip of the day: only do a thing when you have a good feeling about it because you don't have to do it and tomorrow is another day.
```

---
## \#764 Posted by: Mobutusan Posted at: 2019-05-05T18:29:44.119Z Reads: 131

```
Another great video. You're clearing those jumps so nicely and smoothly now. What does your board weigh these days? You seem to be able to throw it around pretty well, but I'm sure most of that comes from experience and conditioning. I'm working on putting a light weight, high power, short range board for hooning around and jumping, but I'm not sure what a realistic minimum weight would be. It seems like 22-24lbs (10-11kg) could be attainable, but maybe still challenging to hit that?
```

---
## \#765 Posted by: rich Posted at: 2019-05-05T18:49:31.419Z Reads: 131

```
Thanks a lot! It is a great feeling clearing it after 2 years. I increased the height of the jumps in very small steps to get a feeling how the board reacts while flying. I think the most important thing is to land on the wheels after a jump and not on your ass, back, shoulder or head. Crashing after landing on at least 2 wheels is not that bad compared to lose control in the air. I always hurted myself when trying to increase the skills in a bigger step, small steps usually doesn't hurt.

[quote="Mobutusan, post:764, topic:45377"]
What does your board weigh these days?
[/quote]

16kg (35lbs) :face_with_raised_eyebrow:

[quote="Mobutusan, post:764, topic:45377"]
I’m working on putting a light weight, high power, short range board for hooning around and jumping, but I’m not sure what a realistic minimum weight would be. It seems like 22-24lbs (10-11kg) could be attainable, but maybe still challenging to hit that?
[/quote]

Me, too :sunglasses:, except high power (which means more weight).

I try to achieve between 11-12kg (24.3 - 26.5lbs) which is not easy. 10kg sounds like a dream.
```

---
## \#766 Posted by: Mobutusan Posted at: 2019-05-05T20:12:08.882Z Reads: 126

```
Dang. 16kg is pretty hefty, but fairy normal, I guess. I think that's around where mine is at. Even more impressive you can air it out like that though. :muscle: Keep up the good work, bro. :metal:

So, 10kg. is the goal, huh? I'm gonna shoot for that and see how close I can get. Gotta start weighing some components. I've got some MBS trucks with 9.5mm axles, that are probably a little lighter than the 12mm ones, but I'm concerned about their strength and bending axles. Only one way to find out though. And I'm hoping the 12s 6Ah 65c Graphenes will provide all the power needed without blowing the weight budget.
```

---
## \#767 Posted by: DeepSeaSwan Posted at: 2019-05-06T06:48:49.974Z Reads: 124

```
magic in the making! lighter and faster with only enough juice to blast off the mega ramp. I believe in you guys  @rich awesome footage bro!  you are lucky to have access to the perfect foundation! such a dope playground!
```

---
## \#768 Posted by: Resonant Posted at: 2019-05-06T07:21:37.350Z Reads: 125

```
When are the backflips coming?
```

---
## \#769 Posted by: rich Posted at: 2019-05-06T12:59:13.706Z Reads: 133

```
Thanks :blush:! Yeah the main problem is speed, often it's not possible to ride faster before hitting a jump to get more airtime. The parks are made for bicycles and the tracks/kickers are often too narrow so it can be even a challenge to reach the kicker at proper speed. Furthermore I think I'm at the limit stability wise and need more dampening for higher speed in off-road conditions before take off.

That's why I ordered stiffer elastomere damper elements in 90A (the original black ones are 70A). Well, big mistake because it's impossible to steer, I mean zero you just lift the opposite wheel :laughing:. Perfect for setting a new high speed world record with channel trucks so if this is your plan I have something for you, for me it's useless.

![060153h|690x388](upload://xySEtypEEIHlOZzymaVABJICeJh.jpeg) 

Anyway with the E-Toxx retainers you can add pre-tension on the elastomere dampers which helps but unfortunately I have no access to the rear ones because of the enclosure. On the other side I only had stability problems with the front truck so adding pre-tension there could be enough, need more testing. But when not jumping high I prefer without pre-tension for the good steering.

[quote="Resonant, post:768, topic:45377, full:true"]
When are the backflips coming?
[/quote]

Probably never, I'm too old (41 years) to break my neck :laughing:

My next goal is a 360 which is not easy because of the extra kilos on the rear truck for rotation. Also every fail hurts a lot so I'm not really motivated especially not in dirt park. Also even a 180 is tricky for me there because the rotation kills the speed. And I don't have yet the balls to try that with bigger speed and airtime. Here is the only 180 on tape from last summer

https://youtu.be/3Zy8Ytu32Rk?t=82


My 8A charger arrived, it is huuuuuge but it works (not like the 4A which came broken, had to fix it)

![125812he|690x388](upload://hl81dr7WIlPyZiispFCe2vP5QrV.jpeg) 

![130030he|690x388](upload://vJWRTdTNahMDULrFK7wkrxNFhKN.jpeg)
```

---
## \#770 Posted by: Andy87 Posted at: 2019-05-06T13:05:48.286Z Reads: 124

```
Welcome to the 8A charger club 👍
```

---
## \#771 Posted by: taz Posted at: 2019-05-06T13:32:04.896Z Reads: 127

```
That is a BIG charger. I never realized just how big these are.

Do you use the inner or outer truck holes for the elastomer dampers?\
I have the trampa version which is the same as e-toxx use them on the inner holes as if I put them on the outer holes it is almost impossible to steer at low speed.
```

---
## \#772 Posted by: rich Posted at: 2019-05-06T14:18:17.679Z Reads: 126

```
My trucks have outer holes only but that's fine for MTB. I can do very tight turns at low speed but only with extreme lean which is a lot of fun. You can also get tighter steering by putting more of your weight on the front truck, that helps a lot.

![dampers1a-gif|360x203](upload://8UDmEJ2jTUE1UkraotJVLyuiwOk.gif)
```

---
## \#773 Posted by: DeepSeaSwan Posted at: 2019-05-06T17:35:53.983Z Reads: 125

```
@rich how old is the hawk, bro?? old guys rule, means we have dad strength. preprogrammed in our DNA. once you hit 27 you get increasingly stronger until 50 then it all falls apart.... you got 9 more years of upside down  lifestylin... we need access to a foam pit. bottom line. my wife would be pissed if I broke my neck lol.
```

---
## \#774 Posted by: rich Posted at: 2019-05-09T18:53:25.295Z Reads: 129

```
Some progress on the 12s6p. But this Sikaflex is not my friend, it's getting dry so fast. If you order it then don't forget to order 10 additional tips. When you want to use it again the sikaflex inside the tip is dry despite proper sealing. After using it 2 times with 2 fresh tips I couldn't even get something out of the tube because the tip had a small crack. Last option was to open the aluminium can with a metal saw :face_with_raised_eyebrow:

![201553h|690x388](upload://bmJsldNcggrd0zN12nXzYC9OSNI.jpeg) 

Cutted strips of fishpaper. For those who don't find fishpaper online, it's called insualtion sheet/paper/gasket.

![010039h|690x388](upload://pVZTMR0n1P1UJ3UZBqnVBlQ5yL2.jpeg) 

Parallel packs insulated for serial bondings.

![011635h|690x388](upload://vdvVlYTMggWSqaS5YFOoLU9B8GO.jpeg) 

4 lines of Sikaflex for maximum strength using a 20ml syringe.

![175844h|690x388](upload://j3Hjj33TQTgnkwz9642zEWXC1bR.jpeg) 

Also filled all remaining connections/gaps on the side with Sikaflex.

![184850h|690x388](upload://2qejM2XAotUrfVdhsCjxUbw7sRx.jpeg) 

Gluing done, squeezed a bit in shape for curing the next 48 hours.

![184831h|690x388](upload://iKNXK02QQ9nIAKwAkhjuan2ahP4.jpeg)
```

---
## \#775 Posted by: taz Posted at: 2019-05-09T20:31:20.328Z Reads: 121

```
You probably know this but just in case: Don't forget the fishpaper rings on the positive poles.
```

---
## \#776 Posted by: banjaxxed Posted at: 2019-05-09T22:12:47.599Z Reads: 123

```
Those pants need fishpaper protection too
```

---
## \#777 Posted by: Andy87 Posted at: 2019-05-10T00:21:31.212Z Reads: 126

```
Sikaflex is horrible to work with 😂 don’t forget to buy a pack of one way gloves as well if you plan to work with it. @rich you can buy sikaflex in flex tubes which look like sausage 😅 
![image|690x475](upload://bYklMDB3FAh8X11A7u0WFlU39wI.jpeg) 
advantaged on it, you can just cut the 1cm which gets dry and than continue to work with. Disadvantage, you need a special pump to use it, or just use plastic sticks to apply the sika on the place you want.
```

---
## \#778 Posted by: banjaxxed Posted at: 2019-05-10T14:32:01.586Z Reads: 120

```
I can understand how a 360 is damned near impossible given the mount/motor weight at the rear, battery no problem in the middle

Maybes at some stage you split the motors front and back? That way less slow pendulum effect perhaps who knows you're pretty much alone on these big jumps on this forum anyway
```

---
## \#779 Posted by: rich Posted at: 2019-05-10T22:16:05.772Z Reads: 127

```
[quote="taz, post:775, topic:45377"]
Don’t forget the fishpaper rings on the positive poles
[/quote]

I won't forget :v: :sunglasses: just wait until I cut strips and spot weld, hopefully in 1-2 weeks.

Interesting info for Lipo orders from Hobbyking. 2 years ago I couldn't order from UK warehouse to EU but now it works and a 3s 5Ah 65-130C Nano-Tech is on the way :grin:

[quote="Andy87, post:777, topic:45377"]
you can buy sikaflex in flex tubes which look like sausage
[/quote]

Haha didn't know that :fries::beers:

[quote="banjaxxed, post:778, topic:45377"]
I can understand how a 360 is damned near impossible given the mount/motor weight at the rear
[/quote]

True, I mean with enough airtime everything is possible but I don't have the balls for this kind of russian roulette. So the weight on the rear truck and the overalll weight should be reduced to the minimum. 

Actually I'm building a light weight jumping board mainly from Trampa spare parts with cheap stuff below 12kg (26lbs). Maybe it won't survive the maiden ride/jump. I think in 1-2 months it's ready to rumble and I'll post a new topic then, for now a teaser:

![194409|690x388](upload://tCcdB32QjGgwg4Y4NDnhWIm9B5j.jpeg) 

[quote="banjaxxed, post:778, topic:45377"]
Maybes at some stage you split the motors front and back?
[/quote]

Planning to try that with the board for jumping vs. dual rear. I guess the balance is better in the air but not sure if it makes a big difference for rotations but of course there must be a difference. But lifting the front or ollie gets harder :thinking: And forgot to mention the motor plates are 3mm stainless steel and should be connected with crossbars otherwise they bend. But maybe not if I just try it once or twice :laughing:
```

---
## \#780 Posted by: banjaxxed Posted at: 2019-05-10T22:20:09.105Z Reads: 122

```
Yeah you need thicker mounts that way mon frere, looking forward to what you come with
```

---
## \#781 Posted by: Andy87 Posted at: 2019-05-11T00:45:09.678Z Reads: 118

```
With this red speed stripe you could probably also go with single drive only 😆
```

---
## \#782 Posted by: Gaza65 Posted at: 2019-05-11T03:57:35.537Z Reads: 116

```
We're did you get those dampers from?
```

---
## \#783 Posted by: Gaza65 Posted at: 2019-05-11T04:31:55.494Z Reads: 115

```
If you don't want those dampers I'll buy them off you...
```

---
## \#784 Posted by: rich Posted at: 2019-05-11T17:58:11.220Z Reads: 113

```
[quote="Andy87, post:781, topic:45377"]
With this red speed stripe you could probably also go with single drive only :laughing:
[/quote]

That's smart, what happens if I add a second stripe? No motors needed? :sunglasses:

[quote="Gaza65, post:783, topic:45377, full:true"]
If you don’t want those dampers I’ll buy them off you…
[/quote]

You would need 8x retainers from E-Toxx or Trampa additionally. But the more I think about it they could be dangerous. Beside the fact that steering is impossible I imagine what would happen if you loose balance at speed. You would tilt over and that could hurt a lot
```

---
## \#785 Posted by: Andy87 Posted at: 2019-05-11T18:46:54.063Z Reads: 117

```
[quote="rich, post:784, topic:45377"]
second stripe
[/quote]

The second just add range, sorry... 💁‍♂️😂
```

---
## \#786 Posted by: Gaza65 Posted at: 2019-05-12T05:05:34.315Z Reads: 112

```
I have the black ones already so I was thinking about trying them on the back
```

---
## \#787 Posted by: rich Posted at: 2019-05-15T22:50:23.821Z Reads: 119

```
You could also use an aluminium tube between hanger and baseplate with 1 small rubber washer, that's how the red elastomere dampers feel :laughing: If you really want them you can PM me but it doesn't really make sense.

Did you try to add pre-tension on the rear dampers?

I removed the foil on the SK8's and shot some videos for my warranty claim at HK. I haven't filled out the RMA yet because I'm afraid they want me to send them back first and they are out of stock atm. I have only one spare and want to ride again soon.

Anyhow I had to remove the glued gear for the first time with a small blow torch. After a while it smokes and smells, then it's easy to get it off.

I can move the can a few mm sideways :smirk:

Time to open the motor for inspection. There is thread locker on the screws on the side. 10-15 seconds blow torch and it's possible to unscrew them with Wera hex plus without stripping.


![033731h|690x388](upload://a5PXMNFTxDLsR45plmxQT7QL2ch.jpeg) 

![033955h|690x388](upload://4gNAcodZN1JLuwa08cak8t1Nnxy.jpeg) 

I couldn't get the can off and pinched my thumb like a noob. Well with a rubber mallet I finally knocked the can off. Crazy how 4mm make that difference, this 59mm stator looks tiny.

![041437h|690x388](upload://7KkrTyFOHmeEQ4KkEUEhHL8h2VA.jpeg) 

Sealed motor :sweat_smile:

![041542h|690x388](upload://sahwu4ZlNBvygXL5Fk2pICO0M0O.jpeg) 

![042057h|690x388](upload://lZIX9ufLgdsYOeyHmKI4NHfReqk.jpeg) 

Compared to sealed 6374 Maytech

![142447h|690x388](upload://4OHnxtS1IVcAA4Puw9C8ItVuHZm.jpeg) 

![061230h|690x388](upload://mG41bmphYlT93RFdSbW9SwaCHM8.jpeg) 

I was searching for the root of the clicking noise when spinning the SK8. The sensor PCB is not really centered and one sensor sticks out a bit. But there are no scratching marks on the magnets.

![202101h|690x388](upload://ppAvAimyb7gQHm48yQpAHdQLCvc.jpeg) 

Also there are no loose magnets or windings and the stator still has a strong connection to the motor plate. I have no idea where all the different rattling and knocking noises are coming from :thinking:. The bearings sound a bit rough and there is a little vibration but they spin for a long time.

The internal fan has some resistance when spinning but not that bad.

Meanwhile the sikaflex cured and I have a massive brick that won't separate. Maybe I place it inside the Pelicase first before I bend a new enclosure which needs time. Tomorrow evening  it's time to test the kweld for the first time before spot welding the pack. Also I haven't decided where to route all wires. It's difficult but I try to have no wires on top and bottom :grin:

![195740h|690x388](upload://wGNFmyyujYJSzSfKEUBLQLJ9x0E.jpeg) 

But the wiring also depends on which BMS I gonna use. I want to use the small 13s version but need to test if it works with 12s as the seller claims. Need to wire up some Lipos for testing first.
```

---
## \#788 Posted by: Andy87 Posted at: 2019-05-16T09:14:59.549Z Reads: 108

```
[quote="rich, post:787, topic:45377"]
It’s difficult but I try to have no wires on top and bottom
[/quote]

pretty much how i plan my pack as well. I will use H formed nickle and just bend it over on the main + and - terminal like on the cell level fusing packs so that i can solder the main leads on the side and not on top or bottom.
```

---
## \#789 Posted by: telnoi Posted at: 2019-05-16T10:21:07.396Z Reads: 111

```
[quote="rich, post:787, topic:45377"]
Also there are no loose magnets or windings and the stator still has a strong connection to the motor plate.
[/quote]

In short, actually looks to be a quality motor like the SK3. High probability nothing catastrophic would have happened if you kept driving it.

Would still be interesting to see if you can figure out what caused it. Next step might be just replacing the bearings and put it all together again.
```

---
## \#790 Posted by: sebaszz Posted at: 2019-05-16T12:24:03.002Z Reads: 113

```
Maybe battle hardening the motors.... avoids moving windings (and magnets) during load.

https://www.youtube.com/watch?v=5MFjzSP5Oiw

impressive battery btw, your topic always interesting to read :+1:
```

---
## \#791 Posted by: Gaza65 Posted at: 2019-05-16T13:23:02.567Z Reads: 114

```
Thought about it anymore?
```

---
## \#792 Posted by: rich Posted at: 2019-05-16T13:48:40.200Z Reads: 117

```
[quote="Andy87, post:788, topic:45377"]
I will use H formed nickle and just bend it over on the main + and - terminal like on the cell level fusing packs so that i can solder the main leads on the side and not on top or bottom.
[/quote]

:metal: I gonna use L-shape and bent tabs for balance leads. Only 1 nickel strip everywhere.

![145811h|690x388](upload://pjtKuQd5fjvCwFtyk3fO7nJUvMx.jpeg) 

The great thing is that a single 25mmx0.2mm nickel strip is more than enough. For the serial connections the width of the strip is the same as the cell. Did some maths and that means a 18mm wide 0.2mm strip is optimal for 16.46A continious and acceptable for 24.68A continious per cell. That's also good for inner resistance.

The problem is that I need to know if I can use the 13s BMS, soldered for testing balance adapters, next step is soldering adapters for the 4s lipos.

![145410h|690x388](upload://5tOFYniXp8hzuPWsJhEt13BC29g.jpeg) 

As you can see B- and P- are on the same side with cables. That's not usual and means the Li-ion pack needs to be flipped including balance leads. I have better Bestech BMS but I would prefer a small BMS with discharge, let's see. Also I want to place the BMS on the side and not on the top.

[quote="telnoi, post:789, topic:45377"]
In short, actually looks to be a quality motor like the SK3. High probability nothing catastrophic would have happened if you kept driving it.
[/quote]

TBH I only kept riding it because you said you had similar noises for a while :grinning: I had this clicking noises on Maytech's, too but after a short while the clicking turned into increasing resistance (some kind of internal short) and bad overheating. Reaching 80°C and thermal cut off within 3 minutes. I was inspecting for many hours but couldn't find the root for clicking (bearings were butter smooth).

The problem with the SK8 is that the can with shaft got play sideways (I have absolutely no idea how this could happen) which might not be too bad with straight gears but probably not good for helicals.

[quote="sebaszz, post:790, topic:45377"]
Maybe battle hardening the motors… avoids moving windings (and magnets) during load.
[/quote]

I was thinking about that but I'm not sure if it's neccesary because there is nothing loose inside and I really abused this motors especially with jumping, more than just heavy vibrations. And I don't remember reading about problems with loose magnets on SK3 or SK8. Or short said my fingers are too big for this can :laughing: and I hate epoxy (have no workshop).

[quote="sebaszz, post:790, topic:45377"]
impressive battery btw, your topic always interesting to read :+1:
[/quote]

:blush:

[quote="Gaza65, post:791, topic:45377, full:true"]
Thought about it anymore?
[/quote]

If you talk about the dampers PM me
```

---
## \#793 Posted by: Andy87 Posted at: 2019-05-16T13:53:31.127Z Reads: 110

```
[quote="rich, post:792, topic:45377"]
18mm wide 0.2mm strip is optimal for 16.46A continious
[/quote]

Where did you find this values? Couldn’t find any good overview on Nickel besides the old endless sphere one which is floating around.
```

---
## \#794 Posted by: rich Posted at: 2019-05-16T14:03:26.984Z Reads: 111

```
Haha, my maths are based exactly on this chart :laughing:

If you translate the 0.2mmx7mm value for nickel to 18mm you get 16.46A (optimal) and 24.68A (acceptable).

![Cu%2C%20Ni%2C%20Steel%20efficiency%20chart|549x500](upload://67AaXbcHal5oa69BBd33ZyGIqvU.png)
```

---
## \#795 Posted by: Andy87 Posted at: 2019-05-16T14:12:43.324Z Reads: 110

```
😂 ok 👌

What I don’t like in this chart, (maybe I just didn’t found) but there is nowhere written on which length of nickel this values are applicable. To assume that the length of nickel between cells is usually not more than 18-20mm I could imagine that the nickel can handle more than in this chart stated. If somebody has some more info or stress test of nickel strips I would be super interested in looking into it.
```

---
## \#796 Posted by: rich Posted at: 2019-05-16T14:18:19.732Z Reads: 111

```
True that would be very good to know but I guess this chart is for shorter connections because it's about battery building but who knows.

It's also funny when looking at rating for cables (with no info about length). There are charts where a 10AWG is rated for 50A instead of 140A  :sweat_smile: that must be a very long wire.
```

---
## \#797 Posted by: rich Posted at: 2019-05-16T14:21:04.797Z Reads: 106

```
Found this nice chart (can't remeber where I downloaded it). According to this chart 0.2mmx7mm is 5.7A so only slightly different to 6.4A of the other chart

![Ampacity%20Chart|603x500](upload://xkf1v4b7PE6nrnCWUnBYzNSm20v.jpg)
```

---
## \#798 Posted by: Andy87 Posted at: 2019-05-16T14:22:13.196Z Reads: 103

```
[quote="rich, post:796, topic:45377"]
50A
[/quote]
That’s the constant current value

[quote="rich, post:796, topic:45377"]
140A
[/quote]
It’s than probably the fusing current. The current when the wire melt after idk 10s at 20cm length. 

I think I found a chart for it a while ago. Maybe I find it later again
```

---
## \#799 Posted by: rich Posted at: 2019-05-16T14:35:19.259Z Reads: 115

```
Huh 50A?

I'm no expert but I believe in charts which state

* 140A for 10AWG (5.5mm bullets)

* 88A for 12AWG (XT90 = 4.5mm bullets)

* 55A for 14AWG (XT60 = 3.5mm bullets)

That makes especially sense when looking at the corresponding connector ratings.

Here is such chart but with no info about length, just resistance per km.

![PNG|560x500](upload://ishV9addd4uowWEb2upLbWZCR5D.jpeg) 

[quote="Andy87, post:798, topic:45377"]
It’s than probably the fusing current
[/quote]

According to this chart the fusing current for 10AWG is 333A 

![WireFusingCurrents|690x432](upload://a7T4DUShNFmfX99qRAuIBDBdFMw.PNG)
```

---
## \#800 Posted by: Andy87 Posted at: 2019-05-16T15:03:47.337Z Reads: 113

```


https://www.powerstream.com/Wire_Size.htm

55A for 10awg according to this chart.

Maybe I get something wrong.

[quote="rich, post:799, topic:45377"]
fusing current for 10AWG is 333A
[/quote]

That can be as well. I didn’t find the fusing chart yet.
```

---
## \#801 Posted by: sebaszz Posted at: 2019-05-16T18:33:43.932Z Reads: 110

```
i don’t if this is the case now but battle hardening can help if you have “clicking” noises. these can be caused my the moving windings under inductive field forces. that’s why you don’t see any damages nor issues moving the motor by hand.

the endless sphere table is spot on. I tested these values againt real live testing with high current injection tool.
```

---
## \#802 Posted by: rich Posted at: 2019-05-16T19:19:40.711Z Reads: 118

```
[quote="sebaszz, post:801, topic:45377"]
i don’t if this is the case now but battle hardening can help if you have “clicking” noises. these can be caused my the moving windings under inductive field forces. that’s why you don’t see any damages nor issues moving the motor by hand.
[/quote]

Good point, gonna think about battle hardening. I have a slightly preference for just mounting the spare SK8 so I have more time for inspecting plus I can ride. Also the clicking motor was strange from beginning. There was a bit play sideways, the others don't have this. I put shim spacers between motor bearing and helical so the play was gone. It's a miracle why the movement came back and even got worse. 

[quote="sebaszz, post:801, topic:45377"]
I tested these values againt real live testing with high current injection tool.
[/quote]

Nice! What was the length of the strips?

Meanwhile I soldered the adapter to test the BMS

![203250h|690x388](upload://t3LI3eoTasxONsVVRV0ciHIT6V5.jpeg) 

Well, 12s pack has 44.4V

![203651h|690x388](upload://j6tDuRKy9kpRputLwTDvHZbBEaR.jpeg) 

Let's see what the BMS output voltage is....... :scream::rage:

![203627h|690x388](upload://vqDbhl8wWUhbHTnHMyCWvS2F50F.jpeg) 

Damn it, all connections are correct, also measured each pin of the balance connector.

Spent too much time to wire this up for nothing! Have to rethink BMS options (2 left) and whole wiring of the Li-ion. One step forward, 2 steps back.
```

---
## \#803 Posted by: sebaszz Posted at: 2019-05-16T21:15:21.584Z Reads: 117

```
I can imagine sideway play can increase over time in your case. Disadvantage of helical gears is they produce axial thrust force. Normally you need to have thrust bearing to absorb the force. Herringbone gears would solve this but more complex to produce. Unfortunately helical gears are actually not proven yet for esk8 on the long run. Maybe this is not the case but it should be considered as a possible cause.

only tested short piece of nickel. More length only causes voltage drop. Heat is our enemy, length is too short for significant voltage drop
```

---
## \#804 Posted by: rich Posted at: 2019-05-19T12:30:26.770Z Reads: 128

```
[quote="sebaszz, post:803, topic:45377"]
I can imagine sideway play can increase over time in your case
[/quote]

But how? The only reason I can think about would be crushed or damaged bearings with play inside. Between motor bearing and glued gear are washers with zero gap. The can and shaft had play sideways when the motor was brand new but after gluing the gear it was gone but came back even worse. 

[quote="sebaszz, post:803, topic:45377"]
Unfortunately helical gears are actually not proven yet for esk8 on the long run
[/quote]

I used them for about 500-600km so far but see no problems. I need to ride more for long term experience. Good point with the bearings. Probably they need to be replaced earlier than with straight gears. I will research if there are thrust bearings in the correct size available, good hint!

It would be interesting to know how much pressure or which force actually is on the motor bearing due to helicals. Radial bearings can take axial forces if they are not too big.
```

---
## \#805 Posted by: rich Posted at: 2019-05-19T21:01:01.898Z Reads: 132

```
I was time to test the kweld and have a spot weld party :sunglasses:

![133715h|690x388](upload://sS5iIr9IugZvlu6mN8tLQKL5ynt.jpeg) 

![133859h|690x388](upload://5emlGDcRFRXIMhy1NKCQTJeGBVr.jpeg) 

First tests with a single weld with 0.2mm thick nickel strip

![005023h|690x388](upload://hW83wzL5FbuzbRK8AohGXTJ8uHJ.jpeg) 

![005125h|690x388](upload://tQRMszhsADUrvPwEa5sYse6AukY.jpeg) 

after removing with pliers

![005621h|690x388](upload://iaG9VZR5yzmpmwmddgmbtmGUqJQ.jpeg) 

Now testing 3 welds each strip with 30-50 Joule.

![011915h|690x388](upload://oin9ehom6jGMMFCLddYbmgd5k0c.jpeg) 

![011905h|690x388](upload://wYY4eG5qYTfr2Rq1Sp78fbnfqxe.jpeg)

Removing the strips is not easy at all with 3 welds, especially 40 and 50 Joule as you can see.

![012138h|690x388](upload://zNrbHH26uK5UXVNaHT4tGZwERQM.jpeg) 

It was time to test 0.3mm nickel strip with 50-100 Joule. The welds are so strong that it is impossible to remove them with pliers, only the steel blade breaks apart :grin:

![122443h|690x388](upload://eOQzWQ6bwbx7bBK642qy4PBzRsf.jpeg) 

After a while we realized that all the black marks on the backside of the steel blades come from the burnt wood which is laying underneath :rofl:

![122614h|690x388](upload://5pqHtYJ9OtvZ6k0oe792bJhc8yj.jpeg) 

Then the idea, I have a solder mat where you can put the soldering iron directly on it without any damage. So perfect to withstand the heat of the spot welds. Well........ not really

![125302h|690x388](upload://ri57rqU0JcHuQILUMOuPDYfwyhn.jpeg) 

Instead of black marks there are now white marks on the backside of the blade :crazy_face:

However this spot welder does a great job and with the nano-tech 65C-130C lipo it welds with 1300A :laughing: 

During testing the cables and lipo stayed cool with 0.2mm nickel strip. When welding 0.3mm nickel with higher settings both got warm. The tips don't get hot because of their massive size. I'm curious if they get warm when welding a whole pack (or half).
```

---
## \#806 Posted by: ducktaperules Posted at: 2019-05-19T22:43:57.689Z Reads: 123

```
[quote="rich, post:805, topic:45377"]
The tips don’t get hot because of their massive size. I’m curious if they get warm when welding a whole pack (or half).
[/quote]

can confirm that once you get into the flow of welding tabs those probes will start to heat up. because you are focused it will start to get uncomfortable to hold but you will think "its ok i will keep going till the end of this row". By the end of the row they will be VERY HOT.
```

---
## \#807 Posted by: sebaszz Posted at: 2019-05-24T16:24:04.619Z Reads: 113

```
I think bearings should be damaged then.

Would be nice if you can find the mechanical failure.

Would the geardrive in general not put extra stress on your motors as well by heavy abuse. Belt drive dampens the vibrations transfered from the wheel.
```

---
## \#808 Posted by: sebaszz Posted at: 2019-05-24T16:25:35.027Z Reads: 112

```
Nice work with the testing of the spotwelder
```

---
## \#809 Posted by: mmaner Posted at: 2019-05-24T18:06:33.359Z Reads: 114

```
@rich & @ducktaperules, and anyone else using the kWeld system.  Would you mind outlining the settings you use on standard 8 x .15 nickel?  My brother just bought one of these and is trying to get some info before it's delivered.
```

---
## \#810 Posted by: rich Posted at: 2019-05-25T01:53:47.322Z Reads: 121

```
[quote="sebaszz, post:807, topic:45377"]
Would be nice if you can find the mechanical failure.
[/quote]

Found it :face_with_raised_eyebrow: 

First massive failure is this hole

![005252h|690x388](upload://2qbUHfE5sukttexXeOx1htXsx5r.jpeg) 

Now I know why I had metal chips inside the can. You can look through the bell WTF!

![005230h|690x388](upload://xvb2ZcySFuaqSZEjWu9RPg6sGwk.jpeg) 

Second I finally found some loose windings which I can move.

![005335h|690x388](upload://qF0qpPF0cuZYIBSbGnzOyByH3nm.jpeg) 

But now another disappointing story. I prepared the new SK8 motor for the helical including cutting the shaft. Today before work I glued the gear to the shaft with Loctite 638 and wanted to do it very accurate. I applied and spread it on the inside of the gear and on the shaft. Then I made a ring around the tip of the shaft. Very slow and by turning I slided the gear on the shaft for maximum strength. Just before finishing I wanted to soak the tiny bit retaining compound at the end with kitchen roll paper. That's the end of the story. I realized the retaining compound got monster sticky already after about 3 minutes and I couldn't move the gear anymore. Even with a pulley remover it was impossible. Also my small blow torch didn't help. Daaaaaaaamn :sob:

![005656h|690x388](upload://cuznFiLKUqBZtPWFfLjJBooFkgc.jpeg) 

One step forward, two steps back, that was a bad moment. Next step is to buy a proper blow torch for removing the gear without cooking it.

[quote="mmaner, post:809, topic:45377"]
Would you mind outlining the settings you use on standard 8 x .15 nickel?
[/quote]

I have 0.2mm and 0.3mm nickel strips only but this is a suggestion from the manual:

![J|276x94](upload://pOdM5cizKSiwcPTCPRIs10fmwSu.png) 

From the testing of 0.2mm nickel 40 Joule is enough IMO, even 30 would work. So I guess for 0.15mm nickel it's maybe 25-35 Joule. Best is to test it first. This values are for nickel on steel. Nickel on nickel need higher values.

Just a short explanation about Joule

![J1|690x65](upload://2kAGaROYtnMUnCWuHtZ0lgiZFSJ.png) 

This is the [kweld manual](https://www.keenlab.de/wp-content/uploads/2018/07/kWeld-operation-manual-r3.0.pdf) and here the [assembly manual](https://www.keenlab.de/wp-content/uploads/2018/07/kWeld-assembly-manual-r5.0.pdf) if your brother didn't download them already.
```

---
## \#811 Posted by: mmaner Posted at: 2019-05-25T02:01:18.097Z Reads: 109

```
Good info, thank you.
```

---
## \#812 Posted by: rich Posted at: 2019-05-25T02:19:15.454Z Reads: 115

```
Forgot to post the pic when testing the fishpaper, this is after 1 weld.

![005028h|690x388](upload://wmuvldTSM0i6vNBJxSUyn6IEx5h.jpeg) 

This is the bottom side

![005055h|690x388](upload://6FcDPSafAAEr9vCp3TYKspj4zQ7.jpeg) 

There is no hole but it's also 1 weld only and I would feel safer with at least 2 layers. For example if someone welds nickel tabs (with pre-soldered balance wire) in between 2 cells then there are fishpaper rings underneath. Or better avoid doing this :laughing:.
```

---
## \#813 Posted by: legend27 Posted at: 2019-05-25T15:35:50.487Z Reads: 109

```
[quote="rich, post:810, topic:45377"]
Next step is to buy a proper blow torch for removing the gear without cooking it
[/quote]

I’ve used a heat gun on 420 degrees Celsius a couple of times now and it worked great. Took some time but got the job done. Doesn’t burn the gear either.
```

---
## \#814 Posted by: pjotr47 Posted at: 2019-05-25T16:01:55.196Z Reads: 110

```
I use always a cheap weed burner of 5 euros. Works perfect. Heat the pulley for 30 seconde and it come off without any problem.
```

---
## \#815 Posted by: rich Posted at: 2019-05-25T23:05:50.236Z Reads: 118

```
This is the new blow torch compared to the old :laughing:

![223430h|690x388](upload://hpi3Hl3bQCnSdjwskPAMmf4UIej.jpeg) 

![223320h|690x388](upload://70GzyR4JWvCWz05qJUVc69VAnIa.jpeg) 

What an epic flame, it took 30-45 seconds until it started to smoke and smell and I could remove the gear. With the small one it took several minutes.

![230055h|690x388](upload://wviK6UHX9OD5sjT1uBj94DoGtK1.jpeg) 

After a bit sanding and cleaning I finally glued the gear on the shaft and this time like it should be. If you stay within 1-2 minutes then it's no problem.

![004926h|690x388](upload://MWanPwdm1uPngiYIwirf9KvdQ4.jpeg) 

[quote="legend27, post:813, topic:45377"]
Doesn’t burn the gear either.
[/quote]

True. This time I didn't burn anything because I heated the shaft only.
```

---
## \#816 Posted by: ducktaperules Posted at: 2019-05-27T18:20:17.404Z Reads: 112

```
@mmaner im using the Malectrics spot welder.
```

---
## \#817 Posted by: mmaner Posted at: 2019-05-27T18:24:23.201Z Reads: 114

```
My little brother has a kweld system coming, it looks pretty great.

My malectrucs is dead ☹️
```

---
## \#818 Posted by: rich Posted at: 2019-06-01T11:32:59.634Z Reads: 106

```
Soldered sensor extensions and finished wiring plus added new foil on the motors.

Finally it was time to put everything together, or not?

![182712h|690x388](upload://wrpvgeUoPhleH4r6Dy2TxR1xJnJ.jpeg) 

It seems I didn't hail skatan enough because the new SK8 has heavy resistance when spinning. I realized it when adjusting the backlash of the helicals. Feels like a small internal short. Just to be sure I removed the wiring but no bullet had contact. When spinning the can only the difference is smaller but the resistance is heavy when spinning the gears :tired_face:

https://youtu.be/A-W6fClXgbk

Instantly I had to take the Urban Burro and go for a ride to forget about this disaster. I had a lot of fun and got dirty on all terrain and fell off a couple of times because of no bindings. Then the dirt path was wet and while turning the rear of the board slipped away so one foot left the board, tried to balance with the rear foot on the ground. That didn't work and ended in eating the bush and dirt :laughing:

![201922h|690x388](upload://m8yHgdGHcM0sw2IygRcUOhRX221.jpeg) 

But nothing happened beside dirty clothes, just a funny moment.
```

---
## \#819 Posted by: slade Posted at: 2019-06-18T18:46:43.169Z Reads: 101

```
Damn that's the number one reason why I've always been worried about putting permanent threadlockers on any of my bolts :sweat_smile: If you had a spare stator drive shaft and helical motor pulley, would you have been able to remove the shaft/helical gear assembly and just replace it with a new set?
```

---
## \#820 Posted by: rich Posted at: 2019-06-22T20:01:27.633Z Reads: 103

```
It's really easy to remove glued pulleys/gears with a blow torch or bolts with the mini torch. I was only scared before the first time doing it, like with many things.

[quote="slade, post:819, topic:45377"]
If you had a spare stator drive shaft and helical motor pulley, would you have been able to remove the shaft/helical gear assembly and just replace it with a new set?
[/quote]

Not really because you have to remove the gear before you can open the motor to remove the shaft anyway.

I bought cheap (before tax) 6384 200kv motors because I want to switch to 1:6,25 gearing :blush: and furthermore need replacement motors/helicals. I'm tired of all the breaks due to broken motors.

![163255h|690x388](upload://8RzNo7bax3DF4lgY6EoZRjsIxGO.jpeg) 

![025633|690x388](upload://qFU6U1V7KMo1hKnqa9BsQfkGg6f.jpeg) 

Compared to 6374 SK8 which is even longer than the 6384 

![213132h|690x388](upload://bXPHJGW6fphwfhdsDNM3tPICmPX.jpeg) 

![213213h|690x388](upload://pDZRiocqeeZymXNm60qhrt4uAQE.jpeg) 

There were some loose windings

![182342h|690x388](upload://lT0xYqAH2PvB7lpToICX3X5sTGq.jpeg) 

Also because of no retaining ring the magnets are crooked with different spacings. I'm afraid they won't run smooth, let's see.

![182834he|690x388](upload://ogiKIppjgiUPG7LQCh9FgaDV8lx.jpeg) 

No way to test them so they got a special treatment

![025922|690x388](upload://dDGsuDdhSpWYc60LEj7NoudRx64.jpeg) 

![124228|690x388](upload://5FzLOjOuRSaB6gCWpDa6UXij5ll.jpeg) 

Secured all cables against movement, next thing is to replace the 16AWG phase wires.

![185925|690x388](upload://dGMiL10Fnk237EA1M0lIJmfkllW.jpeg) 

Also put silicone on the blank sensors

![150717e|690x388](upload://hoJSwm3s4aqETkghWoNChYSVBVC.jpeg) 

Next problem were the 10mm shafts because I need 8mm for the 8T helicals. Removing the shafts was not easy because they are pressed in. I damaged my drill press when trying to remove them. In the end it was raw power with a hammer.


Fortunately a friend of a friend could turn the shafts down to 8mm at the tips, that was no easy task even with a very expensive commercial machine due to hardened steel.

![012846|690x388](upload://mraMAUouBaVzZnIQLNCamgp8FGB.jpeg) 

![014456|690x388](upload://sieAvsP62L3SpZkvBUIbfx4ZjLa.jpeg) 

Before inserting the shaft it's best to use a foam or in my case a yoga mat to protect the magnets. The shaft will slam on the magnets if not 90% centered.

![144126|690x388](upload://4DHSchuysRDt8BYELeXL4ZhlfsR.jpeg) 

I put oil on the shaft and bell for easier assembling. Pressed the shafts back with the small and then with the bigger hammer. It was quite easy.

![144259|690x388](upload://ah1IehGZca9bHhU6ESLQBvrMBM.jpeg) 

![144944|690x388](upload://zpeV72gYU9oWInEA0Wkdhcq6KP8.jpeg) 

When I tried to re-assemble the first motor I pressed out the front motor bearing because of the sharp edge at the reduction from 10mm to 8mm. So I rounded the edges with a dremel.

![154816|690x388](upload://wnE3K7cCus5Tq3SDgWJOLhwXwPl.jpeg)

 The magnets are so strong that it is very difficult to put the bell smooth on the stator despite mounted on the motor mount. I took a piece of wood and yoga mat to catch the bell.

![142809|690x388](upload://f3IITtMLgHIBYLqGniDXo56vsbz.jpeg) 

Catched... now it was easy to slide further to the 10mm part of the shaft slow and smooth.

![142849|690x388](upload://tUQB003mRazDELmpFmyoIja07K6.jpeg) 

Next thing is to do motor detection and pray that everything is in order including sensors. Then I'll glue the helicals and change the thin phase wires and extend the 5pin sensor wires to 6pin.
```

---
## \#821 Posted by: ducktaperules Posted at: 2019-07-10T10:24:49.025Z Reads: 94

```
@rich you still got those orange barrels. I'm keen to try them. I'm a big guy and find most setups too lose for me. I been wanting some barrels but I'm worried the standard ones will be to soft.
```

---
## \#822 Posted by: Andy87 Posted at: 2019-07-10T10:44:05.753Z Reads: 98

```
just have found some 6384 120kV yesterday for like 50€ and thought to maybe give them a try with all the mods you did as well :sweat_smile:
how did you change the phase wires? the ones on the motor i was looking at wheres super slim as well.
Did you already have a time to try those motors out?

Why you change to 6.25 gearing and go up with kV? i mean the end result of torque and speed should be similar than, no?
```

---
## \#823 Posted by: rich Posted at: 2019-07-12T14:17:35.569Z Reads: 102

```
[quote="ducktaperules, post:821, topic:45377"]
orange barrels
[/quote]
Damn you remind me that I totally forgot to send them to @Gaza65 as promised :face_with_hand_over_mouth: But I can't recommend them, it would need at least 3-4 people strapped on the same deck to be able to steer. Or all people land on the ass instead of steering.

[quote="Andy87, post:822, topic:45377"]
just have found some 6384 120kV yesterday for like 50€
[/quote]

I think they are all from the same manufacture, hit or miss. I've read about people with loose and broken magnets after the first kilometers, others run fine. Unfortunately I haven't had time to test them yet but looking forward to mount them within the next days.

Strange is that when spinning by hand one motor sometimes makes scraping noises plus resistance like if windings would touch the magnets. This is not possible because they are glued so I have no idea what it is. This behaviour I had on other motors (Maytech, APS), too and couldn't find the reason, but they worked.

[quote="Andy87, post:822, topic:45377"]
how did you change the phase wires?
[/quote]

Haven't changed them yet, the phase wires are 16AWG, gonna cut them after 5-10cm and directly solder "thicker" 14AWG to them :laughing:.

[quote="Andy87, post:822, topic:45377"]
Why you change to 6.25 gearing and go up with kV?
[/quote]

The man to blame is @Nowind, I already ordered 10T helicals with 10mm bore for other motors than Maytech or SK8 and later that day I read his post somewhere that his actual setup with 200kv motors and 1:6.25 is super aggressive. I had to change my order to 8T helicals :grin:.  I think I get more instant power due to bigger stator size of the 6384 (despite the 200kv) plus higher gearing.  Also I remember @taz wrote that his 190kv Maytech had more power than SK8 149kv on MTB with the same gearing.

Or short I do it for science.

The main reason why I had no time (beside work) to run the new motors is following:

![192427|690x388](upload://hivP4HZ0blakFvsAq1gUQ59EqGN.jpeg) 

It's hard to see on the pic but the lipos are really puffed and got damn hot during use. After use they felt like jelly, scary. Time to let them rest in peace. The graphenes had a short life of 1 year.

Furthermore I recognized this evil thing on one balance connector, I guess I had just luck.

![191807e|690x388](upload://7Ap2Bv1xJdgrtdGvcPJkQeGASqZ.jpeg) 

So it was time to weld and finish the 12s6p to be able to ride again.

I have different fishpaper rings but these are my favourite, the inner hole is perfect sized.


![191121|690x388](upload://a2ijhBXTHVjwl7IyF9l7iREoudC.jpeg) 

Tight fishpaper porn

![191021|690x388](upload://jqOjqOX3givWZCNy3P58hOrOzn9.jpeg) 

Cut the 0.2mm nickel strip with tin snips after transferring the shape of the cardboard template with a pencil.

![220543|690x388](upload://t7d45CDxUnWshde5Gqp4OslVMpd.jpeg) 

Held the nickel with magnets and welded the negative side first.

![000212|690x388](upload://htqrAFdQ7bwLWzphVPGM5xwoGvr.jpeg) 

Then with help of the fishpaper rings the positive side, that helped a lot.

![004708|690x388](upload://98SAfuDjelf6FMMPY2Onxe6IwaU.jpeg) 

After the top side I finished the bottom, you can find some smileys in the pic

![013934|690x388](upload://zubW8Jr9HBJq0d7Jw0ckHzE0UNk.jpeg) 

My plan was to make all wiring and connections on the sides to keep the height low for a new enclosure. Reality is that I needed the battery now and also didn't have the smaller BMS yet so I took the Bestech and thought about modular wiring. I decided to have the wiring on top and use the Pelicase 1150 for now.

Soldered 3x 16AWG wires to the positive and negative nickel strips before welding. The thin wire is for charge port/voltmeter. I prefer to have an exta wire instead of splitting it later.

![202402|690x388](upload://ig0SYgN4dCnzs5UBRlOCY2pjfQv.jpeg) 

Insulated with kapton tape and fishpaper for + and -.

![202812|690x388](upload://4OEltaUHMwQOjt0nsULogf912oK.jpeg) 

After that I soldered the 2x 6s balance connectors on top

![215741|690x388](upload://d8XQN13EqKKVS2NvweBYflS1CJN.jpeg) 

and on bottom

![030432|690x388](upload://pquW4aFhyaAnYVg61ydfmA7ZZ6w.jpeg) 

For easy connecting in tight space I soldered 3.5mm bullets on the negative 16AWG wires. The plus wires are soldered nicely to 10AWG wie without connector. Now I can easy change the BMS or even ride without BMS and charge with a balance charger in case of a broken BMS or charger.

![220114|690x388](upload://4b4XvaMmLxRvRCkpE84dxsOKGY8.jpeg) 

I decided to put the fuse for charge port directly on the positive wire instead of after the connector for saving space. I have 8A or 16A fuses so I chose the 16A because of 8A charging current. But even the small fuse is big so I had an idea... took the fusing strip

![143133|690x388](upload://wyjGwRLlGewToNVYdFw5eimuwhC.jpeg) 

![144321|690x388](upload://e6ovXWsTiDjaHFdtFOrmqpN2rF0.jpeg) 

Kapton tube and fishpaper

![150934|690x388](upload://cuIGkhQgnpoF2BCD7VwelSkBTVc.jpeg) 

Finished

![154754|690x388](upload://i7vKG9LGj4Dee3qWi5q8OBOrJxj.jpeg) 

Glued 2mm neoprene foam on the bottom side to protect the solder joints.

![172119|690x388](upload://8kZ517TQSUjsktTydLETsrWeBL7.jpeg) 

It was time to charge it for the first time to check everything. Well the charge port and charging plug of the 4A charger got hot within minutes that's why I soldered a new charging port but nothing changed. Damn so I tried the 8A charger and it worked, the 5.5x2.1mm charge port got warm only. It seems like the charge plug of the 4A charger is faulty. With active cooling I could charge the 18Ah within 135 minutes without any problems.

![190223|690x388](upload://uB4KjFAKGYjSKBITT5yigg4layf.jpeg) 

Then I needed a sturdy divider to seperate the battery from the BMS inside the enclosure. I bent 0.8mm aluminium sheet to desired shape.

![211958|690x388](upload://67Rk2YcmWPjldhba93J3HZXFP0z.jpeg) 

This way the 3.5kg battery can't squeeze the BMS, it's a case in a case.

![212036|690x388](upload://rEfk6hCFvlrFRcEDg7Bdfp2cFgY.jpeg) 

Of course I've insulated the aluminium with duct tape and glued 2mm foam

![233530|690x388](upload://t1B0VPplRoUvN6NyUOFiWqLY2mf.jpeg) 

The BMS is secured with foam and can't move.

![235703|690x388](upload://hRWotUE60cGuOHTxhBLAkaDBGbl.jpeg) 

Foam on both sides of the aluminium

![000827|690x388](upload://cpLULkRODa9MXaKvCG1rpVYnAEu.jpeg) 

For the sides of the battery I used a sandwich of 2mm neoprene foam and fluffy soft foam in the middle

![183456|690x388](upload://2wfARF5yP9awrPCMazcGM2UJosM.jpeg) 

On top different foams to reach the same height which is taller than the balance connectors.

![185640|690x388](upload://mr33yWsEYXrYXPlvla1iaWPQyZB.jpeg) 

Finally super soft foam on top.

![190602|690x388](upload://j0vEuWcfJa2zK6xwJ9Cyb2TnJjB.jpeg) 

So I was ready to riiiiiiide :heart_eyes:

I rode 2 hours and discharged from 4.2V to 3.5V per cell and had a range of 30.4km (18.9miles), a bit disappointing, it was mainly flat offroad on gravel paths and dirt.

The added weight is no problem when riding but makes a difference when ollie or turning 180° on standstill. When jumping on the BMX track I didn't recognize a big difference. Also the battery didn't fall apart which is a good sign :laughing:

Now the battery is charged for the second ride but it started raining :disappointed_relieved:, guess I have to wait and get dirty afterwards.
```

---
## \#824 Posted by: legend27 Posted at: 2019-07-12T15:54:13.920Z Reads: 92

```
That’s a really nice battery. Good idea using the fish paper rings as a helper :ok_hand:

Btw. Where did you get that neoprene foam?
```

---
## \#825 Posted by: rich Posted at: 2019-07-12T16:16:00.343Z Reads: 95

```
[quote="legend27, post:824, topic:45377"]
Good idea using the fish paper rings as a helper
[/quote]

It was very relaxing to know that you weld on the right spot without blowing a hole in the nickel strip.

Other hint I found out is alcohol against sticky electrodes but not the one for drinking :beers:. After some welding the positive electrode starts to stick on the nickel. It helps to sand it a bit but you lose material every time. After cleaning with alcohol it works again without any sanding :grin:

[quote="legend27, post:824, topic:45377"]
Where did you get that neoprene foam?
[/quote]

The neoprene foam I buy in germany : https://www.fugendichtband24.de/Neopren-Zellkautschuk.htm

I also use the non-adhesive EPDM foam which you can get for cheap e.g. on amazon (up to 80-90° C), neoprene foam is up to 100° C.
```

---
## \#826 Posted by: Gaza65 Posted at: 2019-07-14T12:21:46.846Z Reads: 89

```
Nice
And yes still waiting for them...
```

---
## \#827 Posted by: rich Posted at: 2019-07-15T15:59:43.435Z Reads: 88

```
Sorry for the delay, packing them right now :innocent:

Yesterday I finally glued the helicals with Loctite 638 so in 2 days I can test the higher gearing plus the 6384 200kv motors :beers:.

![171534|690x388](upload://wcep4Jbg6Ai9OSf321ChZaywUuR.jpeg) 

![171314|690x388](upload://hKpXjv0lZMMKbZ9dyluyDXyA0vJ.jpeg)
```

---
## \#828 Posted by: Gaza65 Posted at: 2019-07-16T00:14:43.118Z Reads: 82

```
I have the same motors and like the speed range...
```

---
## \#829 Posted by: rich Posted at: 2019-07-17T15:52:43.369Z Reads: 81

```
Today I switched to latest FW 3.58 with the SK8's to see if there is any difference before mounting the 6384. Before I was using FW 3.38, I'm curious about the locking brakes problem or in my case the brake releases before standstill, very dangerous. I had bloody knees and pain because of this bug.

However I'm a bit scared because the 6384 have no temp sensor. Yesterday the SK8's got into thermal cutoff after 15km and 100% throttle meant 0% power. I had to take a 15 minutes break.

But now I go for a test ride with the new FW :grin:

![201503h|690x388](upload://36a7FObkt6MSyBJTicnZVHop90k.jpeg) 

The more I ride the more I recognize the added weight from 16kg to 17.6kg. On the other hand I can ride longer, my furthest was 37km discharged to 3.3V/cell, a bit above 40km should be doable. But I would like to have 100km range tbh, you can't have enough range :rofl:
```

---
## \#830 Posted by: slade Posted at: 2019-07-17T16:16:09.752Z Reads: 82

```
I recently finished a build with SK8 6374s and I think I've noticed a difference in temps compared to the SK3s I previously used those ones for a road only build and they have the internal fan blades and air flow exits on the back. Do you think you'd ever switch motors to something with large exposed air vents? I'd love to find something with better cooling but don't know how much crap would get sucked in or caught in it
```

---
## \#831 Posted by: rich Posted at: 2019-07-17T18:23:42.904Z Reads: 79

```
The SK8 have the internal fans as well just no exits. 

[quote="slade, post:830, topic:45377"]
Do you think you’d ever switch motors to something with large exposed air vents?
[/quote]

Yes within the next hours :laughing:, gonna ride tomorrow with the new motors which have some venting holes.

![201850|690x388](upload://2o8UL32sBLg8vK8E7sbfjiDrCFC.jpeg) 

But that's no guarantee against heat, I had closed Maytech as well which never hit thermal cutoff.

I had to finish my test ride because the SK8's got boiling hot after 20-30 minutes which is weird, it's only 25°C outside. 

The other thing is the new FW didn't fix my "releasing brake" problem but my motors jitter and sound like a fart shortly before standstill. That should fix the "locking brakes" which I never had. Also the brake feels weaker with the same settings as before. Now I change the regen Batt to ridiculous -40A each Vesc (equal to motor min) just to see if that would fix my brake problem. If not I return to FW 3.38 before I mount the 6384. Damn I've expected better performance...
```

---
## \#832 Posted by: telnoi Posted at: 2019-07-19T17:24:12.259Z Reads: 71

```
Somehow, I feel lucky with all my old shit.
Still on SK3. The bells are now starting to rust a little bit, but they are still moving along just fine. 
Still on BLDC. No sensors...no canbus... Just needs a shove forward to get going. Oh, old focboxes on 12s.
```

---
## \#833 Posted by: rich Posted at: 2019-07-20T21:44:51.188Z Reads: 71

```
[quote="telnoi, post:832, topic:45377"]
The bells are now starting to rust a little bit
[/quote]

I wish I were you :rofl:!

One or both SK8 started to make additional noises at certain RPM plus the annoying drag from the newest one. All 3 motors I had are pretty done.

It took more time as expected but I could finish the motor swap, hopefully they don't fall apart on the first ride.

Soldering "just" a few wires :smile:
![055455|690x388](upload://oE76Xm4Cs8EYyMHdZFIG7VQ5Gro.jpeg) 
5pin to 6 pin hall sensor cable
![044841|690x388](upload://ttwLQpR9gQoU5TAZu4fftNHFOi8.jpeg) 

![094024|690x388](upload://9hMzl4evnEwKNJFNLMv2e5OT2fm.jpeg) 

Due to the construction of the motors and the smaller motor helicals there were holes.
![190722|690x388](upload://19FKAlS18aG40Dxzi5vmDVKCUtd.jpeg) 

Closed them with flexible glue (removable).
![191813|690x388](upload://jQ2caeZxLtmZMoFYfXP7JF6dgBa.jpeg) 

Just the wheels are missing now, I'm very curious about the maiden voyage tomorrow and how they perform.
![222027|690x388](upload://d53emDfWPWRoTF5QRJkHUpT3Q2A.jpeg)
```

---
## \#834 Posted by: rich Posted at: 2019-07-22T11:15:03.542Z Reads: 59

```
[quote="Andy87, post:822, topic:45377"]
Why you change to 6.25 gearing and go up with kV? i mean the end result of torque and speed should be similar than, no?
[/quote]

I quote this the second time because now I have a real answer :grin:

Ok as mentioned I've expected better performance but it is not better, it is much better! I can climb hills which were unrideable with 1:5 gearing and 149kv. It's difficult to describe but the dirt machine turned into the real dirt machine. When braking hard it's difficult to keep riding straight, a wicked new experience. When climbing hills while accelerating hard the front wheels start to lift :laughing:

Unfortunately the 6384 have the same problem with heat as the SK8, after about 20 minutes I hit 85-100° C. The motors have no temp sensor so I depends on me to save them from burning.

One motor helical got loose after 1 hour so I had to walk back home and need to glue it again, this time with more Loctite.
```

---
## \#835 Posted by: Andy87 Posted at: 2019-07-22T12:00:01.050Z Reads: 59

```
I didn´t ride anything less than 170kV yet, but with my actual setup at 170kV 6384 and 1:4.67gearing at 80A bat 90A motor I´m pretty happy. if i hit the throttle the front wheels lift up easy. once, twice that much that the board just shoot out under me when accerlating out of a turn :rofl: 
good to see that the cheap motors worked out for you!
```

---
## \#836 Posted by: rich Posted at: 2019-07-22T12:39:27.935Z Reads: 57

```
Ha didn't know your setup is that powerful, great :muscle: 

My front wheels only lift uphill.
```

---
## \#837 Posted by: Andy87 Posted at: 2019-07-22T13:04:06.029Z Reads: 56

```
I don´t think mine is more powerful than your.
I wonder about your range. I did a range test with my 12s7p VTC5A which i think should be around the same capacity wise than your 12s6p and i make around 28km till 3.4V on mostly flat street, gravel. 
I think gears and your light weight add up to 10-12% more efficent riding. super interesting.
hope one day i will get gears as well and a bit more range too :sweat_smile:
```

---
## \#838 Posted by: rich Posted at: 2019-07-22T13:14:42.322Z Reads: 56

```
[quote="Andy87, post:837, topic:45377"]
28km till 3.4V on mostly flat street, gravel
[/quote]

I have about the same range,

28-30km until 3.5V, 37km until 3.2. The end of discharge is 2.5V so I guess I could reach 43km. Too bad my BMS shut down at 3V.

I realized that Li-ion keep the low voltage much longer than lipos. My 8Ah lipo decreased from 3.5V to 3.2V within 50-100 meters, with Li-ion it's at least 7km.
```

---
## \#839 Posted by: Andy87 Posted at: 2019-07-22T13:22:24.002Z Reads: 58

```
7km out of the 3.5-3.2V is a lot. 
I think you can easy discharge till 3.0-2.8 cut off if the bms wouldn´t cut out before.
As it was the first runs on mine i didn´t wanted to go that low as I first wanted to figure out how much the pack sags in the low voltage area. I think for offroad better to stay around 3.3-3.1V though.
```

---
