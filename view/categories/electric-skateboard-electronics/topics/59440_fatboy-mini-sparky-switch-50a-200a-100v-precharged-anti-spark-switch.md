# FatBoy Mini Sparky Switch 50A - 200A 100V PreCharged Anti-Spark Switch

### Replies: 91 Views: 3546

## \#1 Posted by: Kug3lis Posted at: 2018-06-20T02:15:54.323Z Reads: 452

```
Hi guys, today I would like to announce a smaller more universal and better anti-spark switch

After doing a lot of research of making switching least painful in our cases and minimizing the switch to small 2 x 18650 size (36mm x 65mm) Also much cheaper for simple projects from 50A to 200A on paper with bit tinkering could do much more :)

## Features:
* High Side Switching (Switches positive wires)
* Push button (hold 0.5s to turn on / 3s to turn off)
* Output for power indicator (will require resistor according to your selected led specs)
* Multiple IRF DirectFet mosfets (N+1 for PreCharge)
* Pre-Charge circuit before turning on main MOSFET's to charge capacitors via a resistor to limit inrush current.

## Specifications:
* Up to 100V (23S)
* 1 to 4 MOSFET's
* In rush current limited to (V/2 A) (for e.g. 50/2 = 25A max inrush current)
* Dimensions would be 36mm x 65mm (2 x 18650)

It will have a small aluminum plate under it to cool down the MOSFET's a bit.

Here is simulation I have done with this style design, as you can see no inrush current higher than 50A @ 100V.

### Without inrush limiting:

![image|690x377](upload://kZinL9aHKIW4VcbkNZ6Pw41ZKkb.jpg)

### With pre-charge:

![image|690x369](upload://d54gxurkotuSHk6RXylGtFdWMZr.jpg)

## Pictures:

![image|360x499](upload://7LSpy4ERxlIcskomgNhsw9U5arL.jpg)

![image|379x500](upload://oEFcFnSMvtNPLBoa2dp4MhjgLcQ.jpg)
```

---
## \#2 Posted by: SeanHacker Posted at: 2018-06-20T02:27:55.837Z Reads: 402

```
You make some cool shit dude! I'm so glad you came to this forum. When will you hopefully be selling these?
```

---
## \#3 Posted by: onepunchboard Posted at: 2018-06-20T02:31:14.120Z Reads: 394

```
also interested
```

---
## \#4 Posted by: Colson003 Posted at: 2018-06-20T04:57:38.815Z Reads: 382

```
Oh I’d be interested in picking up a few of these! I’ve been looking for an eswitch that can reliably handle 13S
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-06-20T07:53:17.757Z Reads: 354

```
We will be ordering PCB's today for all the projects and doing some testings with it after everything works I guess maybe in the first weeks of July or something similar.
```

---
## \#6 Posted by: L3chef Posted at: 2018-06-20T08:06:30.424Z Reads: 337

```
Nice ! :fist_right:
How thick will these be with alu heatsink ?
```

---
## \#7 Posted by: b264 Posted at: 2018-06-20T08:09:27.555Z Reads: 342

```
[quote="Kug3lis, post:1, topic:59440"]
Push button (hold 0.5s to turn on / 3s to turn off)
[/quote]

This is AWESOME.  Any way to lower the turn-on hold to like 100ms?

I really like how flying road debris can't shut your board down...
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-06-20T08:14:02.559Z Reads: 325

```
At the moment I can't tell but definitely not thicker than 10mm or for 100% sure not thicker than 18mm (18650 thickness)
```

---
## \#9 Posted by: JonathanLau1983 Posted at: 2018-06-20T08:18:04.848Z Reads: 323

```
Awesome!
Any idea on price range of this one compared to the non mini version?
```

---
## \#10 Posted by: linsus Posted at: 2018-06-20T09:04:56.427Z Reads: 302

```
Heatsink really shouldnt be needed. If there is a need for a heatsink, you got the wrong mosfets or too few in parallell
```

---
## \#11 Posted by: L3chef Posted at: 2018-06-20T09:06:32.664Z Reads: 291

```
Awesome! I'm in for a set!
```

---
## \#12 Posted by: Maxid Posted at: 2018-06-20T09:24:56.421Z Reads: 281

