# Hall sensor location on vesc?

### Replies: 11 Views: 1637

## \#1 Posted by: MannyM0E Posted at: 2018-01-31T23:48:19.439Z Reads: 143

```
Just got a hall sensor I think it's called from DIY 
Question is where do I put it in the vesc ?
```

---
## \#2 Posted by: Namasaki Posted at: 2018-01-31T23:58:39.491Z Reads: 137

```
![a86bd0202f208651b56d2d4dd1cb653c379d55b8_1_690x460|690x460](upload://tjJ4RbQgGTVa3ICEyzdTBlQAiqR.png)
```

---
## \#3 Posted by: MannyM0E Posted at: 2018-02-01T00:06:51.456Z Reads: 130

```
Thank you was trying to find this. Could delete thread if you like
```

---
## \#4 Posted by: Namasaki Posted at: 2018-02-01T00:25:24.252Z Reads: 129

```
Better to leave this thread up for others to reference.
I found this pic on another thread under a different topic.
```

---
## \#5 Posted by: ZackoryCramer Posted at: 2018-02-01T00:35:44.736Z Reads: 123

```
Ha. I remember the first time when I was trying out BLDC sensored. Every time I ran sensor detection, the VESC shuts off like there's a short. Realised after 2 weeks, I plugged the sensored cord into program/debug port :rofl: and since it was DIY VESC, the sensor port was hidden by the 10awg wires. Had a big facepalm afterwards.
```

---
## \#6 Posted by: MannyM0E Posted at: 2018-02-01T01:38:16.890Z Reads: 107

```
Just installed the Hall Sensor onto the VESC, selected sensor and configured everything with my motor on the VESC Program. But I really didn't noticed anything different on my ride. Did I do something wrong ? 🤔
```

---
## \#7 Posted by: krloz Posted at: 2018-02-01T01:43:57.119Z Reads: 101

```
What were you expecting to notice? 
Before using sensors did you have to foot push to start?  If yes check now starting from a full stop. 
By the way.  After configuring sensors did you set sensor or hybrid?
```

---
## \#8 Posted by: MannyM0E Posted at: 2018-02-01T23:52:39.188Z Reads: 80

```
I still have too push. Nothing changed for as all I know. I selected sensor. Hybrid I didn't a option for that
```

---
## \#9 Posted by: krloz Posted at: 2018-02-01T23:57:46.667Z Reads: 76

```
[quote="MannyM0E, post:8, topic:45204"]
Hybrid I didn’t a option for that
[/quote]
Here
![20180202_005710|690x361](upload://5IWlVPL3U9wEKRp3LzFpkhewqZY.png)
```

---
## \#10 Posted by: MannyM0E Posted at: 2018-02-02T00:28:09.962Z Reads: 66

```
Will the hybrid be fine with 9s ?
```

---
## \#11 Posted by: ZackoryCramer Posted at: 2018-02-02T00:33:37.394Z Reads: 60

```
hybrid is compatible with any voltage/setting compatible with full-sensored or non-sensored setup with hall-sensors.
And the snwer is yes, 9s is fine.
```

---
