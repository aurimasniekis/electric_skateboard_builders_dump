# Vedder Anti-Spark switches for sale (from 18€)

### Replies: 201 Views: 13793

## \#1 Posted by: eLDoska Posted at: 2017-08-30T12:01:48.282Z Reads: 1139

```
<img src="/uploads/db1493/original/3X/f/5/f55b4305cd81bf2f1a1a55800fd144f592fc6aac.jpg" width="666" height="500">

- ready to use Switch (with XT60 or XT90; 40A fuse; heat shrink tube; 10AWG wire; on/off switch) - **25€ / 30$ + shipping**
- PCB with soldered SMD components - **18€ / 21.5$ + shipping**
- other option / bulk price - PM me

shipping to EU/USA ~ **5€**

the components that are used:
https://github.com/vedderb/SparkSwitch/blob/master/SparkSwitch_BOM.ods
```

---
## \#2 Posted by: karosass1 Posted at: 2017-08-30T12:26:50.148Z Reads: 917

```
Where are you shipping from?
```

---
## \#3 Posted by: eLDoska Posted at: 2017-08-30T12:30:47.572Z Reads: 897

```
from Russia
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-08-30T12:34:28.757Z Reads: 887

```
What FETS are you using?
```

---
## \#5 Posted by: eLDoska Posted at: 2017-08-30T12:39:36.712Z Reads: 875

```
all components are from Vedders BOM (IRFS7530TRL7PP)
https://github.com/vedderb/SparkSwitch
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-08-30T12:54:57.785Z Reads: 830

```
gotcha. just FYI these are solid at 10S but at 12S they will give you issues unless you upgrade the FETs.
```

---
## \#7 Posted by: eLDoska Posted at: 2017-08-30T13:21:01.009Z Reads: 798

```
thanks for info. for 12s users I can change IRFS7530 to IRFS7730 for free :)
```

---
## \#8 Posted by: longhairedboy Posted at: 2017-08-30T13:23:46.296Z Reads: 781

```
are you building these by hand? If so, that's a nice upgrade to do on request, but the price difference on bulk orders may not be worth it to keep doing the 60v ones once you run out.
```

---
## \#9 Posted by: eLDoska Posted at: 2017-08-30T13:40:47.275Z Reads: 743

```
yes, I build this by hand (air flow soldering station + heated bed)
```

---
## \#10 Posted by: Garlz Posted at: 2017-11-06T20:11:11.466Z Reads: 694

```
Are you still making these to sell?
```

---
## \#11 Posted by: eLDoska Posted at: 2017-11-06T22:00:41.698Z Reads: 684

```
yes. 

10char
```

---
## \#12 Posted by: GhettoFab.rictation Posted at: 2017-11-07T20:34:19.113Z Reads: 660

```
Hey guys if you rate the mosfet for 14s will the switch run on 12s better or cooler? Or will it limit current
```

---
## \#13 Posted by: eLDoska Posted at: 2017-11-08T10:43:46.554Z Reads: 657

```
[quote="GhettoFab.rictation, post:12, topic:31847"]
if you rate the mosfet for 14s will the switch run on 12s better or cooler
[/quote]
better - maybe. 
cooler - no. switch with IRFS7530 will be cooler that IRFS7730 at the same current.
```

---
## \#14 Posted by: GhettoFab.rictation Posted at: 2017-11-08T11:34:32.987Z Reads: 658

```
[quote="eLDoska, post:13, topic:31847"]
switch with IRFS7530 will be cooler that IRFS7730 at the same current
[/quote]
 What do you mean, so what I'm saying is I have 12s and want to upgrade to 14s in the future can I make one switch for both
```

---
## \#15 Posted by: egzplicit Posted at: 2017-11-08T11:41:34.497Z Reads: 616

```
Does anyone know if the fuse blows if you pull 50A or 60A for short periods (5-10 secs)?
```

---
## \#16 Posted by: eLDoska Posted at: 2017-11-08T13:09:29.024Z Reads: 613

```
[quote="GhettoFab.rictation, post:14, topic:31847"]
can I make one switch for both
[/quote]
yes, you can.
```

---
## \#17 Posted by: eLDoska Posted at: 2017-11-08T14:10:11.744Z Reads: 628

```
[quote="egzplicit, post:15, topic:31847, full:true"]
Does anyone know if the fuse blows if you pull 50A or 60A for short periods (5-10 secs)?
[/quote]

<img src="/uploads/db1493/original/3X/3/b/3b88b9d93b338b6fd29f6d982770b41f49ed4464.jpg" width="282" height="163">
```

---
## \#18 Posted by: egzplicit Posted at: 2017-11-08T14:24:17.783Z Reads: 606

```
Thanks @eLDoska that is really helpful. So you could pull 54A continuously for 30 minutes, that's a very long time. I think I'll increase min per vesc to 25A.. that should give me 50A in total and that only for a few seconds when accelerating hard.
```

---
## \#19 Posted by: GhettoFab.rictation Posted at: 2017-11-09T11:34:12.811Z Reads: 592

```
What do you mean by this?
```

---
## \#20 Posted by: 702vegas Posted at: 2017-11-10T00:57:38.019Z Reads: 576

```
can i change the switch?
```

---
## \#21 Posted by: JdogAwesome Posted at: 2017-11-10T02:58:33.889Z Reads: 535

```
What he means is that the 7530 FETs are more efficient overall but are only reliable for up to about 10S. I would recommend the 7730 for 12S.
```

---
## \#22 Posted by: eLDoska Posted at: 2017-11-10T09:20:36.687Z Reads: 521

```
[quote="702vegas, post:20, topic:31847, full:true"]
can i change the switch?
[/quote]

yes. you will need a SPDT switch with 3 pins
```

---
## \#23 Posted by: Tal Posted at: 2017-11-10T12:26:14.143Z Reads: 504

```
Are these still for sale? Can you ship to Israel?
```

---
## \#24 Posted by: eLDoska Posted at: 2017-11-10T16:35:29.995Z Reads: 505

```
[quote="Tal, post:23, topic:31847, full:true"]
Are these still for sale? Can you ship to Israel?
[/quote]

yes these are still for sale, and yes i can ship to Israel
```

---
## \#25 Posted by: Tal Posted at: 2017-11-10T16:50:52.151Z Reads: 475

```
nice. i want one how do we proceed?
```

---
## \#26 Posted by: eLDoska Posted at: 2017-11-10T17:14:15.265Z Reads: 506

```
[quote="Tal, post:25, topic:31847, full:true"]
nice. i want one how do we proceed?
[/quote]

i sent information to the PM
```

---
## \#27 Posted by: eLDoska Posted at: 2017-11-20T16:00:04.174Z Reads: 515

