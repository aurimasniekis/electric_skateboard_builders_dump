# HW6.4 based ESC - B-box

### Replies: 369 Views: 14926

## \#1 Posted by: bimmer Posted at: 2018-01-22T20:52:14.115Z Reads: 641

```
So whats the legal situation on making these are they open source or not?

I did  some research/math and for 500 of them the costs are for BOM 27000$, assembly 3000$, PCB 2500$, Aluminum Case $4000 Wires and connectors $2500.
All in all about 39000$ about 78$ per controller.
While I would have to talk to my wife before taking such a large amount out of savings the return seems rather quick and plentiful.
Considering most Direktfets are sold out until the middle of the year I  doubt  all those focboxes people ordered will ship soon...and the Bom for 500 is in my cart waiting 100% stocked.
E-teknet in AZ say they can have them done in 10 days after receiving all parts.
And 3d hubs can have the housings  done and shipped next week.

Lets say I would sell these at  a moderate 130$ + tax(5.6%)=137$ I am pretty sure they'd sell out in a month.

Cheaper than a Focbox and made in the USA.

To gather for People not wanting to weed through the whole thing.

I am making 50 Hw6.4 clones designed by @stewii, they will come with a Cover PCB a plastic body and an Aluminum Heat sink.
I am in the phase of the project where all parts are ordered.
```

---
## \#2 Posted by: SORRENTINO Posted at: 2018-01-22T20:59:10.610Z Reads: 587

```
@Deckoz @pshaw
```

---
## \#3 Posted by: Sender Posted at: 2018-01-22T21:04:58.716Z Reads: 592

```
You know, the math sounds good. My concern is when for what ever reason there is an issue during the process and your left with 500 paper weights that need more investment to get them to a reliable and more importantly, sellable state.  Not that this would happen, but it could.  And asking the wife for more out of our savings to fix something like that seems... dangerous? 

But on another note, freaking do it, I'll buy some.
```

---
## \#4 Posted by: JLabs Posted at: 2018-01-22T21:05:51.394Z Reads: 576

```
[quote="bimmer, post:1, topic:44375"]
While I would have to talk to my wife
[/quote]

Why would you have to do that? You make it seem like your going to spend $40k or something
```

---
## \#5 Posted by: bimmer Posted at: 2018-01-22T21:08:44.056Z Reads: 553

```
I am less concerned that the Controllers won't work and more with being sued by trampa :smiley:
```

---
## \#6 Posted by: dragopepper Posted at: 2018-01-22T21:10:14.835Z Reads: 543

```
Whats about the reject goods as output while the esamply from the stuff? Maybe you should also add some buffer in your calculation.
```

---
## \#7 Posted by: bimmer Posted at: 2018-01-22T21:10:34.932Z Reads: 536

```
She'll let me buy another BMW before she'd let me make an investment in "skateboards we don't need"
```

---
## \#8 Posted by: ThermalM16 Posted at: 2018-01-22T21:10:35.817Z Reads: 532

```
I would start with 50 or less to make sure everything is sound, give them a few months, see if they hold up or if you have complaints coming in from customers. If all is well place your order for 500 and you'll already have made about $2600 in the process which will offset some of that huge initial cost.
```

---
## \#9 Posted by: Sender Posted at: 2018-01-22T21:12:52.636Z Reads: 523

```
Valid concern. I'm a worried about everything when talking about that kind of investment...
```

---
## \#10 Posted by: dragopepper Posted at: 2018-01-22T21:13:27.219Z Reads: 521

```
Weeeell... i would take the bmw 😁
```

---
## \#11 Posted by: bimmer Posted at: 2018-01-22T21:19:32.952Z Reads: 513

```
The Boards seem sound so far and I will be testing them more. Considering I hand soldered them and they are running  and running in foc at 245KV  and 260KV  at 12s 3 battery charges so far everything that toasted my 4.12over and over. I will order an initial 10 from the factory and give  them to friends to test. But 500 seems to be the sweet spot between availability, risk and earning. Sadly the normal Mosfets  are  sold out so I'll have to use Automotive ones that can dissipate about 200w more heat but also cost about 33% more.
```

---
## \#12 Posted by: ThermalM16 Posted at: 2018-01-22T21:27:36.221Z Reads: 491

```
Those would probably be preferable anyway. I would buy your product over Trampa's knowing you're using better FETs, since those can cause some of the worst problems on these boards. If you have faith in your PCB manufacturer, I say go for it. I'm unsure how to deal with the rights to the design or anything, but if you're square in the legal section it's a solid idea. If you end up going through with it, let me know I'll buy some and I we can probably work out some kind pricing with you and customers if you want to refer warranty repairs and such to me!
```

---
## \#13 Posted by: scepterr Posted at: 2018-01-22T21:33:15.029Z Reads: 466

```
I'm confused are you making your own PCB or wanting to get @stewii's manufactured in bulk?
```

---
## \#14 Posted by: bimmer Posted at: 2018-01-22T21:35:16.384Z Reads: 464

```
Whatever Is easiest he already said he'd sell his to me in bulk I assumed a price that seems appropriate for that amount.
But could also have my own made.
```

---
## \#15 Posted by: Vanarian Posted at: 2018-01-22T21:38:26.741Z Reads: 466

```
I like this plan.
```

---
## \#16 Posted by: banjaxxed Posted at: 2018-01-22T21:39:14.115Z Reads: 466

```
This approach taken from a whiteboard release could have you meeting mr. Lawyer I'm wonder when vesc6 design will be officially released as much as I like your proposal I wouldn't be sinkyin life savings just yet
```

---
## \#17 Posted by: bimmer Posted at: 2018-01-22T21:41:43.753Z Reads: 464

```
My concern exactly. But life savings is a big word.
```

---
## \#18 Posted by: ATLesk8 Posted at: 2018-01-22T21:44:10.442Z Reads: 473

```
This here sounds like a great solution to the current lack of offerings
```

---
## \#19 Posted by: Vanarian Posted at: 2018-01-22T21:44:59.468Z Reads: 474

```
Depends on what you do, main problem with "VESC6 Trampa edition" is the trademark. Nothing stops you from taking the schematics, making your PCB by yourself, having it full blown compatible with VESC-Tool without mods. As long as either you pay for trademark and call it VESC 6 with Ben's approval, or you name it differently and state "based on..." or "compatible with..." 

This way you're out of pursuit boundaries cause it still originates from an open-source project and not a patented closed project.

BTW, as @stewii has proven, you don't need the reference design to get a quality piece of hardware made. A wonrg turn somewhere was taken in the course of VESC, and I believe people like stewii and you, and even Jason with FOCBOX will take it back to the right path. 

You guys just need to make things fair for the people who will buy your stuff.
```

---
## \#20 Posted by: bimmer Posted at: 2018-01-22T21:46:35.086Z Reads: 449

```
I honestly  don't think its that cut and dry if I did  I would have a 27k mouser order on its way... lol
```

---
## \#22 Posted by: Vanarian Posted at: 2018-01-22T21:48:28.977Z Reads: 433

```
You're right to check and I don't even know where you're living, laws vary but the core logic of most contracts remains the same no matter where you live. 

That's a basic info to be able to check and get accurate backup depending on your country's system.
```

---
## \#23 Posted by: bimmer Posted at: 2018-01-22T21:49:16.182Z Reads: 428

```
Uhm who said no case? Let me add on to that before you start saying no way how about you do some research? I am not asking if you or  the community think the price is possible because that doesn't even matter. This is about if I can legally continue.
```

---
## \#24 Posted by: ThermalM16 Posted at: 2018-01-22T21:54:32.872Z Reads: 426

```
Buying 500 of most electronic components gets you about 40-50% off so it's doable.
```

---
## \#25 Posted by: Deckoz Posted at: 2018-01-22T21:57:08.847Z Reads: 416

```
Good luck..
```

---
## \#26 Posted by: bimmer Posted at: 2018-01-22T21:57:16.334Z Reads: 412

```
Most of the parts are in the more in the  1500 - 3000 ballpark.
```

---
## \#27 Posted by: jmasta Posted at: 2018-01-22T22:00:03.678Z Reads: 406

```
A reliable VESC 6 derivative under $150 would dominate the market.  Currently the VESC 6 is almost $350 shipped from Trampa, which is probably double what most people are willing to pay
```

---
## \#28 Posted by: koralle Posted at: 2018-01-22T22:01:38.557Z Reads: 415

```
So Jason had this to say about manufacturing Vescs in the US
[quote="onloop, post:250, topic:19089"]
we are now manufacturing in a new Shenzen factory that specializes in Tablet & Phone PCBA. Failures rates near ZERO! & Much faster production!
[/quote]

[quote="onloop, post:250, topic:19089"]
Our previous factory in the US had 18% failure rates in the last batch. Our last order was 1000 units & only approx 800 passed our QC process.
[/quote]

[quote="onloop, post:250, topic:19089"]
To our suprise, We discovered they swapped some capacitors to upgraded versions not available from USA sources! we complained originally (because normally swapping means bad) However, after testing with very high-end lab equipment, we realised they were higher spec than our BOM.
[/quote]
```

---
## \#29 Posted by: bimmer Posted at: 2018-01-22T22:04:21.847Z Reads: 417

```
Just take a seat if you're gonna make stuff up they take a day to quote you over 300 or for 7075Al
![housing|690x314](upload://d0ZeSazcFkBmHAwD9Vj65KYkI17.jpg)![housing 2|690x274](upload://2wca51AbwGNK246LmLs4x2CT5qg.jpg)
```

---
## \#31 Posted by: bimmer Posted at: 2018-01-22T22:07:30.241Z Reads: 406

```
Yes your point? Because it all seems correct to me.
```

---
## \#32 Posted by: Giga Posted at: 2018-01-22T22:11:45.214Z Reads: 403

```
Don't forget the software, 5-10% don't hurt anybody and will (hopefully) push development of 100% duty cycle. And without you wont gain nothing.
```

---
## \#33 Posted by: michichopf Posted at: 2018-01-22T22:14:36.251Z Reads: 404

```
Its difficult, a lot of effort. BUT if you pull it off, the hero of the community.
```

---
## \#34 Posted by: bimmer Posted at: 2018-01-22T22:14:45.782Z Reads: 406

```
Yes I would source the parts myself because I'd rather do the head work than the leg work.... and I live about 20 mins from the factory. I am not trying to start a get rich company I want to  offer decent controllers to people that currently cannot afford them. Even at 18% attrition I could sell those at 50% as do it yourself no warranty repairs. Or you know send them back...
```

---
## \#35 Posted by: bimmer Posted at: 2018-01-22T22:15:56.245Z Reads: 398

```
I was absolutely intending on giving proper gratuity to the sources.
```

---
## \#36 Posted by: Kug3lis Posted at: 2018-01-22T22:22:47.044Z Reads: 400

```
To cnc 500 units it will not be done in a week for sure in case you run a house with tenths of machines ;)
```

---
## \#40 Posted by: Kug3lis Posted at: 2018-01-22T22:28:42.013Z Reads: 393

```
Plus not a single company will do 500 units, its not efficient they will suggest to go with casting and finishing ;)
```

---
## \#42 Posted by: koralle Posted at: 2018-01-22T22:30:04.275Z Reads: 391

```
Then teach him instead of mocking!
```

---
## \#43 Posted by: mmaner Posted at: 2018-01-22T22:31:17.800Z Reads: 397

```
[quote="Sender, post:3, topic:44375"]
And asking the wife for more out of our savings to fix something like that seems… dangerous?

But on another note, freaking do it, I’ll buy some.
[/quote]

Your definitely from the south...  Hey y'all, watch this shit! :slight_smile:
```

---
## \#45 Posted by: Surfer Posted at: 2018-01-22T22:32:35.630Z Reads: 390

```
Oh yeah I love telenovelas!!
```

---
## \#47 Posted by: Kug3lis Posted at: 2018-01-22T22:33:36.229Z Reads: 393

```
On another topic I would like to see 1000km on that pcb first than do massive manufacture.
```

---
## \#48 Posted by: scrapheap Posted at: 2018-01-22T22:36:28.284Z Reads: 405

```
This is starting to get off-topic.

Frankly, and most of us here will attest to, that the ASSUMED cost of making/building something rarely equals the REAL cost.

You will probably have some legal hurdles. Just do as much research as possible, talk to BV, and remember...most of the legal problems will start if 'VESC6' is anywhere IN the name.
```

---
## \#49 Posted by: Bensaida Posted at: 2018-01-22T22:36:57.972Z Reads: 390

```
VESC7?


10ch
```

---
## \#50 Posted by: Vanarian Posted at: 2018-01-22T22:38:38.366Z Reads: 385

```
M-ESC, how about that
```

---
## \#52 Posted by: Bensaida Posted at: 2018-01-22T22:40:16.625Z Reads: 382

```
VeSc6


10ch
```

