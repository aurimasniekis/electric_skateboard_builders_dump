# Cheap chargers with customizeable end-of-charge voltage

### Replies: 190 Views: 15405

## \#1 Posted by: whitepony Posted at: 2016-07-31T09:28:57.786Z Reads: 903

```
today I found something I looked for since quite a while: cheap notebook style chargers with customizeable end-of-charge voltage: http://www.groetech.de/index.php?main_page=index&cPath=5&zenid=ogh3dl0iql13c2edc1hn83jep1

the description is in german and basically says for most of those charger: there is a poti inside, that allows you to fine tune the end-of-charge voltage which is AWESOME for batteries without a bms.

if you check typical discharge curves, in this example from 2 very familiar cells:
http://abload.de/img/lginr18650hg2vssamsun8ppq8.png

you notice how the cells working interval appears to be probably around 3.3-4.0V, i.e. the small tip from 4.0 -> 4.2V doesnt hold too much capacity and below a certain voltage (probably really around 3.2-3.3V), the voltage also drops really fast (again not too much capacity in that area). 

now reducing your end-of-charge voltage has a 2-fold effect: firstly youll be able to prolong your battery life without much downside really  -> quoting batteryuniversity: _most Li-ions charge to 4.20V/cell, and every reduction in peak charge voltage of 0.10V/cell is said to double the cycle life. For example, a lithium-ion cell charged to 4.20V/cell typically delivers 300–500 cycles. If charged to only 4.10V/cell, the life can be prolonged to 600–1,000 cycles; 4.0V/cell should deliver 1,200–2,000 and 3.90V/cell should provide 2,400–4,000 cycles._

and secondly (and the reason why Im so keen on it): it allows you to essentially run without a BMS for a long time, because even though cells might or might not drift: the headroom for a drifting cell to reach a value beyond 4.2V or below 2.5V is quite large in a safe custom interval like 3.3-4.0V!

and you get these 2 things without much of a downside really - just some capacity loss, which, if you look at the plot, isnt a really big deal. sure, if you got very small batteries like 200Wh and less, you probably cant really afford lower end-of-charge, but people with 400Wh+ should consider it imo!
```

---
## \#2 Posted by: GhettoFab.rictation Posted at: 2016-07-31T09:45:12.260Z Reads: 741

```
I like this comment! Might change the way of charging 18650 's
```

---
## \#3 Posted by: Maxid Posted at: 2016-07-31T09:49:51.953Z Reads: 729

```
Nevermind my comment - just checked and my comment made no sense when you look at the charge currents.
```

---
## \#4 Posted by: whitepony Posted at: 2016-07-31T09:55:56.770Z Reads: 713

```
just wanted to comment and then you already edited it: kinda unfair to compare 4-5A chargers for 70€ with a 1A charger for 40€ :joy:

groetech also has a 1A charger for <40€
```

---
## \#5 Posted by: Maxid Posted at: 2016-07-31T09:57:13.193Z Reads: 663

```
Yeah just checked again and saw the same thing. Sorry for that - already edited my comment again but you were quicker this time :)
```

---
## \#6 Posted by: whitepony Posted at: 2016-07-31T10:00:17.126Z Reads: 635

```
groetech has also these smart BMS that can be customized - particularly interesting for me this one: http://www.groetech.de/index.php?main_page=product_info&products_id=265

if you configure it as balancing while idle, you can just stick it on a battery and after a few hours it will be balanced. if one of my 10S battery will ever show some drifing, Ill buy that module and just stick it on every now and then - no need to have it onboard. :slight_smile:
```

---
## \#7 Posted by: GhettoFab.rictation Posted at: 2016-07-31T10:25:19.357Z Reads: 601

```
I'm going to try and find 12s :open_mouth:
```

---
## \#8 Posted by: GhettoFab.rictation Posted at: 2016-07-31T10:26:21.291Z Reads: 582

```
http://www.groetech.de/index.php?main_page=product_info&cPath=26&products_id=427
```

---
## \#9 Posted by: GhettoFab.rictation Posted at: 2016-07-31T10:31:53.979Z Reads: 566

```
Shit check out the 12s4p for 339
```

---
## \#10 Posted by: Maxid Posted at: 2016-07-31T10:37:23.801Z Reads: 560

```
The base price is for US18650V3 cells however. They have a 10A discharge rate = not enough at 4P. Changing them to high discharge rate batteries costs 2€ per cell = you need to add 12*4*2€ = 96€ to make it ready for esk8s.
```

---
## \#11 Posted by: GhettoFab.rictation Posted at: 2016-07-31T10:40:54.160Z Reads: 543

```
Ah , so the 18650 batteries @barajabali built me are 20 amp? I know they are 12s4p  which would equal out to ten amp unless it's a different 18650 cell
```

---
## \#12 Posted by: Maxid Posted at: 2016-07-31T10:42:55.024Z Reads: 531

```
He is probably using samsung 25r with a 20A discharge rate.
```

---
## \#13 Posted by: GhettoFab.rictation Posted at: 2016-07-31T10:56:26.657Z Reads: 540

```
Check these out, pretty penny. https://batterybro.com/products/samsung-25r5-green-inr1865025r5-2500mah-20a
With this recommended from @whitepony  http://www.groetech.de/index.php?main_page=product_info&cPath=5&products_id=639
```

---
## \#14 Posted by: Randyc1 Posted at: 2016-08-01T14:36:13.625Z Reads: 523

```
Whitepony I have a 42v charger similar to your Evolve charger.
You mentioned yours charges to 41.4V I believe ?,...mine charges to 42.2 ...if i leave it to fully charge .
I wonder if i can modify it to charge to 41V ??
```

---
## \#15 Posted by: treenutter Posted at: 2016-08-01T14:47:50.632Z Reads: 520

```
Thanks for this writeup @whitepony ! I've looked a few times for configurable chargers and BMSs. Charging to 4.1V has the added benefit of reducing the risk of the full battery/regen shutoff that VESC is prone to. It looks like the BMS is configured at the factory and made to order, but the small chargers are user-configurable.

About the chargers (translated):
The final charge voltage can be adjusted at a potentiometer inside the unit to between about 40.5 and about 43.0 volts . If necessary, also to 46V , please inquire. Opening by removing the rubber pads of the feet . Caution : Such manipulations done but at their own risk , may be done only with appropriate expertise ; also voids the guarantee.
```

---
## \#16 Posted by: whitepony Posted at: 2016-08-04T19:37:59.482Z Reads: 522

```
my charger arrived, 4A 42V version for 70€ which I now "modded" to 40.5V!

basically you remove the rubber feet, open the 4 screws and youll find a small potentiometer, that was covered in some form of loctite to fixate it.

i then had my half empty spud battery and connected it - 4A charging is really fast - I quickly got to 40.5V and started dialing the potentiometer. apparantly you turn it right for lower cutoff and left for higher cutoff. I slowly dialed right until the charger led switched to green, unhooked battery again, hooked the charger up, it kept green. unhooed battery again, dialed cutoff a tiny fraction larger, hooked up battery and 5min later led switched from red to green, still at pretty much 40.5V.

then I covered the poti with some loctite and put the charger back together. 

Im really happy about this!! :grinning:

charger hooked up to battery, measuring voltage parallel, led just switched to green!
<img src="/uploads/db1493/original/2X/f/fa2931e3810c244b49f8be05793c7575a3684ce7.jpeg" width="513" height="500">

reapplied some loctite:
<img src="/uploads/db1493/original/2X/7/70f2b9ae884e1515db3235161da5943715ebf40a.jpeg" width="510" height="499">

manufacturer is "modiary", maybe someone finds it cheaper on alibaba or so:
<img src="/uploads/db1493/original/2X/1/1d100b1cd528afe00462c565116048b7c356b31b.jpeg" width="500" height="500">


p.s.: this seems to be the one I got: http://m.alibaba.com/product/60451408649/Electric-Tool-Lithium-Battery-Charger-42V.html
```

---
## \#17 Posted by: Randyc1 Posted at: 2016-08-04T22:58:48.046Z Reads: 474

```
That is great ,... my charger overcharges to 42.2 V so this is a great option !

Is 4A charging for your 10s4P ?


? Link does not mention Ajustable max Voltage ?
```

---
## \#18 Posted by: whitepony Posted at: 2016-08-05T04:01:32.000Z Reads: 482

```
[quote="Randyc1, post:17, topic:6902"]
Link does not mention Ajustable max Voltage ?
[/quote]

i assume its this one from alibaba after opening up the one I bought here: 
http://www.groetech.de/index.php?main_page=product_info&cPath=5&products_id=673

you cant really advertise it as "adjustable" imo. adjustable for the average joe consumer means there is a knob on the outside enclosure. this is more like a mod thats not meant to be, but possible because markus gröbe from groetech tried it out.

he is a superchilled guy btw, we talked for 30min over thw phone about batteries and he said that he has no bms in his batteries either. basically we gave each other mwntal high fives the whole time. :joy:
```