```
i have a new antispark - 3 mosfet pcb with 12v led button :)
<img src="/uploads/db1493/original/3X/e/9/e93bc253d2e2d1c565acc69df205f6b7d4a850c4.jpg" width="690" height="321">
<img src="/uploads/db1493/original/3X/4/1/41c78a2d1c8838879e83148c2bcfd527b1971e19.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/e/a/eaad94f268634f4cc6d63ebf9dc39a0bbec9c8ee.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/7/f/7f60a60b6b74e9f0ee04a592b5063ed724f4ce12.jpg" width="690" height="369">

* ready to use Switch with 3 mosfets (with XT60 or XT90; 40A or 60A fuse; heat shrink tube; 10AWG wire; 12V on/off switch) - **35€** / **43$** + shipping

*  ready to use Switch with 2 mosfets (with XT60 or XT90; 40A or 60A fuse; heat shrink tube; 10AWG wire; 12V on/off switch) - **31€** / **38$** + shipping

* PCB with soldered SMD components (3 mosfets) - **21.5€** / **26.5$** + shipping

* other option / bulk price - PM me

shipping to EU/USA ~ **6€**

PCB dimension 58.5x37mm
```

---
## \#28 Posted by: Goja Posted at: 2017-11-22T23:30:17.610Z Reads: 462

```
Nice, can you PM me so we can discuss the details?
```

---
## \#29 Posted by: eLDoska Posted at: 2017-11-23T17:02:13.558Z Reads: 458

```
sure, i sent information to the PM
```

---
## \#30 Posted by: dzIwan Posted at: 2017-11-28T22:39:30.424Z Reads: 447

```
Can i have also one piece?
```

---
## \#31 Posted by: eLDoska Posted at: 2017-11-28T22:54:45.643Z Reads: 436

```
yes, i sent information to the PM
```

---
## \#32 Posted by: GhettoFab.rictation Posted at: 2017-11-30T06:40:35.801Z Reads: 428

```
Damn I wish you would've mentioned that before I bought the 2 mosfet one, still haven't got it so idk all I'm worried about is will it limit my speed by setting bat max 40a on 12s?
```

---
## \#33 Posted by: eLDoska Posted at: 2017-11-30T13:54:37.744Z Reads: 431

```
[quote="GhettoFab.rictation, post:32, topic:31847"]
will it limit my speed by setting bat max 40a on 12s
[/quote]
hi! no, it will not limit your speed because the speed depends on voltage.
```

---
## \#34 Posted by: GhettoFab.rictation Posted at: 2017-12-01T05:34:27.087Z Reads: 433

```
Got it and it is marvelous! <img src="/uploads/db1493/original/3X/f/a/fa9f6e8dbb441ed398c9363362c11001cd2f7a82.jpg" width="281" height="500">
```

---
## \#35 Posted by: GhettoFab.rictation Posted at: 2017-12-01T05:36:11.669Z Reads: 432

```
@eLDoska can I hook this switch up without having to run my led on the drok step down shown above? <img src="/uploads/db1493/original/3X/8/4/843dca0e513733b52173f4f96646711dbddb9bbd.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/4/f/4ff3de9896480b52c140015ce3daa900d42d63cd.jpg" width="281" height="500">
```

---
## \#36 Posted by: eLDoska Posted at: 2017-12-01T13:40:43.465Z Reads: 424

```
[quote="GhettoFab.rictation, post:35, topic:31847"]
can I hook this switch up without having to run my led on the drok step down shown above?
[/quote]
yes, but you need a resistor. if you have a 12S battery and 12V (~10mA ) button you need a 3.6kOhm 1W resistor.
<img src="/uploads/db1493/original/3X/e/9/e95b777bc14213eb3d06fc2029f724cd2881446f.jpg" width="690" height="403">
```

---
## \#37 Posted by: GhettoFab.rictation Posted at: 2017-12-01T20:40:47.130Z Reads: 431

```
Ok so it actually may be easier to run the led off of the step down converter? The step down converter runs 36w/12v/3amp(max 3a). It won't blow the led at this rate? Edit: it says 12v/16/1 idk if that means 16amp switch 1amp led or what but I'll try to research what it means <img src="/uploads/db1493/original/3X/2/1/217921f998e3ed5cb7989bbc748f3c1fe3aeaed6.jpg" width="281" height="500">
```

---
## \#38 Posted by: eLDoska Posted at: 2017-12-01T21:06:20.781Z Reads: 418

```
[quote="GhettoFab.rictation, post:37, topic:31847"]
Ok so it actually may be easier to run the led off of the step down converter?
[/quote]
do what is easier to you :slight_smile:
[quote="GhettoFab.rictation, post:37, topic:31847"]
It won't blow the led at this rate?
[/quote]
no, led button is a consumer, it will take as much as it need.
```

---
## \#39 Posted by: darkkevind Posted at: 2017-12-01T21:28:36.553Z Reads: 407

```
I'd like a 3 MOSFET 60A one please ready to go... How do I go about ordering please?
```

---
## \#40 Posted by: eLDoska Posted at: 2017-12-01T22:12:24.466Z Reads: 409

```
 i sent information to the PM
```

---
## \#41 Posted by: BigBrit Posted at: 2017-12-04T20:30:54.278Z Reads: 378

```
Hi there, can I purchase one of the 3 mosfet antisparks with the LED switch please?  shipped to UK for 40 euro?

Can you PM details please?
```

---
## \#42 Posted by: eLDoska Posted at: 2017-12-04T20:35:25.823Z Reads: 373

```
i sent information to the PM
```

---
## \#43 Posted by: bplatoff Posted at: 2017-12-05T04:38:46.191Z Reads: 378

```
Are you still selling these
```

---
## \#44 Posted by: eLDoska Posted at: 2017-12-05T05:05:37.145Z Reads: 378

```
[quote="bplatoff, post:43, topic:31847, full:true"]
Are you still selling these
[/quote]
yes
10char
```

---
## \#45 Posted by: bplatoff Posted at: 2017-12-05T12:46:39.458Z Reads: 382

```
if I am using a 10s system what number of mosfets should I use
```

---
## \#46 Posted by: Jofjof Posted at: 2017-12-05T15:00:24.540Z Reads: 374

```
Can I have one as well please ?
```

---
## \#47 Posted by: eLDoska Posted at: 2017-12-05T15:35:47.296Z Reads: 413

```
[quote="bplatoff, post:45, topic:31847, full:true"]
if I am using a 10s system what number of mosfets should I use
[/quote]
number of mosfets depends on current(not on voltage).
roughly - 2 mosfets for 1 motor board, 3 mosfets for 2 motor board.[quote="Jofjof, post:46, topic:31847, full:true"]
Can I have one as well please ?
[/quote]
sure, info in PM
```

---
## \#48 Posted by: bplatoff Posted at: 2017-12-06T22:20:44.952Z Reads: 448

```
alright thanks, im gonna get my board working with batteries and once I do I will get one
```

---
## \#49 Posted by: eLDoska Posted at: 2018-01-08T17:00:16.812Z Reads: 457

