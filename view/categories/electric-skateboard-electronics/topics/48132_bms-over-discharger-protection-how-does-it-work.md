# BMS over discharger protection, how does it work?

### Replies: 9 Views: 475

## \#1 Posted by: trigger4point7 Posted at: 2018-03-04T16:26:10.717Z Reads: 84

```
Forgive me if this has already been discussed, just link me if it has.

I have bought a Bestech BMS and I read on the data sheet that it has over discharge protection at 3.0 volts now I realize this will help protect one or all P groups from going down past 3.0. 

My question is, will it cut power to the board once one P group dips below 3.0v, even for a millisecond? I live on a hill and can see where I might do that towards the end of my ride heading home. I'd like to know what to expect.
```

---
## \#2 Posted by: Namasaki Posted at: 2018-03-04T17:01:04.134Z Reads: 80

```
The bms will cut power and the Vescs will turn off. 
However, this is more likely to happen while climbing hills or accelerating because that is when your voltage will sag. 
While coasting and braking downhill, your voltage will not be sagging and will even increase with regen braking so that it is less likely to dip below the detection voltage.
```

---
## \#3 Posted by: trigger4point7 Posted at: 2018-03-04T17:17:31.907Z Reads: 76

```
Thanks @Namasaki. I also saw that the BMS is programmable. Have you ever tried your hand at this to give you a little extra buffer, maybe setting to 2.8v?
```

---
## \#4 Posted by: thisguyhere Posted at: 2018-03-04T17:51:48.863Z Reads: 66

```
@Namasaki is absolutely right. 

here what can happen if sag goes below bms lower cutoff

 http://www.electric-skateboard.builders/t/ate-shit-today-and-loop-keys/33613/30
```

---
## \#5 Posted by: trigger4point7 Posted at: 2018-03-04T19:13:10.122Z Reads: 57

```
Damn. Maybe I made a huge mistake. Perhaps I should have just used a voltometer and a balance charger...
```

---
## \#6 Posted by: thisguyhere Posted at: 2018-03-04T19:29:34.156Z Reads: 50

```
no you're fine, just make sure to set your lower soft cutoff pretty high so the esc can limit current before bms cuts out
```

---
## \#7 Posted by: Namasaki Posted at: 2018-03-04T19:33:57.974Z Reads: 48

```
It is only programmable at the factory. 
3.0 is is a little high for Li-iion. 
It’s best to monitor  pack voltage while riding and not depend on the bms to do it. 
The bms is for protecting battery cells and not for regulating range. 
You could use the Vesc low voltage start to warn you when your getting close.
Set it at 32v-34v depending on the amount of voltage sag you get.
```

---
## \#8 Posted by: trigger4point7 Posted at: 2018-03-04T21:57:31.991Z Reads: 40

```
That's a great suggestion I'll definitely do that. Bummer it's not user programmable, but what are you going to do. I'm running 10s 6p but I'd like to not leave 4, 5, 6 miles on the table if I can avoid it you know.
```

---
## \#9 Posted by: Namasaki Posted at: 2018-03-04T22:03:37.275Z Reads: 38

```
It's better to not run your battery all the way down.
```

---