---
## \#19 Posted by: Randyc1 Posted at: 2016-08-05T04:16:32.703Z Reads: 463

```
Thanks bud !!,...makes me wonder if all chargers have a poti iside  for the manufacture to fine tune final  Vomtage ??

Think i will open mine just to check ??
```

---
## \#20 Posted by: VladPomogaev Posted at: 2016-08-05T04:21:21.426Z Reads: 458

```
Another method to charge your batteries (for bulk charging with BMS) is to buy a MeanWell (or Chinese ripoff power supply) and modify it by adding a potentiometer. It's sometimes called the R33 mod. Here's an old forum link: https://endless-sphere.com/forums/viewtopic.php?f=2&t=42793

I've done this with the Chinese clones; it's a different resistor but it works just as well.
```

---
## \#21 Posted by: whitepony Posted at: 2016-08-05T04:22:01.130Z Reads: 431

```
i checked my evolve charger already before ordering and it didnt. think its just a very lucky find by groetech!

that manufacturer seems to supply for pedelecs and hover boards. think it was just a cheap way for them to supply different end of charge states for different manufacturers of e-vehicles/tools. not everyone wants to charge to 42V, but insteads wants to increase lifetime!
```

---
## \#22 Posted by: Hummie Posted at: 2016-08-05T04:23:48.775Z Reads: 425

```
I have the meanwell 48volt and its adjustable without having to mod it.  Nice but finicky and for a couple more bucks there's better ones 

This is a nice one for the car

https://www.amazon.com/gp/aw/d/B016ZE6ADU/ref=mp_s_a_1_30?ie=UTF8&qid=1470370730&sr=8-30&pi=SX200_QL40&keywords=48v+charger&dpPl=1&dpID=41C-i5ZXQzL&ref=plSrch


But if u get a bulk charger it can't be for lead acid!!! Don't remember why.
```

---
## \#23 Posted by: VladPomogaev Posted at: 2016-08-05T04:26:20.479Z Reads: 410

```
Adjustable current as well? Usually the default current limit is ~130% of the rated power, and the PSU ends up getting fried without the mod.
```

---
## \#24 Posted by: Hummie Posted at: 2016-08-05T04:39:46.280Z Reads: 412

```
It has a potentiometer tiny screw that adjusts the voltage and the current follows.  It's been good and if it is pushed to its max of 400watts too long it slows down and I have to twist the little screw

Here's a whole slew of stuff from tiny to gigantic.  

All 48 about (12s)

http://www.trcelectronics.com/48-volt-power-supplies-chassis-6.shtml

How do cells respond to charging or discharging when they're in series and unbalanced?  Does it further distance them or suck more from the weaker?   I do the bulk charging and monitoring/balancing and have found stuff stays close a
```

---
## \#25 Posted by: VladPomogaev Posted at: 2016-08-05T04:56:37.644Z Reads: 394

```
Ah, that's the voltage control. Be careful with that. But then again, with a 400 watt power supply you might not need to worry about maxing it out haha. 

LiPo cells vary in both capacity and internal resistance, and both factors determine how much power is actually used from each cell. Meaning that it "distances them further" and does not "suck more from the weaker" in a series configuration. 

In a parallel configuration, the opposite is true. If one cell is a bit over discharged, the other cells will actually charge that cell, meaning it will "suck more from the weaker". There are more risks associated with parallel charging/discharging though.
```

---
## \#26 Posted by: Hummie Posted at: 2016-08-05T17:07:57.957Z Reads: 380

```
I'd thought parallel was safer in charging and discharging as any cells that were out of balance are not sucked from but leveled by the parallel cells.   No cell can get its voltage above or below its paralleled cells so no risk of it dropping too low or high 

In series since the current is forced through every cell I can imagine a cell with higher resistance will get warmer and maybe some energy that would be going into that cell is lost and unbalancing could happen that way but how could series cells become unbalanced.  And on discharge the higher resistance cell will get warmer and waste and maybe it snowballs...warmer increases resistance and less current can flow
```

---
## \#27 Posted by: VladPomogaev Posted at: 2016-08-05T19:17:12.292Z Reads: 379

```
What if one of your cells went kaput? Then all of your other cells would get drained, and they would go kaput as well. Tesla solves this problem by putting a fuse on each cell, and in case a cell accidentally shorts, the fuse blows, and saves the rest of the cells. I'm not saying it's unsafe, I've done it before, you just really need to understand the risks and proceed accordingly. 

That's pretty much how it works. The internal resistance introduces a voltage drop as well, which means that the cell won't get charged as much. And the same thing happens when you charge them.
```

---
## \#28 Posted by: Hummie Posted at: 2016-08-05T19:23:55.468Z Reads: 369

```
What does happen if one of ur parallel or series cells goes kaput?  
(Kaput being a state with low ability to hold a charge, greatly decreasing the energy it could hold, and if charged solo it would hit max charge and max discharge faster than a healthy cell)

My guess is...in a parallel arrangement all cells must have the same voltage so..yea all the cells in parallel would have their voltages dropping quick on discharge and raised quickly on charging.  Not dangerous but less of the parallel cells capacity would be usable even though all those cells would be good.  Safe but lame storage performance from pack 

In series..a kaput cell is going to be forced to low and high voltages and dangerous but won't decrease the pack performance really. 
What u think?
```

---
## \#29 Posted by: Eboostin Posted at: 2016-08-05T19:54:27.704Z Reads: 360

```
Have you measured the lowest voltage it will charge at?
```

---
## \#30 Posted by: VladPomogaev Posted at: 2016-08-05T20:48:36.275Z Reads: 379

```
[quote="Hummie, post:28, topic:6902"]
it could hold, and if charged solo it would hit max charge and max discharge faster than a healthy cell)
[/quote]

The cell could self-discharge itself and other cells that are connected in parallel. Honestly, we're kind-of going off topic now.
```

---
## \#31 Posted by: Hummie Posted at: 2016-08-06T01:20:40.870Z Reads: 392

```
Im back on topic. I do like to wander from topic though sorry. Here's my single cell lipo charger converted from my phone charger.  Just made it. Working.  I only had one low cell and balancing by discharging would've been a waste.  full voltage is 5.2 though so have to watch it. non-adjustable, but hoping someone can tell me how to adjust it.
<img src="/uploads/db1493/original/2X/2/2b9999e0fa2458ff52189ffce35c61f9415cf536.jpeg" width="375" height="500">
<img src="/uploads/db1493/original/2X/d/dfb41a573ef1660ef9a319efc5c12ee2a4fc5e0e.jpeg" width="375" height="500">
<img src="/uploads/db1493/original/2X/d/d3e65f3b389543eca21cf8f6640dce58bbeadf18.jpeg" width="666" height="500">
 since it charges at 5.2 and stated to charge 700ma and I'm connecting it to my battery at 3.2 volts will the current be more than if it was at 4.2?  current decreasing as the voltages get closer?     could you charge a single cell with a 50 volt charger if you decreased the amps a lot?  I'll have to figure the current with my multimeter.  I guess just switch to current. ....tried that and am reminded that my mulitmeter current meter is broken. probably by me

and why would anyone charge to 5.2?  I've seen a lot of odd higher numbers for phones.
```

---
## \#32 Posted by: VladPomogaev Posted at: 2016-08-06T02:07:30.301Z Reads: 375

```
Open it up and see what's inside. If there are any chips that look like this: <img src="/uploads/db1493/original/2X/5/51bf2cb2e06361444d26a3e08b9fd877ab33ab19.jpg" width="254" height="223">
that might be the control chip, and you might be able to Google the part number and see how the voltage is adjusted (usually via resistors). Then, you might be able to change the resistors to match 4.2v. Be careful!

Edit: Also, if the case is heat-sealed, you can pour gasoline (I'm not kidding here) into the crack, wait a bit, then it will open freely. Gasoline tends to weaken/eat through a lot of plastics.
```

---
## \#33 Posted by: Hummie Posted at: 2016-08-06T02:16:45.389Z Reads: 364

```
can i use the single cell charger at the same time as charging everything in series at the main leads to 50v?  i'm guessing yes but would like to be sure.

getting lazy i'll likely just find a 4.2 volt charger.  I dont have any resistors around.
```

---
## \#34 Posted by: kortho Posted at: 2016-08-06T18:21:02.596Z Reads: 357

```
@whitepony it seems the websites only option is in German, do the ship to the US or is there a way to get one of these chargers to the US?
```

