# Unreasonable E-MTB build - Me too, I want to faceplant on dirt at 60km/h (and commute everyday too)

### Replies: 71 Views: 2134

## \#1 Posted by: boubak Posted at: 2018-09-11T16:31:15.715Z Reads: 410

```
Hello,

**Context**

I'm Boubak, a software R&D engineer from France :).

From the very beginning I wanted to build something that make me sh*t in my pants and commute
because as somebody working in Paris, I hate the subway and I really prefer to be outside, exploring the city everyday.

My first attempt was a build based on a loaded tan-tien longboard with paris trucks, i-don-t-know-the-brand-anymore belt motor mounts, APS sensored 220kv 50-ish mm 2200w motors (don't remember to be honest), 2 4.7 vesc and 8S li-po battery pack.

It was great, really!

But I started to neglected it since I realized that it was inconvenient:

* Flexible board with battery pack under, so I never found a satisfactory option to mount other than the temporary rope+plywood+plastic-collars
* Not waterproof at all
* Not offroad enabled
* Need to get off the board to get on sidewalks
* Hardware vulnerable under the deck
* Could be more powerful

So I couldn't really use it daily, and no offroad at all (I was raised a snowboarder, I want to do offroad, I need it..).

**My goals with this project**

So, I wanted to ride something more bullet-proof, rain-proof, offroad-proof, with the hardware uperside, more powerful and that can get on sidewalks.

So, after reading a lot of post on this forum (especially from @NoWind and other no-limit E-MTB builders ), and after spending many months viewing @Nowind youtube channel (and dreaming I was him riding his machines :smiley: ), I decided that it would be an E-MTB ! \o/

**My BOM, so far..**

Considering I'm 175cm, weight ~75kg and carry a 13kg backpack

Board : Trampa HolyPro 35 16 ply with infinity or vertigo trucks, superstar hubs and trampa threads or primo alpha

Motors : APS C8085 sensorless 170kv with AS5047 magnetic encoders

ESC : Dual V6 esc from Trampa or Flipsky, best if with integrated anti-spark switch

Battery pack : 12S Li-po setup (4 x Compact 6200mAh 6s 40c Lipo Pack w/ XT90) with a 200A BMS from Bestech (like the  HCX-D575 ) 

Remote controller and receiver : my hobby remote and receiver

Motor mount : Direct drive (with helical gears?) from @Nowind, if possible with custom motor cages with AS5047 mounting capabilities ( is it possible ? )

Additionnal stuff : Custom aluminium waterproof battery enclosure and custom aluminium heatsinking VESC enclosure CAD-ed by me (I need to train more on freecad) and manufactured by any prototyping company willing to do it. A lot of 8AWG and 10AWG silicon wire. Maybe bluetooth telemetry.

**A lot of questions**

So here is my plan.

And I'm sure about almost nothing XD.

And I ask me a lot of questions:
* What about risks of frying drv with transients on a VESC with a 12S ?
* Will my custom battery enclosure ( that I would between my foots) prevent the board from flexing ?
* Is it really possible to make it rain-proof ?
*  Does 2 C8085 motors fits with motor mounts and cages and AS5047 housing on a standard Trampa Infinity truck
* Is is possible to dissipate enough heat by screwing 2 VESC on an aluminium box (with thermal paste) to run them at constant 100A max motor current  in BLDC?
* The same in FOC ?
* If it works, will I die in the 2 weeks following the completion ?

What do you think about it :slight_smile: ?

Boubak
```

---
## \#2 Posted by: Grozniy Posted at: 2018-09-11T16:37:17.032Z Reads: 356

```
Opinion on batteries: from reading the forum for almost a year, the consensus is that lipo C rating is overrated. That means get more than 60C discharge, preferably graphene batteries. If you go 10S it will safer for the vesc and with proper gearing, you could get the same top speed.
```

---
## \#3 Posted by: Trdolan03 Posted at: 2018-09-11T17:53:28.538Z Reads: 349

```
You are completely fine gunning 12s on vesc 6 hardware. I am a fan of 12s 8p 25r liion packs with NESE modules. Not sure if range is a concern for you but if it is...this will definitely cover what your looking for
```

---
## \#4 Posted by: Okami Posted at: 2018-09-11T17:53:50.477Z Reads: 346

```
@okp @Riako

Both from france. Does a lot of off road / street riding. Maybe can spare a minute to give some tips
```

---
## \#5 Posted by: okp Posted at: 2018-09-11T18:23:45.930Z Reads: 334

```
Hey @boubak. [okp](https://www.instagram.com/ridewithokp/) here Join the ESK8FR shredding session group rides that I organize in Paris. You'll meet diversity with a bunch of people riding different boards !

On my side, you can either get parts from me (unikboards.com) or from Jens (http://e-toxx-shop.com) or from some other folks and I can build you or support you in the build of your board.

I always ride 12S on VESC, FOCBOX on my side but my mate @Nowind  will also advise you.

In any case, you cannot go wrong with @Nowind stuff. I just received a MBS Matrix 2 direct drive from him to build a board and I can tell you, that you cannot buy happiness but this is pretty close.

Join us on the No Car day in Paris this week for some hardcore riding ;)

Cheers !
```

---
## \#6 Posted by: boubak Posted at: 2018-09-12T09:31:06.962Z Reads: 311

