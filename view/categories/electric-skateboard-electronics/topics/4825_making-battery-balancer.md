# Making battery balancer?

### Replies: 7 Views: 827

## \#1 Posted by: Hummie Posted at: 2016-06-17T21:52:21.933Z Reads: 98

```
Who knows electronics?

I've got 48 lg hg2 cells for a 12s4p pack and want to omit the bms.  They are the safest li-ion chemistry and don't even have a gas release valve and my pack will be big enough I won't be fully charging it. 

 Anyway I plan to have both sides of the 4p accessible so I can monitor and balance by discharging.   I've seen this but it's just for monitoring:
http://www.instructables.com/id/Li-Ion-battery-level-indicator/

With my simple understanding of ohms law I feel I could reduce the circuit resistance and that will incrwse the current ...thereby discharging any high voltage cells in the pack.  No?
```

---
## \#2 Posted by: Nordle Posted at: 2016-06-17T22:08:32.057Z Reads: 94

```
Why not get a smart [BMS](https://bmsbattery.com/80-smart-BMS), which stops at 4.15 and balance cell's there. And bypass discharge?
```

---
## \#3 Posted by: Hummie Posted at: 2016-06-17T22:10:20.575Z Reads: 90

```
I want to keep it simple and feel this pack is big enough and the cells safe enough to do it this way.   ..no more room on the deck
```

---
## \#4 Posted by: emepror Posted at: 2016-06-17T22:33:47.482Z Reads: 76

```
Just increasing current draw will only cause the lower voltage cells to discharge more current, and that will cause issues potentially damaging your battery pack. Unless you get a 12 cell balance charger your going to need a BMS. I highly recommend a bms as it allows just plugging in a single connector and you don't have to worry about balancing the cells.
```

---
## \#5 Posted by: Hummie Posted at: 2016-06-17T22:37:24.177Z Reads: 70

```
Now I bulk charge 12s and balance through the addition of battery medic-like devices connected to the balance leads. I like it because I can keep all my batteries connected in series on the board and use one plug to charge.  I want to do the same with this li-ion pack but make the dischargers/monitors that I will attach to the 4 cells in parallel

I want to increase current draw from the 4p to balance
```

---
## \#6 Posted by: barajabali Posted at: 2016-06-17T22:39:10.090Z Reads: 65

```
It would work... As long as you don't over charge or discharge too crazy then the parallels would stay pretty much where they are I would check them once every hundred miles and manually balance them every so often. 

Like I said it would work but it's not ideal but I've seen it done before on E bikes

I don't know people act like batteries are so sensitive. When you charge the pack just make sure to charge at a pretty low amp rating... Like 1-2 at most
```

---
## \#7 Posted by: Hummie Posted at: 2016-06-17T22:40:10.107Z Reads: 62

```
I'm trying to find if I can change the circuitry and maybe Idecrease some of the resistance on a voltmeter so I can connect across the 4,get the voltage, and be discharging at once
```

---
