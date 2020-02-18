# Li-Ion battery pack without bms!?

### Replies: 48 Views: 4846

## \#1 Posted by: Alex.Scheff Posted at: 2018-03-01T06:56:32.797Z Reads: 317

```
Hello, I found this Video on youtube and I think its pretty good, what do you think about it?
https://youtu.be/pljSZcEwc8Q
Alex
```

---
## \#2 Posted by: ZackoryCramer Posted at: 2018-03-01T07:00:55.742Z Reads: 308

```
If you don't use a BMS and don't balance your cells, chances are something is going to go wrong after 10+ cycles. :popcorn:

EDIT: This is completely incorrect.
```

---
## \#3 Posted by: michaelcpg Posted at: 2018-03-01T07:05:49.524Z Reads: 304

```
Good quality cells actually seem to stay in balance pretty well from the few instances I've seen. 

I've also personally never charged my board above 90% (so the BMS balancing function has probably never kicked in) and I would've done somewhere between 500 - 1000km on it so far. The cells were all still within 0.01V of each other last time I checked. 
I also never let my battery go below 25% either though so keeping the battery mostly in the 30% - 80% range the majority of the time probably helps with this, and it certainly increases your cycle life as well.

In saying all that, its still better to have a BMS, particularly if you're not the kind of person who's willing to check their cell voltages every so often
```

---
## \#4 Posted by: MysticalDork Posted at: 2018-03-01T07:08:43.234Z Reads: 293

```
It can be done, and he makes some good points. BUUUUUT, many of those points depend on the user being attentive and careful all the time. I dunno about you, but I have my bad days, and I can't be arsed to care about my battery sometimes. With a BMS, that doesn't matter, since it keeps track of it for you.

Yes, a BMS can become defective. You should always check your stuff once in a while, even if nothing is wrong. It's called preventative maintenance.

Yes, most BMSs only balance at a few tens or hundreds of milliamps. BUT, our batteries are quite a bit smaller than most ebike packs, or powerwall setups, so the actual fraction is larger.



TL;DR yes, you can build a BMSless pack, but it's a more involved process and requires more commitment from the user. A BMS is a labor saving device. What are esk8ers but people who love labor saving devices?
```

---
## \#5 Posted by: rok Posted at: 2018-03-01T07:26:04.541Z Reads: 270

```
You need to double check your answers/advices before you post them :point_up_2:
```

---
## \#6 Posted by: mmaner Posted at: 2018-03-01T14:58:01.551Z Reads: 247

```
[quote="ZackoryCramer, post:2, topic:47818, full:true"]
If you don’t use a BMS and don’t balance your cells, chances are something is going to go wrong after 10+ cycles.
[/quote]

Dude, you gotta stop.

Its a proven fact that you can discharge a pack to 3.4v, charge to 4.1 and it will self-balance.  The problem exist when you discharge too much or fully charge.  I have a 10s3p 30q pack I've been running for months this way, it hasn't been balanced since it was first built and the cells are always within .1v of each other.
```

---
## \#7 Posted by: ZackoryCramer Posted at: 2018-03-01T16:24:40.503Z Reads: 225

```
I mean I guess if you keep a strict cycle. I was just trying to lean him towards getting one. Chances are, he doesn't have a power supply to charge his pack. The lipo that I haven't balanced for 20 cycles already has a max delta of more than 0.1v, that I use a power supply though. :no_mouth: 
@rok You're right brotha :full_moon_with_face:
```

---
## \#8 Posted by: mmaner Posted at: 2018-03-01T16:30:14.209Z Reads: 217

```
Steering someone one direction is fine, but if you do it without telling them its manipulation and that ain't cool.  Just give the info and let them decide...or better yet, let them ask for opinions.

This is a subject that has been given lots of screen time and many people have argued over it for months.  I went so far as to have a 30q pack made so I could prove it one way or another.  It turns out that if you dont fully charge or discharge the cells will self-balance sans BMS.
```

---
## \#9 Posted by: thisguyhere Posted at: 2018-03-01T18:03:58.593Z Reads: 208

```
also, going back to the original video, instead of a bms he's using a balance charger.  so...it's still being balanced.

it's that specific video that led me to use a balance charger on my first build using that exact same charger (1010b+).

i don't know about you, but plugging in a charge cable and balance leads to my board every time to charge got to be a PIA.

[quote="mmaner, post:6, topic:47818"]
you can discharge a pack to 3.4v, charge to 4.1 and it will self-balance
[/quote]

wait, not sure if that's true.  a parallel pack will self balance, so the cells within a P pack will balance out.  but voltage drift across S packs will not self-balance, right?
```

---
## \#10 Posted by: mmaner Posted at: 2018-03-01T18:10:06.573Z Reads: 192