```
new anti spark - 5 mosfets, 100A continuous, reinforced with 2x6mm2 copper wire, 12v led button :slight_smile:

![IMG_20180109_222030_HDR — копия (2)|635x500](upload://2yAfxVXSz8qxDLSHNfwt5yXLKlQ.jpg)

* PCB with soldered SMD components and with 12V LED BLUE on/off switch + heat shrink tube - **46€ / 55$** + shipping

* PCB with soldered SMD components and with standart on/off switch + heat shrink tube - **39,5€ / 47$** + shipping

* other option / bulk price - PM me

shipping to EU/USA ~ **5€**

PCB dimension - 87x44mm

**3 mofet 60A switch with LED Button:** 
http://www.electric-skateboard.builders/t/vedder-anti-spark-switches-for-sale-from-18/31847/27
```

---
## \#50 Posted by: Hansg Posted at: 2018-01-09T20:43:49.091Z Reads: 422

```
[quote="darkkevind, post:39, topic:31847"]
MOSFET 60A
[/quote]

i want this anti spark but i want to know what is 2 mosfets or 3 mosfets
```

---
## \#51 Posted by: eLDoska Posted at: 2018-01-09T21:09:51.736Z Reads: 429

```
![IMG_20171112_231750_HDR — копия — копия|690x368](upload://bVFYJCXGM58NLzherODq5D1UlcP.jpg)

![20171206_200955 — копия — копия|690x321](upload://KZr6bfSmst3f0yZycaZvoXysEY.jpg)

https://en.wikipedia.org/wiki/MOSFET
```

---
## \#52 Posted by: Weilii Posted at: 2018-01-10T22:02:14.133Z Reads: 402

```
Are you still taking orders for on/off switches? I would like one, could you PM me to discuss details? I had a couple questions.
```

---
## \#53 Posted by: eLDoska Posted at: 2018-01-10T22:33:40.378Z Reads: 400

```
sure, info in PM.
```

---
## \#54 Posted by: KickMe Posted at: 2018-01-14T11:03:11.900Z Reads: 387

```
Hey eLDoska, I'd like a 3-mosfet PCB with 2 unsoldered 60A fuses, could you PM me? Thanks.
```

---
## \#55 Posted by: eLDoska Posted at: 2018-01-14T12:45:36.612Z Reads: 382

```
hi. info in PM
```

---
## \#56 Posted by: Ghettobird117 Posted at: 2018-01-15T00:04:22.872Z Reads: 394

```
Are there any drawbacks to using the 5 mosfet package over the 3 if i wont even come close to maxing out the 3?

Considering the 5 mosfet package if I ever feel like repurposing it in the future
```

---
## \#57 Posted by: eLDoska Posted at: 2018-01-15T14:04:08.219Z Reads: 397

```
the difference between 3 and 5 mosfet is:
5 mosfet - 100Acont., reinforced with 2x6mm2 copper, pcb dimension  - 87x44mm
3 mosfet - 60Acont., pcb dimension 58.5x37mm
other characteristics are identical.
![IMG_20180111_144440_HDR|666x500](upload://tyXRYMcwMjvnO759HTnbE0LOB49.jpg)
```

---
## \#58 Posted by: Lumaci Posted at: 2018-01-15T14:11:36.946Z Reads: 373

```
Still selling?
```

---
## \#59 Posted by: eLDoska Posted at: 2018-01-15T14:22:48.679Z Reads: 365

```
yes
10char
```

---
## \#60 Posted by: Lumaci Posted at: 2018-01-15T14:33:57.587Z Reads: 359

```
Awesome awesome, might be interested in one soon.
```

---
## \#61 Posted by: Ghettobird117 Posted at: 2018-01-15T22:53:48.924Z Reads: 359

```
Interested in a 5 mosfet package soldered up with illuminated switch (is a red one possible?), would a high amp blade fuse holder soldered direct to the board be an issue?

Thinking of the heavier duty switch with a smaller 60A fuse
```

---
## \#62 Posted by: Cobber Posted at: 2018-01-15T23:09:24.854Z Reads: 372

```
[quote="eLDoska, post:49, topic:31847"]
new anti spark - 5 mosfets, 100A continuous, reinforced with 2x6mm2 copper wire, 12v led button :slight_smile:

PCB with soldered SMD components and with 12V LED BLUE on/off switch + heat shrink tube - 46€ / 55$ + shipping
[/quote]

<img src="http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/1/1/11ed2b7249e000e8d79737be62dbd86d42cf93ba_1_635x500.jpg" alt="IMG_20180109_222030_HDR — копия (2)"/>

Looks tough dude!

how much to ship down under? (Au)
```

---
## \#63 Posted by: eLDoska Posted at: 2018-01-15T23:35:46.163Z Reads: 358

```
[quote="Ghettobird117, post:61, topic:31847"]
Interested in a 5 mosfet package soldered up with illuminated switch (is a red one possible?
[/quote]

5 mosfet switch comes like on photo + heatsink tube, and without wires and connectors, because i dont have 6-8AWG wire. 
led collor of the switch is only blue. but you can change the buttoun yourself. just take the button from the holder and put your button.

[quote="Ghettobird117, post:61, topic:31847"]
would a high amp blade fuse holder soldered direct to the board be an issue?
[/quote]
i dont recommend to solder fuse holders, because in most cases the contact area with fuse holder is smaller than by direct soldering. 

[quote="Cobber, post:62, topic:31847"]
how much to ship down under? (Au)
[/quote]

shipping to Au ~ 5€/6$
```

---
## \#64 Posted by: Cobber Posted at: 2018-01-15T23:50:09.348Z Reads: 339

```
Could I or you add screw terminals to the 5 mosfet switch?
I have started to crimp my 6-8-10 awg wire connections... :muscle:
```

---
## \#65 Posted by: eLDoska Posted at: 2018-01-15T23:58:05.156Z Reads: 340

```
[quote="Cobber, post:64, topic:31847"]
Could I or you add screw terminals to the 5 mosfet switch?
[/quote]

sorry, i dont have any screw terminals, but you can add them yourself.
```

---
## \#66 Posted by: Cobber Posted at: 2018-01-16T00:11:44.712Z Reads: 349

```
so if I use a bolt-washer-pcb (switch)-washer-ring terminal-spring washer-nut and drill the pcb with my drill press it should be adequate?

Anything I should look out for?

The ev guys discuss using bellville washers, but also mention 1kv & pcb temps over 120 degrees which is over kill for my application.

https://en.wikipedia.org/wiki/Belleville_washer
```

---
## \#67 Posted by: eLDoska Posted at: 2018-01-16T00:23:28.247Z Reads: 335

```
[quote="Cobber, post:66, topic:31847"]
so if I use a bolt-washer-pcb (switch)-washer-ring terminal-spring washer-nut and drill the pcb with my drill press it should be adequate?
[/quote]

i recommend to solder your wires to make better contact between your wires ans copper reinforcement on pcb
```

