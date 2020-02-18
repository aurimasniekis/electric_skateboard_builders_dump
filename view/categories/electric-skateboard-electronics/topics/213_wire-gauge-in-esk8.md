# Wire Gauge in Esk8

### Replies: 40 Views: 11291

## \#1 Posted by: treenutter Posted at: 2015-09-17T12:58:09.853Z Reads: 729

```
I'm about to solder a bunch of things together and it occurred to me; I have 4 different wire gauges I'm using in my electrical setup and I haven't thoroughly thought this through.

The forums I've reviewed in the RC world suggest that this would be alright, but I'd feel a lot more confident with some input from all of you!

In the pic there are the 4 different wire gauges in my build. The 16AWG serial adapter seems like the most likely bottleneck; but I think 16AWG is able to handle the draw from an 8S battery to a 245Kv motor. Does that sound right?

Other info about the build: Enertion VESC, 14T/40T, 127mm pneumatic wheels

<img src="/uploads/db1493/original/1X/74343b84df6c7c738a3d59dc456803dc1dd05f14.jpg" width="575" height="500">
```

---
## \#2 Posted by: lowGuido Posted at: 2015-09-17T13:27:53.962Z Reads: 721

```
In any electrical system you are only as good as your weakest link.
in your case its the 16AWG joiner.  which according to the chart below is good for 35Amps
Personaly I'd use a minimum of 12AWG throughout.

<img src='/uploads/db1493/original/1X/7dd620e04f19d6750c05cf0b55bab78e0a0d5611.jpg'>
```

---
## \#3 Posted by: longhairedboy Posted at: 2015-09-17T14:07:23.678Z Reads: 706

```
I use 10 gauge silicone wire on everything unless I'm trying to preserve a particular component for a possible return if it fails. 10 guage silicone and 5.5mm bullet connectors on both sides of the ESC. 

But i think what you'll find typical is 10 gauge between the battery and ESC and 12 gauge between the ESC and the motors. I'm pretty sure that Enertion is the only vendor putting 10 gauge silicone leads on the motors with 5.5mm bullets. Most motors we use have 12 guage non-silicone leads which i would then replace with 10 gauge silicone.

However, I'd be shocked if I saw any performance difference at all between a completely 12 gauge wiring harness and a 10 gauge harness at 6S. Maybe at 8S or 10S you might see a difference in heat or load handling or something. In fact I'm considering going completely 12 gauge in my 6S system because it will help eliminate some of the spaghetti monster as well as shed a few grams of metal.
```

---
## \#4 Posted by: treenutter Posted at: 2015-09-17T15:01:45.005Z Reads: 669

```
Thanks @lowGuido , I'm going to toss the serial adapter I have and make a new one using 12AWG silicone wire. I'll use the remaining 12AWG wire for the rest of the connections, and solder that onto my VESC.
```

---
## \#5 Posted by: treenutter Posted at: 2015-09-17T15:07:04.939Z Reads: 650

```
Thanks @longhairedboy - Your response begs another question; does everyone replace their motor wires if they buy a "hobby" motor (i.e. one that isn't from @onloop or @torqueboards ?) I have an SK3 and truthfully, the wire coming out of it looks flimsy. I thought I would just have to live with it because I wasn't aware that motor wire is replaceable. 

Can I just snip the leads that extend from the motor and then solder on the 10AWG, or do you suggest that I dismantle it and replace the wire from its source?

This forum rocks! Thanks everyone!
```

---
## \#6 Posted by: lowGuido Posted at: 2015-09-17T16:37:53.751Z Reads: 597

```
you can "replace" the motor wires, I have done it before. but it is a little painful.
because the "leads" coming from the motor are actually a group of intertwined single strand windings of the stator they **are** the source, so to speak. and all the strands are individually insulated from each other.  
so if you do decide to cut the leads and replace them you will need to scratch the insulator off each strand first.

I have had a little success with dipping the ends in acetone before soldering, but it was painful and potentially dangerous.

edit: in case I haven't been clear.. don't do this. its not worth the effort for the little (if any) reward.
```

---
## \#7 Posted by: treenutter Posted at: 2015-09-17T16:40:37.083Z Reads: 560

