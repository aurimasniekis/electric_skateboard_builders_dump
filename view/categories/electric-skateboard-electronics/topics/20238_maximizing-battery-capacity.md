# Maximizing battery capacity

### Replies: 5 Views: 577

## \#1 Posted by: thisguyhere Posted at: 2017-04-04T05:56:36.369Z Reads: 123

```
So I'm running 10s4p pack with a single 6374 190kv motor + vesc 4.12.

Using a [balance charger](http://media.progressiverc.com/media/catalog/product/cache/1/image/1000x/040ec09b1e35df139433887a97daa66f/i/m/img_0311.jpg) I get the total pack up to 41 volts.

The Vesc is configured to start battery cutoff at 31v and end at 30v.

Problem is, once the pack gets down to about 33v there's a very noticeable drop in performance, and a damn near stop at around 32v.  Shouldn't the motor pretty much run at full power until the cutoff starts?

Just wondering if some of my settings are no good...

This would probably help with a screenshot of my vesc bldc configuration, I can post it later if needed.
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-04-04T06:26:27.358Z Reads: 116

```
The gap between  cutoff start and cutoff off end is no needed to soften the cutoff. Yours is only 1V. Set cutoff end to 28V and it should be softer.
```

---
## \#3 Posted by: saul Posted at: 2017-04-04T08:09:30.820Z Reads: 93

```
10V difference from full to empty, plus voltage sag! 
the performance is not going to be the same, just the way it is. for now. 

a bigger pack would help, so you're not running down to empty all the time.
```

---
## \#4 Posted by: PXSS Posted at: 2017-04-04T11:22:08.747Z Reads: 77

```
Which cells are you using and post your settings. Ackmaniac and I can probably help once u add this
```

---
## \#5 Posted by: thisguyhere Posted at: 2017-04-04T16:46:54.652Z Reads: 56

```
You got it, using Samsung 25r cells.

I'll screencap settings tonight.

Thanks.
```

---
