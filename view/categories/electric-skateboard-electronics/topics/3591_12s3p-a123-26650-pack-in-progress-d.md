# 12s3p A123 26650 pack in progress :D

### Replies: 59 Views: 9739

## \#1 Posted by: L3thaltank Posted at: 2016-05-21T07:37:05.510Z Reads: 653

```

**A123 26650 Cells:**
http://www.a123batteries.com/product-p/anr26650m1-b.htm

**BMS:** 
http://www.ebay.com/itm/321746365404?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

**Charger:**
http://www.ebay.com/itm/321751879896?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

<img src="/uploads/db1493/original/2X/8/8f1ac5e5ea29230ce7dccdc9b52cb43d3d23ae3e.jpg" width="690" height="388">

<img src="/uploads/db1493/original/2X/4/4788e815fff7da9ddf07537ad8f666633dcdff58.jpg" width="281" height="500">

<img src="/uploads/db1493/original/2X/b/b338a9b682c618b1aa1815be6e40d309862f823c.jpg" width="281" height="500">

<img src="/uploads/db1493/original/2X/7/72b53f34f0c0c39cb33fd6a566e676458b69f841.jpg" width="690" height="388">
```

---
## \#2 Posted by: lox897 Posted at: 2016-05-21T09:00:18.356Z Reads: 593

```
The pack only needs to be charged to 43.2v (3.6 x 12) not 43.8 (That is for 3.65 lifepo4 cells) Not sure if this is correct. Please advise me why if it isn't correct.
```

---
## \#4 Posted by: Kaly Posted at: 2016-05-21T12:14:35.326Z Reads: 597

```
The over discharge protection of this bms is too low for the A123 cells (2.1 ± 0.05 V) you will need to monitor this with the VESC low cut off voltage at start 2.6V and finish at 2.5V.

@lox897 you are correct on this

@L3thaltank can you please measure the dimension of the pcb itself and the aluminium heat sink.
```

---
## \#6 Posted by: willpark16 Posted at: 2016-05-21T12:28:46.012Z Reads: 574

```
get the bms from here 
http://www.a123rc.com/goods-1596-12S30A+PCMBMS+for+36V12S+Lifepo4+battery+pack.html
```

---
## \#7 Posted by: L3thaltank Posted at: 2016-05-21T16:29:08.127Z Reads: 561

```
source for this voltage cutoff range? I found it to be 2.0V

Check out this PDF:
http://www.formula-hybrid.org/wp-content/uploads/A123_AMP20_battery_Design_guide.pdf

pg.59 
Appendix A
Cell Specifications
ANR26650M1B
Recommended end of discharge cutoff 2.0V
```

---
## \#8 Posted by: L3thaltank Posted at: 2016-05-21T16:35:07.345Z Reads: 539

```
I have found that the Maximum allowable charge voltage is: 4.2V MAX

so i should be fine charging to 3.65V per cell vs 3.6V.

Source: http://www.radicalrc.com/category/A123-Cells-Packs-199
```

---
## \#9 Posted by: L3thaltank Posted at: 2016-05-21T16:50:00.314Z Reads: 524

```
**PCB:**
Length: 6.625 inches
Width: 2.875 inches
Thickness: 1/16 inches

**Heatsink:**
Length: 7.875 inches
Width:4 inches
Thickness: 1/16 inches
```

---
## \#10 Posted by: Kaly Posted at: 2016-05-21T17:15:05.188Z Reads: 499

```
This will greatly diminish the life of the pack. 
Tesla goes from 3.6V to 2.5V and it increases the life of the pack. 

This is the manufacturer pdf. http://a123batteries.com/v/vspfiles/images/pdf/26650.pdf

Well thank you for the dimensions and good luck with your pack. 👍🏻👍🏻
```

---
## \#11 Posted by: L3thaltank Posted at: 2016-05-21T17:25:02.816Z Reads: 500

