# Trying to balance while still with series connections

### Replies: 10 Views: 507

## \#1 Posted by: Hummie Posted at: 2017-04-11T20:34:45.048Z Reads: 115

```

Anyone integrate a switch of plug set-up where u could discharge in series and charge all cells in parallel?

Wouldn't need a balance charger. Couldn't be a more simplified charging method. A lot of wires though and worried they might create too much inductance for foc or need more caps
```

---
## \#2 Posted by: Nordle Posted at: 2017-04-12T07:52:34.990Z Reads: 82

```
you would need long time to charge that stuff, or 100A charger @4.2V :P
```

---
## \#3 Posted by: Hummie Posted at: 2017-04-12T15:56:10.645Z Reads: 65

```
How dissimilar voltages u think is safe to throw together in parallel?  I'm sure I've asked before but still haven't found. I'm guessing it's bad news even w Maybe tenth a volt.  
Trying to figure options to the bms always. Theoretically this is an easy solution but would take a lot of wiring. I was imagining a high amp 24 pin that would connect the cells all in series, so simply connecting the pins together and would be ON. And take the 24 pin connector plug off for OFF. And then. All cells could be connected in parallel to a 4.2 source to simply balance.  
Maybe all in parallel even with a regulated  power supply in such a situation would still put a big burden/current on the lowest cell even if regulated at 4.2
```

---
## \#4 Posted by: Nordle Posted at: 2017-04-12T18:04:54.762Z Reads: 46

```
I think you listed enough flaws in this idea yourself.
```

---
## \#5 Posted by: smurf Posted at: 2017-04-12T18:26:57.592Z Reads: 38

```
Charge at 42v and just connecting them in parallel will balance them
```

---
## \#6 Posted by: Hummie Posted at: 2017-04-12T18:34:02.870Z Reads: 36

```
I just read on rcgroups that throwing cells as distant in voltage as 50% is ok!  that seems like a huge in rush current.  
@Nordle I don't see anything wrong with doing it if that's the case but I'd like a second opinion as 50% difference in charge states being thrown together sounds like bad news.

but the wiring would be a huge pain and a plug that could handle such current would be huge.


Im still always on the hunt for an easy balancer if someone has an idea.  (discharge balancer or maybe linear supply with 12 primary and secondary or maybe get away with 12 secondary and one primary, or 12 regulated switching supplies.  
the goal is to balance solely with the balance leads and keep all the series connections intact
```

---
## \#7 Posted by: smurf Posted at: 2017-04-12T18:39:33.512Z Reads: 32

```
That's crazy talk! The smaller the better.
```

---
## \#8 Posted by: Hummie Posted at: 2017-04-12T18:42:45.352Z Reads: 32

```
this is small and cheap and ideal except it's so slow and just does 6s.  this is what I use but would rather find a more powerful version or another method.  this method is ideal, and I've found versions that could be built for 12s that are more powerful with bulbs but they're like 100$ each

https://www.tvc-mall.com/details/3-in-1-lcd-discharger-balancer-meter-tester-for-2-6s-lipo-li-fe-battery-sku87000241a.html?c=USD&utm_source=google&utm_medium=pla&utm_campaign=cse&gclid=CPDu1-7In9MCFUhffgodIIYGKQ
```

---
## \#9 Posted by: Hummie Posted at: 2017-04-12T22:27:19.861Z Reads: 26

```
anyone know if getting 12 of these little chargers and hooking them all up to individual cells and then hooking them all in parallel to a 5v power source would work or short since it says linear?  They wouldn't all work from the same supply  if these work by switching right ?

https://wholesaler.alibaba.com/product-detail/TP4056-Single-Cell-LiPo-Battery-Charger_60531963374.html?spm=a2700.7782932.1998701000.4.9KuCzN
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-04-12T22:47:22.895Z Reads: 21

```
I have them to charge batterys with small solar panels. They have a diode included so that the current doesn't go back to the solar panel. But i don't know if the diode is strong enough to block it if you go 12S. Maybe 2S is already too much.
```

---