```
Thanks everybody for your replies !


@Grozniy :  

[quote="Grozniy, post:2, topic:67726, full:true"]
Opinion on batteries: from reading the forum for almost a year, the consensus is that lipo C rating is overrated. That means get more than 60C discharge, preferably graphene batteries. If you go 10S it will safer for the vesc and with proper gearing, you could get the same top speed.
[/quote]

For my battery pack, I didn't cogitate at all, I just choose the same initial setup as @Nowind :)  thinking that if it works for him, it will for me.

I will take a look at graphene batteries, thank you :slight_smile:

My main goal is more having torque than top speed (even if top speed is cool too) so I fear that If setup a 10S
battery pack, for the same top speed, I will need a higher KV motor. And for the same power it will draw more current ( so my electronic setup will maybe suffer more or need more heatsinking ).
Another problem is that I want to go with the @Nowind Direct drive unit, so the gearing seems constraint by the size and shape of it. 



@Trdolan03 :

[quote="Trdolan03, post:3, topic:67726"]
You are completely fine gunning 12s on vesc 6 hardware.
[/quote]

Even if I draw a lot of current ? (like 100A per motor). If that's the case, it's very cool !


[quote="Trdolan03, post:3, topic:67726"]
I am a fan of 12s 8p 25r liion packs with NESE modules. Not sure if range is a concern for you but if it is…this will definitely cover what your looking for
[/quote]
About the battery pack, my main concern is not really the range, more the capability of giving a lot of current and the size.
If I can ride 15-20 kms on a single charge accross Paris, It's perfect for me.
Do you think it's achievable considering the build I want to do ?

I will take a look at the li-ion elements you advised anyway :slight_smile: , Thank you.

@Okami : 
 
Thank you for the tips :slight_smile: 

@okp : 

[quote="okp, post:5, topic:67726"]
Hey @boubak. [okp](https://www.instagram.com/ridewithokp/) here Join the ESK8FR shredding session group rides that I organize in Paris. You’ll meet diversity with a bunch of people riding different boards !
[/quote]

I will join with pleasure as soon as my build is ready :smile: ! ( I didn't realize there was such events from the French esk8 community ).

[quote="okp, post:5, topic:67726"]
On my side, you can either get parts from me ([unikboards.com](http://unikboards.com)) or from Jens (http://e-toxx-shop.com) or from some other folks and I can build you or support you in the build of your board.
[/quote]

I think I will a lot a questions to ask you, thank you ! Do you have a physical shop in Paris ?

[quote="okp, post:5, topic:67726"]
In any case, you cannot go wrong with @Nowind stuff. I just received a MBS Matrix 2 direct drive from him to build a board and I can tell you, that you cannot buy happiness but this is pretty close.
[/quote]

Yes, seems to be the kind of high quality stuff you want at least to take with you in the bed in case you need to look at it because you can't sleep, continuously thinking about it :stuck_out_tongue_closed_eyes:

[quote="okp, post:5, topic:67726"]
Join us on the No Car day in Paris this week for some hardcore riding :wink:
[/quote]

I can't since for now I haven't any esk8 build complete anymore >< (I dismantled my previous one).
I need to live in shame being a pedestrian..

Cheers !
```

---
## \#7 Posted by: Andy87 Posted at: 2018-09-12T09:51:55.355Z Reads: 239

```
[quote="boubak, post:1, topic:67726"]
* Will my custom battery enclosure ( that I would between my foots) prevent the board from flexing ?
* Is it really possible to make it rain-proof ?
[/quote]

It will not if you design it right.
I split mine to two separate boxes and both I´ll bolt with 4 bolts only in the middle of the box.
Between the box and the deck I´ll add a 5mm spacer which will give the box some more space on the corners.
you could also velcron the battery to your deck.
there is pretty strong velcron available and it always gives some room if board is flexing.

And second, yes for sure it´s possible to get it water prove. Just seal it right. 
I know you want to design your own box, but just wanted to notice that a lot of guys use modified pelican box as battery storage. 
https://www.peli.com/eu/de/products/cases/storm-cases?gclid=CjwKCAjw8uLcBRACEiwAaL6MSepqhj2-I22mYoC9hQ3u-MmikvSk-TGVsawhc1tx9QCTeKent781TxoCYh8QAvD_BwE
Maybe it´s just me being a sissi, but I wouldn´t have a good feeling with my batteries in a aluminum box :sweat_smile:
```

---
## \#8 Posted by: boubak Posted at: 2018-09-12T12:45:03.228Z Reads: 251

```


@Andy87 : 

Thank you for your reply :slight_smile: 

[quote="Andy87, post:7, topic:67726"]
It will not if you design it right.
I split mine to two separate boxes and both I´ll bolt with 4 bolts only in the middle of the box.
Between the box and the deck I´ll add a 5mm spacer which will give the box some more space on the corners.
you could also velcron the battery to your deck.
there is pretty strong velcron available and it always gives some room if board is flexing.
[/quote]

 Ok, I thought about something in that spirit, but I don't understand the *"4 bolts only in the middle of the box"* part. Could you please elaborate ? ( or better, put a picture of your setup :stuck_out_tongue: ) 

I also thought about three more options :

* Adding degres of freedom to my box by anchoring it with rods and ball joints at the 4 bottom corners (a little bit like the anchoring of cells on top of offroad trucks)
* Putting my battery pack box at the opposite of the VESCs box, on top of the front truck --> **Big advantage of balancing the masses of the board**
* Splitting my battery pack in two separate boxes : one on top of the front truck, the other between my feet --> hybrid between your proposition and my second one but meh, not convinced..


[quote="Andy87, post:7, topic:67726"]
And second, yes for sure it´s possible to get it water prove. Just seal it right.
[/quote]

My main concern with this is having a 200A BMS heatsinked properly **inside** my waterproof batteries box :confused: 

[quote="Andy87, post:7, topic:67726"]
And second, yes for sure it´s possible to get it water prove. Just seal it right.
I know you want to design your own box, but just wanted to notice that a lot of guys use modified pelican box as battery storage.
[/quote]

I want to avoid this solution because I never found the right form factor, and it will be hard to heatsink properly, I think.
And beside that, I don't like the look of this solution :confused:, useless handle, round corners, not well integrated in the final product...but that's just personnal taste :slight_smile: 

Boubak
```

---
## \#9 Posted by: Andy87 Posted at: 2018-09-12T13:08:37.681Z Reads: 244

```
![IMG_6038|375x500](upload://7RivHrVtyLjmLtkSPkOC6pXosnU.jpg)

horrible picture but I think you get the point with only in the middle.

I now don´t get your point with the batteries on top of the back side of your vescs on the front truck...
You plan to install the vesc on the front truck?
As kind of balancing the board if I understand right?

In general a good idea, just be aware that with long wires you can get voltage spikes which can fry your vesc. Especially the wires from the battery to the vesc should be as short as possible.
If you need longer wires, add some capacitors which can flatten the voltage spikes.

One thing I also wanted to ask you.
Do you have any experience in how much amp you draw on the road and off road?
100A per vesc is a lot (especially constant) 
if I didn't calculated wrong with a 12s it would be about 8,8kW for your two motors. 
I doubt that there is a hill in paris which would need that power constant to climb up.
just don´t understand the reason behind.
100A constant means also bigger wires, shorter wires, more heat sink etc etc (by the way you know that the VESC 6 in the housing it comes only can handle up to 60A constant)
lot of extras which you probably will not, never ever use.
You could ask here in the round some MTB experts, what´s there average amperage. I can only say you what you will need on the flat road and that´s far away from 200a
```

