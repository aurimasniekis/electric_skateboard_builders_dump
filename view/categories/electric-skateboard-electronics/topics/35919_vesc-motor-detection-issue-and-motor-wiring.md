# VESC motor detection issue and motor wiring

### Replies: 23 Views: 1515

## \#1 Posted by: spullen Posted at: 2017-10-19T00:49:45.443Z Reads: 98

```
So here's my configuration:

VESC v2.18 
Torque Board 6374 190kv motor
9s battery (three 3s batteries in series), each has 20c-30c discharge and 5000mAh

VESC and motor from 

My first question, to possibly rule out my other issue, how do I wire the motor to the VESC? I can't seem to find anything about this online. I've watched a few videos (the one's that diyelectricskateboard links to), and matched up the wiring to what I saw in the video.

However, my main issue is when I try to configure the VESC. When I go through the BLDC detect motor process to set the Integrator limit and BEMF coupling I get a "bad detection result received" error. I've tried a couple of things suggested elsewhere on the forum (changing the battery cutoffs a little, upping the amp from 6 to 8 amps) without any luck. So, what's my next step to solve this problem?

<img src="/uploads/db1493/original/3X/3/6/36303cd9089dbd9444778315ecb9a6b74d828704.png" width="690" height="367">

Any help would be great, thanks!
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-10-19T02:05:35.601Z Reads: 87

```
try loosening motor mount screws
```

---
## \#3 Posted by: spullen Posted at: 2017-10-19T23:51:51.702Z Reads: 76

```
That didn't work, but definitely could have been contributing to the problem. After I loosened the motor on the motor mount a bit I was able to turn the motor more freely than I was able to before.

Not sure if this helps at all, but here's how I have my VESC connected to my motor:

<img src="/uploads/db1493/original/3X/c/7/c7950fb1aea9d36d947d4485e04e40fb84812839.jpg" width="374" height="500">
Yellow is connected to the VESC on the same side that the usb port is on, blue is the middle.
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-10-19T23:54:39.741Z Reads: 73

```
your motor mount screws were probably shorting your motor.  cut them down a bit and youll be good to go
```

---
## \#5 Posted by: spullen Posted at: 2017-10-20T00:12:56.828Z Reads: 71

```
If they are shorting the motor, will this have caused any permanent damage to the motor or esc?
```

---
## \#6 Posted by: Funga Posted at: 2017-10-20T00:55:08.192Z Reads: 69

```
Hey, with your phase wires, you see that the heat shrink doesn’t cover the whole connection. It may not be the problem but make sure they aren’t contacting each other. With mine I just put extra electrical tape over them. 

Also maybe try switching wires around? It won’t do any harm just switch direction of motor.
```

---
## \#7 Posted by: spullen Posted at: 2017-10-20T01:05:57.463Z Reads: 69

```
They're bullet connectors, which is why there's no heat shrink over them. When connected, they seem to be in there pretty good.
```

---
## \#8 Posted by: Funga Posted at: 2017-10-20T01:22:58.858Z Reads: 66

```
The problem isn’t them not being in properly. Some people have had detection problems cause the phase wires actually touch each other and short the motor. Just be weary of that :slight_smile:
```

---
## \#9 Posted by: spullen Posted at: 2017-10-20T23:44:26.729Z Reads: 61

```
I don't believe they were touching when I was trying to program the VESC, but I'll definitely wrap them in electrical tape to prevent that from happening once I get everything sorted out.
```

---
## \#10 Posted by: cwazy1 Posted at: 2017-10-20T23:49:28.936Z Reads: 62

```
[quote="spullen, post:3, topic:35919"]
After I loosened the motor on the motor mount a bit I was able to turn the motor more freely than I was able to before
[/quote]

Is it still tough to turn? Because if so, you need to back the motor screws out even further...

it doesn't matter which order your phase wires are connected. Just plug them in. You can also flip around wires. 

If your motor spins backwards, flip 2 of the wires.
```

