# Adding new 18650 cells to battery, best way to balance cells?

### Replies: 14 Views: 2375

## \#1 Posted by: michaelcpg Posted at: 2016-07-11T00:03:39.249Z Reads: 140

```
Hey guys, I'm in the process of upgrading my 10S3P Space Cell (which is currently in pieces) to a 10S4P battery. I've ordered another 10 cells so I'm wondering if you guys have any recommendations in regards to the best way to balance all the cells before adding the new 18650's to my pack? 

I've bought a single cell 18650 charger so I can charge each new cell separately to the same voltage that my space cell is currently sitting at (was planning to just keep an eye on each cell's voltage with my multi-meter as it's charging but I feel like this might get tedious after a while and would mean I'd constantly have to be monitor each cell as it charges so that I don't overcharge them) so I'm wondering if there's a more effective way of doing this?

I'm thinking maybe it's possible to wire the space cell's BMS up to all the old and new cells to balance them before I start building them into 10 packs of 4?

Cheers
```

---
## \#2 Posted by: laurnts Posted at: 2016-07-11T00:37:54.313Z Reads: 135

```
As I believe, if youre planning to upgrade from 10s3p to 10s4p you dont need to do anything at all besides adding the new batteries properly. That means positioning each of the 10 batteries individually to each 10 series packs. By doing this, the BMS will automatically balance charge and discharge the cells for you. But remember, its best to have them all with the same brand / type otherwise you might have problems.
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-07-11T00:48:21.302Z Reads: 130

```
Cheers for the reply. So to confirm, if I'm adding a new cell to each of my 10 current 3p packs, I shouldn't have to balance each new cell before adding it to the old 3 cells? I thought that adding a new cell to a parallel pack in this way when the new cells are initially charged to different voltages than the old cells would cause the cells to try to rapidly balance each other out.

Maybe I've misunderstood, is this then only an issue that occurs when connecting cells with different voltages in series as opposed to parallel?
```

---
## \#4 Posted by: lox897 Posted at: 2016-07-11T01:01:49.148Z Reads: 124

```
You should make sure all cells are at the same voltage before wiring them together. When I start making packs I am going to use my IMAX B6AC V2 with 2x 2 18650 sled so I can charge 4 cells at once, and then discharge them at once.
```

---
## \#5 Posted by: Stevemk14ebr Posted at: 2016-07-11T01:06:26.526Z Reads: 122

```
The 10 new cells you are buying must all be at the same voltage with each other, but can be a different voltage than the other 3 strings already in the space cell. Batteries in series with each other will not balance, batteries in paralell will balance.
```

---
## \#6 Posted by: lox897 Posted at: 2016-07-11T01:13:53.791Z Reads: 116

```
To be safe, I'd do it anyway. @Stevemk14ebr So, when you assemble a new pack, all cells have to be the same voltage? Why not when adding cells?
```

---
## \#7 Posted by: Stevemk14ebr Posted at: 2016-07-11T01:18:36.852Z Reads: 110

```
The bms can rebalance after you put them in parrallel. If im wrong feel free to correct me, its not uncommon for me to confuse myself.

To the op. I personally would just tape the volt meter leads on and check each cell every now and then. Individual cells wont take to long to charge and you mitigate any complications.
```

---
## \#8 Posted by: lox897 Posted at: 2016-07-11T01:20:14.698Z Reads: 105

```
When cells are at different voltage, other cells will rapidly try and balance each other out. This will result in high amps and could damage the cells. @whitepony @lowGuido @barajabali what do you think about this? I could be horribly wrong as well. I guess it is better to be safe than sorry.
```

---
## \#9 Posted by: laurnts Posted at: 2016-07-11T01:52:12.647Z Reads: 98

```
Ohh I have missunderstood abit. Yes you should balance charge all of them before the installation, just to be very safe.
```

---
## \#10 Posted by: cmatson Posted at: 2016-07-11T02:00:42.828Z Reads: 93

```
Ya, definitely balance the 10 cells so that they are close in voltage to the parallel groups of 3 on the space cell. 

Adding a 4v cell to a 3.3v parallel pack probably wouldn't work out very well.. Even with them all in parallel, the gap is huge, and the bms could easily overcharge that cell in the parallel group.
```

---
## \#11 Posted by: michaelcpg Posted at: 2016-07-11T02:10:48.096Z Reads: 90

```
Thanks for the info guys. Think I'll charge the cells beforehand then. How close do they ideally need to be? 

From memory, the old cells are currently sitting at 3.98V while the new ones are sitting at 3.64V
```

---
## \#12 Posted by: cmatson Posted at: 2016-07-11T02:30:51.549Z Reads: 86

```
Just get them around 3.9-4  if you can
```

---
## \#13 Posted by: lox897 Posted at: 2016-07-11T03:28:30.881Z Reads: 82

```
0.01 of a volt is ideal. Try and get them as close as possible.
```

---
## \#14 Posted by: chaka Posted at: 2016-07-11T04:25:31.189Z Reads: 79

```
Don't be too worried about getting cells perfectly matched before adding them to the pack. Within 0.2v is fine. Well within the amount a cell will drift when a charge of around 1C is applied.
```

---