```
36mm by 65mm is like half the size of a Focbox (=64 by 64mm with case) - just for switching it on/off.
Is there a possibility that you really make a mini version? My Lou needs a switch but space is very limited :(
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-06-20T09:26:39.203Z Reads: 273

```
There will be multiple options (price levels) so for all of them there will be heatsink included as even on lowest level you could still pull more than 50A but heatsink will be required same as Focbox and etc ;)
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-06-20T09:33:16.328Z Reads: 274

```
If you take off heatsink, remove button connector you should end up with like 3-5mm height so you can put it on top of your batteries... I will think about smaller version but I don't think it wil be  anything soon as I have other projects which needs to be finished for Evo project :P
```

---
## \#15 Posted by: Silverline Posted at: 2018-06-20T09:39:34.146Z Reads: 260

```
I'm in for one :slight_smile:
```

---
## \#16 Posted by: Maxid Posted at: 2018-06-20T09:42:37.703Z Reads: 265

```
The battery compartment in the Lou is exactly the height of the battery inside the hardcase - no way to fit even a 1mm switch on top. But to put it somewhere else it needs to have a smaller footprint.
Well i guess my search continues.
```

---
## \#17 Posted by: Kug3lis Posted at: 2018-06-20T09:44:06.530Z Reads: 269

```
What current ratings you are looking into?
```

---
## \#18 Posted by: Maxid Posted at: 2018-06-20T09:57:05.326Z Reads: 280

```
Well the battery is 10S1P so even if i upgrade the cells to VTC6 I am looking at a max of 30A for short bursts (10s-30s otherwise voltage sag will probably cause an undervoltage error in the focbox anyway). I guess we are rather looking at 5A continuous or something like that. The original battery has XT30 connectors - that says it all :D
```

---
## \#19 Posted by: Kug3lis Posted at: 2018-06-20T10:03:32.198Z Reads: 280

```
I will try to think of something but no promises :)
```

---
## \#20 Posted by: Kug3lis Posted at: 2018-06-29T22:45:36.664Z Reads: 288

```
Today parts and PCB arrived, will be assembling several units and doing some basic testings

https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/4/5/4554252a067558445542f24e8b92b21e4e644766_1_375x500.jpg
```

---
## \#21 Posted by: Nordle Posted at: 2018-07-03T07:34:42.790Z Reads: 250

```
would you mind sharing the schematics? i’m doing a mouser order and need to reach 50€ for free shipping:)
```

---
## \#22 Posted by: tex Posted at: 2018-07-03T07:42:41.288Z Reads: 247

```
Really cool work ;)
```

---
## \#23 Posted by: Kug3lis Posted at: 2018-07-03T09:08:10.713Z Reads: 245

```
I don't understand how my product schematics are related with your mouser free shipping?
```

---
## \#24 Posted by: Maxid Posted at: 2018-07-03T10:36:37.275Z Reads: 242

```
This is not an OS thing like the Vedder/Fechter AS.
```

---
## \#25 Posted by: Nordle Posted at: 2018-07-03T12:02:36.060Z Reads: 247

```
[quote="Kug3lis, post:23, topic:59440, full:true"]
I don’t understand how my product schematics are related with your mouser free shipping?
[/quote]
i want to built a brake chopper, parts cost me 20€, i need an antispark too and would like one with a soft latching switch. so i doubt i could built this. no interest in making any profit with your design just deadbug one or two for myself:)

[quote="Maxid, post:24, topic:59440, full:true"]
This is not an OS thing like the Vedder/Fechter AS.
[/quote]
i know, i just asked:)
```

---
## \#26 Posted by: Kug3lis Posted at: 2018-07-03T12:35:13.155Z Reads: 233

```
It's not just schematic, it involves programming too, so sorry if you want this you will have to wait until it's available to buy. 

@Maxid yes this one is not OS
```

---
## \#27 Posted by: Nordle Posted at: 2018-07-03T12:57:53.056Z Reads: 232

```
no problem thanks anyways, will make one myself then;)
```

---
## \#28 Posted by: Kug3lis Posted at: 2018-07-04T11:04:35.576Z Reads: 236

```
Just a quick question before I do some changes to the board, would someone be interested in this "push to start" feature on this switch?
```