---
## \#53 Posted by: Giga Posted at: 2018-01-22T22:40:55.883Z Reads: 380

```
6CSEV?

10Ch
```

---
## \#54 Posted by: Sebike Posted at: 2018-01-22T22:42:23.282Z Reads: 383

```
https://scontent.cdninstagram.com/t51.2885-15/s320x320/sh0.08/e35/c135.0.810.810/25024151_426322311104271_4654613967442804736_n.jpg
```

---
## \#55 Posted by: Vanarian Posted at: 2018-01-22T22:42:29.416Z Reads: 380

```
Where is even the ESC in that lol
```

---
## \#56 Posted by: Deckoz Posted at: 2018-01-22T22:42:58.706Z Reads: 381

```
It's backwards...
```

---
## \#57 Posted by: Vanarian Posted at: 2018-01-22T22:43:37.494Z Reads: 387

```
Dumb me, thanks for showing it
```

---
## \#58 Posted by: Mobutusan Posted at: 2018-01-22T22:43:42.011Z Reads: 384

```
VESCalator VI
```

---
## \#59 Posted by: Sebike Posted at: 2018-01-22T22:45:01.817Z Reads: 384

```
Name it FrESC and even Frank will be happy!
```

---
## \#60 Posted by: Bensaida Posted at: 2018-01-22T22:45:47.306Z Reads: 380

```
@trampa can i name my shampoo-brand VESC6?
```

---
## \#61 Posted by: JohnnyMeduse Posted at: 2018-01-22T22:48:51.753Z Reads: 379

```
Hi, 

@bimmer, before you go any further, I highly suggest you to contact those factory to see exactly the work they will do for you. They could also guide you through the hole process. Because you can’t just get a quotation from there website, it is never really representative of the reality. I was reading your quotation and some of these number seemed off, and other important part are missing. 

Also, Time wise it isn’t really adding up, I can tell you from experience a project like this is can easily take 3-4 month (not 10 days), and you probably have to invest 150-200hours of tour own time (just for the production, I’m not talking about supporting your product)

As for your question « Is it worth the risk? » it is up to you, If you’re ready to take the risk, why not, but it is far from being a easy project, specially if you have no experience.
```

---
## \#62 Posted by: Deckoz Posted at: 2018-01-22T22:50:39.998Z Reads: 370

```
Anyway.. the extra parts.. the extra cost... No 100% duty... I've got four sitting here... They're no better then the focbox to me as it stands...

I'm sure people will buy it. But I sure hope you know what to do when people don't... Or there's failures.
```

---
## \#63 Posted by: Surfer Posted at: 2018-01-22T22:53:18.833Z Reads: 359

```
Mind you to explain a bit this? No 100% duty, do you mean duty cycle? I didn't read anything about it, please.
```

---
## \#64 Posted by: bimmer Posted at: 2018-01-22T22:59:08.187Z Reads: 364

```
So  none of this is set in stone and the prices were more to get your attention. This thread is more about is it legal or not... My knowledge about manufacturing is not up for debate especially not based of of what I do in this forum after work... No of y'all  money is at risk I will end up with working boards or not. I will weigh my options on new designs with or without nrf and without that garstly gyro sensor. Also I will schedule an appointment with a lawyer just to be safe. The money wont hurt (me) if it fails my wife might be mad though...I will rather do my research.

Just FYI the price for the cases is agreed upon I just don't wan't to show my emails around a public forum.
Also the price for the  parts as of now is with NRF and is also not avariable.
I assume prices for the fab and  assembly may change as I have so  far only asked @stewii the price for 40 pcb's and if he would sell me his gerber files which the latter has not been responded to yet.
```

---
## \#65 Posted by: bimmer Posted at: 2018-01-22T23:03:22.968Z Reads: 361

```
I agree  with you 100% and I am thank full for any input you have. I have 6 years of experience in manufacturing aircraft parts but have never guided a whole project  from start to end. Also electronics aren't my field but I assumed something I soldered up on my kitchen counter  would be cake work for  a factory.
```

---
## \#66 Posted by: Deckoz Posted at: 2018-01-22T23:03:49.266Z Reads: 364

```
Vesc4 and below couldn't do 100% duty because of only two current sensors and the time delay between phases so it is limited to 0.95 or 95% duty in the software


The 6 schematic has 3 current sense circuits, but still cannot do 100% duty reliably. Even though the DRV supports 100% duty. That's it.
```

---
## \#67 Posted by: Surfer Posted at: 2018-01-22T23:07:18.859Z Reads: 365

```
Thanks a lot, that was a nice explanation. 👍
```

---
## \#68 Posted by: Namasaki Posted at: 2018-01-22T23:07:46.363Z Reads: 368

```
[quote="bimmer, post:5, topic:44375"]
I am less concerned that the Controllers won’t work and more with being sued by trampa :smiley:
[/quote]

Just don’t call it a Vesc
```

---
## \#69 Posted by: Bensaida Posted at: 2018-01-22T23:10:01.600Z Reads: 359

```
Bimmer ESC (BESC)
```

---
## \#70 Posted by: Namasaki Posted at: 2018-01-22T23:10:28.850Z Reads: 349

```
[quote="Deckoz, post:62, topic:44375"]
They’re no better then the focbox to me as it stands…
[/quote]
Don’t they have higher erpm limit ?
```

---
## \#71 Posted by: Deckoz Posted at: 2018-01-22T23:14:47.510Z Reads: 346

```
The higher erpm is mostly because of the speed of direct fets..it's why you can do over 100kerpm in the focbox... More then what any of us would need on esk8..
```

---
## \#72 Posted by: JohnnyMeduse Posted at: 2018-01-22T23:15:50.924Z Reads: 351

```
[quote="bimmer, post:65, topic:44375"]
Also electronics aren’t my field but I assumed something I soldered up on my kitchen counter  would be cake work for  a factory.
[/quote]

Not really... the best exemple (related to our field) is the Focbox as mentioned earlier, over 20% of failure strait from the factory, and they weren’t not event able to fix them (I know because they all ended on my desk). And they where able to find those defective, because the lead engineer from Enertion decide to put test jig in place, if he haven’t can you image how many people would have been disappointed (it would probably have been the end of Enertion).
```

---
## \#73 Posted by: JohnnyMeduse Posted at: 2018-01-22T23:16:35.129Z Reads: 337

```
Also there no Erpm limit in FOC anyway 🤪
```

---
## \#74 Posted by: Deckoz Posted at: 2018-01-22T23:17:04.018Z Reads: 340

```
And that ^
```

---
## \#75 Posted by: b264 Posted at: 2018-01-22T23:17:43.037Z Reads: 349

```
[quote="Deckoz, post:71, topic:44375"]
More then what any of us would need
[/quote]

Almost all historical failures seem to start as a "nobody would ever need that" many years earlier.  Refrain from doing this
```

---
## \#76 Posted by: Deckoz Posted at: 2018-01-22T23:21:40.920Z Reads: 351

```
I'm not doing that.. I'm simply stating..

The upside to spending the money on additional components over the 4.12 bom and having 3 current sensors would be 100% duty. But it's not... Focbox and vesc6 erpm max is basically the same. Just add more aluminum to disipate heat  I was saying apples to apples the erpm is based on the speed of directfets and how cool you run them.

Also I said never because 60v max. On a 260kv motor... On 14S is ~107kerpm... 

I know I wouldn't ever use a high kv motor on 14s...it's not practical due to saturation.

Can you say in anyway an esk8 you would hit higher then 107k? @b264

I mean let's think about it hubs are in the 10k-26k erpm range depending on kv

A mountain board that you could use the extra erpm with more reduction...  Let's take 14s as the max(if you had magura disc brakes and braking disabled on the esc) and a large reduction of 12/80 on 8" tires that's still 54mph...  On 7" 47mph. Dunno about you but mountain boards aren't for speed.. they need torque. So erpm is out the window there. Especially since you can't run a big reduction with small tires

13s 190kv... Done... that's  only about 74k erpm... And about the max voltage... And will easily do 40mph..

How many more erpms do you need?

Anything faster and I'd rather be on an analog board.
```

---
## \#77 Posted by: b264 Posted at: 2018-01-23T00:08:30.687Z Reads: 332

```
Yeah I can think of a situation where I'd need more.  I'm not going to say much about it other than think about different amounts of motor poles too...

Plus things that run more efficiently at higher RPM
```

---
## \#78 Posted by: Deckoz Posted at: 2018-01-23T00:28:53.357Z Reads: 329

```
28 poles ey? Whatcha making a stepper motor?  ...higher poles make less power at high rpm..your right more efficient but less power.

If your considering high rpm application with 28 poles and want power I'd suggest two wye motor windings and two escs on the same stator 😈
```

---
## \#79 Posted by: b264 Posted at: 2018-01-23T00:32:55.072Z Reads: 326

```
There is still a certain application that needs more.  But I don't want to reveal what I'm thinking.  All I have to say is "you're too focused on there being a motor"
```

---
## \#80 Posted by: Deckoz Posted at: 2018-01-23T00:35:43.057Z Reads: 324

```
.... The only other thing with 3 phases is a generator...which is the same thing as a  motor.. but it generates power instead of using it... 

You gonna make a windmill? ...hand crank computer power supply? Bike as a power wall charger?
```

---
## \#81 Posted by: bimmer Posted at: 2018-01-23T06:49:40.213Z Reads: 327

```
As it turns out my wife's opinion on go big or go home is not the same as mine. The family treasurer has given me permission to make 50...and wait a month to see responses. This is not a group buy I and am going in 100% self funded I'd like to gauge Interesst at 150$. No EU shipping. 
It would be. 
1 x Bimmers-foc-esc hw6.4 70mm 
awg 10 power wires xt-90/xt-60, 
awg 12 60mm 4mm bullet motor wires
1x Aluminum case 7075
1x Cover for said case
I'll have these made and will test every single one for motor detection, uart ( bluetooth) , sensors and ppm.
They will have nrf but it will be untested.
```

---
## \#82 Posted by: Clonkex Posted at: 2018-01-23T07:25:25.659Z Reads: 328

```
When you say

[quote="bimmer, post:81, topic:44375"]
No EU shipping
[/quote]

...why specifically EU?
```

---
## \#83 Posted by: chuttney1 Posted at: 2018-01-23T07:29:07.421Z Reads: 323

```
If you are making these, what is the maximum voltage you will allow under the normal condition?
```

---
## \#84 Posted by: bimmer Posted at: 2018-01-23T08:54:42.762Z Reads: 326

```
Oh short shipping and response time also lower shipping cost incase of rma. Basically this is a test and if something goes wrong 5.60$ shipping sounds better than 18$ ontop of refunding someone or replacing/fixing something.
```

---
## \#85 Posted by: linsus Posted at: 2018-01-23T08:55:05.413Z Reads: 324

```
..except for the fact that the FOC box isnt based on(last i checked) the new hardware but the old. basically 4.12 with some direct fets and makeup on. From what I know the components used arent top either..Just to clarify, I'm not saying it doesnt work. I'm sayin its two entirely different products as whole, even tho one showcases as the real deal.
```

---
## \#86 Posted by: bimmer Posted at: 2018-01-23T08:55:30.264Z Reads: 323

```
I will test 13s for a while before I say more than 12s or 50.4V.
```

---
## \#87 Posted by: koralle Posted at: 2018-01-23T09:13:26.331Z Reads: 327

```
Please consider factoring in 10$ per module as a thank you to BV who engineered this thing!
```

---
## \#88 Posted by: bimmer Posted at: 2018-01-23T09:16:10.402Z Reads: 329

```
Has always been considered.
```

---
## \#89 Posted by: Pimousse Posted at: 2018-01-23T10:02:21.844Z Reads: 332

```
BESC is a name already used :
http://bitwizard.nl/shop/BitWizard-ESC
```

---
## \#90 Posted by: bimmer Posted at: 2018-01-23T10:15:33.100Z Reads: 320

```
Consider it edited
```

---
## \#91 Posted by: TarzanHBK Posted at: 2018-01-23T10:49:55.082Z Reads: 320

```
why do we not know about this??
```

---
## \#92 Posted by: Skitch Posted at: 2018-01-23T11:08:35.169Z Reads: 327

```
Just out of curiosity, how long does it take to sell 50 ESC's?
```

---
## \#93 Posted by: Schulerbible Posted at: 2018-01-23T11:09:34.447Z Reads: 320

```
I would use Al 6060 over Al 6061 and/or 7075 due to its better thermal conductivity.
```

---
## \#94 Posted by: bimmer Posted at: 2018-01-23T11:10:27.100Z Reads: 317

```
Boards could take a while lol
```

---
## \#95 Posted by: GrecoMan Posted at: 2018-01-23T12:10:33.858Z Reads: 316

```
can ship first class international for less than $6 😉
```

---
## \#96 Posted by: ThierryGTLTS Posted at: 2018-01-23T12:23:54.887Z Reads: 316

