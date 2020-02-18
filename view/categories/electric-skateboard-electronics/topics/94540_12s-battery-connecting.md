# 12s battery connecting

### Replies: 7 Views: 208

## \#1 Posted by: pshclover Posted at: 2019-05-21T15:39:50.534Z Reads: 58

```
if I were to connect two 6s4p batteries with a bms inside both of them, would I need a bms for the newly connected 12s4p battery?
```

---
## \#2 Posted by: pshclover Posted at: 2019-05-21T15:43:33.183Z Reads: 57

```
and on youtube, people only connect lipo batteries together, could I connect two lithium ion battery packs together?
```

---
## \#3 Posted by: ZachTetra Posted at: 2019-05-21T15:56:44.556Z Reads: 45

```
Each half would use its own BMS, no third BMS needed.  But you have to note YOU CAN ONLY CHARGE ONE AT A TIME, if you charge both from a similar power source, they will short out across the charger input and kill everything.  If you have 2 independent power sources (different ac networks then you can)
```

---
## \#4 Posted by: Wilsonliang777 Posted at: 2019-05-21T15:59:06.243Z Reads: 44

```
No.   You don't need a bms if the liion packs has bms inside. Lipo and li ion both should have a bms
```

---
## \#5 Posted by: Wilsonliang777 Posted at: 2019-05-21T16:07:04.620Z Reads: 42

```
It might be better to disconnect the 6s bms and merge the batteries to a 12s and connect it to a 12s bms.   But we run into the problem of new cells and old cells and are the cells all the  same kind problem.
```

---
## \#6 Posted by: pshclover Posted at: 2019-05-21T16:16:02.874Z Reads: 39

```
could I use a charge balancer to charge both at one time
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-05-21T16:32:46.842Z Reads: 33

```
Not while they are in series.  If you separate the packs to charge then its totally fine, nothing unusual will happen since it would be 2 completely separate batteries.  If you want to charge both while they are connected, then you need 2 isolated power sources or the negative lead will be connected at 2 points in the battery and short out.

I think you can take a 12s power source and wire 2 '6s' charge ports in series for the output instead of a single 12s charge port, but any imbalance would cause one pack to have more resistance and the other pack would have to much voltage.

Best bet is to use a 12s BMS or separate the packs completely.  For separate batteries you can use a balance charger (2 individual or 1 dual)  or 2 BMSs with either a shared (parallel) 6s voltage source or just separate chargers
```

---
