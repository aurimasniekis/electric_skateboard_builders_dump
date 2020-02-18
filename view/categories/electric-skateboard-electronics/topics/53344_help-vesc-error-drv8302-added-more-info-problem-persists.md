# \[HELP\] Vesc error drv8302: Added more INFO, problem persists

### Replies: 8 Views: 448

## \#1 Posted by: TehAtheist Posted at: 2018-04-24T14:40:59.530Z Reads: 72

```
Hi,

Since recently my board has been throwing DRV8302 error in the first minute of riding, after that it's **entirely fine**.
Anyone knows why? I've got the most recent firmware and 4.12 hardware.
It just stops accelerating for a second when I'm getting the error but it does concern me.

![image|281x500](upload://7D2tb6ak06GGlz1Y9CD9ttHmfrj.jpg)



**Edit: Adding more info, updated firmware to 3.38 and problem was gone for a ride, but now it's back again...**

This is a  metr.at graph, that shows the start of a run with multiple DRV8302 faults in a very short timeframe. The second one is after a restart, riding to where I had to go.

https://metr.at/r/Z1e0N

https://metr.at/r/GECXv

These are my settings:

Motor Settings GENERAL:
![image|690x346](upload://1bzBZ1O7GniuKTMzKkIPPDHnf8e.png)
![image|690x347](upload://blL4g11PWf3hbixESJh4LYZAck7.png)
![image|690x346](upload://mnNkOm8vEF0tgVKK2IhA289lH86.png)
![image|690x346](upload://cMXN9zLcfBEpqB2Ifk9DZOc0NTa.png)
![image|690x346](upload://5PhwboDzCzwNSYFt9PCwqUBNZVa.png)
![image|690x346](upload://5sl8kwuUAQ3yaVeEv3TCBeQgI8B.png)

Motor Settings BLDC:
![image|690x346](upload://2LduWfupEafEmzALAxQLDhMUhIa.png)
![image|690x346](upload://rRRMncAhhG8n2iBlUGMM1hObgS6.png)

Starting to get quite desperate to solve this issue. It's extremely annoying to place my board on the road when everyone's watching and not being able to ride off in one go :stuck_out_tongue: 

Thanks in advance!
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-04-24T14:51:30.556Z Reads: 65

```
did u limit erpm?
```

---
## \#3 Posted by: TehAtheist Posted at: 2018-04-24T14:56:11.859Z Reads: 60

```
@onepunchboard Yes, ERPM is limit as that's my way to limit my topspeed.
```

---
## \#4 Posted by: Acidfie Posted at: 2018-04-24T15:13:00.138Z Reads: 53

```
is the box beneath it checked? "Limit erpm with negative torque" ?
```

---
## \#5 Posted by: TehAtheist Posted at: 2018-04-24T15:32:34.281Z Reads: 50

```
nope, my ERPM is also not reached.
```

---
## \#6 Posted by: TehAtheist Posted at: 2018-05-03T19:57:08.192Z Reads: 28

```
[Bump] Added more info to the first post. I'm still having issues with this error and I can't seem to find the culprit.
```

---
## \#7 Posted by: RedEagle Posted at: 2018-05-03T22:44:42.328Z Reads: 26

```
Your regen seems high. Have you checked the vesc for solder balls/damaged components?
Have you ridden it in the rain? How waterproof is your enclosure? Have you checked the caps?
Do you run sensored? You were braking for almost a minute in the second log. Were you going downhill or something?
```

---
## \#8 Posted by: TehAtheist Posted at: 2018-05-03T23:07:37.236Z Reads: 24

```
I have set my battery regen fairly high indeed. Should be 10A instead of 30A.
Never the less, I don't see why that would cause the faults at the start where I'm not even braking.

The VESC seems totally intact. My enclosure is pretty much water proof and the vesc is trapped in some type of foam material, making it nearly impossible to have gotten wet. I pretty much never ride in the rain.

I have not checked the capacitors. I'll try to when I've got the time.

I run uncensored and yes, there is a very steep hill when I come back from the GYM, as I'm very cautious, I apply a constant brake and ride really slowly down :p . Cause I cannot brake with my foot.
```

---
