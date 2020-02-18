# The Saw &#124; R-Spec Drive &#124; 4WD &#124; dual Unity &#124; Haya &#124; 12S4P &#124; 97mm

### Replies: 101 Views: 4742

## \#1 Posted by: Blasto Posted at: 2019-01-17T21:20:51.123Z Reads: 631

```
While i'm waiting for parts, here's the build log.

![image|690x208](upload://9BpKDAj9sYZlTL4bzCkG3jgZ7ur.png) 

Each slot of the Haya will house 12S2P 18650's. All the connections including battery sense wires are done through the pcb. Both packs will have a 40A fuse, the tracks of the pcb are designed for a 30A continuous with a 10 degree temperature rise.

The BMS is discharge circuit is by-passed from the high current path. However, it's discharge circuit can control the Unity switch . Meaning if the BMs detects an undervoltage fault, it is able to shutdown the Unity via the switch.
![image|690x390](upload://5m0ZboKK9Nj6Vo8Mn2b6wGyPhCP.png) 

closer look at all the connectors
![image|690x448](upload://12KLZwVYhjcnzNSuxbkVztGzS3N.png) 

connector for the charge port, with onboard fuse
connector for the bms
input connector for the switch, output connector to the Unity
input connector for the CAN bus, the output connector is alllll the way at the other end of the pcb

![image|330x500](upload://AozLKVQ9y8f2yaeYcP5MfsiDgq.png) 

Another interesting thing with the CAN bus, i've connected both 5V of each Unity together with an inline 5 Ohm resistor, this will allow me to turn on both Unity's with a single switch.

![image|478x222](upload://t4Pt0aQHplt90EBBzTluPjCRGti.png) 

Rear riser pad
![image|690x398](upload://sNw9Atvu7IgT9gTIvk35h8buxrd.jpeg) 

Front riser pad
![image|546x442](upload://o4BhaYCGYsSg1g0o5xDV2ykHm9O.jpeg) 

led display that will be housed inside the front riser
![image|690x216](upload://af9yW0Fqad0zwRdpEDTvSRRPXJO.png) 
![image|690x378](upload://6EGurE9c51fEHTgM2bZrQ0BQoLq.jpeg) 

a little buffer to allow the NanoX's Channel 2 to control battery voltage for a light bar
![image|539x288](upload://ljqnsNorWLJh9EA0W7PsCgiS9Ck.jpeg) 

some real photos
![image|690x136](upload://fGeGzJXoDl2YicPnmmooCrIDno0.jpeg) 

![image|690x239](upload://fqa2tgotAY6TEKk6FtMnFudD8Vs.jpeg) 

![image|364x500](upload://nXa7o9NfWAr4KziQH78EchMo38s.jpeg) 

![image|690x192](upload://311dv0ccJOp32TUmU36JolXVDxF.jpeg) 

some dicking around with tests

light bar test

https://youtu.be/Wc1zAoTLr4w

Can bus test

https://youtu.be/RpobAAIR71o

[garbage BMS used](https://www.ebay.ca/itm/BMS-6S-7S-8S-9S-10S-11S-12S-13S-4-2V-25A-Adjustable-BMS-Lithium-Li-ion-18650-PCM/253959939283?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649)

[Light bar used](https://www.digikey.ca/product-detail/en/seoul-semiconductor-inc/SMJF-LF08C00-XX/897-1233-ND/4696192)
```

---
## \#2 Posted by: Deodand Posted at: 2019-01-17T21:51:18.785Z Reads: 530

```
How will you be integrating the windmill?

How many amps does the light bar draw?
```

---
## \#3 Posted by: Blasto Posted at: 2019-01-17T22:04:12.634Z Reads: 525

```
[quote="Deodand, post:2, topic:81220"]
How will you be integrating the windmill?
[/quote]

beside the beer dispenser
```

---
## \#4 Posted by: ducktaperules Posted at: 2019-01-17T22:14:06.221Z Reads: 512

```
[quote="Blasto, post:1, topic:81220"]
However, it’s discharge circuit can control the Unity switch . Meaning if the BMs detects an undervoltage fault, it is able to shutdown the Unity via the switch.
[/quote]


Thats a dam good idea. I guess even a super cheep low current BMS could be used to do this.

It would be great to have a small pcb that could be put inline with the switch cable that has just this circuitry on it.
```

