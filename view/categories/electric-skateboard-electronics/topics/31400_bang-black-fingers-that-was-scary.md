# Bang! Black Fingers! That was scary!

### Replies: 28 Views: 1654

## \#1 Posted by: flywithgriff Posted at: 2017-08-24T17:16:06.265Z Reads: 284

```
I'm in the process of wiring a 10s2p lipo pack. I connected all of the balance leads and without thinking attempted to join the two 10s1p packs in parallel. In case you didn't know, it makes a big spark!! And will also turn your fingers black! Any chance this killed a pack?
<img src="/uploads/db1493/original/3X/1/9/195c725ee2a250bdb1d8c53722f270c71c79ddbb.JPG" width="500" height="500">
```

---
## \#2 Posted by: wafflejock Posted at: 2017-08-24T17:22:21.762Z Reads: 278

```
If it was momentary contact it should probably be fine, the quick charging of the battery with lower voltage from the one with higher voltage might have caused some damage to that battery.

If there is a large voltage difference between two batteries and you connect them in parallel you effectively end up dumping charge from the higher voltage one into the lower voltage one, this is okay if there isn't a big difference but in this case it must have been pretty substantial.  Would check both batteries with a voltmeter or if you have it a balance lead tester (can also do that with a voltmeter but a bit more tedious trying to keep on the contacts).
```

---
## \#3 Posted by: ShutterShock Posted at: 2017-08-24T17:22:47.613Z Reads: 269

```
That must have been quite the startling experience haha :grin:

I would imagine the pack is fine, just got a big spark from the high voltage, I would check each cell and see if they are still balanced.
```

---
## \#4 Posted by: thisguyhere Posted at: 2017-08-24T17:25:57.777Z Reads: 259

```
This is how I destroyed my first bms...
```

---
## \#5 Posted by: wafflejock Posted at: 2017-08-24T17:27:27.812Z Reads: 258

```
Yeah it's a pretty common problem when people are hooking up quadcopter batteries for parallel charging.  I have a parallel charging board but never really used it somewhat out of fear of frying something (think I understand this all well enough to use it now but just haven't done it yet).
```

---
## \#6 Posted by: Deckoz Posted at: 2017-08-24T17:29:31.150Z Reads: 249

```
Those bullets look a little small.... you should be using 5.5mm  bullets...the spark will be like a nuclear reactor, but shouldn't do to much... just gotta make sure the bullets you use can carry the ampacity of the inrush current. but really, wire in an antispark xt90 loop key
```

---
## \#7 Posted by: flywithgriff Posted at: 2017-08-24T18:06:56.535Z Reads: 223

```
It was certainly a startling experience! The tow batteries were about 4% apart in voltage. I was expecting a small pop when they equalized but damn! I am using xt90 connections for the final wiring. I was simply touching them to release this spark.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-08-24T19:57:23.198Z Reads: 187

```
[quote="flywithgriff, post:7, topic:31400"]
I was simply touching them to release this spark.
[/quote]

And it has work 😜
```

---
## \#9 Posted by: flywithgriff Posted at: 2017-08-24T19:58:01.019Z Reads: 185

```
Haha it definitely worked!!
```

---
## \#10 Posted by: scepterr Posted at: 2017-08-24T20:43:24.722Z Reads: 168

```
Next time bottle the spark :grin:
```

---
## \#11 Posted by: Hummie Posted at: 2017-08-24T20:55:28.470Z Reads: 160

```
was it just a big voltage difference with the two paralled packs or maybe two balance leads were connected and you completed a circuit with the leads connecting?  that's a big black spot
```

---
## \#12 Posted by: flywithgriff Posted at: 2017-08-24T22:23:27.609Z Reads: 149

```
The balance leads for the two packs are connected in parallel.
```

---
## \#13 Posted by: Hummie Posted at: 2017-08-24T22:59:34.151Z Reads: 140

```
yea I was thinking you could possibly put the balance leads in the wrong parallel order and not notice and then you'd be making a circuit with possible every cell in series when you put the mains in parallel.  

here's my guess about cells put in parallel and hope someone can correct me.   when two cells are put in parallel the voltage of the lower cell will instantly rise, and the higher cell instantly fall, the current will follow the voltage and balance as quickly as it can with only the pack resistance to decrease the possible amp flow.  The math would be the voltage difference between the packs divided by the resistance of both packs would give the current flow.  What would determine how long it would happen?
```

---
## \#14 Posted by: flywithgriff Posted at: 2017-08-24T23:40:52.861Z Reads: 124

```
I'm 99.9% sure all the balance wires are correct and I have already soldered the main negative leads in parallel. Will certainly be connecting the positive leads with a bit of reservation!
```

---
## \#15 Posted by: mmaner Posted at: 2017-08-25T00:15:07.979Z Reads: 121

```
I would suggest you double check the balance leads from 1 to 10 with a volt meter just to be sure.  Other than that, use an ct90s to connect the parallel packs. That's what I did anyways 😀.
```

---
## \#16 Posted by: Wilsonliang777 Posted at: 2017-08-25T01:24:39.984Z Reads: 111

```
I have this problem a lot. I end up soldiering balance lead and xt90 plugs all the time.  The xt90 positive and negative connectors often melts when I attempted to connect my batteries in parallel.  I end up resoldering it or have to disassemble the battery. That is why I am thinking of using a antispark xt90 plug on all my parallel cables  

