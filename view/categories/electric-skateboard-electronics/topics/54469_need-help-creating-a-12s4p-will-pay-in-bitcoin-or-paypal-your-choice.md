# Need help creating a 12S4P - will pay in Bitcoin (or Paypal) - your choice

### Replies: 40 Views: 2526

## \#1 Posted by: ripcurldog Posted at: 2018-05-05T08:49:06.145Z Reads: 313

```
I need some help and am willing to compensate you with a bit of Bitcoin, or Paypal (whichever you prefer0. 
 
I just purchased a Trampa electric mountain board (beast of a board).  I am getting ready to build my own 12S4P 18650 battery, using 48 * Samsung 30Q's.  The Tramps E-mountainboard comes with a case for a battery, and although 48 cells will fit within the case, they need to be laid out in a specific format (see image):

![batterysetup|375x500](upload://pIs051XiXn7m3ZNLTJV2E6tGSU6.jpg)

I would like to see if anyone can help me with a wiring diagram for this setup?  I also need the following included in the diagram:
1):  location for the 12S BMS wiring.
2):  how to attach my LED battery display?
3);  How to attach a ON/OFF SWITCH with ANTI SPARK?
4):  The best method to charge this using a 4amp charger, found here (where to buy a connector, how to connect, etc.).:
products/12s-4a-battery-charger?variant=7296823853079

I think I have most components (some have arrived, some are on the way).  I already have the Spot wedler and the rest of the tools to do this, but this will be my first DIY battery, so looking for some help and willing to pay for your time ($50 in Bitcoin, or a direct payment via Paypal after completion - i'm good for it :-).
 
My email is brettdenaro@gmail.com.

Cheers.
```

---
## \#2 Posted by: koralle Posted at: 2018-05-05T08:58:03.274Z Reads: 297

```
Hey mate do you want someone to be physically there and help you or just information? I think you can get all the information you need and more here for free if you ask the right questions and back them up with pics.

edit: nevermind just read your post properly - you need a wiring diagram.
```

---
## \#3 Posted by: koralle Posted at: 2018-05-05T09:00:53.921Z Reads: 290

```
pic of your anti spark and bms pls
```

---
## \#4 Posted by: chocol4te Posted at: 2018-05-05T09:04:59.440Z Reads: 295

```
Here's one for free. You'd be best served making 12 packs of 4 cells in parallel, then arranging in the following pattern so your positive and negative terminals are at the same end:

![IMG_0668|375x500](upload://heKQ4CKMm5b0v0M9kZEBhoW0D1W.JPG)


Please excuse my poor drawing skills. The middle 2 rows are underneath the top and bottom rows. I also drew a a side view.

Out of interest, why are you double stacking the cells? You could easily fit a single layer on a Trampa mountainboard by making it longer.

1) The BMS leads should attach to the positive and negative terminals of the battery (+) and (-) on the diagram, and the balance wires go between each pack.

2) LED battery display also attaches to the battery terminals

3) Switch and anti spark goes in series with either the positive or negative lead from the BMS to the ESC.

4) Charger can be attached to the BMS charge input, but I don't know which BMS you have so I don't know where those would be.
```

---
## \#6 Posted by: Namasaki Posted at: 2018-05-05T17:50:13.548Z Reads: 242

```
Check here for diagrams. There might be one you can use. 

http://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2018-05-05T17:58:32.838Z Reads: 233

```
im using the pictures of actual gear, it can help giv ideas
```

---
## \#8 Posted by: ripcurldog Posted at: 2018-05-05T18:08:20.470Z Reads: 245

```
Thank you so much for your help - VERY much appreciated.  
The battery pack and the 'Beast Box' (this is what Trampa calls the battery enclosure) sit on top of the deck, in between the riders feet.  The reason being that this particular board is the Mountainboard version (versus the street or urban version).  The E-Mountainboard is designed to go anywhere (rocks, etc.), so clearance at the bottom of the deck is important when off-roading.
 
