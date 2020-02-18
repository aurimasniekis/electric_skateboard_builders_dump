# ESCALATE &#124;&#124;&#124; a VESC 6 derivative

### Replies: 106 Views: 5159

## \#1 Posted by: fedestanco Posted at: 2018-06-05T20:49:41.531Z Reads: 641

```
Hi guys,
this winter I had some free time so I decided to start learning about electronics, even though what I am studying (mechanical engineering) doesn't formally require it.

I thought that starting with something interesting would help me learn faster; so I downloaded altium and I slowly built libraries, schematics and pcb layout of VESC 6.4 .

The whole process, expecially the library production, took quite some time to accomplish; for this reason I thought it would be nice to share my work with the experienced guys, which don't need to learn the basics.
![pcb2|674x500](upload://fewUZT55ZeTv0eWL7QL2ARxMZvO.PNG)

![pcb1|636x500](upload://69Cv19dd6TqFBZ5Vk0pSJrh3f6i.PNG)

_Open hardware but..._ 
To respect Ben Vedder decision about not sharing the gerbers -with the goal of keeping the project in the hands of experienced guys to avoid poor quality vescs- these are the conditions to get the files :
1) you have electronics experience and  have some open-source contribution records
2) if you plan to sell the hardware you agree to donate a fixed % to Vedder

The documentation that I will share includes everything: gerbers, schematics, libraries, pcb source files and enclosure 3d model (in the works..). 

Example of people who can ask for the files are : @jtag , @solidgeek , @Ackmaniac ...
```

---
## \#2 Posted by: fedestanco Posted at: 2018-06-05T20:51:25.416Z Reads: 596

```
About the name:
if the name doesn't sound good in english, please PM me a better one!

About the hardware:
1) as you can see the tallest components have been routed as far as possible from the fets; the reason is to keep  more mass close to the mosfets

2) connectors are still JST PH 2.0, just a surface mount type. I used the industry standard 1.5mm pitch for the SENSOR connector, so no more adapters are needed; the PPM connector has been substituited with a more convenient solder pad (so the wire can be presoldered at the fab)

3) dimensions are 61.5 x 59.1 mm

4) since directfets seem always out of stock, I will make a second version of this pcb with 4 [ntmfs5c604](https://datasheet.octopart.com/NTMFS5C604NLT1G-ON-Semiconductor-datasheet-33954820.pdf) per gate providing about half of the 2 directfet RDSon

5) a fancy ic-based anti-spark switch is being developed and will be opensource without restrictions. It will include some features like e-fuse, transitient voltage suppression, overvoltage and overcurrent protection
```

---
## \#3 Posted by: JTAG Posted at: 2018-06-05T21:19:39.641Z Reads: 556

```
Holy sh* it looks SO good :blush:!

Did you build one already ?!?!?! And what a honor ^^!
```

---
## \#4 Posted by: karma Posted at: 2018-06-05T21:20:36.886Z Reads: 551

```
I would also like to know if this has been built and confirmed working :)
```

---
## \#5 Posted by: fedestanco Posted at: 2018-06-05T21:24:05.987Z Reads: 544

```
This week I am ordering the pcbs, but the exam session has started and there isn't much time to work on hobby stuff...
```

---
## \#6 Posted by: fedestanco Posted at: 2018-06-05T21:30:12.607Z Reads: 535

```
Your appreciation means a lot , thanks! This is the first pcb I ever made so I had many doubts while designing; many have been solved looking at your bms design: the power of opensource.

Give me a couple days to clean the schematics from my notes in italian and will send you the files.
```

---
## \#7 Posted by: solidgeek Posted at: 2018-06-05T23:18:46.952Z Reads: 513

```
Well done, it looks amazing :+1: !!! I am dazzled by how you have mastered Altium Designer in less than a year, making something as complex as a VESC 6 while also studying. Thanks for your mention of me, I am glad you like my work! 

If you find any difficulties/issues testing the prototypes I would be happy to help (and I would love to fabricate one myself) :crazy_face:
```

---
## \#8 Posted by: Devilmycry Posted at: 2018-06-06T01:06:49.791Z Reads: 497

```
This is amazing job man 

I wish I can building my
```

---
## \#9 Posted by: Blacksheep Posted at: 2018-06-06T01:10:25.900Z Reads: 489

```
This is really cool
```

---
## \#10 Posted by: Seikeau Posted at: 2018-06-06T07:56:49.517Z Reads: 470

```
I thought Trampa had an exclusive patent on squares :joy:
```

---
## \#11 Posted by: linsus Posted at: 2018-06-06T08:19:09.511Z Reads: 463

```
PMed you about the layout :)
```

---
## \#12 Posted by: Pimousse Posted at: 2018-06-06T09:46:58.813Z Reads: 461

```
Learning electronics by building your own VESC 6 is kind of a challenge !
Congrats !!
I'm in the same process, but can't find time (ATM I learned C code to but a custom FW. Step by step :) ).
```

---
## \#13 Posted by: banjaxxed Posted at: 2018-06-06T10:33:47.154Z Reads: 462

