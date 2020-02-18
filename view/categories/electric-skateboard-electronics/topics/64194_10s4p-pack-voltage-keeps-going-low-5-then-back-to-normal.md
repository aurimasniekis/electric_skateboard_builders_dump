# 10S4P pack voltage keeps going low (&lt;5%) then back to normal

### Replies: 20 Views: 385

## \#1 Posted by: lilracerboi Posted at: 2018-08-08T01:55:42.510Z Reads: 149

```
I went on a small ride yesterday and at some point not long after I left, the board stopped responding. I checked the battery meter and it reported very low, like sub 5% low. Now the weird part is after letting it sit for a few seconds it would rise back to 80-something%. I did fully charge it before leaving too. So now, I have the same issue with the pack going super low after throttling. There are some cases where I would have to throttle a bit so the voltage goes back up. I can actually see the percentage go down then back up. I checked each cell with a multimeter and found one cell is super low versus the rest of the cells (3.6V vs 4.13). I don't know if that has anything to do with the issues I'm having, but it'll need to be fixed anyways before causing other issues.

TLDR: 10S4P pack voltage keeps going super low (<5%) then back to normal. Also, one cell is low (3.6V vs. 4.13V).

@barajabali Because I don't know of anyone else specifically who works with batteries and you repaired my battery (granted it was a while back), I figured I'd get your input. Also note, the range seems very poor. Not sure what it is, but it doesn't feel like it lasts very long, even with modest throttling.
```

---
## \#2 Posted by: never4getf150forums Posted at: 2018-08-08T02:10:54.214Z Reads: 136

```
unbalanced cell affects the entire pack, you need to bring that cell that's 3.6v up to 4.13 or just replace it entirely.
```

---
## \#3 Posted by: lilracerboi Posted at: 2018-08-08T02:16:56.114Z Reads: 135

```
Can I charge cells separately? I don't have the tools to put it back together if I separate them.
```

---
## \#4 Posted by: b264 Posted at: 2018-08-08T02:21:22.137Z Reads: 131

```
Connect the cell to another cell in parallel *through an incandescent car light bulb* and let it sit for a few days to manually balance them together
```

---
## \#5 Posted by: lilracerboi Posted at: 2018-08-08T03:49:28.607Z Reads: 118

```
Is it possible to connect that cell to my hobby charger via the balance cable and set it to 1S charging?

@b264 I'm not sure how that wiring works. Are you assuming the cell is disassembled from the entire pack already?
```

---
## \#6 Posted by: b264 Posted at: 2018-08-08T04:14:46.467Z Reads: 106

```
Yes, but if you have a hobby charger then you won't ever need to do what I suggested.
```

---
## \#7 Posted by: pat.speed Posted at: 2018-08-08T07:12:36.456Z Reads: 93

```
Connect the the cells balance lead holes directly to the hobby charger and select 1s, it should charge up fine. You will need the right type of connector though to connect them
```

---
## \#8 Posted by: lilracerboi Posted at: 2018-08-08T07:32:17.473Z Reads: 88

```
I'm doing that right now. I just soldered a couple jumper cables to an XT-60 connector. Worked fine. Been on there for 2 hours charging at 1A.
```

---
## \#9 Posted by: pat.speed Posted at: 2018-08-08T07:38:52.514Z Reads: 87

```
Sounds good, take it off when it’s close to the other cells
```

---
## \#10 Posted by: lilracerboi Posted at: 2018-08-08T22:09:22.598Z Reads: 70

```
Everything seems to be good now. I had to leave it charging for up to 6 hours. Once it hit 4.2V it switched to constant voltage and the current began slowly dropping from 1A.
```

---
## \#11 Posted by: pat.speed Posted at: 2018-08-08T22:15:10.078Z Reads: 67

```
okay, you shouldn't have charged it that high though because now the other cells are out of balance
```

---
## \#12 Posted by: lilracerboi Posted at: 2018-08-08T22:34:35.852Z Reads: 64

```
Well the cells were in pretty bad shape. They're balanced now. When I first put it on the charger the voltage would go up towards 4.2V, but as soon as I took it off it would drop down to 3.6V (the starting voltage). Over time I would take it off the charger to check it and it would start reporting higher voltages.
In the end, I brought it up to the other cells, took it for a short test ride down the street doing full throttles and checked all the cells again. All balanced. Then I put it on the charger and checked the cells again after it was done.
```

---
## \#13 Posted by: pat.speed Posted at: 2018-08-09T05:49:34.526Z Reads: 57

```
Ok, for the next couple rides I would suggest monitoring that cell very closely. If it still happens to lose charge quicker than the others I would send it to someone like @barajabali to have it fixed or rebuilt
```

---
## \#14 Posted by: lilracerboi Posted at: 2018-08-09T08:38:27.373Z Reads: 52

```
Yeah, that's what I was planning on doing. It'll mostly be used on campus for a while since my next semester is packed.
```

---
## \#15 Posted by: lilracerboi Posted at: 2018-08-27T16:32:59.832Z Reads: 39

```
The problem with the voltage dropping to zero on a full charge is back. The cells are still fine as a full charge reports 100% instead of ~94%.

I just thought of it, but could the power switch be causing the problems? I'm using an old Vedder's anti-sparking switch I got a long time ago.
```

---
## \#16 Posted by: taz Posted at: 2018-08-27T16:34:50.675Z Reads: 39

```
I would check the pack's series connections.
You may have a few broken ones.
```

---
## \#17 Posted by: lilracerboi Posted at: 2018-08-27T16:43:03.781Z Reads: 37

```
Alright, I'll check it when I go home.
```

---
## \#18 Posted by: lilracerboi Posted at: 2018-08-27T18:21:09.938Z Reads: 33

```
Yeah it was none of those issues. The real culprit was the fuse. It was physically damaged. I could hear electrical noises coming from it when the power is on. The receptacle was also slightly damaged. Looks like one of the terminals melted a bit of plastic and it slid towards the other terminal. Popped in another fuse to see if I get the same problems and I do not, but I'll still replace the receptacle.

Does anyone else use a fuse? Is it necessary? The VESC can limit the current draw from the battery right?
```

---
## \#19 Posted by: TowerCrisis Posted at: 2018-08-27T20:34:56.363Z Reads: 23

```
The vesc can limit current draw during normal operation, but it cannot protect from physical damage to phase wires / battery wires / the vesc itself. That's what a fuse is good for. What kind of fuse are you using?
```

---
## \#20 Posted by: lilracerboi Posted at: 2018-08-27T23:05:57.025Z Reads: 16

```
Yeah, someone at my university explained that to me when I opened up my board (fixed it in the electronics lab).
I've got an automotive bladed fuse. 40A. That's what Enertion used in their packs back when they sold parts.
```

---
