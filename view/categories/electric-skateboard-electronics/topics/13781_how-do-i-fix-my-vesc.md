# How do I fix my vesc?

### Replies: 13 Views: 908

## \#1 Posted by: Hummie Posted at: 2016-11-27T20:24:57.184Z Reads: 77

```
My canbus connection broke for the hundredth time and with no lead solder at the store thought J and B weld would be a good idea:weary:   
It's conductive. Don't know what happened but it was fine till now <img src="/uploads/db1493/original/3X/0/d/0d84508afb2bf60b62d8d89e7c325f3d037d0eb8.jpg" width="281" height="499">
Here's a pic of the lights on both. The one with dim lighting is not normal.  It won't run.  Neither will as it's the master. I was trying to connect the other canbus wire
```

---
## \#2 Posted by: zmoney Posted at: 2016-11-27T20:27:20.886Z Reads: 72

```
Have you tried running them individually? Can you also post pictures with the front and back of both vescs w/ the bulk caps?
```

---
## \#3 Posted by: Hummie Posted at: 2016-11-27T20:30:46.311Z Reads: 75

```
I haven't tried running them individually but they're connected in parallel.  <img src="/uploads/db1493/original/3X/8/7/877a351c004e67ac4f331c2e401f4997cec39532.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/7/c/7c8db5cd057d5c57c9de0997a7b93d962f867267.jpg" width="666" height="500">

Thanks for your help!  I'm hoping the lights would indicate something. The one lights up fine, i imagine it's good, the other has that dim flickering red light which isn't right.  What can I do ?
```

---
## \#4 Posted by: Blasto Posted at: 2016-11-27T20:39:46.765Z Reads: 69

```
You most likely shorted out your can bus, when that happens, U401 blows short, shorting out your 3.3v bus.
```

---
## \#5 Posted by: Hummie Posted at: 2016-11-27T20:41:48.708Z Reads: 70

```
Ok. Is that somewhat easy to replace/fix?  Dammmmmmn!!!! No fuiuuujccckkkk!!!!
```

---
## \#6 Posted by: zmoney Posted at: 2016-11-27T20:43:59.549Z Reads: 69

```
Does it connect to the BLDC tool? If so, can you type in faults in the terminal to see what what pops up? [quote="Blasto, post:4, topic:13781, full:true"]
You most likely shorted out your can bus, when that happens, U401 blows short, shorting out your 3.3v bus.
[/quote]

Also in this case, you might have also blown your STM or DRV
```

---
## \#7 Posted by: Blasto Posted at: 2016-11-27T20:44:29.278Z Reads: 64

```
Ya its a fairly easy chip to replace... you can always contact @JohnnyMeduse
```

---
## \#8 Posted by: Blasto Posted at: 2016-11-27T20:46:30.085Z Reads: 64

```
[quote="zmoney, post:6, topic:13781"]
Also in this case, you might have also blown your STM or DRV
[/quote]

It's always possible, but they're most likely ok. The drv's buck converter will be in ocp, the mcu shoud be fine.
```

---
## \#9 Posted by: Hummie Posted at: 2016-11-27T20:46:33.004Z Reads: 64

```
Ok thanks I'll try the bldc tool when I get back home in 3-4 days.  I wasn't sure if it was ok to even have it plugged in but I guess what's done is done.  I'll tell you what it says then. It flickers and doesn't look good
```

---
## \#10 Posted by: Hummie Posted at: 2016-11-27T20:49:53.330Z Reads: 62

```
It's great having you guys around.  Wish there was a guide to how the vesc works and can be repaired for idiots.
```

---
## \#11 Posted by: Blasto Posted at: 2016-11-27T20:53:46.940Z Reads: 59

```
Replace U401, don't burn shit around u401.

Use a proper CAN bus cable next time, jst ph 4pin
```

---
## \#12 Posted by: Hummie Posted at: 2016-11-27T20:55:30.225Z Reads: 59

```
The proper cable always ends up breaking on me and even soldering does too eventually.  I've been talking about potting them for years and should've long ago...likely would've saved me huge downtime
```

---
## \#13 Posted by: Blasto Posted at: 2016-11-27T20:59:23.220Z Reads: 57

```
This

http://www.digikey.com/product-detail/en/jst-sales-america-inc/PHR-4/455-1164-ND/608606

+

http://www.digikey.com/product-detail/en/jst-sales-america-inc/ASPHSPH24K152/455-3082-ND/6009458

For a reliable connection, i ended up getting a whole bunch of these cables, very handy
```

---