---
## \#5 Posted by: mynamesmatt Posted at: 2019-01-17T23:11:33.218Z Reads: 479

```
what an awesome bunch of ideas!
```

---
## \#6 Posted by: deucesdown Posted at: 2019-01-18T15:38:32.422Z Reads: 451

```
Only 5 replies. I think everyone is dumbstruck at the awesomeness of this build.
```

---
## \#7 Posted by: iKNOWaFATman Posted at: 2019-01-18T16:04:48.710Z Reads: 451

```
...derrrrrrrrrrrrrr.

.



.



.

 ya basicly
```

---
## \#8 Posted by: Riako Posted at: 2019-01-18T16:09:52.365Z Reads: 431

```
Imprevisse setup and layout !
**I love all the details you put in it !!**
Can't wait to see more, do not hesitate to drown us with photos :blush:

Good DIY :v: ;)
```

---
## \#9 Posted by: iKNOWaFATman Posted at: 2019-01-18T16:32:59.597Z Reads: 408

```
Everyon is giving some cool ideas for this haya. Prayin mine comes in so i can wow you all with my first grader skills on my build.
```

---
## \#10 Posted by: dg798 Posted at: 2019-01-18T17:06:14.676Z Reads: 399

```
Watching!!
10 charc
```

---
## \#11 Posted by: Battosaii Posted at: 2019-01-18T17:12:03.477Z Reads: 395

```
Do you think they will update the UI to show all 4 motors and do all 4 motor detections at the same time.
```

---
## \#12 Posted by: Blasto Posted at: 2019-01-18T18:04:18.739Z Reads: 386

```
not in the next release that is for sure
```

---
## \#13 Posted by: guigui Posted at: 2019-01-18T18:16:33.719Z Reads: 377

```
Awesome ideas here ! Curious to see how it's gonna turn out
```

---
## \#14 Posted by: PickSix24 Posted at: 2019-01-18T18:30:19.241Z Reads: 380

```
Took me awhile to pick my jaw off the floor. 
Really nice stuff happening here 👍🏻
```

---
## \#15 Posted by: totalgeek9224 Posted at: 2019-01-18T18:37:17.757Z Reads: 394

```
Yeah no kidding @Blasto
I mean with all the HAYA builds going on here (like @sofu's S3 or @banjaxxed hummie HAYA) i really want a a HAYA too! 
This build is absolutely crazy, and I can't wait to see it when it's done!
Definitely bookmarked!
```

---
## \#16 Posted by: Blasto Posted at: 2019-01-22T03:25:25.484Z Reads: 426

```
While the silicone cures

Voltage led display installed, with little pin holes

Whats really cool, you can’t see the holes when the leds are off

There’s 5 holes, 2 of them are through the grip

![image|375x500](upload://o1mGMLGCMv9ouVGhcb94y6Qk94h.jpeg) 

![image|375x500](upload://bI9kx1D74BPwabigwYZjNC6pcqH.jpeg) ![image|666x500](upload://zLSDtOaMuaH6gEHnYSwWGaa6jUl.jpeg) 

Led strips glued and curring

![image|666x500](upload://jsLgZOSD8Mk46wLapgQDxiuVGTS.jpeg) 

Now i wait
```

---
## \#17 Posted by: briman05 Posted at: 2019-01-22T03:35:10.914Z Reads: 395

```
The power button on the riser? Looks cool are you going to route a slot for the wires.
```

---
## \#18 Posted by: Blasto Posted at: 2019-01-22T03:40:18.348Z Reads: 422

```
I had to sharpen a pencil the other day, had a hell of time... it’s then i realized my wood working skills suck.

So i 3d printed some risers with a little gap for me access the deck openings

![image|375x500](upload://dOD9nQTnUngjKY1WlNkP51pUjOc.jpeg) ![image|375x500](upload://dw9UuHFyjkL7PvO0DfzAm4gQyZd.jpeg)
```

