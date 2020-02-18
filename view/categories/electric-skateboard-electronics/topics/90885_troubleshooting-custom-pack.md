# Troubleshooting custom pack

### Replies: 6 Views: 126

## \#1 Posted by: killaton Posted at: 2019-04-17T15:48:17.245Z Reads: 48

```
I  just built (my first) 8s2p pack using the vruzend 2.0 kit and supower bms. I tested all the cells before building, and the voltage for every group checks out. The voltage at the xt60 reads 30.5V when bms is off and  33V when its on (weird?). However when i swap it with my current(factory) pack the VESC fails to power on. The blue led starts blinking more frequently, but no other signs of life.

I momentarily shorted the pack during the build, but it seemed to have had no impact besides a small spark, voltages remained nearly same on all cells.


How do I go about troubleshooting this pack?
```

---
## \#2 Posted by: RedBaron Posted at: 2019-04-17T15:55:05.726Z Reads: 48

```
Pictures might help. Was the bms connected when you shorted the pack? It is weird you're getting a 3v difference when the bms is on vs off.
```

---
## \#3 Posted by: killaton Posted at: 2019-04-17T16:00:50.591Z Reads: 44

```
I had the b- wire connected and was connecting the bms leads when i briefly bridged the plus and minus terminals of the whole pack.

https://photos.app.goo.gl/uUaLwfczQvd5PVBi6
```

---
## \#4 Posted by: RedBaron Posted at: 2019-04-17T16:06:28.705Z Reads: 39

```
Ah, most likely fried bms. Never have anything connected to the bms when you're messing with any of the leads. Finish and tripple check all leads then connect the bms.
```

---
## \#6 Posted by: killaton Posted at: 2019-04-17T17:00:38.383Z Reads: 33

```
I just soldered on another xt60 bypassing the bms... everything works.
The BMS has no burnt components and was not part of a closed circuit when i shorted the battery, how could it get damaged?
```

---
## \#7 Posted by: RedBaron Posted at: 2019-04-18T06:26:47.232Z Reads: 14

```
So your leads weren't wrong before you connected them to the bms? Either way if the vesc works when you bypassed the bms then your bms is still the problem. Im thinking one of a two things happened. 1 the bms was a dud from the factory or 2 your balance leads where incorrect. I've burned two bms's by having two balance leads in the wrong pins both had the same issues, flickering lights to cutout.
```

---
