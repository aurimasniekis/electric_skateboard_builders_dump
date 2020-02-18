# Building a battery pack for the Inboard M1 (

### Replies: 11 Views: 317

## \#1 Posted by: justice91423 Posted at: 2019-08-05T05:27:04.935Z Reads: 48

```
I recently got an Inboard M1 and I'm hoping to build better battery packs to replace the PowerShift battery packs it normally uses.

I'm pretty good at 3D modeling and printing, so the case shouldn't be a problem.  But while I'm decently knowledgeable about electronics and am good with a soldering iron, battery packs are a new area for me.

I opened up one of the PowerShift battery packs I got with the board and found the following

The cells they use are LG HE4 18650 2500mAh 20A.

The BMS is a PCM-L13S15-876(A). However that BMS is a 13s, and the PowerShift only has 12 cells. Also, one of the MOSFETs was missing from the BMS. I'll attach an image to show which one was missing.

I’m still learning about battery packs, but it seems like making one with some Samsung 40T 21700 4000mAh 30A would be a pretty significant upgrade.

If anyone has knowledge or experience they are willing to share (Especially about how that BMS is set up), I’d LOVE to hear it.

And if anyone wants to partner up on this project, it would be great to share the workload and do this in bulk.

![s-l1600|615x500](upload://d2y8x6NOO7dLjjDQ4dzsrtIBNEv.jpeg)
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-08-05T06:11:30.871Z Reads: 41

```
Don't add a bms to the pack there won't be enough space, just add 2 6s balance leads to the pack.
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-08-05T06:12:00.018Z Reads: 42

```
[quote="justice91423, post:1, topic:99728"]
Also, one of the MOSFETs was missing from the BMS
[/quote]

That's fine.

Their are multiple versions of your bms and the amount of mosfets depend on the bms's charge/ discharge rate
```

---
## \#4 Posted by: justice91423 Posted at: 2019-08-05T06:41:19.619Z Reads: 39

```
[quote="AlanZhou, post:2, topic:99728, full:true"]
Don’t add a bms to the pack there won’t be enough space, just add 2 6s balance leads to the pack
[/quote]

I haven't measured it out, but since I'll be making a custom case I think I'll have enough room.  I may even go with the same size cells in the end.

I want to use a BMS primarily for the over discharge protection. (Feel free to correct me if that's not a legitimate concern)

If I were to go with the 2 6s balance leads, then I would need to use balance changer.  Correct? (Not that I'm against that)
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-08-05T06:42:50.183Z Reads: 34

```
Just saying the bms won't fit in the cavity along with 12 cells

Yeah using a balance charger.

I don't think over discharge is a issue as the esc had a preprogrammed voltage I think

Fun fact: The inboard esc runs on DRV 8301
```

---
## \#6 Posted by: justice91423 Posted at: 2019-08-05T06:44:04.855Z Reads: 37

```
[quote="AlanZhou, post:3, topic:99728"]
> Also, one of the MOSFETs was missing from the BMS

That’s fine.

Their are multiple versions of your bms and the amount of mosfets depend on the bms’s charge/ discharge rate
[/quote]

Okay.  Good info.  Thanks!  I wonder how I'll track down the exact one.  The model number matched up exactl.
```

---
## \#7 Posted by: justice91423 Posted at: 2019-08-05T06:50:36.823Z Reads: 35

```
[quote="AlanZhou, post:5, topic:99728, full:true"]
Just saying the bms won’t fit in the cavity along with 12 cells
[/quote]

The original packs have 12 cells and the BMS, so it's certainly doable.  But if It's better to go with out it, I'm all for it.  Easier and cheaper.

[quote="AlanZhou, post:5, topic:99728, full:true"]
I don’t think over discharge is a issue as the esc had a preprogrammed voltage I think
[/quote]

So the board itself will cut off before I over discharge the batteries?
If so, I imagine there is still a risk of a single cell discharging faster than the others and getting over discharged.  My uneducated guess is that's probably an acceptable risk.  Would you agree?

[quote="AlanZhou, post:5, topic:99728, full:true"]
Fun fact: The inboard esc runs on DRV 8301
[/quote]

I'll have to look up what that means, to get the "fun" out of that fact.  ha ha
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-08-05T07:04:13.257Z Reads: 29

```
[quote="justice91423, post:7, topic:99728"]
If so, I imagine there is still a risk of a single cell discharging faster than the others and getting over discharged. My uneducated guess is that’s probably an acceptable risk. Would you agree?
[/quote]

Nope that won't happen.

Most of us here actually bypass the bms for discharge all together.
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-08-05T07:06:36.144Z Reads: 30

```
[quote="justice91423, post:7, topic:99728"]
So the board itself will cut off before I over discharge the batteries? I
[/quote]

Yeah that's how I think it works for inboard but I may be wrong
```

---
## \#10 Posted by: justice91423 Posted at: 2019-08-05T07:23:22.326Z Reads: 28

```
[quote="AlanZhou, post:8, topic:99728"]
> If so, I imagine there is still a risk of a single cell discharging faster than the others and getting over discharged. My uneducated guess is that’s probably an acceptable risk. Would you agree?

Nope that won’t happen.

Most of us here actually bypass the bms for discharge all together.
[/quote]


Awesome!  Man, I really appreciate all this info.

So can I ask you, does what I posted above sound like the right call to you?  Going with 12 Samsung 40T 21700 4000mAh 30As?
```

---
## \#11 Posted by: selfmadevisionz Posted at: 2020-01-20T20:58:34.625Z Reads: 8

```
Did you ever make this batter pack for the Inboard M1. I'm quite interested in purchasing a battery back that will work for this unit.....
```

---