---
## \#19 Posted by: Pedrodemio Posted at: 2019-01-22T18:59:31.134Z Reads: 408

```
Well done @Blasto , the PCB idea is really great, did you find somewhere that make these large boards cheap?

And looking forward to see what effect the under board lights give, lots of times I thought about incorporating a light strip embedded on the bottom in a channel filled with epoxy, but is was too much work, you may change my mind
```

---
## \#20 Posted by: Blasto Posted at: 2019-01-22T19:09:42.049Z Reads: 409

```
Yeah i got the pcb from pcbway, a little over 300$ for 10 pieces ship incl. Pretty dam cheap for a pcb that size.

I should be able to test the leds on the deck by the end of the week, i'll have to admit i'm a bit afraid that the thickness of the deck will collimate the light and not get the wanted spread... but whatever, we're having fun aren't we?
```

---
## \#21 Posted by: Pedrodemio Posted at: 2019-01-22T19:17:31.296Z Reads: 392

```
That's basically free

You could fill the hole with epoxy and sand it to get a frosted look that would diffuse the light

I was looking at the specs of the light bar, it is powered directly by the battery? That's one road block I stumped on mine, using a 60 led/m strip I would need another DC/DC converter just for the leds
```

---
## \#22 Posted by: Blasto Posted at: 2019-01-22T19:26:16.907Z Reads: 392

```
[Light bar used](https://www.digikey.ca/product-detail/en/seoul-semiconductor-inc/SMJF-LF08C00-XX/897-1233-ND/4696192) , directly battery powered, the foward voltage of the strip is 48V (measured with DMM) the lights become dim as hell when around 41-40V... but for the simplicity of the circuit, i did not care. I've also added a little 15ohm 4W ballast resistor for when the battery are fully charged (50.2V)

I was contemplating on reworking the LED strip in to a 24V operational voltage, normally it's 8 LED in series, i would have changed it up to 4 // 4. But didn't do that, just used as is.

now that I think about it... I should just of  removed one LED out of the circuit, making the forward voltage 42V, that would have covered my entire voltage span with minimal dimming....  oh well, already made 8 holes, not going back
```

---
## \#23 Posted by: deucesdown Posted at: 2019-01-22T20:38:21.056Z Reads: 372

```
[quote="Blasto, post:20, topic:81220"]
10 pieces
[/quote]

Wait did you just say you did a group buy for these giant-ass pcb? :)
```

---
## \#24 Posted by: barajabali Posted at: 2019-01-22T21:52:03.461Z Reads: 353

```
Awesome work dude. So 2 BMS's? one for each side? 

Where can we get those PCBS.... ;)
```

---
## \#25 Posted by: ducktaperules Posted at: 2019-01-22T22:12:56.710Z Reads: 356

```
I been using PCBway recently and i must say that i have been impressed with both quality and turn around time.

a few questions . . . 
what thickness copper did you go with for these boards?

have you used these cheep BMS before?
are they any good?

in your system do the 2 sides run interdependent? is the main power from one half connected to the other?
```

---
## \#26 Posted by: Blasto Posted at: 2019-01-22T22:24:44.548Z Reads: 349

```
2 oz copper, no i haven't used this bms before, i am already a bit disappointed by it, it has no balance circuit... oh well it will be good for charging and cell monitoring

yes i was planning on paralleling up the two 12S2P packs, that way i can use only one charge port... but i could just has easily run them independently, but would require 2 charge ports.
```

---
## \#27 Posted by: Pedrodemio Posted at: 2019-01-22T22:28:31.092Z Reads: 344

```
What about one charge port but connected to each battery with a diode? This way they will still be isolated and no current will flow between them, using a 0.3v drop diode should be no problem
```

---
## \#28 Posted by: ducktaperules Posted at: 2019-01-22T22:41:05.165Z Reads: 350

```
i will be interested to see how this works out. I have a similar setup in my build where i have a 12s battery pack in an enclosure and i have 3 of them in parallel. in my last build i had to join all the balance points between all of the different packs and one big bms, but it means lots of cables between separate enclosures. I had been considering separate bms in each enclosure and just running power and charge to each enclosure but was concerned that something weird might happen.

im this close |------| to trying to make my own bms. but i already have so many projects on the go :frowning:
```