---
## \#29 Posted by: Vanarian Posted at: 2018-07-04T11:16:43.862Z Reads: 232

```
Nice job, any posible preview about pricing ? is the button area PCB soldered or there are pins to wire the button ?
```

---
## \#30 Posted by: Vanarian Posted at: 2018-07-04T11:17:46.621Z Reads: 231

```
Keep me updated on this ! Again I'm also willing to guinea pig for your design :beers:
```

---
## \#31 Posted by: Maxid Posted at: 2018-07-04T11:27:44.717Z Reads: 228

```
Can't imagine anybody saying no to that. Optimally there should be a way to use both - a switch or the push to start.
```

---
## \#32 Posted by: Jc06505n Posted at: 2018-07-04T12:11:29.290Z Reads: 219

```
At least [14 people would like that feature](https://www.electric-skateboard.builders/t/leisure-industry-features-that-we-could-implement/59201?u=jc06505n)
```

---
## \#33 Posted by: Colydog Posted at: 2018-07-23T02:09:45.045Z Reads: 209

```
Any update on this? I'll be looking to buy one soon but if they are going to be a while ill have to go with something else. 

Thanks for all your work.
```

---
## \#34 Posted by: Kug3lis Posted at: 2018-07-23T09:57:03.787Z Reads: 202

```
Should be available in around 1-2 weeks :)
```

---
## \#35 Posted by: ZmasteR Posted at: 2018-08-06T09:09:41.113Z Reads: 197

```
- 2 weeks later -
Hi there @Kug3lis
Sorry gotta ask :stuck_out_tongue: couldn't wait any longer are they operationnal ?
```

---
## \#36 Posted by: Kug3lis Posted at: 2018-08-06T09:10:32.724Z Reads: 194

```
We are waiting for parts to arrive and will be available to buy ;)
```

---
## \#37 Posted by: ZmasteR Posted at: 2018-09-06T15:03:50.613Z Reads: 187

```
By the way didn't ask but what would be (roughly) the price on this ?
```

---
## \#38 Posted by: Kug3lis Posted at: 2018-09-13T11:07:05.165Z Reads: 203

```
It should be in several price tiers based on current capacity you need.

Today we received parts and PCB left some changes for the firmware and it should be available by the end of week.

![image|375x500](upload://qIK4od2Qm5auiXIDYps8RCF1FXD.jpg)

![image|375x500](upload://ytaHJsssVSPJmGVs02nekyyEdYb.jpg)
```

---
## \#39 Posted by: L3chef Posted at: 2018-09-13T11:29:05.011Z Reads: 198

```
Make a 20s version thank you very much :yum:
```

---
## \#40 Posted by: Kug3lis Posted at: 2018-09-13T11:30:27.576Z Reads: 202

```
Well if you dont use push to start feature, you can use it until max mosfet voltage which is 100 :)
```

---
## \#41 Posted by: Kug3lis Posted at: 2018-09-13T11:34:40.420Z Reads: 196

```
By changing mosfets this switch can go up to 400V if anyone needs :D
```

---
## \#42 Posted by: L3chef Posted at: 2018-09-13T11:35:39.964Z Reads: 199

```
That's awesome! Do you have a final price for them? With heatsink
```

---
## \#43 Posted by: Kug3lis Posted at: 2018-09-13T11:37:30.473Z Reads: 202

```
Not yet

10char
```

---
## \#44 Posted by: Kug3lis Posted at: 2018-09-22T11:40:15.194Z Reads: 210

```
All the parts assembled firmware written and everything is tested. Just left to design a heatsink for it.

Here is small showcase video of it turning on by pushing board. Doesn't require any modifications :)

https://youtu.be/qe8vv5mZM0A
```

---
## \#45 Posted by: Kug3lis Posted at: 2018-09-22T18:41:53.446Z Reads: 209