```
Why do you think it will greatly diminish the life of the pack? Charging to 3.65V per cell? or discharging to 2.0V?

Can you show me some examples explaining their voltage cutoffs for these cells? 

Why would they state a recommended cutoff of 2.0V? 

What cutoff do you use with your dual 6s alarms?
```

---
## \#12 Posted by: Kaly Posted at: 2016-05-21T18:12:12.622Z Reads: 503

```
[quote="L3thaltank, post:11, topic:3591"]
Why do you think it will greatly diminish the life of the pack? Charging to 3.65V per cell? or discharging to 2.0V?
[/quote]

laboratory settings are not the same as real world use.  A great number of people are using this cells for other applications and all the charge/discharge logging point to the sweet spot of 3.6V - 2.5V range to increase the life of the pack. The over charge will not be as detrimental compare to the over discharge but will affect too. 

About the examples, all power tools using this batteries cut the discharge at/or around 2.5V. 

[quote="L3thaltank, post:11, topic:3591"]
Why would they state a recommended cutoff of 2.0V?
[/quote]

That's the laboratory setting cut off for marketing porpoises. It can be use but not recommend. If you look closely to the 2 top graphics on the pdf you'll notice on the left side voltage axis. that the initial voltage drops in a exponential way (really really fast) wich means that there's not that much usable capacity in that voltage range. 

The bulk of the usable capacity is in the nominal voltage range. Going now to the right side of the first graph after the 2.5V on the 140W - 180W usage range the discharge curve drops exponentially again wich translate once more in little usable capacity after this voltage range. 

The alarm in my pack, I just use as a volt meter just to check the voltage, this alarms just go as low as 2.7V so I don't use the alarm :-( , I have confirm that from 2.8 - 2.5 the pack still have 30% of the capacity. 

This is the main issue with the lifepo4 cells that there's no way to know the depth of discharge, because of the flat discharge curve and the exponential way in wich the capacity finishes. 

But if you are going to use a VESC to manage the cut off voltage just use 31.2 V for the start voltage cut off and 30V for the end voltage cut off. That way your bms will handle the charging and VESC the discharging.
```

---
## \#13 Posted by: L3thaltank Posted at: 2016-05-21T18:53:01.445Z Reads: 516

```
Thanks for your input! :smiley:
I'm using dual TorqueBoards 12S 120A Car ESC  so i might be able to set a correct voltage cutoff, but might not. I need to check the settings.

I eventually plan on investing in 2 VESC sometime down the road as I just spent a bunch of money on this pack and a Hi5ber Raptor that I ordered :grinning: http://www.hi5ber.com/#!raptor/ca1y
```

---
## \#14 Posted by: Kaly Posted at: 2016-05-21T19:14:27.754Z Reads: 512

```
That deck is sick :grinning:
```

---
## \#15 Posted by: willpark16 Posted at: 2016-05-25T02:19:52.918Z Reads: 510

```
so why did u end up soldering the cells vs sleds? And what type of wire is that?
```

---
## \#16 Posted by: L3thaltank Posted at: 2016-05-25T02:27:39.529Z Reads: 553

```
Here is some more snapshots of this battery build process :grinning:
<img src="/uploads/db1493/original/2X/7/791cede1a537d144105b273babae4f97775810a8.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/5/59bbb81756e1d0a5ab0066b40b488e1eb84fe79c.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/c/c21f19611ab99ffd601f58289bd9fa6d62c301af.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/9/906d2cc1ca556acb25df5c16c75a751b8da17039.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/b/b61caae45c23123b365bcbcd315a5a16942933d9.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/d/df21007002dfef68118bf94097b3c17ce5c0449f.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/d/dfb9d134210011ac0f11e11face2db68290a3b14.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/1/1b8a98dde9a38f0b2da2557253bbc5f4aca0e339.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/4/449f2627bda928b9e671adb4a7fe6c1940b9ed58.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/b/bf8c88c87ff36b16425a277d5130cd247e0f963b.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/b/bfff876e009a32c16079652d6a2dda32e47dfc5e.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/9/9378f6ff2da8a2297a1d6c2f6140bee278bb49df.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/0/06196ed7bf1dea0efd407d74764a71406a2fa555.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/b/b9022c3cfa53519b542e02a7958cb710e87d323c.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/c/c086f3f8c355933a39b9f7163c9bd4bc2f39447c.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/1/1dcf73a7e635ba7dae7c9eade4e3e2f482a304f2.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/a/a2bcae8c2847431245df024c6a89f29022eafcf8.jpg" width="281" height="500">
If anyone has questions about the tools I used or my process I would be happy to help. I still have to splice in my charger port etc.. I will post a full board build thread soon.
```