---
## \#68 Posted by: Cobber Posted at: 2018-01-16T00:28:13.080Z Reads: 337

```
soldering 6awg is a PIA
```

---
## \#69 Posted by: eLDoska Posted at: 2018-01-16T00:42:05.590Z Reads: 356

```
[quote="Cobber, post:68, topic:31847, full:true"]
soldering 6awg is a PIA
[/quote]

if you want to drill this pcb, pls drill it in red areas and use wider washers(black circles as example) to make better contact with copper reinforcement :slight_smile:
![IMG_2018|666x500](upload://wjvA1g4kCjRUKlziSCNQFI3LrAR.jpg)
```

---
## \#70 Posted by: Cobber Posted at: 2018-01-16T00:54:04.528Z Reads: 339

```
Thanks for the advice bro, i'll work it out.
Put me down for one. 
Lets see if I can blow it up on my eMTB :rage:

pm sent
```

---
## \#71 Posted by: K.kris Posted at: 2018-01-16T15:14:27.133Z Reads: 333

```
I'm using a 6s lipo than the 2 Mosfet one should be enough right ? Do you still got one for me ? Needs to go to the Netherlands.
```

---
## \#72 Posted by: eLDoska Posted at: 2018-01-16T15:32:13.200Z Reads: 342

```
[quote="K.kris, post:71, topic:31847"]
I’m using a 6s lipo than the 2 Mosfet one should be enough right ?
[/quote]
yes, 2 mosfet switch works well with up to 10S battery.
info in PM.
```

---
## \#73 Posted by: Kug3lis Posted at: 2018-01-16T17:14:56.108Z Reads: 333

```
@eLDoska just wanted to mention, that just increasing mosfet count is not good design approach you also need to recalculate values of the RC circuit on the gate because it will cause a problem. Check out our discussion in my topic with @SimosMCmuffin
```

---
## \#74 Posted by: eLDoska Posted at: 2018-01-17T01:17:50.542Z Reads: 332

```
i know it. thank you for your care :)
```

---
## \#75 Posted by: SimosMCmuffin Posted at: 2018-01-17T06:23:31.446Z Reads: 335

```
Optionally you could put some real Low-side driver ICs for the FETs to make sure they are driven high or low properly.
```

---
## \#77 Posted by: AJesk8 Posted at: 2018-01-17T10:44:59.869Z Reads: 325

```
can you do 60a
```

---
## \#78 Posted by: Ghettobird117 Posted at: 2018-01-17T11:36:01.696Z Reads: 335

```
Ill take a 5 mosfet package with goodies sent to Australia please kind sir!
```

---
## \#79 Posted by: eLDoska Posted at: 2018-01-17T12:22:22.482Z Reads: 337

```
[quote="Ghettobird117, post:78, topic:31847, full:true"]
Ill take a 5 mosfet package with goodies sent to Australia please kind sir!
[/quote]
info in PM
```

---
## \#80 Posted by: Lauszus Posted at: 2018-01-25T10:07:59.055Z Reads: 334

```
@eLDoska I need two boards. One for a 6S 30A setup and one for a 12S 20A setup. I don't need you to solder anything, as I will do that myself.
```

---
## \#81 Posted by: eLDoska Posted at: 2018-01-25T10:44:55.661Z Reads: 338

```
info in PM.
```

---
## \#82 Posted by: ikjahaa Posted at: 2018-01-28T22:04:36.401Z Reads: 327

```
still on sale ?
I'd need one with 50amp fuse if possible :slight_smile:
```

---
## \#83 Posted by: eLDoska Posted at: 2018-01-28T22:42:38.296Z Reads: 329

```
[quote="ikjahaa, post:82, topic:31847"]
still on sale ?
[/quote]
sure, info in pm.
```

---
## \#84 Posted by: Mich21050 Posted at: 2018-01-29T06:31:50.313Z Reads: 325

```
Hi!
Are they still for sale?
```

---
## \#85 Posted by: eLDoska Posted at: 2018-01-29T09:31:59.991Z Reads: 324

```
yes. info in PM
```

---
## \#86 Posted by: MaB Posted at: 2018-01-31T17:55:08.386Z Reads: 322

```
Hi, can it work as power killer with a magnetic switch (reed sensor like)? It's for an E-foil, up to 80Amp to cut from battery side if the reed open, do you think te 5mosfet could do?
```

---
## \#87 Posted by: eLDoska Posted at: 2018-01-31T18:51:41.361Z Reads: 323

```
i guess that using such mosfet switch as a power killer (turn on/off under load) is not a good idea because of huge power spikes. but i can make you a discount "for science" if you still want to buy one of them :slight_smile:
```

---
## \#88 Posted by: Cobber Posted at: 2018-02-10T11:50:32.320Z Reads: 325

```
Hey @eLDoska,
your switch arrived the other day, thanks mate!

let's see if I can break it :rage: :rofl:

going to build it in to my eMTB with some new speed controllers and a drop in voltage from 14s to 12s...
a bit less crazy and more just fun, got another road going eSk8 i'm building for the crazy :smiling_imp: might need two switches for that one? do you do a bulk discount :wink: 

I'll let you know how I go, still waiting on other parts for the eMTB :)
```

---
## \#89 Posted by: g.gregory8 Posted at: 2018-02-27T02:16:27.356Z Reads: 304

```
@eLDoska I'm interested in a 100A switch for a eFoil setup, similar to MaB. I tried to PM but couldn't find the option, maybe because I'm new and just signed up.

Do you still have available?
```

---
## \#90 Posted by: eLDoska Posted at: 2018-02-27T09:25:46.994Z Reads: 299

```
[quote="g.gregory8, post:89, topic:31847"]
Do you still have available?
[/quote]

sure. info in pm
```

---
## \#91 Posted by: nikoli280 Posted at: 2018-02-28T19:32:33.317Z Reads: 285

```
How many amps can this handle? and what is price of PCB with soldered smd with shipping to denmark
```

---
## \#92 Posted by: eLDoska Posted at: 2018-02-28T23:38:19.492Z Reads: 280

```
info in PM
```

---
## \#93 Posted by: NAF Posted at: 2018-03-01T12:40:27.251Z Reads: 285

```
Does this Anti-Spark have some sort of protection build in like in AntiSparkHeaven switch ? 
I am interested in the 5 moseft one. My bms is rated 60a but I have killed my previous switch completely.
```

---
## \#94 Posted by: eLDoska Posted at: 2018-03-01T15:28:27.844Z Reads: 277

```
this switch is based on original Vedder-Fechter scheme - it has only short circuit / overcurrent protection.
```

---
## \#95 Posted by: Kug3lis Posted at: 2018-03-01T15:30:11.974Z Reads: 276