---
## \#11 Posted by: spullen Posted at: 2017-10-21T15:46:11.932Z Reads: 53

```
Yeah still no luck. Unscrewed the motor screws a bit more. The motor is able to turn pretty freely when I turn it manually. Also wrapped the phase wires with electrical tape where they were exposed.

The VESC seems fine (being able to connect and read/write configurations to it), could it just be a bad motor? Any thing else I could try before going down the route of getting another motor?
```

---
## \#12 Posted by: Hummie Posted at: 2017-10-21T16:00:21.824Z Reads: 53

```
Does it even sputter when testing?  If ud shorted the MOTors w the screws I'd think it would at least stutter and move a little
```

---
## \#13 Posted by: spullen Posted at: 2017-10-21T16:10:14.187Z Reads: 53

```
When I powered everything up for the first time there was a quick sputter, but nothing since.

What about battery, right now my 3 x 3s setup has about 3.72 - 3.76v per cell. Should I charge them up and try again, or would this not change anything I'm seeing?
```

---
## \#14 Posted by: Hummie Posted at: 2017-10-21T17:37:23.091Z Reads: 52

```
maybe youre hitting your low voltage cut offs.  try charging.  you'd be hitting at least the first.  but if you crushed the motor wires that's not good.  you have a high precision multimeter that shows inductance or details resistance to test the motor?
```

---
## \#15 Posted by: nikdyskin Posted at: 2017-10-24T19:38:52.873Z Reads: 49

```
hey man! I have the exact same setup as you and my motor detection is also failing.if you solve this problem please tell me how.thank you.
```

---
## \#16 Posted by: spullen Posted at: 2017-10-25T12:29:45.138Z Reads: 49

```
@nikdyskin will do, likewise if you figure anything out. Been pretty busy the last week so I haven't gotten around to trying anything else out...
```

---
## \#17 Posted by: spullen Posted at: 2017-10-25T23:39:52.746Z Reads: 47

```
Was able to test the resistance on the motor (I don't have anything that tests induction), I've tested the connection between all three of the wires coming out of the motor (wire 1 to 2, wire 1 to 3, wire 2 - 3) and have a complete circuit without any resistance (at least none that registered on my multimeter).

Still haven't gotten around to charging my batteries or changing the configuration of the cutoffs.
```

---
## \#18 Posted by: PedroBaro Posted at: 2017-10-27T23:38:30.449Z Reads: 46

```
That happened to me and I try everything to fix it but I can’t. I think I broke my vesc or motor. If you fix it let me know
```

---
## \#19 Posted by: spullen Posted at: 2017-10-28T14:09:59.506Z Reads: 42

```
Well gave my batteries a charge, and still no luck. Think I might just buy another motor to see if that is the problem.
```

---
## \#20 Posted by: spullen Posted at: 2017-11-04T18:42:07.714Z Reads: 38

```
Bought another VESC and motor. Swapped the motor, no luck. Swapped the VESC everything worked fine. Swapped back the original motor I had and that worked as well! So, bad VESC was the culprit.
```

---
## \#21 Posted by: Hummie Posted at: 2017-11-04T19:07:45.948Z Reads: 38

```
Where's the vesc from?  Seems some sellers sell crap vescs.  Did they replace  it?
```

---
## \#22 Posted by: spullen Posted at: 2017-11-04T19:36:56.801Z Reads: 37

```
It's from  (products/torque-esc-vesc-bldc-electronic-speed-controller). They did not replace it (didn't know it was the VESC until I could narrow it down to that), but I probably will shoot them a message about it.
```

---
## \#23 Posted by: spullen Posted at: 2017-11-08T00:21:37.917Z Reads: 33

```
One thing that was definitely an issue were the motor mounting bolts. As noted above they were seizing the motor because they were too long. I asked the support people at diyelectricskateboard what size they should be and they said the size is an M4 x 8mm. I received M4 x 10mm bolts with the mount that I ordered. Seems to be a recurring theme with stuff that I've ordered from them, some of the components are too big, some too small.
```

---
