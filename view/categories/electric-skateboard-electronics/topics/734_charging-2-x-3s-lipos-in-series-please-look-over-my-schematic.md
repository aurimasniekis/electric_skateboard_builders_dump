# Charging 2 x 3S Lipo&rsquo;s in series: please look over my schematic

### Replies: 39 Views: 15204

## \#1 Posted by: trbt555 Posted at: 2015-12-15T21:02:06.786Z Reads: 395

```
Hi all,

I made some balancing harnesses today to charge 2 x 3S packs in series on my 6S charger.
But when I connect them I get sparks. For the life of me, I cannot find what I'm doing wrong.
Can somebody please look over my schematic, have I gotten something wrong ?
<img src="/uploads/db1493/original/2X/9/9ff40f0c99a0eb721f95725032d4b96c3df6d675.png" width="690" height="489">
```

---
## \#2 Posted by: lowGuido Posted at: 2015-12-15T22:01:31.068Z Reads: 368

```
the schematic may be right but are connectors 1 and 2 correctly connected?
```

---
## \#3 Posted by: lowGuido Posted at: 2015-12-15T22:03:17.573Z Reads: 367

```
http://www.electric-skateboard.builders/t/lipo-spark-when-plugging-into-balance-board/243
```

---
## \#4 Posted by: trbt555 Posted at: 2015-12-16T06:31:23.174Z Reads: 349

```
Thanks, you were right, I focussed so much on the balancing leads I didn't pay attention to the way the charge connectors were wired.
I almost toasted my charger.
```

---
## \#5 Posted by: lowGuido Posted at: 2015-12-16T06:47:41.805Z Reads: 340

```
you are lucky you didn't burn out the balancing resistors on the charger output..

oh and for what its worth you don't need to join the red and black balance leads in the middle.
```

---
## \#6 Posted by: trbt555 Posted at: 2015-12-16T10:12:59.457Z Reads: 340

```
Yeah I opened up my charger to check and the resistors had obviously gotten hot but still working but time will tell for how log they will last.

I'm afraid I don't understand your comment on the middle balance leads.
If I don't join the red one, how will my charger know the voltage of the third cell in pack #1 ?

Thanks, Tom
```

---
## \#7 Posted by: lowGuido Posted at: 2015-12-16T10:44:22.003Z Reads: 341

```
The orange wire in your diagram is connected to the  black lead which is connected between the +ve and -ve of the cells exactly the same as every other balance lead.  When you connect the cells in series as you have the positive lead of the first pack becomes the negative of the second pack.
```

---
## \#8 Posted by: longhairedboy Posted at: 2015-12-16T13:46:45.904Z Reads: 354

```
@trbt555 don't forget to re-post your schematic once you get it all worked out if you have any revisions. This is very good information and i'm sure a lot of people are interested in it. I definitely am.
```

---
## \#9 Posted by: trbt555 Posted at: 2015-12-16T19:21:42.417Z Reads: 351

```
@longhairedboy Here's my revised schematic which I wired and tested today. No smoke. No sparks. :smile:

Lesson learned: the wiring of the charging leads and the wiring of the balance leads should match each other otherwise you'll have fireworks. Luckily the only thing I damaged were the pins of the balance lead connectors.

 <img src="/uploads/db1493/original/2X/0/0d165e17b0a0f987036f3ba4f49d6149d1bd5547.png" width="382" height="500">
```

---
## \#10 Posted by: longhairedboy Posted at: 2015-12-16T20:44:19.163Z Reads: 312

```
Excellent diagram. This is the kind of content people come here for. This, a few connectors, a DIY spot welder and some cells is basically all you need to make your own packs :smile:
```

---
## \#11 Posted by: lowGuido Posted at: 2015-12-16T21:40:11.828Z Reads: 303

```
so if you look at this edited diagram:
<img src="/uploads/db1493/original/2X/b/ba7408cd634a6bf9038c3e3014a4c34277fd7f9c.png" width="382" height="500">

the green orange and blue lines are all the same node.
the long green link that you have made with your Y cable is logically the same as the short green line I have drawn.
you can see this now matches the links between each of all the other cells.
each cell "link" has 1 balance lead going to the JST connector.
in this case I have drawn it in orange.
the red balance lead (I have drawn in blue)  is superfluous.

also by removing the red wire from you balance lead helps remove confusion about plugging which in where and generating shorts. the balance lead with the +ve red wire simply connects to the pack with the thick red charge wire.
```