---
## \#17 Posted by: L3thaltank Posted at: 2016-05-25T02:38:24.298Z Reads: 477

```
I decided the sleds I purchased would be too much of a pain to make them work,especially since I would have to remove the tabs to solder them and then snap them back into place in the plastic holder. Also reading about nickel strip sizing given amperage I decided It would be more reliable to directly solder the cells. 

I used 10AWG silicone wire, some turnigy and some superworm.
```

---
## \#18 Posted by: willpark16 Posted at: 2016-05-25T02:40:06.715Z Reads: 469

```
alright thanks man!
```

---
## \#19 Posted by: shred Posted at: 2016-05-25T06:23:13.456Z Reads: 469

```
nice work man! like the awg10 wiering!
```

---
## \#20 Posted by: willpark16 Posted at: 2016-06-25T03:38:03.095Z Reads: 454

```
what watt iron did u use
```

---
## \#21 Posted by: L3thaltank Posted at: 2016-06-25T19:01:13.334Z Reads: 456

```
100 Watt iron with the included CT6F7 Tip
https://amzn.com/B002I7X7ZS

you can also buy smaller tips for this iron. I got some from Mouser http://www.mouser.com/Search/Refine.aspx?Keyword=W100PG
```

---
## \#22 Posted by: Pantologist Posted at: 2016-06-25T20:57:47.992Z Reads: 451

```
Dang this battery probably costed a hell of a lot.... But it will last super long. I think I will stick to regular Li-ion 18650 packs but this is pretty awesome. 

Boosted uses these same cells too I believe.
```

---
## \#23 Posted by: whitepony Posted at: 2016-06-26T07:08:41.388Z Reads: 439

```
sick battery :scream:

its nearly a shame to squeeze the current through that 100A BMS bottleneck! :frowning:  

[quote="L3thaltank, post:13, topic:3591"]
I'm using dual TorqueBoards 12S 120A Car ESC  so i might be able to set a correct voltage cutoff, but might not. I need to check the settings.
[/quote]

you need to be extremely careful with that voltage cutoff on the torqueboard escs - its not reliable and nearly cost me a battery. read here for my explanation: https://endless-sphere.com/forums/viewtopic.php?f=35&t=72026&p=1117738#p1117738
```

---
## \#24 Posted by: L3thaltank Posted at: 2016-06-26T15:52:02.768Z Reads: 419

```
Yea... it wasn't cheap 36 cells at $9.30 each plus $20 for shipping. I originally was going 2p with 24 cells but bumped up to 3p so I ended up paying $40 shipping for 2 orders and $335 for cells. 

Yes boosted version one uses 12 of these cells. I'm not sure what version 2 uses... people have said lipo but I'm not sure. 

I mainly went with these cells for their cycle life. After calculating costs of building it myself, it made a lot more sense than investing in a space cell.
```

---
## \#25 Posted by: Pantologist Posted at: 2016-06-26T17:45:50.760Z Reads: 411

