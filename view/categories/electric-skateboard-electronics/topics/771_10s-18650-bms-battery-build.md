# 10s 18650 BMS Battery Build

### Replies: 65 Views: 44722

## \#1 Posted by: Jack Posted at: 2015-12-22T00:08:04.048Z Reads: 1648

```
Hi guys,

I am currently using a 6s setup (two zippy 5000mah 3s in series) and I am looking to add a bit of power and also improve the ease of charging and maintaining the packs. I have read what feels like 100s of posts about building a pack but nobody has really done a step by step newbie guide! After sort of grasping all the do's and donts of building a reliable pack this is what I have come up with. 

I want to use 18650 cells, not sure if these are actually samsung cells but look pretty good for the price. (Oh I'm a student so don't have that much disposable income haha)
http://www.aliexpress.com/item/2015-10PCS-Samsung-Original-18650-ICR18650-26F-2600mAh-Li-ion-3-7V-Rechargeable-Battery-Rechargeable-flashlight/32505862751.html

So if i order 2 lots of those for 20 cells i can make a 10s pack with slightly increased mah ratings. Also gonna need a BMS to keep all these cells balanced. Would this be good? http://r.ebay.com/lNASwp

So the question is how to connect the pieces of the puzzle. Illustrator is my friend so I've drawn a pretty simple diagram of the parts and how i think I'm supposed to connect everything. Does this look correct?

Thanks for the help!

<img src="/uploads/db1493/original/2X/c/c3972f6694a065bb5b93d8e85807787449957013.png" width="690" height="490">
```

---
## \#2 Posted by: stuxtruth Posted at: 2015-12-22T00:53:47.164Z Reads: 1459

```
Thank god. I am in the exact situation looking to do the same thing. Hopefully some good info pops up in here.
```

---
## \#3 Posted by: Jack Posted at: 2015-12-22T01:02:01.344Z Reads: 1469

```
Yeah I've found the info really lacking for building small packs for skateboard use. There is some good info on endless sphere but those e-bike packs are huge and expensive!

Once I have this figured out I'm planning on doing a complete build post and also a step by step on building a reliable pack for e-board use. The SPACE cell looks awesome but I have a Loaded Tan Tien thats suuuuper flexy which won't play nice with the hard case of the battery.

I'm pretty much trying to build a DIY space cell that I can configure to fit my board, I don't want to rip off any of enertions awesome designs but it would be really handy for a diagram of the SPACE cell haha :smiley:

Oh also is anyone else on here from the UK?

Jack
```

---
## \#4 Posted by: stuxtruth Posted at: 2015-12-22T01:10:01.101Z Reads: 1412

```
Yea there are local battery  shops around here that will spot weld and heat shrink battery packs for pennies on the dollar but I don't quite understand how to choose the right BMS and wire it in. Also it looks like everyone is using the same laptop charher socket so I would like to get specs on that. For example. Bubblegum boards used the same exact charger port than enertion did on his packs.
```

---
## \#5 Posted by: Jack Posted at: 2015-12-22T01:17:17.731Z Reads: 1389

```
Im pretty sure it doesn't really matter what socket is used for charging. As long as it is rated for the amps your charging the pack. I was planning on using a standard jack like this to charge. Just connect 36v to the terminals. <img src="/uploads/db1493/original/2X/b/b36ccd644600c4a3c2c5dcc842997f753c0872e8.jpg" width="690" height="398">
```

---
## \#6 Posted by: Blasto Posted at: 2015-12-22T01:30:43.701Z Reads: 1327

```
Guys check this build up for some good info

https://endless-sphere.com/forums/viewtopic.php?f=35&t=72026

You're going want to put some cells in parallele
```

---
## \#7 Posted by: Jack Posted at: 2015-12-22T01:52:34.490Z Reads: 1309

```
Thanks for the link. Its weird I read through that thread awesome build by whitepony and it gave me lots of info but he's not using a bms, and I sort of think thats essential based on what I've read.
```

---
## \#8 Posted by: Braylon31 Posted at: 2015-12-22T07:02:51.947Z Reads: 1309

