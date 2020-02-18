# Over volting a motor

### Replies: 12 Views: 337

## \#1 Posted by: jasonlove199450 Posted at: 2018-12-11T22:28:56.138Z Reads: 97

```
Just wondering what would happen if I ran 12s on this motor ? I've already been running 8s on it which it is rated for and it doesn't seem to even get warm. I did 3D print an adapter for the end of the motor which makes the motor act like a fan drawing air threw the motor.  Will running it on 12s work at all ? if so then does anyone know how long its likely to last if at all ?? Thanks

https://www.ebay.co.uk/itm/270KV-N5065-5065-Brushless-Motor-For-DIY-Electric-Skateboard-Scooter-Multicopter/222798519868?_trkparms=aid%3D555018%26algo%3DPL.SIM%26ao%3D2%26asc%3D20160908110712%26meid%3De9c5121670ef4b428f06eab619dffca4%26pid%3D100677%26rk%3D2%26rkt%3D17%26sd%3D223004576753%26itm%3D222798519868&_trksid=p2385738.c100677.m4598
```

---
## \#2 Posted by: pat.speed Posted at: 2018-12-11T22:37:13.686Z Reads: 92

```
Voltage does not really effect bldc motors. It’s the current that does.

Also it’s 270kv on 12s...are you planning to go to the moon?
```

---
## \#3 Posted by: FredrikHems Posted at: 2018-12-11T22:37:21.337Z Reads: 90

```
12s won't be a problem. The motor can likely do hundreds of volts without any problem. 270 kv is imo way too high for 12s tho.
edit: @pat.speed was faster :frowning:
```

---
## \#4 Posted by: jasonlove199450 Posted at: 2018-12-11T22:39:15.746Z Reads: 87

```
what about 10s ??
```

---
## \#5 Posted by: jasonlove199450 Posted at: 2018-12-11T22:40:36.235Z Reads: 83

```
also what motor do you recomend ? i see people are using 190 kv ? should i go with that ?
```

---
## \#6 Posted by: FredrikHems Posted at: 2018-12-11T22:42:22.347Z Reads: 81

```
270 is too high to be efficient no matter what voltage. Maybe good on 4 or 5s, but no ones really uses that low voltage. 170-190kv is the sweet spot for esk8. Lots of different motors available, use the search tool. :smile:
I am using 130kv at 12s, but thats on a e-mtb. Most guys use 170kv for street builds.
```

---
## \#7 Posted by: jasonlove199450 Posted at: 2018-12-11T22:43:54.535Z Reads: 78

```
alright thanks for the help :smiley:
```

---
## \#8 Posted by: pat.speed Posted at: 2018-12-11T22:53:31.104Z Reads: 71

```
Hehe finally my fingers are fast enough.

Yep I agree with @FredrikHems you can run it at 12s but you would be better to buy a new motor in the 170–190kv range. I like to use the Keda 190 or 195kv motors, that’s just my opinion
```

---
## \#9 Posted by: banjaxxed Posted at: 2018-12-11T23:06:12.376Z Reads: 66

```
A 270kv motor running 12v is a shortcut to a blown vesc 4.x
```

---
## \#10 Posted by: nuttyjeff Posted at: 2018-12-11T23:45:09.884Z Reads: 62

```
[quote="FredrikHems, post:3, topic:77742"]
The motor can likely do hundreds of volts without any problem.
[/quote]

Pretty sure you'll be exceeding the rated speed limit of your motor bearings with that kind of voltage.
```

---
## \#11 Posted by: FredrikHems Posted at: 2018-12-11T23:51:43.285Z Reads: 54

```
I agree. But then its the bearings that gets destroyed, not really a «electrical» component of the motor, like the windings or the stator. If you really want to, you could probably find high speed bearings that replaces the stock ones :grinning:
```

---
## \#12 Posted by: briman05 Posted at: 2018-12-11T23:54:04.854Z Reads: 54

```
Plugging this into 10s or 12s is the fast track to blowing up your vesc. 10s should sweet spot for kv is 190-200 kv
```

---
