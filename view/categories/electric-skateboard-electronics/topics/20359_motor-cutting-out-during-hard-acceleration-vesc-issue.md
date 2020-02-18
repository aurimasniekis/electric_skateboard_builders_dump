# Motor cutting out during hard acceleration&hellip; VESC issue?

### Replies: 8 Views: 977

## \#1 Posted by: bluetree70 Posted at: 2017-04-05T16:06:30.130Z Reads: 115

```
I think something is wrong with either my setup or my VESC, help please.

Setup:
SK3 6463 190kv motor
VESC-X from Enertion
Space cell 3 pro

Problem: 
I have been riding this setup for around 3 weeks almost daily without any sort of problem with the electronics
with the following BLDC settings:
<img src="/uploads/db1493/original/3X/9/b/9b5ce18a44a9c11c8e259d7b2f608f09984937ed.png" width="689" height="379">
<img src="/uploads/db1493/original/3X/4/1/4112988d10779ff9bfe2a64c148af93ac270d652.png" width="690" height="357">
<img src="/uploads/db1493/original/3X/c/9/c9b3e778e7f25b02c0c4057185d3899a2c6a9fae.png" width="689" height="335">

Now after riding around, yesterday I figured I wanted to bump up the braking just a bit and changed the motor min(regen) up to -60amps. Wrote it and put everything back together and took it for a 20min ride and everything seemed fine. Now something really strange happened when when I turned on the battery this morning. I heard a small pop and a spark flew out of the motor. I tried accelerating up a hill and the motor cut off every time the load gets higher.

Hooked up my VESC to my PC and ran for faults. This is what I got:
<img src="/uploads/db1493/original/3X/0/2/02b0c66fa00312737aaa9c0b83d83000fef9a33a.png" width="690" height="371">

Well shit looks like I got a DRV failure. But something weird I noticed was the current looks really high for some reason. In all the threads with DRV failures it seemed like the current would be around 0. Does this mean my DRV isn't fried? What do I do if it isn't so that I can actually accelerate uphill?
```

---
## \#2 Posted by: rwxr Posted at: 2017-04-05T17:30:44.095Z Reads: 92

```
Sounds like the phase wires shorted...
```

---
## \#3 Posted by: bluetree70 Posted at: 2017-04-05T17:40:17.002Z Reads: 91

```
How can I tell? How did they get shorted? How can i fix this?
```

---
## \#4 Posted by: rwxr Posted at: 2017-04-05T18:18:34.565Z Reads: 87

```
Look over your cables. Probably broken insulation or something. Or crossing wires inside the motor
```

---
## \#5 Posted by: Stef Posted at: 2017-04-05T22:26:56.984Z Reads: 77

```
If a spark flew out of your motor then there is likely a short or intermittent contact in the motor.
```

---
## \#6 Posted by: bluetree70 Posted at: 2017-04-06T15:46:08.496Z Reads: 65

```
How do I fix it?
```

---
## \#7 Posted by: Stef Posted at: 2017-04-06T17:43:59.388Z Reads: 61

```
Try to isolate the problem first.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-04-07T03:03:48.466Z Reads: 53

```
Sounds like a short in the motor to me as well. Especially since you saw a spark inside the motor.
The bad news is that the motor short could have burned out the Drv chip.
Disconnect the motor from the vesc and turn the motor by hand. If it feels like the brakes are on, then you have a short.
Note: you could have an intermittent short and wiggling the phase wires while turning the motor might make it show up.
I would recommend just replacing the motor. ( preferably a motor designed for E-skate) There are numerous sources for these motors.
https://www.electric-skateboard.builders/t/johnny-vesc-repair-services-now-with-soldering-tips/11267
```

---
