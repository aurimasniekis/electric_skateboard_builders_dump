# MKV3 - Carvon 2.5v Dual 97mm &#124; VESCs &#124; 10S4P Li-ion

### Replies: 69 Views: 7835

## \#1 Posted by: makevoid Posted at: 2017-02-23T01:24:48.549Z Reads: 488

```
Here's my third build (reworked from my [first](http://www.electric-skateboard.builders/t/the-mkv-1-sensored-6374-vesc-koston-deck-lipo-6s-10a-psychotillers-enclosure/2298/) one), hub motor based, It currently has ~50 miles on it and it's very smooth to ride compared to my belt one.

- x2 VESC (Enertion and esk8.de)
- Carvon Dual v2.5
- Sulaco Enclosure from @RunPlayBack 10S4P Li-Ion - 40x 18650 Samsung INR from nkon.nl (~170 eur)
- Battery capacity monitor (coulometer) (~35 eur) [[link]](http://www.ebay.co.uk/itm/181954706863?_trksid=p2060353.m1438.l2649&ssPageName=STRK%3AMEBIDX%3AIT)
- Proto Boards anti spark w led (~46 eur) [[link]](https://www.proto-boards.com/product-page/vedder-spark-switch-assembled-kit-uk)
- 10S BMS 60A (~27 eur) [[link]](http://www.ebay.co.uk/itm/152385098820?_trksid=p2060353.m1438.l2649&ssPageName=STRK%3AMEBIDX%3AIT) - [[link2]](http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html)
- 10S 3A Charger (~30 eur) [[link]](http://www.ebay.co.uk/itm/321534203713?_trksid=p2060353.m1438.l2649&ssPageName=STRK%3AMEBIDX%3AIT)
- Koston deck
- SMTBoard controller (~38 eur) [[link]](https://www.aliexpress.com/store/product/2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/1987363_32607181070.html)

Stats (recorded from the vesc):

w/ rider weight 105kg (230lbs)
Max speed: **44 km/h** (27mph) https://metr.at/r/BxvSe - theoretical max speed 54km/h
Max range: **38km** (25 miles) - at avg speed 20km/h
Max vesc temp: 70C

[Calc](http://calc.esk8.it/#{%22batt-type-lipo%22:0,%22batt-cells%22:10,%22motor-kv%22:85,%22system-efficiency%22:80,%22motor-pulley-teeth%22:1,%22wheel-pulley-teeth%22:1,%22wheel-size%22:97}|) 

---


Replaced hubs, now running dual Carvon v2.5 hubs:

<img src="/uploads/db1493/original/3X/4/3/43022feb372ef397093a05861d3158db11dc2226.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/a/c/ac474702ad709b1346d3a775196d6e3d1fb8c3e9.jpg" width="666" height="500">



VESC ride logs:

- 1 - [A](https://metr.at/r/BxvSe), [B](https://metr.at/r/b4eBQ)


-----

START of the post

<img src="/uploads/db1493/original/3X/c/1/c1da23a3757ef11154fb107c4db7373c48ac2832.jpg" width="375" height="500">

The urethane on the hubs doesn't seem to slip, I tried them at 6S and they became really hot pretty quickly, but with the 10S they seem to stay cool, I have still to try them on a long hilly track to see if they can whitstand the load (I'm ~105kg).
Controllers (I have two of them) are super reliable, both vesc work well and seem to perform almost equally, charger/bms are good. I like the led inside the anti spark switch because not only looks cool but I sometimes forget my old board ([the MKV2](http://www.electric-skateboard.builders/t/the-mkv2-vesc-8s5p-li-ion-drop-down-deck-97mm-60a-bms/6930/7)) on, and the vesc in standby discharges the battery a bit.
The Sulaco enclosure is really massive, it could fit 60+ cells but I think with 10S4P I should be ok for now, I would like to make a 10S5P for more range and less voltage sag in the future 

I've still to route a path for the cables in the deck but I'll probably wait for the Carvon V2.5s to arrive (next week) and I plan to do a quick video comparison between jacob hubs and the carvons next month (carvons w/ 97mm flywheels).

Here are some shots of the old 6S setup, when assembling the current battery pack, power switch / coulometer details etc..

Build details:

<img src="/uploads/db1493/original/3X/9/a/9ae25267cf2e9e4b3daba89822348234de5c58ce.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/e/c/ecebc2b3e9e127198391ea1cf86bcba5498d9236.jpg" width="666" height="500">

The battery meter has good infos (voltage, percent of charge, amps remaining to be consumed) and it flashes while charging which is not bad. 


Assembling the new pack:

<img src="/uploads/db1493/original/3X/3/1/317db88883ad9984fba70043d3cdc3a104fccef5.jpg" width="666" height="500">

I'm using standard 18650 battery spacers, some copper wire soldered on the cell solder tabs (I used a 80w soldering iron)  Added some foam and taped everything together (I need some appropriate heatshrink I know) 

<img src="/uploads/db1493/original/3X/1/5/15aee62d897b6d12f3af391e4bec65b8eab43f40.jpg" width="690" height="381">

<img src="/uploads/db1493/original/3X/e/4/e45a527c3e4aae967d2e97770fb17a5ad808af0e.jpg" width="690" height="388">
```

