# VESC low max ERPM

### Replies: 11 Views: 756

## \#1 Posted by: Moav Posted at: 2019-03-05T18:14:07.267Z Reads: 116

```
I've got a VESC 4.12 connected to a MAYTECH 6365 170KV motor with a 12S. On max throttle testing, the VESC app shows around 46K ERPM. I wonder why is that is its limit? Should be enough for about 50kph but it could reach 100K easy when there's no resistance right?
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-03-05T18:19:58.358Z Reads: 114

```
you should use the search button and look up some formulas and general understanding
```

---
## \#3 Posted by: TowerCrisis Posted at: 2019-03-05T18:53:06.176Z Reads: 109

```
 You should cap out around 60,000 erpm with a 170Kv motor and a 12S pack. 

Are you fully charged? That will greatly affect max speed.

Also, motor KV may not be accurate. Could be quite different from the manufacturer spec.

You also are limited to 95% duty cycle so that further lowers max speed.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-03-05T19:32:06.025Z Reads: 100

```
[quote="Moav, post:1, topic:86223"]
I wonder why is that is its limit
[/quote]
Depends what you set in your vesc tool.
If you set it to 46k than it is.

[quote="Moav, post:1, topic:86223"]
Should be enough for about 50kph
[/quote]
You know that this depends on your gearing and wheel diameter. It’s not connected to the vesc hw version



[quote="Moav, post:1, topic:86223"]
could reach 100K easy
[/quote]

Good luck with it. Besides the fact that your motor top out at close to 60k if the kV rating is correct and your battery is fully charged aaand there is no load at all, 100k would let your maytech 4.12 smoke up a bit...pretty fast
```

---
## \#5 Posted by: Moav Posted at: 2019-03-05T20:48:17.782Z Reads: 80

```
By my calculations the 170KV should give out 8500 RPM it is on 3500 only. the VESC shows 49.7V from the 12S. There's no 46K or close-to limit on any ERPM variable on the app.
```

---
## \#6 Posted by: Moav Posted at: 2019-03-05T21:04:30.325Z Reads: 78

```
My limit on the VESC app seems to be 100K ERPM.
About the max speed, yes my wheels are 85mm so 2*pi*r*rpm*60/1000.
Lastly, if my ERPM is 46K and the Volt is 50 then the motor is at 70kV. Why should the VESC smoke if the amp is not hitting even 10A? (there's a little load of the chain, wheel and metal gear pullies.
```

---
## \#7 Posted by: TowerCrisis Posted at: 2019-03-05T21:59:45.125Z Reads: 69

```
You've made a mistake somewhere in your calculations.

49.7V * 170KV * 7 pole pairs =59143 Erpm.

Also, any vesc 4.12 CANT run more than 60,000 Erpm. They become very unstable.

[quote="Moav, post:6, topic:86223"]
My limit on the VESC app seems to be 100K ERPM
[/quote]
If that's true then you need to lower that limit to 60K, else you risk blowing up your vesc.
```

---
## \#8 Posted by: Moav Posted at: 2019-03-05T23:42:12.140Z Reads: 55

```
I thought it was calculated by counting all poles (14). That makes more sense with 7 poles.

I'll limit it to 60K, still wonder why it can't reach its max rotational speed (20% off) - the app's live meter showed me 46K, it wasn't calculated.
```

---
## \#9 Posted by: Sn4pz Posted at: 2019-03-05T23:59:41.965Z Reads: 52

```
You should really limit it to 50k to have.... somewhat of a safe experience?

I wouldnt trust a regular 4.12 past 35a per vesc, or over 55k :0 

too close to the sun, Icarus :P
```

---
## \#10 Posted by: Moav Posted at: 2019-03-06T07:25:48.556Z Reads: 46

```
I will, but it is strange that the app allow more than that.
I've got both VESCs on aluminum housing attached to the mosfets so i was hoping for a 50A continues.I won't use it much accelerating, but for breaking that could come in handy.
```

---
## \#11 Posted by: Andy87 Posted at: 2019-03-06T09:06:24.261Z Reads: 42

```
[quote="Moav, post:6, topic:86223"]
Why should the VESC smoke if the amp is not hitting even 10A?
[/quote]

https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125?u=andy87

https://www.electric-skateboard.builders/t/what-is-the-problem-of-passing-the-erpm-limit/20690?u=andy87

https://www.electric-skateboard.builders/t/what-is-focbox-vescx-erpm-limit/30614?u=andy87

https://www.electric-skateboard.builders/t/vesc-erpm-limit/61699?u=andy87

plus the links in the threads to the vedder forum etc etc.
hope that´s enough information for you at the moment.
```

---