---
## \#35 Posted by: whitepony Posted at: 2016-08-06T18:23:45.419Z Reads: 350

```
like I said, the manufacturer is modiary and I think its this charger: http://m.alibaba.com/product/60451408649/Electric-Tool-Lithium-Battery-Charger-42V.html

youll probably find it somewhere else too!
```

---
## \#36 Posted by: Titoxd10001 Posted at: 2016-08-06T21:01:27.880Z Reads: 355

```
Something like this would be nice because I want to go 11s
```

---
## \#37 Posted by: Randyc1 Posted at: 2016-08-11T14:08:58.155Z Reads: 359

```
Is the  Ajustable "Poti" in the middle picture the small Yellow knob  ??
```

---
## \#38 Posted by: whitepony Posted at: 2016-08-11T14:13:34.378Z Reads: 366

```
yea :slight_smile:
```

---
## \#39 Posted by: Michaelinvegas Posted at: 2016-08-11T18:02:29.416Z Reads: 372

```

DROK:

Numerical Control Voltage Regulator DC 8-60V to 10-120V 15A Boost Converter, Constant Voltage Current Step Up Module Adjustable Output 48V 24V 12V DC Power Supply with LED Display


https://www.amazon.com/dp/B01GFVI6R6/ref=cm_sw_r_cp_api_j3lRxb0CND1GD
```

---
## \#40 Posted by: Randyc1 Posted at: 2016-08-15T18:05:26.909Z Reads: 366

```
Have you tried a range test at 40.5 V to see the diffefence in range ?
```

---
## \#41 Posted by: whitepony Posted at: 2016-08-15T18:41:04.298Z Reads: 365

```
nope, didnt see the need for it, I rarely get below 34-35V on most of my tours. if you check hg2 discharge curves youll know that it cant be much im missing out on anyway:

https://cdn.shopify.com/s/files/1/0674/3651/files/hg2_dicharge_test_1.jpg
```

---
## \#42 Posted by: mason Posted at: 2016-08-24T01:59:31.261Z Reads: 342

```
sorry if this has been posted already, but has anyone seen [this?](https://www.amazon.com/dp/B01GFVI6R6/ref=wl_it_dp_o_pC_nS_ttl?_encoding=UTF8&colid=10VMT6ZFPJBQU&coliid=IYMFIWQBNESB1&psc=1) looks good for our usage.
```

---
## \#43 Posted by: Hummie Posted at: 2016-08-24T02:25:21.955Z Reads: 342

```
i saw that before but giving it a second look now it's pretty awesome.  The one big missing part to complete awesomeness would be rectifier so it could go in the wall and get ac.  otherwise all it's potential ...how can you get it?  I dont know much about rectifiers or maybe it needs an inverter i forget.  if anyone knows how to do it I'd like to get this.  huge output power beyond anything and also at 50.4 volts
```

---
## \#44 Posted by: Titoxd10001 Posted at: 2016-08-24T02:44:49.867Z Reads: 332

```
I've been eyeing this as well I think you just need a DC power supply with enough Amps and bellow the voltage you're charging to
```

---
## \#45 Posted by: Hummie Posted at: 2016-08-24T05:15:30.064Z Reads: 327

```
Is there something you've found that would be a good match?  A power supply that can do a lot to match this thing's possible output?  And cheap? Maybe not the full potential of this but 400watts at least
```

---
## \#46 Posted by: Titoxd10001 Posted at: 2016-08-24T05:43:46.648Z Reads: 320

```
I have two computer supply that I use for my power lab 6 that push can easily push 20 amps at 12v or 24v combined. I think one would suffice and i got them on sale both for like $50 on ebay
```

---
## \#47 Posted by: Randyc1 Posted at: 2016-08-27T02:41:12.826Z Reads: 307

```
In your comment you say charger can be ajusted between 40.5 and 43v .. then you go on saying also to 46V ??

Is there something other than the Potentiometer  that must be done to get to 46V ??
```

---
## \#48 Posted by: treenutter Posted at: 2016-08-27T02:50:06.886Z Reads: 305

```
@Randyc1 This isn't my text, it is text I translated from the website (originally in German) for everyone's reference. My interpretation is that the potentiometer alone can be adjusted adjust to modify the final voltage of the charger. The company states that you can reach 46V but you must "inquire" about how to do so.
```

---
## \#49 Posted by: Randyc1 Posted at: 2016-08-27T05:33:49.149Z Reads: 304

```
If we could find out how to get to 45V that would be great, we could potentially go to 11 S battery, if needed!

Wonder if whitepony can get the info from them since that is where he bought his ?
```

---
## \#50 Posted by: whitepony Posted at: 2016-08-27T05:41:14.798Z Reads: 300

```
i felt like that poti was adjustable only in a small bias area, 40.5V - 43V sounds reasonable, but i havent checked. also i wont check, cause I put a big blop of loctite to secure the poti position! :yum:

write the guy from groetec, he is a really nice guy who loved talking about batteries and everything around that! :slight_smile:
```

---
## \#51 Posted by: Randyc1 Posted at: 2016-08-27T05:43:19.928Z Reads: 300

```
Does he speak english ?

Ive bought 2 btw
```

---
## \#52 Posted by: Randyc1 Posted at: 2016-09-16T19:10:54.204Z Reads: 308

```
Just recieved 2 Modiary chargers, I had contacted the company,.. asked them about the End voltage Mod i wanted to do , and to my suprise, they Ajusted them for me to 41V !

Thanks for the tip Whitepony!
```

---
## \#53 Posted by: Randyc1 Posted at: 2016-09-16T20:51:14.423Z Reads: 308

```
Hmmm?,... it is charging to correct voltage but green light is not going on ?<img src="/uploads/db1493/original/3X/4/c/4cdc549321c4d26741f9c307344e78b9a6c70ab7.jpg" width="690" height="388">

Edit:...all good ,..green light just came on !!

Perfect!
```

---
## \#54 Posted by: Svenska Posted at: 2016-09-18T07:59:23.600Z Reads: 297

```
@Randyc1 Did you contact Modiary through Alibaba? I couldn't find anything with a reasonable amount of minimum orders. All are >20 pieces minimum order.
```

---
## \#55 Posted by: Randyc1 Posted at: 2016-09-18T13:24:44.390Z Reads: 295

```
Contact Modiary directly at  jock@modiary.com
```

---
## \#56 Posted by: mrpj Posted at: 2016-09-24T15:23:38.161Z Reads: 273

```
Thank you for the hint with the chargers, I was able to find the Mean Well MW CLG-150-48A for a quite low price [on ebay](http://www.ebay.de/itm/122109343069?_trksid=p2060353.m1438.l2649&ssPageName=STRK%3AMEBIDX%3AIT). Seller accepted my offer for 30 euros. 

According to a [topic in a german e-bike forum](http://www.pedelecforum.de/forum/index.php?threads/l%C3%A4dt-fast-alles-das-schaltnetzteil-mean-well-clg-150-48a.35759/) the voltage can be adjust as low as 39,62V - so it would be perfect for 10S+. It has max 3.5A so it`s not that fast with charging, but reasonable in my opinion

I am planning to build a custom 10S pack myself - yet quite unsure if it is really okay/safe to go the route without a bms. (but atleast would include the wiring for it, to rebalance maybe at some point later)
```

---
## \#57 Posted by: DeathCookies Posted at: 2016-09-27T08:47:31.500Z Reads: 272

```
Does anybody know **a reason why** this combination should **not** work to charge a battery **with bms**?

https://www.amazon.de/dp/B0191H4VF2/ref=wl_it_dp_o_pd_S_ttl
https://www.amazon.com/dp/B01GFVI6R6/ref=cm_sw_r_cp_api_j3lRxb0CND1GD
```

---
## \#58 Posted by: DeathCookies Posted at: 2016-09-29T07:04:15.966Z Reads: 254

```
No repsonse means that this is gonna work?
```

---
## \#59 Posted by: lowGuido Posted at: 2016-09-29T11:02:35.673Z Reads: 252

```
buy a supply that's already rated at the output you want instead of trying to up convert it.
```

---
## \#60 Posted by: DeathCookies Posted at: 2016-09-29T11:06:24.154Z Reads: 256

```
The idea is to have one charger for multiple boards with a good amperage rating.
It is inconvenient if you have a charger for 6S, 10S and 12S. (at least the price)