```
So first batch of switches assembled now just left to make heatsinks.

![image|666x500](upload://d0brubQjyCy4zQTDCJFzoH1dgfA.jpeg) 

![image|666x500](upload://pDaZEtUFY7hleIphaI1A0HnwZaF.jpeg) 

## Final Feature List:

* Operational from 8S (25V) up to 19S with PTS or 22S without PTS (must be disabled) (80V with PTS or 100V without PTS)
* Turn on by pressing button (or if PTS enabled pushing your board)
* Turn off by holding a button for 2 sec
* When switch powered up you will hear beep pattern (in my opinion most important feature when having push to start)
* Enable/Disable Push-To-Start
* Pre Charge circuit (Hard limit inrush current limiter to pre-charge any size capacitor bank available on ESC side)
* High Side Power Switching (Positive wire is switched not negative)
* Current capabilities in 4 stages 50A, 100A, 150A, 200A (I know that mosfets are rated higher but its up to you mosfets will be heatsinked so you can try push more)
* Available in DIY style just the switch or fully assembled with push button and XT90 connectors.

## Pricing:

| Current Rating | Price for DIY style | Price for Kit
| ---------- | ------- | --- |
| 50A | 35€ | 55€
| 100A | 45€ | 65€
| 150A | 55€ | 75€
| 200A | 65€ | 85€

_* Prices don't include VAT or Shipping_

Specifications about size and weight will be announced tomorrow as heatsink is yet to be made. Should be available to purchase starting from next week.
```

---
## \#46 Posted by: Kug3lis Posted at: 2018-09-22T18:43:33.036Z Reads: 201

```
P.S. The higher current rating the less heat will be produced so if you concerned about heating issues grab the biggest one :sunny:
```

---
## \#47 Posted by: Kug3lis Posted at: 2018-09-22T20:02:29.947Z Reads: 205

```
Heatsink will look something like this:
![image|659x500](upload://7xex3iM7kS8qhrLDA1dchMx8yId.jpeg)

The heatsink will be around 53x35x8mm and total height should be less than 18mm or something like that :)
```

---
## \#48 Posted by: Kug3lis Posted at: 2018-09-23T15:29:06.716Z Reads: 205

```
So the switch is up online in the store :)

![image|375x500](upload://elg7Usmxp7PPRyCfVWpdTLMF2M9.jpeg) 

![image|375x500](upload://h6E2OIZ3NFAqjR1N4PWtAwDw0i0.jpeg) 

![image|375x500](upload://jNweea2wzTYmHsPJ124HIKj0450.jpeg) 

![image|375x500](upload://cLAPsoDGcs78ZKYPAywLVfFUNjB.jpeg) 

![image|690x274](upload://mIb1Zqs5xjIYpIddTXIyDUn9gQn.jpeg) 

https://shop.3dservisas.eu/collections/fatboy/products/fatboy-mini-sparky-switch-50a-200a-100v-pre-charged-anti-spark-switch-with-push-to-start
```

---
## \#49 Posted by: deucesdown Posted at: 2018-09-23T17:24:39.722Z Reads: 195

```
Awesome as usual. Is the amp spec the continuous, momentary burst, or "a few seconds" number?

With PTS can we run switch-less (like perhaps a timer to turn itself off)?
```

---
## \#50 Posted by: Kug3lis Posted at: 2018-09-23T17:29:09.123Z Reads: 198

```
Well amp settings are the same as esc :) At lower ratings it will warm quite a bit when running at the limits so I always suggest getting bigger as when less heat will produced and you will have some overhead :) Running continues for more than 5-10 min you will definitely will want attach it to something bigger metal or grab higher rating one :)

Regarding PTS there are no auto turn off timer, I don't like to have accidentally turn on board and wait till it turns off or anything happening automatically so for this reason both button and PTS work at the same time :)
```

---
## \#51 Posted by: thiswasandy Posted at: 2018-09-23T18:32:13.580Z Reads: 187

```
Ordered one.

Excited to have one of your products on one of my boards 😀
```

---
## \#52 Posted by: Kug3lis Posted at: 2018-09-24T13:20:21.805Z Reads: 174

```
Few more 100A and 150A added to the stock. More stock will be available with new parts arriving soon
```

---
## \#53 Posted by: Riako Posted at: 2018-09-24T13:47:03.649Z Reads: 170

```
[quote="Kug3lis, post:52, topic:59440"]
More stock will be available with new parts arriving soon
[/quote]

Tease us please :smile:
```

---
## \#54 Posted by: Gamer43 Posted at: 2018-09-25T08:03:52.884Z Reads: 163

