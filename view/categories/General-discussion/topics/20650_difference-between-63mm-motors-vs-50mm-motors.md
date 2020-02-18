# Difference between 63mm motors vs 50mm motors?

### Replies: 15 Views: 1803

## \#1 Posted by: theviith Posted at: 2017-04-09T03:38:32.993Z Reads: 269

```
Hey guys, so I got a quick question, what's the main difference between a 63mm motor vs a 50mm motor if the kv, motor length, and max voltage are all the same?
For example, a 5065 190kv with max voltage of 12S versus a 6365 of the same specs?
```

---
## \#2 Posted by: willpark16 Posted at: 2017-04-09T03:42:49.212Z Reads: 269

```
Stator size so more powerful motor essentially
```

---
## \#3 Posted by: theviith Posted at: 2017-04-09T03:46:30.076Z Reads: 268

```
i see, so torque stays the same right?
and by that theory, does that mean 63mm motors would use up more battery power than the 50mm while providing the same amount of torque?
```

---
## \#4 Posted by: willpark16 Posted at: 2017-04-09T03:47:43.754Z Reads: 262

```
No the 50mm will essentially heat up faster an more likely need more power to compensate for its smaller size but to try and achieve the same performance as a 63
```

---
## \#5 Posted by: theviith Posted at: 2017-04-09T03:59:14.192Z Reads: 254

```
okay, that makes sense. Thanks
```

---
## \#6 Posted by: theviith Posted at: 2017-04-09T04:01:25.179Z Reads: 252

```
so if I want to extend the range, I would need a 63mm motor to conserve battery power right?
```

---
## \#7 Posted by: willpark16 Posted at: 2017-04-09T04:03:49.532Z Reads: 249

```
Yes plus u get more power a 6374 is best for single
```

---
## \#8 Posted by: Stef Posted at: 2017-04-09T06:00:38.727Z Reads: 240

```
The range wont be affected much by the motor size, if at all. Choose your motor based on the power your need, which will mostly depend on whether you want to take on steep hills, how fast you want to go and how heavy your are.
```

---
## \#9 Posted by: makevoid Posted at: 2017-04-09T06:02:31.522Z Reads: 233

```
vesc 4.12 works better with smaller motors, with bigger ones it tends to overheat - if you plan to run a single drive and you're 80kg+ than probably you need to attach a big heatsink on top of the vesc if you don't want your power to be limited when going uphill otherwise choose vesc6/ollin/vescx or another esc and you have no problem even with a single 6374
```

---
## \#10 Posted by: jga Posted at: 2017-04-09T08:32:05.287Z Reads: 218

```
That's an interesting information because I have a 6374 and planned to use my VESC on my board, initially with one motor only. I don't particularly have big hills, or very occasionaly for 50-100m.
The thing is, I do not have a clue how to put this heatsink.
```

---
## \#11 Posted by: RogerD Posted at: 2017-04-10T08:44:07.054Z Reads: 182

```
Google heatsink. Buy heatsink/s from ebay. Stick heatsinks on with thermal paste.

Or... Buy a small 5v fan (powered from your receiver) and point it at your vesc. Works perfectly on single 6374 setup with 8-10s
```

---
## \#12 Posted by: michaelcpg Posted at: 2017-04-10T09:51:32.287Z Reads: 169

```
My understanding is that larger motors require more current to perform optimally and so a smaller motor will actually often be more effective as the VESC will take longer to heat up. 

I've seen videos of people that experience this, comparing a single Enertion 6372 motor with a single Ollin 5065 motor and after going to the smaller motor, they were able to get up larger hills before the VESC overheated.
```

---
## \#13 Posted by: theviith Posted at: 2017-04-13T03:48:03.813Z Reads: 137

```
hm so there appears to be contradictory information, which is it?

I'm planning on a dual motor setup with 10s on 6in pneumatic wheels. Would a 50mm or 63mm be better in terms of range.
```

---
## \#14 Posted by: Ryel Posted at: 2017-06-16T16:16:35.357Z Reads: 107

```
willpark16, you mentioned a 6374 is best for single, but would that be good for dual? I'm thinking of doing a dual setup with two 190kv SK3s.
```

---
## \#15 Posted by: willpark16 Posted at: 2017-06-16T17:23:21.723Z Reads: 103

```
The issue is moreso truck spacing I would recommend larger motors like that for a mountain board
```

---
