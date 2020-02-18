# Dual VESC in serial?

### Replies: 14 Views: 957

## \#1 Posted by: thisguyhere Posted at: 2017-07-05T21:58:14.356Z Reads: 147

```
This shouldn't be done right, connecting two vescs in serial?

<img src="/uploads/db1493/original/3X/9/d/9ddc5a032d35597b1a18b537a1093361a745754e.jpg" width="598" height="499">
```

---
## \#2 Posted by: Smorto Posted at: 2017-07-05T22:04:46.720Z Reads: 144

```
Correct, don't do that. Use a parallel connector like this one if you don't want to solder multiple wires together like that

<img src="/uploads/db1493/original/3X/d/4/d4b1e955857d433006a4c7d2ecc8db0779cf2059.jpg" width="690" height="459">

.<img src="/uploads/db1493/original/3X/7/5/75c793e42521b89ce7ba143ac91a65cf8ee94161.jpg" width="690" height="459">
```

---
## \#3 Posted by: psychotiller Posted at: 2017-07-05T22:05:28.850Z Reads: 139

```
Not sure...I have always run them parallel. I'm sure there are lots of trademark reasons not too though!
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-05T22:05:33.970Z Reads: 137

```
I mean I guess you could if you used double the voltage, but I'm not sure why you'd do that or what benefits or disadvantages there might be.
```

---
## \#5 Posted by: thisguyhere Posted at: 2017-07-05T22:07:38.060Z Reads: 131

```
yea i'm running parallel connectors now, just curious is all.

thanks yalls.

@psychotiller how's your recovery so far?  i know it's only been a few days.
```

---
## \#6 Posted by: psychotiller Posted at: 2017-07-05T22:08:39.803Z Reads: 124

```
It sucks...Feels like its only been a few days I guess :joy:
```

---
## \#7 Posted by: wafflejock Posted at: 2017-07-05T22:15:54.083Z Reads: 124

```
It seems like that wouldn't work out right.... I mean if the VESCs were just resistor loads at a set resistance then it would basically divide the voltage drop across both of them equally assuming they are equal but in the case where the negative from one VESC goes to the positive of another VESC not sure how it would end up equally dividing the voltage unless they were both driving the same power at the same exact time maybe... seems sketchy.

https://www.allaboutcircuits.com/textbook/direct-current/chpt-5/simple-series-circuits/

Seems like you could have very low resistance on one part of the VESC in series setup and high resistance on the other and end up with all the Voltage being dropped through the one VESC.  I dunno maybe it's the best thing ever but I'm not going to be the first one to try :slight_smile:
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-05T22:16:38.766Z Reads: 110

```
You should do it for science @thisguyhere :laughing:
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-07-05T22:18:12.463Z Reads: 103

```
hard pass hahaha
```

---
## \#10 Posted by: Namasaki Posted at: 2017-07-05T23:01:55.862Z Reads: 97

```
[quote="thisguyhere, post:5, topic:26875"]
yea i'm running parallel connectors now, just curious is all.
[/quote]

Careful, that kind of thinking can get you in trouble.
```

---
## \#11 Posted by: flywithgriff Posted at: 2017-07-05T23:12:06.625Z Reads: 92

```
Happy to see this thread and answers that match what I just did! Instead of connectors I made a splitter wire out of 10awg.
```

---
## \#12 Posted by: chaka Posted at: 2017-07-06T13:54:06.742Z Reads: 68

```
Wiring in series will fry the CAN interface on both VESCs. There are probably a few other bad things that can happen but this is what I have seen in the few cases where a customer wired in series instead of parallel.
```

---
## \#13 Posted by: lowGuido Posted at: 2017-07-06T14:10:00.402Z Reads: 64

```
I ususally advocate outside of the box ideas... not this one. don't do this please.
```

---
## \#14 Posted by: longhairedboy Posted at: 2017-07-06T14:36:18.412Z Reads: 56

```
seems like my kind of recipe for disaster!
```

---
