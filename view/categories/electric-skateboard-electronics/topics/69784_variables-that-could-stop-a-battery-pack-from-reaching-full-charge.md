# Variables that could stop a battery pack from reaching full charge

### Replies: 15 Views: 167

## \#1 Posted by: Jcullinan09 Posted at: 2018-10-01T21:50:53.793Z Reads: 65

```
Hi guys,

Here are my parts for a 10S5P that will not charge past 39.5 volts. 

Batteries: Samsung 30Q (50x)
Bestech BMS: https://buildkitboards.com/collections/batteries/products/bestech-bms?variant=7201537687582
Charge plug: https://www.amazon.com/gp/product/B072BXB2Y8/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1
Battery Meter: https://www.amazon.com/gp/product/B01LQ7MT4K/ref=oh_aui_detailpage_o04_s00?ie=UTF8&psc=1
Anti-Spark: https://www.amazon.com/gp/product/B07CMYPZ6Z/ref=oh_aui_detailpage_o04_s00?ie=UTF8&psc=1
VESC's : FocBox.

So I recently made a 10s5p Pack, and now it will not charge past 39.5 volts.
I have checked the voltage at every single one of the 50 cells, and every cell reads 3.95 volts exactly.

I've done some reading, and found that the reason the charger might quit, is because one cell group might read 4.2 volts across, so the charger will shut off. However, none of my groups are at 4.2 volts, They are all at 3.95.

I am at a loss for what could be preventing the pack from reaching a higher voltage...

![IMG_1382](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/1/a/1a53b2b51d4144d6427f2573e362ca8d43498d1c_1_666x500.jpeg)
```

---
## \#2 Posted by: pat.speed Posted at: 2018-10-01T21:52:05.207Z Reads: 60

```
Have you checked the output voltage of your charger?
```

---
## \#3 Posted by: Jcullinan09 Posted at: 2018-10-01T21:52:44.776Z Reads: 62

```
Yes, I have a 2Amp and 4Amp charger, both of which read 42.5 volts, and 41.9 volts respectively.
```

---
## \#4 Posted by: pat.speed Posted at: 2018-10-01T21:57:27.986Z Reads: 60

```
Has there been any damage like shorting or over discharge to the pack. I know this same thing happened to my shorted lipos once
```

---
## \#5 Posted by: Jcullinan09 Posted at: 2018-10-01T21:59:20.381Z Reads: 57

```
I mean I did go for a really long ride, to completely discharge the pack. I brought the whole pack down to 31 volts, and then got home, and right away brought it back up to 42 volts. However the next day (yesterday) It suddenly will not charge past 85% or 39.5 volts.

Isn't that weird?!
```

---
## \#6 Posted by: pat.speed Posted at: 2018-10-01T22:00:37.225Z Reads: 54

```
Hmm this seems a bit sus, 31v is fine for Li-ion. The cells are legit right?
```

---
## \#7 Posted by: bigben Posted at: 2018-10-01T22:02:06.814Z Reads: 55

```
Could it be the BMS causing this?
```

---
## \#8 Posted by: Battosaii Posted at: 2018-10-01T22:02:20.487Z Reads: 54

```
If all the connections are good and the cells are already balanced it may be the BMS.

I would check all the spot welds to make sure nothing came undone.
```

---
## \#9 Posted by: Jcullinan09 Posted at: 2018-10-01T22:02:29.161Z Reads: 52

```
I got all of the batteries from https://www.imrbatteries.com/samsung-30q-18650-3000mah-15a-flat-top-battery/
and measured the voltage on every single one of them, when I bought them. All reading 3.43 volts each.
```

---
## \#10 Posted by: Battosaii Posted at: 2018-10-01T22:03:50.789Z Reads: 52

```
Did you ever short anything while installing the BMS? It's very easy to short something out when installing BMS it could happen to anyone and that would be enough to damage it.
```

---
## \#11 Posted by: Jcullinan09 Posted at: 2018-10-01T22:05:00.461Z Reads: 50

```
I don't think so, but ya know. Maybe I did somewhere along the line.
```

---
## \#12 Posted by: mmaner Posted at: 2018-10-01T22:40:58.227Z Reads: 49

```
I agree with @Battosaii, it sounds like an issue with one of the balance channels on the BMS which typically only happen when a channel cap has been burnt out.   

I would temp install a charge port on the packs main positive & negative and attempt to charge the pack to full.  If it gets pretty close to 4.2 per cell then turn off the charger and replace the BMS.  If it doesn't then your issue is somewhere else.
```

---
## \#13 Posted by: Jcullinan09 Posted at: 2018-10-01T22:53:45.384Z Reads: 48

```
When you say, "a channel cap has been burnt out." Is that referencing to the JST plug(male/female) or something directly soldered onto the PCB of the BMS?
```

---
## \#14 Posted by: mmaner Posted at: 2018-10-01T22:55:30.825Z Reads: 47

```
its a component on the BMS that hold the voltage and keeps it regulated for each balance lead connection.
```

---
## \#15 Posted by: rojitor Posted at: 2018-10-02T11:40:22.096Z Reads: 21

```
New cells sometimes refuse to take full charge.
Make a couple runs and refuel. Maybe they reach 4.2 then. If that fails it's the bms
```

---
