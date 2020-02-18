# Sensor Wire Question

### Replies: 5 Views: 180

## \#1 Posted by: Skatejitsu Posted at: 2019-03-29T20:05:48.021Z Reads: 51

```
I am wiring Racestar motors to my Unity for the first time and have a question on the pin configuration.  5v and ground are clear, but Unity labels the other sensor wires "1, 2, 3" while Racestar labels them "U, V, W".  Which go to which?
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2019-03-29T20:09:13.416Z Reads: 51

```
It doesn't really matter, just connect them and you're fine just connect the 5v and gnd correctly and you're good
```

---
## \#3 Posted by: Skatejitsu Posted at: 2019-03-29T20:13:28.481Z Reads: 44

```
I knew the 3 heavier motor wires themselves can be connected in any order, but just to be sure we're talking about the same thing, the other 3 smaller wires in the plug itself don't matter either?  I would have thought they need to match up with the correct coil...or does the unity just "figure that out" when you run the setup?
```

---
## \#4 Posted by: dareno Posted at: 2019-03-29T20:25:22.529Z Reads: 43

```
Hall sensor order doesn't matter but the 5v and gnd have to be correct.  As @ARetardedPillow stated.
```

---
## \#5 Posted by: wafflejock Posted at: 2019-03-29T20:28:19.073Z Reads: 39

```
Just got a sensored motor myself for the first time and a new VESC (still 4.x hardware but old one was acting a little weird and no longer connecting over USB so figured replace it all at once).  The thicker wires are typically called the "phase wires" and carry power to the coils if you swap any two of the three the motor will run in the opposite direction (with the VESC configuration tool you may be able to reverse the motor without reversing cables but usually easy enough to swap two of the three), not sure about the sensor wire positions though.

Confirmation on order doesn't matter for sensor wires here: https://www.electric-skateboard.builders/t/hal-sensor-wire-pin-out/24502/9 VESC auto detects during motor detection.
```

---