---
## \#10 Posted by: boubak Posted at: 2018-09-12T14:40:35.619Z Reads: 237

```
@Andy87 : 

Thank you for the drawing, it's now perfectly clear :slight_smile:

[quote="Andy87, post:9, topic:67726"]
I now don´t get your point with the batteries on top of the back side of your vescs on the front truck…
You plan to install the vesc on the front truck?
As kind of balancing the board if I understand right?
[/quote]

My explanations were confusing, my bad ><.
What I wanted to said is that I could mount the batteries box on top of the front truck and the VESCs box on top of the rear truck. With this configuration there will be kind of same amount of mass on the front than on the rear :slight_smile: 

[quote="Andy87, post:9, topic:67726"]
In general a good idea, just be aware that with long wires you can get voltage spikes which can fry your vesc. Especially the wires from the battery to the vesc should be as short as possible.
If you need longer wires, add some capacitors which can flatten the voltage spikes.
[/quote]

I didn't know that :open_mouth:, what is the electrical principle involved ?

[quote="Andy87, post:9, topic:67726"]
One thing I also wanted to ask you.
Do you have any experience in how much amp you draw on the road and off road?
100A per vesc is a lot (especially constant)
if I didn’t calculated wrong with a 12s it would be about 8,8kW for your two motors.
I doubt that there is a hill in paris which would need that power constant to climb up.
just don´t understand the reason behind.
100A constant means also bigger wires, shorter wires, more heat sink etc etc (by the way you know that the VESC 6 in the housing it comes only can handle up to 60A constant)
lot of extras which you probably will not, never ever use.
You could ask here in the round some MTB experts, what´s there average amperage. I can only say you what you will need on the flat road and that´s far away from 200a
[/quote]

My previous build was with a longboard, so only a road one without telemetry, but by slowing the wheel mechanically on my test bench with kind of the same amount required by the steepest hill I know, the biggests spike where around 45A per motor.

I'm aware that I will not need 100A constantly, it was more to have a big safe margin considering that I'm quite demanding on my gear when doing a board sport and that I don't want to be constantly monitoring the health of my board if I suddendly decide to go hardcore offroad.
In the spirit of the @Nowind riding style I guess :smile: (that's also why I'm considering the same kind of current values)

Concerning the two VESC 6, my plan is to bolt them on a bigger heatsink/enclosure with thermal paste
I already planned to go big with wires.

Cheers!

Boubak
```

---
## \#11 Posted by: Andy87 Posted at: 2018-09-12T14:59:30.574Z Reads: 198

```
[quote="boubak, post:10, topic:67726"]
I didn’t know that :open_mouth:, what is the electrical principle involved ?
[/quote]

Induction. It also helps to place the plus and minus as close to each other as possible. As the forces work than against each other and minimize the effect
```

---
## \#12 Posted by: boubak Posted at: 2018-09-12T21:01:45.891Z Reads: 206

```
@Andy87 
[quote="Andy87, post:11, topic:67726"]
Induction. It also helps to place the plus and minus as close to each other as possible. As the forces work than against each other and minimize the effect
[/quote]

Thank you for the explanation.
I didn't think it could have such a noticeable effect with wire of just 1 meter length.

Anyway after second thought, I don't think I can put a 12S 2P 12400mAH battery pack with BMS on top of the front truck, it will be too big.


[quote="Andy87, post:7, topic:67726"]
Maybe it´s just me being a sissi, but I wouldn´t have a good feeling with my batteries in a aluminum box :sweat_smile:
[/quote]

Can you elaborate please ? :slight_smile: 

Cheers,

Boubak
```

---
## \#13 Posted by: Andy87 Posted at: 2018-09-13T05:04:18.380Z Reads: 183

```
It’s just because aluminum is electrically conductive. Sure you can heat shrink everything or cover the inside with neoprene than it shouldn’t be an issue.
I just prefer non conducive materials like fiberglass or plastic
```

---
## \#14 Posted by: boubak Posted at: 2018-09-13T07:22:07.299Z Reads: 181

```
Ok, I thought maybe there was something more esoteric I'm not aware of. I plan to do a proper insulation of the inside of the box.

By the way, what about security holes or exhausts in case of battery fire ? 
Is it a common practice amongst the esk8 community or does we just consider we can take the risk because it is very small because we take care of battery pack/we have BMS ?

I don't remember to have read anybody post about that ( but maybe I didn't search hard enough )

Cheers,

Boubak
```

---
## \#15 Posted by: Andy87 Posted at: 2018-09-13T07:31:21.791Z Reads: 175

```
I had a fire and it burned down the sealing and plastic parts of my enclosure...
Don´t know how it would be if you make a full sealed aluminum battery box. You could make some holes which you cover with neoprene or silicon, it will meld away fast and the pressure can release. 

PS: get some fire protection covers, or a fire extinguisher or a big gallon of salt water for your home!!! Better all...if you work with batteries, doesn´t matter which, it should be standard to have some protection close by. 

[quote="boubak, post:14, topic:67726"]
we just consider we can take the risk because it is very small
[/quote]

It´s not small at all!!! don´t take it on the easy side. 300+Wh are a lot of energy if it´s get released in just some seconds
```

---
## \#16 Posted by: boubak Posted at: 2018-09-13T09:14:12.665Z Reads: 178

```
[quote="Andy87, post:15, topic:67726"]
It´s not small at all!!! don´t take it on the easy side. 300+Wh are a lot of energy if it´s get released in just some seconds
[/quote]

What I mean by small is "very unlikely", it was confusing :slight_smile:.
I very well aware of dangerousness of a battery fire.

 [quote="Andy87, post:15, topic:67726"]
PS: get some fire protection covers, or a fire extinguisher or a big gallon of salt water for your home!!! Better all…if you work with batteries, doesn´t matter which, it should be standard to have some protection close by.
[/quote]

I already have all of that in my shop, that's not the first time I work with big batteries :smile:. 

 [quote="Andy87, post:15, topic:67726"]
You could make some holes which you cover with neoprene or silicon, it will meld away fast and the pressure can release.
[/quote]

I thought about something in that spirit, I will do my research on the subject.

Do you know if someone on this forum made something similar?

P.S : Don't take the tone of my posts as a form of inconsistency or a brainless attitude, I'm just free of any assumptions on the questions I ask :slight_smile:.
```

