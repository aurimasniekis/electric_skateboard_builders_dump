# Connectivity issues / Intermittent braking - Need advice

### Replies: 10 Views: 720

## \#1 Posted by: tilmnater Posted at: 2017-03-12T23:37:02.685Z Reads: 49

```
I'm kind of at a loss right now. I can't figure out why I'm all of a sudden having connectivity issues. Now it's to the point that whenever I apply throttle, it will cut out on me after a second. After this occurs, if I try apply throttle again the motor gets glitchy, slightly applying the brakes/locking up for a split second. My guess is it has something to do with the motor. Maybe the internal wires are shorting or something. I really don't think it's the remote at this point, but I will definitely look into it further. Fyi, It's a Steez remote - pretty much brand new. I did recently change a few of the Vesc settings, which were as follows: Motor tab: Unchecked Limit erpm with negative torque, set max erpm to 60k, PPM tab: erpm limit start to 58k, erpm limit end to 60k, min/max pulsewidth to match what display was showing. Also, changed motor/batt min (regen) to 30/-30 to ease up brakes. It's set as current no reverse with brake.

Any help would be greatly appreciated. Thanks much!
```

---
## \#2 Posted by: mmaner Posted at: 2017-03-12T23:38:47.289Z Reads: 46

```
I would suggest you check the solder points between the VESC and motor, sounds like you might have a cold one with the breaks and throttle acting up.
```

---
## \#3 Posted by: tilmnater Posted at: 2017-03-13T00:09:33.483Z Reads: 39

```
Thanks for the quick response. Are you talking about solder points on the actual VESC or within the bullet connectors that connect it to the motor?
```

---
## \#4 Posted by: saul Posted at: 2017-03-13T00:34:25.057Z Reads: 35

```
Sounds like it could be an radio issue. Use safestart and a deadzone of at least .2-.3.
But make sure the range is centered.
```

---
## \#5 Posted by: tilmnater Posted at: 2017-03-13T00:39:00.968Z Reads: 37

```
Are these settings inside the BLDC tool? If so, can you please elaborate? This is the first I am hearing about them. Thanks!
```

---
## \#6 Posted by: mmaner Posted at: 2017-03-13T00:40:09.696Z Reads: 38

```
[quote="tilmnater, post:3, topic:18970"]
Are you talking about solder points on the actual VESC or within the bullet connectors that connect it to the motor?
[/quote]

The bullet or xt connectors from the VESC to the motor, and the points in the VESC where the phase wires begin.
```

---
## \#7 Posted by: saul Posted at: 2017-03-13T00:42:35.748Z Reads: 36

```
Yes. On the ppm tab.
Right in the middle.

I would run motor detection again too. I've had vesc reset randomly.( Maybe I tapped the wrong button?)
But it would cause the motor to stop after a sec...
```

---
## \#8 Posted by: tilmnater Posted at: 2017-03-13T23:45:43.189Z Reads: 26

```
Strange, everything looks good. Still have a couple more places to check but I'm stumped. Still wondering if the motor wires could be at fault here. Could there possibly be a short where they meet up inside the motor? Was thinking about replacing them with some silicone wire.
```

---
## \#9 Posted by: tilmnater Posted at: 2017-03-15T23:43:06.757Z Reads: 19

```
@mmaner @saul Looks like I found the culprit. Bad solder on motor or vesc bullet connector. We shall see if this fixes the problem. Thanks again for you input.<img src="/uploads/db1493/original/3X/a/3/a39384fcbe8096d6531b54fe5b35276651f05f69.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/4/f/4f5fef4025ef822ae3622b1a670901d726ae0e59.jpg" width="666" height="500">
```

---
## \#10 Posted by: mmaner Posted at: 2017-03-15T23:44:21.792Z Reads: 18

```
Good job.  I would go ahead resolder all of the phase wire connectors, both sides.  If one was solderd bad it's likely others were as well.
```

---