```
Im also interested in this was thinking about using  18650 battery holders and soilder the connection to brackets then pop in the batteries then shrink them i was hoping this diagram works i need a simplified answer like this one to the confusing science of lithium batteries  seem like no ones chiming in i kn9w someone has to know something about this post to futher promiseing results come on people lo l:) ???
```

---
## \#9 Posted by: scoobiext Posted at: 2015-12-22T07:20:49.912Z Reads: 1304

```
G'day Jack

I brought my cells ( http://www.batterysupports.com/lg-lgdbhe21865-high-drain-2500mah-36v-20a-lithium-ion-lion-p-345.html ) and BMS ( http://www.batterysupports.com/36v-60a-12s-12x-32v-lifepo4-battery-bms-lfp-pcm-smt-pcb-system-p-251.html ) from SuPower  

I brought 30 cells arranged in 10 x 3P packs (good for a maximum of 60A continuous) and soldered the packs together in series.  The BMS I brought is rated at 60A continuous but apparently can supply up to 80A peak.  The total cost was around $280 delivered to Oz.  The cells arrived in good condition and each had a charge of very close to 3.6V, It was fairly easy dealing with Lillian from SuPower and the delivery time wasn't too bad given that the cells come from China.
<img src="/uploads/db1493/original/2X/3/3c0ddc651131526d90e038748c324e7502bb64e6.png" width="690" height="389">

I haven't had my board running all that long but so far I am impressed with the battery pack and BMS.  I managed to do about 18Kms the other day and still had 34V of charge (I usually charge the pack to about 41.0V).  The BMS does a very good job of keeping the cells in balance, so far my checks have indicated that the cells have been kept close to the stated balance tolerance (a measured maximum difference of 0.054V across all cells).

I soldered my packs together using nickel plated strips.  Ideally I wouldn't recommend soldering the battery packs as its not really that easy and isn't good for the batteries.  Next time I build a pack I will make a capacitive discharge spot welder and weld the packs.  But sometimes you just have to do what you need to do.  I use an XT60 connector to charge the pack in the board mounted enclosure, however I do like the DC jacks that you have suggested and will probably use something similar when I re-design my battery enclosure.

A couple of key points I that I would pass on are to make sure you insulate every thing really well, especially the balance wires and anywhere a positive could come into contact with a negative.  You do not want to short these cells its dangerous and very bad for the cells.  Also try really hard to minimize the heat you put into the cells and make sure you have really strong low resistance joints between cell packs (easier said than done). 

Here is how it all turned out.
<img src="/uploads/db1493/original/2X/0/009ec8a3cc08ec72606f6372fa3ceb85179035fb.png" width="690" height="326">

<img src="/uploads/db1493/original/2X/9/9414e827cbed6674ce5709adcfe21462a716f715.png" width="690" height="390">

I would be happy to provide any further insights into my experiences during the build of the battery pack if you need.

Cheers,
```

---
## \#10 Posted by: scoobiext Posted at: 2015-12-22T07:25:33.225Z Reads: 1178

```
Also I forgot to mention that my battery back is wired exactly as per your drawing.  The only difference I have is that I have a soft switch between the VESC and the battery.
```

---
## \#11 Posted by: lox897 Posted at: 2015-12-22T10:06:28.659Z Reads: 1162

```
I am going to follow this thread. How many cells do you think you are going to put im parallel. Also check out whitepony's diagram on connecting cells because he did a design that folded out so it was flat, may help a bit.

PS: Love your website! The designs are quite cool IMO
```

---
## \#12 Posted by: Jack Posted at: 2015-12-22T10:59:47.934Z Reads: 1153

