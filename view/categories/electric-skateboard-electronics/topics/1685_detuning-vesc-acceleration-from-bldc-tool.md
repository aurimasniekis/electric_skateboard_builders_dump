# Detuning VESC acceleration from BLDC tool

### Replies: 4 Views: 1413

## \#1 Posted by: DougM Posted at: 2016-03-06T04:23:28.445Z Reads: 98

```
Has anyone played around with decreasing the acceleration rate from BLDC tool?  I recall there is a way to do it but my Google fu isn't finding what I'm looking for.

I played around with Backoff and Ramping, but it didn't seem to make a difference.  I need to setup the board for some beginners.

Thanks for any help or pointers,

DougM
```

---
## \#2 Posted by: Dedbny Posted at: 2016-03-06T04:45:33.310Z Reads: 99

```
Try chnaging the max erpm in motor control settings.


24,500 erpm will get you a very nice 20-24km/h great speed for learning, 
 From there 36,000erpm is 30km/h good top speed and 18,000erpm and amp limit at 20amp will give for a very basic board 16km/h not huge acceleration power.
```

---
## \#3 Posted by: NerijusM Posted at: 2016-03-07T09:46:43.097Z Reads: 77

```
Try Startup Boost value
<img src="/uploads/db1493/original/2X/d/d27bc4f8b0e139db011c2d6be505047688f590e7.png" width="657" height="472">
```

---
## \#4 Posted by: DougM Posted at: 2016-03-08T05:50:38.825Z Reads: 67

```
Thanks, I'll try both of these approaches and let you know how they work out.  

DougM
```

---