---
## \#17 Posted by: Andy87 Posted at: 2018-09-13T09:43:16.618Z Reads: 149

```
for now I don´t know anybody who made an aluminum on board mount. most guys here just use the plastic boxes or use a tray for under the deck. 
you could look through the "just pictures" thread, maybe you will find somebody who already made something similar.

no problem about the posts, just ask your things.
better to discuss things and get ideas than just start work and in the end need to redo the half again...
```

---
## \#18 Posted by: boubak Posted at: 2018-09-13T13:54:23.675Z Reads: 173

```
[quote="Andy87, post:17, topic:67726"]
for now I don´t know anybody who made an aluminum on board mount. most guys here just use the plastic boxes or use a tray for under the deck.
you could look through the “just pictures” thread, maybe you will find somebody who already made something similar.
[/quote]

Good idea, thank you !

[quote="Andy87, post:17, topic:67726"]
better to discuss things and get ideas than just start work and in the end need to redo the half again…
[/quote]

I agree :slight_smile:, but I wanted to specify my mind state, I know I can sound very candid with my way of asking questions. 

Cheers,

Boubak
```

---
## \#19 Posted by: Andy87 Posted at: 2018-09-13T13:55:43.208Z Reads: 168

```
For me it’s fine. Keep on going 😜
```

---
## \#20 Posted by: Riako Posted at: 2018-09-13T15:20:07.481Z Reads: 195

```
Fensh Mountainboards shop used Alu box.
Look at Overion.fr he make central and rear Box, full Alu, made by itself, top plate customisable color (anodising) and other custom. All in the box, nothing else :ok_hand: like it so, just a bit heavy of curse VS Carbon fiber or like that.

https://amadridefr.files.wordpress.com/2018/09/img_20180314_175607l.jpg?w=720

https://scontent-lhr3-1.cdninstagram.com/vp/dcfd411a45a1b68ba219e151eb655346/5BE95B2E/t51.2885-15/e35/35616484_1083736291782633_4730868045176635392_n.jpg?ig_cache_key=MTgxNDQ1NTM2OTc0Nzc5ODMwOQ%3D%3D.2
There is also Willozboard with a compact 12s5p bms in a small Alu case.
This two produce and ride eMTB since a long long time already (around 2007), before we start looking info on forum or even think about it :star_struck: they're kind of genius with gold-hand.
https://wib-sport.com/317-large_default/e-mountainboard-willozboard.jpg
https://scontent-ort2-2.cdninstagram.com/vp/c61fa254283bef95eea953f5fa2a9df6/5BEE8F87/t51.2885-15/e35/22860841_1904241743225453_6229204623752691712_n.jpg
```

---
## \#21 Posted by: boubak Posted at: 2018-09-13T15:40:50.826Z Reads: 193

```
OMGOMGOMG ! Thanks a lot @Riako, I will take a look at those marvels :slight_smile:  

Cheers !

Boubak
```

---
## \#22 Posted by: boubak Posted at: 2018-09-19T13:43:38.601Z Reads: 200

```
Unfortunatly none of the two battery pack will fufill my needs:

* Overion box is not waterproof
* Willozboard box can't go higher than 100A

BUT, the willozboard design really inspired me, especially the fastening system with pp belts : 
![Willozboard battery pack fastening system](https://wib-sport.com/396-large_default/e-mountainboard-willozboard.jpg) 

And I have my first dilemma, I want to choose which VESC 6 model to buy, and I want a robust one:

[VESC6 from Trampa](http://www.trampaboards.com/1x-vesc-6-in-cnc-t6-silicone-sealed-aluminium-box-with-genuine-xt90-connectors--vedder-electronic-speed-controller-trampa-special-p-24333.html) : 

* **Pros :**
  *   the official from Benjamin Vedder can go up to 80A continuous
  *   tested and abused by @NoWind, seems to wistand at least 100A continuous under good cooling conditions

* **Cons :**
  *   no integrated anti-spark switch
  *   the most expensive one

[Flipsky FSESC 6.6 with aluminium case](https://flipsky.net/collections/electronic-products/products/fs-esc-6-6)  :

* **Pros :**
  *  with integrated anti-spark switch
  *  seems to be waterproof out of the box
  *  affordable

* **Cons :**
  *  advertised for 60A continuous
  *  not sure if it's quality built
  *  currently sold out

[Flipsky Dual FSESC6.6](https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-based-upon-vesc6-with-aluminum-heatsink) :

* **Pros :**
  *  dual esc on the same PCB
  *  integrated CAN connexion
  *  up to 100A continuous per ESC
  *  affordable

* **Cons :**
  *  no anti-spark switch anymore
  *  not sure if it's quality built.


I can't decide between the three of them.
I'm open to any piece of advice/observation and other VESC based ESC I don't know right now :).

P.S : Can I safely control two anti-spark switch from the same button ? (or maybe there are 200A anti-spark switch?)

Cheers,

Boubak
```

---
## \#23 Posted by: Andy87 Posted at: 2018-09-19T14:12:50.390Z Reads: 187

```
Get one of this
https://www.electric-skateboard.builders/t/escape-group-buy-professional-pcb-assembly/49720?u=andy87

If you lucky stewii has two left for you.

Don’t relay on the Flipsky 6.6 anti spark.
I can’t proof it with own experience, but I read here that the switch is the only down side of this vesc.

Get one of this 
https://www.electric-skateboard.builders/t/push-to-start-switch-out-now/60879?u=andy87

From @Martinsp if i‘m not wrong they work up to 150a
```

---
## \#24 Posted by: Riako Posted at: 2018-09-19T18:19:40.113Z Reads: 162

```
Yes, try to go with the ESCape, or maybe the new fsesc6.6 without antispark.
Put an XT90s or someting like that maybe for your PSA ;)
```

---
## \#25 Posted by: boubak Posted at: 2018-09-22T09:46:32.136Z Reads: 164

```
@Andy87 and @Riako : 

Thank you both for your advice :slight_smile: .

I think I will try to buy dual ESCape from @stewii,  It seems to be very nice, especially with the heatsinked dual enclosure in aluminum.

@Andy87 : 

Thanks, I started to get in touch with @Martinsp for his cool  anti-spark switch.

@Riako : 

PSA :slight_smile: ? Power Switch Alchemy ? Portable Super Anchor ? Peugeot Citroen XD?
```