```
Do you intend to have CE and FCC approvals/certifications like Trampa?!

It costs a lot and takes time.
```

---
## \#97 Posted by: myreala Posted at: 2018-01-23T12:54:10.159Z Reads: 314

```
Also I would suggest @bimmer  to get rid of NRF module or you'll have to get some extra certifications in US which is a huge pain in the ass. I think even Trampa sells non NRF version to US customers.
```

---
## \#98 Posted by: Ixf Posted at: 2018-01-23T13:32:56.242Z Reads: 316

```
Depending on timeline would be interested
```

---
## \#99 Posted by: Deckoz Posted at: 2018-01-23T13:42:13.519Z Reads: 327

```
Uh duh, focbox is 4.12 hardware with direct fets and two current shunts. Vesc 6 has three current shunts

Please tell me what you really think the difference is between the two. Aside from drv8301(limited fault output vs 8302(full fault readout) and the current shunts. Because they're pretty much the same... Lol

Maybe you should take a look at the schematic.. because the gyro/acclerometer and NRF addition to the vesc 6 hardware does nothing for performance...
```

---
## \#100 Posted by: linsus Posted at: 2018-01-23T14:08:45.994Z Reads: 328

```
Well, that depends what you use it for. The approach for the VESC6 isnt solely towards esk8ing but very general. The gyro and acclerometer can be used for many fun things, from a personal perspective I use the vedder nunchuck mod so I dont have to fit a cheap ass e-bay chip+antenna in there that eventually gives up, since its all integrated (which was the reasoning behind the nrf in the first place).  In regards to performance, I havnt burned my DRV on my current VESC6 yet, and I've had one prototype soldered since the very first alfa iteration about 1+year ago... so theres that. Lost count on the replaced DRV's while trying to tune the FOC on the 4.x hardware. But if you say that you dont feel any difference i applaud you.

Havn't had the opportunity to fully test 12S yet but from what i understand alot less units fail due to pushing the voltage boundries compared to 4.xx. 

Regarding the Three shunts, with only two shunts the 3d current reading is calculated instead of a live value. Which turned out to be unfavorable in many cases. But there are many applications where two shunts are enough.
```

---
## \#101 Posted by: ThermalM16 Posted at: 2018-01-23T14:16:35.318Z Reads: 324

```
Selling 6.4 HW for $130 would sell out very quickly in my opinion. I’d buy two to replace my brand new FOCBOXs with these and then just sell those. These are cheaper than FOCBOXes, better than FOCBOXes, and more accessible than FOCBOXes for all US esk8 riders. They would all sell for certain but I would assume less than a month if I had to guess.
```

---
## \#102 Posted by: longhairedboy Posted at: 2018-01-23T14:33:14.487Z Reads: 337

```
i wish everyone would stop talking about vesc legal shit here. ITs not fucking rocket surgery and its barely relevant. 

VESC 6 is open source. If you avoid the registered TRADEMARKS, you're fine. You can make them all damned day and charge whatever you want as long as you don't call it a VESC. End of legal. 

i really don't know why people find this so damn complicated. Trampa's not going to sue anybody. if the weight of their VESC 6 hoarding doesn't crush them completely, they're barely be able to afford legal anyway after they stock them all and no one buys them because they're too goddamned expensive for what they are. 

And you assholes need to stop trying to intimidate people into not doing things. I'm sick of that shit. I have a pile of PMs in my inbox that i keep and laugh at. Every one of them is a vendor, on this site, telling me what  i shouldn't get into. Fuck all of you for sending me that shit. I'm not going to name names until my book is published, and there will be a long list of "fuck you i did it anyway you sore fucking losers" credits to read through. I don't care how long you've been doing it and what issues you had. That doesn't make you some kind of special snowflake who is the only one that can do a thing. Suck it. Either provide constructive feedback or GTFO. 

@bimmer do it and i'll start buying from you if they prove reliable. If you like you can send me test units and we'll beat the crap out of them and provide plenty of feedback. I already have retail in place so i'd be happy to help you move them. I was going to try and have some made anyway for the same reasons.
```

---
## \#103 Posted by: darkkevind Posted at: 2018-01-23T14:34:58.047Z Reads: 319

```
There's nothing - legally - stopping you from creating an ESC that has the same specifications as the VESC 6, you just can't call it a VESC.

Electrical items are manufactured either identical or practically identical to other electrical items daily, there's nothing the law can do about it because those components used to make that item are freely available on the market for anyone to buy and construct. As long as you steer clear of the name VESC and ideally, come up with some differentiator between this ESC and a VESC 6, you will be fine.
Certain people won't like it, but you'll be fine, legally...
```

---
## \#104 Posted by: Sebike Posted at: 2018-01-23T17:19:45.614Z Reads: 318

```
Speaking of name stealing... VESC was a name used by Volvo for a concept car back in '72. 

Google it to see pics of a real OG old school VESC. 😁
```

---
## \#105 Posted by: banjaxxed Posted at: 2018-01-23T18:36:57.045Z Reads: 318

```
I and my lawyer look forward to your biography @longhairedboy
```

---
## \#106 Posted by: longhairedboy Posted at: 2018-01-23T19:33:31.151Z Reads: 322

```
the critics are heralding it as "an autobigraphical autobiography autobiographed by an autobiographer." 

higher praise can't even.
```

---
## \#107 Posted by: PredatorBoards Posted at: 2018-01-23T19:44:34.310Z Reads: 320

```
I say this investment is well worth. At least do a small batch to make sure something as much as an improperly sized copper pad isnt out of place.
```

---
## \#108 Posted by: JohnnyMeduse Posted at: 2018-01-23T19:45:40.581Z Reads: 325

```
Can I get an Autographed copy, by autobiographer ?
```

---
## \#109 Posted by: Kaly Posted at: 2018-01-23T19:47:02.412Z Reads: 328

```
[quote="longhairedboy, post:106, topic:44375"]
the critics are heralding it as “an autobigraphical autobiography autobiographed by an autobiographer.”
[/quote]

Please make sure to send me a copy :star_struck:
```

---
## \#110 Posted by: Kaly Posted at: 2018-01-23T19:49:20.260Z Reads: 326

```
Man send some stuff your way :-) 
Let me know when it get good to drop by your area
```

---
## \#111 Posted by: JohnnyMeduse Posted at: 2018-01-23T20:01:28.968Z Reads: 329

```
It will need at least 2 month, snow and ice everywhere...

![image|666x500](upload://pIO8CMbl9ujzM6dqZopoOunMWPQ.jpeg)
```

---
## \#112 Posted by: Kaly Posted at: 2018-01-23T20:19:24.579Z Reads: 322

```
Ugh 
Any ways 
I want to go in the spring
```

---
## \#122 Posted by: bimmer Posted at: 2018-01-24T03:27:49.912Z Reads: 322

```
I have 4 prototypes done that are driving me to lunch daily. :slight_smile:
```

---
## \#123 Posted by: Eboosted Posted at: 2018-01-24T07:30:47.938Z Reads: 323

```
I think @stewii has already developed this idea and it's working good so far, he just needs to automate things and mass produce them in order to lower the cost.

I can see everyone is trying to develop this idea so I hope we have VESCs 6 with good price tags available from different sources soon.

Btw my ESCape from @stewii is running pretty good after 300kms will let you guys know when I reach 1000 miles, on the other hand so are my focboxes on my Darth Maul and my @torqueboards 4.12 on my Vanguard after more that 5000kms
```

---
## \#124 Posted by: PredatorBoards Posted at: 2018-01-24T08:11:24.586Z Reads: 313

```
Gimme a number so I can buy some! Wanna use these for an upcoming product coming down the line... if only I wasn't so engrossed in the manufacturing of the current boards I'm selling, i'd share the production costs with you...
```

---
## \#125 Posted by: bimmer Posted at: 2018-01-24T10:13:26.201Z Reads: 309

```
Stewie and I have come to an accord.
```

---
## \#126 Posted by: abenny Posted at: 2018-01-24T15:29:33.039Z Reads: 309

```
I waaaaaaaant one!! Or 2...  :grin:
```

---
## \#127 Posted by: ThierryGTLTS Posted at: 2018-01-24T15:58:28.136Z Reads: 322

```
Fine.

Just pay attention when choosing the caps (MLCC and ELCOs), they are the most critical parts.

Thierry
```

---
## \#128 Posted by: bimmer Posted at: 2018-01-26T21:53:29.860Z Reads: 324

```
Soo the first 50 can come with a nylon 3d printed enclosure  with heatsink 3$ or aluminum +25$. 
![1517003347521631868695|281x500](upload://kJ7I988GlLc0jbF9uziS6uEQQ0R.jpg)a![1517003570521915473887|281x500](upload://1O1HKAzkJh1rnagxA6T3IcJTAwO.jpg)
Preferences?
```

---
## \#129 Posted by: scepterr Posted at: 2018-01-26T22:03:10.587Z Reads: 317

```
I would go with full aluminum
```

---
## \#130 Posted by: Cobber Posted at: 2018-01-26T22:15:34.941Z Reads: 320

```
[quote="scepterr, post:129, topic:44375, full:true"]
I would go with full aluminum
[/quote]

what he said, with changes to the heat sink you have effectively changed a critical part of the design and could get mass failures without your own testing.
```

---
## \#131 Posted by: bimmer Posted at: 2018-01-26T22:16:31.310Z Reads: 317

```
Every option has a heatsink the cutout is for exactly those.
```

---
## \#132 Posted by: Deckoz Posted at: 2018-01-26T22:44:47.387Z Reads: 316

```
Tiny block of aluminum ≠ bigger block
```

---
## \#133 Posted by: cosmicc89 Posted at: 2018-01-27T04:41:57.610Z Reads: 313

```
I would also rather pay a bit more and get all aluminum
```

---
## \#134 Posted by: monkey32 Posted at: 2018-01-27T06:23:13.388Z Reads: 305

```
AL way better. Also when. Can I buy?
```

---
## \#135 Posted by: abenny Posted at: 2018-01-27T06:31:01.876Z Reads: 310

```
same, when can i get one (or two)
```

---
## \#136 Posted by: chinzw Posted at: 2018-01-29T16:59:43.466Z Reads: 321

```
[quote="Kug3lis, post:40, topic:44375"]
Plus not a single company will do 500 units, its not efficient they will suggest to go with casting and finishing :wink:
[/quote]

You're saying bimmer has no idea about production. But in reality it is you that has no idea.
There's plenty machine shops that are able to manage that amount of work.
```

---
## \#137 Posted by: Kug3lis Posted at: 2018-01-29T17:29:05.574Z Reads: 317

```
Lol, yes any shop can do this, buts it's not efficient that's why I am saying not many shops would like to work on single piece for weeks ;)

P.S. I have background in much bigger productions like 1000 times ;)
```

---
## \#138 Posted by: Minim Posted at: 2018-01-29T18:24:33.723Z Reads: 314

```
Not many shops would like same part for weeks? That’s awesome. I would love something like that. I could make special fixtures for my mill and order pre cut materials. Quickly load 30 pieces on the table, hit cycle start and go do smt else until the M30 light goes off. Less time fiddling and more machining time is good for business.
```

---
## \#139 Posted by: chinzw Posted at: 2018-01-29T18:26:19.062Z Reads: 309

```
Repetitive work is where gains are made. Fixturing and setup are very costly. On the other hand, replacing stock and running cam is not.
```

---
## \#140 Posted by: Kug3lis Posted at: 2018-01-29T18:44:15.714Z Reads: 312

```
Yes, but shop will better do more jobs on lower scale and earn more money on fixturing than doing same design over and over that's just my experience with shops in Europe side ;)
```

---
## \#141 Posted by: banjaxxed Posted at: 2018-01-29T19:25:20.693Z Reads: 310

```
🍿 work ethic 😂
```

---
## \#142 Posted by: bimmer Posted at: 2018-01-30T02:48:45.750Z Reads: 322

```
I'm over talking about machining. I've reduced material by 30% and machine time by 40% with out sacrificing heat sinking. I am trying to offer a good product for a reasonable price not get rich and make high end parts.
All electronics will remain 100% original according to Bom by Stewie.
The case is going to be a 3 part: Aluminum base, Abs midsection and PCB top(cover).
![Render2|690x351](upload://mcgRbKxhOJEQCja8kUdXDwGlLXS.jpg)![case|690x351](upload://3Wj19ELspb3f5mP8Xy7jTlyeLRN.jpg)
Just realized I don't need the inserts anymore.
```

---
## \#143 Posted by: Minim Posted at: 2018-02-01T22:46:15.511Z Reads: 317

```
Is the case open source? I’d love to mill a few if they fit Stevie’s design.
```

---
## \#144 Posted by: bimmer Posted at: 2018-02-01T23:49:40.155Z Reads: 312

```
What cad format do you need? @Minim
```

---
## \#145 Posted by: telnoi Posted at: 2018-02-02T06:49:44.607Z Reads: 311

