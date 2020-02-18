# How vsec can control acceleration

### Replies: 3 Views: 1066

## \#1 Posted by: anoop54 Posted at: 2017-03-04T08:18:09.952Z Reads: 106

```
Hey I wanted to know how acceleration was controlled on the vsec? My assumption is that by setting the motor current lower torque will decrease meaning it will take longer to hit top speed. Is there any other way? 
Im asking this because it feels like riding the board is way too unsmooth.
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-03-04T11:51:35.836Z Reads: 94

```
Give my firmware mod a try.
You should try watt control and adjust the throttle curve. That will make your board much more controllable.
More info here

http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#3 Posted by: rpn314 Posted at: 2017-03-04T14:48:15.220Z Reads: 67

```
There's a few things that go into controlling the acceleration. There's a few values that can be changed in BLDC Tool: the Max Current is one and I think "Speed Ramp Limit Step" and maybe "Duty Ramp Step". It would be fiddling with some numbers around there (just don't quote me on the last two, I can't remember right now).

However @Ackmaniac has created a better overall solution for your exact issue, so I'd go with that :)
```

---
