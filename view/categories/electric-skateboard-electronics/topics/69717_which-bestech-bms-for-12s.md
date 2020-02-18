# Which Bestech BMS for 12S

### Replies: 13 Views: 751

## \#1 Posted by: Marsen Posted at: 2018-10-01T08:30:53.327Z Reads: 187

```
Hi Guys looking for a 12S BMS from Bestech, any recommendations? So far the HCX-D223V1 looks favorite. Doesn't have a battery temperature probe tho just the board temperature.
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-10-01T10:21:28.243Z Reads: 182

```
either get it from buildkitboards.com or direct from bestech. dunno the model number but either the 60a or 80a discharge boards are great
```

---
## \#3 Posted by: dareno Posted at: 2018-10-03T03:39:12.287Z Reads: 158

```
Better off with a reseller as @mynamesmatt says  Bestech have a 2 unit minimum.  If you are going discharge and charge then the higher the amp rating the better.  You don't want it interfering at high loads.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-03T04:57:29.456Z Reads: 143

```
Charge/ discharge d596
Charge only d140

@dareno always good to get 2 units...
Either you short something 
Or you get into your second build
Or resell it here, bms are always needed 😅
```

---
## \#5 Posted by: dareno Posted at: 2018-10-03T05:08:16.138Z Reads: 131

```
[quote="Andy87, post:4, topic:69717"]
always good to get 2 units…
[/quote]

too true brother too true
```

---
## \#6 Posted by: Eboosted Posted at: 2018-10-03T05:26:35.094Z Reads: 125

```
[quote="Andy87, post:4, topic:69717"]
Charge only d140
[/quote]

I use d122 it's almost the same size, can handle 15A charging and it also has the equilibrium function.
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-03T05:37:34.155Z Reads: 120

```
the d140 can handle 15a charging too, but what is the equilibrium function?
```

---
## \#8 Posted by: Eboosted Posted at: 2018-10-03T05:55:26.418Z Reads: 120

```
Yes, both are 15A

It's suppose to make all packs to have the same voltage somehow
```

---
## \#9 Posted by: Andy87 Posted at: 2018-10-03T05:58:24.885Z Reads: 116

```
but isn´t a bms always making the cells the same vollatge?
or you mean that the d140 only balance when fully charged and charger plugged and the d122 also balance when the cells "rest" without charger attached?
```

---
## \#10 Posted by: Eboosted Posted at: 2018-10-03T06:01:48.731Z Reads: 111

```
Most BMSs on the market won't keep the cells balanced if they have different voltages, they will only prevent to be charged if there is big difference, avoid overcharge, avoid overdischarge, but usually won't balance p groups
```

---
## \#11 Posted by: Andy87 Posted at: 2018-10-03T06:09:48.265Z Reads: 109

```
that´s new to me, or i just got it wrong.
do you mean that a usual bms not balance all single cells in a p-group? than we speak about the same.
as far as I understood a bms will balance all p groups according to there overall voltage (doesn´t matter how much cells in the p-group).
If there cells with different volltage in the p-group they not getting active ballanced by the bms (but by voltage floating inbetween the pack maybe?)
```

---
## \#12 Posted by: Eboosted Posted at: 2018-10-03T06:24:54.364Z Reads: 107

```
Only some bms will balance p-groups, I have used several BMSs in the past, they suppose to start to reduce the voltage of the highest voltage pack when they reach the balance voltage which is usually above 4.2V by applying resistance, however the resistors are usually tiny and it's takes forever to just balance a 0.1V difference. 

The second issue is that the charger usually stops supplying voltage to the pack when it reaches EOC voltage even before reaching balance voltage
```

---
## \#13 Posted by: Andy87 Posted at: 2018-10-03T06:38:49.484Z Reads: 101

```
According to it it wouldn’t make a sense at all to use a bms for charge only 🤔
As long as the bms doesn’t start balancing before 4.2v.
Bit If it is a cc/cv charger he will not stop charging as long as there is a current request from the bms. So even with 4.2v in time of balancing of the bms the Charger should output 50-100ma (that’s what the balance current should be about)
No?
```

---
