# DieBie JTAG 12s BMS &#124; Gauging Interest &#124; NONPROFIT

### Replies: 467 Views: 24764

## \#1 Posted by: fedestanco Posted at: 2017-04-13T19:11:23.929Z Reads: 1064

```
In the past months @jtag worked on a smart programmable bms capable of high current flow (**check the** [original thread](https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639) **for specs**). He shared every single step on [github](https://github.com/DieBieEngineering) and he did it for free.
Unfortunately he doesn't have time to carry on the production but he left all the necessary for someone else to do it. I didn't want this project to be buried in the forum so I contacted several (tens) factories and came up with this:
## Prices
In the spirit of the original project I will handle all the production, payments, shippings totally nonprofit. My calculations for a 20pcs batch are the following:
pcb factory+ pick and place robot labour+ metal stencil factory+ BOM+ shipping to my home+ 24% VAT and duties= **from 90 to 110€** (this oscillates because of components prices) for a complete, fully assembled product.

I will ask you to make a **"mandatory donation" of 10€/bms** to @JTAG paypal link (if he wants to provide one :wink:) .

## Quality
**PCBs**: FR4; 2oz copper on inner and outer layers; gold immersion; "flying probe" testing.
**Industrial metal stencil**: laser etched; medium thickness stainless steel.
**Automated assembly**: lead-free; carried out by these machines: YS24, YS12, YV100XG, Heller reflow oven; AOI testing.
**BOM**: of course I will provide the factory with original components sourced in Europe (for ex. Wurth) and in China. 

## a little help on the firmware please...
To be honest I don't have any idea on how to upload the [firmware](https://github.com/DieBieEngineering/DieBieMS-Firmware) on the ICs. I would truly appreciate if **somebody experienced** could make a step by step video, so that me or a chinese guy at the factory can make the hardware working.



## Let me know if you are interested (we need 20 boards minimum for a reasonable price) SIGN UP HERE https://goo.gl/forms/rx24hQARRauqUp452

...and if you have useful suggestions...Thanks!

:arrow_double_down:                             :arrow_double_down:
```

---
## \#3 Posted by: jackw Posted at: 2017-04-13T19:28:07.489Z Reads: 817

```
I would probably be in for one, whats a rough timeframe here?
```

---
## \#4 Posted by: fedestanco Posted at: 2017-04-13T19:35:56.998Z Reads: 794

```
1 week for pcbs, 1-3 days for automated assemby, 5-10 days for shipping to me+ customs+repacking. BOM gathering is not predictable yet, probably less than 2 weeks (this can be done at the same time of pcb manufacturing).
```

---
## \#5 Posted by: SirDiff Posted at: 2017-04-13T21:54:37.112Z Reads: 770

```
I'm not jumping on this one because I'm pretty broke and don't need a bms right now, but I can tell you that fedestanco works very well with these group buys/non or very little profit productions. I bought from him and he knows what he's doing, if any of you is hesitant because of the recent problems happened on group buys, don't worry about this one. Good luck, this is a great deal!
```

---
## \#6 Posted by: Blacksheep Posted at: 2017-04-13T22:20:48.935Z Reads: 716

```
Maybe one maybe
```

---
## \#7 Posted by: boards Posted at: 2017-04-14T01:17:51.125Z Reads: 678

```
i don't get it, don't you like getting goods and services?
```

---
## \#8 Posted by: NickTheDude Posted at: 2017-04-14T01:33:09.753Z Reads: 651

```
I'm no expert so I don't quite understand the specs from the other thread. So, if it comes with a switch and can handle 60A at 12S then I'm in.
```

---
## \#9 Posted by: fedestanco Posted at: 2017-04-14T03:07:56.642Z Reads: 647

```
Few specs from the original thread: up to 12s (4,2*12= 50.4v); technically up to 140Amp, tested up to 100 if I am not wrong.

I dont loose or gain anything if this GB reaches the goal or not. However this is the "vesc of BMSs" so the winners will be the buyers and the community itself 😄.

You can still make it yourself and have fun doing it! I am just bringing an "open source pro-manufacturing" probably for a lower price 😉.
```

---
## \#10 Posted by: Tarzan Posted at: 2017-04-14T07:10:31.525Z Reads: 605

```
I'm interested!
```

---
## \#11 Posted by: IDVert3X Posted at: 2017-04-14T09:33:10.946Z Reads: 628

```
[quote="fedestanco, post:1, topic:20947"]
To be honest I don't have any idea on how to upload the firmware on the ICs. I would truly appreciate if somebody experienced could make a step by step video, so that me or a chinese guy at the factory can make the hardware working.
[/quote]

It uses STM32F303 microcontroller, you will need STLink ( programmer ) to upload the firmware.
You can use ST-Link V2 Utility ( software ) to upload the binaries and verify the contents of memory.
```

---
## \#12 Posted by: fedestanco Posted at: 2017-04-21T18:50:43.822Z Reads: 628

```
Hi guys I obtained few pics of both factories' previous works. <img src="/uploads/db1493/original/3X/0/d/0d7fd3c277463a90569ba302ccf5341e94843976.jpg" width="690" height="429"><img src="/uploads/db1493/original/3X/9/9/990133ec12e2a56b3a3fb4eaf75998800ed85faa.jpg" width="690" height="412"><img src="/uploads/db1493/original/3X/d/a/dab0371e0317e26a03170e2ba977dcc533104f60.jpg" width="500" height="500"><img src="/uploads/db1493/original/3X/7/4/7436d9c0fb6817fabfb1f05d2fa68dd8b3144993.jpg" width="500" height="500"><img src="/uploads/db1493/original/3X/a/2/a27ef097776806d5e47168f5bc03186f6058896c.jpg" width="500" height="500">

I will open a google form. Once it reaches 20 orders I can start gathering payments and planning the production.
```

---
## \#13 Posted by: Pantologist Posted at: 2017-04-25T01:30:29.712Z Reads: 554

```
Nice, how much will shipping to the USA be, roughly?
```

---
## \#14 Posted by: TarzanHBK Posted at: 2017-04-25T06:35:59.646Z Reads: 541

```
was this bms programmable to set values by yourself? Suitable for lifepo4?
```

---
## \#15 Posted by: fedestanco Posted at: 2017-04-25T11:58:51.049Z Reads: 544

```
@TarzanHBK quote readme: " Cell voltage range 2.5V to 4.5V" maybe @JTAG can confirm.

@Pantologist 4,6€ untracked (if the bms weights 100g).
```

---
## \#16 Posted by: TarzanHBK Posted at: 2017-04-25T12:14:48.536Z Reads: 538

```
alright I just figured out : "Chrome based programming"
So should be easy after a firmware upload to set parameters
```

---
## \#17 Posted by: fedestanco Posted at: 2017-04-25T19:07:06.152Z Reads: 543

```
## Sign up here if you are interested
https://goo.gl/forms/rx24hQARRauqUp452
```

---
## \#18 Posted by: riva_00 Posted at: 2017-04-25T20:01:45.309Z Reads: 544

```
I've just signed for 2, can you post the dimensions? Can't seem to find them on the main thread.

Edit - found them, 140x60x15mm LxWxH
```

---
## \#19 Posted by: rwxr Posted at: 2017-04-27T07:43:14.405Z Reads: 531

```
150mm height?
```

---
## \#20 Posted by: fedestanco Posted at: 2017-04-27T08:17:37.697Z Reads: 523

```
15mm height https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/65?u=fedestanco
```

---
## \#21 Posted by: riva_00 Posted at: 2017-04-27T09:13:52.744Z Reads: 515

```
I've haven't edited my post, it always said 15mm height :)
```

---
## \#22 Posted by: Brad Posted at: 2017-04-27T10:25:47.984Z Reads: 456

```
I will buy one off you.
```

---
## \#23 Posted by: Okami Posted at: 2017-05-20T19:37:42.099Z Reads: 450

```
Hi! @fedestanco is it still needed to 'promote' this production run?

There might be a few ebike people interested in such setup with this level of customization.

I just want to know is it still worthwhile to share the info with them unless you have also posted on Endless Sphere forums?
```

---
## \#24 Posted by: fedestanco Posted at: 2017-05-21T04:28:32.850Z Reads: 449

```
Yes I gave my availability to put this into production whenever 20 requests are reached (see form above).
```

---
## \#25 Posted by: Okami Posted at: 2017-05-21T12:35:39.503Z Reads: 470

```
Ok will proceed with this further then. Im pretty sure some of them should be able to use 12S and there are people who put even a few thousand on their tuned ebikes..

@fedestanco As I understand - I can share this link:

https://github.com/DieBieEngineering/DieBieMS

As that is the most documented one of what the BMS is going to offer right?

And then I just send them here.

Do you also have some sort of email, so they wouldnt need to log on to the forum?

--

Ok done, shared on facebook group and if needed, maybe a notice in forum itself would be also good. 12S is not that low after all, even if some of them use 14s+ voltages.
```

---
## \#26 Posted by: fedestanco Posted at: 2017-05-21T14:18:39.284Z Reads: 425

```
Great! I'd love to see this project spread over as much as possible.
```

---
## \#27 Posted by: Pantologist Posted at: 2017-05-27T02:25:32.654Z Reads: 415

```
How many people are interested so far?

Form: https://goo.gl/forms/rx24hQARRauqUp452
```

---
## \#28 Posted by: fedestanco Posted at: 2017-05-27T02:37:14.209Z Reads: 404

```
14 bmss right now, 6 left.
```

---
## \#29 Posted by: Pantologist Posted at: 2017-05-27T02:41:31.179Z Reads: 400

```
You should add the google forms link to the original post so people can find it easily.
```

---
## \#30 Posted by: fedestanco Posted at: 2017-05-27T18:57:36.555Z Reads: 394

```
Done. 10 char
```

---
## \#31 Posted by: zeno Posted at: 2017-05-30T19:43:47.004Z Reads: 388

```
Plus one for me :) (added to the Google form already)
```

---
## \#32 Posted by: fedestanco Posted at: 2017-05-30T19:47:09.773Z Reads: 382

```
I might be able to start this in 10days. Lets see if we can hit the 20 by then.
```

---
## \#33 Posted by: Pantologist Posted at: 2017-06-06T18:53:13.415Z Reads: 369

```
Anyone else interested?
```

---
## \#34 Posted by: fedestanco Posted at: 2017-06-06T19:29:57.616Z Reads: 368

```
We are at 18 now btw.
```

---
## \#35 Posted by: Brad Posted at: 2017-06-07T08:28:36.731Z Reads: 364

```
That is good news.

Will have to put my build on hold till I get one of these babies
```

---
## \#36 Posted by: jaysoncena Posted at: 2017-06-07T11:40:53.640Z Reads: 352

```
Anyone knows how settings can be updated on this BMS?
```

---
## \#37 Posted by: lock Posted at: 2017-06-08T02:27:43.141Z Reads: 378

```
Good question, which leads to further questions🤔.

Worst case I'd say you have to clear the storage on the chip, change config parameters in the source code, build, and upload to device. The default parameters are laid out nicely in [`modConfig.c`](https://github.com/DieBieEngineering/DieBieMS-Firmware/blob/master/Modules/Src/modConfig.c#L10) ... I'm guessing some of the comments haven't kept up with the actual values.

        // VALUES WILL ONLY UPDATE AFTER FLASH ERASE!
		modConfigGeneralConfigStructTypedef defaultConfig;
		defaultConfig.noOfCells 			=	6;			// 12 Cells in series
		defaultConfig.batteryCapacity		=	10.00f;		// 12Ah battery
		defaultConfig.cellHardUnderVoltage	= 2.40f;		// Worst case 2.4V as lowest cell voltage
		defaultConfig.cellHardOverVoltage	= 4.45f;		// Worst case 4.35V as highest cell voltage
		defaultConfig.cellSoftUnderVoltage	= 2.60f;		// Normal lowest cell voltage 2.6V
        ...
        ...

Best case is that someone writes an app for Win/Linux etc that writes those values direct to the EPROM via a USB connection. The dev tools may let you do this already.

There's little documentation in the repo on how you would build and deploy the firmware. Seems JTAG is using the [Keil ARM](https://www.keil.com/) development tools for this(???). It's a commercial dev environment and there may be some licensing cost (depends how big the firmware is). I'd probably be happier if it was a Makefile and list of Ubuntu packages... but don't even know if that's feasible. I'm certainly no embedded systems developer.

A lot of work has gone into this project, it'd be a real shame not to see it picked up. Real question is for @JTAG, do you have any time to deal with some support questions that may come up? Maybe even a quick tutorial (youtube, blog post) on what we'd need to build and deploy the firmware.

I'm pretty close to signing up, this looks like a great and much needed project.
```

---
## \#38 Posted by: JTAG Posted at: 2017-06-08T11:04:05.433Z Reads: 379

```
Hi guys!

Indeed the comments behind the default config do not always match with the code. I have about 8 DieBieMS es in use in various applications, I need to change the source and upload every time a different BMS battery combination needs programming. It indeed needs a UI that can do this :sweat_smile:.

Yeah modConfigGeneralConfig stores all battery dependant parameters in runtime, it gets loaded from flash emulated EEPROM at startup. For now indeed the only way to change the battery parameters is to change the values in the source code in the defaultConfig. The defaultConfig strucht get stored when the EEPROM is empty (at first run of the code).

Everything is written such that it should be easy to make a PC UI to changes these configuration values in runtime and store them. My main focus was on the safety systems in the firmware and fixing bugs that occur in very rare circumstances. For the past months I have been intensively riding my skateboard and electric scooter that both have a DieBieMS managing the battery, beating the bugs that I found. For the past three weeks everything works perfect and as expected. 

Making a chrome app it comply new to me. I think Ill first make a quick and dirty nodejs command line tool to change the parameters, that will be very easy and cross platform. There are probably very talented people around here that could polish the pc app and make it into a shiney UI. My specialties are hardware en embedded software, I can do PC software but not to a production level :P.
```

---
## \#39 Posted by: lock Posted at: 2017-06-08T11:36:02.107Z Reads: 353

```
Ok @fedestanco, I'm in for 2 assuming you're ok shipping to Australia. One to use, another to play around with.

The nodejs command line interface sounds great @JTAG.  It'd be a great starting point for someone to pickup from and make something a bit more pretty.
```

---
## \#40 Posted by: fedestanco Posted at: 2017-06-08T12:07:20.170Z Reads: 357

```
Well I guess I can start collecting the money. 
I will double check the BOM cost, yuan-euro exchange rate and wire transfer fees to give the most accurate final price. 

Since the final weight is unknown, I cannot calculate the shipping costs to your home, thus I will now ask you all to pay JUST FOR THE BMS.

Once I get the boards at home I will eventually ask you a second payment for the SHIPPING TO YOU.

@JTAG  do you believe the quality standards I listed in the first post are up to the task or you have special standards to be applied?
```

---
## \#41 Posted by: JTAG Posted at: 2017-06-08T14:47:39.728Z Reads: 332

```
No, everything is standard process!
```

---
## \#42 Posted by: chsknight Posted at: 2017-06-21T21:02:33.010Z Reads: 299

```
Any updates!  This BMS would be clutch in my build.
```

---
## \#43 Posted by: fedestanco Posted at: 2017-06-21T21:55:15.803Z Reads: 307

```
Yes! When I do group buys I never collect the money untill I can focus 100% to bring them from start to end. Right now (and for at least a week) I cant spend time on this because of exams.

If you guys prefer I can start collecting money but bear in mind that they will remain unused in my paypal for a while.
```

---
## \#44 Posted by: Pantologist Posted at: 2017-06-22T02:19:53.957Z Reads: 321

```
What is roughly the final bill for 1 BMS to the US?

Also does it come with the balance cables? That shouldn't be hard to get but I'm just wondering.
```

---
## \#45 Posted by: fedestanco Posted at: 2017-06-22T08:11:08.691Z Reads: 308

```
The complete bms will be 100€ or less. Since fuse, balance cables, switch and screen cables are not included in the bom I did not include them in the price but I can order them for you.
Maybe they will add another 4/5€. Will calculate that later.
```

---
## \#46 Posted by: Steve-81 Posted at: 2017-07-02T10:59:23.561Z Reads: 314

```
Hello, I just signd up for a BMS, I really love the way how this pcb is designed.
Can it be possible, to count with that extra 4-5 €, so everything comes together, no need to search fir missing parts?
```

---
## \#47 Posted by: SkaterBoy58 Posted at: 2017-07-03T05:58:33.697Z Reads: 320

```
Have just signed up for 2 
Cheers
```

---
## \#48 Posted by: riva_00 Posted at: 2017-07-03T11:54:51.970Z Reads: 312

```
I'd defo order the extra cables with the BMS, saves hassle really...
Looking forward to this hardware :slight_smile:
```

---
## \#49 Posted by: fedestanco Posted at: 2017-07-03T16:30:04.082Z Reads: 317

```
As I said I am in the middle of my finals. Soon I will be able to search for cables, fuses and lcds.

I am sorry if this delay is affecting your projects.
```

---
## \#50 Posted by: Steve-81 Posted at: 2017-07-03T21:40:40.031Z Reads: 302

```
No worries man :) Thank you for your respond, so I know I am not late, and the whole projekt is still on :)
```

---
## \#51 Posted by: riva_00 Posted at: 2017-07-04T11:20:35.118Z Reads: 305

```
Take your time m8y.
Best of luck with your finals.
```

---
## \#52 Posted by: banjaxxed Posted at: 2017-07-05T00:20:18.717Z Reads: 305

```
Signed up for two thanks, don't have an android device only iOS hopefully won't be a problem.

Would also like balance wires -
2 x s10
1 x s12

Cheers
```

---
## \#53 Posted by: emepror Posted at: 2017-07-05T01:38:41.396Z Reads: 290

```
What specifically are you looking for? I believe the fuses are littelfuse brand. I might be able to help figure out the rest of it if you need a hand.
```

---
## \#54 Posted by: fedestanco Posted at: 2017-07-05T10:31:22.135Z Reads: 296

```
Fuse model is littelfuse bf1 58v and price is pretty high in europe (2,3€). 

The connector is used in the automotive industry afaik so it wont be diffucult to have it precrimped in china ( @banjaxxed I will order them all with 16 cables assembled so both for 12s or 10s I will send you the same cable).
Only one thing: @JTAG do you know if this molex connector is compatible http://www.molex.com/molex/products/datasheet.jsp?part=active/0430251600_CRIMP_HOUSINGS.xml if not I will order the wurth one.
```

---
## \#55 Posted by: oyta Posted at: 2017-07-05T21:39:36.453Z Reads: 270

```
I am in! The BMS looks good! Love the features!
```

---
## \#56 Posted by: banjaxxed Posted at: 2017-07-06T04:02:55.517Z Reads: 264

```
Ok thanks fedestanco, I was in fact looking really for an extra cable for another 10s bms I bought from Banggood. maybe forget it and just send with cables for the two bms I would like from this group buy thanks
```

---
## \#57 Posted by: Steve-81 Posted at: 2017-07-07T07:16:19.258Z Reads: 264

```
@fedestanco I hope you are getting on well with your finals. I don't want to disturb you, just would like to know, what can be counted for arrival of this beauties? I’m just planning to build my first mountain board (not a Trampa), and I ordered the vescs, batteries already. Still looking for the right 6374 outrunners. I know my build will not be cheap, but I really want a board that can be used for ages.
```

---
## \#58 Posted by: fedestanco Posted at: 2017-07-07T08:48:39.674Z Reads: 290

```
From the day I pay the factories:
 [quote="fedestanco, post:4, topic:20947, full:true"]
1 week for pcbs, 1-3 days for automated assemby, 5-10 days for shipping to me+ customs+repacking. BOM gathering is not predictable yet, probably less than 2 weeks (this can be done at the same time of pcb manufacturing).
[/quote]
```

---
## \#59 Posted by: Steve-81 Posted at: 2017-07-07T12:50:30.347Z Reads: 286

```
Sounds good, when will you start collecting money?
Did you pass finals?
```

---
## \#60 Posted by: fedestanco Posted at: 2017-07-07T15:27:41.527Z Reads: 311

