# Split ppm question

### Replies: 25 Views: 582

## \#1 Posted by: yanggatang Posted at: 2019-01-03T08:00:22.096Z Reads: 139

```
For split ppm, do you have to use a ysplit ppm or can you use 2 separate ppm and connect it to the receiver? 
Like this video https://www.youtube.com/watch?v=qpovd2XRKqc?

Currently using this remote with 2 VESC 4.12 from diyelectric
https://www.amazon.com/XCSOURCE-Transmitter-Controller-Skateboard-OS917/dp/B073GX83NH
```

---
## \#2 Posted by: yanggatang Posted at: 2019-01-03T08:01:41.497Z Reads: 137

```
Also, in the forums i keep seeing that people need to cut the 5v line. Which line is that? Sorry, kinda new to dual motor setup
```

---
## \#3 Posted by: b264 Posted at: 2019-01-03T08:17:05.693Z Reads: 132

```
On some remotes, that remote being one of them, you can use 2 receivers.  So you have 3 options:

1) Split PPM
2) CANBUS master/slave
3) Dual PPM (some remotes)

I prefer #3 on receivers that support it, like the Mini Remote you linked.  You'd need [an extra receiver](collections/remote-controller/products/2-4ghz-mini-receiver).
```

---
## \#4 Posted by: TowerCrisis Posted at: 2019-01-03T08:18:31.843Z Reads: 121

```
Also, keep in mind that you can have traction control with a can bus master / slave setup.
```

---
## \#5 Posted by: b264 Posted at: 2019-01-03T08:19:25.248Z Reads: 121

```
Yes.  However dual PPM can give you redundancy so if one drive train malfunctions for any reason you have another one still running -- aka: you still might have brakes.
#1 could have that depending on the specific failure, and #2 will almost never have that.  #3 will almost always have that.
```

---
## \#6 Posted by: yanggatang Posted at: 2019-01-03T08:19:43.900Z Reads: 117

```
yeah, i'm just having trouble setting up canbus. I'm not sure if I fried my canbus or maybe the settings are wrong, but only the master motor spins while the slave doesn't
```

---
## \#7 Posted by: yanggatang Posted at: 2019-01-03T08:23:13.082Z Reads: 115

```
So it wouldn't be possible to just use 2 PPM and connect it to the mini's receiver like the video right?
https://youtu.be/qpovd2XRKqc?t=312
```

---
## \#8 Posted by: yanggatang Posted at: 2019-01-03T08:23:37.684Z Reads: 113

```
For dual PPM, would the settings be the same as split ppm?
```

---
## \#9 Posted by: b264 Posted at: 2019-01-03T08:24:04.242Z Reads: 112

```
[quote="yanggatang, post:7, topic:79732, full:true"]
So it wouldn’t be possible to just use 2 PPM and connect it to the mini’s receiver like the video right?
[/quote]

Yeah, that's "Split PPM"
```

---
## \#10 Posted by: b264 Posted at: 2019-01-03T08:24:58.080Z Reads: 106

```
[quote="yanggatang, post:8, topic:79732, full:true"]
For dual PPM, would the settings be the same as split ppm?
[/quote]

For any of the PPM options you can configure each ESC independently so they could be the same, or different.  Your choice.  I've never used CANBUS so I don't know about that one.
```

---
## \#11 Posted by: linsus Posted at: 2019-01-03T09:21:14.299Z Reads: 101

```
Damn, am I the only one using the NRF over CAN on this forum? #Feelsbadman
```

---
## \#12 Posted by: yanggatang Posted at: 2019-01-03T20:44:20.543Z Reads: 73

```
So for split ppm would this work? 
https://www.amazon.com/12-inch-Servo-Y-Cables-Pack-5/dp/B007XP0NXE
```

---
## \#13 Posted by: b264 Posted at: 2019-01-03T20:54:14.992Z Reads: 72

```
I don't think so; one of the connectors is male instead of 3 female ones.

I would highly recommend just soldering them though and then coating all connections with some sort of conformal coating for waterproofing

The connector in the receiver itself I wouldn't solder
```

---
## \#15 Posted by: Andy87 Posted at: 2019-01-03T21:16:33.326Z Reads: 69

```
And cut the middle cable on one plug to one of the vescs 😉
```

---
## \#16 Posted by: dareno Posted at: 2019-01-03T21:17:15.573Z Reads: 71

```
Its early.
```

---
## \#17 Posted by: Andy87 Posted at: 2019-01-03T21:18:48.618Z Reads: 68

```
Here it’s late... other side of the world 😂
```

---
## \#18 Posted by: yanggatang Posted at: 2019-01-03T21:20:38.632Z Reads: 69

```
so I have two male to male ppm cables. if i just connect the two male ends to the female would that work? I'm not sure if trust my own soldering skills hehe
```

---
## \#19 Posted by: dareno Posted at: 2019-01-03T21:21:28.862Z Reads: 67

```
I think the cutting the 5v cable was discussed above anyway so there
```

---
## \#20 Posted by: bigben Posted at: 2019-01-03T21:22:09.802Z Reads: 67

```
https://www.electric-skateboard.builders/t/y-piece-or-canbus/26461
I asked the same question some time ago. More replies than you can shake a stick at.
```

---
## \#21 Posted by: Andy87 Posted at: 2019-01-03T21:26:30.248Z Reads: 64

```
Can be...can’t hold up to all the stuff I read 😅
And thought better to mention than it got lost 😌
```

---
## \#23 Posted by: b264 Posted at: 2019-01-03T21:46:02.243Z Reads: 57

```
If you can't solder, you should learn how.  Learn on things that aren't your electric skateboard.
```

---
## \#24 Posted by: b264 Posted at: 2019-01-03T21:47:03.081Z Reads: 58

```
[quote="dareno, post:22, topic:79732"]
Vesc has a female ppm plug
[/quote]

Some VESC have a male.  Some VESC have no connector at all and only pads on the PCB.  That's an unsafe generalisation.
```

---
## \#25 Posted by: dareno Posted at: 2019-01-03T22:01:27.449Z Reads: 56

```
Well don't I feel like the fucking asshole?  You are quite correct my friend the tb one does in fact have a male I believe.  Should have established that first.  I stand corrected.  I will delete my heinous comments forthwith.
```

---
## \#26 Posted by: Superflim Posted at: 2019-08-24T15:27:53.196Z Reads: 33

```
With option 3; Does the Bluetooth app still work with that option?
```

---
## \#27 Posted by: b264 Posted at: 2019-08-24T20:58:01.882Z Reads: 29

```
@Superflim Most of us went to the new builders forum.  There is more information in the thread for this

https://forum./t/how-to-bind-the-mini-remote/95

You can ask any questions over there
```

---