---
## \#2 Posted by: benwong Posted at: 2017-02-23T02:33:31.978Z Reads: 370

```
nice works~~ i like the meter, i planning to use this meter too, but still figuring how to mount on top the deck instead at the bottom. Because can directly see meter while riding~~

Did you have wiring diagram of the meter?
```

---
## \#3 Posted by: makevoid Posted at: 2017-02-23T08:58:51.544Z Reads: 368

```
Thanks, yes, that thing is awesome, seems so precise, I used the diagram found here in this post

http://www.electric-skateboard.builders/t/installed-and-tested-a-coulometer-fuel-gauge/1753/5?u=makevoid

I have the 50A version and there is only the positive wire to connect to, the negative is taken from the amp "sensor" directly

**Video:**

https://youtu.be/eDmxK_z0aQ0
```

---
## \#4 Posted by: benwong Posted at: 2017-02-23T10:09:33.390Z Reads: 340

```
<img src="/uploads/db1493/original/3X/e/f/efb5b60f2d4bf5e4c750d371f2e0a379a9278ba7.jpg" width="690" height="271">

This diagram is base on my understanding. 
sensor have a B+ port, i not need link to which side (AorB). 

You meter will light up when charging?
Becoz i wish to see the battery level while charging. 

Beside using coulometer, anyone know how to wiring a meter to show battery level when charging?
```

---
## \#5 Posted by: makevoid Posted at: 2017-02-23T10:49:27.756Z Reads: 319

```
<img src="/uploads/db1493/original/3X/0/e/0e30e5818fd43f800333d9669354aff265e4d670.jpg" width="690" height="384">

here's my diagram, as I don't have the 350A version but the 50A the layout is a bit different

everything goes before the anti spark so it can track the battery status when charging

the plus coming out from the battery meter goes on the + line

the minus need to pass from the sensor, the meter will get current from the meter itself (there are 3 cables that go to the sensor, 2 of them are black ^^)

hope that helps
```

---
## \#6 Posted by: benwong Posted at: 2017-02-23T10:51:46.907Z Reads: 286

```
okay, so as my diagram, i should using A link. but the meter will always turn on event i dint charge or use? 
or i need connect between bms and lipo?
```

---
## \#7 Posted by: makevoid Posted at: 2017-02-23T11:41:21.097Z Reads: 288

```
Yes I have an additional switch on the cable marked as + but I didn't expose it outside the enclosure. I guess that the consumption is minimal because the lcd backlight goes off (standby) until you start charging the battery or press a button.
I will probably switch it off only when I don't plan to use the board for long periods
```

---
## \#8 Posted by: makevoid Posted at: 2017-02-25T03:12:16.549Z Reads: 301

```
more pics of the second board, I needed to change deck because I cracked it failing to get over a small step lol, it's a cheap deck but it works ([yocaher drop down](https://www.yocaher.com/product/punked-drop-down-yinyang-longboard-deck) I got from amazon uk)
It flexes a bit on the drop which is nice even if it's 9ply. I have ridden it a lot so for what it costs I was more than fine with the idea to get a new one.

I would like to try another drop down deck, probably I will get the[gravity tequila sunrise](https://www.muirskate.com/longboard/decks/69894/gravity-big-kick-longboard-skateboard-deck-w-grip) soon. 
If someone knows of any similar/good drop down decks with a very big wheelbase (33"+) please tell me ^^


enough with the words

here's a photo update!

cracked deck lol (mkv2):

<img src="/uploads/db1493/original/3X/6/e/6e508f56daeecfda835271e4f707f0d8d40b5db3.jpg" width="375" height="500">

new setup for my previous board:

<img src="/uploads/db1493/original/3X/2/d/2d7c73baef799cc17ba7f07c4f0da80af8cb0cf0.jpg" width="375" height="500">


here they are, the two builds side by side:

<img src="/uploads/db1493/original/3X/b/1/b1dcbf7b4c5c1b3e49f20a1892d0b73ec9cc78c8.jpg" width="375" height="500">

mkv3's (dirty) top - old mkv2 enclosure will have holes for the cables for the top motor as well, this time (because I have a second working build) I will manage the cables a bit better :D

<img src="/uploads/db1493/original/3X/3/e/3e6ac5ace6cf96fcf640a3f8ab916ef72e5eeb31.jpg" width="375" height="500">


10S 3A li-ion chargers [edit]
```

---
## \#9 Posted by: makevoid Posted at: 2017-02-25T16:37:30.507Z Reads: 285