```

## LET'S START : I will contact you by email and/or PM to inform you about my paypal address and the amount
As I already said the price is not definitive : depends on components availability, tax, shipping weight and final quantity. For this reason payments will be organized as following:
**1st payment** : possibly before the end of next week to cover my extimation of the production costs

**2nd payment**: when the bmss arrive and I can weight them and purchase the shipping labels 
(The 2nd one will also cover any price adjustment; example: VAT turns out to be 3$ cheaper --> you will pay 3$ less on the second payment)

------------
My only concern:  if you all send money by "good and services" this could happen https://youtu.be/t1rYgD8luGw :basically this guy organized a big group buy and **paypal froze the money until all the items were delivered**. If this happened I woulnt be able to pay for the production and items couldnt be delivered...

I know there have been quite a few scams on this forum, so **some of you may not feel confident in sending me your money through "friends and family"**. If these people are just a few, then they can try "good and services" and we will see if paypal is  fine with it.

BTW I have proven many times not to be a scammer :see my past group buys and personal sales I made on this forum.
```

---
## \#61 Posted by: fedestanco Posted at: 2017-07-07T17:18:45.627Z Reads: 283

```
Message/email sent. If you haven't received it PM me please.
```

---
## \#62 Posted by: Sander Posted at: 2017-07-07T18:41:30.301Z Reads: 252

```
Have you tried https://www.pcbway.com ?
I think the assemble might be cheaper, im not sure.
```

---
## \#63 Posted by: DoubtingThomas Posted at: 2017-07-07T19:08:47.602Z Reads: 248

```
I've sent payment. Thank you again for all your work !
```

---
## \#64 Posted by: fedestanco Posted at: 2017-07-07T19:28:11.727Z Reads: 255

```
Can you check please and tell me the prices?
I am open to all the options.

Btw the most expensive part of the production is the assembly because it is carried out by ipc certified pick and place machines and it is not done by hand.
```

---
## \#65 Posted by: SirDiff Posted at: 2017-07-07T19:53:10.785Z Reads: 255

```
[quote="fedestanco, post:60, topic:20947"]
some of you may not feel confident in sending me your money through "friends and family"
[/quote]

I can't guarantee for any of you, but I can confirm that he's done some pretty successful group buys, providing assistance even after the delivery of the items. He's a good guy from what I've seen :)
```

---
## \#66 Posted by: Sander Posted at: 2017-07-07T20:05:57.195Z Reads: 249

```
How many layers are the BMS?
```

---
## \#67 Posted by: fedestanco Posted at: 2017-07-07T20:07:21.373Z Reads: 245

```
2 oz, gold immersion, 4 layers. And I also asked for rohs compliant materials.
```

---
## \#68 Posted by: Sander Posted at: 2017-07-07T20:12:23.349Z Reads: 257

```
**For 20 PCBs**
**PCB Cost:** US $ 91
**Assembly Service Cost:** US $ 440
**Shipping:**US $ 24
**Total**: US $ 555

So, 1 PCB Assembled cost 555/20 = 27.5 USD + Components that might cost around 50 USD? 
That will be 77.5USD.

Btw you will receive them after 1 week or before.
```

---
## \#69 Posted by: fedestanco Posted at: 2017-07-07T20:18:54.639Z Reads: 246

```
The price is indeed similar, maybe a bit higher after tax. Would you mind asking also a quote for the BOM? Having all done by 1 factory would definitely be easier.

And the most important thing: is the assembly cost referring to automatic or hand soldering?
```

---
## \#70 Posted by: Sander Posted at: 2017-07-07T20:20:18.598Z Reads: 245

```
Sure!
- - -- - - -- - - -
```

---
## \#71 Posted by: fedestanco Posted at: 2017-07-09T14:09:39.595Z Reads: 243

```
UPDATE. Received payments for 10 bmss. I hope to see the another 10 payments in the upcoming week considering 25 people filled the form :) .
```

---
## \#72 Posted by: fedestanco Posted at: 2017-07-10T12:45:41.934Z Reads: 242

```
Hi, have you had a quotation back? 

Btw I just read the last part of your message: no way the BOM is only 50€. At the very least, soucing parts from the cheapest resellers it comes down to 65€; really, check it out.
```

---
## \#73 Posted by: Sander Posted at: 2017-07-10T13:48:24.079Z Reads: 245

```
I think the pcbway is too expensive for quantities like 20.
```

---
## \#74 Posted by: fedestanco Posted at: 2017-07-10T14:05:44.849Z Reads: 247

```
I agree on that. The price point I am at is 85€ (100€ with vat, which is a real thing even for small quantities http://www.electric-skateboard.builders/t/raphael-chang-bms-and-esc/8952/321?u=fedestanco) and I truly believe it is not quite possible to go lower without loosing quality.
For instance at this price point we could make vesc 4.12 for about 65€.
```

---
## \#75 Posted by: lock Posted at: 2017-07-11T07:05:01.127Z Reads: 238

```
FWIW I did upload the BOM to Element14 (Farnell) and it came out to what would be equivalent to 100euro (single order). That wasn't including some components, and no PCB or assembly. The supplier you've found seems pretty good 👍.

Interesting the bolt on connectors seemed to be one of the more expensive components. Guess you could do a cheaper build without some of them, but I quite like the idea of being able to bolt on (instead of solder) live wires.
```

---
## \#76 Posted by: fedestanco Posted at: 2017-07-11T07:34:16.997Z Reads: 231

```
Little update: 9 BMSs left to pay.
```

---
## \#77 Posted by: Steve-81 Posted at: 2017-07-11T10:13:32.679Z Reads: 232

```
You said 25 BMS-s where pre-ordered. I really hope the missing 9 pcs will be payed ASAP. Would be a shame to quit such a good looking, probably well function BMS.
```

---
## \#78 Posted by: fedestanco Posted at: 2017-07-11T11:01:42.700Z Reads: 239

```
Actually 25 responses, which translates into 35 bmss booked. Probably some people still arent aware that I am collecting payments.

Btw one more has been paid: 8 to go.
```

---
## \#79 Posted by: Brad Posted at: 2017-07-11T11:23:39.112Z Reads: 235

```
Slowly but surely :cold_sweat:
```

---
## \#80 Posted by: Steve-81 Posted at: 2017-07-11T11:59:10.339Z Reads: 238

```
Maybe we should write them all e-mails. (I meen all people who payed should write to all who didn't).with a writing like:

"fedestanco at esk8 started collecting money for the DieBieMS, try to not be cut off from such a cool BMS"

nothing more, just that they see a lot of mails going into their mailbox :)
```

---
## \#81 Posted by: longhairedboy Posted at: 2017-07-11T13:03:47.148Z Reads: 239

```
its not too late is it? i just signed up. I need these badly. Not in an immediate sense, but more in a long term i need a reliable and more feature rich BMS that does all of these things.
```

---
## \#82 Posted by: fedestanco Posted at: 2017-07-11T13:22:32.253Z Reads: 218

```
@Steve-81 Initially the form was just to check interest so no email address was asked to the very first participants. I admit it was a huge mistake.

@longhairedboy I pm'd you the instructions to the payment.
```

---
## \#83 Posted by: Brad Posted at: 2017-07-11T13:23:18.323Z Reads: 215

```
I remember you saying you wanted to buy 10! I understand that might be in jest, but if you would buy the remaining 8, that would be awesome!
```

---
## \#84 Posted by: fedestanco Posted at: 2017-07-11T13:27:59.374Z Reads: 222

```
In the US you have to pay import tax over 800$ if I remember right, so I would suggest not to take more than 7 to avoid such taxes.
```

---
## \#85 Posted by: fedestanco Posted at: 2017-07-11T13:48:57.914Z Reads: 220

```
Update: just 4 are unpaid !
```

---
## \#86 Posted by: longhairedboy Posted at: 2017-07-11T13:49:31.568Z Reads: 226

```
i just bought 4. 

10 was a slight exaggeration for a sample amount, but beleive me, if these guys work out.. i will be ordering them by the 10's. 

Also as a side note i'm doing insane things with a 13S BMS i just got from battery supports involving an unwitting focbox but that's off topic.
```

---
## \#87 Posted by: JTAG Posted at: 2017-07-11T14:50:39.280Z Reads: 226

```
You must be the one and only guy who likes the smell of DRV in the morning don't you :innocent:?
```

---
## \#88 Posted by: longhairedboy Posted at: 2017-07-11T14:56:07.240Z Reads: 232

```
the smell.. the feel.. the aroma and sensation.. of magic smoke is alluring.. intoxcating... i must have more burning componentry in my sphere of being..
```

---
## \#89 Posted by: flatsp0t Posted at: 2017-07-11T19:08:51.708Z Reads: 235

```
Sorry, i was on my hard earned "no mails"-vacation, will pay ASAP.
@fedestanco i am not sure, did i order one or two?
```

---
## \#90 Posted by: fedestanco Posted at: 2017-07-11T19:26:06.471Z Reads: 229

```
Take as many as you need. We are at 19 currently so yours could be the last one.
```

---
## \#91 Posted by: flatsp0t Posted at: 2017-07-11T19:27:16.717Z Reads: 232

```
i am pretty sure i had just one, just did not want to mess sth up with you planning.
```

---
## \#92 Posted by: flatsp0t Posted at: 2017-07-11T19:31:41.288Z Reads: 227

```
Money sent.
```

---
## \#93 Posted by: fedestanco Posted at: 2017-07-11T19:41:57.999Z Reads: 234

```
Received. We are full. 
Tomorrow I will place the first order for all the Wurth components. 
Special thanks to @DoubtingThomas since he agreed to forward the stuff to me from Germany.
```

---
## \#94 Posted by: fedestanco Posted at: 2017-07-11T22:54:08.245Z Reads: 238

```
VOTE ONLY IF YOU ARE A "BACKER", thanks

FUSE POLL: Please choose the amperage that best suits you needs. To make things easier, everybody will get the same (the winner).

[poll type=regular public=true]
* 60 amps
* 80 amps
* 100 amps
[/poll]
```

---
## \#95 Posted by: Pantologist Posted at: 2017-07-12T00:55:20.799Z Reads: 228

```
The current draw can be adjusted on the vesc and the BMS itself so this is really just for protection in case of a short, so I'd say 80A or 100A.
```

---
## \#96 Posted by: fedestanco Posted at: 2017-07-12T17:56:23.393Z Reads: 232

```
Fuse will be 100A.
First order placed in Germany.

Need to buy an ST LINK for programming, suggestions are appreciated.
```

---
## \#97 Posted by: Steve-81 Posted at: 2017-07-14T10:24:45.828Z Reads: 231

```
The only site I found is:
http://www.st.com/en/development-tools/st-link-v2.html
they have European distributors, and price isn't bad at all, something about 23-25 USD.
I'm not home in those things, but it says it works on STM8 and STM32 too.
```

---
## \#99 Posted by: Brad Posted at: 2017-07-15T01:00:18.880Z Reads: 241

```
Nice find.

I thought I found one also on [](diy-electric-skateboard-kits-parts/vesc-usb-programmer-stlinkv2/), but it stated it for programming ESCs.(not sure it can work on BMS as in erase current esc data and put on BMS program) $15USD.
```

---
## \#100 Posted by: chinzw Posted at: 2017-07-15T02:08:48.889Z Reads: 252

```
The VESC is STM32 so that should work just fine for the BMS as well
BTW, its very easy to find STM programmers:
https://www.adafruit.com/product/2548
http://ca.mouser.com/ProductDetail/STMicroelectronics/ST-LINK-V2/?qs=H4BOwPtf9MC1sDQ8j3cy4w%3D%3D
https://www.digikey.ca/product-detail/en/stmicroelectronics/ST-LINK-V2/497-10484-ND/2214535
```

---
## \#101 Posted by: rpn314 Posted at: 2017-07-17T02:01:55.087Z Reads: 244

```
I have one of these. No problems uploading the boot-loader to a new VESC; should work for what you need.
http://www.ebay.com/itm/STLink-V2-Programmer-Unit-Metal-Shell-STM8-STM32-Emulator-Downloader-DIY-/162195254305?hash=item25c3972c21:g:Z-YAAOSwMgdX0NYc
```

---
## \#102 Posted by: fedestanco Posted at: 2017-07-17T11:14:29.916Z Reads: 243

```
UPDATE: 
Cables all ordered and are being crimped; they are 4/bms and came out 3,5€/bms. There is no more margin for a fuse so I will just give back 0,5€ in the next payment.
The balance cable is custom crimped and I choose 50cm 22awg balance leads.

COMPONENTS: jtag just confirmed the BOM so I can now place the big order
Wurth stuff has been ordered BUT there are few screwholders in backorder. I hope they wont take much to restock.

PCBassembly and PCBs are still not paid because jtag wanted to double check the files (very nice of him).
```

---
## \#103 Posted by: JTAG Posted at: 2017-07-17T23:09:30.197Z Reads: 227

```
[quote="fedestanco, post:102, topic:20947"]
im).
[/quote]

Yes, Ill start checking tomorrow!
```

---
## \#104 Posted by: jos Posted at: 2017-07-18T12:00:49.769Z Reads: 227

```
@JTAG where did you buy your fuses? All the places I found had a MOC of 500... One extra may be good to have, but 499 seems like overkill :)
```

---
## \#105 Posted by: JTAG Posted at: 2017-07-18T12:06:49.072Z Reads: 230

```
http://nl.farnell.com/littelfuse/153-5631-6101/bolt-on-fuse-slow-blow-100a-32v/dp/2508414

I order so much by them I must be shareholder by now xD.
```

---
## \#106 Posted by: fedestanco Posted at: 2017-07-18T12:50:21.581Z Reads: 228

```
Isnt 32v the wrong model? I thought 58v was the right one.
```

---
## \#107 Posted by: jos Posted at: 2017-07-18T12:52:04.396Z Reads: 231

```
I was looking for the 58V rated one, which seems much harder to find. Do you think it's OK to use the 32V rated fuse in a 10S setup?
```

---
## \#108 Posted by: JTAG Posted at: 2017-07-18T13:22:20.544Z Reads: 239

```
My apologies, yes 58V is preferred ofc, however since we are dealing wit mainly capacities loads arcing wont be such a big deal (I mix 58V and 32V fused on different builds, but on the other hand, I never had a blown fuse xD). 

Mouser does have quite a few in stock where you can order single units:
http://nl.mouser.com/Search/Refine.aspx?Keyword=bf1+58v
```

---
## \#109 Posted by: chinzw Posted at: 2017-07-18T16:44:31.087Z Reads: 232

```
Digikey also has them in stock and you can order 1.
https://www.digikey.ca/product-detail/en/littelfuse-inc/142.5631.6102/F6794-ND/2515912
```

---
## \#110 Posted by: Steve-81 Posted at: 2017-07-25T14:22:51.483Z Reads: 232

```
Hello everyone, So nothing’s special going on here?
I'm just curious how the BMSs are getting on, maybe we can give a bit help if needed?
```

---
## \#111 Posted by: DeathCookies Posted at: 2017-07-25T14:59:27.859Z Reads: 231

```
What is the currently calculated Price for one or two BMS?
```

---
## \#112 Posted by: fedestanco Posted at: 2017-07-25T16:09:23.345Z Reads: 257

```
Hi Steve, actually everything is proceeding: I am gathering components from basically everywhere and once I've got everything they will fly express to China.
10 components are slowing everything down because of availability.
Cables are done and seem pretty well made.<img src="/uploads/db1493/original/3X/6/e/6e63ab33b79d695e29a6afc4fe6ba6134eaea568.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/f/b/fb08b9db88e6442d13f9792e872986fb3c483f32.jpg" width="375" height="500">
Pcbs and pcb assembly are already paid.

A realistic timeframe is 2 weeks after all the components are in stock.
```

---
## \#113 Posted by: longhairedboy Posted at: 2017-07-25T16:20:12.300Z Reads: 235

```
YAY! I can't wait to start testing these.
```

---
## \#114 Posted by: sl33py Posted at: 2017-07-25T17:04:45.349Z Reads: 236

```
Look forward to hearing how this goes - wish i'd pulled the trigger earlier to join the first group.  If successful let us know how to get in on group 2!?
```

---
## \#115 Posted by: Steve-81 Posted at: 2017-07-26T07:55:42.085Z Reads: 237

```
The connectors, cables look nice. All components are ordered, and you are waiting for some of them to get on stock? Just asking because maybe someone of us has a solution for missing parts 😊
```

---
## \#116 Posted by: lock Posted at: 2017-07-26T10:57:15.605Z Reads: 228

```
Pretty sure @JTAG has been making a few tweaks to the firmware too. Looks like we won't have to upload a new firmware just to change config params 👍.
```

---
## \#117 Posted by: fedestanco Posted at: 2017-07-26T16:40:09.824Z Reads: 227

```
I will pm you the list of components on backorder this evening. I dont want to overload this thread with boring info.
```

---
## \#118 Posted by: longhairedboy Posted at: 2017-07-28T16:36:00.098Z Reads: 223

```
i was going to say 80 but ok. What's the BMS protection shut off set at again? or is that adjustable?
```

---
## \#119 Posted by: chinzw Posted at: 2017-08-03T16:43:51.387Z Reads: 218

```
@fedestanco any news? how's the component sourcing going?
```

---
## \#120 Posted by: Steve-81 Posted at: 2017-08-03T19:17:24.992Z Reads: 220

```
He is waiting for Jtag to make some small changes. Jtag is going to put a heat protection on the pcb
```

---
## \#121 Posted by: Brad Posted at: 2017-08-17T06:12:05.989Z Reads: 217

```
Just need to check. I assume the heat protection on the pcb will not change the overall dimension of 60mm by 140mm?
```

---
## \#122 Posted by: longjohn Posted at: 2017-08-17T06:28:31.376Z Reads: 220

```
Hopefully we get our BMSes before 2020.
```

---
## \#123 Posted by: fedestanco Posted at: 2017-08-17T08:18:24.346Z Reads: 206

```
@Brad  the mod, which will be assembled and tested by @JTAG in the next days, adds just 2 small components so the dimensions are not affected much (if at all)

@longjohn hope that too
```

---
## \#124 Posted by: banjaxxed Posted at: 2017-08-17T10:55:39.560Z Reads: 217

```
Since these are custom design rather than mass produced I'm happy for design considerations to come before hasty production. @fedestanco and @JTAG thanks
```

---
## \#125 Posted by: JTAG Posted at: 2017-08-17T11:16:16.694Z Reads: 228

```
I just received the tracking number of the latest PCB's, they expect to deliver them tomorrow. Ill do my best to assemble and verify them this weekend.

@Brad The outline and mounting holes did not change, I did remote the holes for the OLED display. I will add/update the .step 3D file on github and report back when I did.
```

---
## \#126 Posted by: JTAG Posted at: 2017-08-17T14:20:32.663Z Reads: 234

```
Updated and on Github!

<img src="/uploads/db1493/original/3X/d/c/dcfda892634aab6e6532d77d5f9519227056c0f3.png" width="690" height="303">
```

---
## \#127 Posted by: akira Posted at: 2017-08-17T15:59:56.199Z Reads: 226

```
This looks damn sweet !
Impressive github share : even the pick and place files !! I wish I had such a machine !
Thank you very much !
```

---
## \#128 Posted by: akhlut Posted at: 2017-08-17T17:05:33.427Z Reads: 235

```
I want to order a set of PCB's off OSH Park, but the Altium drill file isn't playing nice.

<img src="/uploads/db1493/original/3X/f/4/f463f7c48b941837c51c7c6b144cbf2f640c78f4.png" width="690" height="293">

@JTAG - Since I don't have access to Altium, do you mind generating a set of gerbers according to [this spec](http://docs.oshpark.com/design-tools/altium-designer/)? 

Thanks man!

http://docs.oshpark.com/design-tools/altium-designer/drill-files/
http://techdocs.altium.com/display/ADOH/NC+Drill+Output+Options#
```

---
## \#129 Posted by: longhairedboy Posted at: 2017-08-17T17:56:34.050Z Reads: 230

```
Does that mean we'll see them soon? *squeeeeeee*
```

---
## \#130 Posted by: JTAG Posted at: 2017-08-17T19:30:20.739Z Reads: 231

```
[quote="akhlut, post:128, topic:20947"]
ating a set of gerbers
[/quote]

Hi @akhlut, the gerbers I normally generate and send to the manufacturer are in the format I placed on github. I will generate new files with the suggested format required by OSH Park (they are indeed different than I generate). Give me a moment and Ill add them to Github.
```

---
## \#131 Posted by: JTAG Posted at: 2017-08-17T19:32:15.928Z Reads: 230

```
YES! But those are the PCB's I ordered to verify my latest updates :blush:.
```

---
## \#132 Posted by: longhairedboy Posted at: 2017-08-17T19:36:19.106Z Reads: 231

```
And thank you for open sourcing this. The world needed this.
```

---
## \#133 Posted by: longhairedboy Posted at: 2017-08-17T20:01:16.900Z Reads: 240