---
## \#29 Posted by: Blasto Posted at: 2019-01-23T15:57:14.715Z Reads: 339

```
[quote="ducktaperules, post:28, topic:81220"]
im this close |------| to trying to make my own bms. but i already have so many projects on the go
[/quote]

do it, make a de-featured version of the DiebieMS,  no need for high discharge, cell balance + monitoring, CAN communication, LCD port, Unity switch control, charge control. would be dope.
```

---
## \#30 Posted by: ducktaperules Posted at: 2019-01-23T16:04:09.499Z Reads: 329

```
yeah this is exactly what i was thinking.
```

---
## \#31 Posted by: Blasto Posted at: 2019-01-23T16:06:30.545Z Reads: 363

```
[quote="Pedrodemio, post:27, topic:81220, full:true"]
What about one charge port but connected to each battery with a diode? This way they will still be isolated and no current will flow between them, using a 0.3v drop diode should be no problem
[/quote]

Yeah that should work, only problem is it would charge the battery to around 49.9V

![image|375x500](upload://ZCDqjkGzPKSnxoGu386EghydiR.jpeg)
```

---
## \#32 Posted by: hazza Posted at: 2019-01-23T16:10:03.230Z Reads: 332

```
Hey there, awesome build. I am wondering how much amperage you plan to put through the hubs?
```

---
## \#33 Posted by: Blasto Posted at: 2019-01-23T16:14:02.613Z Reads: 359

```
This is the nomenclature i went for

![image|375x500](upload://3yllE528WVQW8qypulStpQ6KnlZ.jpeg) 

[quote="hazza, post:32, topic:81220"]
I am wondering how much amperage you plan to put through the hubs?
[/quote]

Probably 60A motor and 30A batt
```

---
## \#34 Posted by: hazza Posted at: 2019-01-23T16:15:35.034Z Reads: 333

```
when do you think you will have it running? will you do any videos of it?
```

---
## \#35 Posted by: akhlut Posted at: 2019-01-23T16:18:49.635Z Reads: 336

```
Go 16s pls if possible.
```

---
## \#36 Posted by: Blasto Posted at: 2019-01-23T16:19:17.092Z Reads: 361

```
i should be done in a few weeks, still waiting for parts...

won't be able to ride it until a few months

![image|690x412](upload://tTGNjX8ls4B4lShjtoeyuoaoSRc.jpeg)
```

---
## \#37 Posted by: Blasto Posted at: 2019-01-31T04:07:53.597Z Reads: 365

```
Led array, 5 leds all good, 1 led no good

![image|375x500](upload://uTo88FrHaWtZl5kk71NEdOXwlzW.jpeg) ![image|375x500](upload://y6Le8nTBVSSVgQaVs8BPVbs9Gp9.jpeg)
![image|375x500](upload://fFciLUseU1VNdBakUADmfkts66C.jpeg)
```

---
## \#38 Posted by: Blasto Posted at: 2019-02-07T03:05:31.775Z Reads: 363

```
Hubz are in, #12 suiting up

![image|375x500](upload://v1f4bnxzrv7gVl78zTbiLkESKzS.jpeg) ![image|375x500](upload://oCCZNfQO7fr91gYL35K97y4KDqv.jpeg)

![image|375x500](upload://kNyLtcz5yAUCo7RSPNf3yGowRRD.jpeg) ![image|375x500](upload://d8fl3M9u5465vgV8qe3ETxg6Ldt.jpeg)

![image|666x500](upload://iuVzH8guMLUfyishnk5UFxTIDG0.jpeg) ![image|666x500](upload://1WDa1vUGFxbSxZ6M7lpMJuANUUe.jpeg)

![image|666x500](upload://yB6hemSDyqkR4MdBDHj0v1J8iXl.jpeg)
```

---
## \#39 Posted by: mishrasubhransu Posted at: 2019-02-07T04:29:38.341Z Reads: 342

```
oooooh! the connectors, minimum wiring, repeatable setup is my kinda porn.
```

---
## \#40 Posted by: Blasto Posted at: 2019-02-07T04:34:38.992Z Reads: 352

