# Parallel LiPo discharge with balance ports connected

### Replies: 5 Views: 1251

## \#1 Posted by: kovjanos Posted at: 2016-06-09T15:33:18.510Z Reads: 100

```
Hi,

I checked some diagrams and custom builds based on pre-built (xS1P) LiPo blocks with parallel connected blocks and found out that for the discharge configuration (e.g. when you ride your board) the balance ports are not connected.

I would like to charge multiple blocks the same time using a balance-board. For this the cells in the same position (within a xS1P) must be on the same charge level (+- 0.1 V if I remember correctly) otherwise the cells would start to balance each other generating quite high current over those thin wires and through the board.
If I charge the blocks one-by-one to the same level first, then I can connect them parallel through the balance charge board and continue charging them together.
If all fully charged they go back to power up the board. 


What about to keep the balancing ports connected while discharging them?


1. First of all the right ports must be connected to make sure the same cells get parallel what the balance charge board would make parallel
2. **_This is the goal:_** that way while discharging, the cells in the same position would be discharged to the same level, which would eliminate the extra preparation step while charging (e.g. to get the cells close to each other) to be able to parallel connect the blocks on the balance charge board.


Would it work? Is it feasible? Did I miss something that would burn my legs down?


Is it true that there is only minimal stress (current) over those balance charge ports between the parallel cells?


Many thanks, J.
```

---
## \#2 Posted by: Hummie Posted at: 2016-06-09T15:36:26.588Z Reads: 89

```
Ud be doing a series and parallel connection and shorting if u leave the balance wires connected to each other and discharge
```

---
## \#3 Posted by: kovjanos Posted at: 2016-06-09T16:03:54.446Z Reads: 78

```

Why would this make shorting? Could you please elaborate?

Probably I wasn't clear enough... try to imagine this configuration:
- you have 2 pieces of  2S  blocks (2S1P) 
- you connect them parallel (e.g. you have enough voltage but you opt for higher current / C-rate)
- in this case you already connected the same ends of the two blocks together: ++ and -- .
- if you discharge this configuration each of the blocks will be on the same total voltage, let's say 3.4 V, but the cells inside the blocks could have different charge levels, e.g.: 
   o first block:  3.5V - 3.3V
   o second block: 3.3V - 3.5V
- you would have +- 0.2V differences between the cells on the same positions. 
(- if you would try to connect them to a balance charger board it could burn the connector pin with the spark that made for balancing the cells between the two blocks)


So change the configuration to the following:
- first of all, connect the same ends together: ++ and --
- that way you have the same configuration like before
- second step is to connect the balancing ports together. Balancing ports have 3 pins: the + and - ends and the middle connection from between the two cells from the 2S block.
- The ++ and the -- are already connected, so connecting the balancing ports would add only one more: connecting the two middle cells together. 

What the extra connection makes? 
- I think it will not short anything as this is the same as how custom LiOn packs are wired
- it will let the cells in the same position discharged to the same level. If both blocks are discharged to 3.4V (forced as they are parallel), the cells in the same position would be also on the same level, e.g.: 
   o first block:  3.5V - 3.3V
   o second block: 3.5V - 3.3V

Why is it good? 
- For charging I can connect the two blocks to the balance charge board immediately, without the need of pre-balancing and without any worry about the sparks.

Hope I cleared the picture a bit, but let me know if it's still confusing.

Many thanks, J.
```

---
## \#4 Posted by: Hummie Posted at: 2016-06-09T16:37:15.287Z Reads: 66

```
  If ur putting cells in parallel for discharging and also keeping the same parallel connections for charging that's fine.  Maybe hats what ur writing.  But if u are discharging in series and keeping the parallel connections then a short.  I think u mean the first option.
u could keep the parallel connections of the balance wires permanently (for the inner cell) as long as ur charging in parallel and discharging in parallel
```

---
## \#5 Posted by: kovjanos Posted at: 2016-06-09T16:44:07.619Z Reads: 62

```
Yes, that's the proper term: "keeping the same parallel connection for charging and discharging".

Thanks, J.
```

---
