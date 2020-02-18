# Imax b6 overcharging one cell

### Replies: 18 Views: 1074

## \#1 Posted by: IsTalo Posted at: 2017-05-07T14:12:23.114Z Reads: 69

```
Hey guys, so I have a 6s battery and a Imax b6 v2, but this one is overcharging one cell to 4.4v and don't charge one cell that is 3.83v, what should I do? Like, I put in balance mode and the 4.4v change between 4.1v and 4.45v and I don't know what to do, always my Imax b6 indicates the "Overvoltage cell" alarm, help me, should I change It and definitely buy a Bms?
```

---
## \#2 Posted by: flywithgriff Posted at: 2017-05-07T14:15:54.166Z Reads: 70

```
I have a similar issue but mine undercharges one cell by .15.
```

---
## \#3 Posted by: IsTalo Posted at: 2017-05-07T14:18:29.449Z Reads: 69

```
Like, 4.05v?
```

---
## \#4 Posted by: Namasaki Posted at: 2017-05-07T14:58:49.126Z Reads: 61

```
The charger should not over charge ever. 
Are you sure you have it set correctly?
Is your charger an authentic skyrc brand?
Did you buy it on eBay for a cheap price?
Could it be a counterfeit?
```

---
## \#5 Posted by: IsTalo Posted at: 2017-05-07T15:03:49.007Z Reads: 55

```
Yep, I set it to Balance Mode, 6s and 3.0A.
It seens autentic, have the holographic sticker in the back, but I can't see if it is fake or not because the Skyrc don't open in my iphone or in my Pc, could you see for me? I send you a pic
I bought it from a local hobbystore in Brazil
Yeah, it could be counterfeit
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-07T15:13:00.197Z Reads: 52

```
Did you set the mah limit in settings menu?
Make sure you have it set for correct lithium  chemistry. 
If all settings are correct, then your charger must be defective. 
Be careful, overcharging lithium batteries like that can be dangerous.
```

---
## \#7 Posted by: IsTalo Posted at: 2017-05-07T15:16:13.326Z Reads: 52

```
You mean, Capacity Cut-Off? It was off, but now I've put it on!
Yeah, It just have Lipo option
```

---
## \#8 Posted by: Hummie Posted at: 2017-05-07T16:16:11.607Z Reads: 46

```
damn that's scary.  You think youre all safe with your balance charger and then bam!
4.45 and THEN finally an over-voltage alarm...maybe it will tell you after it lights your house on fire.
```

---
## \#9 Posted by: IsTalo Posted at: 2017-05-07T16:17:14.868Z Reads: 46

```
Yep, but is the problem with the charger? Because it overcharge one cell and don't charge other
```

---
## \#10 Posted by: Hummie Posted at: 2017-05-07T16:19:40.966Z Reads: 45

```
my broken record advice is get a bulk charger,  charge at 4x the speed, and monitor and balance with one of those little balancer.  the bms and balance charger are too complicated and then youre relying on computers.   set the bulk charger to a max of 4.1 each cell and set the low voltage cut offs on the vesc  to the combined voltage with 3.6 and 3.5 each cell if lipo.  hope you got the vesc.  

a whole lot easier and definitely safer in your case
```

---
## \#11 Posted by: Hummie Posted at: 2017-05-07T16:24:18.615Z Reads: 39

```
yea sounds like the charger is broken.  not balancing.  I'd think that should happen regardless as long as your set to lipo.  try another battery on it maybe but i can't see the battery being the issue
```

---
## \#12 Posted by: IsTalo Posted at: 2017-05-07T16:36:59.779Z Reads: 39

```
Fine, I'll bring it to the hobbystore and see
```

---
## \#13 Posted by: IsTalo Posted at: 2017-05-07T16:38:18.643Z Reads: 39

```
Wait, you're telling me to configure the Imax? Yeah, I have the Vesc and a Buzzer
```

---
## \#14 Posted by: Hummie Posted at: 2017-05-07T16:44:18.521Z Reads: 39

```
was saying forget the balance charger and get a fast charging bulk charger and little discharge balancer.
```

---
## \#15 Posted by: IsTalo Posted at: 2017-05-07T16:55:44.901Z Reads: 38

```
What about a Bms?
```

---
## \#16 Posted by: Hummie Posted at: 2017-05-07T17:41:13.559Z Reads: 32

```
my opinion is to not bother with the bms.  simplify everything because everything breaks.  even my simple xt90s plug (instead of a switch) eventually dies and i need to replace it.  but thats easy to replace and an easy fix.  really you dont even need an anti spark switch or plug and worst case you carbonize your connectors and slowly build resistance there and need to replace them.  (or someone here was using dielectric grease on them ironically, stopping the arc through the air and then smoothing the metal good connection together.  never tried it but sounds like a simple option.
but the bms...if the low voltage cutoffs are set on the vesc and youre around when you charge and maybe even check your individual voltages even every time you charge... I feel safe.   This is a typical charging method for diy ebikers.  takes a bit more responsibility but I enjoy being more involved.  And then you have more money and more room for batteries!
```

---
## \#17 Posted by: 2-alex-2 Posted at: 2017-05-07T18:10:15.051Z Reads: 29

```
I would recommend trying a new battery or another one that's good. As it maybe that you also have a dead cell which is charging to quick compared to the others. The charger it's self may be fine.
```

---
## \#18 Posted by: IsTalo Posted at: 2017-05-07T18:20:22.344Z Reads: 28

```
I dont think so, because when the guy at the hobbystore charged with his charger it just worked fine, the cells that was 4.2 stayed 4.2 and the other charged, but I dont happened to me, I put to charge when one cell was 4.05v and than it overcharged
```

---
