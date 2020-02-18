# Ebay dangerous jst connector

### Replies: 18 Views: 3058

## \#1 Posted by: stuxtruth Posted at: 2016-01-02T19:48:56.000Z Reads: 153

```
So I order a jst series connector from ebay so I can charge my 2 3s batteries at the same time and turn 2 3s batteries into one 6s battery essentially. But when I go to plug them in it sparks and smokes. Who can tell what is wrong with the wiring?<img src="/uploads/db1493/original/2X/5/54f1ab195acc3be3c65f925921a439116cd1bf52.jpg" width="281" height="500">
```

---
## \#2 Posted by: psychotiller Posted at: 2016-01-02T20:07:15.207Z Reads: 147

```
You need to cut that middle red wire. They all come that way.
```

---
## \#3 Posted by: stuxtruth Posted at: 2016-01-02T20:19:30.760Z Reads: 144

```
Thanks!

<img src="/uploads/db1493/original/2X/b/baa2a468e93fc2c6f5e310584ba2ed42f1428291.jpg" width="690" height="388">
```

---
## \#4 Posted by: stuxtruth Posted at: 2016-01-02T20:33:13.516Z Reads: 138

```
<img src="/uploads/db1493/original/2X/5/578c29ca00a8b0f12b0a691ef739a3ef26d4fff3.png" width="281" height="500">

Now I'm wondering if I shouldn't have cut the red wire.
```

---
## \#5 Posted by: chaka Posted at: 2016-01-02T20:37:24.985Z Reads: 133

```
Nope you shouldn't have. You had them plugged in backwards. You need to swap the balance leads so they are in the proper order in series.
```

---
## \#6 Posted by: stuxtruth Posted at: 2016-01-02T20:44:32.118Z Reads: 132

```
Well I guess I'm ordering another lol.
```

---
## \#7 Posted by: chaka Posted at: 2016-01-02T20:49:41.610Z Reads: 134

```
No soldering iron? Nudge nudge.
```

---
## \#8 Posted by: stuxtruth Posted at: 2016-01-02T20:51:05.515Z Reads: 134

```
Yes I do but I'm very OCD when it comes to cleanliness and the connector was 4.99 shipped
```

---
## \#9 Posted by: psychotiller Posted at: 2016-01-02T20:55:11.429Z Reads: 138

```
I thought that was the only way you could balance charge in series. Parallel is different
```

---
## \#10 Posted by: lowGuido Posted at: 2016-01-02T22:12:30.437Z Reads: 135

```
Cutting the red wire is fine. In fact I recommend it. 
There is already 2 other topics on this exact thing.
http://www.electric-skateboard.builders/t/lipo-spark-when-plugging-into-balance-board/243
http://www.electric-skateboard.builders/t/charging-2-x-3s-lipos-in-series-please-look-over-my-schematic/734
```

---
## \#11 Posted by: stuxtruth Posted at: 2016-01-03T01:49:30.429Z Reads: 120

```
<img src="/uploads/db1493/original/2X/a/a2610d83103ae0714b003c4fabd6c15dca4a5627.png" width="281" height="500">
```

---
## \#12 Posted by: stuxtruth Posted at: 2016-01-03T02:09:20.825Z Reads: 113

```
I de-pinned the red wire. The charger seems to read all 6 cells fine and charge fine but the max amps it will charhe with both hooked up at the same time is 2.2 amps rather than 4.2 with each 3s hooked up at once. [Uploading...]()
```

---
## \#13 Posted by: lowGuido Posted at: 2016-01-03T02:11:08.205Z Reads: 113

```
Continuing the discussion from [Charging 2 x 3S Lipo&#x27;s in series: please look over my schematic](http://www.electric-skateboard.builders/t/charging-2-x-3s-lipos-in-series-please-look-over-my-schematic/734/11):

[quote="lowGuido, post:11, topic:734, full:true"]
so if you look at this edited diagram:
<img src="/uploads/db1493/original/2X/b/ba7408cd634a6bf9038c3e3014a4c34277fd7f9c.png" width="382" height="500">

the green orange and blue lines are all the same node.
the long green link that you have made with your Y cable is logically the same as the short green line I have drawn.
you can see this now matches the links between each of all the other cells.
each cell "link" has 1 balance lead going to the JST connector.
in this case I have drawn it in orange.
the red balance lead (I have drawn in blue)  is superfluous.

also by removing the red wire from you balance lead helps remove confusion about plugging which in where and generating shorts. the balance lead with the +ve red wire simply connects to the pack with the thick red charge wire.
[/quote]

pay special attention to this part:
[quote]also by removing the red wire from you balance lead helps remove confusion about plugging which in where and generating shorts. the balance lead with the +ve red wire simply connects to the pack with the thick red charge wire.
[/quote]
```

---
## \#14 Posted by: stuxtruth Posted at: 2016-01-03T02:15:17.241Z Reads: 99

```
Thanks for the clarification.
```

---
## \#15 Posted by: mattdig Posted at: 2016-05-01T14:50:22.801Z Reads: 80

```
Do not unplug that wire. Get a new connector. You're going to ruin your battery.
```

---
## \#16 Posted by: thisrealhuman Posted at: 2016-05-01T15:05:30.341Z Reads: 81

```
I have the same charger, it is only 50W. 50w / 22.2v =2.2A.
I charge 5s in parallel, my max is 2.6A.
```

---
## \#17 Posted by: laurnts Posted at: 2016-05-01T23:21:12.071Z Reads: 75

```
This is what as chaka said, you need to switch the balance plug around. You dont need to cut anything. If the series harness is always attach, cutting or not cutting doesnt change anything. If you cut it and you detatch series harness it wont charge as 6s batteries.
```

---
## \#18 Posted by: lowGuido Posted at: 2016-05-06T08:00:52.571Z Reads: 60

```
I always suggest you cut the red wire off because if you do accidentally get it the wrong way around you wont short across your entire battery.

you are right it makes absolutely no difference if its cut or not, but its just safer to be cut. in case..
you still need to put them the right way around in either case.
```

---