```
Nice work @fedestanco, I have some of stewii's pcbs to populate already or I would be jumping in on it.

Since I enjoy disruption in general, it would be rich irony to use the name -

ESCapade

!!!

Ps. CAPs normally close to each other for hot glue and vibration breaking avoidance?

(I like your ESC naming)
```

---
## \#14 Posted by: district9prawn Posted at: 2018-06-06T10:36:57.336Z Reads: 447

```
Very nice! I'm totally down for a directfet or SO-FL-8 pcb once you have one assembled and running.
```

---
## \#15 Posted by: Cobber Posted at: 2018-06-06T11:55:36.697Z Reads: 455

```
Looks cool Bro? well done congrats :+1:

While I am not after any files or plan on building a ESC of my own... generation 4.xx VESC all files were released. I think it was a strategic move by Vedder (who has done the community some amazing work, albeit opensource so with the help of others) & Co to slow things down on this release so they could build their TM and make sales un-apposed.
& while I applaud your sentiment of returning some profits to Vedder acting like a gate keapper and refusing to share anything unless there is payment kind of goes against something being open source... it is more open commerce.
We really are at the beginning of this HW.6X journey. From a advanced development perspective for the real development to happen the cash cow that is the VESC 6 needs to be killed. As long as there is such price disparity products will only compete on price. Once some of that margin is taken away (like back to the price Trampa sell a VESC 6 with a complete) then the real innovation from people like your self will happen bro. HW.6X will then begin competing for features, or lack of features so that the product suits the market.

This is the basic premise of innovation and disruption. While you have learnt some mad skills quickly you are now stalling to tread water where you could be contributing to a incremental evolution of the product or better still disrupting the market and changing the game.

All that said I think downloading bldc tool from Vedder and donating for it is a great idea and of course you should follow all requirements for the opensource hardware software as laid down in the GPL.

finally...

[quote="banjaxxed, post:13, topic:57947"]
CAPs normally close to each other for hot glue and vibration breaking avoidance?
[/quote]

As Jaxxy mentioned the two big caps will break their own legs from their weight/vibration in use, i'd silicone them in place in the enclosure with a neutral cure silicone (hot glue can work, but it also gets soft when it gets hot). You could make a mold and insert a couple of pre-molded silicone pads so they can be removed for service, but not really required.

Anyway good luck again dude, knock a couple of those badboys out and give them to a beast in the community and see if they hold up as good as a VESC.6
```

---
## \#16 Posted by: fedestanco Posted at: 2018-06-06T16:01:52.572Z Reads: 416

```
@linsus @solidgeek please pm me your email adress.

[quote="banjaxxed, post:13, topic:57947"]
I would be jumping in on it
[/quote]

Nothing to jump on yet :) it's still in testing stage. ESCapate is cool but a bit too sillar to stewii's.

[quote="Cobber, post:15, topic:57947"]
it is more open commerce.
[/quote]

let's call this open commerce then. 

[quote="Cobber, post:15, topic:57947"]
two big caps will break their own legs from their weight/vibration in use
[/quote]

natural cure silicon is too slow. Never heard of hot glue on focbox melting so it remains the best option yet. Maybe a memory foam support underneath could also help.
```

---
## \#17 Posted by: banjaxxed Posted at: 2018-06-06T16:04:55.822Z Reads: 395

```
And that's why it's ironic, the whole TM thing about naming conventions and avoiding similar product names [quote="fedestanco, post:16, topic:57947"]
ESCapate is cool but a bit too sillar to stewii’s.
[/quote]
```

---
## \#18 Posted by: zhud Posted at: 2018-06-06T16:10:44.201Z Reads: 406

```
Electrical and computer engineer here. 

Liking what I am seeing, great work!

If you are in need of some testing and debugging, I can definitely be a resource for you. I've been working with these VESCs for about a year now and I am familiar with the designs. Shoot me a PM if you need a professional tester.

Looking forward to this development. Cheers!
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2018-06-06T16:14:42.150Z Reads: 400

```
[quote="fedestanco, post:16, topic:57947"]
Never heard of hot glue on focbox melting
[/quote]

FOCBOX use silicone :wink:
```

---
## \#20 Posted by: moon Posted at: 2018-06-06T16:14:43.084Z Reads: 392

```
Pablo ESCobar? :rofl::rofl:
```

---
## \#21 Posted by: Deckoz Posted at: 2018-06-06T16:15:17.385Z Reads: 384

```
[quote="zhud, post:18, topic:57947"]
professional tester.
[/quote]

Not sure how one can be a professional tester...

Lol. I test shit, I'm also electrical/power engineering and software engineering background. But my job isn't a product tester..

Are you a professional product tester for a company? Lol.. professional tester ^^ this makes me giggle
```

---
## \#22 Posted by: moon Posted at: 2018-06-06T16:15:25.457Z Reads: 363

```
Doesn't silicone also provide dampening properties but hot glue doesn't?
```

---
## \#23 Posted by: Kug3lis Posted at: 2018-06-06T16:16:35.253Z Reads: 360

```
I think its more needed to hold it tight so it wouldn't move not dampening :)
```

---
## \#24 Posted by: fedestanco Posted at: 2018-06-06T16:17:33.273Z Reads: 362

```
Name suggestions in PM please. Cool name though.

