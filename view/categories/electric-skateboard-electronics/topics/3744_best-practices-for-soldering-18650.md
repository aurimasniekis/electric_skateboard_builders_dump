# Best practices for soldering 18650?

### Replies: 53 Views: 46507

## \#1 Posted by: Maxid Posted at: 2016-05-24T08:07:45.980Z Reads: 785

```
Hi guys,

I would like to build my own 18650 pack. I was thinking of Samsung 25R cells and 2x5S packs in series with 3 or 4 cells in parallel. This way I could balance charge them separately with my 6S charger and would not need a BMS.
However for a single battery it is not economical to buy a spot welder so soldering is my only chance.
After reading about nickel strips, or copper welding rods for the connection of cells I was wondering what the actual best method for soldering 18650 packs is. Can you simply use 10mm^2 cables, remove the insulation at the position of a cell and solder them onto the cell? Or use 2x6mm^2 speaker cables?
Also I read about the danger of the cells becoming hot - can that be solved by dipping the rest of the cell into a liquid (distilled water or isopropyl) to allow for fast heat dissipation while soldering the cable onto the other end?

If there is a tutorial on how to solder 18650 packs let me know - so far I only read about finished products and not so much about the actual process.
```

---
## \#2 Posted by: seanpain4 Posted at: 2016-05-24T08:14:41.255Z Reads: 758

```
Usually easier to solder with copper rod. To minimize the contact time of your soldering iron on the cell, make sure the surface is scuffed up sufficiently and you use plenty of flux to allow for fast solder flow. To keep it cool i would suggest using compressed air before and after making the soldering connection. 

Also, one other thing, it is better to have a good quality high wattage iron with good thermal capacity so it can deliver the heat to the joint quickly so you don't have to hold the iron to the battery for ages and let the heat seep into it, causing damage to the battery.

Safety wise, it really isn't that dangerous, especially because you are buying good quality cells. I have soldered 100's of used laptop cells without any issue.
```

---
## \#3 Posted by: Maxid Posted at: 2016-05-24T08:38:44.590Z Reads: 729

```
[quote="seanpain4, post:2, topic:3744, full:true"]
To keep it cool i would suggest using compressed air before and after making the soldering connection. 
[/quote]

I once saw in a video that you should never blow on a fresh solder joint because the rapid cooling would cause wrong crystallization of the solder and decrease the quality of the joint. 
I usually don't care for my simple joints with LEDs and stuff but was wondering if this is an actual issue when soldering batteries - especially for the type of high currents we use?
```

---
## \#4 Posted by: seanpain4 Posted at: 2016-05-24T08:48:48.186Z Reads: 688

```
I don't mean rapidly cool the joint. You cool the cell then work your way up to the top, and by then the joint will be cool enough for the direct cold air. It is the internals you need cold. 

The tip of the cell doesn't transfer a ton of heat to the cell due it it not being 100% connected, as you would be able to see on the top around the positive terminal.
```

---
## \#5 Posted by: Bender Posted at: 2016-05-24T12:29:05.204Z Reads: 666

```
What about freezing them beforehand or would that damage the cell?
```

---
## \#6 Posted by: Maxid Posted at: 2016-05-24T12:35:59.350Z Reads: 660

```
[quote="seanpain4, post:4, topic:3744, full:true"]
I don't mean rapidly cool the joint.
[/quote]

So blowing on a joint is indeed not a good idea? I will probably be terrified to just leave the joint to cool on its own when there is a battery involved ;)
```

---
## \#7 Posted by: delta_19 Posted at: 2016-05-24T12:39:02.610Z Reads: 640

```
Blowing on the joint is bad, yes.
```

---
## \#8 Posted by: seanpain4 Posted at: 2016-05-24T12:45:44.918Z Reads: 629

```
Your goal is to have the cell stay cool, not frozen and to allow the joint to cool normally.
```

---
## \#9 Posted by: chaka Posted at: 2016-05-24T14:08:18.857Z Reads: 626

```
No need to scuff the cells, you are soldering nickel to nickel. Use a good liquid flux and pre-tin your cells with a little pool of solder hitting them with a wet sponge after removing the iron.  We only scuff metals that have oxidation, remember soldering is not a mechanical bond.
```

