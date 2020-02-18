# Finding The Best BMS

### Replies: 11 Views: 2923

## \#1 Posted by: Esrapp21 Posted at: 2016-11-09T01:51:55.818Z Reads: 276

```
In my discussion "Series and Parallel Circuits" some people brought up the idea that a BMS would solve a lot of my problems. I became uneasy about using BMS after watching this video: https://youtu.be/pljSZcEwc8Q Are there any BMSs that show voltage and can display whether it is working properly?
```

---
## \#2 Posted by: chinzw Posted at: 2016-11-09T01:59:27.164Z Reads: 275

```
There's quite a few "smart" bms that has LEDs and some with USB/BT. I also have a working arduino monitor to check the battery and bms.
```

---
## \#3 Posted by: Namasaki Posted at: 2016-11-09T06:59:43.138Z Reads: 256

```
Bestech is a reputable source for battery management systems and they also offer models with communication capabilities.
http://bestechpower.com/products/
```

---
## \#4 Posted by: Esrapp21 Posted at: 2016-11-09T12:45:51.569Z Reads: 232

```
@Namasaki the only thing is that when I am changing the circuit from series to Parallel and vise versa, it switches between 6s and 12s, but the BMS doesn't offer that range.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-11-09T13:03:45.900Z Reads: 207

```
I have tested switching from 12s to 6s with 2 6s Lipos
You don't gain range switching to 6s because you pull twice the amps. 
The only thing you accomplish switching to 6s is having less torque.
Voltage X MAH = watt hours
Watt hours detemine range
```

---
## \#6 Posted by: Esrapp21 Posted at: 2016-11-09T15:01:54.183Z Reads: 184

```
But when charging, it is much easier to charge 2 6s in parallel because you can use a regular hobby charger.
```

---
## \#7 Posted by: deucesdown Posted at: 2016-11-09T15:09:22.378Z Reads: 173

```
If you have 12s with BMS, buy a 12s bulk charger for $20-60. The charger will handle the CC/CV and cutoff, the BMS will balance and provide a safety net.

You buy the BMS and bulk charger so you can stop using 6s hobby chargers.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-11-09T15:54:13.296Z Reads: 166

```
It's not easier with a hobby charger and it's not a good idea to charge Lipos in parallel.
@deucesdown 
The reason it's not a good idea is that when you charge in parallel, your basically taking 2 cells with different internal resistance and calling them 1 cell. 
Since their internal resistance is different, they will not charge or discharge evenly. 
Anytime you put lithium cells in parallel, it's a comprise.
Balancing cells individually is always the best option.
This is my opinion.
```

---
## \#9 Posted by: deucesdown Posted at: 2016-11-09T16:12:13.535Z Reads: 162

```
[quote="Namasaki, post:8, topic:12743"]
not a good idea to charge Lipos in parallel
[/quote]

If you know what you're doing, I don't think parallel charging is unsafe, at least not anymore than charging lipos in general?

Each "s" cell must be in similar state of charge with its parallel pair, as they will charge/discharge each other until equilibrium is reached. Which should be the case if the pack was being run in series in the board, if there are no "problems" like unequal resistances, uneven heating.

And the cells must generally be in good condition.

I don't think the capacities need to really match, as the one with more capacity will take more of the power.

Beyond that, I don't see how it's any more dangerous than series charging?

But as with anything with diy lithium ion, you really should know what you're doing, and be prepared for the worst.
```

---
## \#10 Posted by: chinzw Posted at: 2016-11-09T18:17:56.086Z Reads: 147

```
Actually, parallel charging cells will "balance" them.
```

---
## \#11 Posted by: Namasaki Posted at: 2016-11-09T18:57:19.353Z Reads: 141

```
[quote="chinzw, post:10, topic:12743, full:true"]
Actually, parallel charging cells will "balance" them.
[/quote]
True, however, it has been mentioned before on this forum that multiple cells charged in parallel will level out suddenly and this can shock them if there voltages are not close already when the leveling occurs. 
This was in regards to building Li-ion packs and ensuring that cells where matched before assembly.
I believe In the case of a Li-ion pack, once the cells in each parallel group are level, they should remain level because they are permanently connected in parallel. 
In the case of Lipo packs used in series and then connected in parallel for charging, the cells will have to level out every time you charge and with the risk of shocking the cells. 
So, what I did when I was using 2 6s Lipo packs in series on my first build was to disconnect them and charge them separately with a dual bank hobby charger. 
<img src="/uploads/db1493/original/3X/b/c/bc022cb17de76b77561c1209eb73a67b3b40429e.jpeg" width="372" height="500">
<img src="/uploads/db1493/original/3X/a/a/aa00d76d264e2c95f657ca1d895ba13e669484ad.jpeg" width="375" height="500">
```

---
