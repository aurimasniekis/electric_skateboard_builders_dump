# 10S bestech bms without balance wires - weird behaviour

### Replies: 5 Views: 150

## \#1 Posted by: lesh Posted at: 2019-09-04T14:43:00.893Z Reads: 37

```
Hi, I'm in the middle of a build, 

using HCX-D223 10S-80A BMS
I didn't connect balance wires yet.. I'm trying to use it to charge the battery and as an e-switch only for now.

two questions,

1. during charging, it's main heat sink is getting very hot (about 70-80 degrees Celsius) - is this normal? 

2. it's e-switch is on, but output gives me some weird voltage, 28ish volts and falling as I'm measuring, as if I'm measuring a small capacitor. battery voltage is in the normal range, 38-ish volts

I'd expect balance wires to become relevant when battery is fully charged, but is the whole device behaving weird because balance wires are not connected?

tnx!
```

---
## \#2 Posted by: olestra Posted at: 2019-09-04T15:09:26.507Z Reads: 33

```
far as I know, that's a good way to destroy a BMS and possibly your batteries -- you don't charge a li-ion or li-poly pack without balancing.
```

---
## \#3 Posted by: lesh Posted at: 2019-09-04T15:12:00.902Z Reads: 30

```
that's not correct, especially short term (I'm in a middle of the build) and if not maximally charging and discharging

https://www.electric-skateboard.builders/t/li-ion-battery-pack-without-bms/47818/6
```

---
## \#4 Posted by: olestra Posted at: 2019-09-04T15:15:24.585Z Reads: 34

```
okay -- I'll agree that one can treat the batteries like that and get away with it.

what about the BMS? I don't think they would do well, dumping the current through without the leads attached. 
the BMS would be thinking all the cells are at 0
```

---
## \#5 Posted by: lesh Posted at: 2019-09-04T19:52:47.586Z Reads: 21

```
Just to answer and close this,

everything is ok after balance wires are connected, which, in retrospect is kinda expectable given + line never goes to the BMS otherwise :D 

Main heatsink does get hot still, I suppose it's controlling the voltage through resistance, so that's expected I guess.


(for wiring reference)

https://www.electric-skateboard.builders/t/bestech-hcx-d596-the-new-80a-bms-wiring/41047/14?u=lesh
```

---