---
## \#26 Posted by: Riako Posted at: 2018-09-22T09:52:18.113Z Reads: 154

```
Sorry, to use an XT90S as Power Switch Anti-spark ;) 

[sl33py](https://www.electric-skateboard.builders/u/sl33py) make a good how to if you want more details > https://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204
```

---
## \#27 Posted by: boubak Posted at: 2018-09-22T10:13:43.852Z Reads: 151

```
Thank you :slight_smile: I will take a look but I think I prefer an electronic anti-spark switch.

By the way can an XT90 connector sustain a 200A current indefinitely ?

Cheers,

Boubak
```

---
## \#28 Posted by: Octave Posted at: 2018-09-22T10:16:32.528Z Reads: 145

```
I'm pretty sure an xt90 can take up to 90 amps.
https://electricbike.com/forum/forum/builds/new-builder-questions/30414-xt90-max-watts
```

---
## \#29 Posted by: boubak Posted at: 2018-09-22T10:49:04.939Z Reads: 144

```
Thanks for the information, so with my goal of oversizing stuff for bullet-proofing my build, it's maybe not a good idea to have XT90 connector to handle 200A.

Cheers,

Boubak
```

---
## \#30 Posted by: Andy87 Posted at: 2018-09-22T12:36:04.241Z Reads: 146

```
which wires you want to use for 200a?
If you really think you need to oversize your build you can run only positive wires through one xt90 and only negative wires through one xt90.
It would give you 180a in total.
```

---
## \#31 Posted by: boubak Posted at: 2018-09-22T17:51:28.817Z Reads: 146

```
8 or 6 awg

And I will not use XT90 for the main power wires,
but big bullet connectors instead.
```

---
## \#32 Posted by: Kug3lis Posted at: 2018-09-22T18:14:25.195Z Reads: 164

```
Good luck trying to achieve 200A :D I am running ±90A mot/bat battery never reached more than 50A on bat per esc. XT90 is more than enough. I am at the moment running everything via AWG 12 and even MT60 motor phase connectors they get a bit warm after long rides but everything else is not even warming up :)

Plus not a single esc on this forum apart maybe arc (haven't tried or didn't hear anything about it yet) could handle 100A bat continues without heavy sweating :) 

Don't forget your battery wires are not even bigger than 10AWG and internal tabs will not handle more than 100A continues just short burst of high current :)

ESK8 Loads are short burst so wires/connectors don't even feel it :) It's more concerned for like E-Foils where they have constant loads :) 

So I don't see the point of over-engineering this stuff :slight_smile: just a waste of money :)

![image|375x500](upload://7HHU3CXaOFAxJ3yE8Jiw5HRbqrD.jpeg)
```

---
## \#33 Posted by: boubak Posted at: 2018-09-26T06:59:44.058Z Reads: 164

```
@Kug3lis 

Thanks for your message !

I disagree :slight_smile: and I will try to explain my logic :

You don't take into account my initial constraints, especially one  : 
*   bullet-proof

From the strict engineering point of view, I have no interest in lowering the modularity of my system by downgrading subcomponents of the power chain to match them with their neighbors. It will just be an pre-optimisation, for gaining what? Small savings and a little bit of weight.

And money was never in the constraints (neither weight by the way).

I will add that 200A continuously is my goal for having a safety margin considering the worst case.

Plus we have two kinds of components : 
*  the self-protected
*. the others

In the "self-protected" category we have all the bottlenecks , naming the ESCs and the battery pack (according to the fact that I will put a BMS).
They will cut before burning.

In the "others" category I have : 
*  Motors -> APS C8085 : big safety margin
*  anti-spark switch -> dual push to start from @Martinsp : 200A continuously 240A in burst
*  Wires and connectors -> I want a big safety margin too, because as the two previous from the same category, they will not protect themselves.

Doing that will insure me that I don't add point of failures and that if someday I change my ESCs for something that can withstand 200A continuously, I will not have to change other components. So it keeps my build modular.

And I prefer having just my ESCs sweating instead of everything in the worst case.

[quote="Kug3lis, post:32, topic:67726"]
Don’t forget your battery wires are not even bigger than 10AWG and internal tabs will not handle more than 100A continues just short burst of high current :slight_smile:
[/quote]

I want to build a 12s2p pack from 4 Compact 6200mAh 6s 40c Lipo Pack from Zippy, that makes a 12400mAh 40C pack : even if considering that it's bullshit and that I must only take account of 20C for safety reasons, that means drawing 248A max continuously.
Plus they will be managed by the BMS.

And I have turnigy lipos from an other project that have 8AWG wires, so 10AWG is not the max at all on commercial packs.

I will add that you're giving me your ride values, but it's irrelevant :slight_smile: : we probably don't ride the same way, not with the same  hills, not with the same external temperatures, so I'm pretty sure we have different needs(commuting in Paris is just a part of the story).
And I know myself and I am pretty demanding on the gear I use when doing board sports and motor sports.

And I know that It will be more difficult to build ( especially the "heatsinking the BMS" part, I fear)

But maybe my logic is faulted somewhere and I will be happy to now before doing something crappy. :smile: 

And now you know my reasons and that it's not just brainlessness.

Cheers,

Boubak
```

---
## \#34 Posted by: Kug3lis Posted at: 2018-09-26T07:29:47.604Z Reads: 159

```
Well, I am from London, I ride really aggressively and high speeds my average speed on a commute to work is probably will be double than yours :)

![image|230x500](upload://iX5rzPou0e3zH5qHpajdY01nWJQ.jpeg)

![image|230x500](upload://sYNISFdf5F1Hu7OUyJp5X7atCRD.jpeg) 

![image|230x500](upload://t2DZH67I5D8iBGXifKbHNonYMtT.jpeg)  

These are just like highest values I can find consumed from the battery and etc :) 

But yeah I was the same thinking like adding copper 2cm bus bars and etc on the build I am currently riding and was thinking that I will need attach everything directly to it and other things after riding for more than 5k miles I just swapped to MT60 connectors still use XT90 on focboxes but if I build next one I will just go with XT60

By the way, my both motor and bat are ±90A never seen it on any of logs :)

But yeah try it out after some time you will come to realise the same as me :D I will be able to tell more after I switch my motors to 80100 in upcoming weeks :) Probably MT60 will heat up quite a bit but still I don't expect more power consumption than now as my board will not change much its weight or resistance and etc probably will even drop as new gear drive is more efficient than the current one :)

But yeah I am not riding much off road yet so maybe I will see more current spikes and etc when I will enter mud roads :D

P.S. Even if you manage to consume 200A you will need to heat sink the shit out of that anti spark switch :) and other components in power delivery side especially BMS if you will be able to find a good BMS with good mosfets and etc :)

But yeah keep working project looks good :)
```

