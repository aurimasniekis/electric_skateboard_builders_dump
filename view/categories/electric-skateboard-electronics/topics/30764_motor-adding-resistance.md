# Motor adding resistance

### Replies: 6 Views: 416

## \#1 Posted by: chewydinosaurs Posted at: 2017-08-16T02:47:11.987Z Reads: 69

```
I assume it's a vesc setting as Ive been playing around with them but for some reason when powered on the motor is resisting rotation unless throttle is given. So much resistance that you cannot manually push the board unless you give it throttle. What would this be? <img src="/uploads/db1493/original/3X/8/8/881ae16852cb1b54ccef78ac52c91b26796d347a.PNG" width="690" height="353">
```

---
## \#2 Posted by: jammin Posted at: 2017-08-16T02:52:51.541Z Reads: 62

```
Are you using a hub motor or satellite (belts / pulleys) motor? With belts and pulleys there is considerable drag that is pretty noticeable.

You <i>could</i> try messing around with the throttle trim under App Config to get it into a sweetspot (would only work moving forward), but I wouldn't recommend it...
```

---
## \#3 Posted by: chewydinosaurs Posted at: 2017-08-16T03:09:26.287Z Reads: 59

```
it's a satellite motor, it kicks in only after I give it some throttle. I'll play around with the settings in the throttle since I'm assuming that's what it's gonna be, but ive never had this issue until I switched over to the torque board mini controller.
```

---
## \#4 Posted by: jammin Posted at: 2017-08-16T03:16:34.991Z Reads: 55

```
did you calibrate the throttle trim after you switched remotes?
```

---
## \#5 Posted by: saul Posted at: 2017-08-16T03:17:21.593Z Reads: 49

```
99% sure this is a side effect of the remote issue.. fix that. this will go away.
```

---
## \#6 Posted by: chewydinosaurs Posted at: 2017-08-17T00:49:57.836Z Reads: 27

```
Yep the reading left it at 50% so it was still fine, so far it looks like the issue was one of the trims on the remote was not centered (although a pairing video between the receiver and transmitter said to turn the trim). I guess you could say that adjusting that trim knob kind of acts like a parking break.
```

---