What can I do to prevent my balance lead from spark and melting.
```

---
## \#17 Posted by: scepterr Posted at: 2017-08-25T01:37:14.810Z Reads: 103

```
Are the parallel packs at the same voltage?
 I've never encountered issues hooking up parallel packs,  always check that they are balanced. I combined 2 7S80P 18650 PowerWalls without a single spark. On a side note I have about 10Kwh of energy storage in a PowerWall made from salvaged 18650s 😁
```

---
## \#18 Posted by: flywithgriff Posted at: 2017-08-25T01:38:14.429Z Reads: 110

```
Balance leads are paired by order as well as color.really no way to get that part wrong. They are however not connected to the BMS. I will be placing a xt90 anti spark going into the vesc.
```

---
## \#19 Posted by: flywithgriff Posted at: 2017-08-25T01:41:21.278Z Reads: 106

```
These packs are 5x 2s 5ah 30c each. I have just connected them in parallel and have not had any additional sparks.
<img src="/uploads/db1493/original/3X/3/8/3879d432a1c3335c88cd696b66da79842b67ada4.jpg" width="666" height="500">
```

---
## \#20 Posted by: lowGuido Posted at: 2017-08-25T03:44:48.376Z Reads: 99

```
You are doing something wrong. This shouldn't happen.
Thats the spark of a short,  not just slightly different voltage in parallel cells.
```

---
## \#21 Posted by: flywithgriff Posted at: 2017-08-25T03:45:41.820Z Reads: 94

```
I have traced every wire as well as connections and everything is correct.
```

---
## \#22 Posted by: wafflejock Posted at: 2017-08-25T17:11:41.752Z Reads: 76

```
Seems like if the voltage is far enough off you could still have an inrush but it does seem like an excessively large spark, I was getting bad sparks (frying xt-90s) with hooking up a 12S to a VESC just from the inrush current into the capacitors, an antispark plug has completely eliminated the problem for me (also using 10S now).  In this case the antispark would also help to reduce the chance of dumping a large amount of energy from one battery to another since the resistor in the antispark will help to "regulate" the current flow (assuming it's not so high it burns up the resistor too, I have done that before and is really hard to pull out the antispark plug once the resistor inflates after frying, make sure it's fully inserted before you start drawing power through it).
```

---
## \#23 Posted by: trancejunkiexxl Posted at: 2017-08-25T17:23:44.370Z Reads: 70

```
 i can't wait to hear how you fixed it! =)
```

---
## \#24 Posted by: flywithgriff Posted at: 2017-08-25T18:14:25.144Z Reads: 64

```
It seems it fixed itself with a big ass spark. I haven't had any other problems so far. The packs are wired in parallel and the positive leads are connected to the vesc. As soon as my BMS shows up I'll connect the negative lead tonit and then to the vesc. I am however running an xt90 antispark going into the vesc.
```

---
## \#25 Posted by: Hummie Posted at: 2017-08-25T22:00:43.565Z Reads: 55

```
someone here was using anti-electric paste to stop the spark.  it woudnt reduce the current flow and protect the caps or your cells in paralllel but as the connectors come together the paste has higher resistance than air so no spark possible.  cheap-man's antispark.
```

---
## \#26 Posted by: lowGuido Posted at: 2017-08-26T04:05:54.988Z Reads: 44

```
spark size is directly proportional to voltage. its Paschen's law.
if a dead cell is 3.0V and a full cell is 4.2V thats a 1.2V MAXIMUM difference.

The spark in the photo was not a 1.2V spark.
just sayin.
```

---
## \#27 Posted by: flywithgriff Posted at: 2017-08-26T04:43:58.483Z Reads: 43

```
But 10s times 1.2v is a 12v spark. Not sure if the fact it's a 2p would make a difference. However, everything is wired together and soldered and I have had zero sparks.
```

---
## \#28 Posted by: wafflejock Posted at: 2017-08-26T06:25:52.248Z Reads: 42

```
https://en.wikipedia.org/wiki/Electric_arc
^^ believe it was this kind of thing that was happening to me and might have happened here.  It's not that we're getting to the thousands of volts needed to actually jump across the air along but once the connection is made and current has started to flow as the wires come apart (maybe they bounced a little as making the connection) and the current continues to flow across the air resulting in a bright hot spark but at relatively low voltage.
```

---