```
I'm just curious, how does your switch generate the 12V bootstrapped rail for driving the high side N-Channel MOSFETS?

Also, couldn't a precharge transistor be avoided by adding a RC network between the mosfet driver, mosfet gate, and ground? That's what Linear Technologies recommends with their LTC700x line of high side mosfet drivers.
```

---
## \#55 Posted by: Kug3lis Posted at: 2018-09-25T08:13:42.946Z Reads: 159

```
It uses magic ;) Well mosfets don't like to work as linear regulators while you make them do pre-charge :) They work out of their comfort zone :) So I better dump everything through separate resistor :)
```

---
## \#56 Posted by: Gamer43 Posted at: 2018-09-25T09:06:35.913Z Reads: 167

```
Please don't tell me you are using a 555 Timer as a charge pump; I was considering that design, but I opted to spend the extra money for the LTC7004 (and PCBs to solder the pesky thing onto) instead.

I would highly recommend the LTC7000-1, you get 135V operation, current limiting feature, and no need for additional components aside from the transistors themselves and some passives. I think I saw someone else on this forum using that chip with some chassis mount MOSFET blocks, but he was charging well over $100 for it. 

You are right that it is best to avoid operating MOSFETs in their linear region, but sometimes you can cut costs :stuck_out_tongue: for both yourself and the end user with minimal impact on performance, or use a smaller transistor for pre-charging since it only needs to pass like 10% of the rated load current for a short time.
As long as you keep the slew rate reasonable with regards to the load capacitance, MOSFETs will have no problem operating in their linear region for a short period of time, just make sure to have a sufficiently long rise time (10-500ms) or to not exceed avalanche energy if the rise time is under 10ms, which shouldn't be a problem with International Rectifier MOSFETs since the actual MOSFET die is so big (this is also why their gate charge characteristics suck, but since this is a static application, that characteristic is irrelevant). 
If this method didn't work, Linear Technologies wouldn't recommend it in their datasheets and application notes.
```

---
## \#57 Posted by: Kug3lis Posted at: 2018-09-25T09:22:45.270Z Reads: 160

```
Yeah, I use 555 timer and some other logic chips to implement 4 bit MCU design for all the logic I am doing :laughing: 

It was me who made that switch but it wasn't using that chip and its solid switch. This switch if not MOSFETs and some other components can do up to 1000V ;)

Well, I am not a Chinese manufacturer to cut corners to increase profits, I want my device to be solid and robust and not just "working".

P.S. Not all application notes and datasheets are good examples to follow, from my experiences and some other well know engineers and some youtube guys have discussed this topic.
```

---
## \#58 Posted by: Gamer43 Posted at: 2018-09-25T10:13:35.703Z Reads: 166

```
So you are using a 555 TImer. :open_mouth: 

All manufacturers, not just Chinese, cut corners (civil engineering failures in the U.S. are clear indications of that), but there is a difference between cutting corners and adding unnecessary cost and complexity. Many times, it is best to keep it simple because it reduces the number of required components and allows you to provide a lower cost to your customers. 
LTC7000 -1 only needs like five extra passive components and the transistor. 
I literally plugged my switch in backwards (by mistake) and after correcting that, it still works no problem. 

But, I guess using a 555 Timer instead of a MOSFET Driver is already being cost efficient (50 cents for a CMOS 555 vs 4-5 dollars for the LTC7000).
I have no idea whether a 555 or the LTC7000 would be more rugged for this application :laughing:. I did blow up quite a few 555 Timers when I was prototyping my charge pump idea, but I've also blown up many bootstrapped MOSFET drivers (none from LT though, I did some crazy stuff to other LT chips and they didn't die, haha.)
If you want really rugged parts, try Allegro Microsystems, all their parts are automotive rated, and despite being shorted, overvolted, overheated, the chips I got from them still work perfectly fine. 

Most, if not all, datasheets from large semiconductor manufacturers contain good and reliable information. The issue is not with the datasheets or ANs, but that many engineers don't read them or misinterpret their information, and as result, end up selecting more expensive and inferior parts, or straight up select the wrong part altogether (there is this story of someone who was designing a triangle arduino board, and he ended up selecting the wrong 3.3V regulator or designed the PCB for it incorrectly because he neglected to read the datasheet, the enable pin ended up having inverted logic). 

It is impressive that you designed such a device to work off a 555 timer and implemented pre-charge functionality in such a small form factor and for only ~$40 despite the complexity. I was only able to figure out how to implement pre-charge on a lowside configuration :disappointed:. High side pre-charge is much more complicated; I'm guessing this is why Linear Technologies opted for the RC network approach.
```

