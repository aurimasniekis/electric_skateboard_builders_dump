# Slave motor randomly disengaging

### Replies: 20 Views: 686

## \#1 Posted by: Eboosted Posted at: 2018-03-16T20:54:13.864Z Reads: 129

```
It started to happen 1 hour ago, any pointers before I tear the board down?

https://youtu.be/UKO4bKY1zuU
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-03-16T21:00:47.988Z Reads: 127

```
cold solder somewhere?
```

---
## \#3 Posted by: pat.speed Posted at: 2018-03-16T21:21:19.758Z Reads: 118

```
Loose phase wire?
```

---
## \#4 Posted by: Deckoz Posted at: 2018-03-16T22:46:23.028Z Reads: 110

```
Canbus or split ppm?
```

---
## \#5 Posted by: Eboosted Posted at: 2018-03-16T23:00:57.294Z Reads: 101

```
Canbus, are there any known issues?
```

---
## \#6 Posted by: Deckoz Posted at: 2018-03-16T23:10:46.576Z Reads: 100

```
I always glue/tape my canbus wired in because canbus vibrating loose from iffy Plastic jst connectors is likely what causes most people's issues with canbus and slaves dying or having the settings reset on thier own.
```

---
## \#7 Posted by: Eboosted Posted at: 2018-03-17T05:34:29.219Z Reads: 90

```
I glued the can bus wire with hot glue, but the issue persisted. So I'm pretty sure I have a shot ESCape :cry:

https://www.youtube.com/watch?v=NjwE8Z1Ncbc&feature=youtu.be
```

---
## \#8 Posted by: Exiledd_Top Posted at: 2018-03-17T06:16:23.798Z Reads: 88

```
Try splitting ppm wire and configuring the second vesc maybe u just shot the can bus port and the escape works perfectly try a servo y splitter
```

---
## \#9 Posted by: Exiledd_Top Posted at: 2018-03-17T06:17:16.998Z Reads: 88

```
But if I recall there's a problem with vesc 6 hardware with ppm wire y splitter has to have no ground or something like that
```

---
## \#10 Posted by: Namasaki Posted at: 2018-03-17T17:19:20.683Z Reads: 71

```
As anyone ever actually had a problem using split ppm on Vesc 6 or is it just a theory.
The reason I ask is because the theory was suppose to apply to Vesc 4 as well and was proven wrong.
```

---
## \#11 Posted by: Deckoz Posted at: 2018-03-17T17:36:33.077Z Reads: 73

```
There was a thread on here with a vesc6 beta tester.. but they received it after the schematic of the vesc6 was release in Nov 2016 if I'm not mistaken..I'll edit if I can find the thread
```

---
## \#12 Posted by: L3chef Posted at: 2018-03-17T19:09:43.809Z Reads: 73

```
Sensor or sensorless? This happened to me last year with a 4.10 vesc. It was the hall sensor wire that was broken.
```

---
## \#13 Posted by: Eboosted Posted at: 2018-03-17T21:21:27.962Z Reads: 72

```
Ok, I have found the issue. 

This is important for two things:

1. ESCape is still ok
2. I 'm gonna sleep good tonight
3. I'm learning a lot, in this case I've learned that overvoltage faults are "always" caused by erratic connection on the power supply, this means bad solder connections between battery packs, ESC power lines or broken ESC capacitors legs.

https://www.youtube.com/watch?v=_KvFTwoQVAc
```

---
## \#14 Posted by: Eboosted Posted at: 2018-03-18T01:03:59.422Z Reads: 59

```
Damn, problems again.

Now, I'm getting this issue:

Fault            : FAULT_CODE_DRV
Current          : -3.9
Current filtered : -0.5
Voltage          : 46.57
Duty             : 0.014
RPM              : 0.0
Tacho            : 616
Cycles running   : 2
TIM duty         : 117
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 8400
Comm step        : 3
Temperature      : 38.58
DRV8301_FAULTS   : | FETLC_OC | GVDD_OV |
```

---
## \#15 Posted by: scepterr Posted at: 2018-03-18T01:21:00.601Z Reads: 54

```
Maybe caps got damaged? Try without the caps on the PCB?
```

---
## \#16 Posted by: Eboosted Posted at: 2018-03-18T01:37:13.371Z Reads: 52

```
That might be the issue, but before failing again I was able to run really stromg for 1km
```

---
## \#17 Posted by: scepterr Posted at: 2018-03-18T01:39:23.328Z Reads: 50

```
Sounds like the cap or the trace from the cap
```

---
## \#18 Posted by: RedEagle Posted at: 2018-03-18T02:30:43.546Z Reads: 45

```
[quote="Eboosted, post:14, topic:49304"]
GVDD_OV
[/quote]

Unstable ground line. On hw 4.xx it's solved by putting another cap parallel to c18. Don't know how to solve it with your hardware though.

Edit: mostly happens in foc mode
```

---
## \#19 Posted by: Eboosted Posted at: 2018-03-18T18:13:51.853Z Reads: 34

```
That's great to hear, the legs on the caps were very short, I soldered them back but I guess they broke again, I'm gonna try to find those caps locally
```

---
## \#20 Posted by: RedEagle Posted at: 2018-03-18T18:18:17.981Z Reads: 32

```
http://vedder.se/forums/viewtopic.php?f=5&t=68&p=318&hilit=c18+gvdd#p318
```

---
