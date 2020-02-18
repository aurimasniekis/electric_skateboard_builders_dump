# FatBoy Sparky Switch 300A 60V Anti-Spark Switch

### Replies: 72 Views: 4855

## \#1 Posted by: Kug3lis Posted at: 2018-04-08T01:28:17.674Z Reads: 530

```
Hi guys, today I would like to announce new project created by me (My father works on all mechanical ideas)

After reading a lot of discussions, a lot of shower thoughts and trials I finally created in my opinion perfect anti-spark switch for any variety load. 

## Features:

* High Side Switching (Switches positive wires)
* Push button (hold 0.5s to turn on / 3s to turn off)
* Output for power indicator (will require resistor according to your selected led specs)
* Single industrial size MOSFET in SOT-227 package
* Ability to use any size of wires/bus bars

## Specifications:

* Up to 60V (14S)
* 300A (MOSFET is rated up to 420A and impulses up to 1,000A) (200A constant limited by MOSFET leads)
* Dimensions with screw and MOSFET is 16mm x 25mm x 45mm (2 x 18650)

For high currents, the heatsink will be required to be attached to MOSFET (Will have to research how much current can't handle without a heatsink at normal case temperature)

![image|632x500](upload://mDQ7N6GLlYJFrS9BhWD5cTrRblO.png)

![3d_front_profile|598x500](upload://jBc1Lp7ijZB73WjFS4ruP7BrLx4.jpg)

![3d_profile|614x499](upload://bmBEmTK9h9QF9j2yudsEmngLGUu.jpg)

![3d_side|690x390](upload://xwnWv8LiLGbJSr46BA8Kl06MbXI.PNG)

## Connecting diagram:

![image|690x218](upload://cojqylMoDVFVMjucyrs2TorBve.png)

I do not provide fuse, as not all people would use 300A and etc, because decent 300A fuse cost a bit of money, so to save space and cost I am leaving it to the user.

## Availability

Parts are already ordered, PCB will be ordered on Monday, so best guess around 1-3 weeks will be available to buy from our online store https://shop.3dservisas.eu
```

---
## \#2 Posted by: b264 Posted at: 2018-04-08T01:31:16.395Z Reads: 443

```
Finally an overbuilt antispark switch that hopefully might not fail
```

---
## \#3 Posted by: b264 Posted at: 2018-04-08T01:31:47.818Z Reads: 435

```
Does this have any safety features like push to turn on, but push-and-hold to turn off?
```

---
## \#4 Posted by: Kug3lis Posted at: 2018-04-08T01:33:07.762Z Reads: 424

```
At the moment I have decided these protections:

* Turn on: hold switch for 0.5s
* Turn off: hold switch for 3s
```

---
## \#5 Posted by: E1Allen Posted at: 2018-04-08T01:33:28.385Z Reads: 412

```
Any reason for the 60v cutoff?  The ebike world could use this but up to 100v and same amp limit.  Prices?
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-04-08T01:35:26.747Z Reads: 397

```
Switch control chip is limited to 65V I did not intended this for ebike's
```

---
## \#7 Posted by: JLabs Posted at: 2018-04-08T01:50:07.702Z Reads: 387

```
Ohhh I could put this through it’s paces on a 13s Evo Build, and if they work out well, maybe I can help distribute them in the USA.
```

---
## \#8 Posted by: thisguyhere Posted at: 2018-04-08T01:50:33.207Z Reads: 384

```
this is great.

what do you think the price will be?

will it come with the push switch, or do we supply that as well?  if the latter, is there a switch you'd recommend?
```

---
## \#9 Posted by: Kug3lis Posted at: 2018-04-08T01:53:26.452Z Reads: 377

```
About the price don't know yet so can't really promise anything but something around 50 eur mark

At the moment to make it release faster as people building projects for spring first batch will be only the PCB with MOSFET and screws.

You can use any switch/led as it require momentary push button (I would recommend those vandal switches as they look cool)
```

---
## \#10 Posted by: barajabali Posted at: 2018-04-08T02:17:43.465Z Reads: 362

```
I’ll take 1 for sure
```

---
## \#11 Posted by: intensivegecko Posted at: 2018-04-08T20:08:07.286Z Reads: 341

```
I may pick one up :blush:
```

---
## \#12 Posted by: Acido Posted at: 2018-04-08T20:14:14.537Z Reads: 333

```
300a fuse is like 3$ malelectrics or whatever 
The place where you can get a spotwelder
Its not much since they probably have like a 200% margain profit
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-04-08T20:43:52.971Z Reads: 327