Edit: I also want to set my voltage to xS - 1V for longer battery life ;)
```

---
## \#61 Posted by: lowGuido Posted at: 2016-09-29T13:37:47.085Z Reads: 246

```
well then buy one that's rated for the highest voltage and down convert it rather than up convert. :)
```

---
## \#62 Posted by: Hummie Posted at: 2016-09-29T13:54:17.768Z Reads: 244

```
My Meanwell 48volt won't go down more than maybe ten volts.  Those two should go together but I've never heard of anyone doing it.   I forget the details that screen will show but with those bulk chargers they don't tell you what's going on and that drok thing seems good for that
```

---
## \#63 Posted by: mrpj Posted at: 2016-10-03T09:05:46.495Z Reads: 247

```
[quote="Hummie, post:62, topic:6902, full:true"]
My Meanwell 48volt won't go down more than maybe ten volts.  Those two should go together but I've never heard of anyone doing it.   I forget the details that screen will show but with those bulk chargers they don't tell you what's going on and that drok thing seems good for that
[/quote]

At whom was this directed?
```

---
## \#64 Posted by: Hummie Posted at: 2016-10-03T13:29:07.758Z Reads: 244

```
Deathcookies. He wants to get down to 6s
```

---
## \#65 Posted by: boards Posted at: 2016-10-03T15:57:12.344Z Reads: 243

```
Anybody who bought modiary willing to sell me an extra? @Randyc1
```

---
## \#66 Posted by: Randyc1 Posted at: 2016-10-03T17:39:14.312Z Reads: 234

```
Want dont you just contact Modiary, i put contact in an earlier post .
```

---
## \#67 Posted by: smurf Posted at: 2016-11-02T18:35:56.495Z Reads: 237

```
It's would be more efficient and more powerful at 24v or 36v going into the boost converter.
```

---
## \#68 Posted by: smurf Posted at: 2016-11-02T18:48:00.002Z Reads: 237

```
The real question is how do you remove and  surface mount the display board into a project box?
```

---
## \#69 Posted by: jmasta Posted at: 2016-11-02T19:09:13.811Z Reads: 241

```
It looks to me like the LCD PCB on the regulator is just a shield.  You can see a row of pins on each side.  I bet you could just pull off the LCD shield and reconnect with wires
```

---
## \#70 Posted by: smurf Posted at: 2016-11-02T20:07:36.426Z Reads: 242

```
I'm new to hardware hacking and I really don't want to undertake a project like this.
Sense no one else is doing it first I guess I'll have to take one for the team.
```

---
## \#71 Posted by: SageTX Posted at: 2016-11-02T20:23:35.526Z Reads: 237

```
I'm  rooting for ya. I bought one of those dc-dc converters so I can charge directly from my truck batteries.  I want to put it in some sort of box so it'll travel easier.   

Keep us updated!
```

---
## \#72 Posted by: smurf Posted at: 2016-11-02T20:32:00.818Z Reads: 238

```
I'm thinking using this one

http://www.banggood.com/600W-Digital-Control-DC-DC-Adjustable-Step-Up-Module-Constant-Voltage-Current-Solar-Charging-p-1082316.html?rmmds=category

If I F it up I'm not out as much money and 10 amp's should be plenty
```

---
## \#73 Posted by: Maxid Posted at: 2016-11-02T20:57:20.284Z Reads: 242

```
this would make it easier for you to put in a box nicely:
http://www.banggood.com/DP50V5A-Buck-Adjustable-DC-Power-Supply-Module-With-Integrated-Voltmeter-Ammeter-Color-Display-p-1050061.html?rmmds=category
```

---
## \#74 Posted by: jmasta Posted at: 2016-11-02T21:08:13.562Z Reads: 233

```
That last one is a step-down regulator. So you have to over-supply voltage by 5-10%
```

---
## \#75 Posted by: Maxid Posted at: 2016-11-02T21:10:43.313Z Reads: 241

```
oh - didn't realize. thanks for noticing :thumbsup:
```

---
## \#76 Posted by: DeathCookies Posted at: 2016-11-02T21:29:22.913Z Reads: 249

```
I wanted to switch from LiPo to LiIon and therefor i have planned to use this combo since a while:
Power Supply
https://www.amazon.de/gp/product/B0191H4VF2/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
Charger
https://www.amazon.de/dp/B01E8LJVHO/ref=wl_it_dp_o_pd_S_ttl?_encoding=UTF8&colid=17BENO76NCTU&coliid=I36V1SPFFRSVHX&psc=1

Plan: no BMS like it should be @whitepony
Just take care of enough P's in the batteries to keep the cells evenly balanced and less drain and also keep the voltage in a healty level.
```

---
## \#77 Posted by: smurf Posted at: 2016-11-02T21:48:30.310Z Reads: 243

```
If your going to use 12 volt use a standard PC power supply cheap if not free

https://youtube.com/watch?v=O1z0pyGWCAQ
```

---
## \#78 Posted by: DeathCookies Posted at: 2016-11-02T21:59:36.130Z Reads: 241

```
A PC power supply is kinda bulky... I want it to be as small as possible and i somehow trust these newer 3d printer power supplys to deliver a decent energy. Therefore i will try this combo.

This combo could be merged with a 3d printed enclosure nicely
```

---
## \#79 Posted by: smurf Posted at: 2016-11-02T22:11:31.674Z Reads: 234

```
I'm planning on just using it for 10s-14s
So a 36 volt psu is more efficient for me.
I can get 4 units from China for less money than one that is already here in the states.

https://m.alibaba.com/product/60528992371/Meanwell-EPP-400-36-dc-36v.html?spm=a2706.7843667.1998817009.85.g8Bb6w

I feel that I have a trust problem with cheap Chinese electronics
```

---
## \#80 Posted by: jmasta Posted at: 2016-11-03T02:34:43.414Z Reads: 231

```
If you decide to make one of these, you will probably need to add a transistor to prevent backflow into the voltage regulator.  When I was researching this last week, a lot of the voltage regulators required one if you are going to be charging batteries.  Some even include the transistor
```

---
## \#81 Posted by: smurf Posted at: 2016-11-03T03:13:25.926Z Reads: 232

```
Now that you say something I think I remember hearing that somewhere.

If I had to guess this is the right thing to connect the LCD shield to the main board.

https://www.amazon.com/Elegoo-120pcs-Multicolored-Breadboard-arduino/dp/B01EV70C78/ref=pd_rhf_eeolp_s_cp_1?ie=UTF8&pd_rd_i=B01EV70C78&pd_rd_r=XGNY6TGS0HFR5YCD2DB9&pd_rd_w=9wnhk&pd_rd_wg=jbjSH&psc=1&refRID=XGNY6TGS0HFR5YCD2DB9
```

---
## \#82 Posted by: smurf Posted at: 2016-11-05T08:03:43.110Z Reads: 230

```
This is the psu I'm going to use now I just need to find a vendor

http://www.meanwellusa.com/productPdf.aspx?i=716
```

---
## \#83 Posted by: smurf Posted at: 2016-11-05T08:33:47.843Z Reads: 235

```
https://m.youtube.com/watch?v=0Z5QWzSSvdI
```

---
## \#84 Posted by: 2-alex-2 Posted at: 2016-11-05T09:45:01.122Z Reads: 228

```
Anyone have a link for a good 6s 25v 4amp charger Eu preferably.
```

---
## \#85 Posted by: SageTX Posted at: 2016-11-05T20:35:30.338Z Reads: 220

```
That video is why i bought that charger / converter.  Just waiting for your case mod! :yum:
```

---
## \#86 Posted by: smurf Posted at: 2016-11-05T21:31:09.749Z Reads: 219

```
Have you used it yet?
```

---
## \#87 Posted by: SageTX Posted at: 2016-11-05T21:38:00.619Z Reads: 220

```
No.  Board not built yet.  It's actually still sitting in the mailbox.
```

---
## \#88 Posted by: smurf Posted at: 2016-11-06T20:57:10.339Z Reads: 224

```
http://m.ebay.com/itm/111974443418?_trksid=p2057872.m2749.l2649&_mwBanner=1
```

---
## \#89 Posted by: smurf Posted at: 2016-11-08T18:32:03.161Z Reads: 227

```
Instructions for the drok
https://www.dropbox.com/s/gp7rxnjk8tkns2x/200150%20Instruction.pdf?dl=0
```

---
## \#90 Posted by: smurf Posted at: 2016-11-08T20:03:50.820Z Reads: 229

```
https://www.instagram.com/p/BMj9Xmrj3rC/

The little LCD shied definitely comes off
```

---
## \#91 Posted by: smurf Posted at: 2016-11-08T21:41:26.584Z Reads: 229

```
Unless someone has a better idea I'm stuck with this guy as a example

https://m.youtube.com/watch?v=E4lyVt3w0rk
```

---
## \#92 Posted by: Okami Posted at: 2016-11-18T23:50:05.078Z Reads: 224

```
Have you figured it out? 

