# Can a vesc be run on high kv with higher voltage

### Replies: 12 Views: 1134

## \#1 Posted by: willpark16 Posted at: 2016-12-16T06:05:19.577Z Reads: 121

```
If speed were limited to 22 mph on a 230-245kv motor on 10s would it not still be efficient? And is it even possible to do this with the vesc?
```

---
## \#2 Posted by: Iceni Posted at: 2016-12-16T11:09:37.031Z Reads: 109

```
I run 10s and 245-ish kv on mine (not sure about exact number since I rewound it) and it runs fine.
A bit on the fast side even with 13/36 gearing, so it's not as efficient as it could be.
```

---
## \#3 Posted by: willpark16 Posted at: 2016-12-16T14:48:01.308Z Reads: 97

```
U don't limit speed?
```

---
## \#4 Posted by: LukeL Posted at: 2016-12-16T16:42:09.224Z Reads: 88

```
The ERPM limit is basically a speed limit (the speed will be dependent on your gearing/wheel size/motor)

When you're not running at full throttle PWM is applied to the MOSFETs on the ESC, turning them on and off is inefficient (energy is lost when creating the channel from source to drain, due to parasitic capacitance that need to be charged/discharged).

But at top speed when there is more current flowing through the MOSFETs (which have a small resistance when on) they are dissapating more power and getting hotter which makes them less efficient.

so a system with 190kv may be more efficient but as you're changing speed a lot and unlikely to be going at top speed most of the time I don't think this is much to worry about, the ERPM blowing up the drv chip is a much bigger worry.

I am using a 10S 240kv setup and haven't had any issues.
```

---
## \#5 Posted by: willpark16 Posted at: 2016-12-16T17:23:42.960Z Reads: 69

```
vesc brand??
```

---
## \#6 Posted by: willpark16 Posted at: 2016-12-16T17:23:57.427Z Reads: 66

```
what tiype of vesc?
```

---
## \#7 Posted by: Iceni Posted at: 2016-12-16T17:39:49.405Z Reads: 64

```
Havn't bothered to set the speedlimit in the software, i just limit my finger :P

Using vescs from esk8.de
```

---
## \#8 Posted by: willpark16 Posted at: 2016-12-16T17:41:21.093Z Reads: 65

```
top speed youve chosen to reach?
```

---
## \#9 Posted by: LukeL Posted at: 2016-12-16T17:42:03.747Z Reads: 66

```
Mines enertion but shouldn't matter as long as it's from somewhere reputable
```

---
## \#10 Posted by: willpark16 Posted at: 2016-12-16T17:44:14.220Z Reads: 64

```
the vesc battle is a constant one but ive found that higher kv motors on higher voltages are running better on enertion vescs
```

---
## \#11 Posted by: Iceni Posted at: 2016-12-16T21:20:36.557Z Reads: 53

```
Generally keep around 25-35km/h, which for me is fast enough, especially in city environments.
```

---
## \#12 Posted by: Hummie Posted at: 2017-01-25T19:08:27.420Z Reads: 42

```
from what I can find it seems a higher kv motor might be more efficient in the motor as the current is better smoothed out but would likely create greater switching losses in the esc.

I'd like to see what the ripple is on an osiliscope.

http://electronics.stackexchange.com/questions/151713/how-to-compute-the-effective-voltage-across-a-dc-motor-driven-by-a-pulse-train
```

---
