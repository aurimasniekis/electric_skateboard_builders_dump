# Focbox unity dual drive issue

### Replies: 13 Views: 625

## \#1 Posted by: JKUK Posted at: 2019-05-11T18:06:01.910Z Reads: 177

```
Hello

I've got an issue where one motor goes faster than the other. The other eventually catches up when going full throttle but as you can see in the diagram not when just accelerating normally.

Any ideas what this could be ?

![Screenshot_20190511-184902|236x500](upload://eTfDHl5KUR9srmPdRLTe7q3FVmg.jpeg)
```

---
## \#2 Posted by: rusins Posted at: 2019-05-11T19:42:43.191Z Reads: 165

```
Do you feel any difference in the resistance the motors give when spinning their cans just by hand? It could be due to different belt tensions, but this is quite extreme.
```

---
## \#3 Posted by: L3chef Posted at: 2019-05-11T20:15:30.917Z Reads: 164

```
You might get the help needed over at this thread.
https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861
```

---
## \#4 Posted by: JKUK Posted at: 2019-05-12T17:05:16.649Z Reads: 145

```
I loosened the black screws and let the belt have a bit of slack. That seemed to help slightly but still a fair bit of difference. Any thing else I could adjust?

![IMG_20190512_180250|375x500](upload://eZ01TiiQaubuqr8kTE6jHms3qjg.jpeg) 

What does the mwb mean in the diagram below? As they look different.
![Screenshot_20190512-180218|236x500](upload://qFKFTLAgIzE239mKQ2AhvHgkaIk.jpeg)
```

---
## \#5 Posted by: CarlCollins Posted at: 2019-05-12T18:00:53.648Z Reads: 136

```
Have you tried this 
When doing detection
make sure of the following
1: When software ask you to roll the motors with your hand, roll them
2: In the forward direction.
3: Single time
4: As hard as you can
5: Both together

I hope this will fix it
```

---
## \#6 Posted by: Deodand Posted at: 2019-05-12T18:04:49.578Z Reads: 133

```
Calibration looks fine I'd just turn up motor amps. Does seem like a an awful lot of friction difference if 4 amps causes that big of difference. 

You could also turn on traction control in the advanced motor settings...

The mwb numbers is mwb its mathematically related to the kv of the motor and the number of motor poles. A small amount of variance isn't surprising.
```

---
## \#7 Posted by: JKUK Posted at: 2019-05-12T20:22:34.198Z Reads: 129

```
I didn't do both at the same time, do I need to?

I've done one at a time before and same result.

Okay I will try traction control, what will it do?
```

---
## \#8 Posted by: CarlCollins Posted at: 2019-05-14T20:05:27.148Z Reads: 111

```
I think you need to do that
```

---
## \#9 Posted by: JKUK Posted at: 2019-05-19T08:47:06.743Z Reads: 91

```
Turning on traction control fixed the issue. They are perfectly synced now.

I'm having major torque however, what's the best way of lowering the torque/acceleration? 50% of what it is would be perfect
```

---
## \#10 Posted by: McErono Posted at: 2019-05-19T09:55:14.179Z Reads: 79

```
So you are not on motor max 10amp anymore are you? What remote you got?
```

---
## \#11 Posted by: JKUK Posted at: 2019-05-19T11:09:39.375Z Reads: 76

```
Nope changed to 60 and -60 which was defaults now. Got the nano x remote. What you think I should change?
```

---
## \#12 Posted by: McErono Posted at: 2019-05-19T12:04:44.443Z Reads: 75

```
ok. make sure you calibrate the remote everytime before you turn on the board (full throttle, full brake). without calibration the remote only sends full throttle, full brakes no matter your input on the remote. then just play with the motor max settings until you are happy. maybe start with 40amps.

max motor current - most motors do 80amps but start with 40 or even 30. it does increase torque the higher you go.

max battery discharge current - most good batteries use samsung 30q cells at the moment and they are rated at 15amps - so lets say you got a 12s4p battery you multiply the parallel cell count (4p) with the 15amps = 60amps battery max.

max braking regen current - does affect the brakes at highspeed. your battery is safe to take 4amps per parallel cell so 4p equals -16amps regen current (its a minus value). lower the value for weaker brakes.

max brake current - does affect low speed braking. basevalue is the 60amps from the max battery discharge current. if you need smoother brakes set a lower value like 50amps here.
```

---
## \#13 Posted by: JKUK Posted at: 2019-05-21T20:47:12.034Z Reads: 51

```
Thanks dude
```

---