```
That's what I've heard, but in practice, on my pack specifically built for this test, I have had no drift over .1v across P groups.  I have literally never balanced this pack, for the sole purpose of finding out what happens when not balancing and only charging to 90%, discharging 90% of its capacity.  I have well over 1000 miles on this pack, no issues to date.
```

---
## \#11 Posted by: thisguyhere Posted at: 2018-03-01T18:22:33.360Z Reads: 184

```
right, new high quality cells from the same production batch should have nearly identical properties, ie internal resistance, and would / should charge and discharge at nearly identical rates.

now...my 12s3p pack of 25r cells, despite being brand new when it was built, does drift a bit when fully discharged down to 3v per cell, so a balance is needed when charging.

moral of the story is, you may NOT need to balance, but balance to be safe and ensure longevity.
```

---
## \#12 Posted by: scrapheap Posted at: 2018-03-01T18:24:52.545Z Reads: 179

```
@whitepony runs all his builds with no BMS last I checked... and he hasn't had any problems yet...though I think he occasionally will check to see their voltages as a precaution.

A BMS is an simple, one-plug-to-charge solution. There are alternatives, like using hobby chargers, modified VGA ports, ebike ports, etc. Lots of stuff to try, if one is willing to experiment.
```

---
## \#13 Posted by: mmaner Posted at: 2018-03-01T18:25:03.186Z Reads: 170

```
Absolutely, balancing in NEVER bad.  I just wanted to know for sure if you could run a battery pack for a long time without balancing if you did not completely charge and discharge.  I'm satisfied that you can.  I actually have a BMS for this pack, just haven't had a need to put it on it yet :).
```

---
## \#14 Posted by: Alex.Scheff Posted at: 2018-03-01T18:32:18.480Z Reads: 162

```
What If I install a bms on my battery pack but just for charging. For discharge I simply plug in the plus and minus of the battery.
Does this work?
```

---
## \#15 Posted by: mccloed Posted at: 2018-03-01T18:32:35.308Z Reads: 161

```
I have several 10s 4p boards that do not have BMS's. They each have about 300 miles on them. I got tired of the BMS's killing cells. With that said, it is always a good idea to have a QUALITY BMS in the mix. 

Damn! I should probably check the cells. I haven't in a couple months. :smile:
```

---
## \#16 Posted by: Alex.Scheff Posted at: 2018-03-01T18:34:45.229Z Reads: 154

```
@mccloed And how do you charge and discharge safelly?
```

---
## \#17 Posted by: mccloed Posted at: 2018-03-01T18:37:19.500Z Reads: 151

```
Laptop style charger and voltage cutoff settings in the VESC's. Might not be the safest, but that's what I do.
```

---
## \#18 Posted by: Alex.Scheff Posted at: 2018-03-01T18:38:26.853Z Reads: 146

```
What vesc do you use?
```

---
## \#19 Posted by: mccloed Posted at: 2018-03-01T18:47:40.859Z Reads: 146

```
Both Focboxes and Torqueboards VESC's.
```

---
## \#20 Posted by: Alex.Scheff Posted at: 2018-03-01T19:04:40.358Z Reads: 143

```
How did you made the vesc to cut off at a specific voltage?
```

---
## \#21 Posted by: treenutter Posted at: 2018-03-01T19:21:37.505Z Reads: 135

```
[quote="ZackoryCramer, post:2, topic:47818, full:true"]
If you don’t use a BMS and don’t balance your cells, chances are something is going to go wrong after 10+ cycles.
[/quote]


This is completely incorrect. @ZackoryCramer pls refrain from providing input if you're not sure you're right. When it comes to batteries, incorrect information  = :fire:
```

---
## \#22 Posted by: ZackoryCramer Posted at: 2018-03-01T19:23:24.651Z Reads: 133

```
You got me brotha 🙏🏻 Thanks.
```

---
## \#23 Posted by: mccloed Posted at: 2018-03-01T19:43:16.590Z Reads: 131

```
You may want to read through this: http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980

You can set the Start and End voltage.

![image|690x401](upload://tHJed6Jnbw9pU7cXYlYNCZJUBoW.png)
```

---
## \#24 Posted by: Pedrodemio Posted at: 2018-03-01T19:53:05.661Z Reads: 125

```
Wrong, lithium doesn’t self balance, that is on the serial connections, on the parallel it obviously get even voltage in the same group

The main example of self balance it’s lead acid, that when the cells reaches a given voltage it’s stays there and starts to warm to dissipate th excess energy

With lithium if you keep increasing the voltage the cell will keep increasing and then something bad will happen, that’s why it’s recomended to use a BMS at least for charging

If you use quality cells the internal resistance is almost the same in each one, this way the energy loss as heat on each cell is almost equal so no significantly imbalance will occur 

Of course in thousands of cycles this diferences add up and the difference can grow to an unacceptable level

Edit:

To make and exception if I’m not mistaken sony had an self balancing chemistry
```