[quote="JohnnyMeduse, post:19, topic:57947"]
FOCBOX use silicone
[/quote]
Good to know, I might look into it. There might exist a silicone which is both fast and natural cure...

@zhud any github page I can check out to have a look a your projects?
```

---
## \#25 Posted by: moon Posted at: 2018-06-06T16:17:38.997Z Reads: 361

```
Oh ok I always thought it was a bit of both because of esk8 vibrations and all
```

---
## \#26 Posted by: zhud Posted at: 2018-06-06T16:18:00.372Z Reads: 368

```
If it makes it easier to digest for you I'll categorically label myself a professional and a tester, but I'm not here to decipher your perception on the world. Carry on!
```

---
## \#27 Posted by: Deckoz Posted at: 2018-06-06T16:18:54.618Z Reads: 359

```
Lol ^^^^ still giggling
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2018-06-06T16:19:25.316Z Reads: 360

```
Well I personally use KAFUTER 704 RT which cure enough for manipulation in 10-15Min
```

---
## \#29 Posted by: zhud Posted at: 2018-06-06T16:35:15.366Z Reads: 360

```
I am a computer systems engineer at an unnamed aeronautics and research institution and my work is not available to share publicly :) 

But if you are interested I can give you some info from my personal projects. My work is mostly CMOS and hardware architecture with some work in AI and robotics as well.
```

---
## \#30 Posted by: Deckoz Posted at: 2018-06-06T16:41:25.805Z Reads: 376

```
[quote="zhud, post:29, topic:57947"]
work is not available to share publicly :slight_smile:
[/quote]

[quote="fedestanco, post:1, topic:57947"]
you have electronics experience and have some open-source contribution records
[/quote]

Lol. We all have actual careers with work that cannot be shared. I've contributed to the OS community, but not Esk8 OS community. Which is why you don't see me asking because his criteria we're pretty clear.

Ugh
![giphy%20(8)|300x232](upload://zCLpyhlBG2r1BKVIm5qJpL5yPKC.gif)
```

---
## \#31 Posted by: DavidLee Posted at: 2018-06-07T13:16:12.927Z Reads: 358

```
It's a really a big challenge to study design an ESC.and what can I do for you?:smile:
```

---
## \#33 Posted by: banjaxxed Posted at: 2018-06-07T17:32:26.591Z Reads: 370

```
But not covert!

[quote="zhud, post:29, topic:57947"]
an unnamed aeronautics and research institution
[/quote]

![IMG_8951|281x500](upload://rb9KD3FY8ru9EL9Gcojhy8xyDn.PNG)

I'm a little disappointed that NASA were unable to make their own variant using Vedders schematic
```

---
## \#34 Posted by: fedestanco Posted at: 2018-06-07T19:43:42.624Z Reads: 364

```
PCB update: I re-routed a shunt amplifier closer to the shunt resistor to minimize EMI on the sense traces.

![new%20layout|637x500](upload://4Bd1fM1VBrFDDZ1IbYRB5fhDyfw.PNG)

Case update: I sketched up this case. I had as priorities: 
1)cnc cost: the whole case can be routed with 0 tool changes. Only 4mm bit is required.
2)the smaller the better (65 x 62mm)
3)pcb should't be in contact with metal to avoid vibration transfer. I obtained this by using 2 o-rings on the 2 lateral supports. The 3rd support is already substained by the heat transfer pad, which already acts as vibration dampening.

![outlines|690x426](upload://4tfA1KBnYljM48X2jKCCVrUAcz2.PNG)
![how%20pcb%20is%20mounted|690x444](upload://llbec8pWnmXF0DVk0PxrY8gZXiB.PNG)
```

---
## \#35 Posted by: PatRocks Posted at: 2018-06-07T19:45:15.713Z Reads: 350

```
@banjaxxed LOL
@Deckoz i was wondering what you do for a living!
@Cobber really interesting perspective. I like where your head's at as usual 
Back on topic, @fedestanco it's really great to see you working on this. Your contribution to the forum is awe inspiring. Best of luck with the exams! I'm eager to see what you can do with this "ESCiMO" lol
```

---
## \#36 Posted by: fedestanco Posted at: 2018-06-07T19:52:32.935Z Reads: 352

```
[quote="Deckoz, post:30, topic:57947"]
I’ve contributed to the OS community, but not Esk8 OS community
[/quote]
Actually this is fine; my goal is to share this with people that are already into the open-source game: this way the probability of them sharing back any improvement is much higher, but yet not assured.

[quote="DavidLee, post:31, topic:57947"]
what can I do for you?
[/quote]
you joined 2 days ago so contribute to the community, learn electronics, do open source stuff and then come back.
```

---
## \#37 Posted by: okp Posted at: 2018-06-07T20:15:59.570Z Reads: 339

