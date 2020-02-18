# Changing how remote works

### Replies: 10 Views: 187

## \#1 Posted by: kalebludlow Posted at: 2018-10-06T03:10:45.980Z Reads: 91

```
Okay so I have finally gotten my build together, and I'm not too happy with how the remote responds. On my diyeboard build, when I held the throttle in the same position, it would not increase speed. The current setup will increase speed even if the throttle doesnt move. So Im wondering if there is something in vesc-tool that will do this. To simplify: I want 50% throttle = 50% max speed. Sorry if this is obvious. 

Also, is there a way reduce the dead zone in the middle of the throttle range?
```

---
## \#2 Posted by: mmaner Posted at: 2018-10-06T03:27:51.620Z Reads: 87

```
Did you do the PPM detection?  You can also decrease the dead band in PPM settings. Look up throttle curves, that will likely resolve your issue.
```

---
## \#3 Posted by: kalebludlow Posted at: 2018-10-06T03:31:58.515Z Reads: 80

```
I'll double check PPM settings when I open the enclosure soon. Will there be any unexpected issues running 0% or 1% deadband?
```

---
## \#4 Posted by: mmaner Posted at: 2018-10-06T03:33:56.309Z Reads: 78

```
I wouldn't, I'd use at least 5%. With none it very little dead band you'll accelerate and brake rapidly & back and forth. The control at slow speeds will suck. 

Search for throttle curves, they are awesome and easy to setup, it makes a powerful board much easier to control.
```

---
## \#5 Posted by: kalebludlow Posted at: 2018-10-06T03:35:27.028Z Reads: 72

```
Should I be flashing ackmaniac firmware for more control over everything or is the stock firmware enough? Still tinkering with vesc-tool so I don't wanna break things
```

---
## \#6 Posted by: mmaner Posted at: 2018-10-06T03:36:55.108Z Reads: 65

```
I don't like the stock firmware, lots of people do. It's just preference. @Ackmaniac's firmware is far more configurable and makes sense. Plus his implementation of throttle curves is far superior to the stock firmware.
```

---
## \#7 Posted by: kalebludlow Posted at: 2018-10-06T03:37:52.017Z Reads: 63

```
You've convinced me. Thanks heaps for the help mate
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-10-06T08:56:01.340Z Reads: 53

```
I dont think any firmware will give you speed control instead of current :) Its like car you push throttle you get torque and on any level torque you can speed up or slow down same with current as current = torque. I even sometimes able to reach top speed at like 20% of throttle :)
```

---
## \#9 Posted by: kalebludlow Posted at: 2018-10-06T08:58:05.135Z Reads: 53

```
I think I just need to spend more time riding and adapt to the way things work. I just wan't sure if it was possible
```

---
## \#10 Posted by: Kug3lis Posted at: 2018-10-06T09:00:07.930Z Reads: 49

```
Well speed can be reached at any current level based on the load on wheels, so that's why we do current control if you stock on hill that you control how much torque wheel gets not other way, as imagine you wheels spinning in place and etc :)
```

---
