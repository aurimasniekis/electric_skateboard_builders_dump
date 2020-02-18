# VESC Speed Tiers via. Remote (think boosted)

### Replies: 18 Views: 1553

## \#1 Posted by: 8dotzero Posted at: 2016-09-04T19:21:49.790Z Reads: 148

```
I want to change my maximum speed with a button on my remote.
My idea is to change beetween different speed modes.
is this possible ?
```

---
## \#2 Posted by: mason Posted at: 2016-09-04T22:48:43.915Z Reads: 131

```
yes, it is possible.
```

---
## \#3 Posted by: sl33py Posted at: 2016-09-04T23:55:59.962Z Reads: 125

```
How?  This is a major factor/thing i like about production boards - ability to change "modes" on the fly (usually stopped not rolling), and hand it to a friend in a "starter" mode w/ limited accel/brakes and top speed.

Would love an easy way to toggle like this on VESC w/ GT2b.

More detail on how to do this?
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-05T00:08:14.367Z Reads: 122

```
not possible on current control mode (unless you can dynamically limit erpm) as it will speed up/slow down on various inclines or loads. Duty cycle or PID may be possible but these are inferior control modes for the VESC
```

---
## \#5 Posted by: Stevemk14ebr Posted at: 2016-09-05T00:09:53.429Z Reads: 115

```
Just limit the max output of the controller. They use ppm so if the max value it can send is 2000 units long limit it to 1000 or so if it's supposed to be at half speed.
```

---
## \#6 Posted by: Namasaki Posted at: 2016-09-05T00:12:07.279Z Reads: 112

```
It could be possible to do with the bldc mobile app and smartphone. But I think it's still in development stages. 
I Don't think there's any remote available that could do that.
```

---
## \#7 Posted by: Jinra Posted at: 2016-09-05T00:13:10.496Z Reads: 110

```
Benchwheel remote has two modes for half throttle, but this won't limit max speed in current control mode, it will only limit acceleration.

It would limit speed on duty cycle or PID though.
```

---
## \#8 Posted by: evoheyax Posted at: 2016-09-05T00:15:56.022Z Reads: 111

```
It's possible in current control to some degree. Just limit amps and you will go slower. But you will need to write a custom application and setup a communication system between the uart port and  your switch on the remote.

I think this would be a great feature, just someone needs to make it.
```

---
## \#9 Posted by: Jinra Posted at: 2016-09-05T00:19:13.415Z Reads: 103

```
limiting amps doesn't limit speed. you will start accelerating fast during declines, and you'll slow to a crawl during inclines vs flats. Not to mention it'll affect different people differently.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-09-05T00:19:45.309Z Reads: 101

```
After experiencing current control mode, I would never want to go 🔙 to duty cycle mode⚠️
```

---
## \#11 Posted by: Jinra Posted at: 2016-09-05T00:20:43.790Z Reads: 96

```
yea me either, lol. I would like a duty cycle mode that works like the Evolve gt though, that was great.
```

---
## \#12 Posted by: evoheyax Posted at: 2016-09-05T00:32:35.992Z Reads: 91

```
It will have some effect on top speed and you will accelerate slower. If you don't believe me, limited your vesc's to 10 amps per motor and tell me how it accelerates to your current settings. 15 amps per motor and 25 amps per motor is like night and day in how fast you can accelerate, which is really the danger for new riders. Too much torque throws people off. If they don't want to hit high speeds, they can stop climbing at any point...
```

---
## \#13 Posted by: Namasaki Posted at: 2016-09-05T00:36:11.971Z Reads: 85

```
I think the idea of preset modes or settings would be cool but I imagine that feature would have to be written into the bldc software code.  Good luck with that. 
I'm still holding my breath for the bldc mobile app.
```

---
## \#14 Posted by: evoheyax Posted at: 2016-09-05T00:39:09.473Z Reads: 87

```
Yea, it's true it's not easy. I am planning on talking to some of my professors to see if it would be interested in helping me understand what's going on with his code. I really want to help develop some features, but it is deep stuff.
```

---
## \#15 Posted by: Stevemk14ebr Posted at: 2016-09-05T00:39:14.171Z Reads: 87

```
Eventually when I'm back home I'll make an open source controller for the community with some throttle curve settings and redundant radios for reliability. Maybe have a screen like the gt remotes too. We'll see, until then the vest is your only hope of changing the throttle curve
```

---
## \#16 Posted by: Jinra Posted at: 2016-09-05T00:42:24.897Z Reads: 82

```
i know how it affects speed because I've used a current limiter on the VESC. I'm saying it won't work well due to the largely varying speeds on inclines and declines. It'll only be semi consistent on flats. As i mentioned above it'll largely affect acceleration. 

Current control in general is not the best control mode to use for limiting speed. Best practice is to just throttle when you need it.
```

---
## \#17 Posted by: makevoid Posted at: 2016-09-05T03:54:13.653Z Reads: 72

```
I think it should set something like reduced motor max current to limit acceleration and reduce max erpm to limit max speed. It could be done via an app that uses the serial interface (uart) over bluetooth and probably Jacob's app is the closest to have such feature (even if that involves setting the values manually at the moment). I would have probably three settings, a slow mode with 60% motor max and 50% max erpm that limits both acceleration and speed, a mode with just 70% erpm and then normal mode (fastest,  100% both values). I guess that the most obvious/generic thing to implement that feature would be to be able to save presets of the BLDC tool configs and recall them / set them very easily with few taps...  some day ^^
```

---
## \#18 Posted by: elkick Posted at: 2016-09-05T05:23:24.145Z Reads: 62

```
The next gen BLDC tool might include things like that this. Plus an easier to use user interface. I don't know the exact time line though, but I guess it's not that far away.
```

---
