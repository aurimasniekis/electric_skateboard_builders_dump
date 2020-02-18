# Dual Raptor, One motor constantly stuttering?

### Replies: 13 Views: 869

## \#1 Posted by: Drbrule Posted at: 2017-04-16T03:22:29.626Z Reads: 107

```
Hey everyone,

I'm having a problem with one of my motors, Yesterday i was riding home, and the board didn't feel right, so i got off, and one motor is constantly stuttering. Not just at takeoff, unrideable stuttering. 

I noticed it stuttering a bit more the last few weeks on takeoff, nothing too bad, I'm quite heavy 95-100kg, lots of steep hills and hard work for the board.

Testing the motors later, the stuttering motor will eventually get going if i give it full power, it will randomly stop stuttering and go full speed, but its unrideable at the moment.

I've left all the BLDC settings default and the board has been working perfect for the last 6 months.

I've been using the flysky GT2B remote. 

Anothing thing i just noticed, is my battery is showing, L 3, when it starts up not L10, and it says 100% charged even though i know its at least below 50%.


Any help would be much appreciated!


Thanks
```

---
## \#2 Posted by: Namasaki Posted at: 2017-04-16T06:53:42.987Z Reads: 94

```
The stuttering is likely caused by an intermittent poor connection between the vesc and motor.
If one of the phase wires disconnects, it will cause the motor to stutter.
Check the bullet connectors between the vesc and motor. Check the wires for damage. 
Check where the wires are soldered to the vesc. If none of these is the culprit, then you may have one of the phase wires coming loose in the motor.

As for your meter, There is a programing button switch on the meter that is likely getting bumped inside the battery pack.
I believe this is a common problem.
You'll need to get to the meter and re-program it.
```

---
## \#3 Posted by: Drbrule Posted at: 2017-04-16T09:19:54.693Z Reads: 85

```
Thanks Namasaki, Loose phase wire inside the motor is the culprit. i'll take it apart tomorrow and have a look!

Cheers
```

---
## \#4 Posted by: Jebe Posted at: 2017-04-16T11:38:30.082Z Reads: 79

```
<img src="/uploads/db1493/original/3X/e/5/e54daebcbceeab9e6d734445e5233161b5125d07.JPG" width="690" height="388">
```

---
## \#5 Posted by: Adam0311 Posted at: 2017-04-16T14:50:59.956Z Reads: 68

```
check for shorts in the windings while you have the motor disassembled. I've had it with two of my Enertion motors. Liquid electrical tape has been my fix, held up for few hundred miles so far.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-04-16T16:26:35.553Z Reads: 66

```
It is very fortunate that it did not short out. That would have killed the Vesc's DRV chip.
```

---
## \#7 Posted by: Drbrule Posted at: 2017-04-22T01:36:19.698Z Reads: 53

```
Hey, 

I'm having some trouble getting the cog off my motor? 

Circlip is off, and the alan key locking screw, is there something im not doing?
```

---
## \#8 Posted by: Jebe Posted at: 2017-04-22T01:48:59.846Z Reads: 54

```
try a heat gun
```

---
## \#9 Posted by: Drbrule Posted at: 2017-04-22T03:13:23.620Z Reads: 53

```
Should it just slide straight off
```

---
## \#10 Posted by: Jebe Posted at: 2017-04-22T03:26:25.037Z Reads: 53

```
If a pulley retaining compound was used it will take some removing still.
Try heating it.
```

---
## \#11 Posted by: CamBo Posted at: 2017-04-22T04:19:35.899Z Reads: 49

```
+1 for shorts in the windings.  I developed the same symptoms on both my raptor motors.  It appears that the coating that insulates the wires and holds them in place inside the can prior to the winding fails.  Resolved by adding additional heat shrink around the wires after they enter the motor.     Now they run good as new.
```

---
## \#12 Posted by: CamBo Posted at: 2017-04-22T04:21:57.359Z Reads: 48

```
Full thread here
https://www.electric-skateboard.builders/t/r-spec-shorted-phase-wire-problem-solution/6474/56

Worked great for me
```

---
## \#13 Posted by: Drbrule Posted at: 2017-04-22T08:38:06.014Z Reads: 40

```
Yeah thanks, I've been trying to get the motor apart this afternoon to have a look and a clean, 

but the little piece of metal that locks the pulley cog into the shaft of the motor, is stuck in the shaft, really stuck, i got my other good motor apart no problem, because i plan to heat shrink both now while they're apart.

I'll try it again tomorrow, any suggestions would be much appreciated.
```

---