```
@scoobiext Your pack looks amazing, I'm loving the CF case also!

I'm thinking of using 2 cells parallel and using the same wiring diagram as I posted for 10s2P Am I right in thinking that will give me just over 5000mah as the cells are 2600mah. How would the discharge current handling capability be with 10 less cells than you? I don't really do long journeys so there isn't much point carrying around the extra bulk and cost.

Are you pleased with the BMS? I think the one your using looks better than the link I posted. Does it get very hot during heavy use? I wanted to put it on top of the cells as I don't have much space but would that damage the cells in the long term?

Oh also whats that black heat shrink wrapped thing in the bottom right in the middle photo? Looks like a DC jack :smiley: 

@lox897 Im looking at using 20 cells total so hopefully 2 parallel will work for me. Im trying to keep the cost and space down as I don't really travel far on one charge. 

Thanks for the kind words about my website, as part of my university course I'm looking for internship opportunities next year so its a good way to make a good first impression with my work! Cheers

Jack
```

---
## \#13 Posted by: lox897 Posted at: 2015-12-22T11:15:07.973Z Reads: 1053

```
Yeah, it will give you 5.2amps/5200mah. According to chaka if your going 30 mph (depends on weight, gearing, hill/no hill etc) you will be drawing 20 amps 740 watts. Your batteries should have a 20 amp constant rating and your BMS at 40 amps should be fine. If anyone can explain this in more detail or more correct that would be good.
```

---
## \#14 Posted by: lox897 Posted at: 2015-12-22T11:16:39.648Z Reads: 1026

```
I'd use a watt meter on your board now and see how many watts you are pulling then you can tell us that and then people can tell you what you need.
```

---
## \#15 Posted by: Jack Posted at: 2015-12-22T11:18:49.348Z Reads: 1030

```
Yeah there is a lot of conflicting info here. Thats why I'm trying to get to a point where theres some solid data and easy to build pack for e-boards. Unfortunately my board is down as my ESC went into meltdown. I'm waiting for 10 VESC PCBs from china which should be here in the next few days.
```

---
## \#16 Posted by: cmatson Posted at: 2015-12-22T15:05:51.665Z Reads: 1043

```
I'm sure you've seen this thread I put up, but I'd be happy to give you any more detailed pics if you're looking for something specific. 

Here's the thread though for anyone interested 
http://www.electric-skateboard.builders/t/space-cell-opened-up/510
```

---
## \#17 Posted by: psychotiller Posted at: 2015-12-22T16:57:42.097Z Reads: 978

```
Where can I buy these from? Do you have a link? (I'm talking about the charge plugs)
Thanks!

Edit! I found some
```

---
## \#18 Posted by: stuxtruth Posted at: 2015-12-22T18:00:48.184Z Reads: 958

```
Where did you find them?
```

---
## \#19 Posted by: psychotiller Posted at: 2015-12-22T18:24:02.241Z Reads: 957

```
On Amazon. Bought 10 for under 4 bucks with frees shipping
```

---
## \#20 Posted by: scoobiext Posted at: 2015-12-23T01:57:33.147Z Reads: 1034

```
Thanks for your comments Jack.

Sorry for confusing the issue, the cells, BMS and wiring diagram in your original post would all work.  Also given that the original space cells are 40A rated I would assume that 40A is enough to power a e-board and you should be right to go with your intended setup.

You are right with regards to the battery capacity.  The battery capacity will be the total of the single cell capacity times the number of parallel cells.  The discharge current is also the total of the single cell discharge times the number of cells in parallel (e.g. for 2P @ 20A = 40A and 3P @ 20A = 60A).  I think LG make a high discharge 3000 mAh cell so if you wanted a little more range you could go down that track, although as you say you you don't need to go too far on one charge

The range of a battery pack depends on the energy stored in the battery pack and the amount of load on the battery.  The stored energy in the battery can be worked out by multiplying the battery capacity with the battery voltage.  For example a 10S2P pack with a single cell capacity of 2500mAh ( a total of 5 Ah) would give you 180 Wh, To work out how long this battery back would last you need to divide the amount of available energy by the load.  So for a continuous 740w load, this battery pack would last about 15 minutes.  Note that it would be unusual to have a continuous load in a e-board application and real world figures would suggest that you would get more like double this run time.

The main reason I went to a 3P pack was to achieve a higher maximum discharge current to allow for the extra load when I go up hills, and so I could run two motors.   Having said this I think it would be very rare that I would even get close to 60A's.  You can decrease the amount of current drawn from a battery by placing more cells in series.  To explain this, P(power) =V(volts) x I(amps),  so in lox897 example if you use 10S (36V) you would draw a nominal current of 20A, if you stepped up to 12S (43.6V) you would only draw about 17A (sorry if this is teaching you to suck eggs).  I guess the important thing with current draw is to give yourself a bit of a buffer between your expected current draw (load) and the battery maximum continuous discharge for instances when you use more current such as going up hills and starting.

I am happy with my BMS and I haven't noticed any signs of over heating (its hard to check when you are using the board).  The BMS you have linked to actually looks very similar in design to mine, just a little smaller which can probably be attributed to the lower current rating.  Basically you need to match your BMS cutoff current with the maximum continuous discharge of the batteries, which you have in your example. I would be a little reluctant to put the BMS on top of the batteries as you will get some heat from the BMS (mostly through the transistors/FETs, but also a little from the discharge resistors). If you shield the batteries enough from the heat from the FETs you will probably be okay though.

The shrink wrapped thing in my pictures is a capacitor which is wired to the battery terminals of the speed controller.  I have since swapped this style of cap to the cap board used by others such as Vedder, Enertion and Chaka.

You mentioned your board is very flexible, I would be careful with this with any battery pack that is assembled using solid links.  For your application you might be better of wiring each set of cells together with flexible wiring to ensure there are no torsional loads placed on the links between packs.  This is partially the reason I have my battery back sitting in a CF tray.

Sorry for the long winded reply but hopefully this helps.
```

