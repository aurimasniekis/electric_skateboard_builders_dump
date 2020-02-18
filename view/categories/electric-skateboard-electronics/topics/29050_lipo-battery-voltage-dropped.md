# Lipo battery voltage dropped

### Replies: 5 Views: 345

## \#1 Posted by: mattdig Posted at: 2017-07-29T17:02:39.918Z Reads: 55

```
I was riding for a while yesterday, and suddenly Cell-1 (furthest on the Negative side) on my 8 cell Lipo pack went from about 3.6V to 2.5V (I have a constant readout for each cell on my deck where I can see it). Luckily I was close to my destination so I stopped riding. I put it on a charger for about 30 minutes and then all cells, including the 1 that read 2.5, were up to about 3.7. I know my voltage monitor was working fine, because I re-tested the pack with another volt meter and it was around 2.5 on that cell. I still don't understand how the voltage on 1 cell dropped so fast, or why it went back up to normal after just 30 min of charging. It's a new-ish pack (3 months of riding) so could the cell be dead or is this just a weird glitch? I have not ridden the board yet, I've got the whole pack on a very slow charge right now.
```

---
## \#2 Posted by: evoheyax Posted at: 2017-07-29T17:12:08.571Z Reads: 52

```
You get to about 3.5 ish, lipos drop off a cliff. You should never let your cells get below 3.2.

I have abused many lipos like this, and they usually are fine if it's not for long and you quickly get it back up above 3.2.

Discharge curve is not linear. You go from 4.2 to 4 very quickly (1 minute or less of riding in many cases), 4 to 3.6 is a steady, linear like discharge, followed by a quick drop off from 3.5/3.6 to 3.2.
```

---
## \#3 Posted by: mattdig Posted at: 2017-07-29T17:58:39.897Z Reads: 46

```
I'll definitely be more careful from now on, I just hope I haven't ruined that 1 cell, and then have to replace the whole pack.
```

---
## \#4 Posted by: MannyM0E Posted at: 2018-01-29T20:53:41.647Z Reads: 25

```
How can you pervent your cells to not get below 3.2V because I'm in the same situation.
Is it on the vesc setting ? Cutoff time I'm assuming but I set it up to 9s & applied whatever the recommendation was
```

---
## \#5 Posted by: louwii Posted at: 2018-01-30T01:46:50.253Z Reads: 16

```
Your cut-off end should be set at 9 x 3.3V = 29.7V
I would recommend even more than that to be safe, like 3.4 or 3.5
```

---