```
I went for a ride today, 6 miles total, hubs handled very steep and long hills better than my single 6374 build (1 motor caused the vesc to overheat, with 2 vesc and these guys it seems fine, I still have to check the vesc temp to confirm this though...). braking was very good, the only downside is that where I live the roads/pavements are really not good, thus the thin urethane that covers the 90mm motorized wheels is not enough to dampen vibrations, I will try to get softer risers to see if that's better.   

Pushing is still a bit hard (I'd say at par as a single motor) because the magnet inside the motor make some resistance while pushing, I'm curious about this aspect with other hub motors, I tried an  inboard and it was very smooth, but hopefully I won't need to push much because the board will work 100% of the rides and I will never finish the battery, right? ^^

I was able to finish the ride but near home I noticed a thing...

here are some pics:

<img src="/uploads/db1493/original/3X/3/2/32ac79582e431989b8743a878d47d9e93928c7c9.jpg" width="666" height="500">

I noticed one motor vibrating a lot, the grub screw came loose and it rotated a bit


<img src="/uploads/db1493/original/3X/4/7/47175876ee9c00331fc2bdeef9d23a18a0f3fc54.jpg" width="375" height="500">

the cables were shorting a bit, I re-insulated them, tightened the grub screw and put a lot of thread locker this time, hopefully it will stay

<img src="/uploads/db1493/original/3X/4/1/41932d7e4756437aa01a7f9b44f724914b10a306.jpg" width="375" height="500">
```

---
## \#10 Posted by: makevoid Posted at: 2017-03-02T00:57:23.426Z Reads: 274

```
the hub stays, I had slightly slipping urethane  on one wheel which I think I can fix with some double sided strong tape and/or some glue. Today Carvon(s) V2.5 arrived and I decided to try them while I fix the others (actually this made me think of starting a third build even if I think that I will probably make it and then sell another one because I don't think I can have 3 or my wife will kill me lol).

will glue/tape these soon:

<img src="/uploads/db1493/original/3X/4/2/42bac2f4e6db38cda82e2054e858e8def9b03681.jpg" width="375" height="500">

dual carvon v2.5 mounted, detected ok, will try them in BLDC soon:

<img src="/uploads/db1493/original/3X/4/3/43022feb372ef397093a05861d3158db11dc2226.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/a/c/ac474702ad709b1346d3a775196d6e3d1fb8c3e9.jpg" width="666" height="500">


dual vescs + lcd consume 2w in standby

<img src="/uploads/db1493/original/3X/b/1/b13339bc500bc1272d512504db9f87e9cbe9727d.jpg" width="375" height="500">


The other build (dual 6374) has really a lot of power, I want to try that soon as well, looking forward to the w/e, hopefully I can make a short video too!
```

---
## \#11 Posted by: Eboostin Posted at: 2017-03-02T14:57:12.139Z Reads: 239

```
Have you tried the chargers yet? It says the output voltage is 16.8v. 

Everything else is looking good!
```

---
## \#12 Posted by: makevoid Posted at: 2017-03-02T15:14:23.412Z Reads: 242

```
loll, I posted the wrong pic! They sent me the wrong ones I actually sent those back and they replaced them very quickly, that was the pic I used as proof for them, the new chargers are 3A 42V, also I have [this charger](http://www.ebay.co.uk/itm/161782114198?_trksid=p2057872.m2749.l2649&var=460755871237&ssPageName=STRK%3AMEBIDX%3AIT) which is nice because it charges very slowly at 41.2v (95%) charge which should increase the battery life a bit.
```

---
## \#13 Posted by: Eboostin Posted at: 2017-03-03T00:10:09.381Z Reads: 245

```
Good to hear! 

Does the second charger (that charges at 41.2v) stop at 41.2 or does it go all the way to 42?
```

---
## \#14 Posted by: makevoid Posted at: 2017-03-03T07:34:12.528Z Reads: 250

```
It stops at 41.2v, ~95%, it charges the battery very slowly (36w vs 130w of the 3A charger) so I usually leave it overnight. That should help increasing battery life too
```

---
## \#15 Posted by: makevoid Posted at: 2017-03-24T09:59:45.947Z Reads: 246

```
I wanted to make a video, I haven't used the gimbal in a long time, I was a bit sleepy and this happened lol :)

https://youtu.be/eDmxK_z0aQ0

The gimbal was a bit broken already (my wife and his boss used it improperly) so I hope I can get a new one soon next month to make a full video of my usual ride (25m one way)

here's the ride log (data from 1 vesc)

https://metr.at/r/CoFQt
```

---
## \#16 Posted by: wmj259 Posted at: 2017-03-24T18:40:59.073Z Reads: 223

```
What app did you get that data from, it's really nice
```

---
## \#17 Posted by: OskarCastrone Posted at: 2017-03-24T19:00:25.365Z Reads: 227

```
@makevoid I would like to know which app you used as well! You mist have it connected to your VESC with bluetooth?
```

---
## \#18 Posted by: Maxid Posted at: 2017-03-24T19:06:36.913Z Reads: 229

```
http://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483
```

---
## \#19 Posted by: noazark Posted at: 2017-03-24T20:35:56.468Z Reads: 224

```
How long did  it take for you to get your v2.5's? @makevoid
```