---
## \#21 Posted by: Jack Posted at: 2015-12-25T16:42:37.631Z Reads: 873

```
@scoobiext great thanks for that I've just realised after ordering 40pcs of the Samsung 18650-26f that they are only rated to 5A discharge per cell. So that's not going to work :(

I'm thinking is it possible to attach a bms to the zippy lipo packs?  Add another 3s pack for 9s and just connect the bms to the balance plug?
```

---
## \#22 Posted by: jrocca122 Posted at: 2016-04-25T17:20:59.307Z Reads: 822

```
@scoobiext How did u wire the 12S BMS with the 10S battery?
```

---
## \#23 Posted by: scoobiext Posted at: 2016-05-06T07:49:25.726Z Reads: 813

```
G'day Jrocca122

My BMS is a 10S BMS.  I'm fairly sure the same company do make a 12s BMS if that is what you are after.
```

---
## \#24 Posted by: jrocca122 Posted at: 2016-05-06T20:01:40.412Z Reads: 803

```
@scoobiext I was only asking because the link you put early in this topic for your BMS is for a 12S BMS, and I accidentally ordered it
```

---
## \#25 Posted by: delta_19 Posted at: 2016-05-07T00:12:37.330Z Reads: 788

```
Easy fix, how many cells are you using?
```

---
## \#26 Posted by: jrocca122 Posted at: 2016-05-07T01:22:44.378Z Reads: 778

```
@delta_19 i'm making a 10S
```

---
## \#27 Posted by: delta_19 Posted at: 2016-05-07T04:43:33.853Z Reads: 778

```
Yeah but you ordered a 12s bms. Depending on how many cells you have you can still use it.
```

---
## \#28 Posted by: seanpain4 Posted at: 2016-05-07T07:17:55.411Z Reads: 792

```
@jrocca122 If you are making a 10S and you have a 12s BMS it will still work. Also allows you to upgrade at a later date.
```

---
## \#29 Posted by: whitepony Posted at: 2016-05-07T19:55:36.004Z Reads: 850