```
Thanks for the link, I was looking at DigiKey for devent fuses with high voltage ratings, not 12V so maybe that's why. But still first batch will be only PCB and MOSFET, later on we will provide with wiring and switch :) But to make it faster will only sell first without them ;)
```

---
## \#14 Posted by: Nordle Posted at: 2018-04-09T07:01:32.355Z Reads: 316

```
Nice, why isn‘t the jst connector facing the other side?
```

---
## \#15 Posted by: Martinsp Posted at: 2018-04-09T08:11:58.217Z Reads: 317

```
Great design!
I finished my version of soft latching switch two days ago and ran into an issue which is common with the standard Vedder switches where if you are using the processor to pull the gate up or in another words have the gate connected to a pull up resistor to keep it from floating. I had this in one of the test versions and when connecting 4x2200uF capacitors simulating 4wd setup I found out that the high current for even less then 1ms when the capacitors are connected can charcoal the semiconductor inside the FETs which meant that it got stuck in closed state. I avoided that using pull down instead of pull up and software protection too so that the FETs dont get fried. Just curious if that is present or possible with these big FETs too.
```

---
## \#16 Posted by: Kug3lis Posted at: 2018-04-09T10:21:02.667Z Reads: 302

```
@Nordle I used connector only for the holes, I will not be populating it to not increase the height of whole thing.

@Martinsp I am not connecting FET directly to MCU as I am using high side switching for that I am using gate driver. Regarding high capacitance load you need to control output voltage rise time in order prevent killing FET
```

---
## \#17 Posted by: L3chef Posted at: 2018-04-09T10:30:35.633Z Reads: 299

```
Naaajs! Need to get payed now so I can order one or 2
```

---
## \#18 Posted by: Kug3lis Posted at: 2018-04-12T12:11:24.132Z Reads: 296

```
We received the PCB but there was a mistake made by me... Ground planes were disabled then I was generating gerbers... But for testing, it will be more than enough to see the performance of it.

![image|690x483](upload://oeIYAsuN4ucqr8cP9Lx890m7Tmm.jpg)
```

---
## \#19 Posted by: Kug3lis Posted at: 2018-04-17T17:01:17.978Z Reads: 286

```
After first turn on, with some light load of 10A it was working fine, next step is bit higher constant 80A don't have yet higher current source available to test higher constant currents ;)
```

---
## \#20 Posted by: SORRENTINO Posted at: 2018-04-17T17:07:14.517Z Reads: 290

```
Im sold if 80amp constant works out :)
```

---
## \#21 Posted by: Kug3lis Posted at: 2018-04-20T13:57:32.540Z Reads: 288

```
Some updated information regarding the switch, we have done some testing and decided that even at low currents like 50A constant heat-sink is required so we are making a aluminum case there MOSFET will sit inside and PCB will cover it.

The price will be 70 eur + VAT + Shipping.

It will be available in 1-2 Weeks ordered new PCB today.

![image|310x500](upload://rC09yhLKJHSZ8SbXws78FxtmRNP.jpg)
```

---
## \#22 Posted by: Charles_Chan Posted at: 2018-04-20T14:59:46.578Z Reads: 273

```
For the Spark Switch , I saw someone sale it with IRFS7530 MOSFET and someone sale it with IRFS7730. which is best for use?
```

---
## \#23 Posted by: Kug3lis Posted at: 2018-04-20T15:21:10.540Z Reads: 274

```
They are all too small for this application ;)
```

---
## \#24 Posted by: Charles_Chan Posted at: 2018-04-20T15:37:03.496Z Reads: 276

```
Thanks. good to know it. 
For the MOSFET of your Sparky switch, is it SOT-227 ?
```

---
## \#25 Posted by: Kug3lis Posted at: 2018-04-20T15:48:58.194Z Reads: 275

```
It's mosfet in SOT-227 package

![image|300x236](upload://yLI5WJlmR7B1lgxmwy1KSuA9oZI.jpg)
```

---
## \#26 Posted by: Deckoz Posted at: 2018-04-20T16:17:39.793Z Reads: 271