---
## \#20 Posted by: makevoid Posted at: 2017-03-24T21:12:57.271Z Reads: 225

```
not too much, they were worth the wait ;)
```

---
## \#21 Posted by: makevoid Posted at: 2017-04-02T22:31:54.257Z Reads: 222

```
latest (logged) rides:

- first
https://metr.at/r/Og8rS
https://metr.at/r/svOJh

https://metr.at/r/Og8rS

---

https://metr.at/r/svOJh

---

---

---

- second
https://metr.at/r/L8E60 
https://metr.at/r/TbGB2

https://metr.at/r/L8E60

---

https://metr.at/r/TbGB2
```

---
## \#22 Posted by: rpasichnyk Posted at: 2017-04-05T16:38:36.593Z Reads: 191

```
I have CarvON v2 dual and it's interesting to compare our data

https://metr.at/r/sc9Np

and return trip

https://metr.at/r/2aXho

I went a little bit faster, but still I'm far away from using the full potential of v2. At 50% duty cycle it gets too scary. I wish I had v2.5, but they didn't exist back then. Still, I'm happy because I bought v2 for $399. On your v2.5 you have 84% duty cycle (there's still room to grow) and I imagine much better torque!:+1:
```

---
## \#23 Posted by: makevoid Posted at: 2017-04-05T17:43:58.354Z Reads: 177

```
on here I reach 95% (44kmh) 

https://metr.at/r/BxvSe

but I forgot to enable location tracking  so no map :/
```

---
## \#24 Posted by: rpasichnyk Posted at: 2017-04-05T19:15:34.364Z Reads: 166

```
Maybe it's even better that you forgot, police could check this forum and find you next time :sweat_smile: If you feel like you may want more speed at some point you can still go 12S with these motors
```

---
## \#25 Posted by: makevoid Posted at: 2017-04-05T19:52:54.399Z Reads: 188

```
I am fine with the speed, I think 40km/h is already enough for me at the moment,  I'm not sure I can handle that speed for a sustained amount of time w/o crashing, that's why I am looking forward to [this thread](https://www.electric-skateboard.builders/t/riding-tipps-introduction-to-high-speed-skating/19006) and other similar tips. btw I tried the video overlay generator and I have few comments about it, I'll write them on the other post

edit: latest ride logs

https://metr.at/r/S3q8x

---

---

---

https://metr.at/r/5DrjO


---

https://metr.at/r/HFWFk
```

---
## \#26 Posted by: makevoid Posted at: 2017-04-21T23:46:00.742Z Reads: 183

```
Tried FOC today, overall it felt very good, super smooth acceleration, here's the log:


https://metr.at/r/IcoKh 


This is the first time I try it on dual and on hubs. I tried foc in the past with a single sensored and it was super good but I've never played with its settings much. On this one I seem to have a small intermittent issue with one of the two motors stuttering a bit when accelerating and braking hard.This issue at the motor (maybe phase wires, internal or probably related to the vesc) doesn't affects BLDC and only a little bit FOC (it's totally ridable as you can see) and I'll probably spend some time and recheck everything soon: connections, VESC and motor wires, but for now I'll just try to change the vesc settings and ride :D. 


That's how I configured the vescs - 2 attempts: first:
Detection succeeded smoothly, I tried to start the board from a stop with the default value of Observer gain (13.46) but I felt that it wasn't very good, I used light stuttering of the motor as a test factor. 
Second attempt, changed 1 value): I looked at the forum but then checked jacobbloy 's  instructions for the VESC configuration in foc. On those there's a suggestion by Ben to set Observer gain to 100. The board started much nicely with that. I checked the forum and I guess that I should try to up the motor max amps a bit because it feels a bit low for FOC (60A currenly)

I will switch from 60A to 75A/80A motor max and add 5A to brakes (motor min) as well, I'm also curious to try crazy values like 110A motor max because as I'll probably never reach them and they should help against the current acceleration curve - I would like to try Ackmaniac's firmware too soon so I can delegate this "fix" to the watt control mode instead of just brutally changing the max motor amp.
I would like to have more acceleration for starting quickly from a stop (after a push ofc),  I missed that a bit on my first ride (good feature to have in urban environments), I believe that if the hubs were sensored this was not a problem.


Also I would like to change other foc related values (the one located in "FOC - General", "FOC - Sensorless Startup" for example to improve the situation)

I also lowered the cutoffs which were pretty conservatives (32/30) to 30V start 28V even if I always fully charge my board before riding but this should prevent any cutoffs

Overall I can see/feel straight away that the acceleration is super smooth, hubs are silent, energy consumption seems less but I don't know how much.
You can see from the log that I had a problem when testing hard braking on this one at 10:47 - https://metr.at/r/IcoKh - there's a spike down during the deceleration even if I wasn't braking 100%. 

btw I love foc for now, hopefully I will have a video up soon, oops I wrote too much ^^
```

---
## \#27 Posted by: makevoid Posted at: 2017-04-22T23:55:30.060Z Reads: 174

