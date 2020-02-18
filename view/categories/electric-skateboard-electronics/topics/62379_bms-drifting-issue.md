# Bms drifting issue

### Replies: 10 Views: 260

## \#1 Posted by: Flaco Posted at: 2018-07-20T17:04:21.534Z Reads: 90

```
Hi, need help diagnosing this. I found 1 pack of 12 unbalanced. After manually balancing and charging it I see that the same pack number 4 keeps loosing voltage. I've replaced with a new pack and the drift continues. Then I disconnected the bms ( bestech hcx-d223v1 ) and this pack keeps voltage perfectly.
Everything points to a failure in the bms to me. I've checked all the wiring and it seems ok.
Any thoughts?
```

---
## \#2 Posted by: E1Allen Posted at: 2018-07-20T17:07:04.974Z Reads: 88

```
BMS issue.
```

---
## \#3 Posted by: Flaco Posted at: 2018-07-20T17:10:54.313Z Reads: 79

```
So there is something else to be done besides replacing it?
```

---
## \#4 Posted by: AutoItKing Posted at: 2018-07-20T19:41:35.413Z Reads: 72

```
Unless you have some electronics training/knowledge it would be best to just replace it. Probably a failed transistor or resistor. Maybe a comparator. Chinese components have fairly high failure rates.
```

---
## \#5 Posted by: b264 Posted at: 2018-07-20T20:42:24.820Z Reads: 57

```
Without knowing any more, it would indicate a BMS issue.  You can also manually inspect the BMS to see if a part is accidentally missing, but replacing it would be a good start.
```

---
## \#6 Posted by: thisguyhere Posted at: 2018-07-20T20:51:08.899Z Reads: 50

```
how much of a drift?
```

---
## \#7 Posted by: Flaco Posted at: 2018-07-21T15:32:23.937Z Reads: 36

```
So as your suggestions I've checked the bms and look this

![IMG_4364|666x500](upload://4nfEKabNKCo5KuAZbwl2KHPWC9y.JPG)
![IMG_4366|375x500](upload://5RIpyA2DuvE4fnB2XY4s5ziIZFJ.JPG)

It's a focboxs bolt in the bms. So easily removed and I was so happy, I thought this was the end of it ... but no.
Now it won't start AND keeps drifting pack 4 from 3.70v to 3.52 in a night.
```

---
## \#8 Posted by: trigger4point7 Posted at: 2018-07-23T17:27:00.188Z Reads: 27

```
It probably shorted out some of the components, I would toss that thing in the trash and get a charging only BMS from ebay.
```

---
## \#9 Posted by: trigger4point7 Posted at: 2018-07-23T19:07:13.309Z Reads: 23

```
I mean, I have a bestech as well, and they do seem to be great, but to get you back on the road, ebay could be a faster alternative.
```

---
## \#10 Posted by: Flaco Posted at: 2018-07-23T19:40:09.586Z Reads: 21

```
I think I found the culprit. Makes sense way the pack number 4 was drifitng.

![Copia%20de%20IMG_4370|666x500](upload://7dSIYExoF70h2gkgv9eWn7j0h9v.JPG)

Although now the e-switch is the one not working, the bms it's always on.
```

---