```
Also i found a problem with your balance traces and fixed them. I hope you don't mind uploading these changes immediately. 

<img src="/uploads/db1493/original/3X/1/2/128fa6e583eaac6ccc06eb215893bd02fbd14d73.png" width="690" height="293">
```

---
## \#134 Posted by: akira Posted at: 2017-08-17T20:11:25.430Z Reads: 232

```
Took me a minute to understand the joke.
Excellent !!!
```

---
## \#135 Posted by: JTAG Posted at: 2017-08-17T20:16:05.342Z Reads: 239

```
I changed it a little to meet my desires:

<img src="/uploads/db1493/original/3X/2/8/2866541063df9a68d947df8ab9cfd372562311a0.jpg" width="690" height="316">
```

---
## \#136 Posted by: JTAG Posted at: 2017-08-17T20:41:35.710Z Reads: 249

```
<img src="/uploads/db1493/original/3X/b/3/b39c05a6ea5c3109d5e32a96bddb02dab806fe60.png" width="600" height="500">

<img src="/uploads/db1493/original/3X/3/f/3f549f62aceba4ba444eb6223b2b965934f8bd76.png" width="227" height="500">

It eats it now xD.

If you look for a regular PCB manufacturer and only want a single PCB you can go cheaper:

<img src="/uploads/db1493/original/3X/5/0/50300833cf9e78d73ae228460d4ec3dd9b045de0.png" width="626" height="499">
```

---
## \#137 Posted by: longhairedboy Posted at: 2017-08-17T23:14:52.568Z Reads: 236

```
LOL what's funny about that is i know Shorthairedgirl. Longhairedboy was actually a sarcastic response to her blog's domain name. I dated her for quite a while and recently she gave me permission to use that name in conjunction with a lower powered board for introducing people to esk8s and getting them hooked. So on a number of levels, this is both hilarious and spooky.
```

---
## \#138 Posted by: akhlut Posted at: 2017-08-18T01:04:30.114Z Reads: 233

```
@JTAG you, sir, are awesome!
```

---
## \#139 Posted by: karma Posted at: 2017-08-18T10:48:29.571Z Reads: 236

```
@fedestanco Are ordering done or are you waiting for more changes and able to add one more? :)
```

---
## \#140 Posted by: fedestanco Posted at: 2017-08-18T11:03:28.238Z Reads: 236

```
I already ordered some parts so it'd be quite a mess to add partecipants now.
```

---
## \#141 Posted by: karma Posted at: 2017-08-18T11:04:30.046Z Reads: 233

```
@fedestanco alright, I'll join if there will be another group buy in the future :)
```

---
## \#142 Posted by: Pimousse Posted at: 2017-08-18T22:42:59.238Z Reads: 233

```
Hi ! Thank you very much for taking care of the production of this great project.
I'm in for the next batch as well. ;)
```

---
## \#143 Posted by: akira Posted at: 2017-08-19T06:04:41.629Z Reads: 224

```
Hello Pimousse, 
Would you like to try to solder it ?
I would be in to group to ordering 3 PCBs from OSHpark.
```

---
## \#144 Posted by: Pimousse Posted at: 2017-08-19T06:17:34.787Z Reads: 219

```
Unfortunately, I don't have any skills/equipment to solder SMD components.
```

---
## \#145 Posted by: akira Posted at: 2017-08-19T07:16:08.264Z Reads: 223

```
I do.
Hot air station, microscope and (soon) reflow oven.
```

---
## \#146 Posted by: Pimousse Posted at: 2017-08-19T07:30:18.478Z Reads: 221

```
That case, count me in ! ;)
```

---
## \#147 Posted by: Steve-81 Posted at: 2017-08-30T18:16:03.294Z Reads: 226

```
@fedestanco are there any progresses? A lot of weeks are gone since last post from you. Did you got all orders, did @JTAG finish with all his small changes? Do you have any information how long it will take to get the finished BMS-es?
Don't take me wrong, I'm not impatient, just would be nice to have some information sometimes about progress.
I believe most of us "pre-financing" are all curious, and can't wait to hold those masterpieces in our hands :slight_smile:
```

---
## \#148 Posted by: fedestanco Posted at: 2017-08-30T18:54:56.375Z Reads: 223

```
Yes I owe you an update.
These days should be the very last in the testing process of @JTAG .
Believe me, given the fact that the latest GBs in this forum failed miserably, I want to feed you guys with some pcbs pictures as soon as possible. If it was for me, I would already sent the design to the pcb factory, which btw has already been paid.

Components update:
In the newest BOM some components have been removed, some others have been added. The cost shouldnt vary much. 
I am also trying a cheap fuse to include with the bmss, since ,as I told you, littlefuse is out of budjet.

I am also trying to understand chinese taxation regarding incoming goods. If there is any I may switch plans and buy some stuff in China (still original).

Any further questions please ask.
```

---
## \#149 Posted by: Steve-81 Posted at: 2017-08-30T19:08:18.695Z Reads: 209

```
Wow, that was a quick answer :slight_smile:
So what you think, when do the PCB plans go to the factory?
```

---
## \#150 Posted by: fedestanco Posted at: 2017-08-30T19:12:50.964Z Reads: 220

```
The same day jtag will post an update on the new version. As I said the factory has been paid so the production can start right away.
```

---
## \#151 Posted by: longhairedboy Posted at: 2017-08-30T19:17:42.003Z Reads: 223

```
i'm looking forward to these. Like really, really looking forward to these. 

Hopefully they'll be absolutely perfect and solve all of my problems, or else i'll have to cry like a baby on the forums and demand a full refund and when i don't get it make death threats until i get banned and cry some more on other social media sites, you know, like an adult.
```

---
## \#152 Posted by: Steve-81 Posted at: 2017-08-30T19:24:40.570Z Reads: 221

```
@longhairedboy man I'm laughing only with reading your post :slight_smile:
Sorry for that, but I saw your works and webpage, I just imagined you crying like a baby :D
```

---
## \#153 Posted by: longhairedboy Posted at: 2017-08-30T19:27:23.110Z Reads: 219

```
one of my many roles in the community is to keep things entertaining. I appreciate your appreciation.
```

---
## \#154 Posted by: chinzw Posted at: 2017-08-30T21:42:13.989Z Reads: 215

```
hahaha! thanks for the humor
```

---
## \#155 Posted by: Steve-81 Posted at: 2017-09-01T09:14:41.068Z Reads: 213

```
@JTAG your DieBieMS is a super BMS. I've never seen anything so complex and well made before. Do you know when your plans are ready for production, so we (the average users) can have fun with our boards built around them?
```

---
## \#156 Posted by: JTAG Posted at: 2017-09-04T17:51:04.055Z Reads: 213

```
Thanks for the complement. I really hope it will meet everyones expectations :flushed: !

I finally had the time to evaluate my latest design ( V0.4 ) and found a very minor mistake (wrong valued resistor), this is now fixed in the latest design ( V0.5 , will push it to Github within an hour ).

I am really exited to see this design being semi mass produced :heart_eyes:.
```

---
## \#157 Posted by: Steve-81 Posted at: 2017-09-04T17:56:45.883Z Reads: 210

```
Super

This means we are looking forward to test them :)
```

---
## \#158 Posted by: JTAG Posted at: 2017-09-04T18:05:35.667Z Reads: 220

```
I personally have no plans to start producing them (I am only producing them for personal/friends use). I just wanted to share the design to help others. Everyone is free to produce them themselves if they want. 

Maybe if the popularity increases and the design/firmware is fully matured others might start producing and selling them.
```

---
## \#159 Posted by: fedestanco Posted at: 2017-09-04T19:02:28.970Z Reads: 228

```
I am happy that the only bug was minor and already solved.
Tomorrow will send the files to the factory so maybe next week pcbs will be ready to be assembled.

I suggest you to put a Creative Commons non commercial license on the files. The last thing I want is this beautiful design to be produced with low quality standards and sold by random chinese.
```

---
## \#160 Posted by: Steve-81 Posted at: 2017-09-05T07:54:27.085Z Reads: 220

```
I would suggest the same, but as we know, in China it doesn't matter at all if something is licensed :(
```

---
## \#161 Posted by: Steve-81 Posted at: 2017-09-09T19:26:19.738Z Reads: 219

```
@fedestanco how is everything going? Did the factory start producing our so strongly waited BMS-es?
```

---
## \#162 Posted by: fedestanco Posted at: 2017-09-09T21:19:18.280Z Reads: 238

```
Yes. Starting from yesterday. I asked for an extimate shipping time for the pcbs and we are looking at 7 working days. This is because I requested the top stuff like gold immersion and 2 oz copper. <img src="/uploads/db1493/original/3X/6/d/6d0aa972e9c4cb7862a496f3a2b3d666527733d1.jpg" width="281" height="500">

BOM on the other hand is quite a pain in the ass: I decided to sort the most expensive stuff directly in China because there is a real risk on paying export tax sending a heavy package with a courier.

I am working hard to find original components directly in China. 
My leadtime prediction still stands: we will receive the stuff 2 weeks after all the components are gathered.
Any question please ask.
```

---
## \#163 Posted by: OnAmps Posted at: 2017-09-09T23:20:31.156Z Reads: 216

```
@fedestanco Thanks for driving all this. Had to finally create a username and let you know I'll be on the list next to purchase a couple, if another one happens. 

I work at a big semiconductor company and know a lot of CM/ODMs, if this CM doesn't work out, would love to reach out to a few and see how much they can build these for us. 

Crossing fingers for everyone, the layout looks good! I can have one of the our layout engineers review if there are any issues found (I've been telling some of the engineers in the office about my build and we were going to design something just like this but no point in redesigning the wheel).
```

---
## \#164 Posted by: fedestanco Posted at: 2017-09-10T17:07:53.615Z Reads: 205

```
Good to know there are some professionals following the project. Maybe you can run the next batch if you gather some interest.
```

---
## \#165 Posted by: mishrasubhransu Posted at: 2017-09-13T17:48:14.726Z Reads: 213

```
Are there any extras? I am hoping there's 1 left.
```

---
## \#166 Posted by: fedestanco Posted at: 2017-09-14T14:25:23.860Z Reads: 215

```
No seats left. If someone wants to drop out I'll let you know.
```

---
## \#167 Posted by: stormboard Posted at: 2017-09-14T23:39:53.662Z Reads: 216

```
if 2 drop out ill take one 100%,just send me a pm and ill send the money straigh away bro
```

---
## \#168 Posted by: fedestanco Posted at: 2017-09-15T11:09:40.563Z Reads: 223

```
<img src="/uploads/db1493/original/3X/5/5/55581132d499aa9e656c23b30d36c89968360a92.jpg" width="690" height="388">

Stuff is slowly coming in...
```

---
## \#169 Posted by: banjaxxed Posted at: 2017-09-15T11:13:29.840Z Reads: 222

```
ooooooh look at those doohickeys!
```

---
## \#170 Posted by: longhairedboy Posted at: 2017-09-15T14:41:19.561Z Reads: 225

```
i'm ready and waiting. With drool.
```

---
## \#171 Posted by: fedestanco Posted at: 2017-09-22T07:58:59.648Z Reads: 230

```
<img src="/uploads/db1493/original/3X/3/4/34c34b517cd641c906d61a77c551ccb6709f23d9.jpg" width="375" height="500">
Straight out of the oven. Next step: assembly.
```

---
## \#172 Posted by: Brad Posted at: 2017-09-22T08:08:14.716Z Reads: 223

```
Never felt so good looking at a PCB board.
```

---
## \#173 Posted by: stormboard Posted at: 2017-09-22T10:02:41.246Z Reads: 211

```
anybody wanna give me half theres xD
```

---
## \#174 Posted by: chinzw Posted at: 2017-09-22T17:20:21.663Z Reads: 205

```
Almost on the home stretch!
```

---
## \#175 Posted by: Steve-81 Posted at: 2017-09-24T19:35:19.056Z Reads: 206

```
Wow, looking good

Can't wait to hold it in my hands :)
```

---
## \#176 Posted by: Steve-81 Posted at: 2017-09-25T15:35:19.973Z Reads: 204

```
@longhairedboy how many of this boards did you order? Just wondering cause I think shipping to the US will cost you a lot of extra coins.
```

---
## \#177 Posted by: fedestanco Posted at: 2017-09-25T16:07:27.792Z Reads: 203

```
He is actually saving more than the other peeps. I can ship with UPS, up to 5kg (40 bms), for 25€ to america. And he doesnt even have to pay tax under 800$ value.
```

---
## \#178 Posted by: longhairedboy Posted at: 2017-09-25T16:56:24.439Z Reads: 209

```
i ordered 4 but i actually need about a dozen of them. 

I'll settle for four now. 

@fedestanco  I'd be happy to run a batch of these through somebody in the US if anyone has recommendations on who would be the best fab shop to do it. I'm going to need these moving forward so i was hoping to work something out so that i could make my own and have some money flow back to the project somehow. Or at least to the designer.
```

---
## \#179 Posted by: Steve-81 Posted at: 2017-09-25T20:47:13.912Z Reads: 208

```
So you want to put them into your builds. I guess you don't only want to build crazy looking but crazy boards :slight_smile:
You should try building a mountainboard too.
```

---
## \#180 Posted by: fedestanco Posted at: 2017-09-25T21:13:49.033Z Reads: 211

```
Here is a list of most of the assembly fabs in the US 
https://smtnet.com/company/index.cfm?fuseaction=browse_companies&category=17&country=263

I completely agree to support the creator. In fact I ordered 9 more bare pcbs to resell. 100% of the profits (hopefully 90€) will be donated. 
Please @JTAG provide donation link :slight_smile:
```

---
## \#181 Posted by: emepror Posted at: 2017-09-26T01:43:41.043Z Reads: 213

```
Check out MacroFab and CircuitHub. Macrofab does direct manufacturing in Texas and CircuitHub acts as a front end for a bunch of companies.

Both should have pretty good pricing for smaller batch stuff. I'm probably going to use Macrofab to do a run of VESC6's once i get a design.
```

---
## \#182 Posted by: Steve-81 Posted at: 2017-09-26T07:15:25.324Z Reads: 204

```
@fedestanco I'm up for a 5-10 EUR extra payment if that goes to @JTAG
```

---
## \#183 Posted by: Steve-81 Posted at: 2017-09-26T07:16:22.299Z Reads: 202

```
Maybe some others are thinking on the same way, and a bit of extra will be collected
```

---
## \#184 Posted by: longhairedboy Posted at: 2017-09-26T11:32:34.535Z Reads: 203

```
i use macrofab for my e-switches currently and i'm not disappointed in the quality so far. I am disappointed that the price steadily keeps creeping up, and i've heard rumors about shadey stuff (nothing concrete or even specific) , but overall i'm happy with them. I just want to make sure i don't put all my eggs in one basket without at least trying a few other baskets. 

Thanks!
```

---
## \#185 Posted by: banjaxxed Posted at: 2017-10-02T15:32:51.501Z Reads: 207

```
And so I am continuing my 12s build & holding my breath for these lovely BMSs.
Hopefully the balancing will be tolerant of slighly out of balance cells..Otherwise it a big rip-apart in my future :cold_sweat:
```

---
## \#186 Posted by: pbram Posted at: 2017-10-02T16:55:16.105Z Reads: 209

```
Hi, I just joined this forum. I would like to participate in this build for 2 BMS. fedestanco, I signed for two in the link you provided. Let me know the next steps. 
JTAG, I really like your design and thank you for sharing it with community.
thx
```

---
## \#187 Posted by: fedestanco Posted at: 2017-10-02T17:28:45.394Z Reads: 204

```
Sorry to tell you that the GB is no more open to new participants.

Update for the partecipans: 1-8 october the company is closed for holidays so we should expect the boards to be finished few days after that date. Will post pics as soon as I get any.
```

---
## \#188 Posted by: pbram Posted at: 2017-10-02T17:55:27.504Z Reads: 200

```
oh okay, thanks for the update. If anyone wants to do another build by pooling other interested users, please let me know.
thx
```

---
## \#189 Posted by: longhairedboy Posted at: 2017-10-02T18:42:06.351Z Reads: 198

```
are these things shipping soon?
```

---
## \#190 Posted by: fedestanco Posted at: 2017-10-02T19:06:40.604Z Reads: 195

```
Probably within 1 week after the holidays.
```

---
## \#191 Posted by: longhairedboy Posted at: 2017-10-02T19:08:29.493Z Reads: 196

```
So January?
```

---
## \#192 Posted by: fedestanco Posted at: 2017-10-02T19:10:26.381Z Reads: 195

```
Haha hopefully sooner. Only thing I can promise is that on my side wont be any delays: receive on monday ship to you on tuesday.
```

---
## \#193 Posted by: Steve-81 Posted at: 2017-10-02T21:12:16.913Z Reads: 198

```
Wow we are getting closed to have them :slight_smile:
I hope @longhairedboy you're not right, but if it gets january than at least we can say it is a nice beginning of a year
```

---
## \#194 Posted by: fedestanco Posted at: 2017-10-02T21:33:49.090Z Reads: 208

```
I meant chinese holidays btw (1-8 oct)
```

---
## \#195 Posted by: Steve-81 Posted at: 2017-10-03T10:22:02.308Z Reads: 208

```
@fedestanco do you have a Chinese origin? Just asking because when you shared the screenshot about your chat with the factory. I guess most of us only see some "pictures" in that chat, nothing more. But must be cool to speak a language in which you can arrange everything. I'm a bit envious, I only speak some European languages :(
```

---
## \#196 Posted by: fedestanco Posted at: 2017-10-03T18:53:25.208Z Reads: 204

```
I picked mandarin as the second foreign language in high school. Talking to vendors is a good way to review it.
```

---
## \#197 Posted by: Steve-81 Posted at: 2017-10-10T12:57:30.773Z Reads: 208

```
Hello,

Any upgrades regarding to those BMS-es?
```

---
## \#198 Posted by: fedestanco Posted at: 2017-10-10T23:53:20.002Z Reads: 216

```
Yes. All but 1 component arrived at the assembly fab. There is a strange delay for the wurth screwholders. I emailing back and forth the chinese customs to get this thing released. Will get back to you with some assembled pcbs in few days.<img src="/uploads/db1493/original/3X/2/5/25b4bcd5373d3f9de8ab1e54a13a5c3becc28c47.png" width="281" height="500">
```

---
## \#199 Posted by: Steve-81 Posted at: 2017-10-11T06:44:31.608Z Reads: 214

```
@fedestanco you are doing a good job, I wouldn't do it. I would be so pissed up that I have to go behind everything. I don't have the patience to go trough every single thing more times.
```

---
## \#200 Posted by: banjaxxed Posted at: 2017-10-11T08:26:08.568Z Reads: 213

```
Tell them to stop screwing around, we need balance!
```

---
## \#201 Posted by: fedestanco Posted at: 2017-10-16T16:09:01.085Z Reads: 216

```
The last part arrived at the assembly fab. They agreed to give max priority to the assembly: tomorrow pcbs will be done and I will post here some pics.

The following steps are :send the boards to the forwarder, pay the forwarder and wait to finally receive the stuff.
```

---
## \#202 Posted by: Steve-81 Posted at: 2017-10-16T16:49:01.953Z Reads: 216

```
Wow, sounds like we will get them in the near future :)
```

---
## \#203 Posted by: chinzw Posted at: 2017-10-16T17:14:20.824Z Reads: 207

```
Early xmass present :)
```

---
## \#204 Posted by: longhairedboy Posted at: 2017-10-16T17:25:06.978Z Reads: 212

```
I'm holding my breath until they arrive so hurry up or i'll be dead.
```

---
## \#205 Posted by: banjaxxed Posted at: 2017-10-16T18:18:38.709Z Reads: 216

```
Holding breath that long is dangerous without venting, kinda like a lipo
```

---
## \#206 Posted by: longhairedboy Posted at: 2017-10-16T18:30:43.754Z Reads: 215

```
Too late, i already puffed myself.
```

---
## \#207 Posted by: fedestanco Posted at: 2017-10-17T10:00:42.872Z Reads: 227

```
<img src="/uploads/db1493/original/3X/c/b/cbc8f078d7ac41b55adc881617bf62cd0999e6a7.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/9/c/9cf72ecb691dc244e09496729d2e9bc774c99a5e.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/6/2/628f00311dee48ac197a4ae7d54d3a98186b6007.jpg" width="666" height="500">
```

---
## \#208 Posted by: fedestanco Posted at: 2017-10-17T10:07:04.769Z Reads: 220