```
Offer a no warranty option for EU?
Warranty is usually limited anyway with user installed electronics. For the price you are asking, some may be willing to risk it.
```

---
## \#146 Posted by: bimmer Posted at: 2018-02-02T09:13:20.438Z Reads: 320

```
![Catch7706|375x366](upload://tddMWPcZGt464J35xnVIRwdDLTJ.jpg)
![C8FEB142-1320-46C4-B5FB-20C89A97E279|375x500](upload://eu9UUqPZtKCyDNNdSAVXIUb4N94.jpeg) heatsinks are done and inroute aswell as all electrical components. 
Just waiting for the pcb's now.
```

---
## \#147 Posted by: monkey32 Posted at: 2018-02-02T12:49:30.621Z Reads: 313

```
Where am is sending the monies/placing the order???
```

---
## \#148 Posted by: bimmer Posted at: 2018-02-02T15:03:38.411Z Reads: 314

```
You don't yet, I don't want anyones money unless I have full controll over everything. The heatsinks could get held up at customs etc
But I might set up a pre order form or such where you can secure one of the 50 when they are ready. 
EDIT: I've goten alot of messages asking for pre orders. I need everyone to understand that if I do offer pre order it will take the time it takes if you can't wait do not send me money. I will wait and see how people feel about this and if its mostly positive, I  will publish the form.
```

---
## \#149 Posted by: stormboard1 Posted at: 2018-02-02T15:05:36.334Z Reads: 308

```
How much roughly would the preorder ones be ?im in lol
```

---
## \#150 Posted by: ATLesk8 Posted at: 2018-02-02T15:23:18.112Z Reads: 307

```
Im in too too too
```

---
## \#151 Posted by: chsknight Posted at: 2018-02-02T16:41:27.263Z Reads: 308

```
Ill take one too!
```

---
## \#152 Posted by: Mobutusan Posted at: 2018-02-02T17:32:21.500Z Reads: 306

```
I'm down for two. These look great so far.
```

---
## \#153 Posted by: louwii Posted at: 2018-02-02T17:50:55.333Z Reads: 310

```
It would be cool to have one tested in really rough conditions. Unless that's been done already ?
```

---
## \#154 Posted by: b264 Posted at: 2018-02-02T21:08:06.094Z Reads: 310

```
I want 2 of these
```

---
## \#155 Posted by: Minim Posted at: 2018-02-02T23:57:29.808Z Reads: 304

```
something that fusion 360 can eat :D
```

---
## \#156 Posted by: ARetardedPillow Posted at: 2018-02-03T06:02:23.639Z Reads: 305

```
I want one!
```

---
## \#157 Posted by: bimmer Posted at: 2018-02-03T11:35:12.860Z Reads: 304

```
Ipt? Fusion is autodesk.
```

---
## \#159 Posted by: Cobber Posted at: 2018-02-03T12:45:01.787Z Reads: 311

```
hey dude I know you have the best of intentions but you are not a regular or level three member so you can not do a group buy according to the forum rules. 

This was let go before as you were bank rolling this your self, you need to get another member state side to get involved who is the right level or the mods will shut this down. Id suggest editing your above post and look for a level three near you I am sure all will be willing to help to make this happen.

Where do you live bro?

@b264
@stormboard1
@louwii
@cosmicc89
@Deckoz
@scepterr
@JohnnyMeduse   
@mmaner 
@longhairedboy

here are a few options who have been involved in this thread, I could do it but I'm downunder bro
```

---
## \#160 Posted by: PXSS Posted at: 2018-02-03T12:51:16.888Z Reads: 298

```
I'd be willing to help with requirements of lvl 3 member and handling the group buy. 

PM me @Bimmer and we can work out something.
```

---
## \#161 Posted by: bimmer Posted at: 2018-02-03T14:43:25.447Z Reads: 290

```
I am still bankrolling this myself everything has been purchased by me. You are not participating in a group buy but merely reserving one for yourself, if that breaks the rules I will remove that option and sell them on a first come first serve basis.
```

---
## \#163 Posted by: Stevemk14ebr Posted at: 2018-02-03T14:55:07.403Z Reads: 294

```
@Cobber 

I'm fine with him doing this, if you dont like being the police then dont be. Let an admin yell at him if he's breaking the rules, until then i'd prefer if everyone lets him do his thing.

A group buy implies someone acting as a middle-man, this however seems more like a simple business selling a product.
```

---
## \#167 Posted by: scrapheap Posted at: 2018-02-03T15:07:49.646Z Reads: 297

```
The admins, if they see something that violates the rules, will just close the topic with a succinct post as to why they shut it down.

The rules are in place for a reason. Yes it's frustrating for those trying to establish themselves and help the community, but rules are rules and there are reasons behind each one.

On another note, I hope this thread doesn't get shut down. Hopefully a level 3 member will volunteer to help with this situation, since it's a great opportunity for the community to have access to HW6.4 without the exorbitant price tag.
```

---
## \#169 Posted by: Cobber Posted at: 2018-02-03T15:38:43.757Z Reads: 294

```
yet again it seems the near youngest member of the forum is also showing the most maturity...
tiz a crazy world...
```

---
## \#170 Posted by: GrecoMan Posted at: 2018-02-03T15:39:50.768Z Reads: 291

```
guys...

@Cobber is right. You don’t get lvl 3 from sitting around afk and doing nothing... you’d think they’d realize that regulars (me and cobber both have 20+ days read) know the rules just a bit better than they do... guess not 🤔
```

---
## \#171 Posted by: Deckoz Posted at: 2018-02-03T15:45:49.689Z Reads: 298

```
I'll help if need be...just put me on the list of people to get one... Haha

Really. I don't think this is a group buy as @bimmer is fronting everything himself. And at a later date selling. No funds exchanged to make the product go to production. He is selling the once they are in hand. I think he's fine.
```

---
## \#172 Posted by: GrecoMan Posted at: 2018-02-03T15:49:51.871Z Reads: 296

```
doesn’t reserving one cost $$?

if no, then carry on, he can sell as long as he doesn’t collect money before the product is in his hand.
```

---
## \#173 Posted by: Namasaki Posted at: 2018-02-03T15:51:04.783Z Reads: 299

```
@bimmer as a level 2, you can sell parts in the new items catagory. 
Whether it's a group buy or Pre-order or reservation or what ever you want to call it.
 As a level 2, you may not take members money until you have the items ready to ship.
You need to just buy the parts and make the Esc's and then sell them on a first come first serve basis.
I am shutting this topic down and you can repost your Esc's for sale when you have them ready to ship.
```

---
## \#176 Posted by: Namasaki Posted at: 2018-02-09T12:59:01.343Z Reads: 288

```

```

---
## \#177 Posted by: Namasaki Posted at: 2018-02-09T12:59:05.568Z Reads: 288

```

```

---
## \#178 Posted by: Namasaki Posted at: 2018-02-09T13:00:36.835Z Reads: 293

```
I am reopening this topic in lieu  of @bimmer recent promotion to level 3
```

---
## \#179 Posted by: Stevemk14ebr Posted at: 2018-02-09T14:17:22.858Z Reads: 292

```
congrats on the upgrade @bimmer, welcome back to the thread!
```

---
## \#180 Posted by: bimmer Posted at: 2018-02-09T15:24:19.706Z Reads: 300

```
Thank you @Namasaki 

An update on the Esc's,  PCB's and Covers are inroute.

Heatsinks are here and I might solder up an ESC this afternoon to send to @longhairedboy  so he can abuse it.

It would still be the old Pcb not the new 2Oz and immersion gold one.

For now I have ordered the basic BOM which would give you only the ESC (FOC/BLDC) functionality and no NRF or motion sensor. Is this enough or do people want the NRF? (I am under the impression there is only 1 remote that works so far and it has to be assembled). I am looking into having those made as well but we just signed to build a house and I probably won't get the OK to start another project until this one is done with.
```

---
## \#181 Posted by: longhairedboy Posted at: 2018-02-09T15:29:24.238Z Reads: 294

```
i can't speak for eveyone, but as long as PPM and UART are physically present i'm good.
```

---
## \#182 Posted by: Nordle Posted at: 2018-02-09T15:32:24.711Z Reads: 290

```
What purpose does the motion sensor have on the esc?
```

---
## \#183 Posted by: bimmer Posted at: 2018-02-09T15:38:19.896Z Reads: 291

```
Just imagine a 4.12 that doesn't fry and comes in a fancy box. Can forwarding works wonderfully and also I have turned them On one after another and it did not kill one or both like the old one :smiley:
```

---
## \#184 Posted by: bimmer Posted at: 2018-02-09T15:38:43.797Z Reads: 289

```
I really do not know it was on the BOM.
```

---
## \#185 Posted by: bevilacqua Posted at: 2018-02-09T15:43:09.080Z Reads: 295

```
Mainly Robotics, and other smaller aplications I think. VESC 6.X is suposed to be a more open platform. 

Cheers, 
Mathias
```

---
## \#186 Posted by: bimmer Posted at: 2018-02-09T15:43:57.265Z Reads: 294

```
So for our application we can spare ourselves the extra parts.
```

---
## \#187 Posted by: JonathanLau1983 Posted at: 2018-02-09T15:45:55.311Z Reads: 283

```
Think you can use the motion sensor for turning indicators.
```

---
## \#188 Posted by: longhairedboy Posted at: 2018-02-09T15:49:54.995Z Reads: 282

```
i'm mainly interested in the increased power handling and abuse tolerance. I've managed to eak about as much life out of a focbox as i can get using just settings and vibrational damping techniques. They last pretty much forever in my boards now, but anything that eliminates accidental failures during installation would be welcome.
```

---
## \#189 Posted by: sk8l8r Posted at: 2018-02-09T16:05:49.425Z Reads: 282

```
[quote="JonathanLau1983, post:187, topic:44375"]
motion sensor
[/quote]

hmm interesting I wonder if it would output G-forces?


please put me down for 2 also
```

---
## \#190 Posted by: MatwoSvK Posted at: 2018-02-09T16:12:11.909Z Reads: 274

```
@bimmer
 Looks good, i would take 2 if you still not have all 50 reserved.
```

---
## \#191 Posted by: Minim Posted at: 2018-02-09T16:16:49.827Z Reads: 273

```
Was it possible to get the design files for the box? The thread got locked last time so I couldn’t respond In the thread. I need to open them in Fusion 360. 

Do you ship to Europe?
```

---
## \#192 Posted by: Nordle Posted at: 2018-02-09T16:21:27.572Z Reads: 275

```
E-Skate is a robot tough... if anyone has a better answer thank you.
Which motion does it sense?
```

---
## \#193 Posted by: bevilacqua Posted at: 2018-02-09T16:27:45.581Z Reads: 280

```
I guess it works like the accelerometrer on your smartphone. If you wont work with complicated torque vectoring aplications (witch would need even more data to work) I dont think it would be of any use...
```

---
## \#194 Posted by: banjaxxed Posted at: 2018-02-09T16:35:24.305Z Reads: 285

```
I'm down for two; one for my lawyer and one for me :wink: but we can wait for theose sexy new PCBs
```

---
## \#195 Posted by: bimmer Posted at: 2018-02-09T18:16:17.860Z Reads: 288

```
It is not implemented in the firmware yet so it serves no function other than preparing it for the future.
```

---
## \#196 Posted by: scepterr Posted at: 2018-02-09T18:21:35.916Z Reads: 289

```
I filled out the form you posted before for 2 units, is that good enough or should I watch out for a diff form?
```

---
## \#197 Posted by: bimmer Posted at: 2018-02-09T18:41:32.116Z Reads: 295

```
That'll be fine I haven't followed up due to the stipulations that were in place. I'll repost it and send out the e-mails coming week if you're on it now your spot is safe.
```

---
## \#198 Posted by: monkey32 Posted at: 2018-02-09T19:02:51.472Z Reads: 302

```
Hope I can jump in if not already on this form.....
```

---
## \#199 Posted by: bimmer Posted at: 2018-02-09T19:40:16.260Z Reads: 309

```
Currently:
pxss
Scepterr
stevemk14ebr
abenny
b264
Have their slots

https://docs.google.com/forms/d/1QbpQWJAd8oy1G9sD3S1dGwXv9YPar-sEDCh56AikP9o/viewform?edit_requested=true

the pre payment will only come due once everything is here and ready to be assembled after that Full payment will come due within 14 days. If you fail to pay the final amount in time you lose your slot and the pre-payment is refunded.
```

---
## \#200 Posted by: b264 Posted at: 2018-02-09T19:42:44.363Z Reads: 308

```
[quote="bimmer, post:180, topic:44375"]
For now I have ordered the basic BOM which would give you only the ESC (FOC/BLDC) functionality and no NRF or motion sensor. Is this enough or do people want the NRF?
[/quote]

I need the MPU9150 / MPU9250 motion-sensor; it is essential to my use-case

It can be added by hand if needed, as long as the pads are there
```

