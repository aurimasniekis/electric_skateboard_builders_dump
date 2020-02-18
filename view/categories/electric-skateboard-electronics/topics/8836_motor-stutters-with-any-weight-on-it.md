# Motor stutters with any weight on it

### Replies: 6 Views: 1113

## \#1 Posted by: dylancook Posted at: 2016-09-03T02:18:04.040Z Reads: 138

```
I've rode over 60mies with my current setup and haven't had any problems, but today when I went to ride, If I try to accelerate, the motor kind of stutters. I hooked it up to my computer, and tried to find something out of the ordinary, but I can't seem to figure out why it's doing this. 

It spins perfectly fine with no weight on it(upside down). But if I hold the motor with my hand or try to ride, It stutters. 

another note.. when using the keyboard to control the motor, if i press up on the keyboard, the motor spins full speed, and I can hold it with my fingers and it stutters. But if I press right, the motor spins roughly half speed, and I cannot hold it with my hand. 

EDIT: The motor does have the strength to get me up to speed while ridding, but it stutters while doing so. Once I get to a speed, if I hold the throttle there, it doesn't stutter, but if I try to accelerate it does. I can take a video tomorrow if anyone wants one.

Setup:
batteries: 10S    5000mAh 5s LiPo x2 in series
motor: Turnigy SK3 149kv outrunner
enertion VESC

BLDC settings:
<img src="/uploads/db1493/original/2X/e/ebb1cd28f546cf08a1b263614bbe06b0c3189ceb.png" width="690" height="364"><img src="/uploads/db1493/original/2X/1/15c095cf7a681e190a8ea082b6fefa33e9dbb3e8.png" width="690" height="364"><img src="/uploads/db1493/original/2X/b/b396ef0a20a176d16df3b68d055bcbcbaa7fd172.png" width="690" height="364"><img src="/uploads/db1493/original/2X/a/a6db83cb1f91149e8dbe9493766c4bc8188755f4.png" width="690" height="364">
```

---
## \#2 Posted by: saul Posted at: 2016-09-03T03:06:08.386Z Reads: 119

```
You motor max amps is a bit low. I use 45a on 12s. Battery amps are very low. Should be the same as motor. Where else would the amps come from? 
I'm guessing the vesc is hitting your amp limit then cutting out, hence not enough torque which can cause stuttering.

Regen. Min amps seems low also.
```

---
## \#3 Posted by: alhow Posted at: 2018-03-30T03:24:21.331Z Reads: 57

```
I have this exact same problem.. Did you ever find a solution to your motor stuttering issue?
```

---
## \#4 Posted by: dg798 Posted at: 2018-03-30T03:29:00.476Z Reads: 54

```
Type faults into the terminal. Sometimes this can be a drv error or a shorter motor.
```

---
## \#5 Posted by: Jebe Posted at: 2018-03-30T03:31:25.195Z Reads: 54

```
check windings aren't shorting to motor frame
```

---
## \#6 Posted by: Acido Posted at: 2018-03-30T08:03:24.962Z Reads: 34

```
A phase wire has a bad connection or one of the windings has a broken wire
```

---
