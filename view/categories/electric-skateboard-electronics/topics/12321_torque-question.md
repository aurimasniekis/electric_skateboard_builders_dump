# Torque Question

### Replies: 9 Views: 659

## \#1 Posted by: BoringOldOrange Posted at: 2016-11-02T16:50:51.156Z Reads: 119

```
I'm running a 8s 10ah>VESC>enertion 6355 and have a question regarding torque as the battery drains. When the battery is near 80% there is noticibly less torque then fully charged. Is this normal? Or should be the same output till it dies?<img src="/uploads/db1493/original/3X/8/c/8c2a63ceabc51914c4fa3ce3a2e4e5512b154ebb.jpeg" width="300" height="500">
```

---
## \#2 Posted by: mmaner Posted at: 2016-11-02T17:02:00.489Z Reads: 113

```
I understand the attraction of Li-Po over Lion is that the delivery of voltage is constant, where Lion voltage is delivered on steeper curve downward as the total voltage falls.  I'm interested in the answer to this as well.
```

---
## \#3 Posted by: BoringOldOrange Posted at: 2016-11-02T17:03:43.382Z Reads: 113

```
That's good to know, I should mention it is a lipo pack.
```

---
## \#4 Posted by: Jinra Posted at: 2016-11-02T17:07:54.326Z Reads: 111

```
What's your battery voltage cutoff start/end? It could be doing the soft backoff due to hitting the voltage floor.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-11-02T17:51:48.321Z Reads: 94

```
@mmaner
@BoringOldOrange
The total voltage of a Li-ion or Lipo pack drops as the pack's capacity is used up. 
As the voltage drops, performance will be diminished accordingly. 

A pack with a lower current capability or discharge rate, will be depleted faster. 
Lipos are capable of very high current while discharging and are relatively compact.  
Li-ion packs can not handle as much current while discharging unless they are substantially larger.
```

---
## \#6 Posted by: BoringOldOrange Posted at: 2016-11-02T17:56:20.395Z Reads: 88

```
Thats good to know, thank for the info. I think I have the bat cutoff set too high so I'll also check that as well!
```

---
## \#7 Posted by: Jinra Posted at: 2016-11-02T18:13:54.663Z Reads: 80

```
For reference, your cutoff start should be about 26v for li-ion 18650's and 28v for lipos.
```

---
## \#8 Posted by: BoringOldOrange Posted at: 2016-11-02T18:15:40.694Z Reads: 78

```
Perfect, thanks again.
```

---
## \#9 Posted by: BoringOldOrange Posted at: 2016-11-02T22:39:33.121Z Reads: 56

```
Just an update... I had my cutoff set to 32 volts! So that changes things quite a bit haha. Thanks guys.
```

---