```
Sorry, but I can't see any protection on this switch at all ;)

EDIT: Apart Fuse
```

---
## \#96 Posted by: eLDoska Posted at: 2018-03-01T15:38:46.243Z Reads: 276

```
[quote="Kug3lis, post:95, topic:31847"]
EDIT: Apart Fuse
[/quote]

that is great that you noiticed such an unnoticeable thing as a fuse :slight_smile:
yes it is responsible for short circuit / overcurrent protection.
```

---
## \#97 Posted by: Kug3lis Posted at: 2018-03-01T15:41:54.299Z Reads: 277

```
It will not protect from short circuit or overcurrent ;) Short impulse of low current ~10A which would fry all IC and your fuse is still intact ;) Plus protection, means it will turn off the switch and then the short is removed it will turn on again.
```

---
## \#98 Posted by: eLDoska Posted at: 2018-03-01T16:01:13.635Z Reads: 294

```
[quote="Kug3lis, post:97, topic:31847"]
It will not protect from short circuit or overcurrent
[/quote]

i guess we have different understanding what and from what should be protected.
fuse on plus protects at first the battery. it protects the battery from short circuit / overcurrent.
maybe my explanation is not obviously - sorry i try my best :)
```

---
## \#99 Posted by: Hexagown Posted at: 2018-03-03T21:29:36.564Z Reads: 281

```
Hello, I would like to order a 5 moset with 12V LED BLUE on/off switch.
```

---
## \#100 Posted by: eLDoska Posted at: 2018-03-03T21:38:39.131Z Reads: 282

```
info in PM
```

---
## \#101 Posted by: Shagrat Posted at: 2018-03-05T10:16:25.243Z Reads: 282

```
hem.. I'm new here, how do I send a private message? ahhaha
```

---
## \#102 Posted by: L3chef Posted at: 2018-03-05T10:30:05.676Z Reads: 267

```
Click on user name. Then "message"
```

---
## \#103 Posted by: Shagrat Posted at: 2018-03-05T10:58:31.452Z Reads: 265

```
it might be mine problem but I don't have any message button to click on, after been going in his username, probably just because I just created the account 1 hour ago, yes ok I got the message tool avaiable now, thanks anyway
```

---
## \#104 Posted by: wassimBZ Posted at: 2018-03-16T14:35:03.208Z Reads: 258

```
How did you get the "message" option available ? :face_with_raised_eyebrow:
```

---
## \#105 Posted by: Shagrat Posted at: 2018-03-16T14:55:34.619Z Reads: 255

```
Just complete the tutorial bot in the message center and after a while (10min) you should have everything working
```

---
## \#106 Posted by: wassimBZ Posted at: 2018-03-19T00:07:38.816Z Reads: 259

```
Hi,
I cannot PM you but I'd be glad to have more info :slight_smile:
```

---
## \#107 Posted by: eLDoska Posted at: 2018-03-19T00:28:51.669Z Reads: 256

```
hi. info im PM :)
```

---
## \#108 Posted by: Shippo Posted at: 2018-03-22T01:37:27.670Z Reads: 271

```
Hi,

I need one 5 mosfets, 100A continuous, reinforced with 2x6mm2 copper wire, 12v led button
PCB with soldered SMD components and with 12V LED BLUE on/off switch + heat shrink tube - 55$

And one 3 mosfets (with XT90; 40A or 60A fuse; heat shrink tube; 10AWG wire; 12V on/off switch) - 43$

Ship to NY, USA
Please pm me, thanks!

btw, I have 12s5p battery (18650 30Q), is 5 mosfets (100A continuous) the right choice?
another one is 12s2p, should I pick 40A or 60A fuse?
Thank you.
```

---
## \#109 Posted by: eLDoska Posted at: 2018-03-22T08:37:53.684Z Reads: 262

```
info in PM.
```

---
## \#110 Posted by: dilaboards Posted at: 2018-03-27T21:18:29.525Z Reads: 264

```
Hi Doska,

I would be interested for the 3 pcs of 2 mosfet switch. Are you still shipping?

Thanks
```

---
## \#111 Posted by: eLDoska Posted at: 2018-03-27T22:00:11.810Z Reads: 267

```
sure, info in pm.
```

---
## \#112 Posted by: stormboard1 Posted at: 2018-03-28T20:47:48.724Z Reads: 269

```
whats the most amount of mosfets you can fit? would this help with stopping it from blowing?
```

---
## \#113 Posted by: eLDoska Posted at: 2018-03-28T21:10:39.053Z Reads: 290

```
in my opinion 5 mosfet switch is more than enough for 99% of electric boards. 
and qnfortunately quantity of mosfets does not stopp it from blowing.
```

---
## \#114 Posted by: eLDoska Posted at: 2018-04-23T19:15:41.226Z Reads: 314

```
price drop for antispark switches :) 

https://sun9-3.userapi.com/c840520/v840520943/63350/AkPsBo7t4Js.jpg

https://sun9-6.userapi.com/c840520/v840520943/63362/AFxTVIWtnmw.jpg

**2 MOSFET:**  
* Anti-Spark switch (with XT60 or XT90; 40A fuse; heat shrink tube; 10AWG wire; on/off switch) - **28$** + shipping 

* PCB with soldered SMD components - **19.5$** + shipping 
__________________________________________________________________
![IMG_20180|690x495](upload://2CKx3jFPMi8nUnjdFBHFIiTVYvl.jpg)
![IMG_2018042|666x500](upload://w4ovzOK4z7ela1N7nhSNHORSLkO.jpg)

**2 MOSFET with LED button:**
* Anti-Spark switch (with XT60 or XT90; 40A fuse; heat shrink tube; 10AWG wire; on/off switch) - **34$** + shipping 

* PCB with soldered SMD components - **20.5$** + shipping 
__________________________________________________________________

https://pp.userapi.com/c846416/v846416048/3381e/p95VnUtizmc.jpg

https://sun9-3.userapi.com/c840720/v840720670/7ac22/QUh9MgbEJzI.jpg

**3 MOSFET with LED button:** 

* Anti-Spark switch with Led Button (with XT60 or XT90; 40A or 60A fuse; heat shrink tube; 10AWG wire; 12V BLUE LED on/off switch) - **40$** + shipping 

* PCB with soldered SMD components (3 mosfets) - **24.5$** + shipping 

__________________________________________________________________
other option / bulk price - PM me 

Worldwide shipping with tracking number - **4$**
```

---
## \#115 Posted by: longhairedboy Posted at: 2018-04-23T19:24:14.544Z Reads: 293

```
Are you still offering those 5 mosfet monsters?
```

---
## \#116 Posted by: eLDoska Posted at: 2018-04-23T19:46:50.418Z Reads: 289

```
yes, i have couple 5 MOSFET pcb left
```

---
## \#117 Posted by: Grifo Posted at: 2018-05-12T18:57:46.006Z Reads: 282