```
[quote="Kug3lis, post:21, topic:51532"]
50A constant heat-sink is required
[/quote]

Just curious what voltage this was at?
```

---
## \#27 Posted by: Kug3lis Posted at: 2018-04-20T16:19:09.024Z Reads: 267

```
10S didn't have other batteries available, but it should work same with 12s and 14s
```

---
## \#28 Posted by: Deckoz Posted at: 2018-04-20T16:19:57.458Z Reads: 263

```
Was just trying to get a ballpark for the wattage passing through. Thanks..
```

---
## \#29 Posted by: Cobber Posted at: 2018-04-20T16:20:20.657Z Reads: 258

```
50a aint much... I want you to crush this dude! (@Kug3lis)  50a is like last years tech...
```

---
## \#31 Posted by: Cobber Posted at: 2018-04-20T16:22:58.337Z Reads: 253

```
quote in total, 50a is not _fat_, it is not that much.

put another way: a 300a esc that can only do 50a... _is not that much_
```

---
## \#32 Posted by: Kug3lis Posted at: 2018-04-20T16:35:42.020Z Reads: 246

```
I said 50A needs heatsink not that it handles that much maximum ;)
```

---
## \#33 Posted by: Nordle Posted at: 2018-04-20T16:41:51.847Z Reads: 243

```
What mosfet are you using exactly?
I would try to find the one within desired Voltage&Amp ratings and lowest possible drain to sourece resistance [Rds on], that should keep temps as low as possible.
```

---
## \#34 Posted by: Kug3lis Posted at: 2018-04-20T16:48:06.808Z Reads: 242

```
I have already found one ;) and calculated everything required for it :)
```

---
## \#35 Posted by: Kug3lis Posted at: 2018-04-22T19:02:59.459Z Reads: 251

```
Just received mosfets :)

![image|690x488](upload://dSbA6KjiNIAdUu0tHwV64xpiRZY.jpg)
```

---
## \#36 Posted by: Orin635 Posted at: 2018-04-22T21:42:12.184Z Reads: 239

```
where can you buy fuses?
```

---
## \#37 Posted by: Kug3lis Posted at: 2018-04-26T13:12:00.493Z Reads: 236

```
Mouser/Digikey any electronics store ;)
```

---
## \#38 Posted by: Kug3lis Posted at: 2018-04-26T13:13:47.497Z Reads: 255

```
Today received the PCB and probably tomorrow the parts so I guess early next week it will be available to buy early version

![image|375x500](upload://vg8jHT8PiwqwzrSfbuFYLTNzQLR.jpg)

![image|375x500](upload://5RMrhIisoroAwutDHDLVRz83KC1.jpg)

![image|375x500](upload://3smZa4okIys8PczQYpxRil0iEsn.jpg)
```

---
## \#39 Posted by: uigiroux Posted at: 2018-04-26T13:28:47.441Z Reads: 280

```
Looks incredible!

How much will it be in the states?
```

---
## \#40 Posted by: Kug3lis Posted at: 2018-04-26T13:29:14.464Z Reads: 284

```
70 eur + Shipping
```

---
## \#41 Posted by: Kug3lis Posted at: 2018-05-02T13:15:42.134Z Reads: 271

```
Finally it is available to buy

http://www.electric-skateboard.builders/t/selling-fatboy-sparky-switch-v1-0-300v-6s-14s-anti-spark-switch/54128

https://shop.3dservisas.eu/collections/fatboy/products/fatboy-sparky-switch-v1-0
```

---
## \#42 Posted by: Cobber Posted at: 2018-05-02T13:22:50.343Z Reads: 238

```
ok bro so you say 300a with external cooling... more than your heatsink?

I ask as i'm building a board now with 2 x 148a motors (8s), data logs show over 100a a piece constant.
```

---
## \#43 Posted by: Kug3lis Posted at: 2018-05-02T13:24:58.195Z Reads: 229

```
Constant for how long 10-30min? You can run with this block for pulses over 1min no problem it will get warm but not that hot. With over 100A constant for like 10-20min you will need external cooling. But for normal esk8 rides where you get impulses of 100-300A for like 30s it will be enough
```

---
## \#44 Posted by: Cobber Posted at: 2018-05-02T13:28:26.749Z Reads: 219

```
ok

so just a fan like my speed controllers? 

might stick to 8mm anti-spark connectors...

thanks bro, block of aluminium looks cool, love the saw marks on the ends :smiling_imp:
```