---
## \#12 Posted by: trbt555 Posted at: 2015-12-17T10:12:49.487Z Reads: 283

```
Thanks for that useful insight.
```

---
## \#13 Posted by: rafn97 Posted at: 2015-12-20T18:28:07.384Z Reads: 280

```
Hi,
What software did you use to create this schematic diagram?
```

---
## \#14 Posted by: trbt555 Posted at: 2015-12-20T18:43:29.848Z Reads: 275

```
Microsoft Visio.
It isn't specifically geared towards this kind of stuff but very flexible.
```

---
## \#15 Posted by: rafn97 Posted at: 2015-12-20T18:47:05.146Z Reads: 269

```
Which other programs do you recommend?
```

---
## \#16 Posted by: trbt555 Posted at: 2015-12-20T18:59:48.305Z Reads: 272

```
MS Word and MS Excel ;-)

Google Sketchup.

AutoCad LT.
```

---
## \#17 Posted by: Splinters Posted at: 2015-12-27T07:39:38.405Z Reads: 269

```
If you wire the charge connector directly across the red and black wires on the 6s balance connector, you don't need to connect the power connectors on the packs at all and there's no chance of frying anything.

Of course, this means you are supplying the charge current through the balance wires, but they can easily handle 5A,and it's unlikely you'll be charging at a higher current than this for 3S packs.

(You will need to join the red & black leads on the 3S connectors though, as per @trbt555's original schematic).

<img src="/uploads/db1493/original/2X/4/4c106d6e20c36a6de0a628431044f2100d89fa8c.jpg" width="382" height="500">
```

---
## \#18 Posted by: laurnts Posted at: 2016-01-27T17:50:23.796Z Reads: 249

```
[quote="trbt555, post:9, topic:734"]
@longhairedboy Here's my revised schematic which I wired and tested today. No smoke. No sparks. :smile:

Lesson learned: the wiring of the charging leads and the wiring of the balance leads should match each other otherwise you'll have fireworks. Luckily the only thing I damaged were the pins of the balance lead connectors.
[/quote]

Hahaha this diagram is actually what I needed a month ago before I made some crazy fireworks and damage my connectors as well :smiley:

Nowadays I always check with multimeter the way I plugged in my batteries and use permanent marker to mark them so I didn't plug them wrong. But I understand the idea that positive end of the battery must go on the positive side of the balance lead and the negative end of the battery has to go to the negative side of the balance lead!
```

---
## \#19 Posted by: mason Posted at: 2016-05-02T11:35:29.728Z Reads: 210

```
How do you know that the balance wires can handle 5a? I'm considering trying this myself
```

---
## \#20 Posted by: trbt555 Posted at: 2016-05-02T12:26:45.275Z Reads: 216

```
Look up ampacity for copper conductors.
The max amps you can safely put through a certain cross section of copper wire depends largely on how hot it can get (how hot the insulation can get without melting). I don't know the cross section of your balance wires but I suspect max allowable current will be well above 5A.

If you're really worried you can try to charge one of our lipo's (without balancing) through two wires with the same cross section as your balance wires. If they don't get hot, you're good to go.
```

---
## \#21 Posted by: Splinters Posted at: 2016-05-02T14:55:39.766Z Reads: 210

```
@Link5505 - if you don't want to build your own, you can buy an adapter on eBay that is wired exactly as per my diagram:
http://www.ebay.com/itm/Lithium-Lipo-Battery-Balance-Charger-Twins-Adapter-Charge-For-2x3S-Cells-/172181822194?hash=item2816d61af2:g:zwUAAOSw4hdXIDvC

All you have do do is make (or buy) a set of charging leads that connect your charger power output to the Deans plug on the adapter.
```

---
## \#23 Posted by: ikjahaa Posted at: 2016-06-05T11:49:26.682Z Reads: 187

```
Whenever I do this i get a big spark.
I'm using turingy 20C 3S 5000mah lipo's.
the ballance wires are : 
red - yellow - white - black

I did the charge leads first. Then I started to do the ballance leads, but I get a spark whenever my red and black wires touch. This only occurs if the charge leads are connected.

<img src="/uploads/db1493/original/2X/9/9161770a4d2150cc7ec3368e322631d4275f25f5.png" width="640" height="400">
```