```
Regarding the screwholders they told me that they dont have the appropriate equipment to install them. 
I found out that they simply press fitted and not soldered. I will try to install them in my shop.<img src="/uploads/db1493/original/3X/d/d/ddb0ee360b9163f7b10111d303e852b9c62a9b95.jpg" width="96" height="202"><img src="/uploads/db1493/original/3X/2/6/26c242dbd101637521730193e1e5f290d578dec9.jpg" width="570" height="215"><img src="/uploads/db1493/original/3X/5/5/55985bb4678463f77d94f974ddadcabda3e8a458.jpg" width="690" height="396">
```

---
## \#209 Posted by: banjaxxed Posted at: 2017-10-17T10:24:38.862Z Reads: 218

```
looks awesome, thanks so much for producing these treasures.
```

---
## \#210 Posted by: JTAG Posted at: 2017-10-17T16:48:58.277Z Reads: 216

```
DAJUM awesome to see this progress! Looks good as well. Did you purchase the pressfits trough wuth directly? I have contacts that might be able to supply a 3D file to 3D print that could be used as the receiving part of the pressing procedure.
```

---
## \#212 Posted by: Hummie Posted at: 2017-10-17T16:51:31.538Z Reads: 216

```
So so smart
```

---
## \#213 Posted by: Steve-81 Posted at: 2017-10-17T16:53:38.579Z Reads: 214

```
@JTAG How do your prototypes work? Those things look so nice, @fedestanco I can't wait to hold it in my hands :slight_smile:

@longhairedboy I hope you puffed up well, would be a shame for the community to loose such a guy :D
```

---
## \#214 Posted by: longhairedboy Posted at: 2017-10-17T16:59:57.074Z Reads: 210

```
i'm kind of ecstatic about finally seeing these in my hands soon. My mind is blowing as we speak.
```

---
## \#215 Posted by: Steve-81 Posted at: 2017-10-17T17:01:58.105Z Reads: 206

```
Same here :slight_smile:
```

---
## \#216 Posted by: fedestanco Posted at: 2017-10-17T18:03:52.909Z Reads: 207

```
I think I will machine it by myself since the one from wurth seems way too fragile and thin. 

Thanks for the constant support btw. @JTAG please pm your address so I can send you the 9 extra non populated pcbs when they arrive.
```

---
## \#217 Posted by: chinzw Posted at: 2017-10-17T21:18:29.767Z Reads: 207

```
We're at the finish line! Can't wait to try this out!
```

---
## \#218 Posted by: banjaxxed Posted at: 2017-10-17T22:01:08.622Z Reads: 208

```
You the men @fedestanco & @JTAG
Of course there is the configure I need to figure out I'm going to use these for 12s ATB Trampa builds
```

---
## \#219 Posted by: JTAG Posted at: 2017-10-18T09:18:09.346Z Reads: 216

```
I have ambitious to match the VESCs communication style to allow all devices to be on the same bus and have the same communication flexibility ( connect to any device trough any device ) . 

I really hope to have at least a basic cross platform ready tool by the time you receive your boards. 

By the time everybody has their system operational there will likely be other SW engineers willing to help lift everything to a more open source community level ( at the basis I am a HW engineer, I just need the SW to do it something useful xD xD ).
```

---
## \#220 Posted by: banjaxxed Posted at: 2017-10-18T09:43:33.662Z Reads: 213

```
I hope the people who can will get behind it and share the load, yes just basic functionality is all we want starting off.
The cool S/W stuff can be implemented by those with the skills, will and time

Cheers @JTAG
```

---
## \#221 Posted by: JTAG Posted at: 2017-10-18T09:49:29.045Z Reads: 214

```
The BMS is perfectly usable at its current state, the only thing missing is a computer UI. But since so many people will have one on the short term I really want to build it no :nerd:.
```

---
## \#222 Posted by: solbergen Posted at: 2017-10-18T19:09:46.160Z Reads: 208

```
Hi guys, would any one of you be interested in selling one of your coming units to me? We're a company looking to implement this in our product (non esk8), and would be willing to help on SW and also with hw testing, but we need a unit as soon as possible to test-implement it.
```

---
## \#223 Posted by: longhairedboy Posted at: 2017-10-18T19:17:47.077Z Reads: 215

```
I keep hitting the reload button  on my mailbox but the BMSs still aren't in it. I even yelled at the mail man incoherently but nothing happened. So i wait, and suffer. 

I wonder if this is what my customers feel like.
```

---
## \#224 Posted by: GrecoMan Posted at: 2017-10-18T19:36:56.854Z Reads: 207

```
that is exactly what I do when I hear you shipped a board to someone...
```

---
## \#225 Posted by: oyta Posted at: 2017-10-18T20:34:49.771Z Reads: 218

```
[quote="JTAG, post:219, topic:20947"]
I have ambitious to match the VESCs communication style to allow all devices to be on the same bus and have the same communication flexibility ( connect to any device trough any device ) .
[/quote]

That is going to be nice! All the possibilities!

@fedestanco To be prepared I need to get the needed hardware to connect to the BMS. I have tried to search and find the info, but did not succeed.

1. The screw terminals: Are the screws included, if not what diameter and type fits?
2. What type of "cable shoe" fits?
3. What type of connector is needed for the balance wires?

Other stuff I need to get a hold on?

I am looking forward to this piece of hardware (and firmware)! Thanks for all the great work both of you.
```

---
## \#226 Posted by: lock Posted at: 2017-10-18T22:51:42.910Z Reads: 204

```
What would help kickstart development is a really simple proof of concept app that communicates with the BMS via USB (?). Doesn’t need a UI, could simply write some hardcoded params from PC to the BMS, and read the same params back. Could be in any language, but preferably one without an expensive development environment. I imagine there’s a few people round here that could take it forward from that point.
```

---
## \#227 Posted by: fedestanco Posted at: 2017-10-18T23:59:06.695Z Reads: 220

```
1) the treaded hole is 5mm, so any 5mm (metric thread) screw will do the job. 
A lot of amps will flow through that link so you really want to be able to tighten it properly; hex screws may be more appropriate.
2)anything rated according to your current needs with a 5mm hole
3)balance cable is included, custom made. This is where the extra 4€ have gone. You will receive 4 cables: balance, on-off, display, canbus.

As I told you the fuse was totally out of budjet so it will not be included.

@solbergen few people are already in the waiting list; if you PM me some details about the project and company (to make sure you are seriously interested in SW development and not just a random dude) I may decide to lend you one of my 2 boards for a limited amount of time, so that you are covered while you get few boards manufactured (pcbway.com)
```

---
## \#228 Posted by: JdogAwesome Posted at: 2017-10-19T03:04:30.507Z Reads: 217

```
Hey @JTAG your devolpment on these things is just amazing, great work! I'm just curious on why you opted for a STM32F4 microcontrollers instead of something like a F1 or even a small 8 bit IC because of the low CPU load a BMS has? Also you should go with the IRFS7730 instead of the 7734 it's RDSon is only 1.7-2 instead of the like 3Mohms the 34 has. Other than that it looks awesome and I think the DIY community really needs a good DIY BMS.
```

---
## \#229 Posted by: TVE Posted at: 2017-10-24T08:47:31.476Z Reads: 205

```
Are there still units available? I want to buy one.
```

---
## \#230 Posted by: spannepacker Posted at: 2017-10-25T00:05:54.118Z Reads: 212

```
I am definitely interested in picking one up whenever the next round is produced.
```

---
## \#231 Posted by: Steve-81 Posted at: 2017-10-27T13:13:01.141Z Reads: 208

```
Do we have any news? Where are we standing now?
```

---
## \#232 Posted by: fedestanco Posted at: 2017-10-28T00:38:40.804Z Reads: 222

```
Ups was faster than expected: today the package landed in Rome and I wasn't home, so tomorrow or monday I will receive the package. 
I will ask a confirmation for your address via email, so check your inbox this weekend. 
<img src="/uploads/db1493/original/3X/9/c/9ccd788c7ba100731159624f3785f2f7f9a73e8f.png" width="281" height="500">
```

---
## \#233 Posted by: chinzw Posted at: 2017-10-28T00:56:35.626Z Reads: 209

```
Awesome news! That was really quick :slight_smile:
```

---
## \#234 Posted by: fedestanco Posted at: 2017-11-03T17:27:56.635Z Reads: 225

```
Hi guys I owe you an update:

This week UPS had one internal strike so the pcbs came in only today. 

Both assembly and pcb quality is astonishing at the first look; those yamaha pick and place machines did a very good job. 

<img src="/uploads/db1493/original/3X/a/6/a6170f321d841eaba5831a13018cfecc94e81cb1.jpg" width="281" height="500">

Furthermore the screwholders assembly is no more a problem: this is all what it takes: (m4 screw and m4 bolt)
<img src="/uploads/db1493/original/3X/3/1/3198c71915c290c31b5913dd9541a13c28680c4f.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/c/d/cdc9279d2aac806477cdaf65946548992bef5cee.jpg" width="690" height="388">

Although I have an exam on tuesday, I can ship non programmed pcbs on monday. If you want it programmed and with screwholders installed, please wait few more days.
```

---
## \#235 Posted by: JTAG Posted at: 2017-11-03T17:52:53.347Z Reads: 217

```
Daaaaaaaaayum son :upside_down: :nerd:.
```

---
## \#236 Posted by: chinzw Posted at: 2017-11-03T18:02:38.323Z Reads: 216

```
I'm pretty sure we can all get the screw holders in ourselves. I would focus on programming mainly.
```

---
## \#237 Posted by: longhairedboy Posted at: 2017-11-03T18:15:50.088Z Reads: 219

```
yeah never mind the screw holder installation, just include the hardware. I don't have a programmer so firmware is a must.
```

---
## \#238 Posted by: oyta Posted at: 2017-11-03T18:34:28.004Z Reads: 217

```
Second @longhairedboy

And they look nice! Can’t wait!
```

---
## \#239 Posted by: banjaxxed Posted at: 2017-11-03T21:08:50.469Z Reads: 214

```
Nice one, take your time and good luck in your exams ☘️
```

---
## \#240 Posted by: JTAG Posted at: 2017-11-03T23:40:30.371Z Reads: 213

```
Guys please don't underestimate the screw terminals. They should be pressfit, that is not a trivial job and doing it different then decent will make the experience less pleasant/optimal (applying the wrong method of stress to the PCB will likely damage it).

.
```

---
## \#241 Posted by: oyta Posted at: 2017-11-04T08:53:24.691Z Reads: 207

```
Alright, It sounds like I want @fedestanco doing ahead of posting :wink:
```

---
## \#242 Posted by: Brad Posted at: 2017-11-04T12:39:31.481Z Reads: 204

```
I will want the screw holder installation done before shipping.

So close that I can almost smell it! :nose:
```

---
## \#243 Posted by: Steve-81 Posted at: 2017-11-04T17:58:23.566Z Reads: 218

```
Hello @fedestanco

I don't think we would have a problem with some more days. Do your studies for the exams, that is much more important than some pcb-s, even I would love to have my DieBieMS in my hands.

Guys, who cares if we have to wait some more days? We didn't order them yesterday, does it really mater if it takes a bit more?

 @JTAG I do agree with you, that wrongly used forces on the pcb can damage it, and I guess most people here don't have a clue how to make a decent fit. Most people can't change a lightbulb in a car, how would they manage this? ... :slight_smile:
```

---
## \#244 Posted by: evoheyax Posted at: 2017-11-04T18:01:05.527Z Reads: 205

```
Are there any more of the ones made so far that haven't been claimed? I wouldn't mind trying a few out.
```

---
## \#245 Posted by: fedestanco Posted at: 2017-11-04T19:36:19.860Z Reads: 203

```
I would follow @JTAG's suggestion and let me install these bolts for you. 

@evoheyax no boards left, sorry.
```

---
## \#246 Posted by: Steve-81 Posted at: 2017-11-07T18:21:59.280Z Reads: 200

```
How did you manage your exams? I hope you had enough time to prepare.
```

---
## \#247 Posted by: briman05 Posted at: 2017-11-07T19:25:43.714Z Reads: 202

```
How much are these BMS shipped to NJ in the States?
```

---
## \#248 Posted by: bsancken Posted at: 2017-11-07T19:48:03.009Z Reads: 206

```
So from what I can understand reading through this thread is that it is possible to change the config for this to work with something lower than 12s? Can I change this to work with a 6s battery?

I wish I would have been able to get in this GB earlier, Is it still closed or does anyone have and extra one to sell to the US? Thanks
```

---
## \#249 Posted by: fedestanco Posted at: 2017-11-07T20:28:42.730Z Reads: 204

```
Exams went well. @JTAG and I are finding a way to keep programming at the minumum level for you. 
Also a User Interface is in the to-do list.

The offers still stands: if you dont need programming, I will ship the next day.

I measured the weight of 1x(bms, cables and packaging) and it is 150g.

So the shipping options are:
Slow untracked (used it 40 times and never failed):
PRICES FOR 1 OR 2 BMSS
EUROPE 5,20€  6€
AMERICA 8,10€ 8,5€
AUSTRALIA 10,1€ 12€

Slow tracked:
EU 11,8.  13,2
AM 15,3.  17,3
AU 16,7. 22,2

Fast tracked (UPS)
Most EUROPE 16
AMERICA : 26
AUSTRALIA: 49

And please add some pennies for packaging.
```

---
## \#250 Posted by: longhairedboy Posted at: 2017-11-07T20:37:03.883Z Reads: 200

```
didn't realize the terminals were pressed fit. I can wait. 

Should i shoot you the cash for shipping now or what?
```

---
## \#251 Posted by: chinzw Posted at: 2017-11-08T17:38:02.482Z Reads: 197

```
How do we pay for shipping? Is shipping to canada same as america (im asuming you're calling USA "america")?
```

---
## \#252 Posted by: fedestanco Posted at: 2017-11-08T17:41:16.471Z Reads: 202

```
America is meant as continent so mexico,usa, canada....

Payment method is preferrably paypal. If you want it shipped the same day just add the note: no programming needed.
```

---
## \#253 Posted by: Luuke Posted at: 2017-11-08T17:43:34.818Z Reads: 204

```
How much is one BMS?
How long does it take until users are programme the voltage themselves?
```

---
## \#254 Posted by: chinzw Posted at: 2017-11-08T17:50:46.052Z Reads: 201

```
Also, what's the time difference between the fast and slow tracked? I'm about to send the money, just want to make sure what's what.
```

---
## \#255 Posted by: fedestanco Posted at: 2017-11-08T18:40:16.842Z Reads: 199

```
Fast is UPS so basically 3-4 days. Slow should be a couple weeks to canada.
```

---
## \#256 Posted by: chinzw Posted at: 2017-11-08T19:00:20.299Z Reads: 198

```
Perfect, money sent!
```

---
## \#257 Posted by: b264 Posted at: 2017-11-08T19:01:59.328Z Reads: 202

```
[quote="chinzw, post:251, topic:20947"]
im asuming you're calling USA "america"
[/quote]

They were probably referring to Uruguay
```

---
## \#258 Posted by: chinzw Posted at: 2017-11-08T19:43:15.907Z Reads: 204

```
[quote="b264, post:257, topic:20947"]
They were probably referring to Uruguay
[/quote]

Hey smartypants, North America and South America are continents, America is not. Hence my assumption that he was referring to USA.
```

---
## \#259 Posted by: Pantologist Posted at: 2017-11-10T15:08:01.100Z Reads: 197

```
I just saw these updates. Does fast tracked with UPS have any insurance?
```

---
## \#260 Posted by: TVE Posted at: 2017-11-11T14:43:05.549Z Reads: 197

```
So are their still units available or not?
```

---
## \#261 Posted by: fedestanco Posted at: 2017-11-11T16:09:32.085Z Reads: 211

```
Hi guys, I took some time to read through the firmware to figure out a way to deliver already programmed bmss to you.
Even as a software newbie I found the code very readable and well explained.
For example this is the part of code where the battery configuration can be written:
<img src="/uploads/db1493/original/3X/0/d/0d6569ead6a7c91ae6e501eaae1d3318095e324b.PNG" width="690" height="279">
The problem for now is that if you want to write your custom values (changing the blue numbers), is not like in the VESC TOOL where you just click the button "write configuration". Instead, you need a software that rewrites the whole firmware into one hex file. And this software is quite expensive http://www2.keil.com/mdk5 .
Obviously there will soon be a fool-proof program for us to write custom configurations. 

To get your boards to you asap, I have decided to upload to the bmss a "**voltage-based firmware**". To do so **I need to know your battery cell number (10s/12s...)**. This firmware will allow you to have a functional bms without the fancy custom features like max current,highest cell voltage...(see pic above)- these fancy features will be set standard to any bms, and you will eventually change them when a User Interface will be available.
```

---
## \#262 Posted by: Brad Posted at: 2017-11-11T16:27:18.931Z Reads: 198

```
My battery cell number will be in 12 series.
```

---
## \#263 Posted by: fedestanco Posted at: 2017-11-11T16:28:58.165Z Reads: 204

```
Furthermore, an LCD battery meter is already implemented in the firmware. It is based on the measured amp-hour comsumption (so it has to be set _custom to your battery_); 
I believe most people have similar sized battery (10s4p is around 10amp-hour). For this reason all the firmwares will be set accordingly to a 10amp-hour battery. This means that if your battery is about such size, the LCD indication will be quite realistic; if you have a 700wh battery (@longhairedboy) you may want to stick with the ebay voltage meters.

Just to see if my guess is correct, HOW BIG IS YOUR BATTERY? [poll type=regular]
* 7,5 amp-hour (10s3p samsung 25r)
* 10 amp-hour (10s4p)
* 12,5 amp-hour (10s5p)
* 15 amp-hour (10s6p)
[/poll]
```

---
## \#264 Posted by: fedestanco Posted at: 2017-11-11T16:30:08.607Z Reads: 199

```
@pantologist 150EUR insurance
@TVE  nope
@Brad thanks, noted
```

---
## \#265 Posted by: Brad Posted at: 2017-11-11T16:39:55.043Z Reads: 200

```
I would assume 12s5p at 3,000 mAh will still be read accurately as that would bee 15 amp hours, same at the 10s6p?
```

---
## \#266 Posted by: fedestanco Posted at: 2017-11-11T16:41:03.406Z Reads: 201

```
Sure, thats exactly my battery: 5p x 3000mah = 15amp-hour.
```

---
## \#267 Posted by: oyta Posted at: 2017-11-11T18:02:57.677Z Reads: 196

```
I have 10s3p LG HG2 9Ah. I chose 10 Ah in the poll.

And I have Paypal’ed you :slight_smile:
```

---
## \#268 Posted by: Steve-81 Posted at: 2017-11-11T18:03:11.217Z Reads: 198

```
@fedestanco will you contact us via mail how we want the transportation, or should we just write you it here?

Should we just send you money, or will you calculate and tell us after we decided how we want it sent?
```

---
## \#269 Posted by: longhairedboy Posted at: 2017-11-11T23:53:54.502Z Reads: 198

```
650 watt hours is my cap right now. Sorry, i missed the part about volt meters. This includes one or includes the terminals or screen for one or what? I'm lost. Just got back from lego land and decided to load @Ackmaniac 's  vesc tools onto my board and am fiddling with the whole "i can't detect anything" thing that i saw people complaining about.
```

---
## \#270 Posted by: fedestanco Posted at: 2017-11-12T00:41:39.010Z Reads: 201

```
@Steve-81  My preference is that you pay via paypal and tell me your battery type via PM/paypal message/email. Anyways a broadcast email will follow in the next hours.

@longhairedboy you will have the necessary cables both for the lcd and the fancy switch. The LCD module you need to buy is this one: [oled display](https://www.ebay.nl/itm/0-96-I2C-IIC-Serial-128X64-OLED-LCD-LED-White-Display-Module-for-Arduino-Screen-/161836161890?hash=item25ae2fdb62:g:n9MAAOSw7NNUK-pv)
```

---
## \#271 Posted by: longhairedboy Posted at: 2017-11-12T00:47:26.493Z Reads: 197

```
just bought a few of them. Do you need shipping money right now or what? i can shoot you some cash if you need it. 

I think this LED display will go over my front truck. Should nicely match the one on the remotes.
```

---
## \#272 Posted by: lock Posted at: 2017-11-12T02:04:00.399Z Reads: 208

