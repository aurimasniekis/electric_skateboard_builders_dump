# VESCs crash under load. Did I kill my VESCs

### Replies: 10 Views: 244

## \#1 Posted by: mojoo999 Posted at: 2018-09-30T06:09:03.090Z Reads: 113

```
I recently switched to FOC from BLDC and it was working fine for a few miles. Then it just stopped responding under load(when I'm riding on it). The motors still spin on the test bench.  I even switched back to BLDC but it's still not running under load. No faults showing in VESC tool. Did I kill my VESCs? Did I kill one of them or both of them?

My setup:
Dual TB 6355 motors
10s5p Samsung 30q
Two flipsky 4.12 VESCs over CAN

Motor max: 40
Motor min:-40
Battery max: 20
Battery regen: -10
```

---
## \#2 Posted by: b264 Posted at: 2018-09-30T06:22:39.661Z Reads: 107

```
Are you using sensors?  If you push to start rolling first, does it work then?
```

---
## \#3 Posted by: mojoo999 Posted at: 2018-09-30T06:23:42.794Z Reads: 106

```
Yes I'm using sensors. Push to start doesn't work either.
```

---
## \#4 Posted by: b264 Posted at: 2018-09-30T06:27:38.849Z Reads: 101

```
Did you do motor detection and hall sensor detection in FOC mode with no belt on the motor?
```

---
## \#5 Posted by: mojoo999 Posted at: 2018-09-30T06:29:06.054Z Reads: 99

```
I did it with the belt on the motor.
```

---
## \#6 Posted by: b264 Posted at: 2018-09-30T06:30:43.733Z Reads: 100

```
Try it with no load on the motor and if that doesn't work, post screenshots of your settings after clicking "read" on each screen
```

---
## \#7 Posted by: Acidfie Posted at: 2018-09-30T09:49:13.275Z Reads: 78

```
Motor max: 40 -> 60A
Motor min: -40
Battery max: 20 -> 80
Battery regen: -10 -> -15

You can easily change these settings. Check your startup boost to 0.04 for more power out the stand.

EDIT: My bad, -15(!)
```

---
## \#8 Posted by: b264 Posted at: 2018-09-30T10:42:15.029Z Reads: 69

```
Battery regen should be less than zero
```

---
## \#9 Posted by: mojoo999 Posted at: 2018-09-30T15:00:29.440Z Reads: 51

```
I’ve tried different settings already. I think it’s a hardware issue. Maybe a faulty BMS that’s limiting current output? I’ll try to run it without the BMS.
```

---
## \#10 Posted by: mojoo999 Posted at: 2018-10-02T19:18:02.874Z Reads: 25

```
So I tried to run it with BMS bypass but still no luck. Power is still cutting off under load. No idea what it could be now.
```

---
