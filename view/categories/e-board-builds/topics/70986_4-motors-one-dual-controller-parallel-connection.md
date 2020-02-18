# 4 motors one dual controller (parallel connection)

### Replies: 10 Views: 301

## \#1 Posted by: TheGreekGuy Posted at: 2018-10-12T15:56:30.557Z Reads: 145

```
Hi I found that video 
https://www.youtube.com/watch?v=GcAoD5BuItc
in this video, this guy is connecting two motors parallel to one channel of the dual controller and two to the other channel .... apparently, this is possible!? will that mean that the motors are getting half the power? what is going on electronically? Can someone please explain?
```

---
## \#2 Posted by: professor_shartsis Posted at: 2018-10-12T16:39:42.392Z Reads: 128

```
are the motors brushed dc?
```

---
## \#3 Posted by: TowerCrisis Posted at: 2018-10-12T16:45:17.287Z Reads: 124

```
Is he connecting the left front to the left rear, and the right front to the right rear? That would make the most sense. As long as the motors stay in sync / are physically attached to each other then it should be doable. You can't do this with a normal dual rear drive since turning makes them spin at different rates, but with a left right setup then the wheels would always be in sync so long as you keep traction.
```

---
## \#4 Posted by: baxtred Posted at: 2018-10-12T17:03:44.877Z Reads: 118

```
I think the magnets need to be in the same location as well. Like at the same location between copper coils. So although those wheels are going to same speed, one wheel likely is lagging or leading between phases. The sin waves won't line up perfectly... Or at least that's my interpretation.
```

---
## \#5 Posted by: jasonbhuynh Posted at: 2018-10-12T17:12:14.751Z Reads: 109

```
Sounds like more trouble than it's worth...
```

---
## \#6 Posted by: TheGreekGuy Posted at: 2018-10-12T17:32:30.424Z Reads: 100

```
Well he indeed connects the left side together and the right side together.... but I see that he is not connecting the hal sensors also .... maybe that is the solution? can 2 motors (phase and hal) be connected in parallel?
```

---
## \#7 Posted by: b264 Posted at: 2018-10-12T20:31:13.437Z Reads: 79

```
This can only work with brushed DC motors, and not 3-phase AC motors / BLDC motors.
```

---
## \#8 Posted by: TheGreekGuy Posted at: 2018-10-12T21:30:27.351Z Reads: 70

```
If you watch the video you would see that these are BLDC motors that this guy is connecting... but he doesn't connect the Hal sensors of the motors
```

---
## \#9 Posted by: b264 Posted at: 2018-10-12T21:36:30.202Z Reads: 64

```
Then it will be *Extra Shitty* :registered: 

Good luck with range and power.  Also, it will run better on the bench than on an actual street.  Once the wheels are coupled together by the street surface, a lot of the power being supplied will be wasted braking the other motors that are accelerating.  If you ran it on ice, it would work better.
```

---
## \#10 Posted by: Okami Posted at: 2018-10-13T11:45:06.468Z Reads: 38

```
This guy in video is hardcore .. he even made his own baseplate and trucks :smiley:
```

---