I'd also like to build a ''step - up'' charger.. My only concern now is that I need a model which has ''constant current''.. too bad the cheap / weaks ones dont have current regulation.. have to search for some more models probably as Im not sure how to add current control diy style..
```

---
## \#93 Posted by: Maxid Posted at: 2016-11-19T00:54:22.382Z Reads: 219

```
Just get the drok - seems priced pretty competitively.
```

---
## \#94 Posted by: Okami Posted at: 2016-11-19T09:48:44.857Z Reads: 224

```
Seems quite bulky.. And I would probably need 200-300w max for now. (max 8A)

Probably will check the vids, perhaps I get the answer if there is an easy solution for adding contstant current to a power supply / step-up converter. 

-----
So far it seems that the current is regulated with micro controller. It has a shunt = current meter somewhere and it just tries to hold the current in the same place by varying the voltage (as there is voltage drop, the current is depending from supplied voltage, too, it seems. Not sure about the internal mechanics but this is the ''basic'' explanation I got from the net.

----

Second Option is to get this:

http://www.ebay.com/itm/DC-10A-CV-Constant-Current-Step-Down-Regulator-LED-Power-Supply-Battery-Charger-/191939041118?hash=item2cb075575e:g:QwMAAOSwbsBXpI~e

Or

http://www.ebay.com/itm/LED-Voltage-Current-Regulator-DC-DC-Step-Down-Power-Supply-Module-Converter-M6G5-/162115196074?var=&hash=item25bed194aa:m:mF6mQ_6HQi5S5Pqa6AFk9jg

--

These are step down.. So I might just get higher voltage and then buck it down to the desired amount.
```

---
## \#95 Posted by: smurf Posted at: 2016-11-19T18:06:52.982Z Reads: 210

```
http://www.ebay.com/itm/252435551262
```

---
## \#96 Posted by: Okami Posted at: 2016-11-19T18:56:58.802Z Reads: 201

```
120v is quite a lot.. Though, I think it is somewhat good alternative to the ''Drok'' module. (also good feature, that it has fan installed already)
```

---
## \#97 Posted by: smurf Posted at: 2016-11-19T19:24:24.546Z Reads: 205

```
No there is not a easy solution for adding constant current constant voltage to a power supply. But this is the microcontroller
http://www.jameco.com/z/LT1339CSW-PBF-Linear-Technology-DC-Controller-Single-Output-Synchronous-Buck-9-Volt-to-60-Volt-20-Pin-SOIC-W_1734436.html
```

---
## \#98 Posted by: Okami Posted at: 2016-11-19T19:43:00.855Z Reads: 215

```
Yeah, it is easier to just buy a module which has it.. 

Though, I found out the correct term is - 

''current limiter''

Current limiting = allow any current to flow to the load, from 0 up to the set current level limit.

See this:

http://forum.arduino.cc/index.php?topic=70739.0

It seems that constant current might be bad, if it is not limited, as it would ''force'' the current into the battery even if it is not needed to be so high anymore - like at the end of the charge.

Though, I assume not all people will charge their batteries to the max with such ''bulk'' power supply option.. at least I dont intend to do so.. :D
```

---
## \#99 Posted by: smurf Posted at: 2016-11-19T19:58:28.109Z Reads: 215

```

Acronym

Definition

CCCV Constant current, constant voltage (recommended method for charging lithium ion and lithium polymer rechargeable batteries)

http://liionbms.com/php/wp_cccv_charging.php

A side effect of using a BMS is that you no longer have to have a regulated charger: any charger will do, even a "brute force" charger, as long as the BMS can turn it on and off.
```

---
## \#100 Posted by: Okami Posted at: 2016-11-19T21:17:18.759Z Reads: 217

```
Yeah, charging with bms is a lot different story..

I was referring to just bulk charging and then balancing / checking the cells after that..

Though, if something fails in such scenario while charging things probably might go bad, too!.. (bulk charger, no circuits in place to stop the charge if one of the parallel pack's go bad)

---

Might just choose a bms for charging only, as the amp rates wont be that high then.. Ive heard ppl doing it.
```

---
## \#101 Posted by: Hummie Posted at: 2016-11-20T03:10:31.934Z Reads: 220

```
<img src="/uploads/db1493/original/3X/5/f/5fa1301e913176820e100a18e8916ee911d4c8d3.png" width="333" height="500">_`> emphasized text`_I read the cccv link

All the complications of te conversion why not just get a single cccv power supply at meanwell

This is pretty much a stick on bms 
:https://hobbyking.com/en_us/turnigy-dlux-lipo-battery-cell-display-and-balancer-2s-6s.html

But it's not that good. I put it up because it's so small and nicer looking than the others I have. It doesn't balance quickly either and will shut off from overheat.  I wish someone would make a better one.  Or link me again to a guide to making one.  Simple circuit I'm pretty sure
```

---
## \#102 Posted by: Maxid Posted at: 2016-11-21T07:50:27.332Z Reads: 204

```
Just to let the Germans know:
I bought the Drok in the current (I think only valid for today) 20%-off Amazon warehouse deals special.
Cost me 17€ including shipping.

@DeathCookies: if you have not already ordered now is the time ;)

Also I contacted Modiary to get an estimate on their 4A charger. Is there any interest? Then it might make sense to order a couple instead of just one.
```

---
## \#103 Posted by: Maxid Posted at: 2016-11-21T08:47:01.979Z Reads: 208

```
The modiary 4A charger with endvoltage set to 41V can be bought for 23USD. However shipping is 25USD for one or 31 for two. Does anyone want to share an order?

Please keep in mind that these prices are without european VAT and also without that hefty 12€ DHL express fee.

In a worst case scenario it would look something like this:

Fo two people without forward postage:
(2x23USD+31USD)*1.19+12EUR=98 or 49EUR per person plus postage

For three:
(3x23USD+31USD)*1.19+12EUR=124EUR or 41EUR per person plus postage

Edit: European shipping is expensive - wow I did not know.
DHL charges between 8.89€ (no tracking, no insurance) up to 11.09€ (tracking and 50€ insurance). Hermes charges 9.79€.
```

---
## \#104 Posted by: jujet Posted at: 2016-11-21T09:34:43.773Z Reads: 199

```
I'm interested in getting one
```

---
## \#105 Posted by: rmrf Posted at: 2016-11-21T10:14:48.903Z Reads: 200

```
I also want one (Sweden)
```

---
## \#106 Posted by: Maxx Posted at: 2016-11-21T16:59:05.883Z Reads: 206

```
[quote="Maxid, post:102, topic:6902, full:true"]
Just to let the Germans know:
I bought the Drok in the current (I think only valid for today) 20%-off Amazon warehouse deals special.
Cost me 17€ including shipping.
[/quote]

You got a link to that one? The 20% special should last the whole week...
```

---
## \#107 Posted by: Maxid Posted at: 2016-11-21T17:00:42.959Z Reads: 207

```
https://www.amazon.de/gp/offer-listing/B01E8LJVHO/ref=sr_1_1_olp?s=lighting&ie=UTF8&qid=1479747580&sr=8-1&keywords=Yeeco+Einstellbare+8-60V+bis+10-120V+15A+DC+DC+Numerical+Control+Step+up-Boost-Converter+Voltage+Regulator+Booster+Board+Solar-Lade&condition=used

I added the cheapest warehouse deal book I could find to get "free" shipping (well it cost me 76ct - but better than 4€ ;))
```

---
## \#108 Posted by: smurf Posted at: 2016-12-02T21:31:30.449Z Reads: 205

```
https://www.instagram.com/p/BNh6IlUj1mQ/

Now I just have to get it in the box
```

---
## \#109 Posted by: Maxid Posted at: 2016-12-02T22:00:20.190Z Reads: 196

```
what power supply is that? I had the same idea but settled for a 65W 24V laptop style psu - the case is 3D printing now :)
```

---
## \#110 Posted by: smurf Posted at: 2016-12-02T22:26:51.015Z Reads: 203

```
http://www.meanwell.com/webapp/product/search.aspx?prod=EPP-400

https://www.eltech.spb.ru/ckfinder/userfiles/images/EPP-400%201.PNG
```

---
## \#111 Posted by: Okami Posted at: 2016-12-03T12:45:57.652Z Reads: 197

```
At what amps / voltage will you charge? Just want to know how much Watts will you pull from this :)
```

---
## \#112 Posted by: SageTX Posted at: 2016-12-03T16:40:06.502Z Reads: 194

```
Whoah!   Amazing progress.  Did you modify a PC Power supply?

