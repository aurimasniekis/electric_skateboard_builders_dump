# A Final Word on Bypassing BMS for Discharge

### Replies: 91 Views: 9162

## \#1 Posted by: JLabs Posted at: 2017-02-28T02:19:45.954Z Reads: 1021

```
After many comments on my recent battery packs, everyone wants a thinner pack, which is understandable. Only problem is the BMS.. The higher the Amp rating you go the more it costs and the bigger it gets. So, what is the final word on bypassing the BMS's discharge (in conjunction with the VESC of course)? For those who have did it, how are your packs? Any thoughts on whether or not a 'commercially' available pack should have a bypassed BMS? 

If I can recall I thought that the Space Cell has a 30a BMS but I cannot confirm.
```

---
## \#2 Posted by: michaelcpg Posted at: 2017-02-28T02:39:18.572Z Reads: 984

```
Fairly sure all pro version space cells only use 10A BMSs just for charging
```

---
## \#3 Posted by: rpn314 Posted at: 2017-02-28T03:25:59.695Z Reads: 981

```
I think many (personal experience talking here) do that so they don't have to spend as much and get a cheap one from China, but I now do not trust the cheap ones at all now (my pack got unbalanced, though I don't I did damage to it since I caught it quickly)

So I'd say if it's done just for the space requirements and it's still have a quality BMS, that is just smaller, I think it's a good way to slim it down. I thoroughly trust the VESC to properly handle the voltage cutoff and amperage discharge limits. If it's done for the cheap aspect, and you go with a low quality China BMS, then you're asking for trouble.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-02-28T03:55:57.152Z Reads: 948

```
[quote="rpn314, post:3, topic:18351"]
(my pack got unbalanced, though I don't I did damage to it since I caught it quickly)
[/quote]


Just curious, how unbalanced did your pack get and did it occur during charge or discharge?
```

---
## \#5 Posted by: rpn314 Posted at: 2017-02-28T04:12:22.067Z Reads: 926

```
I had 2 sets of cells that were about .75 volts below the rest in my 10s4p Li-ion 25R pack. They were still above the limits for the cells, but below what they should have been. I believe it happened during charging as the charger cutoff below where it used to (at like 90% on my percentage display instead of like 99%) and that triggered me to check the voltages of each set with a multimeter.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-02-28T04:29:04.977Z Reads: 910

```
The problem with BMS's is that they seem to be unable to balance a pack if it gets too far out of balance and will not charge to full charge because of this.
This happened to me one time when I replace one of the 2s Lipo packs in my build. the replacement was at storage charge while the other packs had considerable more charge on them. I wound up having to balance charge each pack individually with my hobby charger and then reconnect them to the bms.
It worked fine after that.
It is most likely that your pack went out of balance during discharge and your bms was unable to rebalance them.
I asked a rep from Bestech and they told me that the bms I use keeps the cells balanced during discharge as well as charge cycles.
I haven't actually tested to prove this however I think that I will soon just to see if it is really true.
If true, then this could be a really good argument for discharging through a bms.
```

---
## \#7 Posted by: rpn314 Posted at: 2017-02-28T04:49:24.252Z Reads: 865

```
Very valid point. There may be some real benefit to do balanced discharging as well, since the VESC cannot currently monitor that. I would be very interested in your findings. I haven't really ridden my board since the unbalanced issue as i took it apart to address the issue with a regular balance charger and to work on actually finishing it (it was functional, but not in enclosures or anything, the VESCs and batteries and such were just rubber banded in place)

I would add to this discussion that the newer "smart" BMS's that are in development around here (by @JTAG and @raphaelchang I believe) are quite small physically and can do everything we'd want them to do. They are on the more expensive side, so they be a great option if the only consideration is pack size (and not as much price)
```

---
## \#8 Posted by: Namasaki Posted at: 2017-02-28T05:06:52.664Z Reads: 836

```
It will be interesting to see what they come up with and as far as the price is concerned, if it's good then it will be worth paying for just like a quality vesc is.
I'm doing a little test right now with one of my builds that is under charging just a little. 41.8v and the green light comes on.
I pulled the cover off and check the voltage of each cell. they all range from 4.18 to 4.19.
I plugged the charger back in and after the green light came on again with the voltage at 41.8, I left the charger on and plugged in and after a little time the total voltage is up to 41.9
So apparently even after the charge light goes green, its still charging. I'm gonna leave it on for a while and see if it goes up to 42.0
I realize that 2/10 of volt is nothing over the entire pack.
In your case where your only getting 90%charge, maybe if you just leave the charger on it will eventually balance out the pack.
```

---
## \#9 Posted by: nmagz3 Posted at: 2017-02-28T06:38:00.636Z Reads: 778

```
@Namasaki @rpn314 I don't currently have a BMS but will be soon taking the plunge.  I have to say I thoroughly enjoyed your guys' discussion.  Thanks :grin:
```

---
## \#10 Posted by: Namasaki Posted at: 2017-02-28T06:57:25.478Z Reads: 766

```
Well I left it on the charger for a little while but it never went above 41.9.
I checked the cells afterwards and they are not perfectly balanced.
they vary from 4.195 to 4.205 which is  probably splitting hairs.
```

---
## \#11 Posted by: treenutter Posted at: 2017-02-28T14:21:56.657Z Reads: 741

```
[quote="Namasaki, post:6, topic:18351"]
a rep from Bestech and they told me that the bms I use keeps the cells balanced during discharge as well as charge cycles
[/quote]

@Namasaki that's interesting, and contrary to all else I've read. If it's true, that's great! Can anyone verify this? 

To add to this discussion @JLabs I current have a Bestech 80A BMS and the problem is that it's huge and heavy. In the future I plan to bypass the BMS and use a good-quality (but physically smaller) BMS, assuming I can find one haha!
```

---
## \#12 Posted by: makevoid Posted at: 2017-02-28T15:25:08.253Z Reads: 703

```
For a 10S I found [this 60A BMS](http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html) to sustain a dual (street, not mtb) build load ok, it's not that big (112mm * 53mm and probably ~12mm thick, can't remember) and it seems to do the job. I have 2, one is connected to a 8S5P (I didn't connect the balance wires 9 and 10) pack and it kept my cells balanced for ~6 months / over 1000 km and they're still inside the +/- 0.5v range.
```

---
## \#13 Posted by: Namasaki Posted at: 2017-02-28T16:37:41.273Z Reads: 684

```
I will be testing this theory very soon. 
I did notice that when I was riding my brakes down a steep hill with a full battery and my pack voltage went up to 42.1 or 42.2 that within seconds after I released the brake and was coasting, the BMS brought my voltage back down to 41.9
```

---
## \#14 Posted by: Namasaki Posted at: 2017-02-28T16:49:46.982Z Reads: 675

```
I have a few problems with Battery Supports BMS. 
1: when I ordered one, they couldn't get my order through customs and after waiting too long I cancelled the order. 
2: they don't have a built in E-switch so you'll need an external E-switch  which means extra cost, more connections  and more space to mount it. 
And since they don't have a switch, it seems that they are always on so how do you reset it if one of the safety circuits trips?
```

---
## \#15 Posted by: makevoid Posted at: 2017-02-28T23:18:07.317Z Reads: 647

```
Yes, I felt the need to have a switch too, I reset it once (desoldering/resoldering a battery wire and unplugging it) but I saw there wasn't the need to in that case, the battery was low (I left lcd and vesc on for long time) but it just needed the (li-ion / brick) charger to slowly charge it to "revive" it, unplugging and replugging the bms was not needed but I agree it can be time consuming if that fails and it's soldered
```

---
## \#16 Posted by: racidon Posted at: 2017-02-28T23:27:30.596Z Reads: 649

```
[quote="JLabs, post:1, topic:18351, full:true"]
After many comments on my recent battery packs, everyone wants a thinner pack, which is understandable. Only problem is the BMS.. The higher the Amp rating you go the more it costs and the bigger it gets. So, what is the final word on bypassing the BMS's discharge (in conjunction with the VESC of course)? For those who have did it, how are your packs? Any thoughts on whether or not a 'commercially' available pack should have a bypassed BMS? 

If I can recall I thought that the Space Cell has a 30a BMS but I cannot confirm.
[/quote]

Being the owner of a space cell I'd advise against it. Mine has likely got dead cells in it as it won't charge pass 92% and barely gets half the range it used to. Before the issue with 92% being the max battery capacity it wouldn't charge pass 96%.
```

---
## \#17 Posted by: JLabs Posted at: 2017-03-01T00:00:41.876Z Reads: 628

```
@barajabali @onloop Do you guys have experience with this? By that I mean bypassing the BMS's discharge. Any comments?

(Jason I dont mean directly respond to the comment above)
```

---
## \#18 Posted by: barajabali Posted at: 2017-03-01T00:25:05.827Z Reads: 623

```
As long as you're using the vesc, bypassing the bms for discharge isn't a big problem. Better to do it with larger batteries rather than smaller. Larger batteries are more stable and generally stay in balance with less effort
```

---
## \#19 Posted by: JLabs Posted at: 2017-03-01T00:54:46.229Z Reads: 617

```
As large you refer to the amount in parallel? So its a no go for 2p but acceptable for 3p+?
```

---
## \#20 Posted by: barajabali Posted at: 2017-03-01T00:59:59.625Z Reads: 622

```
Eh 'large' is sort of relative. Depends on the amps you want to pull in my opinion. 

You'd really just have to do it and test it. I find that no bms discharge  on my 7p batteries is totally fine.
```

---
## \#21 Posted by: JLabs Posted at: 2017-03-01T01:00:46.792Z Reads: 590

```
Ok thanks!
```

---
## \#22 Posted by: Eboostin Posted at: 2017-03-01T07:03:57.238Z Reads: 586

```
Were you using it for charging only?

An 8S pack on a 10S BMS would trigger the low voltage cutoff when the cells are at ~3.6v lesving quite a bit of range on the table
```

---
## \#23 Posted by: lowGuido Posted at: 2017-03-01T08:21:10.821Z Reads: 591

```
I really don't understand the issue with adding a switch to a BMS. I mean FETs are already there, just turn them off.
```

---
## \#24 Posted by: makevoid Posted at: 2017-03-01T08:35:30.499Z Reads: 594

```
edit 

the bms seems not to limit the current below 36v, here's a video where I start at 31 v
https://youtu.be/bxSrCjUnLUc

could it be smart so it bases the cutoff on how many balance leads are actually connected or do you think I lost the discharge protection from the bms?
```

---
## \#25 Posted by: Namasaki Posted at: 2017-03-03T02:27:25.708Z Reads: 582

```
Ok, so I did a little test today. I went out with a full charge through the bms and brick charger. Rode till my battery meter was showing about 38.5v
When home and opened up the enclosure and checked each individual cell. the voltages where
3.855
3.859
3.864 high
3.857
3.859
3.855
3.859
3.855
3.846 low
3.849
Max spread between highest and lowest cells  .018v
Does that sound like the BMS is balancing the pack during discharge or do you think Lipo cells can discharge that evenly without assistance?
```

---
## \#26 Posted by: rpn314 Posted at: 2017-03-03T02:31:46.513Z Reads: 560

```
Those swings aren't too bad. 0.018v high to low I'd consider really good. I think lithium cells can discharge that evenly if they're good cells (which I assume yours are) and they're not very used, but that is such a low swing that I would agree that your BMS is doing some balancing during discharge as well. 

I imagine as the internal resistance of a cell increases (as they age, which I doubt they'd do perfectly together) they don't discharge as well so they become unbalanced easier. Most of that is just gut talking, so feel free to correct me.
```

---
## \#27 Posted by: Namasaki Posted at: 2017-03-03T02:36:47.735Z Reads: 548

```
These are quality packs with very low internal resistance. I tested them when first received and if my memory serves, they where all below 2 miliohms.
I would like to do another test taking the pack from full charge down to at least 36v or 34v and then see how the spread looks.
I'll do that soon and post it here.
```

---
## \#28 Posted by: rpn314 Posted at: 2017-03-03T02:43:29.540Z Reads: 545

```
Much appreciated @Namasaki. We all thank you :bow: (<- that's supposed to be a bow...not sure what it actually looks like)
```

---
## \#29 Posted by: Eboosted Posted at: 2017-03-03T04:51:11.711Z Reads: 533

```
So, to get back on topic. Since I started using my BMS for charge only I haven't had any cut outs due VESC rebooting itself on fully charged battery under braking.

It has been working so good that I'm buying a US$ 10 BMS for charging only for my next build, it'll save me space and keep me out of future problems.
```

---
## \#30 Posted by: Namasaki Posted at: 2017-03-03T06:51:28.932Z Reads: 526

```
I have never had a problem with my Vescs cutting out while braking down steep hills on a full battery while discharging through my BMS.
```

---
## \#31 Posted by: Eboosted Posted at: 2017-03-03T06:57:28.375Z Reads: 520

```
That's because you use a Bestech BMS, the Battery Supports one cut's off current when it's goes beyond 42v
```

---
## \#32 Posted by: Namasaki Posted at: 2017-03-03T06:59:53.051Z Reads: 516

```
Oh, I didn't know that.
Another strike against battery supports
```

---
## \#33 Posted by: Namasaki Posted at: 2017-03-03T07:22:00.619Z Reads: 508

```
This might be a little off topic but I'm wondering how high the voltage on the battery can go temporarily before it presents a hazardous situation.
```

---
## \#34 Posted by: Cuprani Posted at: 2017-03-03T07:39:18.310Z Reads: 509

```
That depends completely on the internal resistance.

With a high internal resistance stock voltage could already fry the battery, while at very low resistance it could take a lot more current. Every battery will be different in that case.
```

---
## \#35 Posted by: Namasaki Posted at: 2017-03-03T13:03:06.050Z Reads: 504

```
Yes but I was talking voltage not current. 
And specifically voltage over 4.2 per cell during regen braking
```

---
## \#36 Posted by: flywithgriff Posted at: 2017-08-27T20:52:38.680Z Reads: 460

```
I have read through this thread an have actually learned a bit. I do still have a question though. If I bypass the bms that has a built in e-switch, do I then need to install an inline switch or will the BMS e-switch still operate.
```

---
## \#37 Posted by: JLabs Posted at: 2017-08-27T21:00:28.363Z Reads: 458

```
The BMS eswitch will not work when bypassing
```

---
## \#38 Posted by: flywithgriff Posted at: 2017-08-27T21:11:15.076Z Reads: 459

```
That sucks. I have a brand new 80A  Bestech BMS that does not power on.
```

---
## \#39 Posted by: darkkevind Posted at: 2017-08-27T21:55:55.229Z Reads: 451

```
I foolishly bought an 8s 60A discharge BMS for my pack that I recently made, (foolish because I decided just to bypass for discharge and 8s high A output BMS' are like rocking horse shit), and after many cycles my pack is in great shape!

Next time I'll just get one that can fast charge and not care about the A discharge rate.
```

---
## \#40 Posted by: flywithgriff Posted at: 2017-08-27T22:01:30.741Z Reads: 447

```
So I can just say the hell with it and order a BMS just for charging?
```

---
## \#41 Posted by: darkkevind Posted at: 2017-08-27T22:04:38.845Z Reads: 424

```
In my experience I'd say yes, but an expert on the matter may say otherwise...
```

---
## \#42 Posted by: flywithgriff Posted at: 2017-08-27T22:06:57.535Z Reads: 420

```
@Namasaki what's your opinion?
```

---
## \#43 Posted by: Namasaki Posted at: 2017-08-27T23:06:25.415Z Reads: 423

```
My opinion is that it is worth having a large high amp output bms in order to have over discharge cell level protection along with short circuit protection.
Plus the bms will protect against over charging while regen braking.
```

---
## \#44 Posted by: flywithgriff Posted at: 2017-08-27T23:09:34.338Z Reads: 425

```
This is pretty defeating. Been waiting a few weeks and my $60 Bestech is dead the same day I install it.
```

---
## \#45 Posted by: Namasaki Posted at: 2017-08-27T23:11:11.046Z Reads: 428

```
I still think something else is wrong. The Bestech are factory tested before they ship it.
I have never got one DOA.
```

---
## \#46 Posted by: willpark16 Posted at: 2017-08-27T23:14:47.193Z Reads: 425

```
I've got working bms if u want one
```

---
## \#47 Posted by: flywithgriff Posted at: 2017-08-27T23:17:09.016Z Reads: 426

```
Please pm me details!!
```

---
## \#48 Posted by: willpark16 Posted at: 2017-08-27T23:20:39.159Z Reads: 426

```
I thought I sent u one
```

---
## \#49 Posted by: kebabbob Posted at: 2017-09-30T21:44:01.417Z Reads: 425

```
I tried searching around, but didn't find anything. What's the preferred way to bypass the BMS for discharging? The main reason I want a BMS is so I can put just one plug on my enclosure and the BMS takes care of balancing the cells as they are charged. I don't really care about over current or them being balanced on the fly or while riding...
```

---
## \#50 Posted by: gogomrrobot Posted at: 2017-10-01T12:35:25.694Z Reads: 431

```
Stay tuned... I am doing a 12s4p build which is almost complete... No BMS. Yet I will have balance charging.  I will be placing (2) 6s balance leads, one on the first set of 6 x 4p packs and another on the second set of 4p packs.  There will be a single xt 60 or 90 plug for the entire 12s4p pack that will serve as the charge port.  That circuit will connect to an antispark as well by splitting the +/- but that is a small detail.

The big deal will be No BMS. I bought a 12s (truly 12s charger) + a server power supply that can deliver 75A to the 12S charger off of ebay.

Here is a preview for now of the 12S charger/port:

Charger: 
<img src="/uploads/db1493/original/3X/7/0/70c7faa43559c7d0472b8fe39309248b695eac32.JPG" width="640" height="480">

Charger plugin 12S card:

<img src="/uploads/db1493/original/3X/2/c/2c2dcd3be744481a7a549fadac03801b99207214.JPG" width="375" height="500">

It really wasn't more expensive than a 12S 48V 60A BMS + dedicated laptop style brick which will cost you $120-$165 based on your shipping options.

It's a one time investment. The only downside is... if I sell the board, the other guy will need to have a 12S charger too. But I don't intend to sell the board ;)
```

---
## \#51 Posted by: GrecoMan Posted at: 2017-10-01T12:43:54.310Z Reads: 421

```
I’m a sucker for prebuilt packs...
No assembly from me = less chance of a problem for me

Edit:  dang I love it when I fill the whole front page with my name 😂
<img src="/uploads/db1493/original/3X/d/d/dd7057eef40f0ea80414cc402d9807c70e3aedf2.png" width="281" height="499">
```

---
## \#52 Posted by: gkeefe10 Posted at: 2017-11-16T03:11:42.391Z Reads: 393

```
ok so Im using a 10 4p battery but I can't afford to buy a 80 a bms would a 40a 10s bus work for charging my battery safely.

The esc that I'm using controls my battery discharge
```

---
## \#53 Posted by: louwii Posted at: 2017-11-16T03:47:23.197Z Reads: 390

```
If you're gonna use the BMS only for charging, you're safe. A low amperage means that the charge will take more time.

I do have a question too regarding BMS. Is it okay to buy a 10S BMS for a < 10S battery ? Just not plug the last wires and that's it ?
```

---
## \#54 Posted by: Eboosted Posted at: 2017-11-16T03:51:28.975Z Reads: 397

```
I've been using my Vanguard battery with bms only for charging, I don't have any safety feature enabled by doing this, so I wouldn't suggest people do it unless, like me, you know exactly when your batteries are drifting and immediately take measures to fix the issue.

This is the procedure I use to check battery status:

1. Check the SOC at the end of my daily commute, if it's 71% as soon as I arrive and goes up to 74% before o plug it to the charger, battery is good and balanced.

2. Check the SOC everyday as soon as I unplugged from the charger, it must be 100%, if it's lower battery drifting is happening

3. Charge my battery everyday with a lab power supply at 41.5V on my 10S4P and see if the current is drops at 0.02A at end of charge, if it still outputs  0.3A or higher for more than 30 minutes, one cell or a full pack is bad.

4. Open the enclosure once a month a measured each pack looking for drifting, check for broken connecting wires, or crooked balancing wires, write down the differences in an excel sheet.

If don't want to go through all this hassle just use bms for charging and discharging and let it do its job.

For me I like doing this and enjoy it very much.
```

---
## \#55 Posted by: gkeefe10 Posted at: 2017-11-24T02:14:26.353Z Reads: 363

```
Im not an expert on this topic but in a video I watched the guy said that that would not work and you need to get the bms for the right voltage of your battery even if its just charging
```

---
## \#56 Posted by: gkeefe10 Posted at: 2017-11-24T02:16:40.242Z Reads: 369

```
Im using a esc that discharges dual 35 a continues per motor and I have two 32a rated motors will this cuase problems with over heating or just kill my motors
```

---
## \#57 Posted by: Eboostin Posted at: 2017-11-24T02:17:17.186Z Reads: 372

```
Was your board that caught on fire also bypassing the BMS?
```

---
## \#58 Posted by: louwii Posted at: 2017-11-24T02:18:57.268Z Reads: 367

```
Yeah that makes sense. Thanks
```

---
## \#59 Posted by: gkeefe10 Posted at: 2017-11-24T02:26:08.833Z Reads: 364

```
Im using a esc that discharges dual 35 a continues per motor and I have two 32a rated motors will this cuase problems with over heating or just kill my motors
```

---
## \#60 Posted by: Eboosted Posted at: 2017-11-24T06:24:10.237Z Reads: 360

```
Yes, it was determined the cause of fire was a loose bullet conector making sparks on a neoprene rubber.

I wonder how would a BMS prevent a fire on this case
```

---
## \#61 Posted by: Deckoz Posted at: 2017-11-24T08:18:22.935Z Reads: 344

```
Us 7mm antispark bullets. If it rattles loose no spark
```

---
## \#62 Posted by: chrisongtj Posted at: 2017-11-24T10:37:03.591Z Reads: 344

```
Best would be to direct solder the motor. No risk of hardware failure.
```

---
## \#63 Posted by: Eboosted Posted at: 2017-11-24T16:22:21.890Z Reads: 346

```
I'm using XT60 after the fire incident, no more spark if they become loose
```

---
## \#64 Posted by: Deckoz Posted at: 2017-11-24T16:26:20.313Z Reads: 349

```
That too ;)
```

---
## \#65 Posted by: tristanrai Posted at: 2018-06-23T16:24:11.407Z Reads: 277

```
hey there i really need your help and you seem like the right person to go to for it ;))

ive had an electric skateboard that served me well, until its cells died after the bms drained it. I got new cells and an exact same BMS, with the only exception of it not having an on/off switch. Do you think its alright to forgo to on off switch and leave my board on all the time? thank u so much
```

---
## \#66 Posted by: Namasaki Posted at: 2018-06-24T03:28:05.083Z Reads: 275

```
Hard to say not being familiar with what bms your using now.
If left on, I would keep an eye on your pack's voltage periodically and make sure that the battery isn't draining too low.
You definitely want to have the Vesc or Vescs disconnected while storing your board.
If your going to store it for an extended period and checking the voltage regularly is not possible then charge the battery to storage voltage and disconnect it from the entire system.
```

---
## \#67 Posted by: tristanrai Posted at: 2018-06-24T06:32:26.013Z Reads: 264

```
By storing for a long period you mean not using it for a long period of time and leaving it on,  or using it regularly and leaving it on all the time
```

---
## \#68 Posted by: pat.speed Posted at: 2018-06-24T07:04:31.700Z Reads: 267

```
I don’t think it’s a good habit to leave the board on as eventually you might forget. 

Fun fact: did you guys know that the eBay esc has an automatic turn off feature that turns the board off after being on for a while
```

---
## \#69 Posted by: Namasaki Posted at: 2018-06-24T14:53:59.751Z Reads: 263

```
[quote="tristanrai, post:67, topic:18351, full:true"]
By storing for a long period you mean not using it for a long period of time and leaving it on, or using it regularly and leaving it on all the time
[/quote]


Either storing it for a long time or simply not using it for a long time. It's basically the same.
You should never leave the the whole system including the Vescs on while your not riding it.
Leaving the bms connected while in storage will depend on the characteristics of the bms.
If your going to store your board for a year or longer then I would recommend a storage charge and disconnect the battery from everything.
```

---
## \#70 Posted by: rockon915 Posted at: 2018-08-26T01:48:59.182Z Reads: 233

```
I am considering bypassing bms because this issue i will explain below.

Would anyone know why the bestech12s bms would cause me to have an early low voltage cutoff? Usually around 44.4V. 12s5p to bestech 12s bms(HCX-D223v1) to 80 amp antispark (from eskating.eu) to dual focbox to dual TB6374. Running 60A motor max 30A battery max. voltage cutoff on focbox start set to 41.0V and end set to 39.0V. Note all cells are verified at 3.7V

antispark link https://eskating.eu/product/anti-spark-power-switch/

bms link https://eskating.eu/product/12s-bestech-bms-80a-12s4p-5p/

Any input would be great as i would like to go for a ride without unexpected cutoff and support hasnt been of much help yet. hopefully they will get back to me with more info.
```

---
## \#71 Posted by: JLabs Posted at: 2018-08-26T01:53:51.331Z Reads: 222

```
Since your running 5p you can go a max of 100A battery current but that’s not realistic. I’d say 65A is good. You cutoff values are insanely high tho. The cutoff end is at 2.8v/cell so that is 33.6v and cut off start is around 3.1v/cell which is 37.2v.
```

---
## \#72 Posted by: rockon915 Posted at: 2018-08-26T02:03:19.918Z Reads: 223

```
Once i trust the battery wont cut off i will probly up the amps. I just read that you dont want to take cells below 3.2v using Samsung 30q i will try lowering the battery cuttoff on the focbox and see if that fixes anything. i will try maybe 38v start and 34v end to be conservative(i may be overconservative with current set up)  but my issue is that its cutting off at 3.7V per cell or 44.4V overall. anyway ill try that and see how she goes
```

---
## \#73 Posted by: JLabs Posted at: 2018-08-26T02:17:03.405Z Reads: 217

```
The only way to test would be with a current load (not the VESC) to see if it is the BMS. If it is, the BMS will cut at 44.4v under load. The anti spark shouldn’t have anything to do with the issue
```

---
## \#74 Posted by: rockon915 Posted at: 2018-08-26T05:20:29.652Z Reads: 216

```
so just went for a ride had an issue at the same point in my ride. finished ride with 3.7v or 44.4v after setting battery cutoff on focbox to 38v start and 34v end.
```

---
## \#75 Posted by: Eboosted Posted at: 2018-08-27T05:06:15.179Z Reads: 211

```
Maybe there is a pack with lower voltage than the others or sagging a lot more than the others, this will cause the BMS to shut down the power in order to protect the lowest P-Group from reaching a pretty low/dangerous voltage.

Unmount your battery and meassure all voltages now.
```

---
## \#76 Posted by: rockon915 Posted at: 2018-08-27T22:51:49.646Z Reads: 201

```
yah i check all voltages after atleast every other ride everything is ballanced even when the cutoff occurs ill stop in the middle of the road open it up and check on the spot and everything is still ballanced. unless like you say one is sagging more than the rest i would have to have a monitor on each individual cell during the ride to notice that. i track all my rides with ackmaniac and havnt noticed anything out of the ordinary there. i did bypass bms last night and had no cutoffs and more torque. altho i would really like to figure out this bms thing as i like the idea of the extra protection on discharge
```

---
## \#77 Posted by: taz Posted at: 2018-08-28T08:02:35.309Z Reads: 197

```
I had a similar problem and it turned out I had broken series connections in my pack.
Most of the time it would work but when it did not the BMS shut down the board.
I bypassed the discharge and the board would cut out for a second then recover.
After I fixed the pack, I reinstated the BMS to discharge also.
Who made your battery?
```

---
## \#78 Posted by: rockon915 Posted at: 2018-08-28T18:02:39.417Z Reads: 195

```
i built it so it will deffinetly be worth checking but i havnt had any issues after i bypassed discharge. still gonna check it all out tho to be sure. thanks
```

---
## \#79 Posted by: asuras Posted at: 2019-04-18T02:52:07.717Z Reads: 135

```
@makevoid Sorry for the bump, but can you give me some advice on my current build? I'm pretty new to electronics in general, but keen to learn. I'm looking to put a dual [Turnigy Aerodrive SK3 - 6374-149KV Brushless Outrunner Motor](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html) onto my A/T rig, these motors specify a max loading of 70a, So does that theoretically mean they might want to pull 140a through the ESC/BMS/battery under full load?

I'm probably going to put a focbox in there, and I have a 10s5p LG HG2 pack which I understand can draw 100a continuous easily, so I'm trying to spec up a suitable charge/discharge BMS to run the whole shebang, but running into space issues in the enclosure, so I'm curious what is the lowest amp BMS I could consider that will do the job...
```

---
## \#80 Posted by: Eboosted Posted at: 2019-04-18T05:37:28.314Z Reads: 126

```
[quote="Eboosted, post:60, topic:18351, full:true"]
Yes, it was determined the cause of fire was a loose bullet conector making sparks on a neoprene rubber.

I wonder how would a BMS prevent a fire on this case
[/quote]

Well, after a lot of thinking I can confirm the real cause of the fire on my Trampa was the lack of fish paper between pgroups
```

---
## \#81 Posted by: Andy87 Posted at: 2019-04-18T06:01:30.095Z Reads: 124

```
Hey I might not be @makevoid but  maybe I can help with some things as well.

There some things you need to understand first.
Battery amps are not motor amps. Means if your motors run at 70A than it doesn´t mean your draw 140A from your battery.

Secondly your battery doesn´t draw 100A, your battery is able to supply 100A continues.

As you will set everything up with focboxes you can set the BAT max value to 50A per focbox, which would mean 100A from your battery. A good BMS for discharge in this case would be the D596 which is a 90A BMS. If you worry that BMS could cut out as 90A is lower than 100A than just set your max current in your focbox to 45A per esc. But even at 50A the BMS shouldn´t cut out as the 90A are continues values and it´s pretty unlikely that you will draw 90A continues from your battery under normal circumstances.
```

---
## \#82 Posted by: makevoid Posted at: 2019-04-18T12:00:22.160Z Reads: 107

```
agree on what Andy87 said!
```

---
## \#83 Posted by: asuras Posted at: 2019-04-18T12:32:15.755Z Reads: 107

```
OK, but things get confusing for me when I consider that I have 2 of these 70a motors and trying to guess at how much juice they're going to need. I'm using a focbox unity which specifies 80a discharge. But what will these motors be wanting to draw under various circumstances? By one calculation I figured that giving them 50a each should be plenty, but that's more than the focbox can deliver. If they're limited to 40a each is that still going to be enough?

I'm pretty light at 65kg, but the area I skate in is somewhat hilly and sometimes I also tow a trailer which can have around 30kg in it, so I'd need something that can comfortably climb hills with around 100kg load.
```

---
## \#84 Posted by: Andy87 Posted at: 2019-04-18T12:38:06.050Z Reads: 113

```
[quote="asuras, post:83, topic:18351"]
climb hills with around 100kg load.
[/quote]

don´t worry about that, that should be possible without issues if your gearing is something between 1:4 , 1:5 

As I said , motor amps not bat amps and you can set all in the unity. if you set your unity up for 80A batt max and 70A for each motor you will have plenty of torque and all parameters in your system are on point.
```

---
## \#85 Posted by: asuras Posted at: 2019-04-18T12:46:39.759Z Reads: 109

```
Perfect, thanks for the explanation!
```

---
## \#86 Posted by: asuras Posted at: 2019-04-18T13:14:33.465Z Reads: 104

```
Come to think of it gearing is one thing I hadn't even considered, my board by default has 15T on the motor and 38T  on the wheel, which I guess puts the gearing at 1:2.5 which is way out of your range, is this going to be a problem? I'm guessing here that if anything this would give me a big safety margin and I could actually increase the ratio safely?
```

---
## \#87 Posted by: Andy87 Posted at: 2019-04-18T13:17:32.664Z Reads: 106

```
sorry my bad, I thought you with 8" pneumatics. with urethane wheels things look different. Maybe somebody more experienced with urethane wheels can suggest you which gearing would fit for you best. your motors are 149kV and your wheels are which diameter?
```

---
## \#88 Posted by: asuras Posted at: 2019-04-18T13:21:47.617Z Reads: 108

```
Yes I am pneumatic, 8" MBS (200mm). I probably won't ever put street wheels onto this rig.
```

---
## \#89 Posted by: Andy87 Posted at: 2019-04-18T13:24:54.377Z Reads: 107

```
than 36 teeth wheel pulley is too less. you want 60th minimum with a 15th motor pulley. better  66th or 72th.
```

---
## \#90 Posted by: asuras Posted at: 2019-04-18T13:48:28.483Z Reads: 105

```
https://www.evolveskateboards.com.au/collections/all/products/at-drive

Problem solved! Thanks heaps for your advice! (Although now I look at that picture I think I might already have these on my board, I had written down 38T but I think thats for the street setup which I don't use...)
```

---
## \#91 Posted by: DJ8055 Posted at: 2019-08-04T11:32:12.905Z Reads: 48

```
Which bms did you go with and how did you bypass for charge only?
```

---