```
Hi there!

Are you still selling?

How much would it be one with 2 MOSFETS and a 60~65A fuse (I do not need the XT connectors nor the 10AWG wires).

Additionally, I also have a 6V led on/off switch. Do you think I could use it?

Thank you in advance!
```

---
## \#118 Posted by: eLDoska Posted at: 2018-05-12T19:32:54.274Z Reads: 282

```
info in PM
```

---
## \#119 Posted by: oripaamoni Posted at: 2018-05-30T05:38:07.386Z Reads: 280

```
Hello! would like a 5 mosfet version with the lit switch + fuse, don't need any connectors on the board otherwise. Please let me know how to pay you.
```

---
## \#120 Posted by: eLDoska Posted at: 2018-05-30T09:33:16.070Z Reads: 272

```
info in PM
```

---
## \#121 Posted by: bsancken Posted at: 2018-06-03T22:14:54.502Z Reads: 267

```
Hey still have (1)  5 mosfet version with the lit switch available?

 Xt60 connectors, otherwise no main connectors. Blue lit switch if available otherwise send with leads soldered for the switch. 

Thanks!
```

---
## \#122 Posted by: eLDoska Posted at: 2018-06-03T22:35:08.660Z Reads: 255

```
info in PM
```

---
## \#123 Posted by: NAF Posted at: 2018-06-05T19:39:04.129Z Reads: 246

```
Sent you PM
```

---
## \#124 Posted by: Hansg Posted at: 2018-06-08T14:19:36.157Z Reads: 245

```
[quote="eLDoska, post:114, topic:31847"]
Anti-Spark switch (with XT60 or XT90; 40A fuse; heat shrink tube; 10AWG wire; on/off switch) - **34$** + shipping
[/quote]

Hi, I want to buy one Anti-Spark with this refrence "Anti-Spark switch (with XT60 or XT90; 40A fuse; heat shrink tube; 10AWG wire; on/off switch) - 34$ + shipping"

The conector VESC XT60 FEMALE and the batteries XT60 MALE, thanks.
```

---
## \#125 Posted by: eLDoska Posted at: 2018-06-08T14:29:49.197Z Reads: 233

```
info in PM
```

---
## \#126 Posted by: Braylon31 Posted at: 2018-06-09T07:03:45.196Z Reads: 232

```
I want one when can i get it and how?
```

---
## \#127 Posted by: eLDoska Posted at: 2018-06-09T08:23:11.291Z Reads: 233

```
info in PM
```

---
## \#128 Posted by: sunnyD Posted at: 2018-06-11T02:11:45.496Z Reads: 230

```
W A N T. but seriously you got any of these left?
```

---
## \#129 Posted by: eLDoska Posted at: 2018-06-11T08:55:33.654Z Reads: 229

```
info in PM
```

---
## \#130 Posted by: Falcon87407 Posted at: 2018-06-11T21:31:16.318Z Reads: 231

```
Do you have one with everything but the switch?
```

---
## \#131 Posted by: eLDoska Posted at: 2018-06-11T21:39:36.104Z Reads: 228

```
info in PM
```

---
## \#132 Posted by: Gaza65 Posted at: 2018-06-12T10:34:46.843Z Reads: 234

```
Hi there
I would like the 3 thx
Regards Garry wagener
```

---
## \#133 Posted by: Gaza65 Posted at: 2018-06-12T10:42:54.339Z Reads: 225

```
With light switch and fuse thx
Regards Garry wagener
```

---
## \#134 Posted by: eLDoska Posted at: 2018-06-12T10:55:13.522Z Reads: 223

```
info in PM
```

---
## \#135 Posted by: jason07 Posted at: 2018-06-13T10:14:12.580Z Reads: 224

```
Hi i would like to get a 3 mosfet  Anti-Spark switch with 60A fuse. 
plaese send me a pm
```

---
## \#136 Posted by: jason07 Posted at: 2018-06-13T10:41:53.442Z Reads: 217

```
i would like to get one
```

---
## \#137 Posted by: eLDoska Posted at: 2018-06-13T11:03:59.511Z Reads: 228

```
info in PM
```

---
## \#138 Posted by: caustin Posted at: 2018-06-19T03:52:43.732Z Reads: 225

```
Hi, looking for a few Vedder anti spark switches for 12S. Xt60 connectors.  Pls let me.  Ow how to purchase ASAP. Thanks!
```

---
## \#139 Posted by: eLDoska Posted at: 2018-06-19T07:08:50.532Z Reads: 230

```
info in PM
```

---
## \#140 Posted by: sayekim Posted at: 2018-07-04T11:31:15.128Z Reads: 232

```
Got mine in. 

![image|666x500](upload://4VNWhou6rgEEDieSaGeklmnc9Y7.jpeg)
```

---
## \#141 Posted by: Devenart Posted at: 2018-07-10T01:13:53.792Z Reads: 224

```
How do we go about buying this ?
```

---
## \#142 Posted by: eLDoska Posted at: 2018-07-10T08:32:13.569Z Reads: 219

```
info in PM
```

---
## \#143 Posted by: Lebram Posted at: 2018-07-14T00:04:04.564Z Reads: 215

```
Hey buddy, I'm interested in this 3 wire switch anti spark. do you have any available to ship to the USA.
thanks 
Richard
```

---
## \#144 Posted by: Lionpuncher Posted at: 2018-07-14T00:19:30.081Z Reads: 217

```
Note to all: 
Got my switches from @eLDoska a few weeks back. Shopping from Europe to Canada was faster than expected. The quality of the pcb and his soldering is quite apparent. I bought the 3 mosfet bare bones and it's been working great thus far. 
Very happy with the purchase of the switches from this fine gentleman. Highly recommended.
```

---
## \#145 Posted by: eLDoska Posted at: 2018-07-14T12:25:49.581Z Reads: 210

```
info in PM
```

---
## \#146 Posted by: bctech Posted at: 2018-08-09T22:53:14.097Z Reads: 189

```
trying to PM you but can't find the option.
Can you please pm me for the details of purchasing.
```

---
## \#147 Posted by: eLDoska Posted at: 2018-08-09T23:44:45.059Z Reads: 186

```
info in PM
```

---
## \#148 Posted by: StefanMe Posted at: 2018-08-26T19:38:56.945Z Reads: 191

```
Can u PM also? I am interested in the latest 3 Mosfet edition. Thanks
```

---
## \#149 Posted by: tricky-fpv Posted at: 2018-08-26T21:32:37.049Z Reads: 198

```
I am intressed in this anti spark

My setup as is
10s5p
Dual 6355 170kv
Dual focbox

Any help would be great

If possible reply to my email adress

Hawkins22111@yahoo.com 

Cheers!
```

---
## \#150 Posted by: Chase Posted at: 2018-08-26T21:35:07.790Z Reads: 193

```
Got my 5 mosfet about a week ago. Thanks again.
```

