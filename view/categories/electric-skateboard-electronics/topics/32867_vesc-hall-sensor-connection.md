# VESC Hall Sensor Connection

### Replies: 76 Views: 6287

## \#1 Posted by: darkkevind Posted at: 2017-09-11T13:43:46.566Z Reads: 504

```
Guys, this may be a silly question, but my sensor connector from my motor doesn't fit either of the connectors on my VESC. Am I missing something?

<img src="/uploads/db1493/original/3X/3/8/38abe23d591ffb45876637a122b0deeb2acc0a34.jpg" width="690" height="388">
```

---
## \#2 Posted by: krloz Posted at: 2017-09-11T13:53:08.227Z Reads: 478

```
Yep. An adapter.
Search for hall sensor adapter in the forum and see if you find yours.  Or an alternative
```

---
## \#3 Posted by: darkkevind Posted at: 2017-09-11T14:04:34.268Z Reads: 473

```
Thanks. Does it go in P1 or P2?
```

---
## \#4 Posted by: krloz Posted at: 2017-09-11T14:18:58.698Z Reads: 476

```
I'm not sure but it looks like your vesc follows this layout. 
https://www.google.es/search?q=vesc+4.12+pinout&client=ms-android-samsung&prmd=isvn&source=lnms&tbm=isch&sa=X&ved=0ahUKEwiDsLirqZ3WAhXI0hoKHQvTDDMQ_AUICSgB&biw=412&bih=652&dpr=2.63#imgrc=6youe0OuS13MoM:
Sorry mine are another layout so i can only guess
```

---
## \#5 Posted by: krloz Posted at: 2017-09-11T14:20:43.875Z Reads: 466

```
Maybe This also helps
https://www.electric-skateboard.builders/t/hall-sensors-5-wires-vs-6-wires/31626/17
```

---
## \#6 Posted by: darkkevind Posted at: 2017-09-11T14:26:24.439Z Reads: 454

```
Yes it does, thank you, that helps. It's P1
```

---
## \#7 Posted by: mmaner Posted at: 2017-09-11T16:27:30.246Z Reads: 437

```
https://psychotiller.com/product/sensor-wire-adaptor
```

---
## \#8 Posted by: bigben Posted at: 2017-09-11T16:39:53.996Z Reads: 419

```
I ended up buying some plugs with flyleads and soldering the new leads to the old ones and heat shrinking them.
Something like this.
http://www.ebay.co.uk/itm/5-Sets-JST-PH-2-0mm-6-Pin-Male-Female-Connector-Plug-Wires-Cables-300mm-/292037564597?hash=item43fecb98b5
```

---
## \#9 Posted by: darkkevind Posted at: 2017-09-11T16:49:34.157Z Reads: 388

```
Thanks man but I'm not sure about the £23 shipping! :scream:
```

---
## \#10 Posted by: darkkevind Posted at: 2017-09-11T16:50:53.688Z Reads: 377

```
Cheers mate, I'll grab this.

What about the wires though? I understand Gnd & 5v are at each end, but do we just miss out the temperature sensor wire and wire up the blue, white & yellow?
```

---
## \#11 Posted by: mmaner Posted at: 2017-09-11T16:52:07.288Z Reads: 365

```
Just as an example.

I would buy some of these and make your own...

MOTOR SIDE  >>  JST-ZH 6 pin 1.5mm pitch
VESC SIDE   >>  JST-PH 6 pin 2.0mm pitch
```

---
## \#12 Posted by: bigben Posted at: 2017-09-11T17:01:28.280Z Reads: 344

```
Yep, for the racerstar motors on my build there is no temperature wire so I missed it out.
```

---
## \#13 Posted by: darkkevind Posted at: 2017-09-11T17:26:49.774Z Reads: 338

```
Yeah this is a racestar. This build is for my son, I haven't even got sensors on MY build! :confused:
```

---
## \#14 Posted by: scepterr Posted at: 2017-09-11T17:33:47.506Z Reads: 331

```
Is C37 missing for a reason?
Btw I don't bother with adapters just snip and solder on the wires from the correct plug
```