```
Holy crap that is a lot.... but these are definitely the best cells to use for an electric skateboard. 

I'm almost sure v2 is using an 18650 10S2P pack of some 2500mAh batteries. That would fit their 199Wh rating. Also Boosted despises Lipos since they were a failure on their first few concepts.

Nice. Personally, I was thinking of a a123 12s1p or 12s2p Samsung 25R pack. Can't decide. Both fit on my board, just one has longer life span and one has a greater capacity. I'm just using this board for fun and small trips so it doesn't really matter to me.
```

---
## \#26 Posted by: willpark16 Posted at: 2016-06-27T04:14:37.741Z Reads: 386

```
can u pm me ur gmail
```

---
## \#27 Posted by: vitormhenrique Posted at: 2016-07-01T19:35:55.218Z Reads: 382

```
[quote="L3thaltank, post:16, topic:3591"]
If anyone has questions about the tools I used or my process I would be happy to help.
[/quote]

Did you cover the battery with foam? and then used a heatshrink to wrap everything?
```

---
## \#28 Posted by: L3thaltank Posted at: 2016-07-01T20:08:44.231Z Reads: 374

```
Yea I covered it with adhesive backed 3m black neoprene like foam, then heatshrinked around the bms and finally headshrinked the entire battery.
```

---
## \#29 Posted by: vitormhenrique Posted at: 2016-07-01T20:22:41.683Z Reads: 367

```
Awesome! where the hell did you find a heatshrink that big?
```

---
## \#30 Posted by: Jinra Posted at: 2016-07-01T20:27:24.793Z Reads: 369

```
why the foam if i may ask? It seems like it would insulate heat.
```

---
## \#31 Posted by: L3thaltank Posted at: 2016-07-01T22:26:40.479Z Reads: 363

```
http://www.batteryspace.com/9.45-240mm-Width-Rubber-like-Heavy-Duty-Heat-Shrink-Wrap-Tube.aspx

They have bigger and smaller sizes also... I asked that it be left in one continuous piece when I ordered.
```

---
## \#32 Posted by: Kaly Posted at: 2016-07-02T11:46:46.481Z Reads: 357

```
I have use this product and That shrink wrap will need a lot of heat and the rubber will keep that heat and transfer it to the battery pack. 
For you not to heat the battery too much, it will be good to place the pack on a damp wet towel, use you heat gun on the shrink wrap and  turn the heated side of the pack on to the towel. That way the heat will be absorb by the water in the towel and not you new battery pack.
```

---
## \#33 Posted by: gaetjen Posted at: 2016-08-15T21:02:35.188Z Reads: 326

```
What's the difference between using 10awg wire and nickel strips? Almost all of the diy battery packs are build with nickel strips. 
Also, is there a difference if you connect each individual cells of one parallel pack with each cell of the next pack or like you did, just connect the last cell with the first cell of the pack?
```

---
## \#34 Posted by: sl33py Posted at: 2016-08-15T21:44:48.267Z Reads: 319

```
great build and should be an awesome long-life pack!

what was the overall length once wrapped?  Simple math says it's no less than 468mm/18.6in, but with the cell spacers maybe a bit more?

How is it running - any issues?
```

---
## \#35 Posted by: willpark16 Posted at: 2016-08-15T22:19:04.489Z Reads: 321

```
10 awg is if u dont wanna use nickel strip
```

---
## \#36 Posted by: shred Posted at: 2016-08-16T06:23:56.064Z Reads: 321

```
The ampere rating between nickel strips (approx. 15A, depending on the nickel strip size) and awg10 wire (more than 55A continuous for silicon wires) is quite different, at least for the serial connections you might need something more than nickel strips.
```

---
## \#37 Posted by: Pantologist Posted at: 2016-08-16T16:03:56.957Z Reads: 307

```
Some tinned copper braid works well.
```

---
## \#38 Posted by: Eboostin Posted at: 2016-08-16T16:31:00.952Z Reads: 309

```
How would the 12s3p A123 range compare to a 10s3p made up of 2500mAh cells?
```

---
## \#39 Posted by: Pantologist Posted at: 2016-08-16T16:35:59.626Z Reads: 312

