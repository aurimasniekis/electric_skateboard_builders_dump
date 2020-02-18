# VESC 4 problem not idea

### Replies: 9 Views: 257

## \#1 Posted by: Ingvarjedi Posted at: 2018-06-28T04:02:01.419Z Reads: 74

```
I have VESC 4 from DIYelectric......
I used Li-Po 12s 15000mAh

When the battery is fully charged, there is a lot of power.
But!
At a voltage of 46 volts, power drops, the board goes slowly. Is this anomalous or not? what could be the problem? I put in the settings VESC cut-off in 42 volts.
```

---
## \#2 Posted by: wafflejock Posted at: 2018-06-28T04:06:27.005Z Reads: 74

```
There are two cut offs, the hard and the soft cut off did you set both to 42V?  The per cell voltage at 42V is 3.5V which is edging on a bit low where you might have some substantial difference between the cells on final discharge so might want to make that 3.6 until you have some trials with it and can see how far off the cells are from each other and decided if you want to go down to 3.5 for that extra little bit.  You might see some dip in top speed but I wouldn't expect much change in acceleration until you hit somewhere in the soft cut off to hard cut off range.  At 46V you're at 3.8V per cell so I wouldn't expect significant performance drop yet you're still just about in the middle of the battery (kv*V = RPM so some decrease).  I do notice my board is more punchy right out the gate but it's not a huge difference.

---

It's possible some overheating issue is causing the power to be limited as well after riding for some time but hard to really pin anything down without telemetry data or some other real time data captures.
```

---
## \#3 Posted by: Ingvarjedi Posted at: 2018-06-28T04:27:13.809Z Reads: 57

```
You can see my telemetry data.
[https://metr.at/r/V0B7j](https://metr.at/r/V0B7j)

There was also a loss of power when driving to the hill, at the very top of the power was not enough.
Time: 20:07:42 - 20:07:57
```

---
## \#4 Posted by: Ingvarjedi Posted at: 2018-06-28T05:08:44.294Z Reads: 54

```
@evoheyax
 say your opinion. Is it the nature of Li-Po?))
```

---
## \#5 Posted by: wafflejock Posted at: 2018-06-28T05:12:03.199Z Reads: 51

```
Based on the data I'd say it's likely a problem between the receiver and vesc or receiver and transmitter.  Guessing this because your voltage stays pretty stable throughout the ride and the amperage is just plateauing at that point.

---

One other interesting thing in the data, at the point where the amperage takes a drop off the 'temperature' reading makes a little spike as well.  I'm not sure where things start getting throttled for thermal control but 80C is pretty toasty for regular processors.

---

For comparison here's my data from a ride a few minutes ago:

https://metr.at/r/uDeqf

Can see the amperage is much more 'granular' looking never really levels off because the input is always changing a bit as my finger moves around.  Also just noticed a big voltage dip in there, I hit a serious crack in the road and felt the board give out as it reset (one of my 2 5S lipos disconnected momentarily from the case)
```

---
## \#6 Posted by: Ingvarjedi Posted at: 2018-06-28T06:30:01.605Z Reads: 38

```
How can I check the receiver and transmitter? it is very difficult


I see. The temperature is very small. Is it worth cooling?


I used Trampa with 200mm whells. can therefore large current surges
```

---
## \#7 Posted by: telnoi Posted at: 2018-06-28T07:26:23.199Z Reads: 35

```
[quote="Ingvarjedi, post:3, topic:60284"]
There was also a loss of power when driving to the hill,
[/quote]

That at least sounds like thermal throttling, especially if the board gradually gains power again after you reach the top. Are the vescs in an enclosure?

If the incline remains equal during a climb, there should be little reason for the board to slow down continuously if the thermal cutoff is not reached.
```

---
## \#8 Posted by: Ingvarjedi Posted at: 2018-06-28T08:45:31.122Z Reads: 31

```
Yes, after climbing, VESC is gaining strength again.

VESC is in a sealed plastic container
```

---
## \#9 Posted by: telnoi Posted at: 2018-06-29T05:08:54.950Z Reads: 21

```
Ok, airflow will most likely resolve your issues. If you can, add heatsinks to your vesc, but airflow is key.
```

---
