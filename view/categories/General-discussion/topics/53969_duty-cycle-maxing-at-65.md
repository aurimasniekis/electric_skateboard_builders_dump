# Duty Cycle Maxing at 65%

### Replies: 4 Views: 277

## \#1 Posted by: zhud Posted at: 2018-04-30T23:30:52.425Z Reads: 79

```
Batt Max: 30A
Motor Max: 80A

I'm not getting anywhere these max amps during my ride. 

65% duty cycle is the max at full throttle . Getting about 700 Watt max output total. Motor is rated for 80A, and about 2500W total, 4000W max. Battery is 10Ah rated at continuous 100A (this may be bullshit) and 200A peak current. The ERPM is set at 60000. It's and ebike, 8s, 33.6V max, geared 15/184, using thumb throttle with duty cycle.

Seems like I am getting around 50A max from the motor and about 22A max from the battery, but like I said, max of around 700W total. 

Just hoping to get some info on why this might be taking place.
```

---
## \#2 Posted by: Pedrodemio Posted at: 2018-05-01T01:06:08.158Z Reads: 59

```
Probably your motor has a Kv that would pass the 60k ERPM, so with that limit it will max out at 65%, duty cycle is proportional to ERPM
```

---
## \#3 Posted by: MysticalDork Posted at: 2018-05-01T01:08:07.266Z Reads: 57

```
Either that or the battery voltage is too low to force any more current through the motor.

Or there's just not enough load to force the motor to draw that much current.
```

---
## \#4 Posted by: professor_shartsis Posted at: 2018-05-01T03:26:34.795Z Reads: 40

```
do you have a graph?
```

---