---
## \#59 Posted by: Kug3lis Posted at: 2018-09-25T10:29:27.581Z Reads: 159

```
Yes, I have implement pre-charge, push to turn on, push and hold to turn off, push to start, beeper melody using 555 and some other logic elements :slight_smile:  Using only 11 components ;)
```

---
## \#60 Posted by: Gamer43 Posted at: 2018-09-25T10:47:53.388Z Reads: 157

```
Wow! Very cool.
I guess the next step would be to add a coulomb counter with bluetooth :laughing:.
```

---
## \#61 Posted by: Komamtb Posted at: 2018-09-29T15:28:29.117Z Reads: 148

```
Then the next batch will be in stock?
```

---
## \#62 Posted by: Riako Posted at: 2018-10-01T22:17:15.762Z Reads: 149

```
https://www.instagram.com/p/BoYxyf-A3YQ/?hl=fr&taken-by=riakobonito
Just received mine today !!
```

---
## \#63 Posted by: pylotope Posted at: 2018-10-23T15:01:31.344Z Reads: 144

```
@Kug3lis _Psst._ Make more. :wink:
```

---
## \#64 Posted by: Kug3lis Posted at: 2018-11-03T13:24:38.952Z Reads: 140

```
Switch is coming back in stock with some modifications for it :) At the moment its limited quantity

https://shop.3dservisas.eu/collections/fatboy/products/fatboy-mini-sparky-switch-50a-200a-100v-pre-charged-anti-spark-switch-with-push-to-start
```

---
## \#65 Posted by: Skunk Posted at: 2018-11-03T13:29:35.149Z Reads: 136

```
Figures you'd get more after i clean out my esk8 funds.... :man_facepalming:
```

---
## \#66 Posted by: Livid Posted at: 2018-11-03T13:31:31.360Z Reads: 134

```
How does the PTS work? I know the flipsky pts switch requires you to run a wire to a phase, same on this?
```

---
## \#67 Posted by: Kug3lis Posted at: 2018-11-03T13:32:09.118Z Reads: 131

```
No this, does not require any additional wiring :)
```

---
## \#68 Posted by: Livid Posted at: 2018-11-03T13:33:22.997Z Reads: 138

```
Very clever, I want one, if only i could afford it lol
```

---
## \#69 Posted by: Battosaii Posted at: 2018-11-09T22:57:43.500Z Reads: 132

```
when will this be back in stock?  old sparky just stopped working randomly i need something new lol
```

---
## \#70 Posted by: Kug3lis Posted at: 2018-11-09T22:59:17.330Z Reads: 138

```
Well it is in stock :) You mean the big one died? Did it stopped just by standing or you were tinkering with it?

https://shop.3dservisas.eu/collections/fatboy/products/fatboy-mini-sparky-switch-50a-200a-100v-pre-charged-anti-spark-switch-with-push-to-start
```

---
## \#71 Posted by: Battosaii Posted at: 2018-11-09T23:05:00.323Z Reads: 135

```
the 200a says out of stock.

yea it was most likely my fault i was setting up my board and wiring my button, i didnt short anything out but noticed my LED button would not turn off whether it was on or off and after turning it on and off a few times now it wont turn on. i checked out the pcb and didnt see anything weird or burnt. 

im running a 12s8p do you think the 150a would handle it or should i wait till you get 200A in stock?
```

---
## \#72 Posted by: Kug3lis Posted at: 2018-11-09T23:06:30.258Z Reads: 132

```
Ahh I see I fixed the stock :)

Were you touching mosfets bolts or etc? Can be ESD or etc killed it
```

---
## \#73 Posted by: Battosaii Posted at: 2018-11-09T23:08:22.958Z Reads: 134

