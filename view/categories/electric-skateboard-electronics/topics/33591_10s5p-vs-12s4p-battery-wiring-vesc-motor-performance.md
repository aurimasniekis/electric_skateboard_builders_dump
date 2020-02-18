# 10s5p vs 12s4p battery wiring&hellip;VESC/Motor performance

### Replies: 4 Views: 1067

## \#1 Posted by: gogomrrobot Posted at: 2017-09-20T18:43:47.792Z Reads: 198

```
10s5p vs 12s4p.  The 10s5p has an increased capacity amp hours (time)... you can drive your board's VESC/motors longer.  The 12s4p increases voltage but decreases capacity amp hours (time) you can run the board for.

So if you want higher top speed you go for 12s4p (48 cells) which will be faster and last shorter amount of time than a 10s5p (50 cells) battery pack which will be slower but last longer.

Is this all correct?  I really thought about building a 10s5p battery pack because 10s balance chargers are out there which then let me ditch the BMS. I couldn't find any 12s balance charger that are still in production, there were a few like the Thunder I guess back about 6-7 years ago.  I don't see any right now.
```

---
## \#2 Posted by: cwazy1 Posted at: 2017-09-20T18:58:04.378Z Reads: 193

```
Lets assume you're using a 3000mAh cell. 
A 10s5p would be 36v @ 15Ah equating to 540 watt hours
A 12s4p would be 43.2v @ 12Ah equating to 518.4 watt hours

So yes, the 10s would have a bit more capacity than the 12s. 

Since motor speed is directly related to motor kv multiplied by the voltage supplied, you would be correct in saying a 12s is faster than a 10s.
```

---
## \#3 Posted by: gogomrrobot Posted at: 2017-09-20T19:46:53.422Z Reads: 184

```
Thanks for the quick reply.  That means back to BMS and leads and all that jazz for that top speed.
```

---
## \#4 Posted by: cwazy1 Posted at: 2017-09-20T21:29:33.541Z Reads: 171

```
Also keep in mind that motor kv and battery voltage isn't the only thing that determines top speed. 

You can minimize your pulley ratios as well as use bigger wheels to reach a higher top speed. What you'll lose is torque. But depending on where you live and if you need huge hill climbing ability you might not care about torque.
```

---
