# 6s only charging to 24v

### Replies: 13 Views: 483

## \#1 Posted by: UltimaA380 Posted at: 2018-04-04T16:44:58.624Z Reads: 88

```
Hey guys,


so I have a board I built with a 6s6p setup and have a supowerbms and am charging it with a 25.2v adapter.


It only charges to about 4v a cell or 24v and the light turns green on the charger. Doesn't seem to charge more at all if I leave it plugged in.


Any ideas?
```

---
## \#2 Posted by: krloz Posted at: 2018-04-04T19:03:02.327Z Reads: 81

```
When you say

[quote="UltimaA380, post:1, topic:51226"]
charging it with a 25.2v adapter.
[/quote]

You sure about that?  Did you measure the charger voltage with a multimeter?
Can you also measure the voltage of each p pack to check they are all at 4v
```

---
## \#3 Posted by: UltimaA380 Posted at: 2018-04-04T19:27:12.011Z Reads: 74

```
I am positive, I checked individual cells, total pack voltage, and the voltage coming out of the charger (two actually, same issue)
```

---
## \#4 Posted by: myreala Posted at: 2018-04-04T19:48:12.271Z Reads: 69

```
Well Assuming you have healthy cells the problem looks to be in the BMS then. Have you tried switching out the BMS?
```

---
## \#5 Posted by: UltimaA380 Posted at: 2018-04-04T21:50:40.501Z Reads: 55

```
I do not have another one to switch it out with, so no.
```

---
## \#6 Posted by: pat.speed Posted at: 2018-04-04T21:54:14.878Z Reads: 51

```
With the chargers the voltage usually needs to be slightly higher then 25.2v when not under load. That way when load is connected the voltage can drop a little bit.

 I think that is what’s happening here have you tied just leaving it plugged in for a few hours
```

---
## \#7 Posted by: UltimaA380 Posted at: 2018-04-04T22:04:22.046Z Reads: 49

```
I can try.

The chargers are made for 6s li-ion and lipo batteries.


Also should note I have a SuPower BMS 6s 30A (am not using discharge function).
```

---
## \#8 Posted by: pat.speed Posted at: 2018-04-04T22:10:46.042Z Reads: 41

```
It will usually be quick to charge up to around 4v and then the rest will take a while because the voltage slowly drops off as the battery becomes charged
```

---
## \#9 Posted by: UltimaA380 Posted at: 2018-04-04T22:21:32.942Z Reads: 39

```
The light on the charger turns green though? I will plug it in and check the voltage a few hrs later.
```

---
## \#10 Posted by: pat.speed Posted at: 2018-04-04T23:59:26.240Z Reads: 35

```
Yeah try that, maybe the charger is dropping out too early
```

---
## \#11 Posted by: krloz Posted at: 2018-04-05T08:11:49.377Z Reads: 31

```
the charger led works based on power draw. it can be posible the charge is going so slow that it cant triger the charging led while still rising the cell voltage.
It could also, as stated, be due to a bit of power loss on the bms, in whic case you would need a hguer V charger, but honestly 1.2V is to much of an acceptable power loss in a bms. If time doesnt fix this and other chargers have the same issue try witth the bms
```

---
## \#12 Posted by: UltimaA380 Posted at: 2018-04-05T13:49:44.905Z Reads: 24

```
was plugged in all night, same thing. 

since I dont have another bms, should I just disconnect the balance leads and plug the charger in? I'd keep tabs on the cell voltage so it doesnt overcharge one or the other..

If I did it this way, the charger + would be going to the battery + and the negative going to bms, then bms to batt negative. Which I dont think should mess anything up when balance leads are disconnected, just shouldnt balance.
```

---
## \#13 Posted by: TowerCrisis Posted at: 2018-04-05T16:13:16.727Z Reads: 15

```
I recommend hooking up a multimeter in current mode and directly measuring the current output of the charger. That way you know exactly what it's doing. If current flows, it's probably a BMS issue. If there's no current, it could be the charger or the BMS.
```

---