---
## \#201 Posted by: bimmer Posted at: 2018-02-09T19:43:37.453Z Reads: 300

```
I have  the parts for 10 here and can add them to yours.
```

---
## \#203 Posted by: banjaxxed Posted at: 2018-02-09T19:55:03.421Z Reads: 298

```
Is there a reservation method on the super-duper new pcbs yet
```

---
## \#204 Posted by: b264 Posted at: 2018-02-09T19:55:43.952Z Reads: 300

```
PCBs come from @stewii I think

B-box comes from @bimmer using @stewii's PCB

If I understand correctly
```

---
## \#205 Posted by: banjaxxed Posted at: 2018-02-09T19:58:44.656Z Reads: 296

```
Ok so @stewii supply chain
```

---
## \#206 Posted by: Exiledd_Top Posted at: 2018-02-09T19:58:45.250Z Reads: 303

```
Can someone tell me the price hw 6.4 ESC id gladly try it out but I don't know the price I scrolled up couldn't find the price
```

---
## \#207 Posted by: chomp Posted at: 2018-02-09T20:20:21.565Z Reads: 306

```
Search this thread. He said he’s gauging interest at 150 for the first 50.
```

---
## \#208 Posted by: chomp Posted at: 2018-02-09T20:28:44.387Z Reads: 307

```
Couple posts up he lists a link to a google doc which I think is the official reserve list.
```

---
## \#209 Posted by: Nordle Posted at: 2018-02-09T20:30:48.028Z Reads: 294

```
For what do you use the sensor? Just Curious:)
```

---
## \#210 Posted by: stewii Posted at: 2018-02-09T20:35:13.121Z Reads: 293

```
B-box cover PCBs also came from me , I customised it for him :)
```

---
## \#211 Posted by: bimmer Posted at: 2018-02-10T15:51:48.564Z Reads: 290

```
They will be the standard for all of them.
```

---
## \#212 Posted by: bimmer Posted at: 2018-02-10T15:53:28.296Z Reads: 289

```
Yes all the props should go to @stewie I am just taking a product he developed and and manufacturing it.
```

---
## \#213 Posted by: bimmer Posted at: 2018-02-10T16:03:03.873Z Reads: 286

```
The price will be 160$
```

---
## \#214 Posted by: lennylogs Posted at: 2018-02-10T16:11:33.620Z Reads: 286

```
That’s a good price. I think I’d like 2 of these...when is expected delivery? Also is there any sort of warranty/maintenance included if something goes wrong with them?
```

---
## \#215 Posted by: Exiledd_Top Posted at: 2018-02-10T16:36:07.132Z Reads: 289

```
From what I heard vesc6 designs are pretty hard to mess up , seller does provide a replacement if does not work on arrival but he tests them as well so am not to sure about failure warranty
```

---
## \#216 Posted by: Nordle Posted at: 2018-02-10T16:52:27.247Z Reads: 286

```
Do you plan to stock them at a later point? I don't need one yet but i want some in the future for sure:)
```

---
## \#217 Posted by: Jc06505n Posted at: 2018-02-10T17:57:55.914Z Reads: 283

```
How do these compare to Focboxes ?
```

---
## \#218 Posted by: bimmer Posted at: 2018-02-10T18:55:41.396Z Reads: 287

```
short answer yes. Not sure how yet.
```

---
## \#219 Posted by: bimmer Posted at: 2018-02-10T22:28:09.974Z Reads: 288

```
Like a scooter to a Porsche. Both will get you there you choose which suits you better.
```

---
## \#220 Posted by: Jc06505n Posted at: 2018-02-10T22:36:18.963Z Reads: 290

```
Oooo who’s the scooter and Porsche in this scenario?
```

---
## \#221 Posted by: b264 Posted at: 2018-02-10T23:29:14.877Z Reads: 299

```
The B-box and the ESCape and the VESC6 are the Porsches.  They all have the same motor.
```

---
## \#222 Posted by: bimmer Posted at: 2018-02-11T02:41:53.781Z Reads: 305

```
@longhairedboy
Sorry I am a day late we had had appointments (building a house here in AZ)
Anyhow starting your B-Box.
![20180210_193825|281x500](upload://kceWDeO338mnOmcaaQLWUuTqyOC.jpg)
```

---
## \#223 Posted by: longhairedboy Posted at: 2018-02-12T14:10:42.433Z Reads: 292

```
I'm pumped. We're probably going to test it in single drive with a terrible ratio and wheel height combo to try and get as much heat as possible and abuse the crap out of it. 

i foresee these simply being called "bimmers" as i have already sort of started calling them that to myself and jake.
```

---
## \#224 Posted by: Cobber Posted at: 2018-02-12T14:24:56.974Z Reads: 291

```
I second the motion!

@bimmer at this point you get no choice ;) bimmers it is, and likely if you arc up out of respect we will start calling them "stan"...

just don't F-up bro or LHB might start calling em bummers!
```

---
## \#225 Posted by: bimmer Posted at: 2018-02-12T18:33:12.067Z Reads: 290

```
I like it! I am currently running in the problem that my Hot-air station is now a Air station.... So there is a delay. But I wont start selling these till we get your seal of approval. Stay tuned amazon is working on a refund.
```

---
## \#226 Posted by: b264 Posted at: 2018-02-12T18:39:13.015Z Reads: 294

```
I respect your decision to abstain from general sales until an esk8 expert abuses the product trying to break it.  Very well done, sir.  Can't wait to have a couple of these and some Carv⏻n SD XL motors...
```

---
## \#227 Posted by: longhairedboy Posted at: 2018-02-12T19:52:49.012Z Reads: 302

```
We use a multi-phase ESC abuse testing schema in our shop with a built in vendor feedback loop. Here are the phases and vendor feedback interface descriptions::

1) hit them with sticks before even opening the box. Toss them around like you're a UPS man on crack and you just found out about some upcoming layoffs. Should this phase fail, the vendor will be beaten with sticks as well. 
2) open the packages carefully using a pair of rabid direwolves instead of a razor. If any product remains in tact, continue testing. If not, feed vendor to direwolves.
3) Travel to north dakota and strap ESC to double bladed axe in a single drive configuration using a 1:1 gearing ratio on 11" steel wheels and ride the axe repeatedly into trees and campers. If trees fall and campers run screaming into the cold night, continue testing. Otherwise ram vendor with axe board until dead. 
4) ride ESC equipped axe into heavy traffic during business hours while dragging a dead moose via tow chain in order to load test the traces and components. Should the ESC overheat, vendor will be dragged through heavy traffic instead of moose using a set of FocBoxes. 
5) remove ESC from axe board and continue to beat with sticks. This time, the sticks should be on fire and the ESCs should be mounted to the face of a statue of Frank from Trampa. Should the ESCs fail to remain in tact, vendor will be pants'd and youtubed. 


If all tests are passed and the ESC and vendor are still in tact, the product will receive our seal of approval. I would also like to point out that our process is more forgiving and less excruciating than becoming UL listed.
```

---
## \#229 Posted by: JohnA Posted at: 2018-02-12T22:23:40.649Z Reads: 289

```
@longhairedboy I used to work at UPS as a package loader. So I can tell you that step one is already done in transit. :thinking: Was never out of the ordinary for my manager to come in to the trailer, pissed about god knows what, and proceed to smash and stomp out 15 or so packages. Working there really opens up your eyes to the true UPS “logistics”.
```

---
## \#230 Posted by: b264 Posted at: 2018-02-12T22:43:24.349Z Reads: 293

```
I worked there as an auditor and as soon as I realized that EVERY truck is unloaded by opening the back door and throwing ALL the packages out the back onto a conveyor belt, the entire way I viewed shipping things changed completely
```

---
## \#231 Posted by: GrecoMan Posted at: 2018-02-12T22:51:39.471Z Reads: 296

```
the key is to make the shit like 600lbs so they can’t throw it 🤣
```

---
## \#232 Posted by: bimmer Posted at: 2018-02-13T03:40:02.872Z Reads: 306

```
Update:
Screws and silicone thermal pads arrived today.
My hot-air station is still busted so I can't flip the blue led :smiley: for @longhairedboy test esc. That being said it is functional right now.  
Right now I am still waiting for:
Pcb's, covers, pre wired xt-90 connectors, pre wired 3.5mm bullet connectors and new Aluminum Capacitors got 16mmx20mm instead of 12.5mmx30mm.
![20180212_203352|281x500](upload://jbtCIobiGrZnTLmGUPl11vlOxEi.jpg)
```

---
## \#233 Posted by: PXSS Posted at: 2018-02-13T04:11:12.049Z Reads: 294

```
Are you soldering all of these by hand?
```

---
## \#234 Posted by: bimmer Posted at: 2018-02-13T04:14:07.738Z Reads: 294

```
Gross No! I am having someone from our Avionics Prototyping department assemble the Pcb's. I'll be adding the cables and testing them before putting them in a Case.
```

---
## \#235 Posted by: scepterr Posted at: 2018-02-13T04:28:39.723Z Reads: 293

```
Did you open the hot air station? Usually its something pretty obvious that blew or disconnected
```

---
## \#236 Posted by: bimmer Posted at: 2018-02-13T04:33:28.077Z Reads: 292

```
Yeah a resistor split in half. They are sending me a new one it was only 4 weeks old.
```

---
## \#237 Posted by: scepterr Posted at: 2018-02-13T04:33:48.235Z Reads: 289

```
Could probably bridge it for now, or maybe not, you know what ita for?
```

---
## \#238 Posted by: bimmer Posted at: 2018-02-13T04:34:17.749Z Reads: 288

```
Tried it did nothing :(
```

---
## \#239 Posted by: scepterr Posted at: 2018-02-13T04:34:52.299Z Reads: 291

```
Hmm probably a pull down
```

---
## \#240 Posted by: bimmer Posted at: 2018-02-13T04:35:19.829Z Reads: 292

```
Not sure, it senses when its on its holder and turns on when its off. It just will not heat up anymore.
```

---
## \#241 Posted by: ThermalM16 Posted at: 2018-02-13T04:41:10.611Z Reads: 297

```
You can ship it as is and I can flip it for you if that's easier. LHB and I live pretty close, so if that's more convenient for you, I don't mind helping out
```

---
## \#242 Posted by: scepterr Posted at: 2018-02-13T04:42:36.695Z Reads: 308

```
Check this out, most of them match this schematic
http://www.heartoftechnology.com/reverse-engineering-the-858d-hot-air-rework-station/
![Screenshot_20180212-234615|281x500](upload://w4wiyntl10ZhZrm9MBcQ5qSwGDJ.jpg)
```

---
## \#243 Posted by: bimmer Posted at: 2018-02-13T04:51:41.846Z Reads: 295

```
It's not really that pressing of a matter as it already works fine its just the power on led.  I'd just prefer something good left my house.
```

---
## \#244 Posted by: bimmer Posted at: 2018-02-13T04:55:00.371Z Reads: 291

```
I think I have the odd one. It uses the exhaust from the soldering irons suction to blow air to the hot-air side. 992DA
```

---
## \#245 Posted by: scepterr Posted at: 2018-02-13T05:05:24.569Z Reads: 291

```
Lol you do have a wierd one..
With all those chinese ones I'de stick with the simplest looking ones, they last. I've got 100s of hours on $40-50 hot air guns
```

---
## \#246 Posted by: bimmer Posted at: 2018-02-13T05:08:19.151Z Reads: 298

```
Yeah.. they are replacing it. If it breaks again I'll use amazons A-Z and get my money back.
```

---
## \#247 Posted by: longhairedboy Posted at: 2018-02-14T12:24:59.929Z Reads: 303

```
i bought a T962 reflow oven recently for about $150. i still haven't fired it up, but sooooooon. This is it right here:
https://www.ebay.com/itm/260799459468

I also have a sunkko 788H spot welder. I don't care what anyone says about those, i've been using mine for almost two years now and its solid. 

also using a generic solder station from MPJA 
http://www.mpja.com/Solder-Station-with-LED-Display-ZD-929C/productinfo/15845+TL/

I could be paying thousands for any one of those tools if i got equivalent "industrial" whatever, i guess you just have to find the stuff that works.
```

---
## \#248 Posted by: PXSS Posted at: 2018-02-15T11:30:46.377Z Reads: 302