---
## \#45 Posted by: Kug3lis Posted at: 2018-05-02T23:27:27.891Z Reads: 201

```
I highly doubt that any of you guys will run AWG0 for high current so first your wires will heat up pretty nicely. If you will be able to show me constant at least 1 min on currents higher than 100A otherwise like I said its normal esk8 loads don't need much cooling as those are not longer than minute long or etc :)
```

---
## \#46 Posted by: Sender Posted at: 2018-05-02T23:28:54.736Z Reads: 198

```
So it doesn't include the actual push button right?  Do you have one you recommend?
```

---
## \#47 Posted by: deucesdown Posted at: 2018-05-02T23:34:42.930Z Reads: 199

```
[quote="Kug3lis, post:45, topic:51532"]
normal esk8 loads
[/quote]

Maybe you can make explicit what this means to you. I'm inferring 100a from the pack for 1min at a time?

The people intetsted are probably the power users and "normal" means different things to different people.
```

---
## \#48 Posted by: PatRocks Posted at: 2018-05-03T00:03:31.876Z Reads: 192

```
What he said, and some of us are shameless hardware-junkies! 

I do like the headroom in this design
```

---
## \#49 Posted by: b264 Posted at: 2018-05-03T00:21:19.442Z Reads: 191

```
In my opinion, "normal esk8 loads" means 8kW peak for up to 1 minute and 500W continuous

At least, that's what it means to me...
```

---
## \#50 Posted by: Kug3lis Posted at: 2018-05-03T00:31:09.728Z Reads: 187

```
Yeah that's right I mean you can do peak 15kW if you want and you wires, connectors will hold it for sure and do like 2kW constant :) otherwise you will need actively cool it down

I am riding myself 10kW setup and never even seen more than 2kW peak per motor (I am running 5:1 high torque setup so current is way higher than normal setups)
```

---
## \#51 Posted by: Kug3lis Posted at: 2018-05-03T00:35:21.740Z Reads: 187

```
Any momentary button will work, even shortening the wires like in movies
```

---
## \#52 Posted by: uigiroux Posted at: 2018-05-12T17:30:12.796Z Reads: 188

```
Is it possible to order one of these with everything hooked up for an extra fee?  Push button, fuse, LED, etc...
```

---
## \#53 Posted by: Kug3lis Posted at: 2018-05-12T17:33:14.739Z Reads: 190

```
Sorry this is DIY kit... Everyone uses different configuration and adapt to their own needs...
```

---
## \#54 Posted by: uigiroux Posted at: 2018-05-12T17:34:02.115Z Reads: 195

```
Ok no worries.  Do you have any left in stock?
```

---
## \#55 Posted by: Kug3lis Posted at: 2018-05-12T17:36:12.656Z Reads: 200

```
Yes there is some left, but I can't guarantee it will be in stock several days later... 

https://shop.3dservisas.eu/collections/fatboy/products/fatboy-sparky-switch-v1-0
```

---
## \#56 Posted by: Kug3lis Posted at: 2018-05-23T22:12:25.774Z Reads: 181

```
Still available :) Also working on smaller version for not so hard core riders

https://shop.3dservisas.eu/collections/fatboy/products/fatboy-sparky-switch-v1-0
```

---
## \#57 Posted by: willpark16 Posted at: 2018-05-24T02:41:57.486Z Reads: 170

```
I’m considering getting this but I need a good bms for it
```

---
## \#58 Posted by: b264 Posted at: 2018-05-24T02:51:28.322Z Reads: 170

```
You can use this wired around your BMS like a loopkey if you want to
```

---
## \#59 Posted by: willpark16 Posted at: 2018-05-24T02:54:54.259Z Reads: 168

```
Ohhhh no I meant I haven’t been able to find a good bms that I can use with it , tbh I’m overthinking it
```

---
## \#60 Posted by: b264 Posted at: 2018-05-24T02:57:31.433Z Reads: 166

```
For 10S, a bestech D190 is good but I'm sure there are better (smaller) ones out there
```

---
## \#61 Posted by: willpark16 Posted at: 2018-05-24T02:58:28.698Z Reads: 165

```
That big one is super reliable but the size of it made it a tad impracticle for my application
```

---
## \#62 Posted by: b264 Posted at: 2018-05-24T02:59:52.900Z Reads: 154