---
## \#15 Posted by: bigben Posted at: 2017-09-11T17:50:38.986Z Reads: 322

```
Strangely I'm doing another build for the kids now. Waiting on parts but using the 270kv motor and FVT120 esc and 6s. Cheeeeeeep
```

---
## \#16 Posted by: ShutterShock Posted at: 2017-09-11T17:53:23.480Z Reads: 318

```
I got the JST connector for it and just spliced it with the motor sensor wires, both on ebay for only a few bucks.
```

---
## \#17 Posted by: scepterr Posted at: 2017-09-11T17:53:50.707Z Reads: 319

```
Don't wanna take this off topic, but IMO the perfect low cost kid setup has to be the ego2 rear truck/motor(160kv) assembly, it's $30 and comes with everything minus wheels and gear for wheel. Indestructible covers on motor and belt. 90mm wheel set with gear installed is $40. 
<img src="/uploads/db1493/original/3X/b/b/bb3079658717200e50591e9adae4d2f6b23f6454.jpg" width="375" height="499">
```

---
## \#18 Posted by: darkkevind Posted at: 2017-09-11T18:20:53.720Z Reads: 300

```
This is an inferior VESC from somewhere unknown, I bought it second hand from someone here on the forum, before I find out it was inferior (of course) and then had to buy another one!

I've already replaced a couple of caps, which one is c37 then?

I'm using this because it's quite underpowered, perfect for my son... Lol
```

---
## \#19 Posted by: darkkevind Posted at: 2017-09-11T18:21:27.991Z Reads: 292

```
That's what I'll probably do :thumbsup:
```

---
## \#20 Posted by: scepterr Posted at: 2017-09-11T18:25:37.668Z Reads: 296

```
<img src="/uploads/db1493/original/3X/f/9/f9c499a3e7e6475fd4b5c5bf1cd9f16c02cd319e.jpg" width="690" height="388">
```

---
## \#21 Posted by: darkkevind Posted at: 2017-09-11T18:28:00.778Z Reads: 280

```
Thanks. What is it responsible for then? Looks like a big one. Would it be that that's making it under powered you think?
You know where I could get one? Rs-components?

Cheers
```

---
## \#22 Posted by: scepterr Posted at: 2017-09-11T18:31:28.440Z Reads: 273

```
I'm surprised it works without it, is c51 on there? They're the same component. You can put 4.7/10/22uf 100V 2220 cap there. 22uf is best if you can get it or stack the others if that's all you can get. Also if you any dead vescs you can take it off c37/c51 on there
```

---
## \#23 Posted by: darkkevind Posted at: 2017-09-11T18:52:05.271Z Reads: 261

```
Where would C51 be!? :confused:

I've already added C44 & C49 because they were missing :(
```

---
## \#24 Posted by: scepterr Posted at: 2017-09-11T18:52:59.700Z Reads: 258

```
It's on the other side, above shunt
```

---
## \#25 Posted by: darkkevind Posted at: 2017-09-11T18:58:41.803Z Reads: 261

```
Not sure what 'shunt' is...

<img src="/uploads/db1493/original/3X/9/0/90222c984795179aab5547f5d292c92c643617a6.jpg" width="690" height="388">
```

---
## \#26 Posted by: scepterr Posted at: 2017-09-11T19:02:42.658Z Reads: 251

```
<img src="/uploads/db1493/original/3X/d/2/d282c4df814492c09930dc83862b1daa06ab02d2.jpg" width="690" height="388">
```

---
## \#27 Posted by: darkkevind Posted at: 2017-09-11T19:04:19.279Z Reads: 241

```
Ah! C51 was one of the ones I had to add in myself :confused:

It was a while ago, I'd forgotten what reference it had.

Well, I guess I'll get a C37 and put it on there, can't hurt can it?
```

---
## \#28 Posted by: scepterr Posted at: 2017-09-11T19:04:58.092Z Reads: 242

```
Hurt, no, help, yes lol
Add c14 too if you have it
```

