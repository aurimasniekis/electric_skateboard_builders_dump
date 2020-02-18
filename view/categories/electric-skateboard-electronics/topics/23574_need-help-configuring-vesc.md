# Need Help Configuring VESC

### Replies: 9 Views: 570

## \#1 Posted by: mm6ix Posted at: 2017-05-20T21:36:42.162Z Reads: 33

```
I'm running a 170 kv sensor-less 6364 motor. 
10s3p Samsung 25r, discharging through bms.
Maytech VESC

These are my settings so far, just want to confirm that everything is okay before I apply any changes:  

<img src="/uploads/db1493/original/3X/f/4/f4ad01871e5b85dbef9d944b49592d74d7910227.png" width="690" height="364">

<img src="/uploads/db1493/original/3X/6/d/6dcdda2b31c7f81e303f9e7250cd6f550552efa4.png" width="690" height="362">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-05-20T21:55:55.707Z Reads: 28

```
Are you sure your battery can handle 20a regent charge?
```

---
## \#3 Posted by: mm6ix Posted at: 2017-05-20T21:57:23.554Z Reads: 28

```
Not sure, what determines the regen value? 

The 20a in the regen box was just the default value.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-05-20T22:02:00.864Z Reads: 27

```
Unless I'm mistaken batt min -20 means 20a charge to the battery while braking but probably only that much if braking hard. 
But I'm no expert about Vescs do maybe someone who is can clarify.
```

---
## \#5 Posted by: mm6ix Posted at: 2017-05-20T22:05:39.878Z Reads: 26

```
hmm, the charger that came with the battery is a 2a charger. So maybe regen should be 2A as well?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-20T22:05:58.451Z Reads: 27

```
Specs for Samsung 25R
Flat Top.
Nominal capacity: 2500 mah.
Max Continuous Rated Discharge: 25 amps (at 25 degrees C)
Nominal voltage: 3.6v.
After a fresh charge: 4.2v.
Cycle info: Capacity drops to 60% after 250 full charge/discharge Cycles.
Don't discharge below: 2.5v.
Standard Charge: CC/CV @ 1 amp / 4.20 volts +/- .05v, 100 mA cut-off.

1C would be 7.5a
I don't know what the safe max would be
```

---
## \#7 Posted by: mm6ix Posted at: 2017-05-20T22:26:44.873Z Reads: 27

```
Thanks for the help! 

Hopefully someone with a similar set up or a VESC expert chimes in. Got any ideas of anyone that would know?
```

---
## \#8 Posted by: Namasaki Posted at: 2017-05-20T22:28:34.320Z Reads: 25

```
I searched a little and I think the max charge for 25R's is 4a per parallel group which means 12a for a 3p pack.
You could ask in the live feed what the max regen charge rate is for 25Rs
```

---
## \#9 Posted by: mm6ix Posted at: 2017-05-20T22:29:52.001Z Reads: 24

```
I'll set it to 10 amps and try asking in the live feed.
```

---