---
## \#35 Posted by: Andy87 Posted at: 2018-09-26T07:45:54.435Z Reads: 134

```
how the f... you stay stable at 80km/h on a trampa?
50-60km/h ok that´s still fine for me, but 80 :sunglasses:
it´s with your own dampas or you ride the white ones :sweat_smile:
```

---
## \#36 Posted by: Kug3lis Posted at: 2018-09-26T07:46:43.934Z Reads: 132

```
blue ones :) I havent even had a single wobble with them :) My dampas are for like up to 40-50kmh max if your legs are strong. Also that was on one big downhill i can't reach more than 68km/h on flat surface :)
```

---
## \#37 Posted by: Andy87 Posted at: 2018-09-26T07:52:29.979Z Reads: 135

```
ok that´s how i expacted it to be :sweat_smile:
I run yellow front and red back and the wobbles start at 50km/h round about.
should be like this.
```

---
## \#38 Posted by: rich Posted at: 2018-09-26T09:01:04.781Z Reads: 154

```
Damn @Kug3lis you ride too fast, hopefully without loose magnets :stuck_out_tongue_winking_eye: 

[quote="Andy87, post:37, topic:67726"]
I run yellow front and red back and the wobbles start at 50km/h round about
[/quote]

I had yellow dampas but after about 1000km they got weaker and speed wobble started at about 40km/h.

@boubak sounds like a fun build, especially with 80mm motors!

Just a few thoughts, if you really reach 200A from battery I send you a gold medal. I think maybe you could have 150A spikes depending on your settings but not continious. I use 6374 motors (65A motor max / 50A batt max) and normally I reach together 100-130A motor max and 50-70A batt max each ride. Only once I reached 97A batt max but only because I wanted to reach it. I did hardcore 100% throttle accelerations from standstill.

I have the Vesc6 inside an ABS enclosure without cooling and quite rainproof. It's getting warm inside but not hot. Even in sizzling summer the temperature of the vescs never exceed 50-60° C. 

BTW my enclosures are fine with rain but I found out that my remote didn't like rain and my voltage meter broke. Easy solution for remote: put hand with remote inside a plastic bag :laughing:

I bolted my pelicase with 4 screws to the deck each 4cm away from center to keep the flex as @Andy87 explained. Best would be more narrow or only in the middle but I'm not sure stability wise. It's important to use some rubber spacers between deck and enclosure for flexing. My first enclosure was steel without rubber spacers and it bent. Now I can bottom out the deck without problems.

![180037|690x388](upload://io0IoXwfL33lVXZogwEuAUwcRFF.jpeg) 
![20171108_200403|690x388](upload://gBP3Sfz6f8ZgNReixKtxw7Rbnvi.jpg) 
![20171204_144005|690x388](upload://oT54yng26SzfqBTz7fxTk13mjxL.jpg)
```

---
## \#39 Posted by: Kug3lis Posted at: 2018-09-26T09:06:26.096Z Reads: 146

```
Still with loose magnets :D But I am with blue dampa so no wories about wobbbles :)
```

---
## \#40 Posted by: rich Posted at: 2018-09-26T09:07:33.497Z Reads: 143

```
I wonder if the motor can lock up with loose magnets, i would be afraid
```

---
## \#41 Posted by: Kug3lis Posted at: 2018-09-26T09:09:55.472Z Reads: 138

```
Well they just make weird noises. Power of inertia of spinning fast in worst case scenario would grind that magnet I guess... :thinking:  As the magnets are supper brittle :)
```

---
## \#42 Posted by: Andy87 Posted at: 2018-09-26T09:14:39.553Z Reads: 140

```
was thinking about it too...
after one of my magnets broke during the first bench test, I was wondering what would happened if one magnet becomes lose on the road.
will it crash into the stator? :thinking:
```

---
## \#43 Posted by: rich Posted at: 2018-09-26T09:46:29.124Z Reads: 135

```
Once I shattered one or 2 magnets a bit (crashed backwards into concrete obstacle) and the motor was 100% locked because of tiny magnet pieces. After removing this pieces it could spin again, but had bent shaft and damaged can.
```

---
## \#44 Posted by: boubak Posted at: 2018-09-27T18:18:25.209Z Reads: 140

```
@Kug3lis : 
Thanks a lot for your message !

I don't think I will go this fast :stuck_out_tongue_closed_eyes:, and yes, your commuting path is probably at least twice longer than mine. 

I know that it will probably be overkill, and that I will probably never reach 200A :smiley:,
but that's the point, big safety margin for peace of mind.

And I know too that you're probably right and that I will realize that I got mad about the safety margin.
But I need to realize it myself or I will never be  at peace when riding it (And you could say "I told you").

Anyway thanks a lot for your data and advice :slight_smile: and I am looking forward to looking at your data once you will have switched your motors to 80100 and will have started going on mud roads !

By the way how is the local police behavior about e-sk8 and e-mtb ? One of my very best friends lives in London and is very fond of skateboarding, so I plan to visit him with my build once completed.

@rich

Thanks a lot for your message too :slight_smile: !

Yes 80mm seems to be the starting point of endless fun and dangers !

Your explanations and pictures are very informative, and give me some ref values and ideas about enclosures, flex with battery pack and so on.

By the way what model/size is your battery pack pelicase ?


**Few questions for everybody :**

**I will order my trampa board soon and after reading a lot on this forum I know that I want :** 
*  **infinity trucks** -> because they seem to be the most rugged, especially if I intend to jump in a dirt park
*  **superstar hubs** -> because of e-toxx direct drive (But @3DServisas FatHubs look pretty cool too ! But I don't know if e-toxx drives fit on them and if it's reasonable for now :) )
*  **35 holypro** -> because of shape

**But What I don't know yet is :**
*  **What ply deck rating should I take ?** -> I'm ~75kg + 13kg  while commuting , and ~75 when doing stupid stuff in dirt park/offroad, and I would like something **very stable, but not totally uncomfortable**
   * so I was thinking about **16ply**
    -> what do you think about it (if someone has some ref points to give me, I will be happy) ?
*  **What tyres should I take ?** -> I want to be able to do road and grass riding wet/dry, dirt park and forest riding dry, beach sand wet/dry, so almost everything except deep mud (I will buy other tyres for this purpose later)
   *  I was thinking about **hard compound trampa treads in 8 inches**
-> what do you  think about that ?

Cheers,

Boubak
```