```
Yeah... It will also last a lot longer.
```

---
## \#40 Posted by: Jinra Posted at: 2016-08-16T16:36:59.359Z Reads: 315

```
about the same 288wh vs 270wh, 12s3p has an extra 6 cells and the cells are bulkier.
```

---
## \#41 Posted by: rubz Posted at: 2016-08-16T16:37:44.222Z Reads: 325

```
If you're talking about 18650 Li-Ion cells, then 10*3*3,6V*2,5Ah = 270Wh (compared to 3*12*3,3V*2,5Ah = 297Wh for 12S3P A123, so the range difference shouldn't be too big; a 10% difference). However keep in mind that A123's will last a longer (in terms of cycles) and can output more amps (and will probably have less voltage sag in this configuration) but it is a lot bulkier.
```

---
## \#42 Posted by: joeykache Posted at: 2016-08-16T19:34:33.860Z Reads: 323

```
Can you show us what the end result was for the battery pack? Want to see how it looks with all of the connectors and charging port.
```

---
## \#43 Posted by: L3thaltank Posted at: 2016-08-16T22:06:41.949Z Reads: 315

```
I haven't had the time to work on it more...but when I finish it will be posted here for sure!
```

---
## \#44 Posted by: Bataleon Posted at: 2016-11-07T17:51:31.161Z Reads: 269

```
Any updates, @L3thaltank? It'd be very interesting to see your progress.
```

---
## \#45 Posted by: L3thaltank Posted at: 2016-11-07T23:30:00.652Z Reads: 265

```
<img src="/uploads/db1493/original/3X/9/2/92a5ae6e145be037503b3bb7b45d9bbd81545891.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/c/6/c65f9b241243d1d70d055d8ed6816000376172fb.jpg" width="690" height="388">

Battery Pack 
Dimensions: 21" Long x 6.75" Wide x 2.25" Tall (highest point)
Weight: Approximately 13.6 lb
```

---
## \#46 Posted by: johnny_261 Posted at: 2016-11-08T08:08:12.817Z Reads: 255

```
Have you tried it out yet? I'm thinking of doing a 12s2p with the same cells.
```

---
## \#47 Posted by: L3thaltank Posted at: 2016-11-09T01:30:41.404Z Reads: 250

```
I haven't tried it out yet... As soon as I finish dialing in my setup and making my enclosure I'll make a build thread with updates. I have been super busy lately.
```

---
## \#48 Posted by: Pantologist Posted at: 2016-11-09T01:32:52.155Z Reads: 249

```
Do it. They are awesome cells. A 1P pack is good enough but 2P would be great. Slight expensive though. The benefits are worth it though.
```

---
## \#49 Posted by: johnny_261 Posted at: 2016-11-09T04:04:48.191Z Reads: 243

```
Yeah, I think I'll do it. Gotta source some batteries now!
```

---
## \#50 Posted by: Highcooley Posted at: 2017-05-29T21:42:22.522Z Reads: 204

```
Any news on this pack? I'm going to build one too, as soon as I get the cells and am wondering about what BMS to use. Does anybody have a recommendation for a a123 12s3p pack with the correct charging protection voltage and amperage? For discharging, I am planning to use the VESC, in order not to worry about expensive BMS or a power bottleneck. Although, I guess a 120A would do for a two motor setup which are rated to 50A max peak each. I hope the VESCs have a good reputation concerning undercharging protection.
```

---
## \#51 Posted by: BigBoyToys Posted at: 2017-05-30T07:26:01.085Z Reads: 196

```
Im just using a 15A bms for charging and bypassing it for discharge.

Look at this on eBay http://www.ebay.com/itm/222302389040
```

---
## \#52 Posted by: onlytesla Posted at: 2017-06-09T11:51:23.414Z Reads: 182

```
It is forbidden to soldering the battery poles. Poor tech!
```

---
## \#53 Posted by: BigBoyToys Posted at: 2017-06-11T18:57:56.234Z Reads: 171

