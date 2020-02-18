# Controller has no variability

### Replies: 8 Views: 756

## \#1 Posted by: ScottHaen Posted at: 2017-01-02T17:56:43.322Z Reads: 84

```
Hi there, I have an Eneriton Nano-x controller, a replacement space cell battery, and single hub motor from Carvon. Everything is working fine, but my controller is functioning less like a controller and more like an on/off button. My motor is either on full or not, and its very difficult to get anywhere in between. Is this a problem with my controller, my VESC settings, or a problem with my motor? Does anyone have any idea how to fix this? Thanks
```

---
## \#2 Posted by: mmaner Posted at: 2017-01-02T17:57:31.812Z Reads: 83

```
Have you done PPM setup in the BLDC tool?
```

---
## \#3 Posted by: ScottHaen Posted at: 2017-01-02T18:01:37.480Z Reads: 81

```
@mmaner Yes, I have
```

---
## \#4 Posted by: mmaner Posted at: 2017-01-02T18:03:35.754Z Reads: 75

```
Not sure how experienced you are, but there's a huge difference between bench testing and and actual load in the motor.
```

---
## \#5 Posted by: ScottHaen Posted at: 2017-01-02T18:04:54.598Z Reads: 71

```
@mmaner That may be the issue. I don't have a battery case yet so I can't ride it yet and I've only been able to do bench testing. This is also my first DIY build
```

---
## \#6 Posted by: Hummie Posted at: 2017-01-02T18:23:12.058Z Reads: 63

```
on the bench the vesc will do only off or on but on the road with resistance it's fine.  think it's current control.  ride it
```

---
## \#7 Posted by: mmaner Posted at: 2017-01-02T20:01:11.850Z Reads: 51

```
No worries, everyone has to learn.  I think that's the issue though.  When you put a load on it it will have much more 'finesse' in the remote trigger travel.
```

---
## \#8 Posted by: Esrapp21 Posted at: 2017-01-02T20:28:40.472Z Reads: 46

```
If you notice it does this while riding it, maybe you are in expert mode. I think beginner mode has better, more gradual acceleration and braking.
```

---