```
Testing the leds... fuck my retina. Technical note, these strips pull 200mA each @50V

![image|375x500](upload://6JrfaDlxXkNNC5k5MZdErQHd3Uw.jpeg) ![image|666x500](upload://j7LuwgOKyZRiXM1SEbj0B9yEpej.jpeg) ![image|375x500](upload://g5yrdk700T7eGJOGqopjqlyhjCV.jpeg) ![image|666x500](upload://hb4BSJOp8X6aHoyC5hQwL8ozurm.jpeg)
```

---
## \#41 Posted by: Komamtb Posted at: 2019-02-07T06:04:19.466Z Reads: 337

```
It's like a house lamp, really great build, what range are you expecting?
```

---
## \#42 Posted by: Blasto Posted at: 2019-02-07T06:14:11.212Z Reads: 341

```
[quote="Komamtb, post:41, topic:81220"]
what range are you expecting?
[/quote]

If i’d had to guess, around 25km. 12s4p 30q cells
```

---
## \#43 Posted by: neiru37 Posted at: 2019-02-07T06:48:50.440Z Reads: 341

```
[quote="Blasto, post:42, topic:81220"]
around 25km
[/quote]

Heh. These hubs really are power hungry. And here I thought I was gonna get good range with my first ever thane build, but it consumes more energy at 33-38wh/mi than my trampa build at 22-25wh/mi
```

---
## \#44 Posted by: Winfly Posted at: 2019-02-07T06:50:41.819Z Reads: 335

```
yup. I did a good 46Wh/mile going up twin peak. lmao. and ~28-30Wh/mile on mostly flat in stop and go traffic.. they ride good but not efficient at all.
```

---
## \#45 Posted by: neiru37 Posted at: 2019-02-07T06:52:56.715Z Reads: 338

```
[quote="Winfly, post:44, topic:81220"]
twin peak.
[/quote]

How's your motor Temps?
```

---
## \#46 Posted by: Winfly Posted at: 2019-02-07T06:55:04.936Z Reads: 334

```
haven't check it yet but I just got batteries for my IR temp gun. the beta value for the thermistor was definitely wrong. and thermal throttles way before it's necessary. I dont think heat is an issue now but it would be nice if I tune the beta value.
```

---
## \#47 Posted by: neiru37 Posted at: 2019-02-07T06:56:03.925Z Reads: 327

```
You have a metr, that logs motor temp.
```

---
## \#48 Posted by: banjaxxed Posted at: 2019-02-07T09:54:23.131Z Reads: 325

```
Hurry up, enertion comp potential
```

---
## \#49 Posted by: bevilacqua Posted at: 2019-02-07T10:32:30.042Z Reads: 335

```
![image|290x174](upload://aiv4PZPA8QFmdZZhocKzRSmUvH4.jpeg)
```

---
## \#50 Posted by: banjaxxed Posted at: 2019-02-07T12:24:04.419Z Reads: 328

```
For sure @Andy87 will be tampering with the voting
```

---
## \#51 Posted by: Blasto Posted at: 2019-02-07T16:11:18.490Z Reads: 335

```
[quote="banjaxxed, post:48, topic:81220, full:true"]
Hurry up, enertion comp potential
[/quote]

sadly don't think i am aloud to participate. 

this build should be done by next week, just need to spot weld some tabs on the batteries then solder them on the pcb.
```

---
## \#52 Posted by: Blasto Posted at: 2019-02-27T04:58:43.961Z Reads: 329

```
Cells spot welded and installed, silicone applied waiting for it to cure for the final install

![image|690x297](upload://ljU68sgW8aW2skWr3mYH12u4lYH.jpeg)
```

---
## \#53 Posted by: Grozniy Posted at: 2019-02-27T07:13:35.289Z Reads: 325

```
Beautiful @Blasto , this has to  win the contest
```

---
## \#54 Posted by: Pedrodemio Posted at: 2019-02-28T00:52:51.250Z Reads: 316

```
Looks really tidy, well done

Have a bottom view? Nickel spot welded to the cell and soldered to the PCB or also spot welded?
```

