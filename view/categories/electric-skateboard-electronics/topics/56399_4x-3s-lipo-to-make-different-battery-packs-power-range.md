# 4x 3s lipo to make different battery packs (power/range)

### Replies: 4 Views: 244

## \#1 Posted by: KevinMinato Posted at: 2018-05-22T20:49:33.707Z Reads: 43

```
Hello, 
I am building my first electric longboard and waiting for my components to come in. I have ordered 4x 3s 5000mAh 20c lipo battery packs which I will be running in series to make a 12s pack. I was wondering though. If I had 2 different battery wiring connecter set ups:

**Torque and power pack** - 12s 5000mAh 
a) all 4 packs in series

**Range pack** - 6s 10000mAh
b) 2 sets of 2x lipo in parallel and then those packs in series

would I be able to just interchange 2 different wiring connector set ups to interchange between range and power based on what I needed for that outing? or would i need to re program the VESC every time? 

Im not sure if I am explaining myself properly so let me know if this makes sense. Basically I want the power for fun short rides but if I am ever doing a long marathon ride I could change the battery wiring for a longer range and less power/top speed
```

---
## \#2 Posted by: AgressivStreetLamp Posted at: 2018-05-22T21:36:56.511Z Reads: 36

```
Hey there so I'm new to all this but I do have a background in Electrical Engineering. For the most part the different working won't make a difference.  At the end of the day it is your battery capacity and power usage that determine the distance you can go.
Assuming all else equal,  if you ride at the same speed (below what your parallel setup will allow) the range  you will get pretty much the same .  Now that doesn't account for the fact that at a higher voltage (more in series) you will pull less current at the same power(speed) and more current produces more loss and this less range. So the higher voltage will actually get you further at the same speed.

tl;Dr  changing your wiring won't really change your range. How fast you go and how large (how much power) your battery is (has)  [in Watthours or Volts x Amphours]. So just go with the larger S and keep a cool head. Or better yet, give your vesc 2 modes, one with a lower current limit.
```

---
## \#3 Posted by: PatRocks Posted at: 2018-05-22T21:53:40.108Z Reads: 28

```
Yep, go 12s, you will be using watts so more voltage requires less amps essentially which will be easier on the esc in most cases
```

---
## \#4 Posted by: KevinMinato Posted at: 2018-05-22T22:23:24.129Z Reads: 22

```
Thank you so much. That is super helpful information. It really does make sense if I will be pulling an equal load. I appreciate the help. :blush:
```

---