```
Video (new gimbal zhyiun z1-pround and good old yi camera) with metr.at logging overlay (w/ some css changes made by me ^^)

https://youtu.be/IJpQjbWci8I

I will try to continue the ride from where I stopped (SD Card was full :/) and film the way back too. Probably I'll switch back to BLDC to show the difference between the two.I plan to record a video for each of my usual rides as if they were commutes ( ~1h total / ~6km each way )


https://metr.at/r/RoEn9

metr.at vesc (foc) log: https://metr.at/r/RoEn9 (9:48 - 9:55) - (+ [ride back](https://metr.at/r/EZgA7))
```

---
## \#28 Posted by: rpasichnyk Posted at: 2017-04-25T17:38:21.118Z Reads: 167

```
that scary moment on the video at 3:04 :sweat_smile:
```

---
## \#29 Posted by: makevoid Posted at: 2017-04-29T14:04:27.337Z Reads: 175

```
Small review of nano x:

- strong signal (damn, I was impressed by that, much better signal than the mini remote which it was really very good, I couln't notice any signal drops, probably it uses a frequency that doesn't clash with speed cameras or it's just stronger, really nice job)
- very compact (for guys with big hands like me it's probably too compact, I have to operate the thumb throttle with the middle of my thumb) 
- simple but strange binding procedure, I'm not sure why but had to wait a bit (few minutes) before it could bind successfully but then it's good

pics:

<img src="/uploads/db1493/original/3X/7/9/79fa6121d66d0d5e3fa578acb99321596aad8dc8.jpg" width="595" height="500">

<img src="/uploads/db1493/original/3X/0/0/00047771f2ff6d0155177351f74685577703e2ef.jpg" width="623" height="500">


It will be my default remote from now

because it's a thumb controller it's less sensitive so I've reduced my motor max from 60A to 50A and motor min from -32A to -27A to be able to control better acceleration and braking

edit: new ride log, much smoother with the new settings

https://metr.at/r/0z24u
```

---
## \#30 Posted by: makevoid Posted at: 2017-04-29T20:46:56.657Z Reads: 173

```
New Video! 

https://youtu.be/yz2Naxn15VI

@rpasichnyk I think the magic number for making the overlay match the video is 0.952 - probably you can change the js that produces the video and set its speed?
I am setting the speed after importing it into the video editing software (premiere, fcx, imovie, shotcut, avidemux, kdenlive, openshot) at 95.2% and this time I think the sync is perfect trougought the video < 1 sec difference between the log and the video I think, I'll test if it's 0.952 for the next video as well - btw thank you for the zoom feature on the logs, very helpful

edit: 

I had set 60A total (my battery is 10s4p li-ion with samsung 25r 's) and had a fuse of only 40A - fuses can blow at a bit lower or higher amps / time deltas if they're not good fuses - I will take a 60A fuse in the future but for now I want to stay a bit lower than 60A, I don't think I need 60A on a cruiser board lol

I got a 50A fuse and I'll try to set 25A per VESC
```

---
## \#31 Posted by: NAF Posted at: 2017-04-29T22:28:34.890Z Reads: 161

```
I want to try FOC with my Carvon 2.5 single hub. BLDC is loud as hell. Louder than belt drives.
```

---
## \#32 Posted by: makevoid Posted at: 2017-04-29T23:05:46.088Z Reads: 163

```
at what voltage are you running the carvon v2.5? also how much do you weigh? hills / crazy speeds or chill riding?

if I were you and had the possibility I would attempt changing to foc, the motor actually supports it if it's not damaged (one of the two that I have has been slightly damaged [damn rock! :D] it doesn't runs perfectly on foc, it stutters a bit at high amps but still runs more than fine for my usage) 

I believe that if you monitor the vesc temp and currents via a bluetooth app like gpxlBen/@evoheyax - @rpasichnyk one or @Ackmaniac 's (which uses the least expensive bluetooth module) you can prevent the vesc from failing. 

I guess that if you monitor values like input (batt) amps and vesc temp and make sure they stay on acceptable limits while you test-ride it ... probably foc will work stable after that

Also follow jacob's / vedder advice and put observer gain at 100 after the foc setup/detection, it works much better than the default (13.6 or something)
```

---
## \#33 Posted by: NAF Posted at: 2017-04-29T23:08:54.496Z Reads: 165

```
@Titoxd10001 helped me setting up my vesc.  This is what I currently have:

<img src="/uploads/db1493/original/3X/f/7/f73b6828ce0ad30c5f3f2cc1f5b63cb565671895.JPG" width="666" height="500">
```

---
## \#34 Posted by: makevoid Posted at: 2017-04-29T23:20:52.565Z Reads: 164

```
Here's Jacob's instructions (he printed and included them in the package of his hubs) for setting up FOC, there are also [some](https://www.youtube.com/watch?v=bYYNbxPXNEU) foc [setup](https://www.youtube.com/watch?v=sFdEmyUDQxU) [videos](https://www.youtube.com/watch?v=xSCEFK7Zljw)

<img src="/uploads/db1493/original/3X/d/f/df664c439da5c625266704ecb3cf725ac956b4bd.jpg" width="334" height="500">

If you have a backup vesc or if your vesc has some kind of warranty than those are probably the best ways to try foc :D
```