---
## \#25 Posted by: ZackoryCramer Posted at: 2018-03-01T19:58:25.971Z Reads: 116

```
Hey I concur with you brotha. 😃 But @mmaner seems to be getting away with it though. Maybe there are discrepancies we should sort out. 🧐
```

---
## \#26 Posted by: Pedrodemio Posted at: 2018-03-01T20:02:46.205Z Reads: 111

```
Sure, with quality cells it will take a long time, take @whitepony as example

With greater number of P cells it gets even better, since you average out the differences of each cells by joining them in parallel
```

---
## \#27 Posted by: mmaner Posted at: 2018-03-01T20:03:24.774Z Reads: 110

```
Im not arguing that fact, it should only balance within the same group.  If its because the chemistry and resistance is almost identical, or because the little battery beasties like me more than anyone else...couldn't say.  I just know that after almost a year its still balanced.
```

---
## \#28 Posted by: mccloed Posted at: 2018-03-01T20:05:32.229Z Reads: 110

```
The beasties must like me too!
```

---
## \#29 Posted by: ZackoryCramer Posted at: 2018-03-01T20:07:10.766Z Reads: 110

```
How do you know the cells are balancing themselves? It could be just that the cells have very litttle difference brotha. 😘
```

---
## \#30 Posted by: mmaner Posted at: 2018-03-01T20:26:05.829Z Reads: 106

```
On multiple occasions I have measured each cells beginning voltage before charge and re-measured after charge.  It shows that there is up to a 0.6v per cell deviation.  After charge there will be, typically, a 0.25v deviation per cell.  After sitting overnight the deviations is typically .1v at most.
```

---
## \#31 Posted by: ZackoryCramer Posted at: 2018-03-01T20:39:12.862Z Reads: 106

```
Strange. The cells seem to have memory of each other. 👻 you should record every charge over night voltage difference, because we want to see how the cells progress over time brotha. 🎃
```

---
## \#32 Posted by: mmaner Posted at: 2018-03-01T21:15:39.672Z Reads: 108

```
I did for about 3 months, got tiring.  I do it about once a month now.  I will eventually stop recording all together if it stays at the limits I described.  

I'm thinking about using a VGA header to make a balance plug and then cooking an enclosure up for a BMS, so I can balance charge multiple packs with a single BMS.
```

---
## \#33 Posted by: Alex.Scheff Posted at: 2018-03-01T22:29:01.244Z Reads: 103

```
So If I just use the bms for charging and not for discharging I don't have to spend 100+€ for a 100A discharge bms. I will say my vesc's they have to shut down If my batter voltage goes down to 30V (or another Voltage). Theorethically I don't damage my battery with over discharge. Is this right or I'm just retarted? :sweat_smile:
Alex
```

---
## \#34 Posted by: mmaner Posted at: 2018-03-01T22:30:34.238Z Reads: 103

```
No, you absolutely can damage a battery with over discharge.  You can use the VESC to set the voltage cutoff values, so using a BMS for discharge only is acceptable.  Its not the safest, but many people do it because they keep on eye on the pack voltage.
```

---
## \#35 Posted by: Alex.Scheff Posted at: 2018-03-01T22:34:33.757Z Reads: 101

```
So I have to spend a lot of money for a 120A discharge bms? :slightly_frowning_face:
```

---
## \#36 Posted by: mmaner Posted at: 2018-03-01T22:36:23.275Z Reads: 98

```
No dude, if you don't let your pack voltage get below 2.9 per cell you are fine.  So set your cutoffs accordingly in the VESC and it will cutoff voltage when it reaches that limit.  You can use a charge only BMS so that the cells are balanced and charged correctly, and discharge directly to the VESC/VESCs.
```

---
## \#37 Posted by: Alex.Scheff Posted at: 2018-03-01T22:37:53.119Z Reads: 99

```
Oh okay now I understand, sorry :sweat_smile:
Thank you very much for your time
```

---
## \#38 Posted by: mmaner Posted at: 2018-03-01T22:40:04.247Z Reads: 102

```
No worries, let me know if you need anything else.
```

---
## \#39 Posted by: Pedrodemio Posted at: 2018-03-01T23:03:10.416Z Reads: 107

```
How are the cells hooked up during charging? Are you measuring directly on the cells or some place along the charge wire? 

But the cells do have some recovery, after a heavy current the can take a while to get to resting voltage, that’s the problem with determining state of charge using voltage only, you never know if the cells is at rest or still recovering
```

---
## \#40 Posted by: SkaterBoy58 Posted at: 2018-03-01T23:08:22.972Z Reads: 112

