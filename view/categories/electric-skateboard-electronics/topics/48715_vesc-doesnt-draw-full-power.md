# VESC doesn&rsquo;t draw full power

### Replies: 7 Views: 326

## \#1 Posted by: Der6FingerJo Posted at: 2018-03-10T19:17:16.866Z Reads: 61

```
Hey everyone 
A buddy of mine is using 2x esk8 VESC 4.12 in his mountainboard and he's got a the weird problem that his setup only draws ~1400W total.

Here is his setup: 
2x esk8.de 170kv 3kW Motors
2x esk8.de 4.12 VESC
Zippy 10S 8000mAh Lipo
15:80 Belt Transmission

We tried in FOC and BLDC and didn't touch anything in VESC Tool besides Motor Detection and different Motor/Battery max combinations (of which all should have used much more than 1400W in dual). The Turnigy Wattmeter only shows 1400W even with full throttle (which is also fine) and i don't know what to test further. His whole driving experience isn't that great so there's definitely no fault in the wattmeter.

 I'd consider myself as fairly good with VESCs so i don't know where to begin troubleshooting. Any input would be appreciated!
```

---
## \#2 Posted by: scepterr Posted at: 2018-03-10T19:22:39.167Z Reads: 54

```
Could the wattmeter be limiting current, is it inline or a sensor meter?
```

---
## \#3 Posted by: myreala Posted at: 2018-03-10T19:24:05.043Z Reads: 52

```
Have you tested under load? Set battery max to 30 each then it should be drawing 1080W per VESC under heavy load.
```

---
## \#4 Posted by: Der6FingerJo Posted at: 2018-03-10T19:26:06.150Z Reads: 49

```
It's inline and i also thought about it.  It's a 100A 60V turnigy wattmeter so that at least shouldn't be part of it's function. You also can't find anything online about that. I will urge im to try without meter but i don't know if it's easily removable since he bought it used.

@myreala the wattmeter shows peak values and they were produced while driving. I've tried it myself, could pull full throttle and barely move.
```

---
## \#5 Posted by: scepterr Posted at: 2018-03-10T19:27:33.210Z Reads: 50

```
I definitely would first try without the wattmeter
```

---
## \#6 Posted by: louwii Posted at: 2018-03-10T20:36:14.942Z Reads: 36

```
You can also buy a bluetooth module (it's dirt cheap), and use Ackmaniac's app on your phone to check the real time values.
```

---
## \#7 Posted by: Der6FingerJo Posted at: 2018-03-10T20:38:17.705Z Reads: 31

```
Thanks! Didn't think of that, will tell him.

Currently we are suspecting the antispark switch, didn't know it had one before :smile:
```

---