---
## \#35 Posted by: NAF Posted at: 2017-04-29T23:24:49.253Z Reads: 148

```
I am using @goaxle vesc. They went the same way as chaka when it comes to upgrading their vesc's. I think most problems with FOC was with 12s setups. My battery is 10s4p.
```

---
## \#36 Posted by: makevoid Posted at: 2017-04-29T23:26:26.123Z Reads: 147

```
how much do you weigh? any long / steep hills during your usual ride?

edit: [Vlad](https://www.electric-skateboard.builders/t/axle-vesc-thread/9240/242) and [MasterCho]( https://www.electric-skateboard.builders/t/axle-vesc-thread/9240/277?u=makevoid) seem to have no issues... maybe you can try it? my suggestion is make sure it starts with a gentle push and accelerating slightly - then test breaks lightly then test accelerating harder and breaking harder in steps - go easy with your first test ride don't go on supersteep hills or at max speed straight away :D
```

---
## \#37 Posted by: NAF Posted at: 2017-04-29T23:28:45.622Z Reads: 144

```
I weight around 75kg. But I have a small backpack always with me. with some gear. not super heavy tho. ..right now with BLDC when I get proper momentum I am riding some hills without any issue.
```

---
## \#38 Posted by: makevoid Posted at: 2017-04-29T23:35:38.690Z Reads: 145

```
you're light, I think that a single 2.5 @ 10s will be enough to drive you around, foc has less acceleration right when you start but when you're over 10km/h you will get more torque than bldc I believe! also acceleration will be smooth than on bldc, but I guess you'll get less top speed (which at least for me is totally fine)
```

---
## \#39 Posted by: NAF Posted at: 2017-04-29T23:41:14.559Z Reads: 143

```
I already have speed limit for around 22mph for riding the city. If I remember correctly Jerry was riding his Single Hub 2.5 at max 28mph.
```

---
## \#40 Posted by: makevoid Posted at: 2017-04-29T23:46:49.745Z Reads: 150

```
top seed on flat should be the same for single and dual, on 10S I get [44km/h](https://www.electric-skateboard.builders/t/mkv3-carvon-2-5v-dual-vescs-10s4p-li-ion/18119/23?u=makevoid) which are ~27mph with BLDC, on FOC my current  max is [39kmh](https://www.electric-skateboard.builders/t/mkv3-carvon-2-5v-dual-vescs-10s4p-li-ion/18119/27?u=makevoid) (~24mph) but I guess I can push it further
```

---
## \#41 Posted by: NAF Posted at: 2017-04-29T23:48:00.109Z Reads: 150

```
24mph in FOC would be perfect me. Good to know that. I'll try FOC settings this week . I'll let you know how it goes.
```

---
## \#42 Posted by: makevoid Posted at: 2017-04-30T19:57:52.593Z Reads: 163

```
New video! 

https://youtu.be/muWsFzVgHRE

Ride log:


https://metr.at/r/y4PsS


On this one I blew the fuse, duh, I had set 30A as my max input current per vesc because my battery can stand it but it was too much for my fuse (rated 40A) so I had to finish the ride/video there - I set 25A per vesc now and put a 50A fuse now :)

edit: the reported current in the log overlays is for 1 vesc only
```

---
## \#43 Posted by: sismeiro Posted at: 2017-05-01T13:19:09.545Z Reads: 147

```
I see that you are not afraid of losing balance and send your longboard to the water channel. :slight_smile:
```

---
## \#44 Posted by: makevoid Posted at: 2017-05-01T13:42:06.052Z Reads: 159

```
I dreamt about it once though lol, also that I let a guy try my board and he ran away with it / on it ^^ hope they're not premonitions

edit: also I did that part of the commute for 3-4 months last year because I was working near whitechapel
```

---
## \#45 Posted by: makevoid Posted at: 2017-05-07T09:21:07.690Z Reads: 156

```
new weekend, new video:

https://youtu.be/kwkgLR-XJFQ

log:

https://metr.at/r/08vJN
```

---
## \#46 Posted by: Eboostin Posted at: 2017-05-07T17:24:36.810Z Reads: 146

```
He tried to steal your board??!
```

---
## \#47 Posted by: makevoid Posted at: 2017-05-07T19:46:23.690Z Reads: 148

```
it was just a dream ^^, but yes I'm a bit afraid of letting people I don't know try my board in general because if they know how to ride a longboard and they run away, for sure I will not be able catch them :) probably a feature to implement on the vesc firmware or on a bluetooth connected app would be a timed or remote kill/switch that makes the board slow down and stop after a cerain time after activating such a mode or if you press a button on your phone... maybe it's just me being too paranoid lol
```

---
## \#48 Posted by: Michael319 Posted at: 2017-05-08T05:30:19.702Z Reads: 143