```
Yikes! Thanks @lowGuido. I think that I'll skip this step in my first build. I'll just use the wire and connectors that came from the factory on the SK3.
```

---
## \#8 Posted by: lowGuido Posted at: 2015-09-17T16:43:36.210Z Reads: 555

```
I have used seven SK3's in my builds and I have always used the stock leads and connectors. never had a problem with them
```

---
## \#9 Posted by: longhairedboy Posted at: 2015-09-17T16:44:17.441Z Reads: 549

```
<img src="/uploads/db1493/original/1X/4fbc9705b9310ba49bbf60dbf7cca852932d3d48.jpeg" width="666" height="500"> 

I didn't go all the way into the stator with these though. I cut the leads at about 1/2" past the casing and butt-soldered the silicone leads on  at that point, then heat shrinked everything together nicely. 

The main reason i did this was because the silicone wire is flexible and springy, which is what you need in this application. Not because i needed a higher gauge wire at the motor. The leads on the motor are properly rated for what the motor can accept already.
```

---
## \#10 Posted by: treenutter Posted at: 2015-09-17T16:48:05.274Z Reads: 529

```
Great to know @lowGuido! Thx again!
```

---
## \#11 Posted by: onloop Posted at: 2015-09-17T22:35:10.449Z Reads: 530

```
I can see an issue with the drive train.

Drive pulley  14  
Driven pulley  40  
Nominal Battery voltage approx  30  
Motor [kV]  245  
Tire diameter [mm]  127  
Final ratio  2.86  
Engine revolution  7350 rpm  
Top speed  62 km/h


This top speed is too high. You will not have enough torque. Especially with pneumatic tyres. I think the motors will overheat and may suffer an early death.

You should aim for max torque with pneumatic.

I suggest gearing for top speed of 35km.

Which means you need a wheel pulley around 70 teeth. 

However the problem with that size pulley it is not much smaller then the wheel and very close to the ground and debris.

After testing several variations I ultimately had to go with 3mm pitch pulleys at 15mm wide so i could achieve an appropriate reduction whilst maximising pulley/ground clearance.
```

---
## \#12 Posted by: treenutter Posted at: 2015-09-18T00:31:00.225Z Reads: 518

```
Thanks for thinking this through @onloop. I've been wondering the same thing; there's a 60T wheel pulley available for the pneumatic wheel I've got, it's 5mm pitch and 9mm wide; probably not optimal, but I think it would accomplish a better gearing. Does that sound like it'd solve this problem?

When I selected the drivetrain, I based it on @psychotiller's pneumatic build posted [here][1] that featured a 245Kv motor, 6-inch pneumatics (opposed to my 5-inch), 14T/40T gearing, and 8S. @psychotiller, maybe you could weigh in on your experience with that build?

Thanks again, so glad to have everyone's input!


  [1]: http://www.electric-skateboard.builders/t/diy-eboard-builds-and-specs/33
```

---
## \#13 Posted by: torqueboards Posted at: 2015-09-18T00:50:17.265Z Reads: 499

```
12AWG is relatively smaller
10AWG is not too bad
8AWG is even thicker.

Depends on how much amps you are pulling at what area.
Ex. 8AWG wire to your UBEC would be pointless.

I think 10AWG is a happy medium for all wiring since it's still relatively small. You can run 8AWG if you plan on running higher amps but it's not recommended since higher amps = more heat.

Onloop makes the motor wires like that since 5.5mm bullet connectors don't come undone like 4mm bullets tend to do. You also can't space out the 4mm male connectors like you can for a 5.5mm male connector.

He uses the 10awg wire to allow the wire to have more flexibility.

It's over spec'ed but doesn't hurt it either. Great idea..

Motors will only deliver 30-80 amps a piece which is rated for like 14AWG wire or something and by default they are usually all 12 awg.

@treenutter - You don't need to replace your motor wires, just don't stress the motor wires and/or if they are being stressed run an extension wire so the wire that flexes is the extension wire and not the actual motor wire.

I find the SK3 motor wires very strong and rigid which is a good thing IMO. You just need to run an extension.
```

---
## \#14 Posted by: psychotiller Posted at: 2015-09-18T01:15:24.439Z Reads: 459