```
I have all three of those and yes, they work but the industrial stuff is just soooo much better. The problem with a lot of that stuff is qc and reliability. I have 2 sunkko welder and one of them is the shit while the other is simply shit... my CNC welder is light years ahead! It makes a week long job into an afternoon worth of watching the thing go. 

Soldering station is the one place where I truly agree that there is no reason to spend thousands. Unless you go for a station that has all the fancy stuff like a pre heater, air reflow, board temp sensors, and a solder pot. Even then, the chinesium stuff usually works 90% as well as the real industrial stuff, just don't trust their temperature readouts. 

The IR heater melts connectors. I've never had great a experience with it. It's great for placing most components though and then finishing connectors up by hand. I use an eaven fancier technic for reflowing! It is called the walmart $10 skillet and block of aluminum on top to spread heat more evenly. You can get your pcb to sit at a toasty 75-100c and then just wave around the reflow pen as the solder flows! Works wonderfully on double sided pcbs too. Industry really saves more money in pick and place machines than the ovens themselves I believe.

Dude!!! Check this out! I need this in my life...
https://www.liteplacer.com
```

---
## \#249 Posted by: longhairedboy Posted at: 2018-02-15T12:08:27.013Z Reads: 289

```
dude... that's how much i paid for my original x-carve kit... how sick would it be to have an ESC assembler droid?
```

---
## \#250 Posted by: Surfer Posted at: 2018-02-15T12:21:18.609Z Reads: 289

```
Hey @bimmer could you say how heavy is your b-box? I got the escape and the whole thingy it's 225gr almost half kilo for 2!!
I'm curious if your approach of the box is noticeable lighter.
Thanks!
```

---
## \#251 Posted by: bimmer Posted at: 2018-02-15T12:21:43.194Z Reads: 287

```
You mean like a open source pick'n'place?
```

---
## \#252 Posted by: longhairedboy Posted at: 2018-02-15T12:27:15.272Z Reads: 286

```
That is literally what that is, yes.
```

---
## \#253 Posted by: PXSS Posted at: 2018-02-15T12:36:13.704Z Reads: 286

```
I want it! I need to convince that money people that we need one lol
```

---
## \#254 Posted by: bimmer Posted at: 2018-02-15T12:41:51.600Z Reads: 291

```
Nightshift... sorry skipped pxss post. Yeah thats pretty cool a little slow but cool.
```

---
## \#255 Posted by: longhairedboy Posted at: 2018-02-15T12:56:09.812Z Reads: 290

```
i think i may have achieved 2 hours of sleep last night so i'm kind of there with you.
```

---
## \#256 Posted by: bevilacqua Posted at: 2018-02-15T16:58:31.775Z Reads: 290

```
Since the housing is a 2 piece system = Alu base/heatsink + Plastic sides, I guess it will be lighter.
```

---
## \#257 Posted by: KeivanM Posted at: 2018-02-16T00:19:21.669Z Reads: 284

```
I just placed a pre order, so the pre order is 40, how much is the final price? shipping it to virginia usa?
```

---
## \#258 Posted by: chomp Posted at: 2018-02-16T01:26:59.485Z Reads: 288

```
Post 213, he said $160. Don’t know if that includes shipping or not.
```

---
## \#259 Posted by: bimmer Posted at: 2018-02-16T07:49:17.942Z Reads: 286

```
shipping is 5$
```

---
## \#260 Posted by: bimmer Posted at: 2018-02-16T07:50:45.027Z Reads: 295

```
Super unhappy with how usps is delivering my stuff lately even amazon prime items are 2-3 days late.
![Pcb's|613x500](upload://nQokneNKlqzYqD5h1C2vQ7I7hFj.jpg)

Edit:  For context these are the Pcb's.
```

---
## \#261 Posted by: b264 Posted at: 2018-02-16T08:03:48.147Z Reads: 288

```
Looks like they are in a trailer sitting at the depot waiting for a tractor LoLz
```

---
## \#262 Posted by: bimmer Posted at: 2018-02-18T04:10:17.366Z Reads: 293

```
![20180217_210854|281x500](upload://nPfrutlIB6yxavQLqnsCGXDCQDT.jpg)
Just waiting on the wires and the new hot-air station.
```

---
## \#263 Posted by: scepterr Posted at: 2018-02-18T04:17:22.946Z Reads: 289

```
Those are kinda skinny power leads 🤔 could be just the photo angle
```

---
## \#264 Posted by: bimmer Posted at: 2018-02-18T04:26:40.553Z Reads: 296

```
You are correct I stole them off a fried Miami Vesc that someone sent me for a few bucks so I could send one to LHB, right before my Hot-air ate Sh*$T. The "real" ones will have Awg 12.![Screenshot_20180217-212505|243x500](upload://uLsQKTHevMLmc5NZkHL9xmKWdAS.jpg)
```

---
## \#265 Posted by: PXSS Posted at: 2018-02-18T04:29:46.391Z Reads: 286

```
@bimmer, you on the west coast?
```

---
## \#266 Posted by: scrapheap Posted at: 2018-02-18T04:37:14.698Z Reads: 284

```
I think he's located in Arizona.
```

---
## \#267 Posted by: PXSS Posted at: 2018-02-18T04:37:42.983Z Reads: 286

```
Ew...
10ch
E:Unless it's flagstaff. That place is pretty cool
```

---
## \#268 Posted by: bimmer Posted at: 2018-02-18T04:38:43.553Z Reads: 290

```
Nah phoenix
```

---
## \#269 Posted by: PXSS Posted at: 2018-02-18T04:39:48.909Z Reads: 291

```
I'll say nothing else...
```

---
## \#270 Posted by: bimmer Posted at: 2018-02-18T04:45:58.359Z Reads: 287

```
You should convince Lockheed that we need a office in Newport lol
```

---
## \#271 Posted by: PXSS Posted at: 2018-02-18T05:01:13.562Z Reads: 288

```
Move to Atlanta. Lockheed has offices here. Or literally anywhere else. If there's a hell on earth, its pheonix. Maybe Yuma. Definitely Yuma
```

---
## \#272 Posted by: ATLesk8 Posted at: 2018-02-18T05:32:48.098Z Reads: 284

```
Dude...who went back up the thread and flagged all our humorous banter? People out flagging like crazy today...grow up
```

---
## \#273 Posted by: Clonkex Posted at: 2018-02-18T22:28:34.332Z Reads: 293

```
[quote="bimmer, post:81, topic:44375"]
No EU shipping.
[/quote]

[quote="Clonkex, post:82, topic:44375"]
…why specifically EU?
[/quote]

[quote="bimmer, post:84, topic:44375, full:true"]
Oh short shipping and response time also lower shipping cost incase of rma. Basically this is a test and if something goes wrong 5.60$ shipping sounds better than 18$ ontop of refunding someone or replacing/fixing something.
[/quote]

Wait wait wait... so when you say "no EU shipping", do you mean "no EU shipping" or "only USA shipping"? Because that's an enormous difference. That's why I asked "Why specifically EU?" It seems strange to limit shipping to "worldwide except EU".

The reason I say this is that I want to prepurchase 2 of these sexy bimmers but I'm in Australia. The thing is, if I have a problem and need to RMA, I'll just pay the shipping costs. I'd rather have the risk of having to pay more shipping than not be able to buy them at all.
```

---
## \#274 Posted by: pixelsilva Posted at: 2018-02-18T23:11:47.383Z Reads: 295

```
....you name it:

**CLON-ESC**

**REPEAT-ESC**

**COPY-ESC**

**XESC**

**iESC**

**ESK8-ESC**

**CC-BOX**

**E-BOX**

...the ESC of all trades.
```

---
## \#275 Posted by: bimmer Posted at: 2018-02-19T01:14:42.433Z Reads: 289

```
OH no EUROPE, its very simple actually Stewie is in Europe and I don't want to be poaching in his territory as I bought the Pcb's from him and it just seems simpler for someone to order from England than the USA that is in Europe.
```

---
## \#276 Posted by: bimmer Posted at: 2018-02-19T01:16:55.113Z Reads: 283

```
I'm not sure the point you are making. It needed a Name and now it has one that doesn't interfere with someone's trademark.
```

---
## \#277 Posted by: ThermalM16 Posted at: 2018-02-19T01:25:21.186Z Reads: 286

```
@bimmer @pixelsilva  Guys come on we can all agree the "ThermalM16 (aka The Board Tech who can fix your VESC if it's broken)-Box" is the best name :joy: It rolls right off the tongue and I was one of the first people to give bimmer totally opinionated advice that had no factual reasoning behind it. I swear I'm not hijacking your thread, it just looks like it
```

---
## \#278 Posted by: bimmer Posted at: 2018-02-19T01:28:42.357Z Reads: 295

```
![Screenshot_20180218-182809|243x500](upload://cb2GWLIHRoXRGwxUXGmfEIgARUc.jpg)alright fixed it.
```

---
## \#279 Posted by: ThermalM16 Posted at: 2018-02-19T01:32:27.033Z Reads: 289

```
I've never been so happy in my life, I'm tearing up a little bit :sob:
```

---
## \#280 Posted by: Clonkex Posted at: 2018-02-19T02:05:41.667Z Reads: 290

```
Aha, I see! Thanks for the clarification, that makes much more sense now :+1:
```

---
## \#281 Posted by: TarzanHBK Posted at: 2018-02-19T07:44:17.474Z Reads: 285

```
I had a Thermal X-Box once... fuckn ring of death..
```

---
## \#282 Posted by: pixelsilva Posted at: 2018-02-19T08:05:24.078Z Reads: 294

```
**Thermal X-Box** sounds good @bimmer :yum::rofl:, besides.... you don't want to have issues later with Bayerische Motoren Werke once they fully enter the electric car business.

![image|334x437](upload://vya9nLxdHGmAxsqWkHG0LDTSHvN.jpg)
```

---
## \#283 Posted by: chuttney1 Posted at: 2018-02-19T08:17:34.919Z Reads: 294

```
Becareful on the X-Box name, Way too similar to Microsoft's Xbox eventhough the B is capitalized and after a hyphen.
```

---
## \#284 Posted by: Clonkex Posted at: 2018-02-19T08:17:55.855Z Reads: 309

```
Honestly I think B-box is fine...
```

---
## \#285 Posted by: bimmer Posted at: 2018-02-19T08:18:49.577Z Reads: 312

```
![15190281639132045638440|281x500](upload://bBg3hbdrqn1TPqUr7rf0JVxfLJt.jpg)I have spoken.
```

---
## \#286 Posted by: Clonkex Posted at: 2018-02-21T23:02:24.347Z Reads: 308

```
Purely out of curiosity... what's goin' on? :) I really just want to see moar pictures of things :P
```

---
## \#287 Posted by: moon Posted at: 2018-02-21T23:41:48.932Z Reads: 305

```
Please share your experiences and the building process :sunny: 

Ps how much did that cost, did it come straight from China or from stewii
```

---
## \#288 Posted by: bimmer Posted at: 2018-02-22T01:30:05.064Z Reads: 306

```
They came from Stewie so England :D  I am still waiting on a couple parts from China, Cables with connectors to be exact. I can share my experiences but they will be made somewhere where I cant take pictures. I will take pictures once I have the Pcb's back and start assembling them.
```

---
## \#289 Posted by: moon Posted at: 2018-02-22T01:37:21.404Z Reads: 297

```
You working in some secret lab or something 😂😂😂
```

---
## \#290 Posted by: bimmer Posted at: 2018-02-22T01:39:37.778Z Reads: 293

```
They will be made where we make our protoypes. So yeah kinda lol
```

---
## \#291 Posted by: banjaxxed Posted at: 2018-02-22T07:57:18.292Z Reads: 290

```
SR72 side project, these ESCs are spy esc.
Skunkesc
```

---
## \#292 Posted by: PXSS Posted at: 2018-02-22T09:14:18.562Z Reads: 285

```
SR72-e model
```

---
## \#294 Posted by: PXSS Posted at: 2018-02-24T01:27:37.975Z Reads: 283

```
What's your problem?
```

---
## \#295 Posted by: Clonkex Posted at: 2018-02-24T01:45:04.578Z Reads: 283

```
It only needs one flag to hide a post. Yeah it's dumb.
```

---
## \#296 Posted by: ATLesk8 Posted at: 2018-02-24T01:47:30.945Z Reads: 289

```
I just wish it showed who flagged it so they could be held accountable publically
```

---
## \#297 Posted by: KeivanM Posted at: 2018-02-24T03:57:44.507Z Reads: 295

```
when do you think they will be for sale?
```

---
## \#298 Posted by: bimmer Posted at: 2018-02-24T14:55:19.734Z Reads: 304

```
I'm sorry it's taking so long. I just want to be sure everything will go as smooth as possible once people have given me their money. I am in the final phase of making these. I have all parts so far. There is a minor discrepancy with the case and lid. I had the heat sinks made according to the old case design but Stewie made the Cover Pcb's according to the new one. I'll have to modify the holes to accommodate this.
As for assembly we should be able to start in a week.![15194872875911551908582|281x500](upload://v51ZXEKcglXtKdar5LtXVMnJZxk.jpg)
```

---
## \#299 Posted by: bigben Posted at: 2018-02-24T18:13:50.002Z Reads: 299

```
This hobby is a waiting game in general. As an outsider it seems you are making very quick progress!
I think you stand a chance of going from just an idea, to delivery quicker than some suppliers can deliver so called in stock items...
```