---
## \#55 Posted by: M.Hboards Posted at: 2019-03-01T02:07:43.026Z Reads: 309

```
Hey @Blasto firstly great build. Secondly can you explain how you got the leds hook up to the nanox's second channel.
```

---
## \#56 Posted by: Mikenopolis Posted at: 2019-03-01T03:49:29.304Z Reads: 306

```
This is so beautiful. Now add in a fog making machines and you'll be set!
```

---
## \#57 Posted by: lrdesigns Posted at: 2019-03-01T04:32:28.943Z Reads: 305

```
This build is too cool. Just be sitting around here waiting for more photos. :sunglasses::beers:
```

---
## \#58 Posted by: Indiangummy Posted at: 2019-03-01T21:40:00.718Z Reads: 301

```
@Blasto would you mind sharing the .stl for the riser? 😁
```

---
## \#59 Posted by: Blasto Posted at: 2019-03-06T16:29:14.862Z Reads: 307

```
I’m out of town for the moment, snaped this before leaving. Soldered the tabs to the pcb, in hindsight should have spot welded instead for a cleaner job

![image|666x500](upload://pJsoWGDvQ3ydA0WANB4L64ns3uv.jpeg) 

[quote="M.Hboards, post:55, topic:81220"]
Secondly can you explain how you got the leds hooke up to the nanox’s second channel.
[/quote]

Yeah i’ll post the schematic when i get back, basically i just optocoupled the output of channel 2 to be able to control battery voltage.


[quote="Indiangummy, post:58, topic:81220"]
would you mind sharing the .stl for the riser?
[/quote]

Yeah i guess, didnt put much effort in to it tbh. I feel with the risers it is a tad to high, but it was the minimum height to fit the on-off switch and charge port
```

---
## \#60 Posted by: StefanMe Posted at: 2019-03-06T18:52:42.824Z Reads: 292

```
Can u spotweld to an PCB? Never thought about that...
```

---
## \#61 Posted by: Blasto Posted at: 2019-03-11T00:32:15.812Z Reads: 294

```
[quote="StefanMe, post:60, topic:81220, full:true"]
Can u spotweld to an PCB? Never thought about that…
[/quote]


yeah you can, need to adjust your spot welder settings and make sure the pcb is able to handle the current, but it can be done.

[quote="M.Hboards, post:55, topic:81220"]
Secondly can you explain how you got the leds hook up to the nanox’s second channel.
[/quote]

![image|690x423](upload://vxFDoZTivmL2LuMOj5m5XPkevix.png)  

second channel is driving an opto-coupler, on the nano-x the channel 2 is toggled by holding down the button near the pinky finger for 5 seconds.

i took the receiver out of it's enclosure and directly soldered it to the pcb, reason why i added another output for channel 1. the pcb is the same size as the receiver

![image|585x308](upload://1tvnGDl2ccRENBhfHcr2gO1xkrk.png) '
![image|690x344](upload://pstY9GTkIznGGgrgmeK7Y3JYl93.png) 
![image|510x316](upload://nx9Clr1jovpUQrEcOs1UPFy5xhr.png) 

@Indiangummy [Riser files for haya](https://www.dropbox.com/sh/cqc47vf8zudspnq/AAAN-H0OJEyo6zMwW-kWdP8ia?dl=0)
```

---
## \#62 Posted by: Indiangummy Posted at: 2019-03-11T03:22:14.720Z Reads: 282

```
Thanks a bunch for the file man!
```

---
## \#63 Posted by: Blasto Posted at: 2019-03-12T02:20:44.557Z Reads: 281

```
Live update, this thing will be done by the end of the night

![image|375x500](upload://yjGDXEu9iWD7Xf1QWIR4gdYL0OP.jpeg)
```

---
## \#65 Posted by: AlanZhou Posted at: 2019-03-12T02:26:02.424Z Reads: 275

```
NVM don't flame me
```

---
## \#66 Posted by: Pedrodemio Posted at: 2019-03-12T02:26:39.399Z Reads: 279

```
Then please post some videos by the end of the night :grin:

A indoor 4WD drive burnout is perfect

Now  seriously, I'm really looking forward to some telemetry data, to see  if the consumption is better with 4 hubs, probably not, only if you halve the current to each
```