```
When I built my pneumatic, I knew with 150mm wheels i'd be pushing the motor. I can bust 40mph on that board, but it does have some grunt too. it hasn't stalled out on any hills I've tried yet. It's a very smooth board to ride.  Get the 60 and if you don't like the 40 switch it out. Easy enough.
```

---
## \#15 Posted by: treenutter Posted at: 2015-09-18T16:00:40.987Z Reads: 440

```
Thanks @psychotiller ... 40mph sounds scary! I'll start off with the 60T and see how it goes.
```

---
## \#16 Posted by: treenutter Posted at: 2015-09-18T16:02:56.492Z Reads: 432

```
Thx @torqueboards I'll keep an eye on the motor wires over time, if they look like they're aging prematurely l'll replace then with more flexible silicone wires.
```

---
## \#17 Posted by: treenutter Posted at: 2015-09-21T14:20:33.735Z Reads: 426

```
In summary, the way to select wire gauge is to compare the power-handling limits of your wires and connectors with the maximum current your motor can draw. 

In my case, the motor has a  max 70A draw. 12AWG wire can handle up to 84.40A, so 12AWG would be the minimum wire gauge to use, just as @lowGuido suggested. Heavier wire (10AWG) would provide further overhead.

That just leaves the issue of connectors! So far I've been using Deans connectors. Although Dean's doesn't publish an official rating, I read lots of reports of folks pulling 100A with no issues. However, these reports are from the RC world, where the duration of a usage session is about 10-20 minutes (much lower than our typical esk8 application). I like Deans because they're small and they seem capable of the draw. I also have a bag of them so I've been practicing my soldering!

Does anyone have experience with Deans (good or bad)?

<img src="/uploads/db1493/original/1X/4270519c3cab8d0a7e86e484b983fd89ff3cae6c.png" width="551" height="232">
```

---
## \#18 Posted by: torqueboards Posted at: 2015-09-22T04:35:24.146Z Reads: 402

```
I think deans are ok. Evolve uses deans and I think I seen a few other decks use Deans. Deans seem like the connected would come off easily. Personally, I like 5.5mm bullets, EC5 or XT90 connectors. The cost isn't much so I'd go for something better. I also think Deans are easier to short on accident.
```

---
## \#19 Posted by: longhairedboy Posted at: 2015-09-22T12:35:22.493Z Reads: 393

```
i prefer bullet connectors because they are a simple butt-joint type connector that can be easily taped or heat shrinked together without taking up any more space in the box than the wire itself. The 4mm for the 12 gauge and the 5.5mm for the 10 gauge wires are basically the only connectors you need in a build. Oh and they're dirt cheap and come by the bag. 

The only disadvantage to using them is the occasional arcing, sparking, and possibly even slag splattering that happens when the battery leads touch each other, but as long as you tape them up during the disconnect process that's a non-issue. Once after accidentally allowing the leads to come in contact with each other i found myself looking down at a shirt covered in molten metal. The connector had literally melted and sprayed onto my shirt much like welding slag. Good times.
```

---
## \#20 Posted by: treenutter Posted at: 2015-09-22T19:32:54.586Z Reads: 382

```
@longhairedboy I can certainly appreciate the space-saving and ease of bullet connectors! As I've been planning out my enclosure I see all kinds opportunities to reduce wasted space; connectors and extra wires are the major culprits my case. I think I'll have quite a spaghetti monster by the end! I'm not as experienced as you are; not sure I trust myself to remember to keep battery leads from making contact!
```

---
## \#21 Posted by: treenutter Posted at: 2015-09-22T19:33:57.251Z Reads: 355

```
Thanks @torqueboards I ordered a bag of XT90s to try them out. I like that I can get a simple antispark device built into a single plug, and the soldering looks pretty straight forward.
```

---
## \#22 Posted by: MonsterCoatings Posted at: 2015-12-10T05:53:13.722Z Reads: 350