```
good job bro !
```

---
## \#38 Posted by: Sebike Posted at: 2018-06-07T20:33:42.028Z Reads: 331

```
Woah. That's the GROTESC! :sweat_smile:
```

---
## \#39 Posted by: Dyspro Posted at: 2018-06-07T20:50:05.347Z Reads: 336

```
I guess our new bastion is GitLab since GitHub was bought by Micro$oft haha.
```

---
## \#40 Posted by: DavidLee Posted at: 2018-06-08T02:51:40.778Z Reads: 339

```
OK,Thank you so much!
```

---
## \#41 Posted by: Gamer43 Posted at: 2018-06-10T09:57:36.353Z Reads: 348

```
Wow, that looks amazing, I've tried PCB design before, and it was just a complete mess trying to arrange and route the smd resistors Dx.
If you have any more stock issues, I would also like the recommend using the TPW1R306PL,L1Q from Toshiba Semiconductor, it has similar electrical characteristics (RDSon and switching charge) to the ON Semi NTMFS5C604NL, but is cheaper and features double sided cooling.  (Honestly, I'd avoid anything from International Rectifier brand in this performance range; their transistors are expensive and inferior to similarly priced competitors on the market.)
Which current shunt amps are you using? I just wanted to let you know that the INA240 from Texas Instruments offers superior electrical characteristics and pricing compared to the ones from Analog Devices that are used on the VESC 6. 
If you don't already, I would highly recommend RC snubbers on all the switch nodes for the DRV8301; I've seen way too many DRV chips die on my friends' VESCs and it's really saddening since many of them aren't able to replace the chips themselves as it is very difficult to replace.
```

---
## \#42 Posted by: Minim Posted at: 2018-06-10T18:42:54.999Z Reads: 336

```
I like how you did the case! I would however not design it so it can be done with 4mm all the way. I made a video of my first set of vesc6 cases and it had 9 tool changes i think but that was including drilling and tapping M3 and M4 in the same operation. It’s way more efficient to remove material with a bigger endmill/rougher :D 

The 3 fixing spots to the enclosure is the way to go. The Escape is only fixed with two M3 over at the fets so there is a lot of strain on the board if the case isn’t filled with silicone around some sweetspots. 

If you need milling of the enclosure I’ll do it for material cost+shipping for a good cause :) I’m not an expert at this so tolerances won’t be aerospace like but should be decent for a case. 

https://m.youtube.com/watch?v=G-xif0AYjOg
```

---
## \#43 Posted by: akhlut Posted at: 2018-06-10T19:06:51.174Z Reads: 327

```
that video is pure filth.  :D  #machineporn
```

---
## \#44 Posted by: moon Posted at: 2018-06-10T19:07:50.591Z Reads: 325

```
Do you run/own your own shop ? :heart_eyes:
```

---
## \#45 Posted by: fedestanco Posted at: 2018-06-10T20:07:19.355Z Reads: 333

```
@okp thanks, I have't forget about you- I'll send you the torture units as soon as they are made; maybe also the new antispark

[quote="Gamer43, post:41, topic:57947"]
TPW1R306PL,L1Q from Toshiba
[/quote]
So many tips in one post, thanks! much appreciated. While choosing the bom I think is wise to beware of China market stock. By this logic the NTMFS5C series is a champion, basically any chinese resaller has them both fake and original. I was thinking about going with the -612 (dual) offering a combined rdson of 0.75 mohm, less gate charge of a directfet and an average price of 0.6eu each (China market) for the originals.
I like the double cooling of the toshiba though so I will look into that, as well as the shunt ic.

[quote="Minim, post:42, topic:57947"]
I would however not design it so it can be done with 4mm all the way
[/quote]
I was meaning that smallest radious is 4mm so it is possible, not mandatory, to do 0 tool changes :slight_smile: . Your offer is very generous; I would feel bad though about outsourcing the big batch for real production after your favor-- and unfortunately outsourcing is almost mandatory to keep costs low and logistics simple. How about if on top of materials+shipping I send you 10 unpopulated pcbs? Thanks for the #cncporn btw.
```

---
## \#46 Posted by: Minim Posted at: 2018-06-10T21:10:51.374Z Reads: 321

```
@moon just as a side business/fun/hobby. 

@fedestanco No worries about outsourcing for a bigger batch. This is more of a hobby anyways and I just wanted to help out on a good project for the prototype :) I just got a set of escapes so Pcb are really not needed but if you really want to it would be cool to try to solder up my first smd project for my kids toy car :p
```

---
## \#47 Posted by: Pimousse Posted at: 2018-06-19T06:55:51.775Z Reads: 306

```
Hi @fedestanco,
Is there any room for another connector ? I'd love to have access to more STM32 spare IO.
I stuck into coding my custom VESC FW integrating mode because no spare IO for interacting with it.
Using Rx/Tx (as coded in the official FW) isn't a way to go as everybody wants BLE now.

Also, to reduce cost of the case, why don't you machine only the bottom and then machine POM walls ?
Less material, less machining, less cost. ;)
```