---
## \#45 Posted by: Kug3lis Posted at: 2018-09-27T18:21:31.168Z Reads: 129

```
Our hubs are compatible with superstar mounts so it will work with etoxx gear drive too :)
```

---
## \#46 Posted by: Eboosted Posted at: 2018-09-27T20:06:06.578Z Reads: 128

```
[quote="boubak, post:1, topic:67726"]
Custom aluminium waterproof battery enclosure
[/quote]

An enclosure made of aluminum would need a lot of isolation material, remember aluminum is conductive and your cells will sit on aluminum. This could represent a big hazard, even if you use padding or fish paper, in a case of a crash it could be a big fire wating to happen.
```

---
## \#47 Posted by: Andy87 Posted at: 2018-09-28T04:01:30.689Z Reads: 130

```
I‘m happy with 16ply and i‘m about 85kg plus some extra stuff.
Still flexing good and stabil non the less.
If you want to get more speed, take 17ply for more stability. For the rest 16 is good choice.
Don’t worry about the tires so much.
If you drive how you say you wanna drive you non the less will need to swap them after 300-500km. Enough to try different compounds.
I have a set of primo alpha 8“ but not because of compound, I bought them as I wanted blue wheels 😅
I also have a set of black hard tires from Ali.
Way much more cheap, but very hard compound.
They seem to hold longer so far, but riding comfort is different....
```

---
## \#48 Posted by: telnoi Posted at: 2018-09-28T05:47:12.305Z Reads: 131

```
[quote="Andy87, post:47, topic:67726"]
I also have a set of black hard tires from Ali.
Way much more cheap, but very hard compound.
They seem to hold longer so far, but riding comfort is different…
[/quote]

They are awesome. Not noticing that much of a difference with the hard compound trampa tires when inflating to 60, plus they are much harder to puncture. Had a flat almost weekly with the softies from trampa and mbs.
```

---
## \#49 Posted by: michaelcpg Posted at: 2018-09-28T06:00:12.651Z Reads: 137

```
https://www.amazon.com/gp/product/B00BFU50CW/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1

This is the enclosure I'm using, it's worked really well. I just have it mounted to the top of my deck using velcro which is strong enough that i can carry the whole board via the handle on the case. I've done 10km rides in heavy rain where my shoes will literally be filled with water by the end of the ride but didn't get a single drop of water in the case :slight_smile:

![20180513_192211|690x388](upload://1osrQyirL30z9IPkpGbjUt3PMul.jpg) 

![20180508_194838|690x388](upload://pyNEmSinVbsNkGCcVd9LvHKpzHL.jpg)
```

---
## \#50 Posted by: rich Posted at: 2018-09-28T07:06:25.224Z Reads: 135

```
[quote="boubak, post:44, topic:67726"]
By the way what model/size is your battery pack pelicase ?
[/quote]

It's a Peli case 1150, internal size is about 21 x 14,5 x 8,9cm

I'm also about your weight and have a 16ply deck and it feels good to me. Without money limitations I would have a 15ply with massive battery for endless touring and a 17ply with tiny battery for jumping. 

About tires, it depends on the terrain. If you ride on concrete or hard surfaces a street tire would be best. For offroad I like Trampa treads (hard compound). Actually I use MBS vine (=Trampa mudplugger) tires, they have less traction in offroad conditions but are more comfortable and durable on concrete and hard surfaces because of the middle tread. Also have the thick Aliexpress version of this tire but untested yet.

I'm very curious if you want to faceplant on dirt at 60km/h with halfcap or fullface helmet :laughing:?
```

---
## \#51 Posted by: Andy87 Posted at: 2018-09-28T07:10:18.102Z Reads: 131

```
To make it more easy, here they are
Schau, was ich auf AliExpress gefunden
https://s.click.aliexpress.com/e/crjiP6Gw

The thing is, or was, if you order more than 2 you need to pay a lot of shipping.
So if you order, than order 2x2 and you come around paying for shipping.
```

---
## \#52 Posted by: Woody1989 Posted at: 2018-09-28T08:56:46.382Z Reads: 133

```
Hey @Trdolan03 where do you find this battery?? Is there a link!? And what sort of Ah are we talking here....
You have my attention :-D
```

---
## \#53 Posted by: Trdolan03 Posted at: 2018-09-28T14:35:36.692Z Reads: 133

```
Battery is 20ah. 12s8p of Samsung 25r cross. I used nese modules to assemble the cells
```

---
## \#54 Posted by: rich Posted at: 2018-09-28T14:49:20.196Z Reads: 130

```
[quote="Trdolan03, post:53, topic:67726"]
20ah
[/quote]

:beers: :yum:
```

---
## \#55 Posted by: Trdolan03 Posted at: 2018-09-28T15:04:14.348Z Reads: 128

```
@rich The range is not all that impressive on pneumies. In the low 20’s with nice tire pressure
```

---
## \#56 Posted by: Kug3lis Posted at: 2018-09-28T15:06:59.621Z Reads: 130

```
It's only for you :) With my 18Ah I am getting near 30mi :)
```

---
## \#57 Posted by: Trdolan03 Posted at: 2018-09-28T15:45:04.912Z Reads: 126

```
@Kug3lis What tire pressure? Even at 50psi I struggle to make 30
```

---
## \#58 Posted by: Kug3lis Posted at: 2018-09-28T15:49:40.276Z Reads: 128

```
Well my tires allow max 35 :) that's when I ride in group rides and etc not fast pace rides :slight_smile:

 ![image|679x499](upload://aA5KUFZEknI48tfgDEfdANMDm9R.png)
```

---
## \#59 Posted by: MrDGOrman Posted at: 2018-09-28T16:09:47.748Z Reads: 124

```
Sorry to jump in. I've not read any of the thread but I saw your pictures. Mainly, the first one.

81kph max speed!? 50mph!?!?! ARE YOU MAD BRUV :laughing:
```