---
## \#29 Posted by: darkkevind Posted at: 2017-09-11T19:05:27.857Z Reads: 237

```
lol. So is C37 the same as C51?
```

---
## \#30 Posted by: scepterr Posted at: 2017-09-11T19:05:39.229Z Reads: 232

```
Yeah it's the same part
```

---
## \#31 Posted by: darkkevind Posted at: 2017-09-11T19:06:16.185Z Reads: 229

```
OK cool. I'll just order the same as I got last time then.

What's this c14? Another one missing?
```

---
## \#32 Posted by: scepterr Posted at: 2017-09-11T19:06:55.526Z Reads: 227

```
Yeah c14 tends be left off cheap vescs, it's not required but helps. I may be mistaken but I think that was one the changes between 4.10 and 4.12, adding c14. 
It's between the red and black wire
```

---
## \#33 Posted by: darkkevind Posted at: 2017-09-11T19:08:44.057Z Reads: 220

```
OK, I'll get it and add it then. Cheers!

This has 4.12 stamped on the PCB. I wonder what happened to it? Maybe it was just someone's test VESC? lol
```

---
## \#34 Posted by: scepterr Posted at: 2017-09-11T19:09:37.232Z Reads: 203

```
Looks like somebody took 2 broken ones and made  1 working lol
```

---
## \#35 Posted by: darkkevind Posted at: 2017-09-11T19:10:51.151Z Reads: 208

```
Yeah you could be spot on there...

Which one out of these should I choose? I can't find my last order :frowning:

http://uk.rs-online.com/web/c/passive-components/capacitors/ceramic-multilayer-capacitors/?searchTerm=22uf
```

---
## \#36 Posted by: scepterr Posted at: 2017-09-11T19:13:14.155Z Reads: 209

```
https://uk.rs-online.com/mobile/p/ceramic-multilayer-capacitors/9163197/
```

---
## \#37 Posted by: darkkevind Posted at: 2017-09-11T19:16:02.964Z Reads: 216

```
What's the difference between these two?

http://uk.rs-online.com/web/p/ceramic-multilayer-capacitors/9163197/

http://uk.rs-online.com/web/p/ceramic-multilayer-capacitors/7883105/
```

---
## \#38 Posted by: scepterr Posted at: 2017-09-11T19:19:00.791Z Reads: 205

```
Not exactly sure, I think they use different materials. 
I haven't seen the 2nd one used in any vescs
```

---
## \#39 Posted by: darkkevind Posted at: 2017-09-11T19:21:09.917Z Reads: 207

```
I'll get the one you linked to. What about C14, is that the same component?
```

---
## \#40 Posted by: scepterr Posted at: 2017-09-11T19:29:12.843Z Reads: 208

```
Standard is 2.2uf 16v upgraded is 4.7uf 16v smd0603
All the 2.2uf caps can be upgraded to 4.7uf if you feel like it
```

---
## \#41 Posted by: darkkevind Posted at: 2017-09-11T19:32:52.238Z Reads: 169

```
I just found where I got C51 from...

https://www.arrow.com/en/products/ckg57kx7s2a156m335jh/tdk

So this one you linked to on rs-components, I can get two of those for C37 and C14?
```

---
## \#42 Posted by: scepterr Posted at: 2017-09-11T19:33:53.768Z Reads: 157

```
C14 is completely different
It's fine for c37/c51
```

---
## \#43 Posted by: darkkevind Posted at: 2017-09-11T19:35:26.058Z Reads: 159

```
Oh! 

Couldn't trouble you for a link could I please?

Is this one alright? http://uk.rs-online.com/web/p/ceramic-multilayer-capacitors/9159145/
```

---
## \#44 Posted by: scepterr Posted at: 2017-09-11T19:36:55.860Z Reads: 161

```
Yeah that's fine
I would definitely stock up on the c37/c51, they're pricey but cheaper than ordering and shipping 2 at a time
```

---
## \#45 Posted by: darkkevind Posted at: 2017-09-11T19:44:54.090Z Reads: 164