Can you double check that I have this right (see image)?  Also, for the 12 groups of four cels, do I spot weld all four together like I have done in the diagram?
![BatteryDiagram|690x359](upload://hklJpfx1Fivrh4MRgO3hGCRyX3S.JPG)
```

---
## \#9 Posted by: ripcurldog Posted at: 2018-05-05T18:12:22.662Z Reads: 227

```
Hi,
here is the Anti Spark ON/OF switch:
https://www.ebay.com/itm/Anti-Spark-Power-On-Off-Switch-for-VESC-or-ESC-electric-skateboard-longboard-LED/162991392682ssPageName=STRK%3AMEBIDX%3AIT&var=462107277751&_trksid=p2057872.m2749.l2649

![AntiSpark|656x500](upload://x5peNIKhdGxF3cgLYjmyUwayvwV.jpg)

And here is the 12S BMS:
https://www.ebay.com/itm/44V-48V-50-4V-12S-60A-Lithium-ion-Li-ion-LiPo-Li-Polymer-Battery-BMS-PCB-System/221644780045?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2648

![BMS|500x373](upload://jp5YVGVnY4lvz224u1FmWIpofm1.jpg)
```

---
## \#10 Posted by: ripcurldog Posted at: 2018-05-05T18:16:05.519Z Reads: 208

```
Yeh, I woke up this morning to you and one other person offering to help for free, AMAZING!  I am planning to do the work myself, but want to make sure I dont fry 48 expensive batteries by wiring them together incorrectly, so I am looking for a wiring diagram to help me.  I posted pics of the BMS and Anti Spark on/off switch below.  Thank you again!
```

---
## \#11 Posted by: ripcurldog Posted at: 2018-05-05T19:48:56.966Z Reads: 200

```
PS:   If my batteries are Samsung 30Q 15amp, will a 60amp BMS do, or can I go higher (120amp)?
```

---
## \#12 Posted by: myreala Posted at: 2018-05-05T19:52:27.383Z Reads: 190

```
No you can go max of 80A, 30q run cooler at 60A though. A 80A bms would be a good Choice.
```

---
## \#13 Posted by: myreala Posted at: 2018-05-05T19:55:22.811Z Reads: 186

```
Your parallel arrangement looks wrong to me, in parallel all four cells positive terminals should only be touching positive terminals. There should be no positive negative connection in 4 parallel cells.
```

---
## \#14 Posted by: chocol4te Posted at: 2018-05-05T20:27:17.761Z Reads: 182

```
Yes, everything but the parallel pack is right. Each set should be 4 in a row batteries all facing the same way - all the positive terminals together and all the negative. At the top right end you will have a 4 long 2 high set of battery ends that need connecting, on the left it will be a 1 high 8 long set and then on the bottom right you will have another 4 long 2 high. So in total the pack will be 3x8x2 batteries.
```

---
## \#15 Posted by: chocol4te Posted at: 2018-05-05T20:30:22.998Z Reads: 178

```
30Qs can do around 20 amps safely, so 80 amps is good :)
```

---
## \#17 Posted by: strattos Posted at: 2018-05-05T22:31:10.074Z Reads: 167

```
Their spec sheet says a single cell can do 80Amps lol but that isn't continuos. Highly wouldn't recommend it but take a look here https://www.google.ca/url?sa=t&source=web&rct=j&url=https://eu.nkon.nl/sk/k/30q.pdf&ved=2ahUKEwi23cvvzu_aAhUL02MKHb2aCSUQFjABegQIARAB&usg=AOvVaw279pV66YaEwoyM-XVvSkL-

Lots of good info there.
```

---
## \#18 Posted by: pat.speed Posted at: 2018-05-05T23:06:18.611Z Reads: 167

```
This is what you need to do, just repeat the step until you have 12 lots. Ignore the writing and stuff.



![image|359x410](upload://4QYEzJUJQv8aT9LVBD0hrNm7K0a.jpeg)
```

---
## \#19 Posted by: koralle Posted at: 2018-05-05T23:53:02.673Z Reads: 165

```
1. get some pure and thicc nickel strip

2. make sure your welds really stick

3. weld and fold your packs like this twice to get your desired form. Dont forget to weld the solder tabs for bms wires before folding.

![battery|690x428](upload://8QhX6HlG7VUHrOnStlMMxZad4mi.jpg)

4. Connect like this

![12s4p diagram|690x404](upload://89LONXlA9ap2pWUiz66RLBeBlkL.jpg)
```

---
## \#20 Posted by: ripcurldog Posted at: 2018-05-06T01:53:19.969Z Reads: 153

```
Hey this is amazing - very clear and easy to follow.  Thank you!
```

---
## \#22 Posted by: ripcurldog Posted at: 2018-05-06T02:00:19.599Z Reads: 145

```
So would you suggest sticking with the 60amp BMS over the 80?
```

---
## \#23 Posted by: ripcurldog Posted at: 2018-05-06T04:30:57.769Z Reads: 143

```
Will this charger work okay with the battery pack, and do you know where I can buy the connection for the battery to connect to that charger?

products/12s-4a-battery-charger?variant=7296823853079
```

---
## \#24 Posted by: strattos Posted at: 2018-05-06T04:57:46.374Z Reads: 145

```
I went for an 80 Amp myself the cells can handle being discharged without over heating at that rating and even more peak (most bms have double the peak rating of continuous I find). Plus its so unlikely that i'd ever pull that much current for more than a few seconds. 

Also i'd rather have something rated for a bit higher than spec with these chinese bms's
```

---
## \#25 Posted by: Naysh Posted at: 2018-05-06T05:12:57.830Z Reads: 144

```
Stop right there! Do not build a pack with Li-ions with that type of enclosure.  I've had the Trampa Beast Box enclosure (similar)but they are built for Lipos which are bulky and square and no room to be creative with the enclosure shape.  With 18650 cells, you can get more creative,  you can fit that into an enclosure that @eboosted has available, flex and under the deck,  real slick looking stuff.  The problem with the Trampa beast box enclosure is that you had 8 bolts to unscrew then take your Lipo batteries out, bolts would fly to the ground and you'd have to pick it up one by one then after the Lipos were charged you had screw it in back in one by one sometimes the nuts would come out and you'd have to pick it up one by one.  Better have it done by @Eboosted, he's a good battery maker too from the work I've seen.

http://www.electric-skateboard.builders/t/eboosted-enclosures-thread/38073
```

---
## \#26 Posted by: koralle Posted at: 2018-05-06T10:44:50.236Z Reads: 127

```
That charger will be fine. Connector should be 5.5x2.1 panel mounted
https://goo.gl/e3dmxG
```

---
## \#27 Posted by: ripcurldog Posted at: 2018-05-06T19:50:28.435Z Reads: 117

```
Sweet, thanks a million!
```

---
## \#28 Posted by: ripcurldog Posted at: 2018-05-06T19:54:37.410Z Reads: 112

```
This is a mountainboard, so it will be mostly ridden over dirt and rocks.  That’s the reason why some Trampa boards have the battery on top of the deck, between the feet.  I already have the evolve carbon GT, so this second board is being for true off road performance.  Also, the Trampa beast box is designed with holes to where you shouldn’t need to open the enclosure once you have finished, and tested the battery.
```

---
## \#29 Posted by: Naysh Posted at: 2018-05-06T21:57:23.237Z Reads: 104

```
My bad, I made the assumption that you were using a emtb for street use, many use it as that.  Why didn't you just go with Lipos, the C ratings are much higher for the same price point.  They don't have a higher cycle rating as li ions though.
```

---
## \#30 Posted by: strattos Posted at: 2018-05-07T03:10:29.095Z Reads: 94

```
Liion>Lipo in almost every way but price
```

---
## \#31 Posted by: ripcurldog Posted at: 2018-05-07T04:13:00.116Z Reads: 95

```
It would have been easier for sure, but from what I have read and watched (youtube videos), the 18650 battery pack (12S4P using Samsung 30Q) is going to to last much longer than something like Hobbyking Li-ion packs (as far as the amount of full charfge/discharge cycles I will get from the batteries).  I am also hearing that the 18650 cells are many times less likely to start a fire, and since I have a baby girl, safety is important here.
```

---
## \#32 Posted by: Naysh Posted at: 2018-05-08T00:18:54.638Z Reads: 91

```
I hear ya.  Safety will always come first especially if you've got a little one.  From what I've read in these forums the majority of e-mtbs are using lipos and I can't remember the reason why.  Just looking at setups from here and in YouTube almost all are using lipos with the boxes on top.
```

---
## \#34 Posted by: koralle Posted at: 2018-05-08T08:04:19.707Z Reads: 89

```
Lipos generally have a much better C rating than Li ions. A 10s2p li ion is a bad idea because it would get crazy voltage sag. 10s2p lipo is rock solid.
The lipos also have a higher energy density. 

Another tip for welding : be sure to *always* apply a decent amount of pressure on your copper electrodes when welding! If something doesn't make a good connection, you're going to blast a hole in your battery.
```

---
## \#35 Posted by: ripcurldog Posted at: 2018-05-08T09:09:20.286Z Reads: 79

```
Hi. I'm making a 12S4P Li-ion pack.  I'm using Samsung 30Q's, 48 total.  They are rated 15a but can do up to 20a according to some people.  So you think the 4 LiPo packs would have more power?
```

---
## \#36 Posted by: koralle Posted at: 2018-05-08T10:13:26.663Z Reads: 84

```
[quote="ripcurldog, post:35, topic:54469"]
4 LiPo
[/quote]

please be more specific
```

---
## \#37 Posted by: ripcurldog Posted at: 2018-05-09T00:49:03.144Z Reads: 78

```
Which would provide more torque:

LiPo config = Hobbyking 6S 6200Mha 40C - four of them for a (12S4P).

Versus

 Li-ion - 12S4P using Samsung 30Q rated 15A.  48 cels total.
```

---
## \#38 Posted by: koralle Posted at: 2018-05-09T00:52:13.408Z Reads: 75

```
I don't think with 12s4p, too little torque will be your problem but yeah Lipos can supply more amps than Li Ion without voltage sag - so more Torque, if the rest of your components can handle it.
```

---
## \#39 Posted by: ripcurldog Posted at: 2018-05-09T01:52:08.319Z Reads: 78

```
I have 2 * VESC.
TRAMPA ELECTRIC Mountainboard - TWIN PRO Motor Mounts
Electric MTB Vertigo Trucks 8 inch Superstar Wheels Ratchet
Bindings - 685e PRO BLACK TWIN Motor
685e E-MTB PRO Vertigo Superstar BLACK
- TWIN Motor
15ply 35º HS11 Electric Board - FIRM
RED DAMPA's - 80a Stiff Steering
136kv TRAMPA Motor - All Round Performance
14 Tooth - All Round gearing
Powder Coated RED Springs
Heel Straps with RED Ratchets
HOBBYKING Rechargable Remote Inc Battery - Pistol grip Finger operated
```

---
## \#40 Posted by: ripcurldog Posted at: 2018-05-09T01:52:53.903Z Reads: 82

```
![trampa1|375x500](upload://stmgOUf8SC0WRpcejChdGFMN5qf.jpg)
```

---
## \#41 Posted by: elaser Posted at: 2018-05-09T08:29:28.080Z Reads: 76

```
hello all, I've been reading here a lot of post regarding batteries and bms and about  Lipos vs li-ion (18650) and the figure I got from the posts here are:
25R - 80 amp cont. discharge/10AH/37v
30Q - 60 amp cont. discharge/12AH/37v
 you probably don’t want to set your battery max to the equivalent of any more than 10-15A per a 30Q cell so multiplied for 4p it gives you that 60amp figure.
The situation is different with the [21700](http://lygte-info.dk/review/batteries2012/Samsung%20INR21700-30T%203000mAh%20(Gray)%20UK.html) with 35A max discharge rate.
[Here an interesting thread on the subject](http://www.electric-skateboard.builders/t/sanyo-2170-battery-ncr20700b/20800/12)
How much amp is needed depends on the kv of the motor. Lower kv like yours means less amp but also lower erpm. For a mountainboard it can have very high energy spikes even at 120a (see [Nowind driving leopard](https://www.youtube.com/watch?v=P_thNysQvNI) ) so it's not a fair comparison but if you go uphill or on dirt I'm sure it can reach that amount of current easily. 
So that's probably why most mountain board riders prefers Lipos even if they are bulky and more expensive at the end.
Do you need a BMS rated for 120A? no you can avoid it completely for the discharge part and get a cheaper one and connect directly the battery to the vesc and let the vesc control the current drawn.
```

---
## \#42 Posted by: ripcurldog Posted at: 2018-05-09T08:50:22.803Z Reads: 81

```
Hi, Can you please clarify something for me (is the blue fold line in my image below correct).  You have your fold line in a place that confuses me (I am new to this).  When you fold your battery, don't you want the positive to be connecting to a negative?  Here is my pack.  So if the blue line is my fold line, is this correct?  I am making a 12S4P battery (I have another row of batteries which I have not yet added to the configuration yet).  I've also included the raw image without editing in case i've confused you (I really appreciate your help!).

My fold line:

![Battery_Folded|377x500](upload://q0scE71frRDa0r9xmomVdm9CERL.JPG)

Battery, raw image:

![Battery_raw|422x500](upload://agPlOJlMhSKcqYkus0SvU9oea7K.JPG)
```

---
## \#43 Posted by: ripcurldog Posted at: 2018-05-09T17:41:37.914Z Reads: 73

```
Thanks for this info.  I've noticed that mountainboards that use LiPo's do not have a BMS on those LiPo's.  Why is it that LiPo's dont need a BMS yet LI-Ion require one?
```

---
## \#44 Posted by: elaser Posted at: 2018-05-09T17:51:20.138Z Reads: 71

```
You can connect LiPo to BMS [(see for example here)](http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/87) it's just uncommon since LiPo charger are usually balanced so you connect to them and for discharge is not mandatory as I was writing.
Li-ion battery are more subject to voltage sag so your battery dies earlier even if in theory is has more mAh then a LiPo... So numbers doesn't always tell the true story ([I was reading this](http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/87) up to the end)
```

---