---
## \#48 Posted by: linsus Posted at: 2018-06-19T07:14:00.112Z Reads: 291

```
What do you need more IOs for? Just make a new pcb with CAN  transciever? :o

@fedestanco sent you another email with pointers
```

---
## \#49 Posted by: Pimousse Posted at: 2018-06-19T07:22:03.941Z Reads: 291

```
Why would I need an additional PCB with CAN transceiver while I only need one or two additional digital input ?
There are a lot of unused IO on the VESC's STM32, so KISS, no ? :slight_smile:
```

---
## \#50 Posted by: linsus Posted at: 2018-06-19T07:23:49.584Z Reads: 291

```
Was just curious what you wanted to use them for :) usually making a separate pcb if its something major makes sense
```

---
## \#51 Posted by: Pimousse Posted at: 2018-06-19T07:37:10.770Z Reads: 305

```
I wrote a firmware that embeds simple mode, compatible with any app (not only ppm).
I collected a LOT of feedbacks from different users (from electric skates, scooters or bike users) about this lack of mode switching just by pushing a button (and not using a smartphone with all known connectivity issues)
In the current firmware, the only way to use digital input is to use :
- Rx/Tx if not in "whatever + UART" app (= impossible to use bluetooth or other UART third-party devices)
- PPM input in ADC mode

Those digital inputs are already used for cruise control or reverse purpose.
The only trick I could do today is to re-program unused ADC3 as a DI on HW6.4. :neutral_face:
This is why having a couple of other DI could a a really good improvement for enhancing the use of VESC in so many applications. :slight_smile:
```

---
## \#52 Posted by: fedestanco Posted at: 2018-06-19T12:21:34.705Z Reads: 295

```
Yes, there is quite some real estate on the bottom side, where the logo is. The purpose of this free space is to solder an FCC certified nrf module, so that even US people can use this feature. 
https://it.aliexpress.com/item/4pcs-Pack-NRF24L01-Chip-Module-RF2401F20-with-FCC-Certification/32335219778.html

Thanks to @linsus' hint I re-routed -again- the 3rd shunt amplifier. BTW I still don't understand well why a PWM signal is more susceptible to EMI than the current sense traces. I thought it was the opposite.

I also made a first draft of the BOM, trying to max out the components specs. 
Octopart says that the best 680uf 63v cap is EEUFR1J681L (21mohm, 10 000h life, 2.8A ripple). But @Blasto claims [focbox caps are 20mohm](https://www.electric-skateboard.builders/t/sesc-a-vesc-6-derivative/58106/76?u=fedestanco); maybe a typo?
```

---
## \#53 Posted by: Pimousse Posted at: 2018-06-19T12:31:37.514Z Reads: 299

```
Isn't it for the reason that AD8418 has already builtin EMI filters ? (if you use those)
Just for my understanding.

![AD8418|428x337](upload://wcYNBOq07JZS5dQcTxrRFWvvA4j.PNG)
```

---
## \#54 Posted by: linsus Posted at: 2018-06-19T12:40:48.359Z Reads: 288

```
Doesn't really matter if the IC is certified or not, you have to certify the Product as an individual unit, thats why trampa doesnt include it in thier US version, simply to complicated and expensive.
```

---
## \#55 Posted by: briman05 Posted at: 2018-06-19T12:54:03.851Z Reads: 290

```
I like where this is heading as the 3d renderings look great.  What I would like to see though is some thing like the focbox unity for the vesc 6.  You do that and there would be a line of people waiting.  I feel like once you have some of your esc out with some real world testing maybe start looking at doing something for a dual drive all in one system because so many people here have the dual setup.  I wish I could lend my knowledge but I do not have much knowledge in the electrical field, If this was the analytical field then I would be able to help.
```

---
## \#56 Posted by: Blasto Posted at: 2018-06-19T15:35:21.782Z Reads: 279

```
huh, you're right, sorry about that. corrected.
```

---
## \#57 Posted by: Kug3lis Posted at: 2018-06-19T15:41:48.183Z Reads: 283

```
I dont remember correctly now but I think if RF module is pre-verified by FCC you don't need to verify whole product as long that module is fixed to your hardware and follows requirements or something like that...
```

---
## \#58 Posted by: linsus Posted at: 2018-06-19T15:55:05.335Z Reads: 285

```
Sounds very unlikly to me. FCC is way more strict then the EMC directives we have in the EU. And here you have to do sevral certifications, EN55xx is just for anything electrical. Addin a radio on it adds sevral other certifications if a commercialy available Product. I love the idea that the manufacturer could promise that, but feels bit farfetched.
```

---
## \#59 Posted by: Kug3lis Posted at: 2018-06-19T15:57:28.589Z Reads: 288

```
Yes, I understand your point as I haven't worked with US market so I can't tell anything about it europe is pretty easy like you say ;)

I found this website regarding `pre-certified` modules maybe it will help @fedestanco

https://emcfastpass.com/rf-modules/
```