---
## \#24 Posted by: lowGuido Posted at: 2016-06-05T11:52:36.810Z Reads: 178

```
your  JST leads are back to front.. 

and that Diagram probably would have beat mine in the beautiful diagrams comp.
```

---
## \#25 Posted by: ikjahaa Posted at: 2016-06-05T11:55:20.397Z Reads: 181

```
yea, I saw it too just now as I was looking at @trbt555's diagram and thinking of what i could have possibly done wrong. Silly me.
```

---
## \#26 Posted by: Yannickseskate Posted at: 2016-11-05T18:46:00.174Z Reads: 134

```
I did exactly the same thing but sometimes my charger says: error Input voltage. What does that mean and how can I fix this?
```

---
## \#27 Posted by: DeathCookies Posted at: 2016-11-07T09:12:29.415Z Reads: 127

```
Either your Voltage of at least one cell is to low or you want to charge 6S while you have a 5S battery attached.
```

---
## \#28 Posted by: Yannickseskate Posted at: 2016-11-08T15:45:22.222Z Reads: 126

```
I have two 3s lipos in series but it could be that one balance charging pin is burnt
```

---
## \#29 Posted by: Challlsss Posted at: 2017-05-03T13:26:16.359Z Reads: 90

```
@lowGuido I remobed the #4 black wire on pack #1 and charged like I think you say in this post, BUT when I plugged everything in my charger started smoking. The only way to make it work was to use both the Negative #4 on pack #1 and the Positive #1 on pack #2 Thoughts?
```

---
## \#30 Posted by: Maxid Posted at: 2017-05-03T13:33:01.931Z Reads: 83

```
sounds to me like you just messed up the order the first time.
The order in the balance wire needs to reflect the order of the batteries.
You probably just paid more attention the second time and connected them properly.
```

---
## \#31 Posted by: Challlsss Posted at: 2017-05-03T13:51:15.691Z Reads: 79

```
I guess it is possible... However I tried it 2x and triple checked before I plugged everything in. Also while plugged in the balance charged detected 5 cells.... Does that mean it was backwards?
```

---
## \#32 Posted by: lowGuido Posted at: 2017-05-03T22:22:42.173Z Reads: 78

```
If it started smoking then you hooked it up wrong.
That charger is probably damaged now. you would have fried the resistors on the ballance connections. 

You need to make sure every cell is in the correct order.
```

---
## \#33 Posted by: Challlsss Posted at: 2017-05-04T13:05:15.341Z Reads: 75

```
I would've thought that too. But once I added the second wire it worked fine. I'm going to take apart the charger and see if there's anything I can do to fix her up. We shall see....
```

---
## \#34 Posted by: lowGuido Posted at: 2017-05-05T11:15:39.867Z Reads: 75

```
if its burnt out the bank of resistors you can just replace them..
```

---
## \#35 Posted by: Challlsss Posted at: 2017-05-05T13:09:26.045Z Reads: 72

```
Yeah I opened it up and the resistors are completely fried. I'm going to try and replace them, but they may have gone through more than just the first layer on the board.
```

---
## \#36 Posted by: lowGuido Posted at: 2017-05-05T21:34:39.302Z Reads: 67

```
So the fact that those resistors are fried is further proof that you had it wired the wrong way. Mixing up the balance leads puts about 25V across those resistors when there is only supposed to be around 3V.
```

---
## \#37 Posted by: Challlsss Posted at: 2017-05-08T16:57:41.873Z Reads: 68

```
Yeah I replaced the resistors and it works fine now
```

---
## \#38 Posted by: Ingvarjedi Posted at: 2017-07-27T21:33:32.428Z Reads: 49

```
Which of these schemes is correct? I'm confused.
```

---
## \#39 Posted by: metos Posted at: 2017-07-27T21:55:28.291Z Reads: 45

```
I charge 2x 3s at a time it works well

[img]http://www.albworkshop.fr/app/media/306721?resize=800x800>[/img]
```

---
## \#40 Posted by: Jpro Posted at: 2018-05-05T15:57:03.983Z Reads: 20

```
After making a series connection what side becomes positive and what side becomes negative or dose it not matter?
```

---
