# VESC releases breaks when in FOC and other issues

### Replies: 7 Views: 918

## \#1 Posted by: Lizardking0069 Posted at: 2016-08-22T01:09:30.031Z Reads: 112

```
Today I switched from BLDC, which works quite well on my setup, to FOC. I followed all steps on from Vedder's youtube video and set out to test it. 

The motor sound is drastically reduced! However, when I apply the breaks they work for a second then just give up and I return to free wheel. Then, if I accelerate, there is a delay of about half a second where the motor turns very slowly and all of a sudden VERY fast. 

I returned to BLDS and it worked flawlessly. Any ideas what could be causing this? 

My setup:
TB VESC v 4.12 firmware 2.18
TB 6355 sensored motor (running sensorless)
8s 5200mah 35c lipo
nunchuck
Default BLDC software settings
```

---
## \#2 Posted by: Bender Posted at: 2016-08-22T01:19:07.243Z Reads: 107

```
After it does this DON'T turn off your board and plug in the vesc to your computer and check the faults (type "faults" in the command line tab)
I'm sure there's some useful info
```

---
## \#3 Posted by: Lizardking0069 Posted at: 2016-08-22T01:26:16.989Z Reads: 107

```
Ok will do, thanks!
```

---
## \#4 Posted by: devin Posted at: 2016-08-22T02:59:47.657Z Reads: 101

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#5 Posted by: treenutter Posted at: 2016-08-22T04:13:21.545Z Reads: 91

```
@Lizardking0069 I had the same braking issue using nunchuck and FOC. I solved it by swapping to a GT2B. My working theory is that the nunchuck's resolution of signal status isn't fine enough to use in FOC. I'm sure there is a better explanation, but I similarly couldn't get it to work.

Also, others have noticed that configuring FOC after a fresh firmware flash seems to fix some bugs, because some settings from BLDC seem to permeate even after you switch modes.

Have you adjusted your battery settings and voltages for your setup in BLDC Tool? If not give that a try.
```

---
## \#6 Posted by: Lizardking0069 Posted at: 2016-08-23T20:43:15.062Z Reads: 64

```
I'll try it out using a ppm based controller. If that is the case i'll keep bdlc and nunchuck. I really love the nunchuck.
```

---
## \#7 Posted by: sl33py Posted at: 2016-08-23T20:52:23.412Z Reads: 61

```
if you like thumb throttle you can also check out the baby bufflo GT2b case mod.  

My GF loves her kama nunchuk, but there are still infrequent disconnects from interference when riding (lots of apartments and 2.4 interference i'd guess).  She goes _really_ slow so it's not been an issue so far.  But i'm planning one of the next GT2b's i do to use the baby buffalo case for her.
```

---