---
## \#60 Posted by: linsus Posted at: 2018-06-19T16:07:11.402Z Reads: 284

```
ah its an entire PCB with shield and Everything, yeah. its plausible. Just like Decawave etc. Looks very promising
```

---
## \#61 Posted by: fedestanco Posted at: 2018-06-19T19:25:13.535Z Reads: 287

```
Thanks for the link. 1-2k is doable. But you must have a very solid and tested design before submitting the request, and it could take a while.

My backup plan to skip stupid legal stuff was to manufacture, instead of the "cover pcb", a 2mm plexiglass cover (which BTW looks much cooler since you can see the interiors) and have the module siliconed to it. This way you don't have to obtain a new certification since you didn't technically create an "rf pcb" but just a support for the module.
The connection to the vesc below this plexiglass can be made by a simple I/O cable.
```

---
## \#62 Posted by: ducktaperules Posted at: 2018-06-19T20:19:39.802Z Reads: 270

```
I agree. I would 100% be all in for a dual vesc6 with built in anti-spark.
```

---
## \#63 Posted by: JohnnyMeduse Posted at: 2018-06-19T20:25:11.329Z Reads: 272

```
[quote="briman05, post:55, topic:57947"]
the focbox unity for the vesc 6.
[/quote]

What do think the Unity is base upon... Not the 4.12 :wink:
```

---
## \#64 Posted by: briman05 Posted at: 2018-06-19T20:28:21.429Z Reads: 268

```
I figured it could be 6 but wasnt sure and why should enertion have all the fun with a single focbox for dual.  I'm sure someone here is smart enough to figure it out.  I just know it wont be me
```

---
## \#65 Posted by: ducktaperules Posted at: 2018-06-19T20:28:42.360Z Reads: 274

```
[quote="JohnnyMeduse, post:63, topic:57947"]
Not the 4.12
[/quote]

oh really? my understanding is that the unity is based on 4.12 but with some improvements for reliability.
```

---
## \#66 Posted by: JohnnyMeduse Posted at: 2018-06-19T20:53:32.348Z Reads: 276

```
Well... it is really a in between product, it is more than just a beefup 4,12, since the heart of the 4.12 was mostly the drv8302. The unity is base upon the DRV8301 like the Vesc6, But I do agree it a bit confusing, since it is not a Vesc6 or neither a vesc 4.12, is it a complete different implementation of the same family of components.
```

---
## \#67 Posted by: fedestanco Posted at: 2018-06-19T20:56:43.691Z Reads: 279

```
Looks very promising and production friendly. Impressive routing job since the components are on one side only.
```

---
## \#68 Posted by: district9prawn Posted at: 2018-06-20T01:45:00.790Z Reads: 282

```
Isn't the unity still 2 low side shunts?
```

---
## \#69 Posted by: EnderWiggin Posted at: 2018-06-24T18:02:29.793Z Reads: 277

```
wow! This is great! Thanks for pointing me here. I was going to use the micro VESC on the race quad and the VESC 6 on my mountain board and battle bot. Any way i can get the github of the project
```

---
## \#70 Posted by: Pimousse Posted at: 2018-06-25T07:56:56.216Z Reads: 276

```
Hi @fedestanco ! I digged into building PCB as well, but with Kicad (would love to stick to Open Source spirit, hope I took the right way though).
About building the library, were you in the need to download each component's CAD, one by one ?

Sure, Altium and Kicad are not the same, but wondering if this process is the same though.
```

---
## \#71 Posted by: fedestanco Posted at: 2018-06-25T12:48:35.276Z Reads: 263

```
[quote="fedestanco, post:1, topic:57947"]
* you have electronics experience and have some open-source contribution records
* if you plan to sell the hardware you agree to donate a fixed % to Vedder
[/quote]

Hi @EnderWiggin ,as I explained you in PM these are the only requirements to get on board. 

@Pimousse I tried to find as much as possible pre made footprints and 3d models already made online. Snapeda is the best source. To design footprints yourself I suggest to use a 3D editor like fusion360 and then import them as dwg. In fact I found the built in footprint designer too oversimplified. 
Btw if you tell me the library format of kikad I can try to convert everything a send the files to you.
```

---
## \#72 Posted by: Pimousse Posted at: 2018-06-25T12:56:41.078Z Reads: 259

```
Thanks for your answer !
Kicad uses *.lib (symbols) and *.mod (footprints) files.

Any chance I can jump into your A-team ? :smiley:
That would ease my process by looking at the way you did (maybe too much ? Should I learn by my own anyway ?)
```

---
## \#73 Posted by: moon Posted at: 2018-06-25T12:57:17.060Z Reads: 268

```
I am not sure for fedestanco but I am collaborating with someone to make a pcb design and I had to find CAD files for JST connecters,USB, switch and the r-sense chip. The rest I found online
```

---
## \#74 Posted by: fedestanco Posted at: 2018-06-25T12:58:52.517Z Reads: 274

```
Sure thing, I saw you made some pull requests to the vesc directory so PM me your email.
```