---
## \#60 Posted by: Trdolan03 Posted at: 2018-09-28T16:32:06.713Z Reads: 124

```
You will only get 32mph on his setup. That is the unloaded speed.
```

---
## \#61 Posted by: boubak Posted at: 2018-09-28T16:37:43.086Z Reads: 122

```
@Kug3lis : Thank you for this information, you're tempting me I need to think about it :slight_smile:
 
@Eboosted : Yes I'm very well aware of that but if I do an aluminium enclosure it will be enough rugged to consider that the crash requiered to make it catch fire will have to be so big that I will have other problems (i.e death), plus, yeah, solid padding material preventing puncturing of lipo packs inside.

@Andy87, @michaelcpg and @rich : Thank you all for those informations and picture, it's very helpful :) !

@rich : I intend to do that the classiest way possible, I will performs some tests series (100 will be a good start) to find out what is the best with my own lab test dirt floor rectangle.

@michaelcpg : I like you battery wiring :slight_smile:  

@Andy87, @rich and also @DanSkates (from who I follow his freestyle e-ATB topic :slight_smile: ) : 

After what you (@Andy87 and @rich)  said, I'm considering 16ply, but a last question : If I intend to do high jumps like @DanSkates (because I forgot to mention that's part of what I want to do with my e-MTB), will I risk to bottom out my board ?

So for the tyres, I dediced, it will be **hard trampa treads** for now (with spares **innova slick cut**)!

Cheers,

Boubak
```

---
## \#62 Posted by: rich Posted at: 2018-09-28T16:57:41.686Z Reads: 116

```
[quote="boubak, post:61, topic:67726"]
will I risk to bottom out my board ?
[/quote]

You will definitely bottom out your board :rofl:
That's why it's important to mount the battery box in a way that it doesn't restrict flex otherwise your box gets damaged or in worst case the battery. And don't forget PADDING!

I think you can bottom out the stiffest board if jumping high enough. With 16 ply and 74kg it needs about 1 meter height. There's a jump in a close by dirt park where I always land with the middle of the deck only without wheels, that's a loud sound and quite uncomfy :laughing:
```

---
## \#63 Posted by: Kug3lis Posted at: 2018-09-28T17:39:01.874Z Reads: 118

```
[quote="Trdolan03, post:60, topic:67726, full:true"]
You will only get 32mph on his setup. That is the unloaded speed.
[/quote]

No, my board unloaded max speed is 70km/h (you can see in previous calculator picture) it was done on going downhill. On flat surface max I have reached was 66km/h but it was done with 200kv motors, now I am switching to 180kv so no more high speeds :( But I also have 1:4 choice so again will try to see what's better for me in city 1:4 or 1:5
```

---
## \#64 Posted by: Trdolan03 Posted at: 2018-09-28T18:50:48.629Z Reads: 110

```
I forgot to look at kv. My bad. My 190kv with same everything else gets 32mph
```

---
## \#65 Posted by: boubak Posted at: 2018-10-02T16:09:33.526Z Reads: 108

```
@rich 

Thanks for the informations :).

[quote="rich, post:62, topic:67726"]
You will definitely bottom out your board :rofl:
[/quote]

[quote="rich, post:62, topic:67726"]
I think you can bottom out the stiffest board if jumping high enough. With 16 ply and 74kg it needs about 1 meter height. There’s a jump in a close by dirt park where I always land with the middle of the deck only without wheels, that’s a loud sound and quite uncomfy :laughing:
[/quote]

But now I'm more confused XD, I don't know if I should take 16 or 17 ply..
I think that since I want to go really hardcore I maybe need 17 ply, but I'm afraid it could be unpleasant/uncomfortable to ride with this stiffness.

What do you think ?

(The best could be if I can test the board of a french comrade near or in Paris)

[quote="rich, post:62, topic:67726"]
That’s why it’s important to mount the battery box in a way that it doesn’t restrict flex otherwise your box gets damaged or in worst case the battery. And don’t forget PADDING!
[/quote]

Yep :) that's my goal the battery box mounting !
By padding, do you mean padding inside the battery box ( in that case yes offcourse :slight_smile: ) or do you mean something else ? 

Cheers,

Boubak
```

---
## \#66 Posted by: Andy87 Posted at: 2018-10-02T16:17:17.844Z Reads: 108

```
Get in contact with @okp
Idk which ply he has but i‘m sure he can help you out with your choice and maybe even with a small test ride if you kind 😜
He’s located in Paris. 
https://www.electric-skateboard.builders/t/unreasonable-e-mtb-build-me-too-i-want-to-faceplant-on-dirt-at-60km-h-and-commute-everyday-too/67726/5?u=andy87
```

---
## \#67 Posted by: boubak Posted at: 2018-10-02T16:22:50.600Z Reads: 109

```
@Andy87 : Thanks ! I just did that :) 

By the way I tried to contact @stewii to buy a dual ESCape from him, still waiting his answer since 10 days :smile:, I hope he still has stock of it.

Cheers,

Boubak
```

---
## \#68 Posted by: boubak Posted at: 2018-10-23T16:24:54.427Z Reads: 101

```
Hello everyone :slight_smile:,
 
I am not dead !

Small update :

  *  I chosen a 17 ply holypro, after severous questions/answers from @trampa, @okp, @Riako and @DanSkates : --> I asked @trampa when they will have stock again and I am waiting that
  *  Since @stewii is not responding and since I read that some of the "I-know-what-I-m-doing" guys from here received their ARC 200 for test, I will wait their conclusion and maybe take 2 ARC 200 instead of an ESCape

Kind regards,

Boubak
```

---
## \#69 Posted by: Grozniy Posted at: 2018-10-23T18:15:14.088Z Reads: 91

```
That's only 600$ of investment ;)
Bread and water for 1 month then :p
```

---
## \#70 Posted by: Andy87 Posted at: 2018-10-23T18:58:49.871Z Reads: 95

```
What he would pay for two vesc 6 from trampa... 🤔 ... 😅 ...
```

---
## \#71 Posted by: boubak Posted at: 2018-12-14T11:12:16.477Z Reads: 76

```
Hello everyone :smiley:,

I finally ordered my trampa board in 17ply (it was out of stock for the past 2 month so I had to be patient)

The story continue ! (slowly)

Kind regards,

Boubak
```

---