NVM... Didn;t Scroll far enough. :(
```

---
## \#113 Posted by: smurf Posted at: 2016-12-03T21:36:13.342Z Reads: 193

```
That's the right question.
The psu will output 250 watts w/o active cooling and 400 @ 25 cfm
I was thinking about keeping it under 300 watts and see how hot it gets with a quiet fan. But it should push 42v 8a or 50v 7a safely
```

---
## \#114 Posted by: Maxid Posted at: 2016-12-03T21:47:40.435Z Reads: 192

```
That would be more than 300W out of the Drok - be careful and also check your mosfet and diode. Some folks on endless-sphere said that they are way underspecced and different parts are used on individual Droks (basically they use whatever cheap leftover parts they can find).
https://endless-sphere.com/forums/viewtopic.php?f=14&t=82731&start=0
```

---
## \#115 Posted by: smurf Posted at: 2016-12-03T22:12:12.949Z Reads: 201

```
https://www.instagram.com/p/BNkkA4Yjjns/

As far as I can tell everything is rated 150V or 200V
```

---
## \#116 Posted by: Maxid Posted at: 2016-12-05T16:37:23.171Z Reads: 201

```
Came out pretty nicely I'd say:
<img src="/uploads/db1493/original/3X/b/c/bc6f033a6cc7177ab2bad10feb5e2fe601679780.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/1/a12aac8ee90f935558c2f93d0e759a0e57444487.jpg" width="375" height="500">
```

---
## \#117 Posted by: Okami Posted at: 2016-12-05T16:39:16.723Z Reads: 200

```
Nice box.. I assume you've got quite a good 3d printer print area but I think you could improve even further.. find some pushbutton caps and add a little glass / acrylic.. this way it will look even more professional and finished ;)

Though, all is up to you.. Would probably leave it the way it is, if it was mine :D unless something were falling out or debris / dust would accumulate too much through the openings..

http://www.ebay.com/itm/10pcs-Momentary-Tact-Tactile-Push-Button-Switch-4-Pin-w-Cap-DT-/252405592335

http://www.ebay.com/itm/20-Pcs-6x6x12mm-Momentary-4pin-Push-Button-Micro-Tactile-Tact-Switch-w-Cap-/321905725517
```

---
## \#118 Posted by: Hummie Posted at: 2016-12-05T16:50:35.326Z Reads: 189

```
What's the practical benefit of getting something like this instead of just a power supply at your battery's voltage? I won't change my voltage in or out and now use a meanwell power supply that does 400 watts at 50 volts, am I missing out without this? Does this have an integrated power supply?
```

---
## \#119 Posted by: Maxid Posted at: 2016-12-05T17:00:24.083Z Reads: 186

```
I put a DROK together with a small meanwell 65W power supply in a 3D printed case. This gives me a cheap (~30€) 41V 1.5A charger plus the freedom to change end-voltage to whatever I want - also it is fun and feels like DIY.
```

---
## \#120 Posted by: smurf Posted at: 2016-12-05T20:10:04.487Z Reads: 192

```
How did you mount the display to the lid ?
```

---
## \#121 Posted by: Maxid Posted at: 2016-12-05T22:30:55.192Z Reads: 190

```
I just put some headers on top of each other. Basically it is still just "standing" in its previous headers - but higher up.
```

---
## \#122 Posted by: jmasta Posted at: 2016-12-05T23:16:55.959Z Reads: 193

```
[quote="Hummie, post:118, topic:6902, full:true"]
What's the practical benefit of getting something like this instead of just a power supply at your battery's voltage? I won't change my voltage in or out and now use a meanwell power supply that does 400 watts at 50 volts, am I missing out without this? Does this have an integrated power supply?
[/quote]

1) First and foremost.. It let's you customize end-of-charge voltage**.  So you could charge your cells to, say, 4.15V instead of 4.20V.  Also lets you charge any series configuration with a single charger (9S, 10S, 12S, etc)

2) It's possible to build a 4+ amp charging system for less than the price of an equivalent charger.  For example, a 12S 4A charger on eBay was something like $85 after shipping from China.  Also, the system can be made from "Amazon-ready" parts. So if you're in the US, you could have your parts in 2 days, rather than a month

3) DIY or bust! ;)

**Note:  The voltage on most of the fixed-voltage PSU's can be tuned slightly.  There is usually a small potentiometer inside the case that let's you adjust from, for example, 50.4 (4.20V/cell) to 49.9 (4.16V/cell)
```

---
## \#123 Posted by: Hummie Posted at: 2016-12-05T23:28:16.932Z Reads: 192

```
All makes sense to me except number 2. I think what you'd be making would be a power source and not a balance charger no?  Why not just get a bulk charger that will do 8 amps at 50 volts for 60$. And its somewhat adjustable to different voltages
```

---
## \#124 Posted by: jmasta Posted at: 2016-12-06T00:45:04.014Z Reads: 197

```
[quote="Hummie, post:123, topic:6902, full:true"]
All makes sense to me except number 2. I think what you'd be making would be a power source and not a balance charger no?  Why not just get a bulk charger that will do 8 amps at 50 volts for 60$. And its somewhat adjustable to different voltages
[/quote]

Yeah it's not a balance charger. You still need a BMS.  It is basically just a Constant-Current / Constant-Voltage power supply with easily adjustable user-specified outputs. The DROK regulator has numerical control for the voltage and current, so you can accurately and reliably change the output with a few button presses, instead of turning a tiny screw on a potentiometer.

That said, I decided to stick with a 2A fixed-voltage laptop-style charger (~$35 plus a month wait from China). I personally don't need a variable voltage PSU at moment.  And even though it takes longer, charging at a slower rate is better for the battery
```

---
## \#125 Posted by: ToMiCcc Posted at: 2016-12-17T16:58:36.742Z Reads: 176

```
You could just get any kind of DC power supply (lap top bricks would work to) and hook it up to a digital dc-dc boost converter... And you got ur self adjustable (current and voltage) charger for less then 25$ 
Very nice stuff for charging everything u have in house... Adjustable voltage and current is realy helpful sometimes
```

---
## \#126 Posted by: DreadBiscuit Posted at: 2017-01-12T16:01:12.221Z Reads: 184

```
I am not that electronic savvy.  I have a Genssi 36V PS I wanted to do the "R33" mod on.  I opened it, read posts, but I have no idea how to track down the correct resistor to add a POTI to.  I adjusted the supply down to the required 33.6V (max of 4.2V per cell for 8S).  I would like to get a maximum of 4.5 A out of the supply to go into my BMS and battery pack.  BMS is rated at 5A for charging. 

 Using Ohm's Law: 
V=IR >> V/I=R              33.6V/4.5A = 7.4666Ohms  
Therefore, couldn't I just put a large 8ohm high-wattage resistor coming out of the negative terminal on the supply which would limit the maximum current to around 4.2 A (using ohms law again...33.6V/8ohms = 4.2A)?  This would limit what the BMS draws from the supply and the BMS would do all the balancing of my battery....right?  Right?!?!  :disappointed_relieved:

**Edit - I want to use the existing PS since I already opened it and voided being able to send it back...
```

---
## \#127 Posted by: smurf Posted at: 2017-01-14T17:08:33.604Z Reads: 188

```
http://www.circuitdiagramworld.com/uploads/allimg/201411/Variable-Power-Supply-0-24V-circuit.jpg

The resistor close to the positive output will control current
```

---
## \#128 Posted by: Paulf Posted at: 2017-01-19T14:29:32.964Z Reads: 190

```
I do have this charger http://www.ebay.ca/itm/361851978526
The only problem with it is that it overcharges my battery up to 42.7V
I've opened it but there doesn't seem to be any potentiometer in it... 
Has anyone already dealt with this charger? Is there a resistor I can change in order to adjust the final voltage?
If it helps, i can upload pics of the inside of the charger...
```

---
## \#129 Posted by: Jinra Posted at: 2017-05-09T03:57:42.349Z Reads: 179

```
Anyone EE's here have any idea on what I may need to do to adjust the output voltage on my charger? I'm guessing I mess with one of the 3 potentiometers in the pic?

<img src="/uploads/db1493/original/3X/4/a/4a72a6ab8ca347a6ecbd3fb970a4b8ebda66dc8e.jpg" width="666" height="500">

EDIT: found out the upper right potentiometer changes voltage, not sure what the other two do though.

If you have an Enertion fast charger or charger with similar circuit board layout, FYI!
```

---
## \#130 Posted by: Conor Posted at: 2017-05-20T05:19:58.151Z Reads: 167

```
[quote="Maxid, post:119, topic:6902, full:true"]
I put a DROK together with a small meanwell 65W power supply in a 3D printed case. This gives me a cheap (~30€) 41V 1.5A charger plus the freedom to change end-voltage to whatever I want - also it is fun and feels like DIY.
[/quote]