```
@makevoid @naf just letting you guys know, I run a single 2.5 on 12s2p on foc, and I usually hit 32-34 mph, max I hit was 38 (slight downhill). I have yet to change observer gain, does, what exactly does it change?
```

---
## \#49 Posted by: makevoid Posted at: 2017-05-08T06:20:07.203Z Reads: 142

```
I'm not totally sure but it should help with the startup.  After changing it from ~13 to 100 I noticed a smoother start and I could start on flat without pushing.
```

---
## \#50 Posted by: rpasichnyk Posted at: 2017-05-08T15:38:54.559Z Reads: 140

```
There is a time in the bottom-right corner of the video, is it added by camera, overlay or Premiere? I noticed that it is one hour earlier than JSON time :nerd: and I wonder why?
```

---
## \#51 Posted by: makevoid Posted at: 2017-05-08T19:14:53.776Z Reads: 138

```
camera :) way easier to sync the video with the timestamp on both :D

edit: I've seen your released a fix on the new version, I'll try it next weekend probably, many thanks!

Edit2: today's ride (a bit rainy so no video)

https://metr.at/r/tT7fb

Also another update: the nano x conflicts with speed cameras frequencies here in London, Uk (losing signal a little bit when you are nearby them) a bit like the other remotes, when the nanox x battery is not fully charged, I noticed no signal loss at all when charged


edit2: also the nano x has a problem I haven't noticed, it breaks very hard unless you press back and forth on the throttle of the remote before powering the board - more infos here: https://www.electric-skateboard.builders/t/abrupt-brakes-new-vesc-x-enertion-solved/23896/ (btw thanks to the guys for finding the solution! much better now)
```

---
## \#52 Posted by: Eboosted Posted at: 2017-05-22T05:06:28.256Z Reads: 118

```
Hey man, great videos!

I love the stabilizationm, what stabilizer do you use?

The last video is far better than the previous ones, since you can see more forward

Your front foot makes me feel uneasy, as it's placed vertically instead of horizontaly, you are steering the board with the back foot and there is not much control on emergency situations, aren't you getting too much strain on the back calf after a short run?
```

---
## \#53 Posted by: makevoid Posted at: 2017-05-22T05:39:44.697Z Reads: 113

```
Zhiyun-1 Pround, yes I got an extension stick which is not perfect but it works, videos are better with it. About the feet well, I am no experienced skater/lb but I did snowboard for quite some time. I started by placing feet almost parallel (snowboard-like position), while that is great for carving at higher speed I found more comfortable to have my front foot (in the w-concave pocket) and more angled towards the direction of travel. This gives me the possibility of putting most of my weight forward on the front foot and actually is putting the weight forward-left or forward-right and crouching a bit that lets me steer, the back foot does almost nothing other than pushing me a bit forward maintaining contact with the deck (useful for sudden braking, accelerating while turning etc). It's not a tuck position but I think the concept is similar, I agree that being with my weight all in front is straining if the road is rough (btw 97mm wheels help), I try to use a different stance for bumpy roads with my feet almost parallel and away from the trucks so that the deck absorbs some vibrations. What's your riding style?
```

---
## \#54 Posted by: Eboosted Posted at: 2017-05-22T05:55:46.493Z Reads: 117

```
At my firsts e-board ridings I used to place the front foot like you, but after more riding I started to realize this foot placement is way better for control, easier on both calfs and you feel safer on tight turns, however you need to get used to it, just give it sometime and soon you should realize what I'm talking about

<img src="/uploads/db1493/original/3X/b/f/bf7a9b8291567995fa7b07de8790c31d8a556282.png" width="690" height="427">

BTW here is a video of me riding in Lima, I would like to make a stabilized video from the perspective of yours with the extension stick.

I just mounted the GoPro on my belt:

https://www.youtube.com/watch?v=X7zmeHiXfuo&
```

---
## \#55 Posted by: makevoid Posted at: 2017-05-22T19:39:10.401Z Reads: 105

```
Very nice ride, I'm more conservative as rider than you, especially when filming. Also your board seems to have a very powerful acceleration, dual belt drive right? Cool.
```

---
## \#56 Posted by: Tuomalar Posted at: 2017-05-22T19:52:42.234Z Reads: 109

```
Differences at road manners are huge. There's no way i could ride like that in traffic where i live. Everyone just panic when they see me because they don't know what to do and skaters are here well known as hooligans :D
```

---
## \#57 Posted by: Eboosted Posted at: 2017-05-22T20:03:02.934Z Reads: 111

```
Yes. It's dual belt drive with 6355 190kv motors.

The acceleration is amazing, however I want more, so I'm building a Trampa with dual 6374 190kv for 40% more power and I'll upgrade to 12S
```

---
## \#58 Posted by: NAF Posted at: 2017-07-04T06:29:30.241Z Reads: 101

```
@makevoid  What MOTOR MAX value do you think would be optimal for Carvon Single v2.5 85kv ?? Do you think I could go with 80a ???  My battery max is 60a as the BMS is 60a.
```

