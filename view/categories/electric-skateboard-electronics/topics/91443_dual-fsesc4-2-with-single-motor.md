# Dual FSESC4.2 with single motor?

### Replies: 13 Views: 179

## \#1 Posted by: 3LD Posted at: 2019-04-23T00:34:21.403Z Reads: 61

```
My Dual FSESC4.2 Plus just arrived, but I'm still waiting on my 2nd motor and mount.  
Can I run it safely on a single motor?
```

---
## \#2 Posted by: mmaner Posted at: 2019-04-23T00:42:32.302Z Reads: 61

```
No, you cannot stop the voltage throughput to the salve VESC.so you will burn it up if you try.
```

---
## \#3 Posted by: ZachTetra Posted at: 2019-04-23T01:02:09.715Z Reads: 58

```
What about with a Unity (friend of mine bought the Easter sale Unity but only has a single motor)?  How long can you go if a motor on a dual dies?
```

---
## \#4 Posted by: kuphjr Posted at: 2019-04-23T01:13:52.599Z Reads: 57

```
This is a good question. I'm really curious now...
```

---
## \#5 Posted by: M.Hboards Posted at: 2019-04-23T01:17:25.039Z Reads: 52

```
@mmaner Doesent flipsky have a switch to disconnect the internal can bus connection so you can run it as a single vesc and since the can bus is disconnected no ppm signal/ power will go to the slave?
```

---
## \#6 Posted by: mmaner Posted at: 2019-04-23T01:24:17.257Z Reads: 51

```
Yes, there is a can bus switch. No it doesn't stop powering the 2nd vesc. I tested it for my own amusement.
```

---
## \#7 Posted by: mmaner Posted at: 2019-04-23T01:24:37.383Z Reads: 50

```
I don't have a unity so I cannot say.
```

---
## \#8 Posted by: M.Hboards Posted at: 2019-04-23T01:26:48.087Z Reads: 49

```
So the vesc still sends power to the phase leads even if you disconnect the can bus?
```

---
## \#9 Posted by: mmaner Posted at: 2019-04-23T02:35:34.290Z Reads: 44

```
As I understand it.
```

---
## \#10 Posted by: mmaner Posted at: 2019-04-23T02:39:18.667Z Reads: 41

```
Can makes control sync, it doesn't actually change anything about power delivery regarding on/off
```

---
## \#11 Posted by: M.Hboards Posted at: 2019-04-23T02:48:02.407Z Reads: 36

```
From the pic below you can see why i thought it can be used in single mode. Doesent can deliver the ppm signal meaning if no signal is given no power is given to the motors just like having the vesc plugged into a battery but is not being used? Also it appears that the plus version doesent have the can switch.

![Capture%20_2019-04-22-22-41-22~2|283x500](upload://3bYC0PWJCZax9BPSRlAf6O5tPg1.jpeg)
```

---
## \#12 Posted by: mmaner Posted at: 2019-04-23T03:28:10.916Z Reads: 35

```
I understand that if you turn off can and have no PPM connected it SHOULDN'T send power to the phase leads. What it does do is power the VESC regardless of can and there is some deviation in output voltage on the 2nd vesc. I don't know why but there is, I tested it in both of mine. 

It's a random increase/decrease in voltage on the 2nd VESC but it increases when PPM is activated on the 1st VESC and decreases when PPM falls off on the 1st VESC.
```

---
## \#13 Posted by: 3LD Posted at: 2019-04-29T01:24:22.724Z Reads: 16

```
Don't do it says Flipsky. 
![dnt|690x131](upload://5oZDrZPwnY3J4BQuJEFJfA4gkOB.jpeg) 

and I'm either blind, or they've removed the canbus switch on the newer dual 4.20 plus with the surface mount caps
```

---
