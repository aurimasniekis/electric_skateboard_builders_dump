# Cooling your battery - What do you do?

### Replies: 11 Views: 648

## \#1 Posted by: Matthias Posted at: 2017-12-31T16:14:24.202Z Reads: 149

```
What do y'all do for cooling your cells? I see a lot of sealed off plastic/composite enclosures that wouldn't seem to be effective for cooling. Has anyone experimented with thermal interface materials between the cells and a heat sink?
```

---
## \#2 Posted by: Kug3lis Posted at: 2017-12-31T16:15:39.121Z Reads: 149

```
If your battery heats up you are doing something wrong...
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-12-31T16:15:42.026Z Reads: 148

```
your cells shouldn’t get hot enough to require cooling.

if your battery is hot, than you wired something wrong
```

---
## \#4 Posted by: Vanarian Posted at: 2017-12-31T16:47:19.964Z Reads: 125

```
What is your ambient temp ? Are you located in a hot area ? Usually the rule is don't overstress your batteries, add a parallel pack till your power level is "normal" to your batt and not abuse anymore.

Now if you're in perma hot climate, an active cooling with fan and heatsink at least might be required (with a filter before the fan or something like that).
```

---
## \#5 Posted by: Matthias Posted at: 2017-12-31T16:52:01.959Z Reads: 116

```
A little more background on this: 

I am looking at a worst case scenario here. The pack I am looking at uses a 3P12S configuration with the Samsung 25R cell. I'd like to consider a scenario where the rider is going up a steep hill, and laying in on the throttle to climb effectively. 

I understand that batteries will heat up during usage due to q=(i^2)*r. The Samsung 25R has an internal resistance of ~0.02 Ohms. Say I am driving my cells at a continuous current of 60A, so 20A per cell. Thats 8 watts of heat. Not a terribly large amount per cell, but if we are looking at a 3P12S config, that's 288 W, which is not a negligible amount of heat production. I understand that this is driving the cells at peak power which isn't normally the case, but in the hill climb scenario, it isn't terribly unrealistic.

Looking at the cells, their environment isn't exactly conducive to heat dissipation with a plastic wrapper, plastic shrink wrap, air gap to the enclosure, and a plastic enclosure. 

Just letting the battery go through cycles of heating up beyond its thermal limits and back down will cause the cell to degrade. A cell's electrodes begin to break down when they reach 70C. I am not worried about thermal runaway as much as usable life.
```

---
## \#6 Posted by: Matthias Posted at: 2017-12-31T16:53:30.134Z Reads: 105

```
For this scenario, lets say the ambient temp is 30C. Hot, but not scorching.
```

---
## \#7 Posted by: Maxid Posted at: 2017-12-31T17:01:25.800Z Reads: 103

```
60A at 12S would be around 3000W to the motor - have a look at VESC logs and you'll see that even when climbing hills you will not reach those numbers. Your VESC will heat up way quicker than your cells and will limit the current accordingly.
```

---
## \#8 Posted by: Matthias Posted at: 2017-12-31T17:09:12.867Z Reads: 97

```
I'll have a look at that
```

---
## \#9 Posted by: Namasaki Posted at: 2017-12-31T17:49:13.760Z Reads: 88

```
@Maxid is correct but another key factor that you should consider is voltage sag which is usually more of a problem than heat. 
Also 25R’s are not the best cells to use. 
Samsung 30Q’s are much better by reputation.
```

---
## \#10 Posted by: Maxid Posted at: 2017-12-31T17:54:32.746Z Reads: 85

```
Another way to look at it: A 3P battery with 25Rs will have 7.5Ah of capacity. At a continuous 60A this will be drained completely in just 7.5Ah/60A=0.125h (which is 7.5min ;) ).
That alone should convince you that such numbers are unrealistic when riding - otherwise we would all be walking home every single time.
```

---
## \#11 Posted by: banjaxxed Posted at: 2017-12-31T18:25:06.745Z Reads: 72

```
If this is imperative then you will need to use cell spacers and either 

a) pc fans moving air along gaps between cells or 
b) a tesla cooling loop paired with a small marine rc pump/rad filled with pc cooolinh loop fluid

Either way your using cell spacers which should give a certain amount less radiant heat
```

---