```
It's OK, I get free shipping from RS as I have an account. :thumbsup:

I was just thinking though, I must have more of those 2.2uf caps lying around because I ordered those for c44 & c49 and I had to order 10...

I'll have a quick look before I pull the trigger lol
```

---
## \#46 Posted by: scepterr Posted at: 2017-09-11T19:46:35.184Z Reads: 161

```
That's a diff size cap actually it's 1206 not 0603
The 1206 caps can be upgraded to 4.7uf 100v btw
```

---
## \#47 Posted by: darkkevind Posted at: 2017-09-11T19:48:56.160Z Reads: 161

```
Oh really!? Oh Bum! I've just found them, got loads of 'em! lol

OK, so definitely can't use the same caps as C44 & C49 for C14? The ones I have are 0805 though?? :confused:

I put these ones on C44 & C49: http://uk.rs-online.com/web/p/ceramic-multilayer-capacitors/7883048/
```

---
## \#48 Posted by: scepterr Posted at: 2017-09-11T19:50:05.143Z Reads: 158

```
I'm not aware of any 0805 on the vesc...
0805 is 1/8 watt 1206 is 1/4 watt..
Clearly it works if that's what you're using but it can't be healthy
You need 16V cap for c14
```

---
## \#49 Posted by: darkkevind Posted at: 2017-09-11T19:53:49.869Z Reads: 149

```
Hang on, I just offered the ones I have up to C44/C49 and the ones I have here are much smaller! I wonder where these came from then? Why did I buy these? lol!

Weird.
```

---
## \#50 Posted by: scepterr Posted at: 2017-09-11T19:54:18.891Z Reads: 146

```
Antispark uses 0805
```

---
## \#51 Posted by: darkkevind Posted at: 2017-09-11T19:55:22.858Z Reads: 143

```
So... go with 0805?
```

---
## \#52 Posted by: scepterr Posted at: 2017-09-11T19:56:51.063Z Reads: 134

```
I would go with the right parts, I don't know what effect using 0805 would have vs 1206
You can use it for now just to get running but I would definitely put the right components on
```

---
## \#53 Posted by: darkkevind Posted at: 2017-09-11T20:00:03.680Z Reads: 136

```
I've ordered the right ones.... pulled the trigger! Should be here tomorrow!

Thanks for all your help mate. Oh by the way, where is C14 located? lol
```

---
## \#54 Posted by: scepterr Posted at: 2017-09-11T20:00:57.749Z Reads: 136

```
Between the black and red wire coming off the vesc, right next to C17
Happy to help, I'm in the middle of fixing a vesc-x atm myself :slight_smile:
```

---
## \#55 Posted by: darkkevind Posted at: 2017-09-11T20:05:55.291Z Reads: 143

```
Oh yeah I see it! Itty tiny one! lol

Thanks so much! Good luck with your fix too :smiley:
```

---
## \#56 Posted by: squishy654 Posted at: 2018-03-29T15:57:47.988Z Reads: 103

```
Do you guys know if Dave's adapter fits the ollin motors sensor cable? OR should I just splice?
```

---
## \#57 Posted by: Doneone Posted at: 2019-10-09T17:03:38.859Z Reads: 24

```
Hi. I am facing the same issue. And I also think about soldering it myself. What happens if I mix up the wires? Can I trust that they come out of the motor the same way they are supposed to go into the vesc?
```

---
## \#58 Posted by: mmaner Posted at: 2019-10-09T17:04:43.093Z Reads: 23

```
The red is always POSITIVE and the BLACK is always negative, don't mix those up.  The sensor wires can be in any configuration so straight through is best.
```

---
## \#59 Posted by: Doneone Posted at: 2019-10-09T17:09:49.569Z Reads: 23

```
Ok great. So it's always black on one end of the connector and red on the other side. And in between it can be mixed up? ![Screenshot_20191007-223511__01|303x500](upload://7MYBXd2y8XuYObUpdPgDzFWdTE4.jpeg) ![Screenshot_20191007-221942|281x500](upload://456YqotfwlTn48U4dEvrkmLyRlP.jpeg) ![Screenshot_20191007-221952__01|329x500](upload://fVAi5j94pRSyVZUjRc2xRcprJWp.jpeg)
```