---
## \#10 Posted by: chaka Posted at: 2016-05-24T14:17:11.806Z Reads: 613

```
And please use at least an 80 watt iron to do this. You have to get in and out quick. If you use a little smd iron you will need to let the iron dwell for much too long and the cell will get hot.
```

---
## \#11 Posted by: Maxid Posted at: 2016-05-24T15:32:40.522Z Reads: 599

```
I was going to use a 85watt weller iron (450°C max. temperature).
Also I am not using nickel strips but either copper desoldering braid, thick cables or welding rods.
What is the sponge for? I thought rapid cooling is not ideal.
```

---
## \#12 Posted by: chaka Posted at: 2016-05-24T15:52:53.074Z Reads: 592

```
It not that rapid, it will be fine. Don't scuff the cells, do scuff the bare copper. I wouldn't use anything too rigid to join the cells. Something flexible is better, more resilient.
```

---
## \#13 Posted by: Ulfberht Posted at: 2016-05-24T19:21:13.069Z Reads: 590

```
I use a Weller 85w WD-1 soldering station and it gets the job done WELL!! If you are using the WP-80 or WSP-80, you will most definitely want to get a nice fat chisel tip. retains temp well and transfers loads of heat quilckly.
 I use the  Weller LTD 4.6mm chisel tip. http://www.ebay.com/itm/WELLER-LTD-Solder-Tip-Chisel-4-6mm-/331348517512?hash=item4d25e92288:g:eDkAAOSwNsdXRJRj
Also, it should go without saying, but you gotta tin those leads up before you try to attach them to the cells. 2-3 seconds per joint max should get it done. :v:
```

---
## \#14 Posted by: Glenn Posted at: 2016-05-26T15:30:59.199Z Reads: 568

```
I do my battery's with a 200 watt soldiering iron. In and out fast, and afterward you need to test your weld by tugging on lead. I've made about 8 battery packs this way.<img src="/uploads/db1493/original/2X/c/ccd561cad55f5ad904f3f576f6272b67138e0c46.jpeg" width="500" height="500"><img src="/uploads/db1493/original/2X/e/e242f25864bc147bbb0e46416b554a28f83ebd83.jpeg" width="500" height="500">
```

---
## \#15 Posted by: c4Lvin Posted at: 2016-05-27T00:49:36.252Z Reads: 552

```
I'm also interested for the first time of making my own 18650 battery. I plan on running dual R-Spec 190Kv motors and would a 10S3P be good enough for a 170lb rider like me? I'm looking for 10-15 miles which I'm sure will be quite tiring after that distance since you're constantly leaning on side or the other. Anyhow, I've been searching and what cells are good? I mean I know LG and Samsung or Panasonic/Sanyo are the best but what specs are good? Is 10A discharge enough for this setup? I will also be soldering them since I don't have a spot welder :( Thanks in advance everybody.
```

---
## \#16 Posted by: Jinra Posted at: 2016-05-27T00:56:28.423Z Reads: 549

```
You're pretty much building a raptor, so yea, you should be able to get that mileage no problem. As for cells, Enertion uses Samsung 25R's for their space cells. I've also heard good things about a123's LiFePo4 cells if you want to go that route. Legit Panasonic and LG cells are a good choice too. You'll probably want 50A+ continuous (rating for the VESC) at least, which means a 3P pack of 25R's would suffice (60A continuous). Make sure you get a 85w+ iron if you're going to solder as the less time in contact with high heat for the battery, the better.
```

---
## \#17 Posted by: c4Lvin Posted at: 2016-05-27T01:00:21.925Z Reads: 544

```
Thank you. I was looking at the Panasonic NCR18650PF which stated that it would have 4000 charge cycles. But it does say each cell is 10A only. Would that be OK for my setup if I built it 10S3P? Perhaps not since that would be only 30A or so continuous? I'm sorry for these dumb questions but I guess it's never too late to learn. Thanks guys.
```

---
## \#18 Posted by: Jinra Posted at: 2016-05-27T01:19:40.359Z Reads: 533

