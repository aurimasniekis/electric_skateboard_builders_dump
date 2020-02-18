# VESC with Four Pole Motor

### Replies: 8 Views: 828

## \#1 Posted by: bdohler Posted at: 2017-07-14T00:54:08.869Z Reads: 120

```
Hi there,

I'm trying to spin up a 4-pole motor with the VESC for a different DIY project. I'm using @Ackmaniac's modified BLDC tool.  

When I run the calibration, the motor begins it's dance, and then about ten seconds later, the UI flashes with "Unknown Error" followed by "Disconnected"

In addition, when I try to use the arrow keys (with parameters that I already have with the motor, the motor begins to jerk back and forth with no smooth operation. 

Photos of the config settings:

<img src="/uploads/db1493/original/3X/8/5/859082957ac677d8738174015f93b102f40eb7c4.png" width="690" height="412">

<img src="/uploads/db1493/original/3X/e/5/e530fd5424c08e2c41d0a15b2729b0444028a8ec.png" width="690" height="412">

Let me know if it's possible to use a four pole motor, or if there's any additional information you need.

Thanks! 
Bdohler
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2017-07-14T21:34:32.826Z Reads: 74

```
Have u tried both bldc and foc? Im at work couldnt really tell the values in your images yet will look after work.. whats your 4pole motor diameter size again and battery? Looks like u tried foc have u tried bldc?? The arrow keys don't work with my motor etiher but dont affect ppm input that is fine

If calibration fails for foc, try bldc, of that fails use an esc or different vesc if u have
```

---
## \#3 Posted by: bdohler Posted at: 2017-07-14T21:56:31.075Z Reads: 70

```
BLDC screeches but spins at random RPM (different in either direction). FOC only dances jerkily. 15V motor at 15 A or so. I'm using a benchtop power supply at 14V with plenty of current. I will try the ppm input later. Tahnks!
```

---
## \#4 Posted by: mccloed Posted at: 2017-07-14T22:09:01.375Z Reads: 63

```
Might be an issue with the "Battery Cut off" start & end. I've noticed the VESC reads a bit lower than actual. Maybe try setting those lower for the 14v power supply?
```

---
## \#5 Posted by: trancejunkiexxl Posted at: 2017-07-15T02:27:50.969Z Reads: 49

```
Really interested in your progress cant wait to see it fixed!
```

---
## \#6 Posted by: bdohler Posted at: 2017-07-17T15:19:06.399Z Reads: 37

```
I've tried the same with setting the battery cutoff voltages to 0.0V and 0.0V, and had no luck. No other updates and not sure what else to try.
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2017-07-19T05:38:41.015Z Reads: 28

```
How are you powering again tried switching sources
```

---
## \#8 Posted by: trampa Posted at: 2017-07-19T06:23:29.205Z Reads: 26

```
The low pole count motors can be tricky. 
You should check the resistance and KV rating.
Motors with a low resistance can kill your HW 4.12 easily. With VESC Six two pole motors with low resistance and high KV worked just fine. This was actually one of the benchmark tests for the new HW/FW. The motor Benjamin used for testing killed the HW 4.12 in milliseconds, while VESC SIX was running it just fine at 150K ERPM.
Scorpion innrunner...
You could go to Benjamins Forum and ask your question there. Help is closer there.

Frank
```

---
