# Feedback on Parallel LiPo Schematic?

### Replies: 4 Views: 197

## \#1 Posted by: MattCarl Posted at: 2019-05-18T01:05:02.002Z Reads: 61

```
I'm building the 3rd version of my board and was hoping to get some feedback/sanity check on my electrical schematic. I've put 1,000+miles on a similar setup with a single 6s 5000mah single BLDC setup, and frankly I love it. but the 5-7 mile range is rough so I'm planning a revamp with three brand new 6s lipo batteries hooked permanently in parallel.  

I've read a bunch on here about permanent parallel batteries and have gathered that it is safe as long as I connect the high power lines together first. The only downside is that I won't be able to monitor each individual cell without opening the electronics box. 

I wanted to keep it a 6s instead of 10s or 12s so I can continue to use a balance charger instead of BMS, that way I can easily monitor cell voltage from the charger and put the battery into storage voltage. 

I've attached the schematic... I'm hoping I could get a sanity check that this will work before I pull the trigger on buying new batteries. 

Thanks!![Electrical_Schematic|690x390](upload://iRNPDaRtCXq1R1EbnZfLE5yypjx.png)
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-05-18T02:10:32.967Z Reads: 50

```
the schematic looks great. you should be fine with this. just make sure you hook up lipos that are all perfectly matched voltages to begin with. if possible, get a 7 pin jst-xh splitter to make it more modular, then have an easy access port to disconnect the balance wires and put in cell tester. lipos go out of balance easier than li-ion and the results can be catastrophic if not caught early on. its not a huge issue, but im always way over cautious when handling batteries

btw, if you are worried about a spark from the lipos when connecting to the vesc for the first time, hook up the negative and bridge the gap between the positive with an ordinary .5w resistor between about 100 and 2k ohms you will then have a few minutes to reconnect without a spark.
```

---
## \#3 Posted by: MattCarl Posted at: 2019-05-19T16:18:18.304Z Reads: 23

```
Thanks so much for the feedback! The splitter and resistors are great ideas!
```

---
## \#4 Posted by: Dirt_Bag Posted at: 2019-05-19T16:44:53.461Z Reads: 13

```
It has worked well for me. I didnt have antispark xt60 connectors so i just used that method. Its really no different than how antispark connectors work, just a bit more difficult
```

---