```
Lots of people solder battery cells frokm what I read. Copper strips just wont hold enough current to work in this application.
```

---
## \#54 Posted by: onlytesla Posted at: 2017-06-11T19:16:32.176Z Reads: 174

```
That's why exist is welding with nickel band, because can care more amps !
```

---
## \#55 Posted by: onlytesla Posted at: 2017-06-11T19:17:35.671Z Reads: 178

```
Take a look here : www.elektrofietsaccu.nl
```

---
## \#56 Posted by: i2oadsweepei2 Posted at: 2017-09-14T12:43:50.921Z Reads: 148

```
[quote="Kaly, post:12, topic:3591"]
The alarm in my pack, I just use as a volt meter just to check the voltage, this alarms just go as low as 2.7V so I don't use the alarm :frowning: , I have confirm that from 2.8 - 2.5 the pack still have 30% of the capacity.
[/quote]


This is most excellent, I haven't ran my pack down to vesc cutoff yet. I have it set to 2.8 and 2.7. So there is even more in it. I'm using a self built 8s3p A123 pack. So far according to the metr app the last run I did was 14+kms and I'm still sitting at 3.2v per cell.i honestly thought something was wrong. When I have time I'm going to try and drain the pack. 

So 8s3p A123 is 198 wh as far as I know. I have the same BMS shown above, but its the 80 amp version. It say it balances for 3.5v per cell which is 28v. How much capacity am I losing by not getting to 3.6v? My gut tells me that i'm at or very near 95%.

These cells don't act like other cells like said above. Am I just running efficiently or am I missing something? I was calculating 198wh divided by 10 to get 19kms distance. It seems I could exceed that fairly well. The regen on this ride gave me 2km more worth of distance.
Something happened with the map part, but the distance and everything else seem right. Its a dual 230kv 16/40 97mm setup.
https://metr.at/r/r4Kjj
```

---
## \#57 Posted by: i2oadsweepei2 Posted at: 2017-09-17T20:47:07.760Z Reads: 130

```
[quote="i2oadsweepei2, post:56, topic:3591"]
These cells don't act like other cells like said above. Am I just running efficiently or am I missing something? I was calculating 198wh divided by 10 to get 19kms distance. It seems I could exceed that fairly well. The regen on this ride gave me 2km more worth of distance.
[/quote]

I can confirm running my pack right to 2.75 cutoff start and 2.6 cutoff end. I had to walk up a few hills but did small stretches on the flat. Ended pushing the rest of the way 1/2 km. I travelled 21.5km. Very happy about that.
```

---
## \#58 Posted by: Travo Posted at: 2018-08-03T05:39:45.963Z Reads: 67

```
Hey everyone, just wondering if I could use this BMS with the 26650 cells, thanks!

10S 60A active bms 2017 new Li-ion smart bms pcm with android Bluetooth app UART correspondence bms wi software (APP) monitor
 http://s.aliexpress.com/fmQRjeYJ
```

---
## \#59 Posted by: deucesdown Posted at: 2018-08-03T05:55:33.807Z Reads: 71

```
Yeah it works great. Everything is configurable. I use it for charge only. The only thing is the bluetooth module unfortunately has a bit of drain, would be smart to put a switch on its power line.

These units can be reconfigured for up to 16s by bridging or unbridging some solder pads and changing some settings.

Oh you should get the one for lifepo4. The units are the same but the settings will be good to go out of the box.
```

---
## \#60 Posted by: Travo Posted at: 2018-08-03T23:12:18.976Z Reads: 58

```
Awesome thanks for the help! Would I be able to charge with a 42v 2a power like in my 18650 pack?
```

---
## \#61 Posted by: deucesdown Posted at: 2018-08-04T01:17:44.494Z Reads: 51

```
Yeah it's excellent for charging slightly less than full as you can configure when and how it balances, and watch what it's doing.
```

---
