# BEMF Coupling and cycle integrator limits with two torqueboard 6355 motors

### Replies: 10 Views: 370

## \#1 Posted by: RazzleDazzle Posted at: 2018-11-30T18:48:53.490Z Reads: 89

```
So i ran the detection for each of my motors and the BEMF coupling and cycle integrator settings are slightly different, is that a cause for concern?
```

---
## \#2 Posted by: Pedrodemio Posted at: 2018-11-30T19:16:48.175Z Reads: 84

```
No problems, no two motors are equal, you probably will get slight different values if you run the detection again on the same motor
```

---
## \#3 Posted by: RazzleDazzle Posted at: 2018-11-30T19:18:43.290Z Reads: 85

```
That def did hapen which made me scratch my head, alas, the values arent too far off.  Also, is it "normal" if one motor starts a few milliseconds before the other?  I noticed one wheel also stops slightly before the other and it varies from time to time.  Im probably over analyzing a bit.
```

---
## \#4 Posted by: Pedrodemio Posted at: 2018-11-30T20:45:38.316Z Reads: 65

```
Yeah, are you using CAN bus? But it’s all normal, booth sides have different belt tension, the bearings aren’t exactly the same and so on
```

---
## \#5 Posted by: mtuan293 Posted at: 2018-11-30T20:56:38.191Z Reads: 52

```
What I do to avoid triggering my OCD:
1. Run motor detection on one motor, hit “Write motor configuration”. 
2. Then hit “Read motor configuration” so all the values are now present on vesc-tool and should be correct from the detection you did. 
3. Plug in the other vesc, hit “Write motor configuration”. Now both vesc should share the indentical motor detection values.

Obviously you should do this when you have a dual setup that uses 2 same motors.
```

---
## \#6 Posted by: Pedrodemio Posted at: 2018-12-01T12:46:55.700Z Reads: 42

```
It would be better to do the detection on both motors, as I said, no two motors are equal, even the same model, any quality motors should be really close that the uncertainty of the detection is higher than the variance between motors, but if somehow they are really different, you will have problems, I could just not spin or if you push you could kill your VESC, again, that’s an extreme case that’s unlikely to happen, but it’s good practice
```

---
## \#7 Posted by: Sn4pz Posted at: 2018-12-01T14:55:09.422Z Reads: 42

```
Its normal if the motors are unloaded to start unevenly sometimes, try it in a real world environment
```

---
## \#8 Posted by: mtuan293 Posted at: 2018-12-01T20:32:30.620Z Reads: 34

```
Well yeah definitely no two motors are identical. But I think the variation between the two motors is the same as the variation every time you do a new detection. So I’d just do detection once, because you’d get values within that variation if you detect each motor individually anyway.
```

---
## \#9 Posted by: pat.speed Posted at: 2018-12-02T00:00:36.692Z Reads: 30

```
I think this is just asking for a drv error, the other problem is that one motor could have a fault and since you didn’t do a proper motor detection you aren’t going to know until it’s too late
```

---
## \#10 Posted by: Friskies Posted at: 2018-12-02T09:24:37.230Z Reads: 17

```
People balance wheels Individually on cars even though they come from the same machines and process. Motors are no different, this is before you even think about different resistance levels from the rest of the drive train - wiring, belt tension, bearings etc etc. 

TL:DR - No two drive trains are the same. Run detection on a per motor/controller basis. The detection of tests will always be different :slight_smile:
```

---