```
im sure it was my fault but its sad to see it go to waste oh well.

thanks for updating im going to order it now and use a back up loop key for now :slight_smile:
```

---
## \#74 Posted by: Battosaii Posted at: 2018-11-09T23:12:06.537Z Reads: 138

```
done ordered, well this will simplify my build since theres no need for an inline fuse now and a big bulky antispark taking up space
```

---
## \#75 Posted by: Kug3lis Posted at: 2018-11-10T14:53:18.186Z Reads: 129

```
Updated stocks again after this rush of orders :) Will have to solder more but it will be shipped in the beginning of week :)
```

---
## \#76 Posted by: nuttyjeff Posted at: 2018-11-10T14:54:33.778Z Reads: 130

```
Is it possible to disable the stqrt up melody?
```

---
## \#77 Posted by: Kug3lis Posted at: 2018-11-10T14:55:46.272Z Reads: 127

```
I was just writing response for you :) Easiest thing is just to tape the hole on buzzer :) In newer PCB I will include jumper to disable buzzer :)
```

---
## \#78 Posted by: nuttyjeff Posted at: 2018-11-10T14:56:54.112Z Reads: 129

```
[quote="Kug3lis, post:77, topic:59440"]
In never PCB
[/quote]

In every* ?
```

---
## \#79 Posted by: Kug3lis Posted at: 2018-11-10T14:59:25.243Z Reads: 132

```
My mistake newer*
```

---
## \#80 Posted by: nuttyjeff Posted at: 2018-11-10T15:00:44.854Z Reads: 139

```
Ah ok. Cool. Thanks :slight_smile: , I've already ordered 1, so i guess i'm just going to have to tape the buzzer hole haha.
```

---
## \#81 Posted by: Kug3lis Posted at: 2018-11-10T15:02:17.205Z Reads: 146

```
Yes, it is already shipped :) But trust me the taping hole disables the whole sound of it... In first development I spent so much time trying to figure out why buzzer doesn't work.. It was just covered..
```

---
## \#82 Posted by: 3DServisas Posted at: 2019-01-05T23:53:43.076Z Reads: 132

```
Well it is in stock :slight_smile:

![IMG_1467|666x500](upload://tVaGerjjOUsCnUGJpbC0cgM39o7.jpeg)
```

---
## \#83 Posted by: 3DServisas Posted at: 2019-01-19T13:49:33.299Z Reads: 113

```
![IMG_1495|375x500](upload://fx4ivcq9atKiaOPRNX94q9S6yRx.jpeg)
```

---
## \#84 Posted by: Sender Posted at: 2019-01-19T13:59:04.399Z Reads: 110

```
Is this different or the same?  

BTW, my gear drives are fucking gorgeous, I am trying to hold off posting too many photos until I get the board up and running.
```

---
## \#85 Posted by: 3DServisas Posted at: 2019-01-19T14:06:01.749Z Reads: 112

```
Improved , Works with 4 VESC .
```

---
## \#86 Posted by: Acido Posted at: 2019-04-13T16:44:44.378Z Reads: 94

```
Interested how this works!
Hopefully this will be the last antispark I ever buy...
```

---
## \#87 Posted by: arturoluq1 Posted at: 2019-07-29T07:43:07.761Z Reads: 77

```
Is the 200A switch able to handle 120 continous current?
```

---
## \#88 Posted by: Kug3lis Posted at: 2019-07-31T09:23:12.337Z Reads: 74

```
If you talking continues current as in efoil and etc you will need to attach the metal part to some active cooling like metal plate which is exposed to water and etc. Esk8 does not have continues currents like efoils and etc, but switch can handle more than 200a if cooled efficiently
```

---
## \#89 Posted by: Jonisonvespa Posted at: 2019-08-13T02:22:14.323Z Reads: 65

```
just wondering why they dont have a fuse fitted?
```

---
## \#90 Posted by: Kug3lis Posted at: 2019-08-14T16:53:06.764Z Reads: 52

```
Mostly because of space issue, but we always recommend run fuse inline to connections.
```

---
## \#91 Posted by: 010203040506070809 Posted at: 2019-10-02T16:22:00.633Z Reads: 36

```
What's the power draw when turned off? How long would a 10s battery last if I don't charge it?
```

---