---
## \#151 Posted by: eLDoska Posted at: 2018-08-27T11:11:09.386Z Reads: 186

```
info in PM
```

---
## \#152 Posted by: Cristian Posted at: 2018-09-21T07:11:36.522Z Reads: 183

```
Hi, I’m interested in 2 mosfet version for a 8s setup. Only pcb with smd soldered. Could you please provide also the fuse ? I’m from Italy
```

---
## \#153 Posted by: eLDoska Posted at: 2018-09-21T15:34:07.503Z Reads: 186

```
hi! info in PM
```

---
## \#154 Posted by: ze12o Posted at: 2018-09-22T06:21:01.990Z Reads: 182

```
Hello, interested in 3 mosfet, please send details and thank you!
```

---
## \#155 Posted by: Luck Posted at: 2018-10-11T19:07:47.774Z Reads: 182

```
Hi. I'm interested in 3 mosfet version.
```

---
## \#156 Posted by: eLDoska Posted at: 2018-10-12T09:00:23.261Z Reads: 183

```
info in pm
```

---
## \#157 Posted by: agtree Posted at: 2018-10-26T22:35:21.968Z Reads: 193

```
hi
I am intressed in 3 units of this anti spark
My setup as is
https://efoil.builders/t/my-3-month-build/3126
14s , bms 150A on discharge
If possible reply to my email adress

alexagtree@gmail.com
Thanks
```

---
## \#158 Posted by: Manu39 Posted at: 2018-12-03T20:17:28.113Z Reads: 181

```
hello I would also be interested in an anti spark for my foil as can you contact me by MP for an article. my configuration is 12s, ESC 150 amp  in  discharge, i thank an anti Spark with 6 mosfet...
I live un France.
Thank.
```

---
## \#159 Posted by: eLDoska Posted at: 2018-12-03T20:24:59.437Z Reads: 177

```
hi!
info in pm
```

---
## \#160 Posted by: 4ng4rp3 Posted at: 2018-12-07T12:30:46.433Z Reads: 176

```
Hi, I would be interested in one of three mosfets with everything assembled. How long would it take to ship to Spain?

Thanks.
```

---
## \#161 Posted by: eLDoska Posted at: 2018-12-07T14:22:36.295Z Reads: 173

```
info in PM
```

---
## \#162 Posted by: Vicdes2 Posted at: 2018-12-22T02:49:09.897Z Reads: 158

```
Hi, I have the same battery set up as this guy (14s, 150a BMS on discharge)!! I'm also looking for an on/off switch most likely the 100a one. PM me or send me an email at vdesa011@fiu.edu.
```

---
## \#163 Posted by: Vicdes2 Posted at: 2018-12-22T02:49:46.870Z Reads: 157

```
See above please!
```

---
## \#164 Posted by: eLDoska Posted at: 2018-12-22T10:32:26.643Z Reads: 153

```
info in PM
```

---
## \#165 Posted by: Ruubie200 Posted at: 2019-01-31T13:47:16.699Z Reads: 146

```
im running 10s 50a max which switch should i get?
```

---
## \#166 Posted by: eLDoska Posted at: 2019-01-31T14:01:28.145Z Reads: 142

```
info in PM
```

---
## \#167 Posted by: sanderfu Posted at: 2019-01-31T15:13:34.034Z Reads: 142

```
Im also running 10s 50a max and interested in a antispark
```

---
## \#168 Posted by: eLDoska Posted at: 2019-01-31T15:26:17.115Z Reads: 141

```
info in PM
```

---
## \#169 Posted by: The_Dude Posted at: 2019-02-16T20:58:36.795Z Reads: 133

```
@eLDoska still selling your modules?
```

---
## \#170 Posted by: eLDoska Posted at: 2019-02-16T21:02:32.585Z Reads: 133

```
yes
10 char
```

---
## \#171 Posted by: The_Dude Posted at: 2019-02-16T21:11:02.571Z Reads: 138

```
Can you tell me whats the current price for the 3- and 5-Mosfet version with xt90 connectors and the LED-switch. Shipping is to Germany. How do I order/pay etc.?
Just to be sure, 12s is ok?
Thanks.
```

---
## \#172 Posted by: eLDoska Posted at: 2019-02-16T21:17:43.262Z Reads: 143

```
[quote="The_Dude, post:171, topic:31847"]
Just to be sure, 12s is ok?
[/quote]
yes, 12S is ok
info in PM
```

---
## \#173 Posted by: MikeTheisen Posted at: 2019-02-21T11:45:52.112Z Reads: 136

```
I need also 2 of it. How do I order. Shipping to Germany.
```

---
## \#174 Posted by: eLDoska Posted at: 2019-02-21T12:13:29.905Z Reads: 135

```
info in PM
```

---
## \#175 Posted by: captclearleft Posted at: 2019-03-16T15:09:13.410Z Reads: 123

```
Thank You @eLDoska - I received mine, and they are fantastic!

Questions:

Can I remove the push button switch / LED, and just use a regular SPDT switch without an LED?   

Can I use the 12v leads to power something else - such as an Arduino, or separate led's or lights?  (what is the maximum milliamps that I could draw?)

Thanks!
```

---
## \#176 Posted by: eLDoska Posted at: 2019-03-16T23:48:47.743Z Reads: 124

```
[quote="captclearleft, post:175, topic:31847"]
I received mine
[/quote]

great news :slight_smile: 

[quote="captclearleft, post:175, topic:31847"]
Can I remove the push button switch / LED, and just use a regular SPDT
[/quote]
yes, you can use a regular SPDT

[quote="captclearleft, post:175, topic:31847"]
what is the maximum milliamps that I could draw?
[/quote]
about 20mA (0,02A)
```

---
## \#177 Posted by: chefboredpanda82 Posted at: 2019-05-12T16:27:00.985Z Reads: 103

```
Hi are you still selling this. I need one for my 12s system. Please PM me!!!
```

---
## \#178 Posted by: eLDoska Posted at: 2019-05-12T16:34:48.138Z Reads: 105

```
hi. 
yes. info in PM
```

---
## \#179 Posted by: arturoluq1 Posted at: 2019-07-25T12:32:08.085Z Reads: 93

```
hi are you planning on making bigger ones? like 200A current
```

---
## \#180 Posted by: AlanZhou Posted at: 2019-07-25T13:25:26.192Z Reads: 94

```
How are you going to draw 120a continuously?
```

---
## \#181 Posted by: arturoluq1 Posted at: 2019-07-25T14:36:46.671Z Reads: 93

```
120 actually, but in case of a peak is better to be safe
```

---
## \#182 Posted by: eLDoska Posted at: 2019-07-26T11:36:19.471Z Reads: 92

```
[quote="arturoluq1, post:179, topic:31847, full:true"]
hi are you planning on making bigger ones? like 200A current
[/quote]

hi. unfortunately i am not planning to make a 200A anti spark

but could you pls describe your build(motors, battery, esc, mountainboard/longboard)?
```