```
ive explained quite often by now in various threads why I think a bms isnt super important really.

what do you want from your bms?

* cut off when voltage is above upper threshold (charging, probably 4.xV/cell)
* cut off when voltage is below lower threshold (riding your board, probably 3.xV/cell)
* balance the parallel packs (parallel packs can drift, cells can age, maybe your superhot mosfets of the vesc heat up some cells a lot, others stay cool and age less, etc etc there are many reasons why different parallel packs can develop slightly different charge states)

now, for charging I use my evolve charger,  it cuts off at 41V on my 10S packs -> charging by single jack, no overvolt protection required! one off the bms list!

during riding, my battery is protected by the vesc settings. im using 32V soft off, 30V lower threshold, so when my board slows down I know that I hit 32V, then I got a few kilometers until it will be dead! another point off the bms list!

finally: drifting! I was aware and extremely afraid of this effect, I build up my batteries carefully and every pack equal, I have heat protection between vescs and cells but I still was afraid of drifting. the first battery I build was for my evolve carbon, 10S6P. I monitored the parallel packs on my balancer output every 2 weeks. then every 4, then finally just whenever I had the case open for whatever reason. in one year of heavy and daily commutes of 20km, I still had zero drift in the cells.

next was my 10S4P battery of LG HG2 cells. coming from my evolve battery, I just went without a BMS, since high current BMS are actually quite expensive and I wanted to use the 80A of the battery and not cut it down to 40A just because I couldnt find a small and powerfull BMS. so I went without a bms for now and started monitoring again. the battery has come a long way, probably 1500-2000km and just a week ago I hit 40km max range on my tesseract carbon build with a single motor. so the battery is still very healthy and again: ZERO drift of the cells.

and even IF the packs were drifting, there is still a headroom of 0.1V to 4.2V per parallel pack (charged only to 4.1V per cell/pack) since my battery is charged only to 41V and only discharged to 30V.

I started to believe, that if you buy quality cells and if you know exactly whats good and whats bad for lithium chemistries (and of course avoid the bad things), there isnt really a need at all for a bms! however, I would still add the balancer cables so you can check the parallel packs with your multimeter every now and then, just to be sure.

:slight_smile:
```

---
## \#30 Posted by: seanpain4 Posted at: 2016-05-08T05:59:18.471Z Reads: 769

```
Do you mean series packs drifting? As when two cells are in parallel they will balance out with each other. Series packs will drift over time without being balance charged or without a BMS. 

If you buy really good quality cells and they are all the exact same, chances are you can get away with not having a BMS, but after a while it would still be recommended to balance them out by adding a BMS or using a balance charger, or even remove the series connection and put them in parallel and wait a few days for it to balance.
```

---
## \#31 Posted by: ILLU Posted at: 2016-05-23T13:25:56.484Z Reads: 730

```
So if i will have a setup like 10S4P based on SAMSUNG INR18650-25R, 2500 mph (decelerated 20A) i need to buy 80A BMS?
When it's like 10S3P = 60A? What about series number, if BMS will be dedicated for 12s, it's still fine to use it with 10s?
```

---
## \#32 Posted by: delta_19 Posted at: 2016-05-23T16:50:05.482Z Reads: 703

```
the series number HAS to match the battery you are building but the max amp dis charge does not have to match your max discharge and would be better if it was lower. so you could use a 60A bms on a 10s4p set up no problem but not a 10s4p set up on a 12s bms.
```

---
## \#33 Posted by: KMeyerson Posted at: 2016-05-23T19:13:01.053Z Reads: 701

```
I'm thinking of repacking/rebuilding a Yuneec 7s3p battery to hold 10s2p.  Who can I trust to tab my battery?

I'm also looking for advice on 10s BMS. I might just do it myself because the Yuneec battery pack is tight on space.
```

---
## \#34 Posted by: seanpain4 Posted at: 2016-05-23T22:34:16.984Z Reads: 699

```
@delta_19 A fair few BMS' allow you to setup a battery with a lower cell count than what it is rated for
```

---
## \#35 Posted by: ZeVinner Posted at: 2016-08-11T00:15:30.434Z Reads: 645

```
I'm making a 10S2P battery and have one 36V 10S BMS that can handle 80A discharge. How would I go about wiring the bms to the 20 cells? I'm trying to keep the battery as flat as possible.
```

---
## \#36 Posted by: Pantologist Posted at: 2016-08-11T00:24:43.098Z Reads: 662

```
You have to write your balance connectors to each pack of series.

Check this for more details. http://www.electric-skateboard.builders/t/connecting-a-bms-quick-guide-how-to/6122
```

---
## \#37 Posted by: Jinra Posted at: 2016-08-11T00:42:38.841Z Reads: 670