---
## \#67 Posted by: Blasto Posted at: 2019-03-12T02:29:04.247Z Reads: 282

```
Lol some turd box bms... didnt noticed it did not have a balance circuit, i rode with it anyways
```

---
## \#68 Posted by: AlanZhou Posted at: 2019-03-12T02:30:48.789Z Reads: 297

```
Haha I was woundering why a 13s bms was so small, wish bestech could make a 12s version of the d124 albiet a bit wider for two extra resistors and components
```

---
## \#69 Posted by: Blasto Posted at: 2019-03-12T03:50:18.311Z Reads: 299

```
Fuck ya boys

https://youtu.be/utyouE4lrrM
```

---
## \#70 Posted by: Riako Posted at: 2019-03-12T04:11:30.095Z Reads: 295

```
**Awesome!** ... what else to say ^^ 

:+1:
```

---
## \#71 Posted by: lrdesigns Posted at: 2019-03-12T04:47:53.829Z Reads: 289

```
:ok_hand::ok_hand::+1::+1::fist_right::fist_left::metal::metal::metal::metal::metal::call_me_hand: awesome :skateboard:
```

---
## \#72 Posted by: skatardude10 Posted at: 2019-03-12T07:08:20.763Z Reads: 278

```
I think a yeet is appropriate right now. 

_in a high screetching pitch..._

**_YEEET!!!!!_**
```

---
## \#73 Posted by: akhlut Posted at: 2019-03-12T08:35:25.611Z Reads: 272

```
Fuck yeah!  

Has snow melted enough to test ride?
```

---
## \#74 Posted by: will_manners Posted at: 2019-03-12T10:24:15.066Z Reads: 270

```
![images%20(7)|295x340](upload://vLoS80n3uakTOg28iZCGcv7qHz0.jpeg)
```

---
## \#75 Posted by: epss4 Posted at: 2019-03-12T12:57:13.321Z Reads: 267

```
Congrats!!!
```

---
## \#76 Posted by: City-Blade-101 Posted at: 2019-03-12T13:14:48.225Z Reads: 264

```
![signal-2018-12-13-203104|200x110](upload://vJTjXilVgAfr1kopzbxzXyGCUxX.gif)
```

---
## \#77 Posted by: Battosaii Posted at: 2019-03-12T13:36:58.349Z Reads: 261

```
How did you get the shut down to work under can?

Is there a custom firmware?
```

---
## \#78 Posted by: Blasto Posted at: 2019-03-12T14:39:50.299Z Reads: 263

```
yeah @Deodand sent me a test version, CAN shutdown will be part of the next official fw release. Let me know if you need it now.

[quote="akhlut, post:73, topic:81220"]
Has snow melted enough to test ride?
[/quote]

sadly no, been dicking around in the shop, the thing has power. bit too much for my style.
```

---
## \#79 Posted by: Battosaii Posted at: 2019-03-12T14:51:34.341Z Reads: 254

```
Thank you I'll need it soon cause my second unity is about to ship next week according to enertion lol
```

---
## \#80 Posted by: Sn4pz Posted at: 2019-03-12T15:03:10.737Z Reads: 256

```
I know it was said last time, but you Canadians have some great natural commentary.... Just like AvE 😂😂
```

---
## \#81 Posted by: Blasto Posted at: 2019-03-12T15:07:38.095Z Reads: 258

```
i'm highly inspired by AvE lol

tried doing videos without a proper introduction.... doesn't feel right
```

---
## \#82 Posted by: akhlut Posted at: 2019-03-12T15:07:44.141Z Reads: 257

```
A treat e'special!
```

---
## \#83 Posted by: mmaner Posted at: 2019-03-12T15:48:37.091Z Reads: 257

```
SICK!  What's traction control like with thane and 4wd?
```

---
## \#84 Posted by: gmurad Posted at: 2019-03-31T01:37:56.792Z Reads: 238

```
Any new update videos, pictures or anything? Snow is clearing here in my area!
```

---
## \#85 Posted by: neiru37 Posted at: 2019-03-31T02:34:34.135Z Reads: 238

