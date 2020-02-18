# Not Charging. Let me know what I&rsquo;m doing wrong

### Replies: 25 Views: 264

## \#1 Posted by: evangreen Posted at: 2019-06-07T13:13:59.159Z Reads: 88

```
So I've just gotten my Wate 46.2V charger after waiting months from China to find that my battery is not charging. 

When I plug it in the light goes to red for just a moment and I can hear the fan start, then it goes to green immediately. My battery pack is at 34V and isn't increasing. Im using a bestech 140 BMS with the following diagram:

As I test with a multimeter with negative on B- and then checking each b2, b2, b3... it builds in 3.1v steps up to 34 on the last one. 

When I put the negative on B- and the positive on P- I get the remaining 12v that is coming out of the wall.  Any ideas here or have I wired this incorrectly?

The hot wire from my charger is going to battery + and the ground going to P-.

(Please note that my balance wires arent as shown in the diagram, was just to show the other BMS wires) 

![WIRING|690x359](upload://oztDqZ7Gj1DsGHMuVcAAdcsrStQ.jpeg)
```

---
## \#2 Posted by: LiquidSkater Posted at: 2019-06-07T13:30:14.790Z Reads: 79

```
I have a similar problem with my battery pack… I went for a long ride and drained my battery to 30.6V. Now, when I plug in the charger nothing happens. When i opened the board the battery pack was a a bit warm in ONE place (the middle on the right row) now its not charging… what should I do? I checked the charging port connectors and everything goes smoothly into BMS but nothing is charging, the charger light doesn’t change to red when plugged in

![1557337143640279613301608802735.jpg](https://www.electric-skateboard.builders/uploads/db1493/original/3X/3/9/390616fb07d3ce97734e461b5a801e8f644749a4.jpeg)

 

![15573371806923218806124129208418.jpg](https://www.electric-skateboard.builders/uploads/db1493/original/3X/2/3/23100b6f44fc55928e927e08e8256d6c221b55a3.jpeg)
```

---
## \#3 Posted by: wafflejock Posted at: 2019-06-07T13:39:34.237Z Reads: 69

```
Is your battery 9S or less? If not 30.6V is too low.  Most chargers will identify a cell below 3.0V as dangerous to charge and will not charge the pack (not sure about this BMS in particular but hobby balance chargers basically all have this safety feature built in)
```

---
## \#4 Posted by: evangreen Posted at: 2019-06-07T13:49:12.448Z Reads: 66

```
My battery is a 11s. I havet really used the batteries at all since purchased from NKON. Just did the calibration etc. They have been sitting all connected for a few months waiting for the charger which I guess could have drained them. 

So how do I get them charged if at 3.1 now?
```

---
## \#5 Posted by: evangreen Posted at: 2019-06-07T13:49:55.729Z Reads: 65

```
Also, mine is at 34, not 30.6v
```

---
## \#6 Posted by: wafflejock Posted at: 2019-06-07T13:54:47.614Z Reads: 64

```
Yah sorry was replying to other post here, generally cells don't drain much just sitting on the shelf, but so long as your cells as hooked to the BMS (if measured using the balance plug) shows below 3.0V then it *could* be an issue but would wait for someone with experience with this BMS to chime in too I'm a big proponent of using balance chargers separate from the board.  In some cases if a balance charger rejects charging a battery because of low voltage you can charge the individual cell that is low but need to determine if that's even a problem in your case and if this BMS has that as a safety feature how you may work around it (maybe jumper pins for lipo vs liion but speculating completely).
```

---
## \#7 Posted by: LiquidSkater Posted at: 2019-06-07T14:06:33.591Z Reads: 59

```
Its 42V it is 10S4P samsung 30q battery pack
```

---
## \#8 Posted by: LiquidSkater Posted at: 2019-06-07T14:07:22.171Z Reads: 60

```
The battery can't  be below 2.5 volts, if its above its all good...
```

---
## \#9 Posted by: LiquidSkater Posted at: 2019-06-07T14:08:49.120Z Reads: 60

```
The charger is working, but the LED on the charger is not charging to RED... how can I check if the BMS isn't  dead?
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-06-07T14:41:10.719Z Reads: 57

```
Some BMS won't charge it the cells are below 3v each.
```

---
## \#11 Posted by: evangreen Posted at: 2019-06-07T15:27:00.411Z Reads: 54

```
How do I get the cells up to that point to charge it then?
```

---
## \#12 Posted by: evangreen Posted at: 2019-06-07T17:07:22.843Z Reads: 49

```
Is it possible to bypass the BMS for a period of time until the cells are charged enough to use it? Maybe with a mini jumper cable?
```

---
## \#13 Posted by: thisguyhere Posted at: 2019-06-07T17:08:46.731Z Reads: 48

```
check individual cell voltage, i bet it's out of balance

https://medium.com/@esk8life.orders/checking-and-correcting-voltage-drift-in-a-battery-pack-616e139d2e3b
```

---
## \#14 Posted by: LiquidSkater Posted at: 2019-07-01T09:52:49.784Z Reads: 27

```
YEP, my battery pack is out of balance, every series is at 3.2 V, but one is at 0.5 V what can I do?
|First|3.2|
|---|---|
|Second|6.5|
|Third|7|
|Fourth|10.2|
|Fifth|13.5|
|Sixth|16.8|
|Seventh|20|
|Eight|23.2|
|Ninth |26.4|
|Tenth|29.7|
Soo the third series is dead or can I fix this somehow?
```

---
## \#15 Posted by: Darkie02 Posted at: 2019-07-01T10:30:52.354Z Reads: 23

```
You need to split the p group and test each cell individually. I see it’s 23 days later so if you had one bad cell it could have killed the other 3 in the p group easily by now. any cell below 2.5v I personally would dispose of. You can replace the bad cells but you need to be aware of mixing new and old cells and the danger this can add.