```
you'd probably want a different cell that can handle more continuous discharge. Also where did you read 4000 cycle count? That's abnormally high for a li-ion cell.
```

---
## \#19 Posted by: c4Lvin Posted at: 2016-05-27T01:29:08.843Z Reads: 529

```
I saw it on eBay. http://www.ebay.com/itm/100-Genuine-Panasonic-NCR18650PF-18650-2900mAh-3-7v-lithium-ion-cells-USA-seller-/162052006286?hash=item25bb0d618e:g:VcIAAOSweW5VWsHE Just exaggeration? Just wondering I was searching for the Samsung 25R and states that the cycle life is only 250? That's very low for any Lithium Ion battery isn't it? I mean that's like Lithium Polymer low! Can anyone expand on that? I know I like LifePO4 since I got an eBike (Prodeco) with it. They are not as energy dense but safe all around. A little pricey but hopefully they will come down with time..as with everything else.
```

---
## \#20 Posted by: Jinra Posted at: 2016-05-27T01:34:06.691Z Reads: 520

```
250 is about the right cycle count for 70%~capacity. Keep in mind this is done in a test environment discharged to 2.5v and recharged to 4.2v. This puts a lot of strain on the battery so if you treat it well it should last a good amount more than that. It doesn't flat out die at 250 cycles, just losses a bit of capacity over time. LiFePo4's are heavier and less dense, but provide over 2000 cycles.
```

---
## \#21 Posted by: c4Lvin Posted at: 2016-05-27T01:43:42.744Z Reads: 495

```
Wow that I didn't know about them testing the battery down to 2.5V! I'm still trying to absorb the 25R's 20A continuous and 35A peak specs. It can strain my old brain! What's a good price per battery for the people that has already built their packs? I know I should not buy those cheap fake China ones.
```

---
## \#22 Posted by: Jinra Posted at: 2016-05-27T01:45:54.060Z Reads: 482

```
If you live in the states you can find 25r's for $5 each easily.
```

---
## \#23 Posted by: philipp Posted at: 2016-06-02T11:51:04.259Z Reads: 465

```
Can someone explain to me why the most used batteries seem to be samsung 25R's?
I've used them for my e-cigarettes way back, but switched to  LG's 18650HG2 because the performance was way better.

They offer 500mAh more per battery, and significantly higher discharge rate.
```

---
## \#24 Posted by: flatsp0t Posted at: 2016-06-02T12:24:45.336Z Reads: 454

```
I think its mostly the price.
They are nearly double the price.

This may not make a huge difference on the few cells you need for smoking, but does on 40-70 cells.
```

---
## \#25 Posted by: Maxid Posted at: 2016-06-02T12:30:35.375Z Reads: 447

```
[quote="philipp, post:23, topic:3744, full:true"]
Can someone explain to me why the most used batteries seem to be samsung 25R's?
They offer 500mAh more per battery, and significantly higher discharge rate.
[/quote]

HG2: ~5.75€ per cell --> 522mAh/€
25R: ~3.65€ per cell --> 685mAh/€
```

---
## \#26 Posted by: flatsp0t Posted at: 2016-06-02T12:33:10.303Z Reads: 439

```
Where do you get your cells?
```

---
## \#27 Posted by: philipp Posted at: 2016-06-02T12:40:00.731Z Reads: 443

```
So it's the price... okay :)
I've found genuine HG2 for 6$, but couldn't find 25R under 5$.
Where did you get these prices from?
```

---
## \#28 Posted by: Maxid Posted at: 2016-06-02T12:56:12.292Z Reads: 428

```
https://eu.nkon.nl/ seems to be the cheapest shop I could find for 18650 batteries.
```

---
## \#29 Posted by: flatsp0t Posted at: 2016-06-02T12:59:30.729Z Reads: 432

```
Nice, they are cheap AF
```

---
## \#30 Posted by: Pantologist Posted at: 2016-08-10T15:46:30.059Z Reads: 423

```
Is there a special solder and flux to use for soldering to nickel strips? I want to attach my balancing leads. 

I've seen people recommending using Aluminum solder and flux. Is that the stuff to get?
```