---
## \#183 Posted by: arturoluq1 Posted at: 2019-07-29T07:19:11.184Z Reads: 85

```
hi, is not a skateboard actually, is for a boat motor because i couldn't find anything better anywhere. In case you change your opinion on making a big one, reply me. Thanks!
```

---
## \#184 Posted by: Jonisonvespa Posted at: 2019-08-13T21:42:32.368Z Reads: 74

```
hi
interested in this do they get hot do they need a heat sink, also are the switches latching or momantary?
```

---
## \#185 Posted by: eLDoska Posted at: 2019-08-13T22:06:07.745Z Reads: 76

```
hi

no, they do not get hot if the current is not higher as the switch is rated for.

switches are momentary
```

---
## \#186 Posted by: eLDoska Posted at: 2019-09-08T15:57:51.186Z Reads: 73

```
https://sun9-13.userapi.com/c853516/v853516443/e7faf/HIc5FxdzyG0.jpg
smaller 3 mosfet anti spark (pcb - 58x27mm)

up to 75V, 70A cont, 360A max

* PCB with soldered SMD components (3 mosfets) -  **24.5$**  + shipping
* PCB with soldered SMD components (3 mosfets) + led button + heat shrink tubing -  **30.5$**  + shipping

worldwide shipping with tracking number - **4$**

other anti-spark switches:
https://www.electric-skateboard.builders/t/vedder-anti-spark-switches-for-sale-from-18/31847/114
```

---
## \#187 Posted by: 702vegas Posted at: 2019-09-13T22:21:16.125Z Reads: 60

```
Where do we order
```

---
## \#188 Posted by: eLDoska Posted at: 2019-09-13T22:27:31.327Z Reads: 64

```
info in PM
```

---
## \#189 Posted by: eLDoska Posted at: 2019-10-11T15:55:47.380Z Reads: 65

```
Anti-spark with key switch and led indicator.

Up to 75V, 60A cont, 360A max

![AirBrush_20191010201133|666x500](upload://dkv1iRNDQpNewWgYS3plwo4u0S6.jpeg)

* Anti-Spark switch with Led Button (with XT60 or XT90; 60A fuse; heat shrink tube; 10AWG wire; 12V  LED indicator; Key on/off switch) -  **45$**  + shipping

Worldwide shipping with tracking number -  **4$**
```

---
## \#190 Posted by: Subusi Posted at: 2019-11-09T18:34:43.687Z Reads: 58

```
hello I would also be interested in a spark protection for my efoil, My configuration is 12s, VESC 75/300  Could you send me an offer via pm?
```

---
## \#191 Posted by: eLDoska Posted at: 2019-11-10T13:31:19.644Z Reads: 51

```
info in pm
```

---
## \#192 Posted by: joseguerra Posted at: 2019-12-29T11:20:19.812Z Reads: 47

```
Hi there, are you still selling the switches?
If yes, I'm looking for one for my eboard - Dual vesc max 100 A continuous and bat is 12s. DM me whenever you are available.

Cheers,
José
```

---
## \#193 Posted by: eLDoska Posted at: 2020-01-02T23:34:43.090Z Reads: 47

```
hi!

yes, i am still selling the switches.

info in PM
```

---
## \#194 Posted by: JFK Posted at: 2020-01-05T18:37:35.747Z Reads: 40

```
Hi all, hi eLDoska,

First of all, I'm acoustician, not electronician (low skills), I did not plan to produce and sell AntiSpark !

I love DIY, so using my little cnc, I have made my first PCB for an AntiSpark, that I'll use in my future projects.

I'm currently on a ESkate and a BoomBox for friends.

ESkate : 36V, 30A, 9.9Ah (10S3P), dual hub, 2xVESC 4.2.

BoomBox : 48V, 30A, 9.9Ah (13S3P), dual amp, DSP, BT5.0...

Using a Software, I have draw this schematic to get a PCB that I can mill : 

The V1 is from the "automatic" PCB maker and the V2 is the same I have re-draw :


The V2 PCB, much more simple ! :

Well ! 
First tests done @24v, 3A (lab power supply) with a 24v light bulb as a load.

Work perfectly, On, OFF, ON, OFF... Perfect.

But, I have an issue and need your help. (Same thing on V1 and V2...)

The second test I have done is with the BoomBox battery @49V charge.

Battery->BMS->AntiSpark->Voltage regulator->Amplifier->Speaker (not on the photo)


Switch OFF, I connect the battery to the switch.

All is OFF, good.

Switch ON, all turn ON, good.

Switch OFF... It doesn't switch OFF.

One of the 3 Mosfet stay closed.

Same after 2 more tests.

Did someone have an idea for me, I have low skills in electronics, I'm learning on every issues ?

Should I add a "big" (how big ?) Diode to help the freeweel of the Mosfets ?


Or the problem is located on the Gate ?... No idea...
I need to understand ! 

Thanks for your help :slight_smile:

Edit 1: Sorry, can't post photos... 

Edit 2: No link too... dunno why...

There is a "link" (add a H first): ttps://drive.google.com/open?id=1TKHm4nMjUXa6Gy_Gc_AsGyMxDTigYueQ
```

---
## \#195 Posted by: BillGordon Posted at: 2020-01-06T00:22:25.027Z Reads: 37

```
Brother, this forum is in dirt nap mode now. Come ask this on the new forum and we'll get some smart dudes in your corner.
```

---
## \#196 Posted by: JFK Posted at: 2020-01-06T09:47:37.846Z Reads: 34

```
Hi, 
Where is the new forum ?
Thanks.
```

---
## \#197 Posted by: nono_fr Posted at: 2020-01-06T13:24:57.617Z Reads: 34

```
 on Google bro' @JFK
```

---
## \#198 Posted by: itsrow Posted at: 2020-01-06T16:05:34.325Z Reads: 36

```
[quote="BillGordon, post:195, topic:31847"]
dirt nap mode
[/quote]

Never lose your wit Bill, absolute gold across both forums.
```

---
## \#199 Posted by: iSalah Posted at: 2020-01-23T19:06:11.507Z Reads: 27

```
Hi 👋 

I’m looking for a 100A antispark switch for 14S battery. Do you still have one in stock ?
```

---
## \#200 Posted by: eLDoska Posted at: 2020-01-23T19:40:53.223Z Reads: 27

```
hi!
sure, info in PM
```

---
## \#201 Posted by: makemesk8again Posted at: 2020-02-05T00:28:44.037Z Reads: 18

```
I'm having shit luck antispark switches from online retailers with my 10s setup. Yours look solid, are you still selling them?
```

---
## \#202 Posted by: eLDoska Posted at: 2020-02-05T01:36:26.210Z Reads: 17

```
hi!
sure, info in PM
```

---
