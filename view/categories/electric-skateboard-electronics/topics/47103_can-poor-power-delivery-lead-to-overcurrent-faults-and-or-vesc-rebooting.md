# Can poor power delivery lead to overcurrent faults and/or VESC rebooting?

### Replies: 5 Views: 290

## \#1 Posted by: Jinra Posted at: 2018-02-22T02:05:08.204Z Reads: 57

```
Please let me know if you've encountered VESC rebooting during your ride! It's incredibly hard to diagnose an issue when your fault codes get wiped by a VESC reboot.

I currently ride in FOC with a 10s4p 30Q battery connected via a 14 awg parallel connector. The battery wire is 12 awg and runs about 3 inches. The parallel connector runs another 3-4 inches and the 10 AWG VESC connector adds another 2-3 inches. All in all that's about 8-9 inches.

I'm curious to know if either 1.) The length of the connection or 2.) the size of the parallel connector (14awg) is causes these reboots on my VESC. The reboots only happen after I hit a large hole/dip/obstacle that causes a large vibration on the board.
```

---
## \#2 Posted by: scepterr Posted at: 2018-02-22T02:07:22.454Z Reads: 55

```
Sounds like a bad connector, or solder joint somewhere
Check all your connectors, see if you find burn marks either inside the female end or the tips of the male ends, replace those
One other thing I can think of is if you have any wires that were flooded with solder and strands broke under the silicone sleeving
```

---
## \#3 Posted by: ARetardedPillow Posted at: 2018-02-22T02:10:20.684Z Reads: 50

```
This happened to me too, twice in around a week. On both occasions it happened right after extremely heavy braking
```

---
## \#4 Posted by: barajabali Posted at: 2018-02-22T02:19:12.026Z Reads: 44

```
Ive had reboots when the battery cant deliver the amps needed. Instantly stopped happening with a more beefy battery

Also it did not happen when the battery was fully charged, tended to happen when the battery was closer to depleted which told me that it was indeed a power delivery issue
```

---
## \#5 Posted by: Eboosted Posted at: 2018-02-22T02:30:18.031Z Reads: 41

```
I had several reboots per minute, diagnosing was pretty hard but at last I was able to find the problem reading the datalog.

[img]https://www.electric-skateboard.builders/uploads/db1493/original/3X/3/8/38b67516b92b1b598c1a9f2019cbd8de52d82735.png[/img]

Check duty cycle on the log, it means throttle is being applied, now check motor current it goes to 0, that means power is being cut off by the VESC probably because of rebooting and it comes back again, this means your RC signal is stable, if you go to faults you can see if it's and overcurrent (usually induced by a power cut on the BMS) or overvoltage (usually a short because of bad connection on the battery, like a broken nickel strip)
```

---
