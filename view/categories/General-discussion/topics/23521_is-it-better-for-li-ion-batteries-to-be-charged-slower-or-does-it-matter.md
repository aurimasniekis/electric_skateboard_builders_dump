# Is it better for Li Ion batteries to be charged slower or does it matter?

### Replies: 10 Views: 806

## \#1 Posted by: headrec Posted at: 2017-05-20T01:23:58.508Z Reads: 74

```
From my drone days I've learned its best to charge lipo batteries around 1c or even .5c.  Just curious if li ion is similar or not affected the same?

Basically, I have a regular charger and a 'fast' charger.  I usually don't need to charge my board fast so wouldn't mind using a slower charger if it's beneficially to the batteries health.

Also I understand Li Ion should be left at a storage charge if not being used for an extended period of time (this is true with lipos) curious if it's the same on this as well.
```

---
## \#2 Posted by: Michael319 Posted at: 2017-05-20T02:04:13.320Z Reads: 67

```
I don't know the science behind it, and I know others can explain it better than me, but yes, charging at a low amperage is the healthiest way to charge lithium ion batteries
```

---
## \#3 Posted by: Okami Posted at: 2017-05-20T02:08:54.544Z Reads: 67

```
well im not sure where the line really starts but from some ebike guys i heard it is better to charge in 4hour time (0.25c) than faster..

Though, I usually charge at close to 0.35c and charge slower only when i dont want to hear fan noise.. 

I personally think it is fine to charge up till 0.5c. maybe at 1c it might be a bit more damaging..

You gonna need to look around, otherwise I hope this topic does not get buried under and someone gonna answer with more detail..


@PXSS might give some insight though im not sure is he available and will he give any thought onto this one
```

---
## \#4 Posted by: saul Posted at: 2017-05-20T02:22:37.749Z Reads: 64

```
Short answer yes. most li ions have a charge rate around .5c and up to 1c.

longer answer:
Charging and discharging at high rates causes more decay inside the cells. The main issue with charging li ion is that dendrites can form and eventually short out the cell(worst case). Even during standard charging some of these dendrites can be created, robbing usable Li in the process, this is why cells lose capacity over time. 

Now if you if charge around .5c most of the time, and then use a fast charger at 1c every now and then, the decrease in capacity probably won't be noticeable.

if you use a fast charger all the time, you'll probably end up on the lower side of the cycle estimate.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-05-20T04:48:11.602Z Reads: 52

```
[quote="saul, post:4, topic:23521"]
dendrites can form and eventually short out the cell
[/quote]

This was the case with lithium metal batteries but not so with Lithium ion batteries.
In fact this is the reason lithium ion batteries where developed. To eliminate the problem of dendrites.
The downside is that Lithium ion batteries have less density than Lithium metal batteries.
It is explained in detail in this video:
https://youtu.be/0PhbhRCZoTM
```

---
## \#6 Posted by: Print3r Posted at: 2017-05-20T07:59:21.608Z Reads: 47

```
According to the datasheet of A123, you can charge their 2300mah lifepo4 cells (ANR26650M1As) at 3A normal 10A fast charge and after 1000charge cycles they should be at 90% full charge max.
```

---
## \#7 Posted by: Jinra Posted at: 2017-05-20T08:02:57.392Z Reads: 45

```
Top things you can do to expand cycle life, among the obvious things such as balancing your cells.

* Charge slower
* Discharge slower (larger parallel packs help with this)
* Don't discharge too much, don't charge to full (every .1v drop from full doubles cycle life)
* Keep them cool
```

---
## \#8 Posted by: PXSS Posted at: 2017-05-20T11:09:58.892Z Reads: 36

```
The four suspected renegades responsible for capacity loss and the eventual end-of-life of the Li-ion battery are:

Mechanical degradation of electrodes or loss of stack pressure in pouch-type cells. Careful cell design and correct electrolyte additives minimize this cause.

Growth of solid electrolyte interface (SEI) on the anode. A barrier forms that obstructs the interaction with graphite, resulting in an increase of internal resistance. SEI is seen as a cause for capacity loss in most graphite-based Li-ion when keeping the charge voltage below 3.92V/cell. Electrolyte additives reduce some of the effect.

Formation of electrolyte oxidation at the cathode that may lead to a sudden capacity loss. Keeping the cells at a voltage above 4.10V/cell and at an elevated temperature promotes this phenomenon.

Lithium-plating on the surface of the anode caused by high charging rates.
```

---
## \#9 Posted by: Okami Posted at: 2017-05-20T11:14:33.301Z Reads: 29

```
yeh, I remember **3.92v** by the fact that sattelites tend to keep batteries at this level or such :D

@PXSS What is your take on charging current? At which point do you think it starts to effect cells more?
```

---
## \#10 Posted by: Namasaki Posted at: 2017-05-20T12:33:06.108Z Reads: 25

```
Good info @PXSS
Guess we still have a long way to go in perfecting Lithium cells.
```

---
