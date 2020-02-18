# 10S4p parallel charging

### Replies: 8 Views: 652

## \#1 Posted by: Crossfire Posted at: 2017-09-18T09:59:25.302Z Reads: 137

```
Hi folks,
I'm planning to assemble 40x Samsung 30Q batteries into 2x 5S4P packs.
Both packs will be spot welded and connected with balancing wires; that way I could charge them with my 20A charger running on a 500W PSU. 

My question is: if a single 30Q can be charged with let's say 1A, if I have them 4x in parallel that makes it 4A charging current. If I parallel charge both packs - 2x 5S4P that makes it 8A. That means that I can balance charge the 10S4P battery in parallel @ 8A without risking or damaging the cells in the long term, right?
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-09-18T10:45:16.824Z Reads: 136

```
The specs on these cell says they can be charged at 4 amps each so really the numbers could be higher. On a 4p pack you could charge at 16 amps. this would be around 45 minutes then a little longer to finish balancing so maybe an hour as an example. Not the healthiest way to charge.

So technically for charging its a 5s8p pack with 24000mah. If you divide that by 8amps it would take 3 hours plus a little to finish balancing. That is a safe charge rate and will help extend the life of the batteries.
```

---
## \#3 Posted by: Crossfire Posted at: 2017-09-18T12:06:16.236Z Reads: 123

```
Standard charge: CCCV, 1.50A, 4.20 ± 0.05 V, 150mA cut-off
Rapid charge: CCCV, 4A, 4.20 ± 0.05 V, 100mA cut-off

Looking at the specs - charging at 1.5A (0.5C) for a single cell of 3000 mAh. When in 4P that's 6A for 12Ah. And further, that's 8x1,5=12A for 8P 24Ah when parallel charging both 5S4P. And we should still be on the safe side, considering standard charge currents per cell. 

That means 24Ah/12A=2 hours of charging time plus a little more for balancing. That's great for a 12Ah 10S4P pack.
Makes sense.
```

---
## \#4 Posted by: Jinra Posted at: 2017-09-18T15:28:39.947Z Reads: 90

```
Curious to why you're splitting the pack into 2?
```

---
## \#5 Posted by: Crossfire Posted at: 2017-09-18T15:57:53.053Z Reads: 80

```
Well, I went the 2x4S 5Ah lipo way in the beginning. Now I've upgraded to dual 6355 190kV motors on 10s4p. From my drone days I own a quality server PSU (500W) and a really nice ISDT sc-620 charger who charges up to 20A and to 6S max.

Investing in a wall charger/psu for the bms and the bms itself would be another 200$ for basically inferior setup. Bms is needed only for charging and to balance the cells - my charger does that even better I always know what's going on. I should easily charge the battery with twice/thrice the amps of what a charger for bms can provide (usually 2-4A).
Plus, no additional hassle under the enclosure and less wires and electronics to get damaged while riding. I'll make the converter which will connect both batteries together in 10S and to charge them, you'll have to unplug it and plug the balance and the power cables in parallel for my RC charger. 12A charging current plus very good balancing performance to exact 4.2V per cell just can't be beat.

My 8S charging setup atm:
https://imgur.com/a/O6eUn
```

---
## \#6 Posted by: Jinra Posted at: 2017-09-18T16:01:32.327Z Reads: 69

```
Just a reminder that charging at the max charging current is not healthy for the cells and will deteriorate cycle life.
```

---
## \#7 Posted by: Crossfire Posted at: 2017-09-18T16:08:31.688Z Reads: 70

```
I'll be charging at 0.5C and no more.
1C for a single cell is 3Ah. 0.5C is 1.5A. 
1C for the pack of 5S8P is 24Ah while charging in parallel; 24*0.5=12A.  
1C for 10S4P is only 12Ah; 0.5*12=6A.

I can charge twice as fast and as safe in parallel. Hence 2x 5S4P configuration.
```

---
## \#8 Posted by: Jinra Posted at: 2017-09-18T16:09:42.027Z Reads: 69

```
ah gotcha :thumbsup:
```

---