Can I get The link to your 65w power supply?
```

---
## \#131 Posted by: Maxid Posted at: 2017-05-20T05:24:30.267Z Reads: 162

```
I used an old laptop psu - don't have a link sorry. I upgraded to a 90W Lenovo one now which fit even better
```

---
## \#132 Posted by: Conor Posted at: 2017-05-20T05:26:11.023Z Reads: 159

```
link to new one? also thanks for the insanely fast reply!
```

---
## \#133 Posted by: Maxid Posted at: 2017-05-20T05:32:57.623Z Reads: 157

```
Again: had that lying around and have no link. It is also not factored into the price as I figured everybody has an old laptop PSU somewhere.
```

---
## \#134 Posted by: Conor Posted at: 2017-05-20T05:54:20.530Z Reads: 152

```
one last thing - about how long does a full charge take with the drok and your laptop psu?
```

---
## \#135 Posted by: Maxid Posted at: 2017-05-20T06:05:49.006Z Reads: 148

```
All depends on charge current and battery capacity. With 90W I can charge my 10S battery at ~2A. Now divide your capacity by 2A and you'll have the time it takes
```

---
## \#136 Posted by: Conor Posted at: 2017-05-20T06:45:02.141Z Reads: 155

```
Can you explain how you wired the laptop psu to the drok
```

---
## \#137 Posted by: Maxid Posted at: 2017-05-20T07:34:02.942Z Reads: 151

```
It's a DC psu - you just connect GND and POS to the corresponding input on the Drok.
```

---
## \#138 Posted by: Jebe Posted at: 2017-05-20T07:48:06.537Z Reads: 154

```
something like this ?
http://www.ebay.com.au/itm/DC-DC-Converter-Module-Adjustable-Step-Up-Boost-Power-Supply-DC8-5V-48V-Input-GL-/282146588265?hash=item41b13f4669:g:FJIAAOSw9NdXu9ES
```

---
## \#139 Posted by: Maxid Posted at: 2017-05-20T07:54:02.438Z Reads: 155

```
that one should work in principle though setting the voltage is a PITA with those potentiometers. I'd try and get one with digital settings
```

---
## \#140 Posted by: Conor Posted at: 2017-05-20T07:54:32.372Z Reads: 154

```
[quote="Maxid, post:137, topic:6902, full:true"]
It's a DC psu - you just connect GND and POS to the corresponding input on the Drok
[/quote]

So you need some kind of DC splitter adapter?
```

---
## \#141 Posted by: Jebe Posted at: 2017-05-20T07:55:54.639Z Reads: 153

```
I'd double check it with my fluke and dc clamp as well.
what about this one. 
http://www.ebay.com.au/itm/150W-DC-DC-Boost-Converter-12-32V-to-12-46V-Step-Up-Voltage-Charger-Module-GO-/371474451566?hash=item567d9a4c6e:g:y18AAOSwo0JWMM36

Bought it - will post a review
```

---
## \#142 Posted by: Maxid Posted at: 2017-05-20T08:07:31.628Z Reads: 153

```
What? Your PSU outputs DC voltage (which only has two wires GND and POS) that you hook up to the Drok. Can't get simpler than that. If you don't feel comfortable with that you should probably not start fiddling around with electricity in the first place.
```

---
## \#143 Posted by: Conor Posted at: 2017-05-20T08:14:23.009Z Reads: 152

```
I am bad at visualizing it would be very helpful if you could post some pictures of your wiring setup thx
```

---
## \#144 Posted by: Maxid Posted at: 2017-05-20T08:20:51.254Z Reads: 160

```
<img src="/uploads/db1493/original/3X/3/4/3417b1b0013e1f621d7226d808eb3a30c1ab908a.jpg" width="375" height="500">
```

---
## \#145 Posted by: Conor Posted at: 2017-05-20T16:28:59.505Z Reads: 157

```
How could I plug this into the drok as input? <img src="/uploads/db1493/original/3X/a/0/a04ab94c66894ea5901cf59cab539e56ec01f78c.jpg" width="281" height="500">
```

---
## \#146 Posted by: Maxid Posted at: 2017-05-20T16:49:57.634Z Reads: 151

```
You cut the plug off
```

---
## \#147 Posted by: smurf Posted at: 2017-05-20T17:03:06.740Z Reads: 155

```
http://www.allelectronics.com/item/dcj-21/2.1mm-coax-power-jack-panel-mount/1.html
```

---
## \#148 Posted by: Conor Posted at: 2017-05-27T06:11:49.719Z Reads: 152

```
How do you know when it is fully charged?
```

---
## \#149 Posted by: Maxid Posted at: 2017-05-27T08:35:29.705Z Reads: 150

```
The charge current drops
```

---
## \#150 Posted by: Conor Posted at: 2017-06-15T21:55:37.835Z Reads: 145

```
So how do you balance all the cells? Or do you need a BMS?
```

---
## \#151 Posted by: Maxid Posted at: 2017-06-15T22:08:55.923Z Reads: 149

```
I don't balance and don't have a BMS. This can be done with quality cells
```

---
## \#152 Posted by: Conor Posted at: 2017-06-15T23:22:23.094Z Reads: 144

```
I am trying to charge a 3s lipo but when I plug it in to the output my drok just turns on then off then on...
```

---
## \#153 Posted by: sl33py Posted at: 2017-06-16T02:59:50.560Z Reads: 150

```
[quote="Conor, post:152, topic:6902, full:true"]
I am trying to charge a 3s lipo but when I plug it in to the output my drok just turns on then off then on...
[/quote]

@Conor - this is going to come across a little harsh, but bear with me a sec.

**_STOP F&#*KING WITH A DROK AND LIPOS - YOU ARE GOING TO BURN YOUR F*#&KING HOUSE DOWN!_**

I'm not kidding.  STOP.  You should not do anything with bare wires or electricity that is not a store purchased power supply/charger with UL listing on it.  And keep it sealed!!!

Slow down a bit, get a reputable charger and balance charge.  Literally plugging a 3s lipo into anything electronic and wondering why it "just turns on then off then on..." is seriously a recipe to hurt yourself, or your house, or your entire apartment complex/neighborhood.  

"News at 9 - guy caught his house on fire trying to charge an electric skateboard.  Next up legislation to ban these dangerous electric skateboards from all public areas..."

**Keep reading, keep learning, and keep asking questions, but you should slow down a bit until you understand how to SAFELY handle electronics with high voltage and amperage.**

again - dickish - sorry, but **_you can truly hurt yourself or others_** if you don't have an idea of what you are doing.  STOP.  Please.

Rob
```

---
## \#154 Posted by: Conor Posted at: 2017-06-16T03:29:19.582Z Reads: 140

```
lol k. Anyways I figured out why it wasn't working my power supply wasn't set to output enough volts
```

---
## \#155 Posted by: smurf Posted at: 2017-06-16T03:36:46.195Z Reads: 141

```
What kind of power supply do you have?
```

---
## \#156 Posted by: Conor Posted at: 2017-06-16T04:55:56.901Z Reads: 138

```
12v-24v rc power supply
```

---
## \#157 Posted by: Maxid Posted at: 2017-06-16T07:24:36.745Z Reads: 143

```
Actually the drok can only boost voltage.
If you set your power supply to 24V the Drok is not able to reduce this to the necessary 3S voltage.
Also NEVER charge a LIpo with just a Drok. Lipos are not quality cells and need to be balanced every time.

I hope your house is not already burning
```

---
## \#158 Posted by: jbruce Posted at: 2017-07-31T09:57:48.214Z Reads: 139

```
I've recently been able to get in contact with modiary who sell the 10s 4A variable end of charge voltage chargers and the agent had confirmed it has the variable end of charge voltage feature. I will be getting a sample of 1 piece for myself and if anyone else likes I can add them to it and ship it out to you when it gets to my place. The cost would be 25USD for the charger + the shipping to me divided by number of people + whatever shipping to you is. I'll update with what shipping to me would be soon. I want to order this within a day or two so let me know asap.
```

---
## \#159 Posted by: Randyc1 Posted at: 2017-07-31T14:28:36.834Z Reads: 137

```
Is it the model P-200 ?

That is 10S to 17S 
And 0-4,5 A 

Is this the one your talking about ?
```

---
## \#160 Posted by: jbruce Posted at: 2017-07-31T19:54:28.811Z Reads: 136

```
This is the model https://m.alibaba.com/product/60451408649/Electric-Tool-Lithium-Battery-Charger-42V.html?subject=Electric--Tool--Lithium--Battery--Charger--42V&spm=a2700.8443308.0.0.llhotG&detailId=60451408649&redirect=1
```

---
## \#161 Posted by: Randyc1 Posted at: 2017-07-31T20:05:38.349Z Reads: 135

```
Did you see the one im talking about ? 
Look in E-bike chargers,..35-60v 

Even better, ...good for 10s and 12s ! 