---
## \#300 Posted by: bimmer Posted at: 2018-02-24T19:21:45.390Z Reads: 294

```
Thanks for the positive feedback. I think its easier since for me things like price are secondary... like using automotive fets instead of waiting on stock for the regular ones
```

---
## \#301 Posted by: michaelcpg Posted at: 2018-02-25T23:56:59.485Z Reads: 290

```
What's the difference automotive fets and the ones that other vendors would be using? Just better reliability I'm guessing?
```

---
## \#302 Posted by: Clonkex Posted at: 2018-02-27T08:58:54.855Z Reads: 284

```
Aw, you changed your profile picture. Tony Stark was the perfect way to imagine you.
```

---
## \#303 Posted by: b264 Posted at: 2018-02-27T09:06:12.553Z Reads: 293

```
[quote="bigben, post:299, topic:44375"]
This hobby
[/quote]

It's not a hobby if you sold your cars
```

---
## \#304 Posted by: pixelsilva Posted at: 2018-02-27T10:28:29.296Z Reads: 296

```
....more like Elon Musk watching his Falcon Heavy boosters coming back to Earth....

https://i.kinja-img.com/gawker-media/image/upload/s--uftXojcy--/c_scale,f_auto,fl_progressive,q_80,w_800/ghhxdp5r1tj5wn1nxmqp.gif
```

---
## \#305 Posted by: gravitycarve Posted at: 2018-02-28T05:43:13.772Z Reads: 285

```
I want some of the goodness.
```

---
## \#306 Posted by: michaelcpg Posted at: 2018-03-06T01:05:53.359Z Reads: 279

```
Any updates available at this stage @bimmer? :)
```

---
## \#307 Posted by: b264 Posted at: 2018-03-06T01:15:40.835Z Reads: 285

```
Last I heard, beta testing and quality control testing is in-progress.  Testing these on real skateboards
```

---
## \#308 Posted by: bimmer Posted at: 2018-03-06T05:10:01.988Z Reads: 286

```
![20180305_220700|281x500](upload://fJn5Lw6r39jHNt0HlIhae7sdEbI.jpg)
I should ship the first 10 this weekend and then we wait and see how people like them.
I got them back from being made and need to place wires and troubleshoot each one individually.
I got one back that will start but shows undervoltage error.
It's a matter of checking all pins and all solder joints and takes forever.
```

---
## \#309 Posted by: Clonkex Posted at: 2018-03-06T05:22:58.277Z Reads: 278

```
[quote="bimmer, post:308, topic:44375"]
It’s a matter of checking all pins and all solder joints and takes forever.
[/quote]

I don't envy you.
```

---
## \#310 Posted by: skslingo21 Posted at: 2018-03-09T18:02:45.011Z Reads: 274

```
Cute cat! Best of luck in these endeavors! I am certainly interested.
```

---
## \#311 Posted by: bimmer Posted at: 2018-03-12T09:29:15.902Z Reads: 271

```
@sMATTEr
If you can find 5 people that also want 2 sets I'll make them for 100$
Just to be clear for everyone else these are diy kits I am talking about.
```

---
## \#312 Posted by: Nordle Posted at: 2018-03-12T10:14:46.143Z Reads: 267

```
I take one set to start with, have no clue in smd soldering, but that has to change:)
```

---
## \#313 Posted by: uigiroux Posted at: 2018-03-12T11:21:52.167Z Reads: 266

```
I'll take 2!
```

---
## \#314 Posted by: bimmer Posted at: 2018-03-12T11:44:20.805Z Reads: 276

```
I am happy to say the first 9 will ship out today.
Here you can see what it is and whats included.
I will be making more soon but work is going to be stressfull for the next 2 weeks and we want to see how these do in the wild.
![B-Box2|281x500](upload://5yWs6MpZf6uxikd4kO2l1KgO5yq.jpg)
![B-Box|690x388](upload://ejeCGsHI9VUJLfyeMmvD2qWWLSU.jpg)

That being said I will start offering do it yourself kit's.

PCB + BOM without NRF or Motion sensor 100$ 
B-BOX complete KIT (wires and case) 120$
Support will be limited to pictures and a guide on flashing. ( I can not troubleshoot your SMD work form around the world nor will I)
```

---
## \#315 Posted by: PXSS Posted at: 2018-03-12T14:25:26.853Z Reads: 266

```
2 of those are mine :' )
This has been the fastest and most effective groupbuy/preorder/not-groupbuy/whatever transaction I have been part of while on these forums. 

Props for making it happen. 

Enertion took 14 weeks to ship a product that was "in stock and ready to ship". 
Carvon dates keep slipping, so far 6 weeks behind schedule. 
You made this happen within 7 weeks of starting this thread and 2 weeks since payment. 

Really, thank you for not being a pain to deal with
```

---
## \#316 Posted by: Stevemk14ebr Posted at: 2018-03-12T14:47:33.180Z Reads: 263

```
I was in on this too, i must commend @bimmer for his response times, it's been a painless and clear-cut process the whole way through with nothing but good energy. Excited to try mine out when i get them!
```

---
## \#317 Posted by: michaelcpg Posted at: 2018-03-13T20:17:57.656Z Reads: 256

```
Awesome stuff @bimmer. Assuming I can get my Focbox order cancelled, I'll be keen for a pair of prebuilt models with the enclosures as soon as the next batch is available :)
Will you be accepting orders from NZ?
```

---
## \#318 Posted by: bimmer Posted at: 2018-03-13T21:45:07.261Z Reads: 254

```
There are 28 people ahead of you and yes but shipping will be expensive.
```

---
## \#319 Posted by: michaelcpg Posted at: 2018-03-13T21:52:33.061Z Reads: 253

```
Expensive shipping is pretty much a given when living in NZ unfortunately :p 
Do you know how many you're planning to build in the next batch?
```

---
## \#320 Posted by: bimmer Posted at: 2018-03-13T22:01:01.778Z Reads: 257

```
Probably a solid 30.
```

---
## \#321 Posted by: Ghettobird117 Posted at: 2018-03-14T01:01:51.140Z Reads: 256

```
Just put my name down for 2
Looking really good so far bimmer!
```

---
## \#322 Posted by: b264 Posted at: 2018-03-15T21:16:22.525Z Reads: 259

```
![20180315_153557_HDR|690x345](upload://mEsCvJBSHLkKvKjsa3VMIvNuEzn.jpg)
```

---
## \#323 Posted by: bimmer Posted at: 2018-03-15T21:58:28.334Z Reads: 257

```
I hope they live up to the hype.
```

---
## \#324 Posted by: pixelsilva Posted at: 2018-03-15T22:57:39.672Z Reads: 254

```
Another example that bsht sounds as bsht could last. Kudos to @bimmer and @stewii :+1: for delivering and not  becoming bshters like those typical esk8 wannabe companies full of lame and bsht excuses.
```

---
## \#325 Posted by: scepterr Posted at: 2018-03-15T23:21:20.683Z Reads: 259

```
Got mine today, coated them 😉
![IMG_20180315_170723__01|676x500](upload://10ENTGEEVumPcc5gjFPBjwmoAJY.jpg)
```

---
## \#326 Posted by: bimmer Posted at: 2018-03-16T00:27:35.080Z Reads: 258

```
Hopefully we will soon get them like that from the smd fab.
```

---
## \#327 Posted by: b264 Posted at: 2018-03-16T00:36:10.618Z Reads: 253

```
I am coating mine with acrylic conformal coating after I power them on and communicate via USB & bluetooth
```

---
## \#328 Posted by: scepterr Posted at: 2018-03-16T00:54:38.240Z Reads: 253

```
Lol replied in pics thread by accident 😂🤣😂🤣😂

Which vesc tool are we supposed to be using?
```

---
## \#329 Posted by: bimmer Posted at: 2018-03-16T00:55:09.784Z Reads: 253

```
Welp I am drunk and answered there....
```

---
## \#330 Posted by: scepterr Posted at: 2018-03-16T00:56:22.534Z Reads: 258

```
Ok to bump it to 3.35 with vesc tool .89?
```

---
## \#331 Posted by: bimmer Posted at: 2018-03-16T00:57:49.733Z Reads: 264

```
Not sure why it wouldn't be?
```

---
## \#332 Posted by: b264 Posted at: 2018-03-16T00:59:38.674Z Reads: 258

```
I definitely won't use that, I'll either use a `vesc_tool_0.87` Linux build or [the Ackamaniac one](https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116/200) if it has 64 firmware
```

---
## \#333 Posted by: scepterr Posted at: 2018-03-16T01:00:33.285Z Reads: 261

```
Hmm well it won't seem to stick for some reason, tried twice, maintains same firmware
```

---
## \#334 Posted by: bimmer Posted at: 2018-03-16T01:00:36.144Z Reads: 261

```
You could always flash it.
```

---
## \#335 Posted by: bimmer Posted at: 2018-03-16T01:11:12.154Z Reads: 266

```
So real talk guys how many B-boxes do you think we need in the U.S? We might have something big coming soon. A game changer, if you will.
Obviously no Nrf don't wanna have to deal with Ajit Pai you know?
```

---
## \#336 Posted by: scepterr Posted at: 2018-03-16T01:17:53.679Z Reads: 263

```
50-100/month, depending if you get resellers involved
```

---
## \#337 Posted by: scepterr Posted at: 2018-03-16T01:33:08.370Z Reads: 263

```
Ok so can't flash to 3.35 with vesc tool .89
Or 3.1 using Ackmaniac tool 😐

I only grabbed 1 bbox with me to play with at home so can't try with the other one yet
```

---
## \#338 Posted by: bimmer Posted at: 2018-03-16T01:44:40.189Z Reads: 258

```
you have an st-link?
```

---
## \#339 Posted by: scepterr Posted at: 2018-03-16T01:46:33.655Z Reads: 259

```
Ok figured it out, missing bootloader, flash bootloader first using tool, then flash firmware
No need for ST Link
```

---
## \#340 Posted by: bimmer Posted at: 2018-03-16T01:48:17.391Z Reads: 265

```
@DeathCookies Hier das sollte dir auch helfen
He actually got the very first ones still in 3d printed enclosures.
```

---
## \#341 Posted by: bimmer Posted at: 2018-03-16T01:51:54.359Z Reads: 268

```
So I've got to level with you guy's I have a masters in Aeronautics. I was not the brains behind the schematics nor the PCB's I am just really good at getting things done. So sometimes when you ask me questions I have no answer :smiley:
```

---
## \#342 Posted by: scepterr Posted at: 2018-03-16T01:51:55.698Z Reads: 263

```
Ok, another interesting thing, it stays powered via USB, disconnected from battery
![IMG_20180315_215254|666x499](upload://kHb4sUcXjkbt5Z99zGmJWH3R28z.jpg)
```

---
## \#343 Posted by: briman05 Posted at: 2018-03-16T01:58:07.009Z Reads: 255

```
Could I ask why there would be a 5.6% tax?
```

---
## \#344 Posted by: deltazeta Posted at: 2018-03-16T02:00:11.870Z Reads: 252

```
The mcu needs power in order flash
```

---
## \#345 Posted by: Clonkex Posted at: 2018-03-16T02:00:44.535Z Reads: 251

```
Maybe that's a change with VESC6? That it can be powered from USB only? Hopefully it wouldn't try to draw lots of current if you tried to do a motor detection or something :confused:
```

---
## \#346 Posted by: bimmer Posted at: 2018-03-16T02:02:01.517Z Reads: 250

```
Where did you get tax from?
```

---
## \#347 Posted by: briman05 Posted at: 2018-03-16T02:06:24.354Z Reads: 249

```
Very first post... Lets say I would sell these at a moderate 130$ + tax(5.6%)=137$ I am pretty sure they’d sell out in a month.

If there is no tax being added then never mind but you can not add on a tax to an item when someone could be living in a state that doesn’t have taxes.
```

---
## \#348 Posted by: Clonkex Posted at: 2018-03-16T02:08:20.011Z Reads: 246

```
I think that was just an estimated price, not the actual final price.
```

---
## \#349 Posted by: bimmer Posted at: 2018-03-16T02:15:02.976Z Reads: 253

```
Yeah that was just brainstorming like 7 weeks ago.
```

---
## \#350 Posted by: briman05 Posted at: 2018-03-16T02:38:52.089Z Reads: 248

```
Ok never mind I just don’t want anyone getting in trouble for charging taxes when they shouldn’t IRS would be on your ass quick
```

---
## \#351 Posted by: mmaner Posted at: 2018-03-16T03:06:12.218Z Reads: 244

```
[quote="briman05, post:347, topic:44375"]
you can not add on a tax to an item when someone could be living in a state that doesn’t have taxe
[/quote]

Unfortunately some states require taxes in items sold...hence sales tax. It's not always about where you purchase from but we're you sell from.
```