---
## \#31 Posted by: themegak Posted at: 2016-08-10T17:15:22.638Z Reads: 430

```
I would recommend skipping the whole soldering directly onto the cells if you can.  Have you considered using 18650 sleds ?  You can do your series/parallel soldering before even placing the batteries inside the sleds and if you ever need to replace a bad cell, it will be super easy to do without risking heating / desoldering individual cells.  Below is what i am talking about and i think you can get them in any number combination you want on ebay for very low cost.  Definitely worth considering.  <img src="/uploads/db1493/original/2X/a/ad96bdd9bfe2f870b74d47130abbb55cbfeb64b6.jpg" width="500" height="500">
```

---
## \#32 Posted by: Jinra Posted at: 2016-08-10T17:26:58.202Z Reads: 408

```
I believe the reason sleds aren't used is because of high current and heat that the sleds can't withstand. I'm guessing the plastic will warp and deform and the constant vibrations may make for a poor connection to the cells since they're not soldered or welded on.
```

---
## \#33 Posted by: themegak Posted at: 2016-08-10T17:41:14.095Z Reads: 407

```
Don't you think heat shrink or some kind of wrap treatment would solve that problem ?  I think Enertion at some point was using sleds in their Space Cell.  Not sure what they are doing now but it would be the sled along with some kind of wrapping to assure everything stays together and is protected.
```

---
## \#34 Posted by: Jinra Posted at: 2016-08-10T17:43:55.580Z Reads: 398

```
I mean the housing for the nickel strip would melt. Enertion never used sleds, but they did use 18650 spacers which are a bit different as they dont' have a nickel strip on them. They just welded the tabs on.
```

---
## \#35 Posted by: Pantologist Posted at: 2016-08-10T17:46:53.717Z Reads: 398

```
Does anyone actually know what to use to solder to nickel strips though?
```

---
## \#36 Posted by: Jinra Posted at: 2016-08-10T17:51:09.644Z Reads: 397

```
I'm sure traditional 60/40 solder would work. That's what I'm planning to use with my build.
```

---
## \#37 Posted by: lox897 Posted at: 2016-08-10T20:31:35.690Z Reads: 395

```
Ask @whitepony. He would know
```

---
## \#38 Posted by: whitepony Posted at: 2016-08-10T21:11:58.656Z Reads: 406

```
Im using standard 60Sn/40Pb (actually 60% Sn, 38% Pb and 2% Cu) too with a soldering flux pen for easy application.
```

---
## \#39 Posted by: brawlincollin Posted at: 2016-11-11T03:14:10.471Z Reads: 362

```
What type of soldering iron do you use? Do you need one that get really hot?
```

---
## \#40 Posted by: lowGuido Posted at: 2016-11-11T04:26:43.969Z Reads: 361

```
standard solder with a good quality iron, probably set around 350degrees
```

---
## \#41 Posted by: Jinra Posted at: 2016-11-11T04:28:21.194Z Reads: 344

```
i soldered at my max 480C, worked great.
```

---
## \#42 Posted by: brawlincollin Posted at: 2016-11-11T04:39:48.575Z Reads: 342

```
Is there a specific watt iron I should buy?
```

---
## \#43 Posted by: Puchuumetal Posted at: 2016-11-18T17:35:37.941Z Reads: 327

```
I only have a 48 watt iron is that gonna be powerful enough it goes all the way to 450 max? And is 62/36/2 rosin core silver bearing solder ok?
```

---
## \#44 Posted by: Eboosted Posted at: 2017-01-23T07:34:11.034Z Reads: 304

```
I've read a lot of people around here advising not to use soldering irons on 18650 batteries because the heat damages them, spot welding seems to be the common practice to build battery packs. 

I went and started my build with a soldering iron and its going pretty good, 3-4 seconds on each cell to bond the nickel strip. 

But how would you test if there was any damage done to the soldered cells? Would there be a way  to test them?
```

---
## \#45 Posted by: willpark16 Posted at: 2017-01-23T07:56:06.915Z Reads: 297

