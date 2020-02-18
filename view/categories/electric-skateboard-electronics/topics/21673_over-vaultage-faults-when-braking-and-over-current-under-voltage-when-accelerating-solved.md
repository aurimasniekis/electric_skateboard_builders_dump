# &ldquo;Over vaultage&rdquo; faults when braking and &ldquo;over current&rdquo; / &ldquo;under voltage&rdquo; when accelerating \[SOLVED\]

### Replies: 9 Views: 613

## \#1 Posted by: pyttroll Posted at: 2017-04-24T11:55:54.571Z Reads: 99

```
I've been having Over vaultage faults for the past 2 weeks, I'm running a 10S5P with a 6355 / 190kv from TB and Ackmaniac's firmware. 

The problem occurs during sustained braking.

I originally thought it was a BMS issue when my battery was close to full so I rewired the BMS to only use it for charge. That did not solve the problem.

I tried swapping the VESC for a VESC-X, rewiring the BMS to charge/discharge in the process but I'm still having the issues...

Here is my latest ride:

https://metr.at/r/p2Nb4

And here is my VESC config (I noticed my battery cutoff values are wrong and they should be 28V and 30V but I don't think that could be the problem...)

<img src="/uploads/db1493/original/3X/7/6/7697b7da322e978e8cac782ed1ac7cfdabb4f964.png" width="690" height="417">

Any help would be really appreciated.

Pyt
```

---
## \#2 Posted by: Blasto Posted at: 2017-04-24T12:08:13.496Z Reads: 85

```
Batt max to 30A? Double check if your max input voltage is indeed 57V.... ??
```

---
## \#3 Posted by: pyttroll Posted at: 2017-04-24T12:11:37.970Z Reads: 86

```
I'm pretty sure it's 57V since it's the default value when I install Ackmaniac's firmware.
As for 30A for batt max, wouldn't that only affect acceleration?
```

---
## \#4 Posted by: pyttroll Posted at: 2017-04-24T20:39:14.126Z Reads: 72

```
Following up on this morning's ride, I just finish riding the opposite way, which is mostly uphill, and I got some OVER CURRENT and UNDER VOLTAGE faults while pushing hard on the trigger. Something is really messed up...
Still got the UNDER VOLTAGE faults too.

Here's the ride:

https://metr.at/r/HTsJn
```

---
## \#5 Posted by: laurnts Posted at: 2017-04-24T22:50:24.545Z Reads: 65

```
Elevation drop, speed drop and voltage increase shows that you are braking and seems that the battery is full so it goes over voltage. The opposites happen, elevation increase, speed increase and voltage decrease seems that your battery is not really capable of supporting your load.

I really think you have very low parallel setup something like 12s1p or 12s2p in which recharges too fast and drained too fast.
```

---
## \#6 Posted by: pyttroll Posted at: 2017-04-24T23:26:33.565Z Reads: 63

```
Thanks for the insight, but I do have a 10S5P so theoretically that should not be a problem.
I do however think that I have a bad connection somewhere, can't see any other causes at this point.
```

---
## \#7 Posted by: Eboosted Posted at: 2017-04-25T05:57:56.883Z Reads: 58

```
You battery cut off start is wrong, use 30v and 28v for cutoff end. Is your build dual or single?
```

---
## \#8 Posted by: pyttroll Posted at: 2017-04-25T12:21:32.162Z Reads: 45

```
Yeah, I mentioned that on the first post, but that should not affect the problem.
```

---
## \#9 Posted by: pyttroll Posted at: 2017-04-25T12:31:47.907Z Reads: 43

```
This build is a vanguard, so I have split enclosures.
Yesterday I rewired all the electronics in the motor side enclosure (VESC, switch, buck converter, battery leads...) and took it for a spin this morning, same problem...

So I decided to check the front enclosure, even though I was sure nothing could have gone wrong in there since there are only batteries.

Unsurprisingly, that's where I found the problem.

One of my nickel strip (using 2 layers per cell bank) detached itself from the underlying strip, causing the connection to be very weak, since it was only holding on by a hair, and very susceptible to vibrations.

Took it for a spin and everything is back to normal :slight_smile:
```

---
