# Vesc settings for single drive 6355, 15/36 GEARING

### Replies: 8 Views: 641

## \#1 Posted by: rok Posted at: 2017-07-22T17:39:40.261Z Reads: 102

```
Before i close my VESC in enclosure i want someone to look at my vesc settings. 
I tried to drive on these settings but i feel that the speed and torque is just too low. 
What am i missing?

10s4p
6355 200kv motor
Vesc

Current settings:
<img src="/uploads/db1493/original/3X/1/f/1f17ace6126c29977ada202a868dc73c7a6b3d95.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/8/2/8238cc742787857cae23b68561a8baed01108c29.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/2/8/289523f8b6e64b671ce008f3310b5a02d1bec25b.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/2/d/2df1eeb572950e14a3a394dc97eb22a4463a881f.jpg" width="666" height="500">
```

---
## \#2 Posted by: TranxFu Posted at: 2017-07-22T17:40:51.046Z Reads: 88

```
Whats your battery setup ?
```

---
## \#3 Posted by: rok Posted at: 2017-07-22T17:47:54.067Z Reads: 89

```
10s4p samasung 25r
```

---
## \#4 Posted by: TranxFu Posted at: 2017-07-22T18:01:59.413Z Reads: 85

```
set your cutoff to 30v and cutoff end to 28v then. You can adjust your startup boost by little increments for better start off
```

---
## \#5 Posted by: rok Posted at: 2017-07-22T18:05:03.142Z Reads: 87

```
Uploaded the new settings:
<img src="/uploads/db1493/original/3X/2/d/2df1eeb572950e14a3a394dc97eb22a4463a881f.jpg" width="666" height="500">

what do you think about my current limits?
```

---
## \#6 Posted by: TranxFu Posted at: 2017-07-22T18:14:20.589Z Reads: 84

```
mhm the standard 60a are okay for your setup. This will limit your "power" but go slow and you can adjust later. Set your max input voltage to 57v.
```

---
## \#7 Posted by: Jinra Posted at: 2017-07-22T18:14:41.504Z Reads: 85

```
You can bump up the batt max to about 40 for more available power. Motor max of 60~ will help too. -30 motor min is a bit low for braking and can go higher as well. I usually put it opposite of my motor max. Regen should be -16 at most. Change the max input voltage to 57, no need to change it from default.
```

---
## \#8 Posted by: rok Posted at: 2017-07-23T15:14:43.366Z Reads: 79

```
Thanks for all the solutions and advices guys :thumbsup:
I can climb some really steep hills and today i reached my top speed which was fucking 42km/h. 
Breaking is also fantastic when set to 60A.
```

---