```
[quote="fedestanco, post:261, topic:20947"]
Instead, you need a software that rewrites the whole firmware into one hex file. And this software is quite expensive http://www2.keil.com/mdk5 .
[/quote]

There's a *free* Keil MDK-Lite version available. It has some restrictions, such as a maximum build size of 32kB. Just in case anyone else was curious....

```
DieBieMS\DieBieMS.axf: error: L6047U: The size of this image (39396 bytes) exceeds the maximum allowed for this version of the linker
Finished: 0 information, 0 warning, 0 error and 1 fatal error messages.
"DieBieMS\DieBieMS.axf" - 1 Error(s), 0 Warning(s).
Target not created.
```

:confounded: It was surprising easy to get it all installed, setup, and building. Removing the CAN library saved all of 500 bytes. You could grab a 7 day trial license that removes this restriction, but it's not a great solution.

Will send you through an email with my battery pack details. a123 (LiFePO4), so the numbers will be a little different to most.
```

---
## \#273 Posted by: Brad Posted at: 2017-11-13T06:43:50.637Z Reads: 194

```
@fedestanco Might want to use BCC instead of CC when sending mass email. I have been getting replies to you from other people :)

Not too sure if BCC will stop mass replies to all recipients or not. I reckon it should.

"Cc means carbon copy and Bcc means blind carbon copy. For emailing, you use Cc when you want to copy others publicly, and Bcc when you want to do it privately. Any recipients on the Bcc line of an email are not visible to others on the email."
```

---
## \#274 Posted by: fedestanco Posted at: 2017-11-13T10:24:08.416Z Reads: 189

```
This is very helpful. Have you received other people personal information like address or something?
```

---
## \#275 Posted by: rene Posted at: 2017-11-13T10:50:43.350Z Reads: 182

```
@fedestanco - I added myself to the buyers list of the DieBie 12s BMS.
```

---
## \#276 Posted by: longhairedboy Posted at: 2017-11-13T12:21:38.054Z Reads: 181

```
I may have contributed to the email problem. Working in a cubicle farm has caused me to develop the habit of hitting Reply All when i receive emails to multiple people.
```

---
## \#277 Posted by: Brad Posted at: 2017-11-13T13:01:13.432Z Reads: 184

```
No, no personal addresses at all. I sent you a PM with a screenshot of what I see.
```

---
## \#278 Posted by: banjaxxed Posted at: 2017-11-13T16:03:21.371Z Reads: 178

```
I paid up Rico, thanks
```

---
## \#279 Posted by: Steve-81 Posted at: 2017-11-13T21:17:36.455Z Reads: 183

```
Hello all :slight_smile:

I guess you are all as happy as I am, that our DieBies will be on their way in the near future :slight_smile:

By the way @fedestanco, I got some replies too, but hey, I think we are a good community, and we all make some mistakes sometimes :slight_smile:
```

---
## \#280 Posted by: Steve-81 Posted at: 2017-11-13T21:25:21.455Z Reads: 186

```
As soon as I will have some spare time, I will have a look in the firmware. I'm really curious what can be done with this masterpiece.

Maybe we should start a DieBieMS programming treat, maybe we have some ideas nobody else thought on, and someone has the ability to make it work. On the end we would have something even @JTAG couldn't imagine to be possible :slight_smile:

An we should build a sculpture to honor him :smiley:
```

---
## \#281 Posted by: banjaxxed Posted at: 2017-11-13T23:36:25.993Z Reads: 184

```
I believe their is a jtag mention on the pcb always good
```

---
## \#282 Posted by: JTAG Posted at: 2017-11-13T23:53:13.378Z Reads: 198

```
Hi guys!

See my update in the DieBieMS topic:
http://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/220

Ill be uploading the latest firmware tommowow, pinky pwomise!

(I will also reply to my PM tommorow, sorry for the wait :sweat:)
```

---
## \#283 Posted by: lock Posted at: 2017-11-14T00:05:48.307Z Reads: 209

```
@fedestanco just paid up for shipping, and sent through a fresh email with all details (shipping address, battery details).

After downloading the free version of Keil I received a follow up email from the local distributors. As stated above it's an expensive (for bobbyists) application, here a 1year license comes in at around 2300AUD and that's the cheap version.

[quote="Steve-81, post:280, topic:20947"]
Maybe we should start a DieBieMS programming treat...
[/quote]
Yeah, or possibly use JTAGs other development thread. Until there's consensus I'll just keep dumping my findings here.

Tried a few other things to get the build size down under the 32kB limit of the free Keil license. The build process generates a `.map` file that contains much useful info including the compiled size of different components...

There's 4 `printf` function calls in the entire firmware, all contained within the `modMessageQueMessage` function. Removing them drops the build size by around 2kB, but you loose out on debug info :unamused:. `printf` pulls in a bunch of other dependencies hence why 4 lines of code contributes so much to the build size.

The largest single component of the firmware is the 7 logos that indicate state on the oled screen. Dropping this down to 3 allows the application size to come in under the 32kB limit.... but that's not really a solution. Instead I'd probably resample these images from 128x64 to 64x32 (before and after examples below) and keep them all.

<img src="/uploads/db1493/original/3X/8/f/8f79d455898e1666bb38dd085d54f80becd9e6d8.png" width="417" height="110">

<img src="/uploads/db1493/original/3X/0/0/00785a0279d3ddab8080e287f0903398b47d3047.png" width="341" height="104">

I'll probably fork JTAGs repo and make these changes just in case anyone else wishes to build the firmware with the free version of Keil. It does involve a fair amount of compromise though, and not just the above hacks. Longer term you'll always be limited by the build size; adding new features would very quickly push it back above the 32kB limit. For the community to pickup firmware dev I think we'll really need to move onto another development stack (Eclipse + GCC ?).

**TL;DR** 
You can compile the firmware including your own custom pack configuration with the free version of Keil, assuming you are ok with some compromises.
```

---
## \#284 Posted by: JTAG Posted at: 2017-11-14T00:20:26.630Z Reads: 203

```
We should definitely step to another IDE!!!! I'll try visual studio with debugger asap, I have seen some nice things about that one.

If you know anything better please suggest ^^.
```

---
## \#285 Posted by: fedestanco Posted at: 2017-11-14T17:48:59.996Z Reads: 206

```
I should obtain the full version of keil through my university soon, so that I will be able to write custom configs for you.

Furthermore after some hours of torturing my bms I have got the correct wiring scheme of the lcd, power button and balance cables. (thanks to @JTAG for the help behind the scene)

<img src="/uploads/db1493/original/3X/6/d/6d541c538ed17d9ea41c37064e1494eacdd1412f.jpg" width="690" height="388">
```

---
## \#286 Posted by: JTAG Posted at: 2017-11-14T17:54:07.676Z Reads: 203

```
Awesome! such much capton tape xD!
```

---
## \#287 Posted by: JTAG Posted at: 2017-11-14T17:56:41.724Z Reads: 204

```
Are you hacking my BMS to operate without a main Fuse :expressionless:? :smiling_imp:?
```

---
## \#288 Posted by: fedestanco Posted at: 2017-11-14T18:20:48.119Z Reads: 211

```
[quote="JTAG, post:287, topic:20947"]
Are you hacking my BMS to operate without a main Fuse :expressionless:? :smiling_imp:?
[/quote]

I would never dare. Here you can see my homemade fuse. Made in Italy.
<img src="/uploads/db1493/original/3X/a/3/a3fec31759a2d24b48991878b4f2f5ffb52c0602.jpg" width="690" height="388">

I heard somewhere that the electrostatic discharge from the fingers could kill an IC. So I always kapton the shit out of my electronics.
```

---
## \#289 Posted by: JTAG Posted at: 2017-11-16T13:34:58.328Z Reads: 205

```
Dear all,

I noticed that some of you are getting your BMSes! AWESOME! I should really be starting with a manual now (will have my priority now).

If you are not absolutely sure on how to connect the balance leads please WAIT WITH THAT, when incorrectly connected components will blow :sob: :sob: (there is no easy way to protect against this). I will make a quick start guide hopefully tonight already :innocent: !
```

---
## \#290 Posted by: longhairedboy Posted at: 2017-11-16T14:10:44.155Z Reads: 205

```
not generating static helps. Shoes on carpet is silly, and dry air is a killer. 

we don't have dry air or carpet in the shop. hell most of the time i'm barefoot on cement. never zap anything. LAst time i zapped something it was the car door and i was in my winter gear. You know, those boots and that one jacket i only seem to need for a bout a week in January when it suddenly drops to a staggering low of 50F.
```

---
## \#291 Posted by: tobbs Posted at: 2017-11-16T14:34:52.879Z Reads: 210

```
JTAG, 
I have just connected a 4s LIPO battery to the BMS and are getting information about the V in each cell. It seams somehow confusing that the cell count starts at 0, is this correct?  
-----   Cell voltages   -----
Cell voltage 0           : 3.900V
Cell voltage 1           : 3.927V
Cell voltage 2           : 3.816V
Cell voltage 3           : 3.931V

Also, how is the charging enabled? I have connected a dc power supply with 28.8V to the common- and Charge+ and get the following readings:   
-----Battery Pack Status-----
Pack voltage          : 15.58V
Pack current          : 0.02A
State of charge       : 0.0%
Remaining capacity    : 0.00Ah
Operational state     : Power down
Load voltage          : 0.00V
Cell voltage high     : 3.931V
Cell voltage low      : 3.816V
Cell voltage average  : 3.894V
Cell voltage mismatch : 0.115V
Discharge enabled     : False
Charge enabled        : False
---End Battery Pack Status---
```

---
## \#292 Posted by: banjaxxed Posted at: 2017-11-16T16:04:08.324Z Reads: 199

```
I always rub my head with a balloon before working on electronics and frequently get a zap off my car
```

---
## \#293 Posted by: JTAG Posted at: 2017-11-16T16:06:52.128Z Reads: 217

```
@tobbs
Starting with 0 is a programmers thing, there everything starts at index 0 :laughing: .

Powering up the BMS can be done in 3 ways:

1. Trough power button (discharge / normal operation / usage)
2. Trough connecting an external power source to the charge port (charging)
3. By connecting USB (ext / configuration)

But state changes are only possible from 1(usage) to 2 (charging). There are a few motivations on why I think this is pleasant but that is to much writing :sweat_smile:. What everyone wants is up to preference / taste, but it is fixed for now.

0) In normal off state all the power to the microcontroller is disabled, it has no way to turn itself on. Once enabled by any of the three options it can keep itself enabled, but once it has disabled itself its back to having no control.

1) (BMS should be off without USB connected ) When you push the power button the power supply turns on enabling the microcontroller, the microcontroller wil then "bypass" the switch to keep itself enabled, it loads the config from the EEPROM and checks whether the loaded configuration matches the connected battery and whether all cell voltages are withing the specified limits, when anything is off / wrong it will depending on the level of the error either give a cross trough the battery (followed by waiting for a while) and turn of, or will state "err" and turn off immediately (happens really fast, you will probably be unable to see it). When everything is OK it will enable the LOAD and supply power to your target. It will keep it enabled for 30 minutes when the load consumes <200mA (else it will timout and turn itself off), when the load at any moment exceeds the 200mA threshold it resets the timeout.

Push button operation:

* Really fast -> the microcontroller had no time to respond, you are to fast, it will only blink the power button and turn back off immediately.
* Normal short press -> the BMS will turn on as expected
* LONG press -> Default config is loaded (be aware that this might be the WRONG config), state of charge is reset and YOLO mode is enabled. The BMS will enable its output and IGNORES ALL (cell voltage) LIMITS. This is useful when a balancing wire came loose and strange voltages are measured and the BMS disconnects the load. This mode is created to allow you to still ride home when a stupid balance lead breaks. This is a gray area (it might break your battery / BMS when you over discharge extremely), please prevent going here and using this :construction_worker:. This mode might need some improving sinds I stopped using it for a while since my balance leeds are now connected firmly :innocent:.

2) (BMS should be off without USB connected OR in usage / be in load enabled mode / be powered on by power button) This mode is enabled when you apply a voltage to the charge+ terminal that is 3V higher than the pack, It will again do all the checks of the regular power on but will enable its charge port instead of the load. You should use a current limited power supply since that power supply wil control the charge rate. 

The charge port / path is enabled when the batteries highest cell voltage is below the soft over voltage threshold, the current that flows at that moment tells the BMS that the charger is still connected (since it has now connected the charger to the battery it has no way of detecting the charger voltage). 

TLDR; use a CC CV charge with an open clamp voltage of at least 3V higher than the highest pack voltage you will reach with a full battery (to have the BMS still detect the charger). All my chargers (mainly PB lead battery chargers and CC CV LED power supplies always meet these requirements). 

This mode shows a charge lightning bolt thingy on the display.

1&2) When you connect a charger in usage mode it will switch to charging mode. When you disconnect the charger it wil wait for a while and turn itself off.

3) To enable this mode just plug in a USB cable and connect it to a computer. The 5V USB voltage will enable a circuit that forces the BMS to be turned on and remain on even when the configuration is wrong. This mode will show EXT on the display. You cannot get out of this mode unless you disconnect the USB.

--end of mode  description--

Short said -> when connecting the usb when the bms was off, you are stuck in this mode but have the freedom to change configuration with stuff happening to your battery (passive mode, no charger and load activity).

when you connect the usb whilst the bms is in charging or discharging mode you can do exactly the same but now you are in active mode and everyhing will respond directly to the changes you apply so be careful! Batteries are scary :mask: .

Also in the "help" list the command to change the battery cells is missing (I forgot to add it to the help list), the usage is:
config_set_cells 8
to set it to for example 8 cells.

Be sure to save the changes to EEPROM by:
config_write
```

---
## \#294 Posted by: chinzw Posted at: 2017-11-21T00:28:34.900Z Reads: 185

```
@fedestanco any news?
```

---
## \#295 Posted by: evoheyax Posted at: 2017-11-21T00:45:57.066Z Reads: 185

```
Any news when more may be for sale?
```

---
## \#296 Posted by: fedestanco Posted at: 2017-11-21T02:17:06.449Z Reads: 190

```
The custom firmwares that @JTAG  wrote for us seem to have a little issue. So all the boards are waiting on my desk to be flashed again.
Other than that screws are installed, address is written and some shipping labels have been purchased.
```

---
## \#297 Posted by: lock Posted at: 2017-11-21T02:32:36.429Z Reads: 200

```
Just on the custom firmwares... Not sure if you're still planning on doing a unique build (with battery specs) for everyone, but with JTAGs VESC Tool integration I'm not sure its really required. Firmware, yes, but it would probably be fine to use the same firmware on all the BMSes.

I'll be plugging mine up to the VESC tool first thing just to confirm all the settings are ok. Not that I don't have faith in you, just be a real shame to blow one of these up 😉.
```

---
## \#298 Posted by: JTAG Posted at: 2017-11-21T09:42:01.469Z Reads: 195

```
Hi Guys,

Yeah I specified the wrong hardware version in the firmware files (I am developing code on old hardware and forgot to change the hardware version) , therefore the firmware thinks its charging whilst its actually not because the microcontroller pin connections on the new hardware is different :rolling_eyes:. 

By the time I had to build the new firmware for @fedestanco I was right in the middle of implementing CAN and configuration of the BMS over CAN trough the VESC (that works now with the terminal). I am currently implementing BMS firmware updating trough the VESC-TOOL, I will try to get this work tonight and decide whether I trust it enough to implement it in the firmware ill send to @fedestanco or not. Ill send the firmwares tomorrow anyway and update here on what I did.
```

---
## \#299 Posted by: fedestanco Posted at: 2017-11-21T12:43:06.706Z Reads: 201

```
@lock your bms will be programmed according to a123 specs but yes, it is a good idea to double check via vesc tool.

@evoheyax keep in mind that I wont start a new batch before at least few weeks of feedback so if you are in a rush check out pcbway.com or macrofab.com
```

---
## \#300 Posted by: JTAG Posted at: 2017-11-22T23:33:15.321Z Reads: 207

```
https://www.youtube.com/watch?v=fnHclxArm9M

Firmware update demo! Have to go to bed now :frowning:, GF is complaining :construction_worker: :sob:.

Firmware version is only shown on startup (I "update" from 0.15 to 0.14). But all the heavy lifting is done now!
```

---
## \#301 Posted by: fedestanco Posted at: 2017-11-23T21:16:51.850Z Reads: 200

```
Hi, just a reminder: if you want the bms non programmed just shoot me a PM and I will ship the next day. I am not holding them hostage, I am just waiting for the last firmware to be available :)
```

---
## \#302 Posted by: Steve-81 Posted at: 2017-11-23T21:29:32.625Z Reads: 200

```
Hello, it's total fine for me, I don't have any problems with some days, weeks extra. We have ugly weather, so I have at least 2 months before I can ride.
```

---
## \#303 Posted by: fedestanco Posted at: 2017-11-28T18:05:37.192Z Reads: 205

```
Hi guys. The new firmware works nicely. Now you will be able to customize your config via usb using the vesc tool. 
I will be shipping everything tomorrow and the day after.
<img src="/uploads/db1493/original/3X/4/8/4861627171c43df50ad04b4e2ebd6a7acbe67b03.jpg" width="690" height="388">
```

---
## \#304 Posted by: chinzw Posted at: 2017-11-28T18:16:38.039Z Reads: 198

```
This is great news! Thanks for all your work fede!
```

---
## \#305 Posted by: longhairedboy Posted at: 2017-11-28T18:32:19.769Z Reads: 199

```
[quote="fedestanco, post:303, topic:20947"]
Now you will be able to customize your config via usb using the vesc tool.
[/quote]

<img src="/uploads/db1493/original/3X/5/b/5b992971d1281c8b82934878ffeaeded52732e2e.png" width="294" height="171">

mind blown. 

will there be.. like...a guide of some sort for all the options? or just a command interface via the console? some kind of --help?
```

---
## \#306 Posted by: fedestanco Posted at: 2017-11-28T18:40:45.936Z Reads: 198

```
I am writing a README pdf explaining step by step how NOT TO fry the bms and how to do simple stuff like connecting the LCD.
```

---
## \#307 Posted by: longhairedboy Posted at: 2017-11-28T18:42:24.245Z Reads: 196

```
that will be tremendously helpful.
```

---
## \#308 Posted by: JTAG Posted at: 2017-11-28T19:04:13.071Z Reads: 192

```
I will collaborate / work in parallel with @fedestanco with the manual, there are so many options. I hope to have the basics covered by the end of the week.
```

---
## \#309 Posted by: longhairedboy Posted at: 2017-11-28T19:11:19.401Z Reads: 201

```
Awesome!

I've got my screens, they showed up a couple of days ago. Can we get some more pics or clips of the display when it has a charge? 

Also is there a way to get it to show balance info? or are those all options?
```

---
## \#310 Posted by: JTAG Posted at: 2017-11-28T19:22:02.043Z Reads: 200

```
Yes! I will look into showing some more interesting stuff on the display instead of the current boring stuff. Most of the annoying and boring stuff has now been addressed (accept for the custom UI). I will start using the github page for requests and bug tracking.
```

---
## \#311 Posted by: longhairedboy Posted at: 2017-11-28T19:22:59.031Z Reads: 202

```
i know firmware updates will be possible of course but will there be a way to alter things like startup bitmaps and things like that? I saw earlier in the thread that was happening. I was just wondering if that was going to be available for anyone to do.
```

---
## \#312 Posted by: JTAG Posted at: 2017-11-28T19:26:08.671Z Reads: 203

```
I expected that one :innocent:, I will look into that, I want to prevent using the regular configuration flash for that but I think I have a solution for that, a bit hacky but doable :grin:.
```

---
## \#313 Posted by: banjaxxed Posted at: 2017-11-28T19:26:59.171Z Reads: 200

```
Faaaaark this is so deadly!!!!
```

---
## \#314 Posted by: longhairedboy Posted at: 2017-11-28T19:28:06.544Z Reads: 199

```
i'm perfectly ok with hacky! That display is going directly over my front truck.
```

---
## \#315 Posted by: Steve-81 Posted at: 2017-12-06T18:56:06.259Z Reads: 195

```
Hello all

@fedestanco any news about those DieBies?

What kind of boards will you guys build them in to? I guess most of us will use Lion packs. I'm going to use it for a 10s6p pack, for a mountainboard with dual drive.
```

---
## \#316 Posted by: chinzw Posted at: 2017-12-06T18:58:58.504Z Reads: 189

```
Mine arrived in the mail yesterday, will probably start setting it up today.
```

---
## \#317 Posted by: longhairedboy Posted at: 2017-12-06T18:59:26.474Z Reads: 198

