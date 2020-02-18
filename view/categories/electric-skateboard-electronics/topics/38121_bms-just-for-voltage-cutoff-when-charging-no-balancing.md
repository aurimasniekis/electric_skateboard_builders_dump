# BMS just for voltage cutoff when charging? No Balancing

### Replies: 7 Views: 726

## \#1 Posted by: michaelcpg Posted at: 2017-11-12T20:46:44.378Z Reads: 55

```
Does anyone know of a really simple 10S BMS that's only purpose is to cut the circuit from a simple laptop brick style charger when the battery reaches 42V? 

I.e I don't want it to do balancing of any kind as this adds a lot of extra wiring to my build that I don't really think I need as my battery is made out of 10 separate, easily removable 1S6P 18650 packs so I can balance them separately when necessary.

Cheers
```

---
## \#2 Posted by: aigenic Posted at: 2017-11-12T21:58:34.026Z Reads: 50

```
I dont think you even need BMS for this, but I might be wrong :) Not an engineer...
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-11-12T22:02:15.356Z Reads: 48

```
for that u dont need bms. open up the charger see if u can dial the voltage to set 42v exactly. than just plug in
```

---
## \#4 Posted by: michaelcpg Posted at: 2017-11-12T22:06:01.446Z Reads: 44

```
Do standard "dumb" chargers like this one actually cut off the voltage when the battery reaches 42V? 

https://www.ebay.com/itm/36-Volt-Battery-Charger-Golf-Cart-36V-Charger-For-Ez-Go-Club-Car-DS-EZgo-TX-A-/291963127502

I had just assumed you still needed some form of BMS to cut the circuit when the battery reaches a specific voltage unless you use something like a hobby balance charger?
```

---
## \#5 Posted by: aigenic Posted at: 2017-11-12T22:09:11.506Z Reads: 39

```
I think this one cuts off when the battery reaches 36V...
```

---
## \#6 Posted by: aigenic Posted at: 2017-11-12T22:12:49.027Z Reads: 38

```
When you are using BMS with brick charger, the charger limits the voltage and the BMS balances all the cells to be equal, tahts how I understand that :) There are also some protection circuits in the BMS limiting the max voltage :slight_smile: which can be a problem when you are regen braking on a full battery
```

---
## \#7 Posted by: b264 Posted at: 2017-11-12T22:13:05.921Z Reads: 38

```
Sounds like you don't need a BMS at all.  If the charger is at 42V, once the battery reaches 42V it will stop drawing current and basically stop charging.  The (end-to-end) battery voltage will never go above the charger voltage.  HOWEVER if any of your cells or P packs are weak, then the other cells/p-packs will overcharge to compensate for it, that's what the balancing prevents

edit: When I say "weak" I don't even necessarily mean weak, just relatively slightly **weaker** than the other ones.  So in effect there is some self-balancing action happening because once one gets a little weaker it will overcharge the others and once they get slightly damaged and take less of a charge, they will be back in balance again.  A bms just does this balancing without damaging anything.
```

---