```
I have been using Deans for years in my R/C projects. Coming from a commercial electrician background where equipment uses awesome fully insulated connectors with screw locking & waterproof options, it is a shame we cannot mineraturize them for our applications. I can appreciate Deans small and simple idiot resistant design. Generally I do not let anyone else work on my projects but it is nice to know that if I loan my project to someone there is only one (right) way to connect things. (Wish Deans made more than one size.)

I like bullet connector designs.  There is a little more flexibility with bullet style. Often to insure correct connections I will offset/stager the wire length with bullet connectors which makes connections logical and also prevents large clusters of connectors in one area.

As far as wire I always error on the side of caution and being on the  larger side of the average rider things heat up faster under me. Also with age vibration and movement wires or strands can break inside the insulation increasing resistance as well as heat. Starting off more strands in a larger gauge wire will offer a larger reserve should a few go bad over time. Ride and evaluate your particular application often if you discover heat building up in your system replace the problem section with upgraded components till the problem is corrected.
```

---
## \#23 Posted by: Ulfberht Posted at: 2016-04-17T06:28:51.655Z Reads: 312

```
Anybody try tinned copper 10 awg? 
Like this Venom stuff:
http://www.venompower.com/collections/soft-silicone-wire/products/venom-10awg-soft-silicone-high-strand-count-wire-red-and-black-1m-3ft
" Do not be fooled by competitors claims that pure copper wire is superior. Venom tin coated wire can outlast the competition 10 fold due to its corrosion and oxidation resistant properties. This means the internal resistance of the wire stays low for longer, thereby channeling more power to your RC models, devices, or other..."
Hype or Ripe?
```

---
## \#24 Posted by: trbt555 Posted at: 2016-04-17T06:41:14.963Z Reads: 305

```
Hype.
But if it makes you feel better about your config, by all means go for it.
```

---
## \#25 Posted by: lowGuido Posted at: 2016-04-17T06:41:29.717Z Reads: 297

```
don't believe the hype.

**IS THAT $18 PER METER?**

omg!

you can buy 6 meters of real wire for $18
```

---
## \#26 Posted by: Ulfberht Posted at: 2016-04-17T07:00:16.043Z Reads: 298

```
LOL. Just putting it out there. 
You can get it much cheaper here:
http://www.buddyrc.com/black-10awg-silicone-wire.html
$1.25/FT But it doesn't say "Venom" on it. LOL
I was reading a few things and came across this article and others like it about tinned copper....
https://www.linkedin.com/pulse/20141202034347-252652481-sharing-information-on-tinned-vs-bare-copper
Food for thought...
```

---
## \#27 Posted by: lowGuido Posted at: 2016-04-17T07:31:59.501Z Reads: 292

```
well that's a much more reasonable price.
I'd consider buying it for that price.
although id the plain copper is cheaper id still get that. :P
```

---
## \#28 Posted by: delta_19 Posted at: 2016-04-17T16:13:33.725Z Reads: 279

```
tin or silver coated copper is nice because it lets solder flow a lot easier and it does hold up from oxidisation a lot better but it is no holy grail that should cost you $20 a meter.
```

---
## \#29 Posted by: Ulfberht Posted at: 2016-04-17T21:19:41.620Z Reads: 274

```
Agreed. I guess that "Venom" brand name adds extra mojo to any build! 
You can get it for $1.25 a foot in that second link I posted. 
http://www.buddyrc.com/black-10awg-silicone-wire.html
Exactly the same stuff!! 
I guess the issue becomes..Is corrosion on eboard wiring a non-issue or could we benefit from using this wire on our builds? I'm willing to explore all options to get the best possible product.
```

---
## \#30 Posted by: delta_19 Posted at: 2016-04-17T21:56:30.952Z Reads: 260

```
I would say with outdoor use it would be nice to have
```

---
## \#31 Posted by: massy Posted at: 2016-04-17T22:22:05.457Z Reads: 258

```
I guess there could be quality differences. The wires on my VESC for example are crazy stiff and doesn't bend easily (the silicone seems worse). I feel the cables I bought for the rest of the board is higher quality but they were only like 7$ for 4 meters, doubt there are any much better wires.
```

---
## \#32 Posted by: longhairedboy Posted at: 2016-04-18T18:31:55.060Z Reads: 260