Other options are slowly charge and discharge the over discharged cells. Some can be revived but this has to be done extremely small currents and in a safe place watching the temp and monitoring capacity. The more the cell was over discharged the more damage has been done internally and the more likely it will end up on fire. IMO for the cost of a cell vs danger I would just dispose of the bad cells below 2.5v (most manufactures min voltage)

Depending on the age of the pack a new cell will have a higher capacity and holed a higher voltage for longer so as it discharges in a pack it will put the pack overall voltage slightly higher you need to compensate for this to not over discharge your other cells. 

The question you should be asking is how did you discharge 1 P Group so badly. Is this a Issie with your charger cutting out and not allowing the BMS to balance the pack. Was it a bad cell that’s died over time and lack of maintenance of the pack got it in a dangerous state. did you have bad welds and some of the cells in the p group have never been connected. Has part of the pack connections overheated and melted. Was it a freak thing that happened that no one can predict.
```

---
## \#16 Posted by: LiquidSkater Posted at: 2019-07-01T10:38:11.290Z Reads: 21

```
Thanks a lot! The pack is almost new, it has been charged less than 10 times, I made 8 welds on each battery, 4 on each side, so the welds are ok, I did a pretty good job on soldering too, butb I guss that being  a 15 year old means that I have messed something up :smile: I'll try to take the cells out, and check individually. Thanks again!
```

---
## \#17 Posted by: LiquidSkater Posted at: 2019-07-01T11:03:42.517Z Reads: 21

```
![20190701_135756|374x500](upload://gaQn9uqXkKvt5RNAMzGAtKbrtO0.jpeg) ![20190701_135851|374x500](upload://xdS3AaXD9GqhNI1fDtFnQLEpHzV.jpeg) ![20190701_135912|374x500](upload://yzS7Uil38XkXeun3lPU7YPC5YED.jpeg) 
I reshrinked the batteries when I made the pack, but they are 30q cells, what I don't understand is why at some places there are some black spots between the series, was the shrink too thin or something... Please enlighten me🙂![15619789997907588643123558924380|375x500](upload://kRSXLvpUPud9v2ZApTcaPnO4GKI.jpeg)
```

---
## \#18 Posted by: Darkie02 Posted at: 2019-07-01T11:21:23.747Z Reads: 19

```
![image|375x500](upload://lIGUWh2Yln54AzEzcZ1renXWBem.jpeg) ![image|690x388](upload://6pG1ROp8CL3Je5sHuffzJnJiiBW.png)
```

---
## \#19 Posted by: LiquidSkater Posted at: 2019-07-01T11:23:18.063Z Reads: 19

```
So the current was too high for the nickel strap?
```

---
## \#20 Posted by: Darkie02 Posted at: 2019-07-01T11:39:57.593Z Reads: 20

```
1 of the issues probably overheating and shorting 
no fish paper over positives terminals

No fish paper between p groups

Bad spot welds both over and under current by the looks of it. 
Could be a tip issue, power supply to the welder, the welder it self, a pressure issue, angle tips were held at.

Lack of Vibration protection to prevent shorts

Sharp cornered on nickle strip

But as you stated before 15 year old so it’s all perfect workmanship! will never have any the mistakes some of any other age could have made!
```

---
## \#21 Posted by: LiquidSkater Posted at: 2019-07-01T11:48:24.058Z Reads: 19

```
Thanks a lot, I'll tear this one apart and try to make a better one, add fish paper, use thicker nickel straps. What do you suggest I do to add better vibration protection?
```

---
## \#22 Posted by: Darkie02 Posted at: 2019-07-01T12:01:10.540Z Reads: 18

```
Fish paper works parity good. end of the day e sk8 vibrations are huge nothing is fool proof. 

The black parts are the result of the battery shorting out and arcing and lucky it’s not been on fire 

Off the top of my head 0.15 by 10mm Nickle strips good for about 7 amp.
4p q30 good for about 80 amp.
![ccmcmcmcm|690x461](upload://fIi84E0KBvTFN8VUHd1anWVsAqD.jpg) 

I’d recommend reading up on battery builds plenty advise over the forum on it. Also need s good clean flat surface to get good spot welds.
```

---
## \#23 Posted by: LiquidSkater Posted at: 2019-07-01T12:12:44.255Z Reads: 18

```
ok i'll look into it
```

---
## \#24 Posted by: SimosMCmuffin Posted at: 2019-07-01T12:34:30.479Z Reads: 18

```
[quote="LiquidSkater, post:17, topic:96104"]
![15619789997907588643123558924380|375x500](upload://kRSXLvpUPud9v2ZApTcaPnO4GKI)

15619789997907588643123558924380.jpg3024×4032 1.23 MB
[/quote]

That's a short circuit right there. That might have killed one of your parallel pack. Does the shown negative terminal belong to the 3rd cell group?

Lucky that you didn't get a fire from this.
```

---
## \#25 Posted by: LiquidSkater Posted at: 2019-07-01T14:18:50.037Z Reads: 10

```
Nope, not a short circuit, perfectly good shrink and batteries thats not a short circuit...
```

---