---
## \#75 Posted by: fedestanco Posted at: 2018-08-20T14:44:38.261Z Reads: 255

```
Update: I can start soldering the first prototype as soon as components arrive. 
![20180820_164324|690x388](upload://1Qlc7BQHOneU55ilqlLuGdfUR1Y.jpg)
```

---
## \#76 Posted by: Pimousse Posted at: 2018-08-20T14:48:50.914Z Reads: 252

```
Congratulations !
```

---
## \#77 Posted by: uigiroux Posted at: 2018-08-20T22:38:36.843Z Reads: 248

```
Looks like the Unity is getting more and more competition!  Good thing for Enertion they priced it 'competitively' and the shipping is reasonable.  Lol... :smile:

This looks amazing! :heart_eyes:  Any idea what the cost will be around?
```

---
## \#78 Posted by: mmaner Posted at: 2018-08-21T00:00:24.644Z Reads: 245

```
You need yo ease up, the last few messages I've read that you wrote are digging at enertion. As far as I know you haven't bought any enertion products so stick to what you know. 

`I say this as a community member, not as a mod.`
```

---
## \#82 Posted by: moon Posted at: 2018-08-21T00:24:59.649Z Reads: 249

```
This is all off topic... Anyway, I had a friend that helped me design a VESC derivative too

![mmexport1534537959796|281x500](upload://hyb5GlBCz3XXEdFqhn7w8IJmliB.jpg)
```

---
## \#83 Posted by: fedestanco Posted at: 2018-08-21T00:29:31.582Z Reads: 249

```
Lets see if shit works first. Anyways I dont expect the price tag to be over 100e depending on how much tax I'll have to pay.
BTW the fab sent me 15 extra boards I didn't pay for. I'd be fine sending them out for free to people with good reflowing skills ( @JohnnyMeduse @JTAG  ...)
```

---
## \#85 Posted by: fedestanco Posted at: 2018-08-21T00:38:11.286Z Reads: 246

```
Mike do you mind stop trolling on this thread? Thanks
```

---
## \#87 Posted by: uigiroux Posted at: 2018-08-21T00:40:30.599Z Reads: 242

```
That's great!  Incredible price, will be keeping a close eye on this thread :slight_smile:

Build quality looks fantastic btw!
```

---
## \#88 Posted by: Pimousse Posted at: 2018-08-21T06:42:57.440Z Reads: 234

```
Just have a new reflow on its way to home (after few weeks of dispute 'cause, you know, a summer job student wanted to honor France football victory while carrying the previous parcel :roll_eyes: ).
So, I might be interested into a PCB although I didn't have any reflow skill yet.
Up to you ! :slight_smile:
```

---
## \#89 Posted by: Andy87 Posted at: 2018-08-21T09:57:48.060Z Reads: 227

```
looks great, but don't you think the main power cables a bit to slim....:stuck_out_tongue_winking_eye::joy::thinking:
```

---
## \#90 Posted by: fedestanco Posted at: 2018-08-26T21:53:06.889Z Reads: 234

```
Bottom side is populated. This is the first time I use hot air soldering and I am pretty happy with the results; just a few solderballs and a cooked connector. Any suggestion about air temp/air speed and such is very welcome.

![20180826_234344|690x388](upload://2mf8QbZQ38w4Ig9CSKlz7gflhoz.jpg)

@Pimousse you may want to start with something easier.
```

---
## \#91 Posted by: fedestanco Posted at: 2018-09-06T20:38:42.829Z Reads: 229

```
They are done. I tested the 5v rail and it works. I bought the wrong 3.3v regulator so have to wait the new one before flashing the fw.
Btw things are going superslow because of exams.
![20180906_223536|690x388](upload://a7rdO7dNAxbf0mSEsp2GxmQDx0x.jpg)
```

---
## \#92 Posted by: akira Posted at: 2018-09-07T09:34:15.696Z Reads: 214

```
Hi @fedestanco,
I'd be interested in a PCB if you have one. I have a reflow air gun and I am repairing a second hand reflow oven.
I have already used them but not for esk8 ... (hacked medical devices)
```

---
## \#93 Posted by: fedestanco Posted at: 2018-09-07T12:34:14.640Z Reads: 207

```
Pm me your address. I'll tell you shipping costs.
```

---
## \#94 Posted by: M77 Posted at: 2019-01-05T13:22:28.143Z Reads: 185

```
Hi @fedestanco,

Do you happen to have any bare PCB left? if so I'm interested in 2-4. Interessted to try these out and hava a chat with my friend who is a Hardware Design engineer, they make everything from prototypes to larger productions. Would be interresting to see what they could do for production and pricing of these.
```

---
## \#95 Posted by: linsus Posted at: 2019-01-05T14:11:05.464Z Reads: 178

```
Then you need the designfiles, not the PCB :p
```

---
## \#96 Posted by: M77 Posted at: 2019-01-05T15:43:01.266Z Reads: 176