```
fucking christ its AudioQuest Diamond cables all over again. 

http://hothardware.com/news/10000-ethernet-cable-claims-earth-shattering-advancement-in-audio-fidelity-if-youre-stupid-enough-to-buy-it

For the record, i have a home recording studio and I have seen with my own eyes that the average person cannot tell the difference between a $100 balanced patch cable and a duct taped section of coat hanger when it comes to analog audio transmission over copper. But this Diamond cable... this took the cake. On so many levels i can't even count. Ethernet is bidirectional, digital signals do not suffer fidelity loss due to wire characteristics, gold connectors are onlly really useful in permanant installs... a $5 ethernet cable from amazon works just as well... I'll stop there. 

I use high strand count silicone insulated Superworm wire. It takes the punishment of DIY esk8 building and is wonderfully flexible and springy, not to mention that high heat insulation can take a bump from the soldering iron without even leaving a mark in most cases. And its cheap for the high quality it provides.
```

---
## \#33 Posted by: treenutter Posted at: 2016-04-19T14:34:04.800Z Reads: 240

```
@longhairedboy I remember buying a (4-inch) Monster patch cable once, for $50! The snakeoil sales in music and A/V are always around to rob anyone who hasn't done their homework!
```

---
## \#34 Posted by: delta_19 Posted at: 2016-04-19T16:21:25.927Z Reads: 240

```
FUCKING WEAK

LOLOLOLOLOL
http://www.coconut-audio.com/xlrinterconnects.html

there are so many of these guys
```

---
## \#35 Posted by: longhairedboy Posted at: 2016-04-19T16:38:24.816Z Reads: 238

```
That's it. I'm going to call the Superworm factory and have them stamp my label on their wire and call it HIGH PERFORMANCE DIAMOND PLATINUM ESK8 POWER CONDUIT WITH DIRECTIONAL ELECTRON PATHWAY TECHNOLOGY and sell it for $1500/ft and after i sell 6 feet of it and pay off my credit cards i'll build the world's first 14S skateboard using coat hanger wire.
```

---
## \#36 Posted by: treenutter Posted at: 2016-04-19T18:10:10.637Z Reads: 234

```
@delta_19 @longhairedboy that has to be a  joke right? No one is paying $8,000 USD for a 1.5 meter USB cable, right? Please tell me it's a joke!
```

---
## \#37 Posted by: Mobutusan Posted at: 2016-04-19T18:14:03.348Z Reads: 228

```
Shit, this is a joke? 

@longhairedboy, I'm gonna have to cancel my order then. :grinning:
Now where am I gonna find wire with DEPT (DIRECTIONAL ELECTRON PATHWAY TECHNOLOGY)? Hmmmmm......
```

---
## \#38 Posted by: longhairedboy Posted at: 2016-04-19T19:35:36.109Z Reads: 230

```
I just noticed that RC Buddy has the Red silicone tin coated copper high strand wire at 1.39 a foot but the black silicone tin coated high strand wire at 1.25 per foot. 

CLEARLY they understand that the red wire has a 20% increase in performance over the black wire and are charging accordingly.  

They sell by the foot and its the same shit i've been getting from amazon, i may start buying 10 and 12 awg from them 20 or 30 feet at a time and keep it on spools. I just made some handy wire dispensers but i don't think they'll hold quite that much, but i can always keep enough to do jobs with in the dispensers and kep the spools elsewhere.
```

---
## \#39 Posted by: longhairedboy Posted at: 2016-04-19T19:36:57.589Z Reads: 230

```
they also have 10S and 12S balance leads for building packs. I'm definitely adding these guys to my sources list.
```

---
## \#40 Posted by: Ulfberht Posted at: 2016-04-19T21:40:09.014Z Reads: 232

```
[quote="longhairedboy, post:35, topic:213, full:true"]
That's it. I'm going to call the Superworm factory and have them stamp my label on their wire and call it HIGH PERFORMANCE DIAMOND PLATINUM ESK8 POWER CONDUIT WITH DIRECTIONAL ELECTRON PATHWAY TECHNOLOGY and sell it for $1500/ft and after i sell 6 feet of it and pay off my credit cards i'll build the world's first 14S skateboard using coat hanger wire.
[/quote]

I'm in!! I'll take 1000 feet. Before you jack the price up to $2000/FT!! It's just that steezy!! :sunglasses:
```

---
