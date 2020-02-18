# Hypothetical: 2 packs in parallel with different capacity?

### Replies: 7 Views: 191

## \#1 Posted by: accrobrandon Posted at: 2018-11-30T03:32:09.072Z Reads: 87

```
so i was thinking about this but didnt know what the actual end result would be... so,.

lets say I have 2 separate packs both with its own BMS. Lets say one is 10ah and the other is 15ah

now i know for a fact you can link multiple packs in parallel (with same capacity) each with its own bms.... and charge all packs off the one input port (assuming the battery shares the same charge/discharge), as Ive been doing it with my ebike with those 2p ebay packs...

so heres the thought...lets say I want to go on some long ass ride (with pnumeis) and I have the 10ah and 15ah paralleled. 
I assume once the 10ah gets depleted first (which it would) the bms hits LVC and shuts the pack off. 

Does the other pack keep working?
Does the vesc recognize some sort of LVC from the BMS and refuse to work? Similar to if you were charging packs in parallel that werent charged from the same starting point...the first one to hit full capacity will trigger the charger to stop charging...

I was assuming the first pack cuts out and the board dies over all, then you could unplug the dead battery.. and the 15ah will continue to work with what ever juice is left. Dont worry about the actual logistics of getting the wiring to be easily accessible.

thoughts?
```

---
## \#2 Posted by: thisguyhere Posted at: 2018-11-30T03:43:16.813Z Reads: 79

```
As long as the two packs are the same voltage in terms of series count and also charge voltage, it will work. 

I have a small board with a 12s2p. Last ride i paralleled an "extended" 12s4p pack in parallel, effectively making a 12s6p pack. At 7ah per mile, i could have gone almost 100 miles on that setup. 

When joining the two packs tho make sure voltage is no more than 0.1v in difference.
```

---
## \#3 Posted by: thisguyhere Posted at: 2018-11-30T03:44:13.422Z Reads: 75

```
[quote="accrobrandon, post:1, topic:76575"]
assume once the 10ah gets depleted first
[/quote]

Nope, they'll drain simultaneously.
```

---
## \#4 Posted by: iTzDiego Posted at: 2018-11-30T03:45:27.767Z Reads: 73

```
can you expand on this?

[quote="thisguyhere, post:3, topic:76575"]
> assume once the 10ah gets depleted first

Nope, they’ll drain simultaneously.
[/quote]
```

---
## \#5 Posted by: accrobrandon Posted at: 2018-11-30T03:45:59.732Z Reads: 64

```
this i get, yeah theyll drain at the same time, but since one has more actual capacity the smaller one has to bottom out first...and then what happens? ....

ok ok.. maybe i forgot a point... lets say... on pack uses cells that are 3000mah and the other is 2200mah...
```

---
## \#6 Posted by: thisguyhere Posted at: 2018-11-30T03:47:35.517Z Reads: 63

```
The larger capacity will effectively charge the smaller one, the two packs in parallel will continue to balance each other.

Heres mine with the extended pack

![1129181946a|690x388](upload://jLDq3TNEZLYPhBKO5TBNX4OlybD.jpeg)

At the end of day after about 25 miles, voltage for the two packs were identical.
```

---
## \#7 Posted by: accrobrandon Posted at: 2018-11-30T04:01:46.472Z Reads: 57

```
lol i recognize that deck...looks like my blank deck!
```

---