```
No kidding @linsus  😉 Want to test them out first, haven't asked for the files since I know he won't give them to just anyone and don't think he will without seeing they are build properly and get some valid feedback first.

Was initially going let my friend have a look at the schematic for the VESC 6 and see if he would be interested in doing the layout, but no need if someone else already seems to have done a great job with that.
```

---
## \#97 Posted by: M77 Posted at: 2019-01-05T15:52:23.973Z Reads: 172

```
Oh and to make it clear about my interest in the PCBs @fedestanco since you wrote earlier on you would send    them out for free to people with good reflowing skills, I'm not asking to get free PCBs. If you have any left I'm interested in buying them. 🙂
```

---
## \#98 Posted by: evbkezzz Posted at: 2019-08-05T18:10:25.901Z Reads: 134

```
@fedestanco 
Great work on escalate mate. I am just amazed on how quickly you learnt those things.
I am from a non-electronics background but recently I have had great interests in these things. I am building my own ebike and would like to learn in depth about electronics. 
Can you please share how you went from a noob to building a VESC derivative? Would of great help to me.
How to start, things to do, etc
```

---
## \#99 Posted by: linsus Posted at: 2019-08-05T21:34:16.183Z Reads: 131

```
think he was studying to become an engineer if I'm not misstaken. soo. go to uni for a few years ? :smiley:
Jokes aside, start with installing kicad and do some youtube tutorials. Pick up some books.
```

---
## \#100 Posted by: evbkezzz Posted at: 2019-08-06T09:51:19.321Z Reads: 124

```
Cool! Thanks! Any good recos for books?
```

---
## \#101 Posted by: Jonisonvespa Posted at: 2019-08-06T13:38:00.060Z Reads: 120

```
Hi 
Wonder is this is available open source ? If so can someome please tel, me where i can find it 
Thanks
```

---
## \#102 Posted by: linsus Posted at: 2019-08-06T13:50:56.030Z Reads: 114

```
The entire vesc project is opensource. Except for the layout, for obvious reasons
```

---
## \#103 Posted by: linsus Posted at: 2019-08-06T14:06:31.901Z Reads: 112

```
Depends abit on your level of knowledge. If you truly wish to get a grasp, the fundamentals of electronics are on the heavy side, mathematic wise, it could easly feel overwhelming. So its really hard to recommend some literature without discouraging people xD.

What exactly is it that you want to learn? PCB schematic and layout? Cause the practical use of the CADtools is like MSpaint for grownups, quite easy to learn. If you want to be able to understand and design off your head I'm afraid there are no shortcuts tho. 

I know one book thats pretty good, i cant remember its name tho, Will try find it. Its in english as well. probably what you prefer :smiley:

Edit: "electrical engineering, principles and applications" by Allan R. Hambley is a good one.
Its a monster of a book. But it covers alot.
```

---
## \#104 Posted by: Jonisonvespa Posted at: 2019-08-07T21:07:37.778Z Reads: 96

```
im a hobbist in electronics, i can layout a pcb no problem but unsure if it works?
are there any pcbs available to buy\?
really dont want to dive in and the project doesnt actually work or had bugs in it
```

---
## \#105 Posted by: moon Posted at: 2019-08-07T21:09:58.753Z Reads: 95

```
Please read bro
```

---
## \#106 Posted by: Jonisonvespa Posted at: 2019-08-07T21:17:21.123Z Reads: 97

```
ok is this an exact copy of 
this, if it is then i will build it for sure could someone cofirm this please so all software and circuit diagram is of that below?
https://www.trampaboards.com/vesc-6-plus-benjamin-vedder-electronic-speed-controller-p-26762.html
```

---
## \#107 Posted by: moon Posted at: 2019-08-07T21:22:32.736Z Reads: 97

```
There isn't any PCBs available here
```

---
## \#108 Posted by: Jonisonvespa Posted at: 2019-08-07T21:27:04.923Z Reads: 95

```
ok this guy is selling this vesc?
```

---
## \#109 Posted by: linsus Posted at: 2019-08-08T08:08:24.237Z Reads: 90

```
If you just want something that works, biting the pricetag on the trampa ones are worth it. They're real good on warranty and support as well. Or if you're patient enough there are some new vescs on its way thats abit cheaper.
```

---
## \#110 Posted by: Jonisonvespa Posted at: 2019-08-08T16:06:45.020Z Reads: 75

```
Hi, 
do you mean there is a new one of these comming? i need 2 soonish so could wait
tyhanks
```

---
## \#111 Posted by: linsus Posted at: 2019-08-08T16:31:36.026Z Reads: 75

```
Depends what you mean, the official controller is the VESC over at trampaboards. You can buy em right away if you please. They're in the "high end" cost and quality wise tho so many are reluctant to spend thier hard earned money. I've yet to see anyone dissapointed however. 

The new VESCs are trampa VESCs. Not derivatives.
```

---
## \#112 Posted by: evbkezzz Posted at: 2019-08-16T05:41:21.268Z Reads: 56

```
Hey linsus,
>If you want to be able to understand and design off your head I’m afraid there are no shortcuts tho.

Yeah, that's what I am interested in.
Thanks for the book reco.
```

---