---
## \#59 Posted by: makevoid Posted at: 2017-07-04T06:58:06.629Z Reads: 97

```
Is your battery 10S too? Try with 50 or 60A first and then add another 10A, do a test ride and see if you need to add more, repeat. I won't go over 80A w carvons 2.5 probably. With the new vesc tool you can set the throttle curve and I think BV suggests to have the same value of input current, motor max and min and adjust the acceleration via the throttle curve if you want to increase it (new vesc tool or ackmaniac s firmware w/ watt control mode). So 60A / -60A motor max/min, 60A input current in theory. Anyway I never tried more than 50A input current at 10S so maybe start with 50A ;)
```

---
## \#60 Posted by: NAF Posted at: 2017-07-04T07:15:08.117Z Reads: 101

```
Yes the battery is 10s 60a with NO FUSE - I am using Extended BLDC TOOL aswell. this what I currently have:
<img src="/uploads/db1493/original/3X/8/d/8d1614d3af57d6666f710a55f8da4eb7dd5987bd.png" width="690" height="360">
```

---
## \#61 Posted by: makevoid Posted at: 2017-07-04T07:17:44.108Z Reads: 93

```
Then probably the best is to leave this settings, use watt control mode and adjust the throttle curve if you need more acceleration
```

---
## \#62 Posted by: NAF Posted at: 2017-11-06T09:39:38.507Z Reads: 78

```
@makevoid Do you have any uphill videos with these dual v2.5 ? Since Carvon is going to realease their v4 XL motor based on 6374 85kv v2.5 I thought I'll ask you about your experience with hills and torque ?
```

---
## \#63 Posted by: makevoid Posted at: 2017-11-06T23:47:46.562Z Reads: 86

```
these two are probably not bad:

---

long hill 
https://youtu.be/kwkgLR-XJFQ?t=7m27s
https://www.google.co.uk/maps/@51.513191,0.0015648,3a,75y,48.68h,79.58t/am=t/data=!3m6!1e1!3m4!1s5XyhOI9aqSLlqR9HBQ6AFg!2e0!7i13312!8i6656?hl=en
you can see it peaks at 1600w (10s battery) to keep me at around 30kmh uphill 

short but steep hill 
https://youtu.be/IJpQjbWci8I?t=1m38s
https://www.google.co.uk/maps/@51.5106332,-0.0395717,3a,75y,6.19h,69.95t/data=!3m9!1e1!3m7!1sa23A_waFAp3-9r78GEGbBg!2e0!7i13312!8i6656!9m2!1b1!2i23?hl=en
climb no problem

----

i'm 110kg so definately the v2.5 have good enough torque for pretty much anything you can find in the cities I think
```

---
## \#64 Posted by: Fecm93 Posted at: 2017-11-27T17:47:38.772Z Reads: 75

```
@makevoid Hi! I'm wondering if you could help me out with a doubt. 
I'm running carvon dual V 2.5 with Space Cell pro 3 and the nano X. 
My ride is really great but I'm looking to switch to FOC for a smoother ride. Nevertheless, when I make the motor detection only one motor spins. I have multiple ESC over can enable, should I make the motor detection on both VESCs separately first?
```

---
## \#65 Posted by: rpasichnyk Posted at: 2017-11-28T21:22:29.670Z Reads: 70

```
Yes you need to make motor detection separately.
```

---
## \#66 Posted by: makevoid Posted at: 2017-11-28T21:43:46.523Z Reads: 69

```
Yes you should do detection separately as @rpasichnyk suggests .

I don't run them on FOC anymore because I damaged one slightly (a rock probably) and it's stuttering a bit on FOC (I guess it's about detecting the rotor position of the damaged motor). I am using a Y split cable without connecting the + on one end, I didn't try with canbus yet. I remember I read on this forum that is better to disable traction control on hubs even if I can't think about why. Definitely change the observer gain to be around 60-100 as Jacob/Vedder suggest (I used 100), I found that changes everything compared to the default value.
```

---
## \#67 Posted by: Fecm93 Posted at: 2017-11-29T21:01:32.209Z Reads: 64

```
@rpasichnyk @makevoid thank you very much!!
```

---
## \#68 Posted by: Eboosted Posted at: 2017-12-04T02:52:31.624Z Reads: 62

```
[quote="makevoid, post:66, topic:18119"]
Definitely change the observer gain to be around 60-100 as Jacob/Vedder suggest (I used 100), I found that changes everything compared to the default value.
[/quote]

Would you mind explaining what does observer gain really does? Is this value only valid for hub motors?
```

---
## \#69 Posted by: makevoid Posted at: 2017-12-10T02:07:27.744Z Reads: 54

```
I really don't know, I just received Jacob hubs with some instructions where he states that Ben Vedder recommends that ( see 
http://www.electric-skateboard.builders/t/mkv3-carvon-2-5v-dual-97mm-vescs-10s4p-li-ion/18119/34?u=makevoid ), I don't know the reason and I never tried to play with the values but 100 was much better than the default value for both Jacob and Carvon 2.5 hubs
```

---