```
Test voltage is what I do when I solder mine , I also bench test for 2 days before riding but that's because I'm paranoid
```

---
## \#46 Posted by: IDVert3X Posted at: 2017-01-23T08:01:14.687Z Reads: 290

```
The only way to tell is by measuring capacity.
Get 200W soldering iron and do it super quickly.
```

---
## \#47 Posted by: B4Me Posted at: 2017-01-23T09:52:01.702Z Reads: 284

```
I did NOT read the rest of the thread, but you can find guides to build a small capacitor based spotwelder for cheap, it is better for the cells, as soldering destroys some of the internal of the cells 
Saw a video of a person rolling a soldered and spot welded battery out, the soldered was discolored on the inside almost 5-8mm down :frowning:
Dont know the impact of the life, but discoloring is normally not a good thing
```

---
## \#48 Posted by: lowGuido Posted at: 2017-01-23T10:11:32.022Z Reads: 277

```
I solder them all the time. Infact I would be so bold as to suggest that soldering is a much better connection than miniscule spot welds.

However an inexperienced solderer may have apply too much heat to the battery and thats bad.

A skilled solderer should be able to solder a battery tab in seconds.
```

---
## \#49 Posted by: Eboosted Posted at: 2017-01-23T14:37:07.460Z Reads: 271

```
I used between 4 and 6 seconds of solder time on each pole, the voltage everytime was exactly as it started, the solder was noticeably better than the spot welding I was doing before, you can not tell if the spot weld is good enough by just looking at it, you need to pull the nickel to strip it off with pliers and see if it holds.

So is there another way to test the battery capacity to see if there has been any damage besides measuring the voltage? Or people says it's bad without scientifical proof?
```

---
## \#50 Posted by: Guacamoleface Posted at: 2017-01-23T17:38:02.937Z Reads: 285

```
I just soldered a 10s4p a week ago, 90w iron, was really quick. Made the mistake to be abit rushed on one of the paralells and soldered another battery to the same copper braid abit to early, and copper leads the heat very fast.
Battery didnt feel to hot but I can almost say it must've gotten really hot, it survived for now, will see how it will hold up with time :) but thats one thing to think about I guess,else it was pretty simple aslong as the surface was ruffed up abit.

Worth to mention Im rusty at soldering as I have not done it all that much for the last couple years.

Im also not sure if the damage it would make shows in long term effects or straight onto the voltage as you work, heard abit of both but never anything to convince me whats correct or not.
```

---
## \#51 Posted by: kbazzy98 Posted at: 2017-02-13T05:10:27.537Z Reads: 269

```
If you're using old laptop batteries like me, it doesn't matter, these old batteries have been over heated many times, a couple seconds with the iron is not gonna do permanent damage.
```

---
## \#52 Posted by: Lucajo16 Posted at: 2018-11-02T22:02:25.458Z Reads: 87

```
Hay guys I'm just gonna add this in here for the people thinking of soldering your batters together....its not safe...if they get to hot they will fail and I don't think you want to be half way into a build and the batter your on go's south. I do have an alternative option....in the world of Arduino there are portable spot welders that you can use. they use a small lipo battery to charge but its much better and gives you more room then a desktop spot welder. here is the link to one I'm buying here [soon](https://www.ebay.com/itm/Arduino-S2-Spot-welder-Soldering-Iron-for-Hakko-T12-EMS-Shipping/202487588570?hash=item2f253366da:g:dnUAAOSwNWhb2ZSS:rk:1:pf:0) . this will save you guys the trouble of having to buy a spot welder and a solder at the same time. I live in an apartment and its old....so I don't think I can use a normal spot welder. I fear ill start a fire or something.
```

---
## \#53 Posted by: flyb0i Posted at: 2019-10-17T04:35:23.549Z Reads: 32

```
Soldering onto the cells could damage safety vents and the CID (Current Interrupt Device). You won't know that you damaged these until it's too late and the cell could fail in a very dangerous manner, such as an explosion or runway thermal event. Unless you are a very expert solderer and have the right equipment, I wouldn't attempt it. In fact, since it's impossible to tell if you damaged these things, I would just avoid soldering altogether.
```

---