```
You shouldn't plan on an 80A discharge current on 2p if you're running 18650 cells. 18650's normally output about 20 per cell (40a in 2p) but you should really plan on using it for 10a per cell.

I'd recommend adding another 1 or 2 parallel groups in your pack. Even with a higher discharge pack you'll probably need a 60A BMS at most, or just bypass the BMS for discharge.
```

---
## \#38 Posted by: ZeVinner Posted at: 2016-08-11T01:03:09.311Z Reads: 653

```
will using the 80A BMS have a negative effect on the cells? I thought that getting a bms that can handle more than the 18650 cells output is fine.
```

---
## \#39 Posted by: ZeVinner Posted at: 2016-08-11T01:03:41.738Z Reads: 649

```
There was a very helpful diagram on that thread, thank you :slight_smile:
```

---
## \#40 Posted by: Jinra Posted at: 2016-08-11T01:19:27.336Z Reads: 651

```
it's fine but why spend the extra money and space? if you want a smaller pack getting a lower discharge bms will save space as well
```

---
## \#41 Posted by: ZeVinner Posted at: 2016-08-11T01:21:39.222Z Reads: 577

```
I'm planning to add 2 more 10S packs later, just planning for the future.
```

---
## \#42 Posted by: Jinra Posted at: 2016-08-11T01:23:22.506Z Reads: 583

```
you'll most likely be fine with a 60A bms don't think you'll need 80.
```

---
## \#43 Posted by: jrpwit Posted at: 2016-08-11T03:13:46.601Z Reads: 592

```
Bigger packs last much longer. I would recommend at least 3 parallel. Street boards won't pull more the 30A from what I have read so 80A is way over kill. Usually people only pull 5 amps when riding.
```

---
## \#44 Posted by: ZeVinner Posted at: 2016-08-11T03:28:20.030Z Reads: 605

```
well then, I'll downgrade when I can.
```

---
## \#45 Posted by: paragon Posted at: 2016-08-11T03:31:05.891Z Reads: 613

```
This may interest you:
http://www.electric-skateboard.builders/t/10s-li-ion-bestech-bms-55-shipped-in-the-usa/7331
```

---
## \#46 Posted by: jrpwit Posted at: 2016-08-11T03:59:29.678Z Reads: 607

```
If you already purchase the 80A bms just use it. Overkill is not bad or anything if anything its a good thing cause things then run cool. Heat is wasted energy and just damages things. Also I do not get the BMS paragon is selling. It is only rated for 20A continuous. For e-skate 40 amp is the bare minimum. 60A will work for everything and 80A also would work just as well if not better.

I would feel bad if you got a new BMS even though it would work perfectly fine.
```

---
## \#47 Posted by: Jinra Posted at: 2016-08-11T04:53:49.247Z Reads: 589

```
Yea if you already have a bms it's no problem. Just know you can go smaller and be fine. Paragon's bms is a good choice too if you bypass it for discharging.
```

---
## \#48 Posted by: ZeVinner Posted at: 2016-08-11T05:25:12.915Z Reads: 567

```
yeah, I already have the 80A bms, it's 2 times the size of a normal one but that shouldn't be too big of a problem because my deck can accommodate it.
```

---
## \#49 Posted by: jrpwit Posted at: 2016-08-11T06:21:41.102Z Reads: 577

```
Great! Again there is no need to downgrade to 60A unless you want something a little smaller. Overspecing your board will make it last longer in the end :slight_smile:
```

---
## \#50 Posted by: jbruce Posted at: 2016-11-14T01:18:33.068Z Reads: 458

```
Just wondering if anyone knows the BMS's charging procedure when charging these li-ion cells. For example can it regulate the inputted voltage and amperage so that you're not frying your battery, and does it balance each cell while charging like a normal hobby battery charger would? BMS's seem very convenient but if they're charging the battery in an incorrect manner I wouldn't want to use one.
```

---
## \#51 Posted by: Jinra Posted at: 2016-11-14T01:31:29.910Z Reads: 450