---
## \#352 Posted by: JLabs Posted at: 2018-03-16T03:19:25.038Z Reads: 247

```
Please don’t turn this into another useless tax debate
```

---
## \#353 Posted by: briman05 Posted at: 2018-03-16T03:20:57.129Z Reads: 248

```
Yeah Jersey has sales tax but it is if you have a presence in the state then you charge the sales taxes. I know for my job some states have a tax on labor but not items when installing equipment.
```

---
## \#354 Posted by: briman05 Posted at: 2018-03-16T03:22:32.799Z Reads: 253

```
I was t trying to it’s just something people have to watch out for. But he isn’t charging taxes so it is done now back to the thread
```

---
## \#355 Posted by: PXSS Posted at: 2018-03-16T03:27:08.664Z Reads: 252

```
Just cause you were doing things wrong and illegally doesn't make the conversation useless. Bimmer is not doing that here.
```

---
## \#356 Posted by: JLabs Posted at: 2018-03-16T03:34:01.571Z Reads: 256

```
Sorry I forgot you guys were Uncle Sam and know everything about running a business

Now there are 12 posts about taxes, which have nothing to do with this thread.. :expressionless:
```

---
## \#357 Posted by: Clonkex Posted at: 2018-03-16T03:59:29.098Z Reads: 258

```
It's pretty simple really. Depending on where you live, you might have to pay tax. That's all we're saying.

And actually it has everything to do with this thread. He's selling items in this thread, therefore taxes are relevant.
```

---
## \#358 Posted by: Idle Posted at: 2018-03-16T04:26:40.777Z Reads: 260

```
I didn't sub this thread to read about taxes.

Enough already please.
```

---
## \#359 Posted by: stewii Posted at: 2018-03-16T08:07:38.383Z Reads: 255

```
Yeah , thanks to R1 0ohm resistor :) Vesc6 might come without it , not sure.
```

---
## \#360 Posted by: chickengun Posted at: 2018-03-17T16:31:06.677Z Reads: 247

```
@stewii Do you plan to offer kits as well? I guess it would be easier to get them for people living in EU.
```

---
## \#361 Posted by: moon Posted at: 2018-03-17T16:36:51.337Z Reads: 247

```
He can sell PCB and stencil

The rest you should be able to get. But stuff is probably on back order
```

---
## \#362 Posted by: Acido Posted at: 2018-03-17T17:21:12.004Z Reads: 249

```
Can someone give me the dimensions of them with the box please
```

---
## \#363 Posted by: scepterr Posted at: 2018-03-17T17:37:30.406Z Reads: 247

```
Is there any possible damage having it powered by just usb? I know it faults and errors but that's just software triggers right? Nothing bad is happening to the mcu or drv?
```

---
## \#364 Posted by: Kug3lis Posted at: 2018-03-17T18:02:18.870Z Reads: 256

```
I think it's injecting 5v to drv 5V rail as there is nothing to prevent it ;)

![image|574x406](upload://emXr2lPy8yTnWRU3PEgmUFrNHu5.png)
```

---
## \#365 Posted by: fedestanco Posted at: 2018-03-17T18:09:39.297Z Reads: 251

```
On vesc6 r1 is not installed if I am right. So if you have a Trampa vesc6, usb will not power your vesc.
Dont know about stewii's vesc tough.
```

---
## \#366 Posted by: stewii Posted at: 2018-03-17T18:32:39.012Z Reads: 249

```
No damage at all :)  in that case the DRV is not running.
```

---
## \#367 Posted by: Kug3lis Posted at: 2018-03-17T18:45:07.930Z Reads: 246

```
but if the board is powered by battery and USB is connected then it's damaging?
```

---
## \#368 Posted by: bimmer Posted at: 2018-03-17T19:00:50.715Z Reads: 238

```
Nope
10char
```

---
## \#369 Posted by: Kug3lis Posted at: 2018-03-17T19:05:23.206Z Reads: 250

```
Can you tell me how it is not damaging? Because it's kinda the same situation then people connect CAN cable with 5V coming from another ESC, or plugging split ppm cable with joined 5V power lead. In those situations, DRV is always popping up so I am trying to imagine how is this different?

Because I don't see any protection against force feeding 5V back to DRV chip.

![image|690x207](upload://eSSSLgcB8A8CaLkMAsZj0FypDke.png)
```

---
## \#370 Posted by: fedestanco Posted at: 2018-03-17T19:09:53.252Z Reads: 243

```
In case of the canbus problem there is a full 5v short circuit.
In this case there is a smaller differential in voltage and the canbus chip may cope with this.

And there is probably a good reason why Vedder left r1 unistalled....
```

---
## \#371 Posted by: stewii Posted at: 2018-03-17T19:32:08.671Z Reads: 245

```
Well can you tell me why is it damaging? I havent damaged ANY ESCape by connecting USB only or USB and battery. 

Not sure where is the "full" short circuit, can you explain?@fedestanco
```

---
## \#372 Posted by: JohnnyMeduse Posted at: 2018-03-17T19:41:35.913Z Reads: 251

```
Not only you can damage your Vesc but also your PC, that why it was removed from the VESC

"The issue is that the two 5 V sources will not be at EXACTLY the same voltage.  One will be a little bit higher, the other a little bit lower.

Each of them will try to regulate the Bus at their voltage, and they will fight each other.

Likely one, or both, power supplies will die, perhaps catastrophically, damaging all of the other circuitry as well."

I think this summerise the issue you will get at a certain point.

(source : https://www.avrfreaks.net/forum/two-5v-power-sources-and-one-usb)
```

---
## \#373 Posted by: fedestanco Posted at: 2018-03-17T19:47:08.073Z Reads: 244

```
I was talking about the canbus problem that emerges when you connect 2 vescs via canbus and one of them is not powered.
```

---
## \#374 Posted by: JohnnyMeduse Posted at: 2018-03-17T19:48:35.028Z Reads: 248

```
The new Can bus chip is not affected by that behavior. It is a little more robust.
```

---
## \#375 Posted by: fedestanco Posted at: 2018-03-17T19:56:35.563Z Reads: 257

```
You got me curious so I compared the 2 datasheets: the old canbus chip has this tolerance on the CANH and CANL pins : -4 to 16v
The new chip brings the tolerance up: -58 to +58v. Thats quite an improvement
.
```

---
## \#376 Posted by: stewii Posted at: 2018-03-17T20:13:29.017Z Reads: 261

```
True, they wont be exactly the same voltage, the higher one will source the current and the lower will sink, i have never had any issue before but anyway it is easy to leave R1 out just in case.
```

---
## \#377 Posted by: scepterr Posted at: 2018-03-18T00:00:14.226Z Reads: 264

```
I'm pretty sure it not safe for whatever is powering through USB, just noticed an interesting behavior, I'm using a windows tablet, when using vesc tool to control motor, everything is fine until I apply brakes, then my touchscreen goes wonky for a few seconds where it touches all over when I touch it, then back to normal, only happens when applying brakes
```

---
## \#378 Posted by: stormboard1 Posted at: 2018-03-23T23:44:24.666Z Reads: 258

```
so whats the story with these i filled out the google doc but got no email back about them
```

---
## \#379 Posted by: bimmer Posted at: 2018-03-24T00:53:11.335Z Reads: 266

```
I made an initial batch. The SMD work I had done (by someone who should have done far better work) was sub par. I don't have the time nor really the expertise to make a larger batch here at home myself.
Since I absolutely want everyone to have a good product and a hassle free setup and ride I cannot with good conscience sell more completed boards at this time. 

Anyone who wants a bare PCB can contact me.

If we get enough people (like 20) I will make DIY kits with all components and documentation to do it yourself.

Hopefully soon we will be able to offer factory made PCB's that will be tested on a jig with a 300KV sensored motor spinning a weight.

Once the PCB's pass they will be assembled according to wishes I guess Single, Dual. Still doing research on acquiring the heatsinks. 

The current heatsink I use only covers 60% of 3 mosfets but so far running in a 12s5p setup I have had no heat related issues so I will sell them with this disclaimer.

I apologize to everyone who got their hopes up we would have a fast, cheap and reliable solution.

I have a 100% refund policy on everything I do and fix any Issue anyone has even if that means I lose money, I do this for the community but at this scale I poses to much risk as of now.

The DIY Kits will be your responsibility unless you come up short on parts there will be no refunds or returns once the first drop of solder has flown.
```

---
## \#380 Posted by: chickengun Posted at: 2018-03-24T00:57:05.464Z Reads: 258

```
I want a kit, I would actually take 4 of em ;) Can't wait :stuck_out_tongue_closed_eyes:
```

---
## \#381 Posted by: Hariboisawesome Posted at: 2018-03-24T02:07:53.110Z Reads: 258

```
I’m in for 2
```

---
## \#382 Posted by: E1Allen Posted at: 2018-03-24T02:11:36.686Z Reads: 265

```
@bimmer
I think it's awesome you took on the project to make these for everyone.  I think it's just as awesome that you recognized the issues with production and instead of sending issues down the line you owned them while still providing an option for people.  Nice work!
```

---
## \#383 Posted by: bimmer Posted at: 2018-03-24T02:16:21.384Z Reads: 275

```
I'll put together a groupbuy for the parts, all the SMD parts I had for these are currently in dispute as I refuse to pay for the joke of soldering work that was delivered and he has my parts.

Mouser and arrow are super fast with shipping so I can ship 7 days after I receive the payments.
```

---
## \#384 Posted by: bimmer Posted at: 2018-03-24T03:10:22.155Z Reads: 284

```
http://www.electric-skateboard.builders/t/b-box-kit-groupbuy/49972
```

---
## \#385 Posted by: Mobutusan Posted at: 2018-03-24T19:57:42.652Z Reads: 278

```
Next question is who has the time and expertise to buy these kits in bulk and assemble/sell them as complete units to the rest of us? If I'm not mistaken, @stewii is serving the EU and beyond with the ESCape and @Bimmer is trying to serve the US with the B-Box? I'm in for a couple complete units in the US, after the dust settles a bit, and I sell off some parts to fund these.
```

---
## \#386 Posted by: bimmer Posted at: 2018-03-24T20:27:45.977Z Reads: 286

```
There are complete kits coming but they will arrive assembled in the future.
```

---
## \#387 Posted by: pixelsilva Posted at: 2018-03-25T18:02:17.901Z Reads: 278

```
@bimmer, I plan to get two complete B-Box when you make them in the near future
```

---
## \#388 Posted by: Fabar Posted at: 2018-04-01T02:10:46.683Z Reads: 270

```
Would be great to get a couple of kits....  could you send us a mini tutorial how to upload the firmware... I would give a try to solder them if you can give a little help how to put everything together.. .
```

---
## \#389 Posted by: longhairedboy Posted at: 2018-04-06T13:47:03.863Z Reads: 261

```
Hello?

Where's my test unit?
```

---
## \#390 Posted by: Kubbur Posted at: 2018-07-11T16:57:48.496Z Reads: 199

```
Hey @bimmer what's the news on this project ?
```

---
## \#391 Posted by: JohnnyMeduse Posted at: 2018-07-11T16:59:55.061Z Reads: 208

```
Dead!!! 

That guys as move out... @stewii is the guys you need to contact 

https://www.electric-skateboard.builders/t/guys-it-has-been-great-bimmer-out/53298
```

---
## \#392 Posted by: ron Posted at: 2018-07-13T07:35:44.818Z Reads: 197

```
Hi there...

I wanted to print out the mid section for the case but I don't know where to get the CAD/STL File for that?! Does anyone who participated in this Group Buy have the 3D Cad files for the Mid Section?

Thanks in advance.

Greetings Ron
```

---
## \#393 Posted by: ron Posted at: 2018-07-31T08:43:24.394Z Reads: 180

```
Are there any of you who didn't received R12 ?! The only part missing in the Package Bimmer sent is the R12 15kOhm Resistor. Need to order this little piece of ...
```

---
## \#394 Posted by: b264 Posted at: 2018-07-31T09:10:08.446Z Reads: 176

```
Try Digikey, it will probably be $0.01 plus $5.00 shipping LoLz
```

---
## \#395 Posted by: Winfly Posted at: 2018-07-31T10:44:11.848Z Reads: 169

```
missing 2 whole kits from bimmer here
```

---
## \#396 Posted by: Dizzee Posted at: 2019-01-17T02:38:25.271Z Reads: 108

```
Could someone please tell where I can download a copy of the stencil file for this ESC?
```

---
## \#397 Posted by: banjaxxed Posted at: 2019-01-17T09:14:32.921Z Reads: 100

```
Same as stewii’s i can send it to you
```

---
## \#398 Posted by: Dizzee Posted at: 2019-01-26T04:42:40.171Z Reads: 80

```
@banjaxxed Thank you . I just sent you a DM.

I wish I thought of this earlier but does anyone have any stencils left over from this project that they would want to sell? I don't know if they can be reused but if they can used is fine with me.
```

---
