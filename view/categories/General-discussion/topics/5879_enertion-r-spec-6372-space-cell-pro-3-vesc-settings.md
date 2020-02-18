# Enertion R-Spec 6372 &#124; Space Cell Pro 3 &#124; VESC settings?

### Replies: 6 Views: 1216

## \#1 Posted by: Haick Posted at: 2016-07-11T00:06:25.737Z Reads: 158

```
I am almost positive this question has been asked before, but I was wondering what specific settings i should set my Enertion VESC 4.12 for my Mono 6372 motor and my space cell pro 3. If there are screenshots posted somewhere already, could someone link them to me?
```

---
## \#2 Posted by: sl33py Posted at: 2016-07-11T01:31:20.582Z Reads: 158

```
you aren't asking about motor detection settings right?

I've run my VESC's at 6-10s without adjusting anything.  Can you - definitely.  But the default just works for me, so i haven't messed with it usually.  Unless there is an under or over voltage error - which i fixed by adjusting just those settings.  It was a while back and if i get a moment later i'll launch one of the ported BLDC to identify them for you.

Space cell is 10s3p before anyone asks.

HTH - GL!
```

---
## \#3 Posted by: Haick Posted at: 2016-07-11T01:38:42.509Z Reads: 150

```
As I understand it, the vesc is pre programmed with settings for the enertion 6355 motors. Just want to make sure that my motors and battery settings for my vesc are all correct so i don't accidentally hurt something.
```

---
## \#4 Posted by: kyo Posted at: 2016-07-11T02:00:57.158Z Reads: 137

```
I have the same question too.
```

---
## \#5 Posted by: cmatson Posted at: 2016-07-11T02:21:40.243Z Reads: 133

```
Search "vesc faq" on the forum, and there a thread on the vesc set up for a space cell.

The only difference is that the space cell is now 40 amps, so where the thread will say 30, change it to 40.
```

---
## \#6 Posted by: sl33py Posted at: 2016-07-11T17:29:40.381Z Reads: 111

```
Yeah, i realize Enertion/Onloop has these programmed for you.

Not to be difficult, but it's still not configured correctly for your motor until you do the calibration yourself.  A R-Spec 6355 is similar but not the same as the R-Spec 6372.  Close enough to ride - most likely.  But even between motors you can see small differences during detection - even one detection to the next (meaning it's probably somewhat forgiving).

I've blown a few VESC's (DRV chips) - so i do a detection every time, for every motor.  A small investment of 5-15min is worth knowing it's 100% right for my motor.  

having killed a few DRV chips - overvoltage and really hard start/stop was what killed mine.  If the 6372 can output more power than the 6355 i would wonder if this is more of a potential issue?  Regardless - when bench testing i'd be a bit gentle on the hard start/stops.

All that said - it's Enertion's warranty and great customer service backing you up.  I've had issues in the past and he's gone above and beyond each time to get me back riding.  If you are riding it like they sent, and no mention of re-detecting for the 6372 vs 6355, you should be GTG.  I'd adjust per @cmatson 's suggestion for the new Amps.  

If you are reasonably skilled w/ a reflow setup - getting a couple DRV chips might be good peace of mind.  about $6 ea from Mouser.  I have a dead DRV on one of my VESCs i'm swapping soon (waiting on chips from mouser).  Luckily i think i have 2 or 3 spare VESC's (for other project boards).  

Good luck!  Read up the FAQ and ask if you get stuck.
```

---