```
Most BMS's work by charging from a single source and measuring voltage across each cell as it's charging. Once it hits the balance voltage (about 4.18v) it will switch to a lower balance charge current which will keep all cells in balance. You'll want to read the documentation on the BMS you're interested in to make sure it fits your needs.
```

---
## \#52 Posted by: Roger Posted at: 2016-11-16T19:25:42.636Z Reads: 456

```
Hello i'm trying to do a 10s lipo pack with two 5000mah 5s batteries and wire to the bms for easy charge. So i need help to how i can wire the batteries with the bms and a swithc on and off. 

Can you help me with some pictures or examples that you made...

Thanak'u
```

---
## \#53 Posted by: Jinra Posted at: 2016-11-16T19:40:10.442Z Reads: 448

```
You'll need a BMS with an e-switch. Wiring is dependent on the BMS you get, so how 1 person does it may be different than how another does it. Check here for examples.

http://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179
```

---
## \#54 Posted by: Tuomalar Posted at: 2016-11-16T21:31:14.615Z Reads: 434

```
European e-skaters. Is there any european bms dealer? It's almost cheaper build 2 x 10s packs than one with bms.
```

---
## \#55 Posted by: Roger Posted at: 2016-11-17T19:33:04.101Z Reads: 437

```
Hello how fast i can go and long with a 190kv motor and 6s4p pack? And with a 10s3p, 10s4p? 

I'm starting with diy electric lognboards so i do not know by a 100% wich option is better because probably a 10s pack i so much... I don't know

Thank'u so much
```

---
## \#56 Posted by: chinzw Posted at: 2016-11-17T22:05:24.697Z Reads: 441

```
Depends on your gearing ratio, wheel size, your weight, etc.
6s = 22.2v
10s = 37v

So:
22.2v x 190kv = 4218rpm
37v x 190kv = 7030rpm

As you can see 10s is about 60% faster.

And for range you would need to provide the data on the cells you want to use as they have different Ah ratings.
```

---
## \#57 Posted by: jbruce Posted at: 2016-11-20T08:37:24.304Z Reads: 432

```
So let's say I have a 8s pack with bms that is fully charged at 33.6v and I input 36v. Will this over charge my batteries or is the bms able to regulate the voltage and not over charge the batteries? Also does a soft switch work as an anti spark switch?
```

---
## \#58 Posted by: Jinra Posted at: 2016-11-20T08:39:22.207Z Reads: 432

```
Check the BMS datasheet, but it should prevent your individual cells from going beyond the specified voltage. An e-switch would negate the need for an anti-spark switch.
```

---
## \#59 Posted by: jbruce Posted at: 2016-11-20T08:41:12.698Z Reads: 435

```
Ok thanks!! Any idea how the e switch works to slow the charge of the capacitors in the esc? @Jinra
```

---
## \#60 Posted by: Jinra Posted at: 2016-11-20T20:51:01.623Z Reads: 436

```
Sorry don't know the answer to that question
```

---
## \#61 Posted by: chinzw Posted at: 2016-11-21T22:45:23.598Z Reads: 412

```
You can read about it here:
https://endless-sphere.com/forums/viewtopic.php?f=3&t=40142
```

---
## \#62 Posted by: Jebe Posted at: 2017-04-04T09:34:03.657Z Reads: 352

```
How good is little creatures !
```

---
## \#63 Posted by: barkgrind Posted at: 2017-08-05T10:04:57.926Z Reads: 290

```
hey mate what deck you running in this photo? 
thanks
```

---
## \#64 Posted by: Ronny_CTS Posted at: 2017-08-05T13:20:07.629Z Reads: 280

```
Looks like a Loaded Poke to me.
```

---
## \#65 Posted by: Redfire1 Posted at: 2018-03-29T05:58:10.863Z Reads: 166

```
@seanpain4 and anyone who know,![image|470x500](upload://6qRKT9lCH3970zgppvLdgFd0biv.jpeg)![image|375x500](upload://djCLTghhICmx9qy9QHpuL8AeJDv.jpeg)I have bought a BMs for my 2 5s connected in series (10s) can I used it for discharging my cells or just charging
```

---
