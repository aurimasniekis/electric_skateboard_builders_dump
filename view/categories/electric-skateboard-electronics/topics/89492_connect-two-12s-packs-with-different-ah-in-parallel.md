# Connect two 12S Packs with different Ah in parallel

### Replies: 35 Views: 338

## \#1 Posted by: directC Posted at: 2019-04-05T17:59:45.816Z Reads: 87

```
Hi

I'm not really findig a clear answer  

Let's say I have 2 Batteries  
Both are 12S  
Both are made with the same cells  
1st Pack is 8P  
2nd Pack is 14P  

Would it be possible to  
1 connect them directly  
OR  
2 put something in between to connect them?

If 2, what is this thing called?
```

---
## \#2 Posted by: Skunk Posted at: 2019-04-05T18:03:10.406Z Reads: 83

```
You trying to make a 12s22p?
```

---
## \#3 Posted by: thisguyhere Posted at: 2019-04-05T18:03:50.065Z Reads: 85

```
[quote="directC, post:1, topic:89492"]
1 connect them directly
[/quote]

no

[quote="directC, post:1, topic:89492"]
2 put something in between to connect them?
[/quote]

a buck step-down converter, that takes 14s voltage and drops it to 8s.

or a voltage step up, that takes 8s voltage up to 14s voltage
```

---
## \#4 Posted by: directC Posted at: 2019-04-05T18:04:05.632Z Reads: 83

```
maybe  
for multiple day rides
```

---
## \#5 Posted by: directC Posted at: 2019-04-05T18:05:31.154Z Reads: 81

```
BOTH are 12S = same voltage

1st is 8P
2nd is 14P = different Ah
```

---
## \#6 Posted by: Stevemk14ebr Posted at: 2019-04-05T18:06:11.194Z Reads: 79

```
put the two batteries in parallel. They're same voltage so it's fine. Same reason you don't do anything special adding more 'P' rows to battery you're building.
```

---
## \#7 Posted by: directC Posted at: 2019-04-05T18:08:55.038Z Reads: 78

```
will they get to 0% the same?
or will the bigger one still have some Ah left? -> won't the smaller one get discharged too low and take damage?
```

---
## \#8 Posted by: ZachTetra Posted at: 2019-04-05T18:09:48.362Z Reads: 78

```
You can connect them in parallel for a 12s22p pack and it will discharge fine

If you connect them in series it will be about 100V and melt everything...do not do that

To charge it you're gonna need to bridge the p-packs so they balance or use 2 BMSs
```

---
## \#9 Posted by: janpom Posted at: 2019-04-05T18:11:00.188Z Reads: 72

```
No, they will remain at the same voltage at all times. Charging is problematic though. You would need two BMSes.
```

---
## \#10 Posted by: Stevemk14ebr Posted at: 2019-04-05T18:11:19.130Z Reads: 72

```
They will provide an unequal amount of amperage, the bigger providing more and will discharge at the same time.
```

---
## \#11 Posted by: directC Posted at: 2019-04-05T18:12:22.943Z Reads: 67

```
For Series I know, but that wouldn't make much sense anyway for current eSkates  
for charging i would anyway use 2 BMS so that's fine
```

---
## \#12 Posted by: directC Posted at: 2019-04-05T18:12:55.217Z Reads: 65

```
Connect in parallel, not series
```

---
## \#13 Posted by: ZachTetra Posted at: 2019-04-05T18:13:04.932Z Reads: 64

```
They will always have the same total voltage so they will get to 0% t the same time
```

---
## \#14 Posted by: janpom Posted at: 2019-04-05T18:14:27.588Z Reads: 62

```
[quote="directC, post:12, topic:89492, full:true"]
Connect in parallel, not series
[/quote]

I know. What's your point?
```

---
## \#15 Posted by: directC Posted at: 2019-04-05T18:14:31.029Z Reads: 60

```
Ok, good so far

How about I have 2 packs BOTH 12S

1st has 30Q cells
2nd has 35E cells

i guess that would still work, as it only changed the Ah?
```

---
## \#16 Posted by: ZachTetra Posted at: 2019-04-05T18:15:22.241Z Reads: 57

```
Absolutely not, never mix cells in a battery
```

---
## \#17 Posted by: directC Posted at: 2019-04-05T18:15:27.277Z Reads: 56

```
sorry, understood your answer wrong  
thought you meant: no, you can't double the voltage
```

---
## \#18 Posted by: directC Posted at: 2019-04-05T18:16:43.505Z Reads: 55

```
but why?
i mean if they're on the same voltage?
```

---
## \#19 Posted by: Pedrodemio Posted at: 2019-04-05T18:17:45.536Z Reads: 57

