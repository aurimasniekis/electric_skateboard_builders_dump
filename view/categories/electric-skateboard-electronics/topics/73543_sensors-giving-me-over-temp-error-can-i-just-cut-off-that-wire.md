# Sensors giving me over temp error, can i just cut off that wire?

### Replies: 5 Views: 141

## \#1 Posted by: Acido Posted at: 2018-11-05T16:28:34.696Z Reads: 48

```
So after troubleshooting a million problems with enertion, and fixing them i get this error that stops me from getting a detection in foc and bldc

I get all the other values except flux i think (the one where the motor spins)

So im wondering if i can just cut off that wire, I guess nothing should go wrong since it would be like sensorless 
There are motors without temp sensors right and they still work with vescs right?
```

---
## \#2 Posted by: marsrover001 Posted at: 2018-11-05T19:50:35.333Z Reads: 39

```
Seems alright to me. Though it seems like you could enter a different temp sensor offset value.

Then the other question is the temp sensor fully open or closed? That could be giving it a under or over temp reading.
```

---
## \#3 Posted by: Acido Posted at: 2018-11-05T19:53:36.834Z Reads: 36

```
that also may be the thing
also i friend my sensors on my old motor and that probably messed up the vesc or the sensor is not calibrated right...
```

---
## \#4 Posted by: Sender Posted at: 2018-11-05T19:57:09.778Z Reads: 37

```
I was get3timg some weird motor temp thermal throttling on a single Sk3 build and want to hack that wire as well.  Subscribed.
```

---
## \#5 Posted by: Acido Posted at: 2018-11-05T20:16:34.393Z Reads: 31

```
enertion told me that its on my own risk than but i doubt that anything can happen since i do not see the difference between sensored without temp and sensorless (temperature wise)

or we can just make an offset that thermal throttling starts on the temp we get+ 60 or whatever you want to set it too, but we would need to test if it detects heat change
```

---