```
@mmaner  You mean something like I made ! with a smart configurable BMS

 ![BMS No 1|690x393](upload://3XILKcKzgwciE3bP07z35xZxIK2.jpg)![BMS - Internals|666x500](upload://2yl8Za34sLD0HOYc4XyMsJNm2Xk.jpg)![bms 7|666x500](upload://xbRjeU5b3raKzUKp2biGZr8nYaS.jpg)![BMS Photo 1|666x500](upload://8wlsrarN9D9yEm0oJ18oIcXbdaj.jpg)![bms photo 6|666x500](upload://f7TDi4wEzPEWjImSFa6hlzipWjE.jpg)![BMS No 2|690x392](upload://ypTjr4S4iFt73QuwAENsFgv3NGF.jpg)
```

---
## \#41 Posted by: mmaner Posted at: 2018-03-01T23:14:46.590Z Reads: 105

```
[quote="Pedrodemio, post:39, topic:47818"]
How are the cells hooked up during charging? Are you measuring directly on the cells or some place along the charge wire?
[/quote]

The charge port is connected directly to the pack POS & NEG.  Im measuring the balance leads individually.
```

---
## \#42 Posted by: mmaner Posted at: 2018-03-01T23:15:40.113Z Reads: 102

```
[quote="SkaterBoy58, post:40, topic:47818"]
You mean something like I made ! with a smart configurable BMS
[/quote]

Well that's just cool as hell :).  Have you done a write up on it?
```

---
## \#43 Posted by: Pedrodemio Posted at: 2018-03-01T23:36:12.528Z Reads: 96

```
Nice, there no is load them, I guess it’s the cells recovering after current in or out
```

---
## \#44 Posted by: ZackoryCramer Posted at: 2018-03-01T23:39:27.303Z Reads: 100

```
Really neat brotha. :lying_face: Mind spilling how you did the software? :yum:
```

---
## \#45 Posted by: SkaterBoy58 Posted at: 2018-03-01T23:46:04.250Z Reads: 104

```
@mmaner    Nah -On my board I have a normal charge socket that connects directly to  battery +ve and -ve .

No BMS in board enclosure at all ( one less thing to break down and I don't need BMS to fail braking down-hill)

My battery has all 11 balance leads bought out to a weatherproof socket ( using  0.75 sq. mm high temp silicon wire) for the external BMS. I put 5A wire fuses in these leads to protect battery ( and prevent a fire) should there be a fault.

So I can charge without BMS directly into normal charge socket  on the board ( which I do 99% of the time) 

 or  I can plug in BMS box to monitor only cell voltages during charging through board charging socket
 
 or I can balance charge through BMS box using the 11 balance wires  ( which I haven't done for a month or so.  

Ultimate flexibility !
```

---
## \#46 Posted by: SkaterBoy58 Posted at: 2018-03-01T23:49:53.981Z Reads: 101

```
BMS from AliExpress - with PC uart connection

Even comes with a Bluetooth module for android phone cell voltage monitoring and configuration capacity


 https://www.aliexpress.com/item/13S-60A-active-bms-2017-new-Li-ion-smart-bms-pcm-with-android-Bluetooth-app-UART/32821764284.html?spm=2114.search0104.3.89.30717e9as0sSvw&ws_ab_test=searchweb0_0,searchweb201602_2_10152_10065_10151_10344_10068_10130_10342_10547_10343_10340_10548_10341_10084_10083_10618_10307_10131_10132_10133_5711211_10313_10059_10534_100031_10103_10627_10626_10624_10623_10622_10621_5722412_10620_5711312,searchweb201603_25,ppcSwitch_5&algo_expid=d1e41397-3fd7-45fc-8cad-7dd843697eb0-13&algo_pvid=d1e41397-3fd7-45fc-8cad-7dd843697eb0&transAbTest=ae803_3&priceBeautifyAB=0
```

---
## \#47 Posted by: darkkevind Posted at: 2018-03-02T00:07:30.021Z Reads: 96

```
Personally I would include a BMS in all my packs that I build, that way they can easily be charged just with a charging brick, however, I generally only use a low rated amp output current BMS, and bypass it for discharge, only using it to charge and balance the cells...

I find this very effective if your ESC handles cutoff voltages such as a VESC derivative.
```

---
## \#48 Posted by: Okami Posted at: 2018-03-03T18:44:03.473Z Reads: 86

```
Thats quite cool bms and "charge monitoring" box u have made. U should definetely make a sepereate post or tell more info about it.

 Looks like u can also configure a few settings or the bluetooth is just for monitoring?

On a side note - to the guy who said his lipos drift in voltage - that is quite true, thats also why li ion tends to be more popular choice, i think, if really high current is not needed, li ion cylindrical cells drift a lot less or almost not at all, if they are from same batch and balanced properly in first place
```

---
