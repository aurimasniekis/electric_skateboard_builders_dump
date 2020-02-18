# Dual ESCapes: uneven motor speed

### Replies: 17 Views: 483

## \#1 Posted by: janpom Posted at: 2018-11-17T14:49:26.597Z Reads: 145

```
I started noticing a weird issue on my eMTB with dual ESCapes. When I put the board on a bench and run it, one of the motors spins much faster than the other one. I tried swapping the motor/ESC connection (connected motor A to VESC B and vice versa) and the problem reversed. So it seems as if one of the ESCapes (the master one) delivers less power than the other one. I also tried swapping master/slave and that still didn't change anything. The slave (former master) still spinned the motor slower than the other ESC. Any ideas where the problem could be and/or how to best debug it?

I thought that there's a problem in the wires between the ESCapes and the battery, which could cause that one of the ESCs is not getting enough juice, but when I thought about it some more, that actually seems very unlikely since the wheels are spinning freely with no load and thus the ESCs only draw about 1-2 amps.
```

---
## \#2 Posted by: hiboute Posted at: 2018-11-17T15:45:22.261Z Reads: 139

```
Is traction control activated?
```

---
## \#3 Posted by: janpom Posted at: 2018-11-17T15:55:23.493Z Reads: 136

```
Good question. No, I had it disabled. I tried enabling it now and that reduced the problem.

I also tried to put a little resistance on the faster motor by pressing on the wheel with my hand. Turned out it requires fairly little resistance to achieve balance in the motors speed. I guess this is not a big deal after all. Spinning the wheels freely probably makes the problem look bigger than it actually is.

I'm still surprised that one of the ESCs clearly delivers more power than the other one. This remains true even if I use exactly the same settings for both motors.
```

---
## \#4 Posted by: Trdolan03 Posted at: 2018-11-17T16:08:04.802Z Reads: 120

```
The speeds won’t be accurate on a bench test. Try riding it at low speeds to test
```

---
## \#5 Posted by: janpom Posted at: 2018-11-17T16:12:17.103Z Reads: 118

```
I'm afraid I don't understand how that helps. If I ride it, the wheels and thus the motors will rotate at the same speed.
```

---
## \#6 Posted by: Trdolan03 Posted at: 2018-11-17T16:23:24.714Z Reads: 110

```
Apply some throttle. If it is really different the board will “push” from the right or left
```

---
## \#7 Posted by: Trdolan03 Posted at: 2018-11-17T16:24:16.599Z Reads: 110

```
Other thing to check would be the erpm limit on each side
```

---
## \#8 Posted by: Jmding Posted at: 2018-11-17T16:30:06.182Z Reads: 111

```
With vesc, by default throttle controls current, not speed. So on a bench, if you apply the same current to both motors, if one has slightly more friction in the drive train than the other, it will spin more slowly. On the road, this differential won't matter at all since your drive train resistance will be negligible compare to your bodyweight inertia.

Or at least, that's the most likely explanation. Hence the suggestion to test it on the road at low speed.
```

---
## \#9 Posted by: Sender Posted at: 2018-11-17T16:30:44.237Z Reads: 107

```
Well put

&nbsp;
```

---
## \#10 Posted by: janpom Posted at: 2018-11-17T17:16:45.583Z Reads: 84

```
As I said, I tried swapping the motors. If the friction in the motor was the culprit of the different speed, it would still be the same motor that rotates more slowly, but that wasn't the case. It's always the same ESC that delivers less speed, regardless of which motor I connect to it.
```

---
## \#11 Posted by: janpom Posted at: 2018-11-17T18:13:12.244Z Reads: 80

```
Other than that, what you say makes a lot of sense though. I was actually trying to say something along the same lines with:

[quote="janpom, post:3, topic:74996"]
Turned out it requires fairly little resistance to achieve balance in the motors speed. I guess this is not a big deal after all. Spinning the wheels freely probably makes the problem look bigger than it actually is.
[/quote]

... but you phrased it much more clearly. Thanks!
```

---
## \#12 Posted by: Jmding Posted at: 2018-11-17T21:08:43.172Z Reads: 67

```
Could be a slightly misaligned belt, different  bearings, different mass of wheels etc. Did  you try riding it yet?
```

---
## \#13 Posted by: janpom Posted at: 2018-11-17T21:18:56.535Z Reads: 63

```
I did. It's actually OK when riding. I was just surprised that there's a difference in speed when the wheels spin freely. I tried that before and never noticed it. Something must have changed.

I still feel like my main point is being missed. I probably haven't been able to express myself clearly. Let me try again. I have two motors MA and MB, and two ESCs EA and EB. Now, whichever motor I connect to the EA, that motor spins more slowly. So it's not like MA is always the slower one or MB is always the slower one. I guess that pretty much rules out any mechanical problem.
```

---
## \#14 Posted by: Trdolan03 Posted at: 2018-11-17T21:20:51.425Z Reads: 61

```
I would just triple check that the setting on both esc are identical
```

---
## \#15 Posted by: dareno Posted at: 2018-11-17T21:53:01.184Z Reads: 54

```
If its a considerable difference then you would notice it riding at slow speed to fast.  If its not you won't.  This said it does seem that there is an issue with that particular vesc.  Especially if it is a new occurrence and not something thats always been there.  You could try running it single drive with each vesc to see the difference in performance.  That will give you a real world test.  Pain to go through all that configuration change though.  Obviously be careful of the canbus when disconnecting though.  Not sure the canbus issue is there with the esccapes but just in case.
```

---
## \#16 Posted by: Jmding Posted at: 2018-11-17T23:24:34.257Z Reads: 47

```
Thematically similar explanation is possible. Tolerances in the circuit components causing one esc to measure currents slightly higher than the other, so when it targets x amps, it delivers slightly lower than that number, resulting in slightly lower motor speed?
```

---
## \#17 Posted by: janpom Posted at: 2018-11-17T23:29:47.382Z Reads: 43

```
Yeah, that does make sense. I'll go with that explanation and stop worrying about it. Thanks!
```

---
