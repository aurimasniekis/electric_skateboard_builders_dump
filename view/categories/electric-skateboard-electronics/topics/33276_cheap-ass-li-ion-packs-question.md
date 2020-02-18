# Cheap ass Li-ion packs question

### Replies: 6 Views: 555

## \#1 Posted by: Eric Posted at: 2017-09-16T18:26:14.016Z Reads: 107

```
So I'm sure most of you have heard of these: http://www.ebay.com/itm/5-LG-36V-4-4AH-BATTERY-PACK-18650-EBIKE-VAPE-POWERWALL-BATTERIES-100-CELLS-BMS-/172660442407?hash=item28335d4527:g:nKUAAOSwuspY9YNZ 
They are extremely cheap, and I currently use 3 LiPo packs in series on my board, but was wondering if I could upgrade to these.  
My first question is, if I were to take all 5 packs of 10s2p, and wire those in parallel, but keeping the bms's on the 5 individual packs, is this do-able?  So essentially I'd end up with a 10s10p. (I probably won't do all 5, maybe 4, but no less than 3)
I don't have a way to draw it out, but I imagine laying them out in a 2x2 configuration on the bottom of my deck (using just 4 as an example), then take the all the positive leads, wire those together, same with the negatives, and run them through probably a vedder switch, or xt90s and to my vesc.  
I don't have a spot welder or anything to make my own pack out of these, but would all the bms's behave themselves if I then attached the charging port between all the packs wired in parallel and the on/off switch that is included with this charger: http://www.batterysupports.com/36v-42v-5a-lithium-ion-battery-charger-10s-10x-36v-lion-lipo-p-166.html 
I feel like this would be a fantastic option not caring about weight, but wanting the distance. Let me know where my idea is flawed. Thanks
```

---
## \#2 Posted by: P.Martin Posted at: 2017-09-16T19:24:16.284Z Reads: 84

```
This would work fine, the bms on each pack would just shut down as battery is lost in each pack until you are at empty, then you just have to plug them in again. My friend ha done this on a electric bike, and it works perfectly, hes getting 25+ miles with 4 packs in parallel, imagine what you'd be getting with a light long board. you would probably have to lengthen the wire though.
```

---
## \#3 Posted by: wafflejock Posted at: 2017-09-16T19:25:49.375Z Reads: 79

```
Trying to poke holes in this but don't take it personally :)  If you have the cells hooked in parallel to each other you are basically going to end up dumping charge from one of the packs into the other if their voltage is different.  So when you initially hook them up you'll want to be sure they have the same charge basically so you don't end up fast charging any cells for too long and end up damaging them.

This brings up an issue too though with the separate BMSes managing the cells separately, if one is putting power into a pack quicker than the others then it will end up balancing across the other packs that are hooked in parallel... is this bad? Probably not you're sort of giving the battery a way to distribute the charge going into it but the charge going from one parallel pack to another will be going from one set of cells to another set of cells in series so it's not like every cell will be balanced perfectly with charge flowing through the parallel connections (not the balance leads), but can't think of any catastrophic scenarios here.
```

---
## \#4 Posted by: P.Martin Posted at: 2017-09-16T19:33:09.815Z Reads: 65

```
Even if one pack is putting out more current than another, the bms will prevent over discharged cells, but I can see the concern of them sort of charging each other, but i think that the bms will prevent any damage from occurring.
```

---
## \#5 Posted by: Eric Posted at: 2017-09-16T23:55:33.264Z Reads: 53

```
Ok, if I end up doing this switch, I'm wondering how it will affect my performance. Currently I have a 12s setup, and downgrading it would decrease the speed (so I've heard). But also I'm told I can raise the max Amps on my VESC, I currently have it at 40a. But lowering the voltage my calculations say I can almost double the amperage.  <img src="/uploads/db1493/original/3X/b/9/b9219a7c7006b0490eed52ce636aec29355ea80d.png" width="281" height="500"> I don't think my VESC can handle this much, so I think I'd limit it to 60a. What changes when I increase the amperage?
```

---
## \#6 Posted by: Chewie Posted at: 2017-09-17T04:56:32.554Z Reads: 34

```
I'm running 3 of these in parallel.  With a 196kv motor, 13:36 gearing and 90mm wheels. App says I'm good for 25 miles averaging 15-20mph, seems pretty accurate.
```

---