```
All you need is here already 

https://www.electric-skateboard.builders/t/top-and-bottom-mounted-enclosure/89402?u=pedrodemio
```

---
## \#20 Posted by: ZachTetra Posted at: 2019-04-05T18:18:06.405Z Reads: 56

```
I mean you can try but the cells with the lease internal resistance will take the brunt of the amp draw and degrade quickly
```

---
## \#21 Posted by: directC Posted at: 2019-04-05T18:18:51.313Z Reads: 52

```
so they would just die faster?
```

---
## \#22 Posted by: ZachTetra Posted at: 2019-04-05T18:22:05.832Z Reads: 49

```
No it will stress the cells out... drastically reduced lifespan
```

---
## \#23 Posted by: janpom Posted at: 2019-04-05T18:30:48.847Z Reads: 49

```
Sorry, this is interesting. How exactly does that work? Is the current drawn primarily from the low internal resistance cells and then they get recharged from the other cells? The P-pack will self balance. Current will be drawn from all cells.
```

---
## \#24 Posted by: ZachTetra Posted at: 2019-04-05T18:34:55.153Z Reads: 48

```
In order to keep the cells at the same voltage they have to discharge at a certain rate, the amp draw is proportional to the capacity
```

---
## \#25 Posted by: directC Posted at: 2019-04-05T18:36:02.225Z Reads: 45

```
i just read that using diodes would work. ?
```

---
## \#26 Posted by: ZachTetra Posted at: 2019-04-05T18:36:03.359Z Reads: 47

```
I mean I'm not an expert by any means but the load will be disproportional.  The highest voltage cells will suffer the most amps, and that may be the lower rated cells
```

---
## \#27 Posted by: Winfly Posted at: 2019-04-05T18:48:44.314Z Reads: 45

```
[quote="ZachTetra, post:20, topic:89492"]
the cells with the lease internal resistance will take the brunt of the amp draw and degrade quickly
[/quote]

He's using the same cells in both packs. And it's is true that when it's under load, it will draw more from the larger pack. But at cell level, each p should discharge at the same rate when both packs are connected in parallel.

And yes it's better to use 2 separate BMS and charge them separately. And it's safer to disconnect the parallel plug when you charge.
```

---
## \#28 Posted by: directC Posted at: 2019-04-05T18:50:21.345Z Reads: 44

```
the question was, if one could connect 2 x 12S packs with different battery types, eg. 30Q + 35E
```

---
## \#29 Posted by: Winfly Posted at: 2019-04-05T19:00:51.097Z Reads: 44

```
Oh. I missed that. In that case he's absolutely right. It will discharge evenly but how much it damage the cells still depends on how many Amp each pack discharge.
```

---
## \#31 Posted by: DEEIF Posted at: 2019-04-05T19:35:36.599Z Reads: 40

```
Like @Pedrodemio said in my thread, you would need both packs to be charged to a perfect 100% before being connected. The pack that is the Extra Range pack would them need to be connected through the pack on the boards charger port. The charger port on the board would NEED to be connected to a bms. This would then work as a XR battery pack. Until the one day you forget to charge both to 100%...
```

---
## \#32 Posted by: janpom Posted at: 2019-04-05T19:52:01.183Z Reads: 36

```
Sure, but I can't really see how that would be a problem as long as the difference in the capacity isn't extreme. I imagine mixing up 30Q and 30E would be fine (though maybe the different C rating rather than different capacity would cause trouble). Also, it looks like @directC is considering using a big battery (22P?) so the load per cell would be pretty low.
```

---
## \#33 Posted by: ZachTetra Posted at: 2019-04-05T19:54:41.915Z Reads: 34

```
That's a fair point, that pack should be fine to draw 200A and I can't imagine you'd need more than 10kW for a skateboard
```

---
## \#34 Posted by: Pedrodemio Posted at: 2019-04-05T21:15:41.482Z Reads: 30

```
Exactly, it’s not needed to be perfectly, 1v of diference is perfectly fine

And about two different cells, since most Liion cells have a similar low voltage limit, it should be fine, but it’s always good to keep and eye on it

If your main cell can take the current you set on the vesc, by joining another one you are only decreasing the load
```

---
## \#36 Posted by: Pedrodemio Posted at: 2019-04-05T21:32:56.766Z Reads: 27

```
Yes, but as I said, if you normally use your main pack, with the currents dialed in for it, and connect a different one, it will not get stressed, on the contrary it will be less stressed
```

---
## \#38 Posted by: Pedrodemio Posted at: 2019-04-05T21:44:52.402Z Reads: 26

```
Yep, to be sure, calculate the internal resistance of both complete packs, and check how the current will be distributed between them, if it’s bellow the limit of both packs go ahead
```

---