---
## \#60 Posted by: mmaner Posted at: 2019-10-09T17:14:52.073Z Reads: 21

```
[quote="Doneone, post:59, topic:32867"]
Ok great. So it’s always black on one end of the connector and red on the other side. And in between it can be mixed up?
[/quote]

correct, dont use the temp sensor.  it shold be labeled on the VESC.
```

---
## \#62 Posted by: Doneone Posted at: 2019-10-09T17:25:12.319Z Reads: 20

```
Awesome! What do you mean by temp sensor? Is it one of the wires in between the red and the black on the connector?
```

---
## \#63 Posted by: mmaner Posted at: 2019-10-09T18:04:34.124Z Reads: 19

```
yes, its marked on the ESC, just dont connect anything on that pin and the rest should be easy.
```

---
## \#64 Posted by: Doneone Posted at: 2019-10-09T18:27:53.474Z Reads: 19

```
Ok, cool. But why would I not want to use the temp sensor?
```

---
## \#65 Posted by: mmaner Posted at: 2019-10-09T18:40:23.447Z Reads: 21

```
because you didn't tell me which ESC your using and it doesn't work on a lot of them, its easier and pretty much useful.
```

---
## \#66 Posted by: Doneone Posted at: 2019-10-09T19:00:49.489Z Reads: 21

```
Ah ok :smile:
Going to use dual vesc 6+ on two maytech 8085 sensored and sealed
```

---
## \#67 Posted by: mmaner Posted at: 2019-10-09T19:06:50.138Z Reads: 22

```
Is that the maytech dual vesc 6+
```

---
## \#68 Posted by: Doneone Posted at: 2019-10-09T19:14:07.216Z Reads: 22

```
Trampa vesc
```

---
## \#69 Posted by: mmaner Posted at: 2019-10-09T19:28:45.443Z Reads: 21

```
You're on your own then, I don't buy Trampa.
```

---
## \#70 Posted by: Doneone Posted at: 2019-10-09T19:38:47.523Z Reads: 20

```
Ok, no problem. I think you solved my problem already. 
Why don't you buy Trampa?
```

---
## \#71 Posted by: mmaner Posted at: 2019-10-09T19:41:03.590Z Reads: 19

```
I don't approve of unfair business practices or people that bully their competition.
```

---
## \#72 Posted by: Doneone Posted at: 2019-10-09T19:46:17.465Z Reads: 19

```
Hmm. Yes I heard about that, but don't have sufficient information. So I don't really know what's going on though.
```

---
## \#73 Posted by: mmaner Posted at: 2019-10-09T21:44:44.105Z Reads: 18

```
Its all good.  Its that I dont have a Trampa VESC, so I cant give you specific help.  Essentially removing the temp sensor is not an issue unless you are going incredibly fast for long periods of time.
```

---
## \#74 Posted by: Doneone Posted at: 2019-10-09T22:33:04.581Z Reads: 18

```
Ok will keep your info in mind. Thx for your support 👍
```

---
## \#75 Posted by: hans_maier Posted at: 2019-11-29T12:45:01.629Z Reads: 9

```
Do have any suggestions on how to proceed in this case > https://www.electric-skateboard.builders/t/hall-sensors-5-wires-vs-6-wires/31626/28?u=hans_maier
```

---
## \#76 Posted by: Supervolant Posted at: 2019-11-29T15:44:05.186Z Reads: 9

```
Just wondering how does one know the pinout of a motor? I for example am sitting there with AlienPowerSystems 6374S 200kv Motors and no clue where to put what pin into a new JST connector fitting to the VESC. Anyone aware of the pinout of AlienPower Motors?
```

---
## \#77 Posted by: hans_maier Posted at: 2019-11-29T21:41:29.398Z Reads: 9

```
May be this helps you too https://www.electric-skateboard.builders/t/hall-sensors-5-wires-vs-6-wires/31626/31?u=hans_maier ?
```

---
