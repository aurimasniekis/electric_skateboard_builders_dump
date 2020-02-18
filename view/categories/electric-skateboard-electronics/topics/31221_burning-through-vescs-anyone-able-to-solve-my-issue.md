# Burning through VESCs. Anyone able to solve my issue?

### Replies: 13 Views: 886

## \#1 Posted by: jtreiman Posted at: 2017-08-22T05:56:43.559Z Reads: 145

```
Alright. My first VESC worked out ok, used default settings, landing me with DRV8302 in about 10 minutes. Attempted repair, replaced chip, ran detection, instant 8302. Got upset, ordered new VESC, tuned settings to the best of my ability, ran about 2 miles, I put it away, took it out an hour later to an 8302 error. No visual damage done the any of the 8302s.

My board consists of:
2x Zippy 5800 30C 3 Cells in series
DIY VESC
6354 260Kv
On/Off Switch

Settings before the last 8302:

Motor:
[![](https://i.gyazo.com/eebd46487d9c1c3c42797d2964c9c5db.png)](https://i.gyazo.com/eebd46487d9c1c3c42797d2964c9c5db.png)

BLDC:
[![](https://i.gyazo.com/c9d6520853abe162a0ef2689e84aafb0.png)](https://i.gyazo.com/c9d6520853abe162a0ef2689e84aafb0.png)

Advanced:
[![](https://i.gyazo.com/65016325a8defb77014d9c08713934c6.png)](https://i.gyazo.com/65016325a8defb77014d9c08713934c6.png)

I am willing to fix the VESC if there is a known solution to the problem, otherwise, would love to trade these two boys for something more reliable.
```

---
## \#2 Posted by: Dariks Posted at: 2017-08-22T06:00:58.021Z Reads: 132

```
Ok the main problem is your motor max it should not be 60amps. It should be under 50amps. Do you have pictures of your esc's you may have burned them out
```

---
## \#3 Posted by: Dariks Posted at: 2017-08-22T06:04:09.403Z Reads: 130

```
Also list you motor type and gear ratio and where you are using your board. Some motors draw more amps then the vesc can provide.
```

---
## \#4 Posted by: jtreiman Posted at: 2017-08-22T06:31:30.226Z Reads: 130

```
For motor, i'm running the Turnigy Aerodrive SK3 - 6354-260KV Brushless Outrunner.
Gear Ratio, not sure exactly, but I used DIY 36T ABEC Pulley Combo Kit.
Environment being flat roads.

PICS of VESC below. Melted connectors on first from heat gun, not usage.
<img src="/uploads/db1493/original/3X/2/3/231825579cd113b22eed1f6eb2ac1c25d8a4872e.jpg" width="257" height="500">
<img src="/uploads/db1493/original/3X/8/a/8a38560ad1899e5fa729923074469b8c324905cf.jpg" width="257" height="500">
<img src="/uploads/db1493/original/3X/f/2/f23744678fe4264d3329b1470267be502816b919.jpg" width="257" height="500">
<img src="/uploads/db1493/original/3X/5/e/5e211aa1b507ae6a574014a0242fc241b79910fd.jpg" width="257" height="500">
```

---
## \#5 Posted by: Namasaki Posted at: 2017-08-23T05:01:27.847Z Reads: 101

```
[quote="Dariks, post:2, topic:31221, full:true"]
Ok the main problem is your motor max it should not be 60amps. It should be under 50amps. Do you have pictures of your esc's you may have burned them out
[/quote]

I've been running my motor max at 80a for over a year with no problems.
60a motor max is not the problem
```

---
## \#6 Posted by: Namasaki Posted at: 2017-08-23T05:10:55.452Z Reads: 96

```
Did you run motor detection with belt off and apply and write config?
The reason I asked is that your BEMF Coupling seems a little high

You are well bellow the erpm limit with 260kv at 6s
You do not appear to have the ramp step bug.
You might be getting a short somewhere in the phase wires or inside the motor.  That will definitely cause a drv failure.
Also check and make sure the main positive wire is not shorting on any pcb socket pins.
```

---
## \#7 Posted by: Jinra Posted at: 2017-08-23T05:28:39.501Z Reads: 93

```
Agreed with this, please post detection results
```

---
## \#8 Posted by: Dariks Posted at: 2017-08-24T00:39:11.689Z Reads: 74

```
Now that we eliminated a few possible issues can you post pic's of the motor winding's and the part of wire with heat shrink on it that's usually where shorts occur on that motor. Also check for belt rubbing I had this problem previously caused major problems with heating up the motor. @Namasaki thanks for the clarification.
```

---
## \#9 Posted by: trancejunkiexxl Posted at: 2017-08-24T03:31:28.794Z Reads: 62

```
if your belts are 2 tight it will kill also kill your vesc
```

---
## \#10 Posted by: jtreiman Posted at: 2017-08-24T22:50:39.707Z Reads: 55

```
Repaired the second VESC. C28 resistor was off. Works good now. Will post detection results on motor.
```

---
## \#11 Posted by: jtreiman Posted at: 2017-08-24T22:52:32.582Z Reads: 54

```
https://i.gyazo.com/3369c04cea173ba95c6b9bac9c0a8650.png
```

---
## \#12 Posted by: NickTheDude Posted at: 2017-08-25T04:56:54.020Z Reads: 42

```
Isn't 60 battery amps too high for a typical VESC? I'd imagine you'd be pulling a lot of amps on 6S and I wouldn't be suprised if thats what did it in.
```

---
## \#13 Posted by: onepunchboard Posted at: 2017-08-25T05:28:45.564Z Reads: 40

```
I'm putting 70. I don't have problem. I've seen much higher. before. so probably not the cause
```

---