```
Mine are wandering around town and have been for the last two days. 

Not in boards, in UPS delivery trucks. They're rescheduled delivery twice already and when i called, they simoly explained that the item has been scanned on the big truck, but not offloaded yet onto the delivery trucks. They cite holidays. 

two days. 

i'm telling you people there's not enough selective serotonin re-uptake inhibitors for this shit man. The rage blooms.
```

---
## \#318 Posted by: Steve-81 Posted at: 2017-12-06T19:03:47.712Z Reads: 191

```
@longhairedboy I can imagine you are pissed up like.....

Look, I live in Hungary, Europe, not far from Italy, but in the eyes of UPS, it is like I would live on a different Planet :slight_smile:

So don't tell me about the nice UPS group :slight_smile:
```

---
## \#319 Posted by: evoheyax Posted at: 2017-12-06T20:23:48.935Z Reads: 194

```
Can't wait for more testing with this bms. If anyone has an extra one they would like to part with for testing, I want to work on linking this to the vesc via uart so we can forward the data to your phone :)
```

---
## \#320 Posted by: longhairedboy Posted at: 2017-12-06T20:29:52.158Z Reads: 198

```
or to the photon remote!
```

---
## \#321 Posted by: evoheyax Posted at: 2017-12-06T20:32:47.685Z Reads: 201

```
Yep. All needs to be done. Don't know why we haven't gotten the community together to build a bms + remote + phone system that plays nice with the vesc. Do you have any spares @longhairedboy? Know you got your hands on a few :)
```

---
## \#322 Posted by: longhairedboy Posted at: 2017-12-06T20:37:26.335Z Reads: 212

```
i have four BMSs coming any minute and the photon remotes should be on their way any day now. I'm going to hit him up again about a status update.
```

---
## \#323 Posted by: longhairedboy Posted at: 2017-12-06T22:29:30.812Z Reads: 213

```
yayyyyyyy!!!!

https://www.instagram.com/p/BcYGzElFby3/?taken-by=longhairedboy
```

---
## \#324 Posted by: lock Posted at: 2017-12-06T22:58:56.664Z Reads: 210

```
Dammit! At least you guys can work through all the kinks before mine shows up😉

@fedestanco have these all been shipped? And if so could you send me through a tracking number, I quite enjoy refreshing tracking site pages... apparently.

Christmas seems to have really clogged up the local post service. Another package I had shipped from the UK on the 15th of Nov, and I'm still waiting for it to show.
```

---
## \#325 Posted by: fedestanco Posted at: 2017-12-06T23:37:12.790Z Reads: 209

```
Hi guys. Everything has already been shipped on thursday, as promised.
Sorry if I haven't emailed you the tracking numbers yet, tomorrow I will do that.

Btw my PC stopped working so I still haven't started making the HOW-TO pdf.
Maybe I will draw the very basic instructions on my phone and publish them here.
```

---
## \#326 Posted by: deucesdown Posted at: 2017-12-07T15:38:13.282Z Reads: 203

```
I think I felt something move down below. Is it weird that a photo of a BMS has this effect?
```

---
## \#327 Posted by: longhairedboy Posted at: 2017-12-07T17:59:43.832Z Reads: 204

```
take your time on the instructions, i'd rather have them right then right now. :slight_smile:
```

---
## \#328 Posted by: chinzw Posted at: 2017-12-12T23:28:43.869Z Reads: 200

```
Does anyone have a copy of vest tool 0.82? That's the version we need to connect to the bms.
```

---
## \#329 Posted by: lock Posted at: 2017-12-12T23:48:27.844Z Reads: 201

```
If you have a Mac? -> https://github.com/rpasichnyk/vesc_tool/releases
```

---
## \#330 Posted by: chinzw Posted at: 2017-12-14T06:42:51.389Z Reads: 210

```
Finally got everything working! Screw terminals are a walk in the park, love them!
Here's some pics:
<img src="/uploads/db1493/original/3X/8/3/83158dd7842a2aae44a1a2d5dd2be52756ecdcaa.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/b/4/b49b606f982e357c5235455de9e0e4d41f190999.jpg" width="375" height="500">

@fedestanco @JTAG you guys did an awesome job!
```

---
## \#331 Posted by: JTAG Posted at: 2017-12-14T13:09:27.322Z Reads: 206

```
Dajum this is clean! Love the display, and the wiring! It all looks so neat.

Where did you find the display?
```

---
## \#332 Posted by: chinzw Posted at: 2017-12-14T18:03:45.914Z Reads: 208

```
Thanks! Its super easy to have clean wiring with screw terminals :slight_smile:

I got the display from ebay, i prefer this one as its a bit smaller, 32pixels vs 64: https://www.ebay.ca/itm/332047978840
```

---
## \#333 Posted by: JTAG Posted at: 2017-12-15T01:44:45.233Z Reads: 211

```
So you updated the driver and images to support this new resolution? Respect!
```

---
## \#334 Posted by: chinzw Posted at: 2017-12-15T02:00:00.062Z Reads: 208

```
No, just used the defaults, its just squeezed.
```

---
## \#335 Posted by: oyta Posted at: 2017-12-16T16:15:52.543Z Reads: 236

```
Wow! Finally received it. Looks good :slight_smile:
<img src="/uploads/db1493/original/3X/d/a/da311f02657664069b2edac6cd52a8dbc68a9d14.jpeg" width="375" height="500">
<img src="/uploads/db1493/original/3X/5/a/5a87efc5c9dd3cfce743f8b35b5e330fe4275065.jpeg" width="666" height="500">

The winter has come around here, so I will install this the coming months.
```

---
## \#336 Posted by: fedestanco Posted at: 2017-12-16T22:08:06.435Z Reads: 237

```
Hi guys. I almost forgot the most the most important thing: donations. I ordered few extra naked pcbs; 100% of this sale's profits will be forwarded to @jtag's paypal.

2oz copper on inner and outer layers
enig gold immersion
fr4 laminate

oshpark price: 130$ for 3
**my price: 15euro/each** (please buy 2 at least)

<img src="/uploads/db1493/original/3X/4/0/4071c259ec178a801985f020b78b9554d481bdda.PNG" width="690" height="280">

<img src="/uploads/db1493/original/3X/b/d/bd09a9973fec505859b3f64604bc6a009eea6123.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/0/7/0716dd88c6987771167dbb1db4d047dcba7dbf32.jpg" width="690" height="388">

*sorry for pics quality
```

---
## \#337 Posted by: longhairedboy Posted at: 2017-12-21T16:02:41.421Z Reads: 222

```
[quote="fedestanco, post:336, topic:20947"]
oshpark price: 130$ for 3
[/quote]

is that for just the PCB without the pressed in terminals or anything baked onto it?
```

---
## \#338 Posted by: fedestanco Posted at: 2017-12-21T16:49:02.458Z Reads: 223

```
Pcb as shown on picture (no components installed). Somebody may not agree with me but I believe oshpark is definitely overpriced.
```

---
## \#339 Posted by: longhairedboy Posted at: 2017-12-21T17:09:52.233Z Reads: 225

```
That's ludicrous. $43 per unit is ludicrous, even for that level of complexity. 

I want to try my hand at baking these on my own. I just bought a reflow oven. I'm also hoping to be able to bake the rest of the things i use in house as well, such as the VESC6 and my eswitches. 

I'm tired of relying on volatile supply chains, and any chance to use elbow grease instead of cash is worth looking at.
```

---
## \#340 Posted by: fedestanco Posted at: 2017-12-21T17:29:28.904Z Reads: 227

```
I believe hand soldering is only good for prototyping and repairs.
Are the 20$ you save hand making vescs really worth 2 hours of your time?
The truth is everytime I imagine you doing repetitive stuff like spot welding, I die a little inside. You are here to make art, let robots(or chinese) do the copy-paste job.

Btw no matter how hard you try, new generation pick&place robots will always be much more accurate than human shaky hands :slight_smile:
```

---
## \#341 Posted by: longhairedboy Posted at: 2017-12-21T18:24:53.375Z Reads: 235

```
You may have missed the part where i mentioned i bought a reflow oven. I'm not scared of manual pick-n-place, nor am i currently under any pressure to produce these. If it doesn't work out oh well. 

Don't die inside. If you had any idea how much money i save building my own packs you'd feel better.  I'm also damned good at it now and can knock out even a huge pack in just a couple hours. The evolve mods, for instance. The entire mod, machining the deck, welding and wiring the pack, and installing everything and testing is only three hours now. Last year it would have taken me all day. 

Besides, if works out i can hire some kids to come in and do the manual stuff. 

Look at what @chaka is doing. Lots of people thought it was a bad idea for him to vertically integrate as well. Now he's got the best 4.12 format direct fet VESC in existence.  Eventually i'm going to do it regardless but i thought i would start dipping a toe into making things now instead of next year. 

I'm starting with this:
https://oshpark.com/shared_projects/MSM2M9LC

Its just a simple triple FET eswitch with support for LED angel-eyes. I just ordered 9 of them and i'm going to make them myself to get an idea of how stupid this plan really is. I'll probably do a VESC 4.12 next to get a handle on it before i do anything more complex. 

There is no timeline on this, i'm already very busy, but it needs to happen eventually so why not start trying things out between stuff in my wait-time. 

i know its hard to tell sometimes.. but i'm building a factory. And as the Steeze Lord of this factory, i must have knowledge of all workings and understandings. If i haven't at least tried my hand at pick-n-place-n-bake-n-spray then i would have failed everyone.
```

---
## \#342 Posted by: banjaxxed Posted at: 2017-12-21T20:49:24.273Z Reads: 223

```
Mine arrived maximus happimus
```

---
## \#343 Posted by: fedestanco Posted at: 2017-12-21T20:59:32.636Z Reads: 224

```
[quote="longhairedboy, post:341, topic:20947"]
You may have missed the part where i mentioned i bought a reflow oven.
[/quote]
This is great, being able to repair stuff on your own is faster and cheaper.

[quote="longhairedboy, post:341, topic:20947"]
Look at what @chaka is doing. Lots of people thought it was a bad idea for him to vertically integrate as well. Now he's got the best 4.12 format direct fet VESC in existence.
[/quote]
The only companies that are doing well in my country are following the same plan: do it locally and do it better. Maybe if oshpark started a USA pick&place service he'd jump on that; the premium package he sells contains extreme QC, R&D, amazon's style service. Auto-assembly wouldn't ruin any of that.

Interesting fact: Michelangelo did't fisically paint all of his paintings; he had assistants to fill most of the easy and repetitive sections like the sky.
```

---
## \#344 Posted by: chinzw Posted at: 2017-12-22T03:52:03.613Z Reads: 208

```
@JTAG hey mate, any plans on adding a custom charge voltage?
I want to undercharge my cells to 4.1v, not sure if Soft/Hard Over voltages would do this.
```

---
## \#345 Posted by: JTAG Posted at: 2017-12-22T12:29:51.311Z Reads: 207

```
What are you asking :sweat_smile:? I don't understand. You can change every voltage you like as long as you stay withing the hardware limits of the chips.
```

---
## \#346 Posted by: longhairedboy Posted at: 2017-12-22T13:34:57.738Z Reads: 208

```
this is perfect. We can leave plenty of room at the top of the pack for braking regen.
```

---
## \#347 Posted by: chinzw Posted at: 2017-12-22T17:29:45.761Z Reads: 212

```
So the soft over voltage will stop the charging process when reached?

Btw, one thing people should be aware of is the 3v higher than the pack voltage for charging. If you disconnect the charger when the pack is close to fully charged, and connect it again then you'll end up with a  pack at less than full charge.
```

---
## \#348 Posted by: Steve-81 Posted at: 2017-12-22T18:19:17.113Z Reads: 217

```
Sounds good that you guys are all working on your DieBie-s :slight_smile:
Mine's still in Italy, the post was so super that they needed more then 2 weeks to get it into international center, but still there.
It is so unfair, for UPS Hungary isn't Europe, we belong to an other zone (I guess I'm the closest to Italy) from all of us....
Hopefully mine will arrive once in January :slight_smile:
```

---
## \#349 Posted by: fedestanco Posted at: 2017-12-22T19:58:02.402Z Reads: 210

```
Have you tried to use the tracking number on your local post service's website?
It is very odd that a package remains too long at the int.fulfillment centre. 
Some Australia guy already received his box btw.
```

---
## \#350 Posted by: Steve-81 Posted at: 2017-12-22T20:18:11.343Z Reads: 216

```
no I haven't but I guess you looked at the italian, and you can see that the package was hold for 2 weeks on 1 place.
I hate everything that's state property, they always are slow, doesn't mater wich country, they can only hire people who don't have a clue to anything....
But, never mind, I'm not fed up, it's not urgent for the BMS to arrive, it's only annoying that they can't manage anything right. If we would work like this at our jobs, our companies would go bankrott :)
```

---
## \#351 Posted by: Steve-81 Posted at: 2017-12-22T20:21:24.427Z Reads: 216

```
I just had a look, item sent abroad, but not in the destiny land now

Post :)
```

---
## \#352 Posted by: Steve-81 Posted at: 2017-12-22T20:24:05.396Z Reads: 215

```
Sorry for the 3rd post in a row, but:

- Shouldn't we make a small paypal for @JTAG? He made a great job with that
```

---
## \#353 Posted by: Johan_R Posted at: 2018-01-04T10:14:12.342Z Reads: 219

```
SO THRILLED ABOUT THIS BUILD! 

Its truly amazing what is being created on this forum!

I imagine that the all of the BMS from this batch is sold already.
So from now, how is it possible to get this BMS in my hands?

/Johan
```

---
## \#354 Posted by: Olloxan Posted at: 2018-01-07T02:25:27.901Z Reads: 215

```
I would like to get one too, if its possible!
```

---
## \#355 Posted by: stewii Posted at: 2018-01-09T18:05:13.934Z Reads: 217

```
Is there still any PCBs left?
```

---
## \#356 Posted by: fedestanco Posted at: 2018-01-09T18:28:03.800Z Reads: 213

```
Yes, only unassembled pcbs.
```

---
## \#357 Posted by: NoWindCH Posted at: 2018-01-09T21:43:52.249Z Reads: 212

```
Hallo from Schwizerland :smiley:

Can i order one too?
```

---
## \#358 Posted by: evoheyax Posted at: 2018-01-16T21:02:17.176Z Reads: 206

```
Any news lately on this?

Still very interested in some completed units.
```

---
## \#359 Posted by: fedestanco Posted at: 2018-01-17T10:52:26.695Z Reads: 209

```
Sorry if this is going slow but I want "beta testers" to write brief reviews before launching another batch. 
If you consider the amount of variables involved it's easy to understand why I want to eliminate the bad suppliers&factories from my list (if there is any). Especially because the next batch will be bigger.

If you are in a rush though, you can buy the unassembled pcb and make your own. (btw only 4 left).
https://www.electric-skateboard.builders/t/diebie-jtag-12s-bms-gauging-interest-nonprofit/20947/336?u=fedestanco
```

---
## \#360 Posted by: longhairedboy Posted at: 2018-01-17T13:38:55.276Z Reads: 208

```
Is there a readme published yet with configuration instructions or some kind of terminal software yet for it that isn't BLDC tool?

Mine are still in the box because of a lack of documentation. If i missed it somehow, please point me to it.
```

---
## \#361 Posted by: evoheyax Posted at: 2018-01-17T17:46:28.222Z Reads: 232

```
I would buy the pcb and assemble. But Unfortunately, I don't feel confident enough. I've been wanting to try assembling a vesc 4.12, which is less complex than this, and that scares me still, haha. One day though, I will.

Especially since this is still beta, I would feel safer buying an assembled one first, so that if it does fail, I know it's not my assembly.

I will keep waiting. Hopefully the 30T cells are ready by then also. Just a bummer, cause I have some battery packs to sell to customers in the coming months and I really don't want to use the shitty bms's out there. This would make a battery pack proper ;)
```

---
## \#362 Posted by: fedestanco Posted at: 2018-01-18T19:53:42.602Z Reads: 235

```
Exam period started again so no time to write an how-to.
You can get started with these schemes and ask questions if you have doubts.
![image|690x330](upload://4sy3718Hll7bEfheqehAJP4SWpy.png)![diebiebms_wiring|690x339](upload://g1MozQD3E7qqwo5egVSjSyPHBRq.jpg)
```

---
## \#363 Posted by: longhairedboy Posted at: 2018-01-18T20:15:38.043Z Reads: 218

```
i need to just hire somebody. Damn kids in school are so casually on the bleeding edge and holding all the cards.
```

---
## \#364 Posted by: evoheyax Posted at: 2018-01-19T04:03:34.799Z Reads: 215

```
I can help you figure it out... I'll need one to test though *cough* *cough* :grin:
```

---
## \#365 Posted by: chinzw Posted at: 2018-01-22T22:30:02.191Z Reads: 213

```
If you need help i can help you out through skype/hangouts. I've got my bms setup and working.
```

---
## \#366 Posted by: lock Posted at: 2018-01-23T11:12:37.091Z Reads: 220

```
I'd be interested in knowing how to unbrick one of these... I swear I haven't busted one yet :grimacing:

I have one of those mini ST-Link V2 USB sticks; just no idea how to connect it and what to watch out for. For example I know with the VESC you have to be careful not to connect up the VCC pin from the ST-Link, that sort of thing.

I'd like to add firmware update capability to that command line app, and given my track record with all things software it's unlikely to work first time. Not working in this instance probably means I'll be turning one of these into a brick (and then hopefully fixing).
```

---
## \#367 Posted by: chsw Posted at: 2018-02-08T10:44:26.856Z Reads: 207

```
I would order a PCB if there is one left. Thanks for letting me know.
```

---
## \#368 Posted by: fedestanco Posted at: 2018-02-08T20:54:07.771Z Reads: 200

```
You mean bare pcbs like these? https://www.electric-skateboard.builders/t/diebie-jtag-12s-bms-gauging-interest-nonprofit/20947/336?u=fedestanco
```

---
## \#369 Posted by: fedestanco Posted at: 2018-02-08T20:56:39.082Z Reads: 200

```
You can connect both 3v and ground safely if you unplug the battery and the balance cables.
```

---
## \#370 Posted by: chsw Posted at: 2018-02-08T23:16:16.478Z Reads: 196

```
Yes. A bare PCB is fine.
```

---
## \#371 Posted by: riva_00 Posted at: 2018-02-15T11:51:32.501Z Reads: 200

```
I want this so much, any update on when it'll be sold as a completed thing?
At the moment i'm charging my LiPO's separately, and holding out for this monument of gloriousness.
```

---
## \#372 Posted by: amees_me Posted at: 2018-02-19T09:40:30.484Z Reads: 200

```
Also very much interested in this BMS, it looks incredible. Almost finished modelling my board, next up is an electronics buying-spree :).
```

---
## \#373 Posted by: fedestanco Posted at: 2018-02-20T17:03:48.985Z Reads: 198

```
@riva_00 @amees_me We don't know enough about reliability yet to run another, bigger batch right away.

For example it'd be interesting to know how 12s is holding up; we opted for irfs7530 which has proven to fail usually when used on antisparks at 12s. But since @JTAG has redesigned the precharge in a new different way, these 60v mosfets should work just fine.
If I am not wrong @lock you were running 12s, have you managed to blow something?
```

---
## \#374 Posted by: lock Posted at: 2018-02-20T22:01:56.566Z Reads: 192

```
Not yet 😉

Worked fine with 12s in my [load testing](https://www.electric-skateboard.builders/t/load-testing-discharging-a-custom-battery-pack/2888/19), but that was with a maximum of 6a. Also, using A123 cells means my 12s pack is more like an 11s pack in terms of voltage.

Just waiting on a few bit from Shapeways so I can finally finish the board and get some real world testing done. Should only be a week or two, but I’ve been saying that for months 😩.
```

---
## \#375 Posted by: PatRocks Posted at: 2018-02-21T00:24:51.199Z Reads: 186

```
I'll test the SHIT out of one, if I can get ahold of one lol. My packs are huge, and kinda old so it might actually be a good idea (wink wink). Could get some real stress test results!!
```

---
## \#376 Posted by: evoheyax Posted at: 2018-03-06T03:37:21.123Z Reads: 185

```
Any more news? Really need one of these. Willing to pay extra to have one made ASAP.
```

---
## \#377 Posted by: lock Posted at: 2018-03-06T04:09:08.953Z Reads: 196