Wonder how much that one wld be ?
```

---
## \#162 Posted by: Ronny_CTS Posted at: 2017-07-31T21:50:09.778Z Reads: 132

```
@Randyc1  Is this the charger your talking about? 

http://www.modiary.com/productshow_en-137-100-1.html

They have it on their website but i can't seem to see it on their Alibaba store...I would be in on a group buy of these charger!
```

---
## \#163 Posted by: Randyc1 Posted at: 2017-07-31T22:52:04.376Z Reads: 132

```
Yes that is the one!
```

---
## \#164 Posted by: jbruce Posted at: 2017-08-01T02:42:56.523Z Reads: 131

```
I figured out shipping for 5 pieces is $55 to the us so it would be $36 + shipping to you if anyone wants one.
```

---
## \#165 Posted by: Ronny_CTS Posted at: 2017-08-01T07:33:56.360Z Reads: 126

```
For which charger?
```

---
## \#166 Posted by: jbruce Posted at: 2017-08-01T08:01:36.828Z Reads: 128

```
The original one I mentioned
```

---
## \#167 Posted by: Ronny_CTS Posted at: 2017-08-01T14:24:14.355Z Reads: 125

```
They also have an 8s-17s 7amp charger as well...model p300...this would be a beast fast charging an e-sk8. I'm gonna contact modiary to know more info on both models.
```

---
## \#168 Posted by: Randyc1 Posted at: 2017-08-01T14:33:09.455Z Reads: 130

```
Does that charger also have Variable Amp setting ,..or fixed at 7A ?
```

---
## \#169 Posted by: Ronny_CTS Posted at: 2017-08-01T14:37:32.193Z Reads: 130

```
I forgot to post the link...the specs say 0-7amp so we can assume it as being variable... ;)

http://www.modiary.com/productshow_en-107-80-1.html

If the specs are true this could be a great charger for a large range of battery packs!
```

---
## \#170 Posted by: Randyc1 Posted at: 2017-08-01T14:41:21.000Z Reads: 130

```
Yes get info on both models if you csn !
```

---
## \#171 Posted by: Eboosted Posted at: 2017-08-01T22:08:23.810Z Reads: 132

```
I'd be interested in the first one, count me in.
```

---
## \#172 Posted by: jbruce Posted at: 2017-08-02T05:56:40.169Z Reads: 130

```
The one I was talking bout?
```

---
## \#173 Posted by: SilentException Posted at: 2017-08-02T09:37:19.036Z Reads: 132

```
Getting confusing here :) How about making a list of available ones with voltage/amperage range specs in one post.

Also, how do you do range adjustment? Modiary does it during production or is it user adjustable? I could not see any accessible pots...
```

---
## \#174 Posted by: Eboosted Posted at: 2017-08-02T14:24:37.069Z Reads: 131

```
The first one for 10s
```

---
## \#175 Posted by: Ronny_CTS Posted at: 2017-08-04T07:52:42.254Z Reads: 136

```
The modiary website is deceptive. I've been talking to a sales rep named Ken and he told me that they do not sale any adjustable chargers with such a large range of adjustment. So no 8s-17s chargers. Basically it's whats in their alibaba store. 

I've tried asking him if his chargers have the feature to fine tune to a specific voltage such as adjusting a 42V charger to 41V but haven't been able to get a straight answer.
```

---
## \#176 Posted by: jbruce Posted at: 2017-08-04T08:32:53.332Z Reads: 138

```
Yeah I ended up asking the sales rep to ask the technical team if it had the feature and he said it did. Even if it doesn't I payed with PayPal and got buyers protection so I'm chillin

On that note, I ended up getting 2, the first for me and the second for whoever wants to snatch it up first. I'm asking $55 shipped free in the US.
```

---
## \#177 Posted by: Eboosted Posted at: 2017-12-07T06:33:38.840Z Reads: 122

```
[quote="jbruce, post:176, topic:6902"]
On that note, I ended up getting 2, the first for me and the second for whoever wants to snatch it up first. I'm asking $55 shipped free in the US.
[/quote]

Did you sell your charger? Was it an adjustable EOC?
```

---
## \#178 Posted by: Hummie Posted at: 2017-12-07T07:11:44.948Z Reads: 125

```
https://www.amazon.com/LM-High-precision-High-stability-Certification-Communications/dp/B06ZYDZCG9/ref=sr_1_4?ie=UTF8&qid=1512630499&sr=8-4&keywords=adjustable+power+supply+60v

why not just get one off amazon there are lots of options
```

---
## \#179 Posted by: DeathCookies Posted at: 2017-12-07T13:24:59.214Z Reads: 124

```
But it does not Support CC/CV?!
```

---
## \#180 Posted by: Kug3lis Posted at: 2017-12-07T14:04:46.805Z Reads: 119

```
For those PSU u will need something like DPS5020 for CC/CV
```

---
## \#181 Posted by: Kug3lis Posted at: 2017-12-07T14:05:22.806Z Reads: 121

```
I am currently building my own power supply using 2.2kW server power supply :)
```

---
## \#182 Posted by: Hummie Posted at: 2017-12-07T15:34:03.468Z Reads: 126

```
We've gone into a cc/cv discussion before and maybe I had it wrong but in my looking at lithium cell's needs the "cc/cv" thing is misleading.  

  This thing above I posted, I guess dubbed a psu, does a constant voltage meaning you set it to a voltage and the current flows at a variable rate based on how high that voltage is set to compared to the pack voltage and ohm's law I think.  With this one you can have about 8 amps flowing if you set it for full voltage while connected to an empty battery and that's far from what will damage a typical li-ion cell we use and far far from a lipo so there is no issue there and there's a lot of info out these days showing that charging at a high rate doesn't even damage the cycle life.  Check out Tesla's charge rate and I posted a related article last time we had this discussion.

And then  on the other hand I have read that lithium doesn't do well with trickle charging  and that will damage cells, and this isn't defined by cc/cv,  but even trickle charging is vague as to what voltage or current it means.
  I'm open, again, to someone telling me specifically why this or any other psu are in any way less suited than another charger but my faulty memory tells me this is good and I know many people use them for bikes or boards
```

---
## \#183 Posted by: chinzw Posted at: 2017-12-14T07:14:11.830Z Reads: 122

```
I totally lost track of this thread, im looking for a 41v charger, but these are not really made. Whats the latest on adjustable end of charge bricks? The DROK im currently using whines so loud i cant be in the same room while charging.
```

---
## \#184 Posted by: DeathCookies Posted at: 2017-12-14T13:34:29.227Z Reads: 122

```
I bet the noise is coming from the fan?!

if so -->
Did you try swapping the original fans with better ones? Like Noctua or so?
```

---
## \#185 Posted by: Eboosted Posted at: 2017-12-14T15:14:14.588Z Reads: 123

```
I search forever I never found a small charger with adjustable EOC.

So I went ahead and bought these:

58.8V/3A Cargador para las células 48V/14 Li-Ion Battery Pack, AC220V

https://m.ebay.com/itm/58-8V-3A-Charger-for-48V-14-CELLS-Li-ion-Battery-Pack-AC220V-/172995901571?txnId=1790684365007#vi__app-cvip-panel

And this:

DROK DC-DC Numerical Control Step Down Voltage Converter, 6-65V to 0-60V 8A 400W Buck Voltage Regulator Stabilizer, Constant Voltage Constant Current Power Supply with Volt Amp Dual LED Display

https://www.amazon.com/gp/aw/d/B01MSJQAKY
```

---
## \#186 Posted by: chinzw Posted at: 2017-12-14T18:01:30.885Z Reads: 118

```
I have plenty 40mm noctuas, but that's not the issue, there's a big coil that whines when you pull current from the dc-dc converter.
```

---
## \#187 Posted by: DeathCookies Posted at: 2017-12-17T18:32:25.533Z Reads: 114

```
I can hear you... Or should i say i can hear the coil :frowning:
Does anybody have an idea how we can reduce the noise of the coil? Adding one in parallel (i have nö clue)
```

---
## \#188 Posted by: DeathCookies Posted at: 2017-12-26T00:20:46.061Z Reads: 111

```
*bump*
anyone wanna give a hint?
```

---
## \#189 Posted by: Toleg Posted at: 2018-06-14T08:58:24.005Z Reads: 78

```
Do you think a DIN plug is OK to use with this 4A charger instead of the XL3 ?
```

---
## \#190 Posted by: atila82 Posted at: 2018-10-30T09:29:00.905Z Reads: 50

```
Hello, i have charger like this but my charger is dead after 1 mounth. Resistor in botad is broken ... can you help me i need to know sing of this resistor ...![20181028_171455|375x500](upload://n7ISPqKWgdb6Qw7BqsykvhEUoXK.jpeg)
```

---
