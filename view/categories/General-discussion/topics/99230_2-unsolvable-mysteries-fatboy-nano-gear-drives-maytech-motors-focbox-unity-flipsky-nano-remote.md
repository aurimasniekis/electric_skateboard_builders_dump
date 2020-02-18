# 2 unsolvable mysteries.. fatboy nano gear drives, maytech motors, focbox unity, flipsky nano remote

### Replies: 10 Views: 395

## \#1 Posted by: ju5t Posted at: 2019-07-28T00:03:52.147Z Reads: 118

```
![51%20(1)|690x388,75%](upload://1U9yovWWxNhOxrlc4ur4Dx8IoBz.jpeg) 
https://youtu.be/beYZeKoMyBg

So close to finishing my baby but i am getting 2 major issues.
I need a little assistance diagnosing and resolving these issues.

1- a cut out at full throttle within 1 second
(flipsky nano remote, focbox unity, maytech motors, fatboy nano gear drive)

2- excessive drag on 1 motor/gear drive.

here is video to show both issues.
for issue 2 i think its the gear drive as tightening down the gear drive caused the drag after the gears were perfectly meshed. I since removed and re-aligned them multiple times but cannot find a way where they fit without this rubbing. @Kug3lis any ideas? 

Or @mackann you've assembled hundreds of these any advice in troubleshooting?
```

---
## \#2 Posted by: goldrabe Posted at: 2019-07-28T01:54:07.302Z Reads: 102

```
I have no experience with the Flipsky Nano remote, but did you calibrate your remote in the highest speed setting? Calibrating your remote in lower settings can cause it to overshoot and cutout.\
When spinning your motors and gears by hand, is there a big difference in drag detectable by hand? If the difference is not too excessive it´s normal that one side stops earlier then the other on the bench. In real life usage e.g. on the street, you won´t see any difference.\
One thought though, have you put some grease under the V-ring?

Edit*\
I re watched your Video once more and the difference seems quite big. Check for correct spacer placement between the pulley and wheel. What happens if you back out the Axle nut by a bit that the wheel is still firm (not wobbling) but not completely tightened. You can try different bearing spacers inside the wheel and see if it gets better.
```

---
## \#3 Posted by: Deodand Posted at: 2019-07-28T02:02:58.737Z Reads: 96

```
Type "faults" command from the terminal in the unity app to see if that turns anything up.
```

---
## \#4 Posted by: Santino Posted at: 2019-07-28T02:36:24.213Z Reads: 92

```
Also check if you over tight  the wheel, maybe a speed ring is missing...Loose the wheel and try again...
```

---
## \#5 Posted by: mackann Posted at: 2019-07-28T07:54:24.397Z Reads: 73

```
1. Have you the newest unity firmware? Did you run calibration of the remote?

2. Is it the same resistant if you hand roll them? Is it the same if you remove the wheels and roll the motor by hand? Have you checked so motorpulley is close to the motor possible so its not scratching the gear case?
```

---
## \#6 Posted by: mackann Posted at: 2019-07-28T07:57:07.083Z Reads: 71

```
After cut out do not power off but do this : (push the ...) 
![ui|230x500](upload://hRFNDmMLeQtXSdIO2lE33HHz28I.jpeg) 

What does it say?
```

---
## \#7 Posted by: legend27 Posted at: 2019-07-28T08:07:56.523Z Reads: 62

```
I had somewhat the same problem with my gear drive. I fixed it by adding a small 0.45mm spacer between the cover and mounting plate. It turned out the gear was hitting the cover.

Try to unscrew the cover screws a tiny bit so you can move the cover a bit out. See if you still have the same issue when you pull the cover a bit out from the mounting plate

Can’t find the spacer rn but pretty sure @Riako designed it. 

I also noticed that the gears will loose up a bit after some usage (40km). Don’t think that’s the case for you though...
```

---
## \#8 Posted by: ju5t Posted at: 2019-07-28T16:56:58.429Z Reads: 44

```
no faults....

recalibrating the remote on the slower setting seemed to fix the cut out.

Think found 2 problems causing the "drag"/friction when mounting the wheels..

1- i used the spacer on 1 side from the original flywheel adaptors... this made it harder to fit everything on.

2- the keyway stick out the end of the motors 2mm i think was the problem too seems to have shaved a bit of the inner casing.
```

---
## \#9 Posted by: laurnts Posted at: 2019-07-28T17:43:31.877Z Reads: 37

```
I think its over current fault. If you throttle gently the issue is gone. It happened to me when I did too high gearing on my system.
```

---
## \#10 Posted by: Riako Posted at: 2019-07-31T17:10:02.479Z Reads: 17

```
https://www.thingiverse.com/thing:3437661

:v: ;)
```

---
