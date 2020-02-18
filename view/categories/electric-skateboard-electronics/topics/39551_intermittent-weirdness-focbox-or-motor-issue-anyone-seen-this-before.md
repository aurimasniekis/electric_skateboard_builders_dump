# Intermittent weirdness - FOCBOX or Motor issue? anyone seen this before?

### Replies: 8 Views: 495

## \#1 Posted by: DavidBanner Posted at: 2017-11-28T17:06:16.646Z Reads: 90

```
I have had an issue appear and I'm wondering has anyone seen this happen before?

When hitting full throttle its taking a few seconds for the motor to spin up properly every now and then.

The video below is me hitting full throttle, then the brake each time. Doesn't seem to be just cogging...

[https://www.youtube.com/watch?v=dN8K9zCQvvQ](https://www.youtube.com/watch?v=dN8K9zCQvvQ)
```

---
## \#2 Posted by: barajabali Posted at: 2017-11-28T17:08:54.236Z Reads: 88

```
Are you running sensors? FOC? FOC without load or sensors can do that
```

---
## \#3 Posted by: DavidBanner Posted at: 2017-11-28T17:10:44.311Z Reads: 87

```
Ah-ha - yes that motor is sensorless, and running FOC.

Thanks @barajabali looks like I have my answer...

That board has had some issues with the RX recently so I am being super cautious and looking for any indications of other trouble.
```

---
## \#4 Posted by: barajabali Posted at: 2017-11-28T17:11:26.107Z Reads: 85

```
No problem, Yea its good to be cautious with these things but you should be okay :)
```

---
## \#5 Posted by: DavidBanner Posted at: 2017-11-28T17:13:14.511Z Reads: 85

```
Indeed, the failsafe on the RX somehow reset and stopped working, it decided full throttle was the best course of action when losing connection :fearful:
```

---
## \#6 Posted by: Deckoz Posted at: 2017-11-28T17:35:29.200Z Reads: 79

```
Ive seen this behavior in 2.18 and 2.54. It happens if you dont calibrate the remote before powering the board.basically the ppm stream is outside of the calibrated pulse width and the vesc goes full throttle and stops. This seems to only be a behavior in FOC.

Normally this can be fixed by turning on the remote, moving the throttle to full and then full brake atleast one time. Then powering on the board.
```

---
## \#7 Posted by: DavidBanner Posted at: 2017-11-28T18:02:40.405Z Reads: 71

```
@Deckoz good to know - thanks for the heads up!

I am now doing a failsafe check every time I power on before I step on the board.
```

---
## \#8 Posted by: Deckoz Posted at: 2017-11-28T18:07:28.150Z Reads: 64

```
Yep...it behaves like a failsafe...but that's cause its the ppm stream out side of the pulse width. 

As long as you set your end points, center point and deadband, and calibrate the remote by doing a full throw before powering the board you should be good. 

Good luck ;)
```

---