```
+1 curious about your motor temps and wh/mi consumption. I just did a twin peaks run (tallest point in SF) and I had to stop twice to let my hubs cool down. I was really considering doing 4wd so I can (theoretically) split the heat.
```

---
## \#86 Posted by: bevilacqua Posted at: 2019-03-31T21:04:51.045Z Reads: 234

```
Since the losses are proportional to the square of the current (which would be halved), the motor-temp would improve quite a bit. 

In theory also the wh/km, but I'm not so sure in that regard, as there are some more factors to take into account when calculating energy consumption.
```

---
## \#87 Posted by: Pedrodemio Posted at: 2019-03-31T21:18:31.064Z Reads: 234

```
the big problem is restraining yourself to not use all the power it have all the time :grinning:
```

---
## \#88 Posted by: bevilacqua Posted at: 2019-03-31T21:21:09.697Z Reads: 235

```
indeed, range anxiety is a real issue :smile:
```

---
## \#89 Posted by: Blasto Posted at: 2019-03-31T22:04:23.348Z Reads: 233

```
Soon enough i’ll be able to try it out. The roads are still covered in gravel and dog shit
```

---
## \#90 Posted by: mikenyc Posted at: 2019-04-01T18:53:28.673Z Reads: 221

```
mmmm canada.
```

---
## \#91 Posted by: JohnnyMeduse Posted at: 2019-04-01T19:13:32.011Z Reads: 219

```
OOOOO Canada :kissing_heart:
```

---
## \#92 Posted by: sharky Posted at: 2019-04-01T19:46:13.889Z Reads: 221

```
What a monster and so clean👍👍
```

---
## \#93 Posted by: mattyB Posted at: 2019-04-12T12:02:51.156Z Reads: 218

```
how did you do the battery percentage indicator with the leds? sorry im a noob
```

---
## \#94 Posted by: Blasto Posted at: 2019-04-13T17:58:02.694Z Reads: 224

```
Quick PSA for those wanting todo the same 4wd topology (via CAN, connecting both 5V supplies with inline resistor)

The little 5ohm resistor was too small of a value, i now cranked that value up to 20-25 ohm

![image|690x248](upload://gNw6NqmoRzl5kijcJJcJSbZ6q74.jpeg)

Also @Deodand should be releasing the official fw cery soon with the CAN shutdown command 

@mackann
@Battosaii
```

---
## \#95 Posted by: Battosaii Posted at: 2019-04-13T18:41:39.097Z Reads: 220

```
Thanks i was about to order the resistors now, ill order a variety pack just incase lol
```

---
## \#96 Posted by: Blasto Posted at: 2019-04-13T19:26:56.070Z Reads: 216

```
Ok i get it now, this 4wd thing is fun... OVP but fun
```

---
## \#97 Posted by: Battosaii Posted at: 2019-04-13T19:39:24.680Z Reads: 216

```
Ovp maybe even for my fat ass i may have to agree but its fun to blast by a skinny guy going full throttle on anyboard lol
```

---
## \#99 Posted by: neiru37 Posted at: 2019-05-19T07:34:56.017Z Reads: 184

```
Have you ridden this thing yet @Blasto?
```

---
## \#100 Posted by: Winfly Posted at: 2019-05-22T18:17:23.826Z Reads: 161

```
[quote="neiru37, post:85, topic:81220"]
I was really considering doing 4wd so I can (theoretically) split the heat.
[/quote]

@neiru37 you can still do 4WD if you buy mine $350
```

---
## \#101 Posted by: neiru37 Posted at: 2019-05-22T18:28:28.966Z Reads: 161

```
[quote="Winfly, post:100, topic:81220"]
$350
[/quote]

At that price I expect it to come with 10 free bubble teas
```

---
## \#102 Posted by: WAVMOB Posted at: 2019-07-27T15:58:20.806Z Reads: 103

```
Do you plan to sale this build?
Any interest in building a small batch for motivated riders?
```

---
## \#103 Posted by: Blasto Posted at: 2019-07-27T17:47:37.681Z Reads: 96

```
Nah no plans on selling this, i’m having enough fun
```

---
