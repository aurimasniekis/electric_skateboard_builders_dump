# Bms is charging unevenly, what is wrong?

### Replies: 13 Views: 254

## \#1 Posted by: 12meterkuk Posted at: 2018-09-03T15:33:19.107Z Reads: 98

```
I’ve got a 12s Li ion bms and a 12s charger, and I’ve wired it according to manufacturer’s diagrams yet when I charge it and charger lights turn green the first 8 cells are at 3.9v while the rest 4.2

I’ve double checked all the connections, wiring is correct, charger voltage is correct, I can’t seem to find the problem.
```

---
## \#2 Posted by: Superflim Posted at: 2018-09-03T15:34:57.916Z Reads: 96

```
If your cells are already too much out of balance, your bms can't balance them. I think you need to drain the higher voltage cells so they get around the same voltage as the rest.
```

---
## \#3 Posted by: 12meterkuk Posted at: 2018-09-03T15:35:52.500Z Reads: 94

```
But my cells were balanced at first, all of them hovering around the 3.7v mark. The bms unbalanced them
```

---
## \#4 Posted by: Superflim Posted at: 2018-09-03T15:36:36.166Z Reads: 90

```
Then the only thing I can think of faulty bms, but for so many cells it's almost impossible.
```

---
## \#5 Posted by: 12meterkuk Posted at: 2018-09-03T15:37:13.347Z Reads: 85

```
I’ll try to discharge them down first and try again, thanks!
```

---
## \#6 Posted by: Superflim Posted at: 2018-09-03T15:37:36.483Z Reads: 85

```
No problem!
```

---
## \#7 Posted by: rey8801 Posted at: 2018-09-03T17:00:18.917Z Reads: 73

```
Same issue here. I have a charge/discharge BMS. As long I was using it for both charging and discharging it worked fine. Since I switched to charging only every 2-3 weeks I need to balance 2 or 3 cells out of 10 because higher than the other. I am getting a new BMS, you should do the same.
```

---
## \#8 Posted by: dareno Posted at: 2018-09-03T19:37:55.874Z Reads: 63

```
What unit is that?
```

---
## \#9 Posted by: rey8801 Posted at: 2018-09-03T19:41:12.899Z Reads: 59

```
For who is the question? :grin:
```

---
## \#10 Posted by: dareno Posted at: 2018-09-03T20:32:40.849Z Reads: 54

```
Sorry you my friend.  Lol
```

---
## \#11 Posted by: rey8801 Posted at: 2018-09-03T21:31:07.765Z Reads: 46

```
Ah ok perfect. Then I used this one 10S 40A/60A bms Li-ion large high current BMS PCM with SAME discharge port for electric bike electric car 60a bms
 http://s.aliexpress.com/3iaIRbuA?fromSns=Copy to Clipboard. Good if you use it with discharge too. Only charging doesn't balance properly.
```

---
## \#12 Posted by: goldrabe Posted at: 2018-09-03T23:42:51.168Z Reads: 38

```
You can also balance them with a TP4056 module through the balance wires.![20180722_083335|281x500](upload://fHX3ivHIlQlU99i2c54MNOZJsQ7.jpg)
```

---
## \#13 Posted by: Namasaki Posted at: 2018-09-04T01:30:33.198Z Reads: 33

```
A BMS balances by trimming down the cells with higher voltages to match the cells with lower voltages.
This occurs when charging stops. It can be a slow process since the balance current of most bms is very low.
It does not balance by limiting charge and will only limit charge current as a safety measure if the cell voltages rise above the overcharge detection value of the bms.

The problem of your cell groups not charging evenly is not likely the fault of the bms.
Assuming that your using all new quality cells, the problem could be caused by bad weld connections in the groups that charged fully before the rest of the groups.
Bad weld connections could cause a reduction of capacity and in turn cause faster charging and discharging.
If your weld connections check out, then you could have one or more bad cells causing a reduction of capacity  in the group or groups that are charging faster than the rest.

It's a lot of work when building a Li-ion pack but I would test every cell for internal resistance and capacity before building the pack.

As for your charger going green before the pack is fully charged, check the output voltage of the charger while charging. If it is not 50.4v under load, it will not fully charge the pack.
```

---