```
The [D190](http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D190.html) is not the big one, I think that's the [D131](http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D131.html)
```

---
## \#63 Posted by: willpark16 Posted at: 2018-05-24T03:10:57.818Z Reads: 158

```
Oh sweet I’ll check that one out
```

---
## \#64 Posted by: pylotope Posted at: 2018-08-22T04:24:29.075Z Reads: 126

```
[quote="Kug3lis, post:56, topic:51532"]
Also working on smaller version for not so hard core riders
[/quote]

May I inquire if it's done yet? :)
```

---
## \#65 Posted by: Battosaii Posted at: 2018-08-22T06:08:54.046Z Reads: 123

```
I got mine it's larger than expected but I can make it fit. I'm considering having part of the heat sink stick out of the enclosure to have it air cooled but that may be Overkill for my set up.
```

---
## \#66 Posted by: Gizmo Posted at: 2018-10-01T16:49:28.856Z Reads: 117

```
I'm kind of a big fan of overkill
```

---
## \#67 Posted by: Battosaii Posted at: 2018-10-01T17:14:23.243Z Reads: 117

```
Actually got around to mock up everything and the damn switch is too big i can't fit my BMS. I'll need to tinker with it some more before I give up.
```

---
## \#68 Posted by: b264 Posted at: 2018-10-01T18:40:57.179Z Reads: 111

```
[quote="Gizmo, post:66, topic:51532, full:true"]
I’m kind of a big fan of overkill
[/quote]

If it's worth doing, it's worth overdoing.  That way, it won't break later.
```

---
## \#69 Posted by: Grozniy Posted at: 2018-10-01T19:01:01.169Z Reads: 114

```
![1j6lfj|640x360](upload://5fcpEjLjZWQILcyr65Hgo65MWDn.jpeg)
```

---
## \#70 Posted by: Battosaii Posted at: 2018-10-26T17:31:30.465Z Reads: 110

```
I'm about to install one of these, can I use an audio 200a fuse for this? 

I was thinking of picking up some of these locally
https://www.bestbuy.com/site/kicker-anl-fuse-2-pack-black-orange/9905871.p?skuId=9905871

Maybe I should get the Mini sparky this one is looking to be very bulky with fuse and all
```

---
## \#71 Posted by: LiquidSkater Posted at: 2019-04-30T19:00:14.053Z Reads: 67

```
[15566504592414279644416883785934|374x500](upload://x6wPjx44n3iAxT1ByffDgT305nu.jpeg) ![15566504847895978260481251717062|375x500](upload://pMbvUX0r742SH0qRQDrnY42ELCJ.jpeg) 
Hi, I bought an anti spark switch on ebay, I had the non - latching button and put another button on the NC wire and it worked perfectly fine. So I set up the board and went for a ride and 800 meters in power started to cit out, then it came back and I continued to ride, but on my way home (2nd km) power completely cut off and something started to smell. When I rushed home and opened the  enclosure I saw that the mosfets had melted a hole in shrink wrap...
I don't know what should I do now. If I had done something wrong or if I should cool it somehow...!
I had the wires soldered correctly but it just melted...

The button i got (model 6)
https://www.ebay.com/itm/Anti-Spark-Power-On-Off-Switch-for-VESC-or-ESC-electric-skateboard-longboard-LED/163610874953?_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D56949%26meid%3D607a686075f5439c9d2f2223b46b5922%26pid%3D100675%26rk%3D1%26rkt%3D15%26sd%3D163610874953%26itm%3D163610874953&_trksid=p2481888.c100675.m4236&_trkparms=pageci%3Ac2cc312f-6b78-11e9-9fab-74dbd180dd14%7Cparentrq%3A6f950d4f16a0aadc417ffeaaffeea806%7Ciid%3A1
```

---
## \#72 Posted by: Battosaii Posted at: 2019-04-30T19:10:35.667Z Reads: 66

```
This thread is for the Fatboy 300a antispark.

Generally antisparks are not reliable especially tge cheap ebay ones id stay away from those. Yours is probably dead now.
```

---
## \#73 Posted by: b264 Posted at: 2019-04-30T19:28:25.890Z Reads: 63

```
https://www.electric-skateboard.builders/t/vedder-antispark-design-problem-or-implementation-problem/77967/4?u=b264
```

---
