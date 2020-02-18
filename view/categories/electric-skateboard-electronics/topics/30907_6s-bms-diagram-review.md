# 6S BMS Diagram Review

### Replies: 18 Views: 2091

## \#1 Posted by: brok249 Posted at: 2017-08-17T18:13:28.245Z Reads: 126

```
Hello!

I finished my esk8 (The Globetrotter) a fair number of weeks ago but finally got around to getting a BMS so I don't have to lug around an iMax B6 ACV2. I wasn't completely sure on how to wire the BMS but after looking at a few diagrams I constructed my own as it helps me keep my head on straight while dealing with circuits and wiring (otherwise I just get confused and give up). This is what I've got, all wires are colored the same in the diagram as their real-counterparts.

<img src="/uploads/db1493/original/3X/9/1/91f88b3ef670284f7019e947ae1925c59ef00f49.PNG" width="690" height="339">

I matched the interior 5 wires by laying both my 6S connector and the connector on the BMS in the same orientation and matching the wires. For reference and to ensure this should work, [this](http://www.ebay.com/itm/Protection-Balance-Module-BMS-PCM-12A-for-6S-22-2V-Li-ion-Li-Po-battery-6S12W003/321790732770?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649) is the BMS I purchased. 

Thanks in advance.
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-17T18:21:35.511Z Reads: 98

```
You may want to have have the thicker wire on B- split off and go to B- on the BMS. Some BMS's are picky about this and the B- from the balance lead may not be enough.
```

---
## \#3 Posted by: krloz Posted at: 2017-08-17T19:21:28.369Z Reads: 89

```
@Jinra is right there.  You are going to be charging through that bms and a couple of amps is to much for the thin balancing wires they're good enough for balancing though.  So wire your B+ and B- to the thick wires of the battery instead of the thin equivalents
```

---
## \#4 Posted by: brok249 Posted at: 2017-08-17T20:14:49.271Z Reads: 75

```
And as long as I don't have the loop key in while charging this should prevent any discharge through the BMS. Makes sense now. And just to be sure, wire the thicker wires INSTEAD of the thin wires (because they serve the same purpose), not in addition.
```

---
## \#5 Posted by: krloz Posted at: 2017-08-17T20:46:41.130Z Reads: 73

```
the bms you posted only has 5 pins in the balance connector. that is because it only carries the between cells connections and the ends of the battery packs are connected to the b+ and b- making a total of 7 conections battery->bms wich is what is expected on a 6S. always one wire more than the cell count. 
inside a baterry the balance conector is wired to all between cells conections and the + and - for balancing and in adition to thick wires to the battery ends for charge and discharge. so inside the battery you have the end connections duplicated. 
and yes as they are welded to the same place better use the thick ones. not necesarily instead but wiring them both would be unnecesary.
```

---
## \#6 Posted by: brok249 Posted at: 2017-08-17T21:01:22.031Z Reads: 65

```
Great, I knew the function and how the wires worked but just wanted to make sure. I'll hopefully work on it this weekend and post the result when done. Thanks so much for your help! You too @Jinra.
```

---
## \#7 Posted by: ReeCorDs Posted at: 2017-11-23T15:27:43.784Z Reads: 53

```
Hello, i will also build an electric skateboard with the same BMS and two 3S batteries. Now, i just want to make sure if i understood it right: 

<img src="/uploads/db1493/original/3X/9/b/9b22c0ddc68d53d681458dec34a95581f0459423.png" width="690" height="339">

Is it right to wire three of the balancing cables of the first battery including the black negative to the BMS and only two of the second battery also to the BMS? And why the negative cable and not the positive of the balancing cable?

Sorry for my bad english, i'm from germany! :-D
```

---
## \#8 Posted by: bluemoon Posted at: 2018-01-12T00:31:03.879Z Reads: 48

```
I would also like to know if this would be okay? I am in the same boat. 
@Jinra @krloz  I noticed you may have some valuable knowledge. Any thoughts?
```

---
## \#9 Posted by: ReeCorDs Posted at: 2018-01-12T11:05:31.787Z Reads: 43

```
Hi! I went from 6S to 10S and made a diagram which is correct. It bypasses the discharge because my BMS has not enough ampere:

![Longboard diagramm - Kopie - Kopie - Kopie - Kopie - Kopie|690x331](upload://7gSiXRr10YrcGvrHOIj9k2YQm0l.png)

Otherwise, i think this is right for 6S:

![Longboard diagramm - Kopie - Kopie|690x331](upload://kjGu6ABWgxy8ymhBDB6HhmnEfe1.jpg)
```

---
## \#10 Posted by: krloz Posted at: 2018-01-12T11:38:14.331Z Reads: 41

```
[quote="bluemoon, post:8, topic:30907"]
if this would be okay
[/quote]

What do you mean by this exactly?
```

---
## \#11 Posted by: krloz Posted at: 2018-01-12T11:41:23.937Z Reads: 38

```
 It's hard to tell on the phone with so much small wires so close but I think both diagrams are correct for a bms that carries both + and - independent from the balance connector.  Ie the balance connector hag one pin less than the cell count
```

---
## \#12 Posted by: bluemoon Posted at: 2018-01-12T15:09:49.372Z Reads: 37

```
Okay great, Just wanted to make sure before I wired everything up. 

Thank you for your time : )
```

---
## \#13 Posted by: bluemoon Posted at: 2018-01-12T15:12:09.852Z Reads: 36

```
Thank you for the diagrams very helpful.
```

---
## \#14 Posted by: ReeCorDs Posted at: 2018-01-12T19:24:00.882Z Reads: 32

```
You are welcome! :slight_smile:
```

---
## \#15 Posted by: EvanWhy Posted at: 2018-09-08T20:40:20.275Z Reads: 15

```
In this diagram, is the bms wired only for charging purposes?
```

---
## \#16 Posted by: danile Posted at: 2018-09-08T21:44:59.967Z Reads: 14

```
Yes.
I did this mod recently and made a post about it: https://dosimplecarbon.com/how-to-wire-6s-bms-to-your-2x3s-lipo-esk8/
The diagram is more elaborate imo

Dani
```

---
## \#17 Posted by: EvanWhy Posted at: 2018-09-11T19:41:58.664Z Reads: 14

```
Hey I'm about to hook up my bms for charging purposes and want to make sure I do it right. I am using two 3s lipos in series. Also would you recommend soldering or just putting the wires into connectors and hot gluing. I also plan on using 10 gauge wire to attach directly to the p- b- and positive charging input. is this correct?

![20180911_123629|281x500](upload://vtGcVSTBaNeLzFj68vdWOr3qAFk.jpg)![20180911_123652|281x500](upload://jFnBzOka61Hswc3sTbH3weObZpq.jpg)
```

---
## \#18 Posted by: danile Posted at: 2018-09-12T19:16:21.789Z Reads: 11

```
Looks good.

As long as you don't run 1-2A to charge, 10awg should be fine.
I always use soldering, that will be my recommendation.

Dani
```

---