```
Haven't killed mine yet, although it really hasn't been pushed hard. Auto off is nice, kind of wish my remote did the same. OLED display is hard to see in direct sunlight, but that's not really the BMS' fault.

The PCB has a buzzer, but I've never heard it make a sound. Is this expected?

![IMG_2067|375x500](upload://q3fYObd7Ts324yV15AWIPJy7Kr1.png)
```

---
## \#378 Posted by: JTAG Posted at: 2018-03-06T05:42:14.553Z Reads: 187

```
Yeah haven't implemented the buzzer yet :grimacing:.

And yeah, we should look for I2C E-Ink displays !!!!
```

---
## \#379 Posted by: lock Posted at: 2018-03-06T05:55:29.362Z Reads: 188

```
Some kind of startup chime (ala Window's sound) and shutdown would be great. That way when it shuts down it'll alert me and I can double check I've turned off the remote too. Maybe a beep if the battery gets below 10% or so... Actually, pretty much any event could have its own special sound/beep (I have no idea what sounds the buzzer is capable of producing). Also my BMS is inside a box, and that box is inside my enclosure, so it may not be audible anyway.

Funny that, just had a look around and there are several e-ink displays that would seem to be close to working (i2c, but diff resolution). I don't see the slow refresh rate being an issue with what a BMS would display either. [I once had a phone](https://en.wikipedia.org/wiki/Motorola_Fone) with an e-ink display, one charge would last a week, the only issue was that when it died you'd never know as it kept displaying whatever was last on the screen 😂.
```

---
## \#380 Posted by: bevilacqua Posted at: 2018-03-06T07:41:37.321Z Reads: 180

```
off topic: The newest maytech remote (proven reliable) has a auto-off feature. After 5min of lack of connection to the board it shuts down.  

Looking forward to the public release of the DieBie JTAG BMS :)
```

---
## \#381 Posted by: JTAG Posted at: 2018-03-06T10:56:18.742Z Reads: 180

```
SHARE LINKS! :grimacing:
```

---
## \#382 Posted by: bevilacqua Posted at: 2018-03-06T11:26:53.799Z Reads: 192

```
https://www.indiegogo.com/projects/light-phone-2-smartphone-design#/
stil on crowdfunding stage though
```

---
## \#383 Posted by: lock Posted at: 2018-03-06T12:25:31.309Z Reads: 196

```
So there’s [this](https://www.tindie.com/products/alexchu/e-ink-e-paper-new-version-display-module-33v-204/). At first look I thought it used the same driver as the oled (ssd1306), but it’s using the ssd1606 and I’m guessing that means you’d need to use a new graphics lib.

You’d also need to slow down the screen updates to once every second. But the bigger issue I see with these eink displays is that they seem to come and go. Whereas those $4 oled displays are available pretty much everywhere.
```

---
## \#384 Posted by: JTAG Posted at: 2018-03-06T12:50:47.222Z Reads: 191

```
Interesting! Somewhat expensive trough :sweat:. I hope more boards like this become available soon!
```

---
## \#385 Posted by: banjaxxed Posted at: 2018-03-07T23:47:48.491Z Reads: 197

```
Like a kindle huh?
```

---
## \#386 Posted by: Mike_Lemon Posted at: 2018-03-09T18:03:38.625Z Reads: 195

```
90 euro?! How did it get so expensive? 

I'd be comfortable to pay 50Euro for one piece and 40 for bulk, would this be possible somewhen in the future?
```

---
## \#387 Posted by: fedestanco Posted at: 2018-03-09T18:43:07.193Z Reads: 198

```
Firstly it was 104 euro and not 90. Now that we have clariefied that you didn't even read one post about this thread let me summarize for you:
If you were to buy BARE pcbs on oshpark, these ALONE would be 50$ each including tax(https://www.electric-skateboard.builders/t/diebie-jtag-12s-bms-gauging-interest-nonprofit/20947/336?u=fedestanco).
Then the BOM at quantity 20 was around 100 on farnell. Farnell prices are without VAT, so including tax that would be 120eur.
Then there is the pick and place assembly which was around 18eur/ piece if I remember correctly.
Then there is the custom made balance cable, 22awg; this thing weights like 10 times a canbus cable (which is sold for 3eur).  I managed to bring the price down to 4 euro.

In a nutshell if today you wanted to make another 20 pieces batch with the original BOM in China, it would cost you at the very least 140eur/each using the shittiest pcbs you can find, and without cables, and shipping.


If I haven't convinced you yet about the nonsense of your comment consider this: a vesc 4.12 costs about half to produce compared to these bms'. Translating your comment in vesc terms, for you a 45eur vesc would be too expensive and you would only be confortable buying a 25eur one. Good luck finding one.
```

---
## \#388 Posted by: Mike_Lemon Posted at: 2018-03-09T19:03:45.646Z Reads: 192

```
So first of all if the product costs so much these is absolutely no point of making it sins the thing it's suppose to "protect" may cost around half that price to make.

Second there are alot of great PCB manufacturers that can make those PCB's for cheaper like PCB way and there is defiantly no need for 2oz 4 layer board for that application(Have some experience with making compact PDB PCB along the BMS in progress) 
Can't understand how the actual BOM reached so high just look up at digikey you should find pretty good prices for components there.

and the price of the VESC is mostly justified sins the BOM includes the 6 and the two small high precision shunts which are quite expensive and the two sided PCB smd assembly along with the 4 layer PCB to make it super compact, can't imagine how it could get any smaller sins there are just components every where on any side.
```

---
## \#389 Posted by: fedestanco Posted at: 2018-03-09T19:23:36.935Z Reads: 195

```
[quote="Mike_Lemon, post:388, topic:20947"]
these is absolutely no point of making it sins the thing it’s suppose to “protect” may cost around half that price to make
[/quote]
c'mon have you at least read the title of the thread? I am the guy how produced them. If you came here for complaints about the design you should report the here: https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639. And BTW how can you even complain for a project that a professional EE made in his free time and he shared for free... at most you could  make a pull request from github

[quote="Mike_Lemon, post:388, topic:20947"]
Second there are alot of great PCB manufacturers that can make those PCB’s for cheaper like PCB way
[/quote]
We also had a quote from them, they were more expensive by 15eur and quality was not as controllable.

[quote="Mike_Lemon, post:388, topic:20947"]
is defiantly no need for 2oz
[/quote]

since it'a high current pcb, 1euro spent on 2oz is a good investiment

[quote="Mike_Lemon, post:388, topic:20947"]
digikey you should find pretty good prices for components there
[/quote]
all the distributors' prices vary amoung a 10% margin at 20pcs batch

[quote="Mike_Lemon, post:388, topic:20947"]
price of the VESC is mostly justified sins the BOM includes the 6 and the two small high precision shunts which are quite expensive
[/quote]
the 2 WSLP2726 shunt resistors on vesc 4.12 are half of the cost of ONE wurth screwholder. And this bms has 6 screwholders.

[quote="Mike_Lemon, post:388, topic:20947"]
and the two sided PCB smd assembly
[/quote]
diebiems also requires a 2 side assembly
```

---
## \#390 Posted by: JTAG Posted at: 2018-03-09T19:53:13.816Z Reads: 181

```
Ow man, this guy is unbelievable. Please do better or go home xD. Nobody wants you to build this or buy this in any way or sense.
```

---
## \#391 Posted by: linsus Posted at: 2018-03-13T14:26:13.362Z Reads: 183

```
Any plans on a new batch of completes? :slight_smile:
If not, I'd love a bare PCB..or two! If there are any left. I'm one of those fanatics who find soldering, rather relaxing, worked my way thru a couple of vescs without any smoke so this should be a breeze :D
```

---
## \#392 Posted by: Acido Posted at: 2018-03-13T14:36:02.100Z Reads: 186

```
I don't think that pcbs are that expensive, check at a different factory like 50e for one is a ripoff
```

---
## \#393 Posted by: fedestanco Posted at: 2018-03-13T14:54:40.760Z Reads: 189

```
They re indeed much cheaper in China. Oshpark price is for reference.
I am selling the leftovers for 15€ for example.
```

---
## \#394 Posted by: fedestanco Posted at: 2018-03-13T14:56:54.582Z Reads: 187

```
Yes there are 3 bare pcbs left, PM me if you want a couple. Just a reminder:100% of the profits from this sale are going to jtag to support further developmemt of the product.
```

---
## \#395 Posted by: Olloxan Posted at: 2018-03-30T07:43:38.278Z Reads: 178

```
Hi @fedestanco,
i wanted to ask, if there are any news on a possible next batch of BMS. Did you get any responses from the current users (testers) yet to assess the choice of used controlers etc.? As summer is getting closer, starting the build is getting interesting again :slight_smile:
```

---
## \#396 Posted by: fedestanco Posted at: 2018-03-30T20:25:15.474Z Reads: 177

```
I am learning Altium so that I can play with the design and optimize costs.
The goal would be to find cheaper solutions for non critical components like : sound buzzer,
less connectors, xt90 instead of screwholders . This way I could make some profit to keep up the motivation and at the same time keep the price steady.
```

---
## \#397 Posted by: lock Posted at: 2018-03-30T23:30:29.826Z Reads: 177

```
I’d probably prefer xt90s, somewhere (on this forum) I saw a pcb mount version was coming out. Maybe jst-ph connectors for the display and power button. Nothing against what the DieBieMS uses right now, it’s just that people are more likely to have jst-ph sitting around as that’s what the vesc uses.

It’d be nice if this was commercialised, and I think there’s pricing room to support your time investment in order to make it sustainable. The Energus TinyBMS sells for about twice what the last group buy price was, specs are comparable.

I keep meaning to have a go at getting the source compiled with gcc, and then start having a play round.
```

---
## \#398 Posted by: uigiroux Posted at: 2018-04-03T20:49:04.752Z Reads: 178

```
So I've been through all the threads for this BMS but am not sure exactly if these are being made and sold or if they are going to be soon...?  Could someone please guide me to where I can place an order if they are available, and also how much?  I noticed there is a LCD display we can hook up, what is the main reason for that?  Thanks for your help guys!
```

---
## \#399 Posted by: chinzw Posted at: 2018-04-03T20:53:04.039Z Reads: 178

```
you didn't go through the threads, otherwise you'd know that @fedestanco made a limited run and that's it for the moment. He has a few spare unpopulated boards, but nothing else at the moment.
```

---
## \#400 Posted by: uigiroux Posted at: 2018-04-03T20:56:48.393Z Reads: 179

```
I did go through the threads,  and I specifically saw that they were made in a limited run, but then some others were talking about making them themselves to be sold so I wasn't sure if some one had started that or if we would have to build ourselves since it's open source.
```

---
## \#401 Posted by: fedestanco Posted at: 2018-04-03T22:07:01.310Z Reads: 177

```
If you want one to be made asap upload the pcb files to pcbway.com or macrofab.com
```

---
## \#402 Posted by: uigiroux Posted at: 2018-04-03T23:15:35.956Z Reads: 183

```
They'll make a complete one with all the firmware uploaded and everything?

Also, does it come with the LCD display or does that have to be added myself. 

Lastly, would you consider this better than any bestech or other name brand BMS?  From what I read about all it can do along with the fantastic design it sure seems to be the best one anyone could get...
```

---
## \#403 Posted by: longhairedboy Posted at: 2018-04-03T23:24:56.275Z Reads: 191

```
i finally got mine wired up. It's amazeballs! Its breathing new life into an older 25R 12S5P i've been riding around on since early last year. 

Is there a standalone terminal for this thing yet or do i still need to use vesc/bldc tool or whatever people are calling it now?
```

---
## \#404 Posted by: uigiroux Posted at: 2018-04-04T00:30:57.609Z Reads: 191

```
Damn I'm so jealous... I really want to order a few of these...
```

---
## \#405 Posted by: chinzw Posted at: 2018-04-04T00:37:36.708Z Reads: 197

```
gotta use the vesc tool for now.
```

---
## \#406 Posted by: lock Posted at: 2018-04-04T01:04:11.436Z Reads: 197

```
Or if the thought of a little Python (programming language, not snake) doesn't put you off...

https://github.com/lachlanhurst/diebiems-cmd-terminal

You don't actually need to program, but the install process requires a certain level of technical ability. Always meant to wrap a GUI around this.
```

---
## \#407 Posted by: uigiroux Posted at: 2018-04-04T01:12:50.981Z Reads: 196

```
Would they charge a reasonable fee for just a one off, or would I need to gather others to get a larger order?  How much were these when you sold them.  I think I saw like $90ish?

Do you still have the 3 PCB's you mentioned a few days back? If you do would you be willing to make a complete or more?
```

---
## \#408 Posted by: chinzw Posted at: 2018-04-04T01:20:23.251Z Reads: 199

```
Those are PCB making companies, they dont actually solder components to them, just the boards.
```

---
## \#422 Posted by: oyta Posted at: 2018-04-05T20:49:34.025Z Reads: 193

```
![esk8 wiring with DieBieMS-2|690x253](upload://9P6WNobs1HxK72i0vsdfnBYdRmL.png)
As the winter comes to an end I will start mounting the BMS :smiley: I have left out the wires to the display and power as that is documented earlier in this thread.

So I wonder:

1. Do the wiring scheme look sane? :blush:
2. Do I need an XT90 antispark on the COMMON- to the VESC?
3. The T1, T2 and TGND on the Molex Connector are optional I presume? Is it for temperature sensor on the battery?
```

---
## \#423 Posted by: Brad Posted at: 2018-04-05T23:31:04.049Z Reads: 192

```
Scheme appears to be the same as what I will be doing.

T section is optional, I do not think JTAG has done the software for it yet. Yes it is for temperature sensors.
```

---
## \#424 Posted by: fedestanco Posted at: 2018-04-05T23:37:32.074Z Reads: 188

```
1 in case of short, an 80amp fuse would blow as well with your battery. So consider an higher value fuse just in case you want to upgrade your battery in the future
2 the less connections you put in the way the better 
3dont know if they are implemented yet. BTW you can uninstall the cables you dont need in the molex harness by using a needle.
```

---
## \#425 Posted by: evoheyax Posted at: 2018-04-06T00:08:46.117Z Reads: 189

```
@fedestanco I need to get one going. Might just grab one of those pcbs and assemble one myself. Is it doable with a solder iron?

@JTAG ever thought of  combining this with 2 or 4 vescs to create a complete electric unit? Been wanting this forever, but haven’t had the money to get an EE to do it for me. I know the day I finally do, 3 others will do the same but until then, nobody seems to want to touch this idea. In my mind, only way to ensure reliability with a hardwired canbus built into the pcb.
```

---
## \#426 Posted by: fedestanco Posted at: 2018-04-06T00:18:59.761Z Reads: 195

```
[quote="evoheyax, post:425, topic:20947"]
ever thought of  combining this with 2 or 4 vescs to create a complete electric unit?
[/quote]

Since altium revealed to be easier than expected I might do it when I finish the esams. I have the 6.4 vesc ready for prototyping so at this point it would only be a copy paste job.

spoiler:![vesc6|690x492](upload://7YnOHf0ST8HzrlooRahKmdd69Er.PNG)
PS @JTAG I am forcing the solder mask over the though hole pads one by one. Is there a command to "pcb filter" all of them at once?
```

---
## \#427 Posted by: JTAG Posted at: 2018-04-06T00:45:19.842Z Reads: 189

```
There are a few! But the fastest / easiest one is by utilizing the "PCB Inspector" (a window you can enable from the view menu). Select the area with the object you would like to change a property of, in the PCB inspector menu tell to only show for example vias, then select tented top and bottom.

PCB Inspector is a crazy powerful tool, I can't imagine why it is hidden by default.
```

---
## \#428 Posted by: Brad Posted at: 2018-04-06T01:31:01.352Z Reads: 187

```
Two vesc and BMS in one would be awesome, but what do you do if one of the vesc is faulty or whatever?

That is one of the advantages of modulation unless it is somehow attachable and removeable on one PCB? (click/pop into and out of place)
```

---
## \#429 Posted by: evoheyax Posted at: 2018-04-06T14:30:41.095Z Reads: 179

```
The same thing you do when your vescs break now... send it to the wizard 😉

I just can’t see any other way to get size and possibly, cost, down.

This I how the laptop industry has moved for example. 5 years ago, everything was connected via a port: gpu, cpu, ram, hard dive, WiFi card, Bluetooth card. And today, on a Mac, it’s a single board. And even other brands are soldering the cpu and gpu. At the end of the day, it saved space and allowed them to fit more in less.

4 vescs  + bms is a lot to fit in a board. If we could bring the size down, then it’s way more plausible.
```

---
## \#430 Posted by: Brad Posted at: 2018-04-06T15:05:04.270Z Reads: 178

```
I see what you are saying, but just sending to the wizard would put the board out of action, whereas with modulation, just replace the one bad VESC.

When reliability and duration increases to last thousands of miles before something goes wrong is when I would buy one of those all in one item in a heartbeat. Unfortunately I do not think we are there yet.

However, if you do get around to building a beta version, I will be happy to buy one off you and give it a good run!
```

---
## \#431 Posted by: evoheyax Posted at: 2018-04-06T15:39:28.595Z Reads: 180

```
I see where your coming from. But if you have 2 or more boards, less of an issue :grin:

[quote="Brad, post:430, topic:20947"]
Unfortunately I do not think we are there yet.
[/quote]

Chaka had that kind of consistency...

I've been riding with 4x chaka 4.12 vescs and hummies hubs (v1, v3 and soon to be v4) for the past 2 years with zero issues. I think belt drives, due to the erpm, are what break the 4.12 vescs, along with the lack of upgrades and fake components most use. I'm convinced that with good components, good assembly and the upgrades chaka posted, paired with hummie hubs, will last.
```

---
## \#432 Posted by: fedestanco Posted at: 2018-04-06T21:27:51.590Z Reads: 178

```
Ok now thats my favourite tool along with smart paste. Thanks!
```

---
## \#433 Posted by: oyta Posted at: 2018-04-08T09:16:05.712Z Reads: 181

```
Thanks for your reply. What is the order of connecting the wires?

1. Power, Display, Fuse, Common-, Load+, Charge+
2. Pack-
3. Pack+
4. Balance wires (molex)

Then after everything is connected I will connect to the BMS with USB and VESC Tool to see if the config is correct and potentially adjust the parameters to my needs.
```

---
## \#434 Posted by: chinzw Posted at: 2018-04-09T19:52:15.909Z Reads: 178

```
I've connected them in any order without issues.
```

---
## \#435 Posted by: JTAG Posted at: 2018-04-09T20:25:10.983Z Reads: 180

```
Order of connection does not really matter, I do however prefer to have either the Pack- or the balance wires (which contains the pack- but than the low current variant) connected first, but this is just a feeling thing, I have no hard reasons why :roll_eyes: (do I sound like a woman yet?).
```

---
## \#436 Posted by: PatRocks Posted at: 2018-04-09T21:30:27.404Z Reads: 183

```
Lol, a nice fat one😂
```

---
## \#437 Posted by: oyta Posted at: 2018-04-11T22:10:57.936Z Reads: 185

```
![IMG_1186|666x500](upload://o54Nm4NVSweQmhneM7Tp1odVWde.JPG)
Jippi! There is light!

But..
![11|690x167](upload://8MrYPc71PvA2UVKndr1amhH5yT3.png)
I cannot find the USB-port in the VESC Tool. I use version 0.82 on MacOs. Does anyone have experience with this on a Mac?
```

---
## \#438 Posted by: lock Posted at: 2018-04-11T23:30:26.195Z Reads: 176

```
You probably need to grab the USB drivers from [here](https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers). Had the same issue on Windows and Mac.
```

---
## \#439 Posted by: oyta Posted at: 2018-04-12T08:00:25.996Z Reads: 172

```
[quote="chinzw, post:328, topic:20947"]
Does anyone have a copy of vest tool 0.82? That’s the version we need to connect to the bms.
[/quote]
Just curious - is this still valid? I couldn’t find any other references to this. The latest version would also work?
```

---
## \#440 Posted by: lock Posted at: 2018-04-12T08:26:07.211Z Reads: 170

```
*Yes.* The VESC Tool asks a connected VESC for its firmware version, each version of the VESC Tool only supports a subset of all firmwares. If the VESC Tool detects a version that it doesn't support it will limit capability to firmware upgrades only. It won't allow you to send terminal commands as required to setup the DieBieMS.

It just so happens the current DieBieMS firmware reports itself as a VESC with a firmware version (cant remember FW version) that is supported by the VESC Tool v0.82.
```

---
## \#441 Posted by: fedestanco Posted at: 2018-04-12T09:00:55.507Z Reads: 168

```
If you give me few days to finish off my exams I can email it to you.
```

