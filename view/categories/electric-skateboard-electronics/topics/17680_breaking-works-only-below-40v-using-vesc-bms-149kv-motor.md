# Breaking works only below 40v (using VESC, BMS, 149kv motor)

### Replies: 6 Views: 645

## \#1 Posted by: Majid Posted at: 2017-02-14T09:24:14.355Z Reads: 67

```
Hi fellow eboarders,
I had noticed that my eboard doesn't always break when I need it. After some troubleshooting with different type of DIY batteries, I noticed that the breaking only works when the battery is discharged below 40v. I'm using a 10S2P battery. I've three packs from different manufacturers, Panasonic, LG and Sanyo. All three show the same issue. I've tried tweaking the configuration of VESC, but that doesn't seem to help. At least not to the extend of my knowledge.
Here is a screenshot of the VESC configuration: http://oi68.tinypic.com/2622m1f.jpg
Also when breaking above 40v the red light on the VESC flashes 3 times. Any ideas how to fix this?
Thanks.
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-02-14T10:00:20.062Z Reads: 61

```
Set your maximum input voltage to 57V instead of 42V. This value stands for the highest the VESC can handle and not for the highest the battery can handle.
```

---
## \#3 Posted by: Majid Posted at: 2017-02-14T10:27:41.341Z Reads: 59

```
Dude, thank you very much for the quick reply! I'll try it and let you know. Cheers.
```

---
## \#4 Posted by: Majid Posted at: 2017-02-14T16:12:03.926Z Reads: 36

```
Yes, just tested it and it works perfectly. Thanks again.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-02-14T18:43:45.347Z Reads: 27

```
I'm curious why we don't set max voltage to 60v
Isn't 60v the max that Vesc can handle?
Or is 57v to allow some headroom?
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-02-14T18:46:16.884Z Reads: 28

```
Correct. But normally you should never reach these high volts. And when you reach them because of a problem you want to give the vesc the chance to shut down before it would damage the components. So you set it a bit lower so that the vesc can react.
```

---
