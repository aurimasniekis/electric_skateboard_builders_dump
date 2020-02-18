# PPM App Configuration - Deadband/Pulsewidth

### Replies: 3 Views: 675

## \#1 Posted by: Michael319 Posted at: 2017-04-04T14:38:49.733Z Reads: 75

```
So I was curious about the PPM App Configuration, I hadn't changed any of the settings and I figured it wouldn't hurt to customize these values for my own build. What I did and How it changed my Board:

1. Changed the deadband from .15 to .05

2. Changed the minimum pulse width to 1.09 from 1.00. Did this because earn my controller was at full brake, I was only getting about 9% Pulsewidth 

3. Changed maximum Pulsewidth to 1.96 from 2.00. Also, because when I was at full throttle I was only getting 94% pulse

1st issue: when the controller was turned off, the pulse width was changed to 55%, which gave it a little acceleration. Fixed this by changing the trim on my gt2b and adjusting the min and max to keep it at 50% Pulsewidth

What this changed, it increased my acceleration and my top speed, this also gave me stronger brakes.
```

---
## \#2 Posted by: Blasto Posted at: 2017-04-04T16:15:22.714Z Reads: 70

```
your deadband is to low, the ppm is always a little noisy varying +-0.1 ms. If your deadband window is to narrow and your signal is not perfectly centered, you will get some funky accelerating or braking. The dead band is centered on the center (min+max)/2. 

meaning if you have a dead band of 0.05ms, it's only 0.025ms away from accelerating

<img src="/uploads/db1493/original/3X/f/7/f7725d7234ea7e30ea022bd0d772002a147da4f9.png" width="690" height="93">
```

---
## \#3 Posted by: Michael319 Posted at: 2017-04-04T16:23:05.483Z Reads: 65

```
Yeah, sorry if I didn't make it clear. I fixed the acceleration issue, while still keeping deadband at .05. No issues so far
```

---