---
## \#442 Posted by: oyta Posted at: 2018-04-12T09:06:31.001Z Reads: 165

```
@lock thank you very much for the explanation. I understand!

@fedestanco would be perfect if you could provide the Linux version 😃
```

---
## \#443 Posted by: Gromok Posted at: 2018-04-12T11:29:14.979Z Reads: 169

```
These little connectors for power and led on the BMS, are these JST SH 1mm or JST GH 1.25mm? These appears a bit smaller than the hall sensor plugs on my motor.

Not complaining but it would be nice if it was JST PH 2mm to match the VESC 6.0.
```

---
## \#444 Posted by: chinzw Posted at: 2018-04-12T15:45:51.019Z Reads: 160

```
I can email you the windows version if it helps
```

---
## \#445 Posted by: oyta Posted at: 2018-04-12T17:44:14.032Z Reads: 174

```
> ---   BMS Configuration   ---
NoOfCells                  : 10
batteryCapacity            : 9.00Ah
cellHardUnderVoltage       : 2.300V
cellHardOverVoltage        : 4.400V
cellSoftUnderVoltage       : 2.500V
cellSoftOverVoltage        : 4.100V
cellBalanceStart           : 3.800V
cellBalanceDiffThreshold   : 0.010V
CAN ID                     : 10
--- End BMS Configuration ---
 
> -----Battery Pack Status-----
Pack voltage          : 39.31V
Pack current          : 0.01A
State of charge       : 0.1%
Remaining capacity    : 0.01Ah
Operational state     : External (USB or CAN)
Load voltage          : 0.00V
Cell voltage high     : 3.950V
Cell voltage low      : 3.934V
Cell voltage average  : 3.943V
Cell voltage mismatch : 0.015V
Discharge enabled     : False
Charge enabled        : False
---End Battery Pack Status---

Thanks to @chinzw and a borrowed windows computer  I got connected! Some questions though.
1. It says "State of charge" 0.01% when then pack voltage is at 39.31V. It seems wrong comparing screenshots from JTAG.
2. I connected my charger which serves 41.7V but the status says "Charge enable: False". I read that @JTAG recommended was it 3-5 V above the full charge voltage you wanted. In my case I set the Soft Over Voltage to 41, then maybe I should have had a charge serving around 45V?
3. Any recommendations for a new charger? :grimacing:
3. Does it say "Charge enabled: False" because it does not sense that the charger is connected when the battery voltage is at 39.31V? 
4. Does it do balancing only when "Charge enable: True"?
```

---
## \#446 Posted by: oyta Posted at: 2018-04-12T17:49:45.544Z Reads: 168

```
Quick reply to myself. I was in config mode as I had connected the USB first. Setting the charging first, then the USB it went in the charge mode. "State of charge: 0.4%" seems odd though? 

Edit: State of charge changed to 100% after charging 😀
 
> -----Battery Pack Status-----
Pack voltage          : 39.68V
Pack current          : 1.91A
State of charge       : 0.4%
Remaining capacity    : 0.04Ah
Operational state     : Charging
Load voltage          : 0.00V
Cell voltage high     : 3.986V
Cell voltage low      : 3.972V
Cell voltage average  : 3.980V
Cell voltage mismatch : 0.014V
Discharge enabled     : False
Charge enabled        : True
---End Battery Pack Status---
```

---
## \#447 Posted by: fedestanco Posted at: 2018-04-13T10:48:21.764Z Reads: 159

```
Suggestions are always welcome. PH2.0 take up more space and PH1.25 cable are dirty cheap. In fact I sent 3 of them with each bms so any user should not have to buy more. Haven't you received them?
```

---
## \#448 Posted by: Gromok Posted at: 2018-04-13T12:34:55.762Z Reads: 159

```
No, just the [Molex](https://www.molex.com/molex/products/datasheet.jsp?part=active/0430251600_CRIMP_HOUSINGS.xml). No JST-GH 1.25mm cables or connectors came with it. PH is 2.0mm.

At least I know what size to buy, so I will do that now.
![Size Chart|690x238](upload://yj0PZs3dk0eLbFYMXv5ydOpIt2U.jpg)
```

---
## \#449 Posted by: fedestanco Posted at: 2018-04-13T12:42:23.087Z Reads: 149

```
I am very sorry. I thought everybody received them. I'll be ordering some some for you also when the next batch comes.
```

---
## \#450 Posted by: Gromok Posted at: 2018-04-13T12:44:30.029Z Reads: 153

```
@fedestanco, Well damn, you were right. I went back to have a look through the drawer to see if I can find said wires and connectors amongst the parts and behold, I found three of it. 

Friendly design feedback incoming...

If you are doing next batch, could you move the balance molex connector over in between the + and - battery terminals instead of leaving it on the side? 

That would be a more natural position due to the location of the battery.
```

---
## \#451 Posted by: DeathCookies Posted at: 2018-04-13T12:44:35.673Z Reads: 150

```
Next batch? Are you going for another run? I would love if you could sell another one or two
```

---
## \#452 Posted by: fedestanco Posted at: 2018-04-13T12:45:35.475Z Reads: 152

```
Yes, there will be a new thread with a new google form in the next hours.
```

---
## \#453 Posted by: Olloxan Posted at: 2018-04-13T13:13:36.515Z Reads: 157

```
@fedestanco
That sounds great! I´ve been waiting for this comment of yours since the beginning of this year :sweat_smile:. could you post in this thread when you open up the new thread with the google form since i get an Email notification with every new post in this thread? I definately don´t want to miss out on the new batch :slight_smile: 
Great work :+1:
```

---
## \#454 Posted by: chocol4te Posted at: 2018-04-14T11:02:04.552Z Reads: 156

```
I bought one of the leftover unpopulated PCBs, I don’t suppose you could PM me that BOM? Thanks :slight_smile:
```

---
## \#455 Posted by: lock Posted at: 2018-04-14T12:34:33.843Z Reads: 154

```
You can grab it straight from [jtag's GitHub repo](https://github.com/DieBieEngineering/DieBieMS/blob/master/Project%20Outputs%20for%20DB10005_DieBieMS/BOM/Bill%20of%20Materials-DB10005_DieBieMS(Production).csv).
```

---
## \#456 Posted by: chocol4te Posted at: 2018-04-14T12:51:33.077Z Reads: 165

```
Thanks! fedestanco mentioned changes to the BOM, were this just functional identical alternatives to mange cost or improvements?
```

---
## \#457 Posted by: fedestanco Posted at: 2018-04-14T12:53:23.573Z Reads: 155

```
They are still to be completed. Obviously any change will be made public.
```

---
## \#458 Posted by: JTAG Posted at: 2018-04-15T23:03:22.352Z Reads: 156

```
Sorry for missing your questions, I had a crazy week :frowning: , I'll reply tomorrow!
```

---
## \#459 Posted by: JTAG Posted at: 2018-04-16T20:36:33.114Z Reads: 167

```
1, State of charge is currently only accumulated charge counted in current (coulomb counting). Once the BMS finds that the battery is charged (when all cells are at the soft high limit and the mismatch is between the mismatch threshold ) the state of charge is set to 100% (jumps to this value), from then on its is just normal use and the state of charge will give an indication.

Indeed when combining all measurements of current and cell voltages a way better approximation of state of charge can be given. If someone has time to look at state of charge calculation / estimation please inform me about the possibilities :grimacing:. I am currently working on adding functionallity like CAN and UI, I could use some help with the SoC calculation :innocent:.

2, yes for the BMS to auto detect a charger the open clamp voltage of the charger when no load should be about 3V higher than the pack (max pack (number of cells in series * cellSoftOverVoltage)) voltage. The BMS could work without this higher voltage but it then just wont auto detect the charger, this is however not yet implemented in the firmware, it is on my (long :disappointed_relieved:) todo list, but I just did not reached it yet.

3, YES led power supplies! Look for the ones with configurable current / voltage, they are affordable and easy to source. 

4, yes most likely, normally in any mode of operation (also the disabled / off mode) the bms wil turn on and when the cell voltages are below cellSoftOverVoltage the Charge enable will go to True, when Charge enable: True and charge desired are true the charger port is connected to the battery and the battery will be charged.

5, yes balancing only happens during charging, in my opinion this is the only mode where dissipation of energy can be justified (but I am open to eye openers :stuck_out_tongue: ).
```

---
## \#460 Posted by: Brad Posted at: 2018-04-25T12:28:30.593Z Reads: 162

```
I assume the switch port on the board is 5volts? Just not sure what volt rated momentary switch I need to buy....
```

---
## \#461 Posted by: JTAG Posted at: 2018-04-25T13:38:28.196Z Reads: 170

```
The power button input I assume u mean? The max voltage on that port is about 16V, when the BMS is on the max voltage is 3.3V. So any mechanical momentary switch that allows >16V is OK, and almost all if not all switches should support that.
```

---
## \#462 Posted by: Brad Posted at: 2018-05-09T04:33:56.561Z Reads: 175

```
I’m ready to test the BMS in the next couple of days.

I’m starting to understand why people make a new thread when the original gets too long as I have to trawl and try to find what software was being use to view battery charge balances like the picture where JTAG did the first charging test.

Will have another look again to see if I can find it or some one tell me what app it is.

Long overdue to start testing but better late than never :)

I see it is battery stack monitor LTC6803-2, but still do not understand as I tried to google it and got hardware stuff.(probably hardware but I have to assume that is already on the BMS and I just need to find the right software for image below)
![image|690x376](upload://kWPML2vNNSGcGqdYb7h2lwsoLPD.png)

EDIT: Wrong thread, was meant for the original thread, but will leave this here in case someone might be able to answer
```

---
## \#463 Posted by: JTAG Posted at: 2018-05-09T08:56:47.836Z Reads: 165

```
It is called "STMStudio", it is a tool from ST to visualise static variables in a microcontroller during runtime (in an non intrusive way) with help of a ST-link debugger. STMStudio knows the names and where to find them in memory bij the DieBieMS.axf file.

Example project files for stm studio with the most usefull values visualised:
https://github.com/DieBieEngineering/DieBieMS-Firmware/tree/master/STMStudio

But for normal use hopefully soon this all will become long gone history when the DieBieMSTool is ready :grimacing::innocent:.
```

---
## \#464 Posted by: Brad Posted at: 2018-05-10T12:00:32.975Z Reads: 167

```
I download the software, was told to download java runtime environment, but still telling me to download it. I guess it cannot work with the latest java which is 8 I believe.

Also do not have a ST-link. I think I will just have to leave that off till you get the DieBieMSTool done :smile:

Will just make do with information through the VESC.
```

---
## \#465 Posted by: JTAG Posted at: 2018-05-10T22:36:17.299Z Reads: 170

```
![200|274x200](upload://sF0TVIecnob6Vc9ankpmT5tDBZb.gif)
```

---
## \#466 Posted by: Brad Posted at: 2018-05-12T13:38:15.287Z Reads: 176

```
Alright, Just one little niggle.

I have this guide for the buttons for the BMS. Easy enough to read. 

GND(-) and PushButton(+) for switching the BMS on and off (nothing to do with powering up the LED light). 

The 3v(+) and LED Smart(-) is for turning the led light on and off (nothing to do with turning the BMS on/off).

2nd GND not to be connected with anything.
![diebiebms_wiring|690x339](upload://g1MozQD3E7qqwo5egVSjSyPHBRq.jpg)

However most guides for momentary button is as below
![_SL1200_|690x360](upload://9SbLmrATYpNkbreaeBqQTKK8A3P.jpg)

So I would assume that GND(-) goes to "-" and PushBotton(+) goes to "C" and the 3V(+ for LED light) will go to "NO" and then connect "NO" to "+" meaning no LED Smart(-) connection at all which does not make sense as there needs to be power circulation. 

Cannot stop thinking that 3V(+) goes to "+" and LED Smart(-) goes to "NO" which should have the same effect as it goes to accessory which is BMS which also happens to be power as well....Need help here please?
```

---
## \#467 Posted by: lock Posted at: 2018-05-13T02:36:38.228Z Reads: 169

```
Was hoping someone else might provide some independent validation on this... I drew up that diagram. FWIW that’s how mine is wired up and it all works fine.

My momentary switch only has 4 contacts, so this reduced the complexity a little. I’m not sure how common what you’ve posted is for _momentary_ switches. They’re usually push to make contact, sometimes push to break contact.

In the case of the DieBieMS the switching capability and the LED should be kept separate. The LED only comes on briefly when you turn it on, and it flashes when charging. It actually turns itself on when you plug it up to a charger (no need to press switch). It flashes a little differently when fully charged. The BMS wouldn’t be able to do any of this if you started wiring the switch and LED together.

The other diagram you’ve posted seems to introduce some smarts to keep the LED lit. We don’t need those smarts as the BMS is smarter 😉. Also I have a theory that other diagram is for _non_-momentary switch types.

Hopefully this has helped and not just confused matters more.
```

---
## \#468 Posted by: Brad Posted at: 2018-05-13T05:21:44.410Z Reads: 176

```
My switch is a momentary switch, not a latch switch.

My terminals below.

![image|521x500](upload://eOW15NEV9Ln0BcecBuv2CWAgRTT.jpeg)

So what terminal did you put the “3V” onto? No GND for it?

That is the kind of info I was trying to find out. Already knew that switch and LED is separate.

Having more terminals should not change anything, it just means I leave the extra terminals disconnected.

So what you did was put switch to “C” and “-“ for switch GND and then 3V to “+” and LED GND to “NC”? See what I need to understand?

If this still cannot be solved, I have a simple + and- two terminal switch I can make do for now.
```

---
## \#469 Posted by: lock Posted at: 2018-05-13T05:47:47.373Z Reads: 177

```
[quote="Brad, post:468, topic:20947"]
So what you did was put switch to “C” and “-“ for switch GND and then 3V to “+” and LED GND to “NC”? See what I need to understand?
[/quote]
No...

Ah sorry, you’re asking about the wiring to the switch and not the BMS. 

The C and NO (switch) need to be wired up to PushButton and Ground (BMS). Order not important as it’s just closing a circuit when pressed.

The + (switch) and 3V (BMS) need to be connected, then the - (switch) and the LED Smart (BMS). Order should be important here, but I noted my LED lit up irrespective of polarity, guessing there’s more that just a LED in that circuit.
```

---
## \#470 Posted by: Brad Posted at: 2018-05-13T06:53:30.506Z Reads: 176

```
Thank you very much, just what I needed :ok_hand:

Edited Image for anyone who might need guidance.

![JTAG BMS Switch Wiring|690x339](upload://nPjUgB8kzoEh36WuhxFIYVpK4a7.jpg)
```

---
## \#471 Posted by: JTAG Posted at: 2018-05-13T14:16:00.542Z Reads: 168

```
The LED should be between GND and LED Smart. When doing it as described the led indication will be inverted :stuck_out_tongue:. That is not problem but you wont be able to tel that the board is on by the LED. 

When the led is connected between GND and LEDSmart the LED will turn on when the BMS is on, blink during charging and will show a pattern of long off and short on when charged.

Display is correct! RST is not used (it is used as an IO on the high amp shield to enable the DC DC converter but that is of no use in skateboard applications).
```

---
## \#472 Posted by: lock Posted at: 2018-05-14T00:16:46.468Z Reads: 168

```
[quote="JTAG, post:471, topic:20947"]
The LED should be between GND and LED Smart. When doing it as described the _led indication will be inverted_ :stuck_out_tongue:. That is not problem but you wont be able to tel that the board is on by the LED.
[/quote]

That's exactly what it does :joy:. I even get long on, short off when it's changed.

When working out the connections I had the PushButton and GND figured out. That left the other GND, LED Smart and  3V. It was either 3V and LED Smart, or LED Smart and GND. 50/50 chance, and I got it wrong... I've never been the gambling type.
```

---
## \#473 Posted by: banjaxxed Posted at: 2018-05-23T13:08:43.447Z Reads: 160

```
**Edit:** Vesc tool 0.82 linked by @fedestancoworksand I can connect to the DieBieMS,this is maybe a blip, will try 0.92 against a vesc again. Reinstalled those linked drivers.

**Edit II:** Weirdness, vesc tool 0.92 now works on the VESCs again, also @lock's nice monitoring python scripts, seems like I have a problem with pack1, either this battery is goosed or I I need to recheck BMs leads
![image|690x81](upload://jC6Qt36YeGGbGMVBJAL0WJFPaVT.png)
```

---
## \#474 Posted by: lock Posted at: 2018-05-24T00:21:51.135Z Reads: 161

```
Cool. I'm glad someone else used it before jtag comes along and supersedes it with his DieBieMS-Tool 😂. I'd double check those numbers against what you get from the VESC Tool, but I fail to see how the code would be broken in a way that returns numbers just a little bit 'off'. Doesn't look great for the pack :slightly_frowning_face:

FWIW I have weirdness connecting to the VESC-Tool. The DieBieMS has always been fine, as has one of my VESCs. But the other VESC ('Official' v6 no less) requires power cycling, rebooting laptop, etc. Never quite found what the right combination was, but never failed to get it to connect.
```

---
## \#475 Posted by: banjaxxed Posted at: 2018-05-24T01:21:24.448Z Reads: 166

```
The pack is a NESE type, I'll pull the cells out of the offending parallel units and inspect each cell individually, thanks for the thoughts on it.

Looking forward to the diebie vesc too too, the preview looks really nice.

Here are my original readings,very strange massive flutuations from the readings of cell pack 0/pack1 I am targetting. I've pulled apart pack 0 and placed 2 cells in a usb charger, they are reading at 3.6+ and look normal to me

![image|690x322](upload://xRr39u0D3h0d5KlnlGYXlZV3SCK.png)
```

---
## \#476 Posted by: lock Posted at: 2018-05-24T09:03:05.272Z Reads: 168

```
[quote="banjaxxed, post:475, topic:20947"]
Here are my original readings,very strange massive flutuations
[/quote]

Looks like you may be getting [this bug](https://github.com/DieBieEngineering/DieBieMS-Firmware/issues/1) in the data. Those fluctuations probably aren't happening. Still the issue that some cell groups are way off the others. It may be that "cell voltage 0" is the last cell group not the first, or something like that.

You shouldn't have to pull apart the cells out of the NESE module. I'd either measure them with a multimeter at the balance connector, or the +/- of each NESE module.

If you test at the balance connected I'd recommend keeping the - probe on the negative terminal of the battery; you probably don't want to accidentally touch the two multimeter probes together while measuring voltage.
```

---
## \#477 Posted by: banjaxxed Posted at: 2018-05-25T01:05:48.102Z Reads: 167

```
Thanks @lock that bug looks promising.

It's so easy to jankout cells that I think the best way for me to address this is to charge them all up to a standard value.

Edit: seems to have worked I pulls the cells from the first two packs & although lost usb connectivity to confirm, it's powering on and the charger gave a good whack of juice(fan).
```

---
## \#478 Posted by: Eboostin Posted at: 2018-05-31T04:59:25.886Z Reads: 170

```
Anyone got an extra they'd like to sell?
```

---
## \#479 Posted by: fedestanco Posted at: 2018-06-02T14:55:50.080Z Reads: 180

```
Hi guys,
the exams will end 27th of july, but there is good news if you want to get one bms:
this guy is willing to sell a few and the quality looks very good.

https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/279?u=fedestanco

I dont know him but he claims to own a tech company and judjing from the pics he knows what he's doing. 
If you planned to get on this GB I would suggest to go with him instead PAYING WITH PAYPAL SERVICES to be safe.
```

---
## \#480 Posted by: Samau18 Posted at: 2018-06-02T15:10:37.570Z Reads: 189

```
Thanks for the referral!  Good luck with your exams!

Sam
```

---
## \#481 Posted by: andi91 Posted at: 2018-10-08T18:20:26.134Z Reads: 126

```
Hey Guys!

We want to build the DieBieMS.
We are looking at the last BOM. (6 months old)
Now there are many things not in stock.
Maybe someone in this forum have an updated BOM, before we are also start looking for it? ;)

thanks
regards
Andreas
```

---
## \#482 Posted by: Klaerke91 Posted at: 2018-10-08T19:34:35.227Z Reads: 122

```
look here - https://www.electric-skateboard.builders/t/diebiems-v0-8-batch-3/65313/88
```

---
## \#483 Posted by: JTAG Posted at: 2018-10-08T22:53:39.839Z Reads: 117

```
Yes the bom stayed the same for quite a while, only some minor mechanical changes where made really the last couple of months. 

Only the main components should stay the same, especially look for the correct micro controller and LTC.
```

---
