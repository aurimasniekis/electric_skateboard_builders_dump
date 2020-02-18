# Charging 6s lipo setup (3 x 2s) thoughts?

### Replies: 11 Views: 340

## \#1 Posted by: Torcn Posted at: 2018-02-06T17:19:35.278Z Reads: 46

```
Hey guys!! I'm building 6s setup on small board with 3 2s lipos. I got balance charger but charging one by one takes forever. I was looking for bms, do you think is worth it? Also what is advantage to use bms not only for charging but also for discharging? Will my packs like be more balanced if I discharge thought bms? Or should I just go with some kind of method to charge multiple packs with the balance charger? 
The priority here is safety and convenience too..
```

---
## \#2 Posted by: dg798 Posted at: 2018-02-06T18:08:06.204Z Reads: 41

```
I think you should just connect the batteries in parallel with a parallel balance board
```

---
## \#3 Posted by: dg798 Posted at: 2018-02-06T18:09:31.179Z Reads: 43

```
Or buy 2 cheap imax b6 clones and charge them at the same time.
I’m not so sure a bms is worth it for 6s. Also you might be able to charge them in series but if something goes wrong then you can get a short so I wouldn’t do that if I were you!
```

---
## \#4 Posted by: Torcn Posted at: 2018-02-06T18:40:49.008Z Reads: 34

```
First I thought about charging with a parallel bord but I read somewhere here that is not safe. Two chargers maybe is to bulky setup
```

---
## \#5 Posted by: krloz Posted at: 2018-02-06T18:41:24.393Z Reads: 29

```
[quote="dg798, post:3, topic:45734"]
Also you might be able to charge them in series but if something goes wrong then you can get a short so I wouldn’t do that if I were you
[/quote]

Can you explain what you mean by this?
```

---
## \#6 Posted by: Blitz Posted at: 2018-02-06T18:43:09.516Z Reads: 25

```
I just returned a imax b6 clone because something fried.
Hobbyking was quite nice and i did not have to pay for return postage.
```

---
## \#7 Posted by: krloz Posted at: 2018-02-06T18:44:08.459Z Reads: 28

```
 If you are only doing 6s you can simply charge them in series just like you discharge them. I'm sure your charger can do 6s.
A bms in discharge will just protect your cells against any of them going under a minimum voltage.  Usually bms don't balance while discharging.  And usually esc take care ou'd cutting out when reaching a certain battery level so discharging through bms usually is not that useful.  Unless your pack is way unbalanced and a cell reached a minimum way before the rest
```

---
## \#8 Posted by: mmaner Posted at: 2018-02-06T18:48:05.499Z Reads: 27

```
THe simplest solution would be to make a x3 2s to 6s adaptor and mount it in the enclosure.  THen you can balance charge all 3 batteries at once with your hobby balance charger.  THe best solution would be to get a 6s BMS and connect it for charge/discharge and use a laptop style charger.
```

---
## \#9 Posted by: Torcn Posted at: 2018-02-06T18:53:12.735Z Reads: 26

```
Is at the bms settings low voltage protection is 2.8v per cell that's to low for lipo cells so discharge through bms is no useful in my case. Mabye get bms and bypass discharge may be the best option
```

---
## \#10 Posted by: mmaner Posted at: 2018-02-06T18:54:38.393Z Reads: 27

```
If you are using a VESC you can set your cutoffs at the VESC.
```

---
## \#11 Posted by: krloz Posted at: 2018-02-06T18:54:44.429Z Reads: 25

```
[quote="Torcn, post:9, topic:45734"]
Mabye get bms and bypass discharge may be the best option
[/quote]

Agree 10 times.  
Because chars
```

---
