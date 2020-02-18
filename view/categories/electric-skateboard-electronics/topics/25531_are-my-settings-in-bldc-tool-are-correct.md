# Are my settings in BLDC tool are correct?

### Replies: 4 Views: 673

## \#1 Posted by: ninja Posted at: 2017-06-16T20:52:37.841Z Reads: 75

```
Hi guys!

I'm about to test my new battery and completely rebuilded board, but before I test it I need to know if my settings are correct in BLDC tool!

So my setup is: SK3 245kv motor, 8s4p 25R battery pack, single drive, 60A BMS, enertion VESC 4.12. Going to use bldc mode. And I'm using  Ackmaniac bldc tool with firmware 2.54

My bigest concerns is about max W, are those 1700w are correct? 
And regen braking. So I do not want that my sistem shuts off from braking with fully charged battery.

So screen shots:
<img src="/uploads/db1493/original/3X/d/f/dffd8402f64d5947f5fdeb66057c5bcc42a8ca8d.jpg" width="690" height="393"><img src="/uploads/db1493/original/3X/2/1/21722a151a564ed6124c3edb2f6c6368cc961ea9.jpg" width="690" height="373"><img src="/uploads/db1493/original/3X/3/e/3e8ced0919d5aa762d055a70e53f56bb7b9269d5.jpg" width="690" height="374"><img src="/uploads/db1493/original/3X/c/1/c11717a384c87ba0c979fbf24bb779b096756081.jpg" width="690" height="374"><img src="/uploads/db1493/original/3X/e/2/e28906a4989e582a509607731654b614798170ff.jpg" width="690" height="377"><img src="/uploads/db1493/original/3X/9/c/9c29ca39d2a29652347c5157fae7cba4b31ef743.jpg" width="690" height="379">

Take care, 
Peace.
```

---
## \#2 Posted by: ninja Posted at: 2017-06-18T20:57:29.903Z Reads: 44

```
I'm about to test my board, but on the bench at full throttle motor is twitching!! I do not want ride board when it twitching and it start doing that from about 70% of throttle.
What causes it? Any ideas?
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-06-18T21:29:26.239Z Reads: 41

```
All looks good. And just stop to torture your board with full speed on the bench.
One small thing. i would recommend to use a linear braking curve. And for the acceleration curve i makes more sense to reduce the power at low % range instead of reducing it at the high percent range.
I recommend these settings for the beginning.
<img src="/uploads/db1493/original/3X/4/9/49eb8b9e0898cdb68fe4845db0befe0a34190d5a.png" width="686" height="499">
```

---
## \#4 Posted by: ninja Posted at: 2017-06-18T22:16:56.100Z Reads: 37

```
Thanx! I'll change braking curve to linear and acelleration curve to your settings.
```

---
