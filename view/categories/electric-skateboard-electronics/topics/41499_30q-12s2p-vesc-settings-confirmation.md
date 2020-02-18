# 30Q 12s2p VESC settings confirmation

### Replies: 12 Views: 750

## \#1 Posted by: DragonSwagin Posted at: 2017-12-19T23:31:25.336Z Reads: 193

```
I had a quick question about where I should set the battery cutoff end for a 12s2p 30Q battery for my board. I've read numbers anywhere from 2.5 to 3.3 volts minimum cutoff end for the cell. The search bar didn't give a clear answer so I figured I'd make a topic to get some real answers. Anyone know best cutoff for 30Q battery?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-12-19T23:58:41.193Z Reads: 192

```
Li-ion cells like the 30Q  can go down to 2.5 but it would be a good practice to not take them down to their low limit.
Personally, I would consider 3.0v to be a conservative low voltage for any Li-ion cell.
If your discharging through a bms then you could safley go down to 2.8v
But if your bypassing the bms and using the Vesc low voltage, I would set the low voltage start at 3.0v and the low voltage end at 2.8v per cell and stop riding when the vesc reduces power from the first threshold.
```

---
## \#3 Posted by: DragonSwagin Posted at: 2017-12-20T00:12:29.643Z Reads: 182

```
So I'm "safe" to use 2.8v if I'm running it through a BMS? How much extra mileage do you think I would get with going for riskier numbers? (In terms of percentage?)
```

---
## \#4 Posted by: Namasaki Posted at: 2017-12-20T00:18:40.526Z Reads: 170

```
The idea is that if you are discharging through the bms, the bms will monitor each cell group and shut down if any cell group reaches the low voltage detection which is usually set at 2.8v for Li-ion.
If this happens when you are acceleration hard or going fast under power, the sudden loss of power could cause you to be thrown off the board.
So you can run it all the way down till the bms shuts down but be careful when your battery gets below 50%
I have had the bms shut down on me a couple times while riding and it was no issue because I was just cruising.
```

---
## \#5 Posted by: rojitor Posted at: 2017-12-20T06:15:02.135Z Reads: 149

```
I never discharge beyond 3.3v it reduces the lifespan.
Also charging to 4.10 doubles  the number of cycles.
```

---
## \#6 Posted by: DragonSwagin Posted at: 2017-12-20T14:48:04.959Z Reads: 131

```
About to get a little question heavy as I'm trying to learn, so here I go. Why does charging to 4.1v instead of the standard 3.7 double the cycles? What are the pros and cons of charging it that far up? Will the increased voltage on a 12s setup have unforeseen effects on the rest of the system?
```

---
## \#7 Posted by: rojitor Posted at: 2017-12-20T15:41:00.924Z Reads: 126

```
3.7v is nominal. 4.2 is full charge and depending on the cell 2.5-2.8v is full discharge. 3.3-3.0 Is the usual common sense lvc 
Those are the usual numbers. The life of the cells is deeply affected by the charge and discharge. It is not good full charge nor full discharge.
The electric cars usually charge to 4v and discharge to 3.3-3.6v therefore after several years of use the cells are like new. You can see people asking for 1k+ usd for used tesla packs and they are worth it. Those cells still have 2/3 of their practical life ahead.
[example](https://endless-sphere.com/forums/viewtopic.php?f=9&t=67661&hilit=Tesla+cells)
[example 2](https://endless-sphere.com/forums/viewtopic.php?f=9&t=88410)
Undercharging li ion is a good practice. The bms usually balances above 4.1 v. I have two chargers for my 6s board. 25.2 and 24v so I usually charge to 24v and every now and then to 25.2 to let the bms do its job.
Smart bms boards can be set to balance lower so no need for that trouble. 
Charging to 4.10 doubles lifespan and charging to 4.0v and discharging to 3.3v triples it, in that case you lose quite some range though.
```

---
## \#8 Posted by: PXSS Posted at: 2017-12-20T17:52:27.218Z Reads: 111

```
[quote="rojitor, post:7, topic:41499"]
Charging to 4.10 doubles lifespan and charging to 4.0v and discharging to 3.3v triples it, in that case you lose quite some range though.
[/quote]

What’s your source?
There is no research as far as I’m aware that states that discharging below 3.3 is degrading.
```

---
## \#9 Posted by: scepterr Posted at: 2017-12-20T18:07:56.994Z Reads: 104

```
https://www.researchgate.net/publication/303890624_Modeling_of_Lithium-Ion_Battery_Degradation_for_Cell_Life_Assessment
```

---
## \#10 Posted by: PXSS Posted at: 2017-12-20T23:18:21.307Z Reads: 94

```
My main gripe with that paper is that they didn’t try using the cell from 50-0%. Would it have been better or worse than 75-25%? Would 90-40% work? 

If I recall correctly, the high voltage accelerates the dendrite formation but there is no explanation as to what reduces the life of a battery if used on the lower end of the curve or if it’s simply because of the lower voltage.
```

---
## \#11 Posted by: scepterr Posted at: 2017-12-20T23:45:37.446Z Reads: 90

```
As far as I understand and I'll try to find some data later is that cell resistance increases at lower V
```

---
## \#12 Posted by: DragonSwagin Posted at: 2017-12-23T04:12:04.434Z Reads: 82

```
The charger I'm using will charge the cells to 4.2 volts. I'm going to do some test rides over the next few days discharging to various numbers (anywhere from 2.8 to 3.3 volts) and graph what sort of range I get by discharging to different numbers. I figure some people may find it useful to see an exact amount of range they can get based on how far they want to stress their batteries.

edit: I'm dumb. What I'm going to do is discharge to 2.8 volts and monitor what sort of range I get at various discharge points and take note of them
```

---
