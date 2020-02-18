# DRV8302 VESC replacement / fix in Sydney-Australia

### Replies: 3 Views: 1245

## \#1 Posted by: rodrigovolkmer Posted at: 2016-11-10T23:31:01.394Z Reads: 79

```
Lately I've done my first buld, thanks to you all in this community for all the amazing information available on a simple search.

My problem was my VESC DRV8302 fried after 5 days of use... didn't use it too hard on the day but it was a big frustration.

<img src="/uploads/db1493/original/3X/d/d/dd4f7f00d892d351fe621403193f194ee80c71f8.jpeg" width="666" height="500">

I already bought another DRV8302 for 10 dollars (with delivery, thanks to RS-Electronics http://au.rs-online.com)
Now I'm on the lookout for someone to replace it for me for a fair price in Sydney (where I live). I made lots of phone calls and found someone willing to do it for $50, which is ok but thought I could find it cheaper.

Going back to why the DRV fried, Don't believe it was my configuration as everything was set minding the low current and low heat. below is my config. if there's something wrong, please let me know.

Baterry: x3 3S 5000mAh - https://hobbyking.com/en_us/turnigy-5000mah-3s-25c-lipo-pack.html
Motor: Turnigy SK3 - 6364-213kv https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html
VESC: MayTech http://www.maytech.cn/en/product/e-skateboard/e-skateboard-esc/e-skateboard-vesc

<img src="/uploads/db1493/original/3X/a/8/a87e4c886687a359077cba3c2a33d4bb2e022790.jpeg" width="690" height="372">

the funniest think (and someone could also explain to me why) whenever I connect the VESC to the BLDC tool, everything works fine, all the readings, real time samples, receives the signal from the PPM RC remote, no fault code at all...
It just doesn't send signal to the motor  (also tested with a multi-test).
the only error message I get is when I try a motor detection:

<img src="/uploads/db1493/original/3X/a/5/a529fc1d2128a6c85201b62711df43f9657663fd.jpeg" width="690" height="366">

but then, as I said, not faults:
<img src="/uploads/db1493/original/3X/7/f/7f29324aefb785b1551d308f8b0761aa44b99f09.jpeg" width="690" height="431">
```

---
## \#2 Posted by: lowGuido Posted at: 2016-11-11T00:16:09.962Z Reads: 60

```
why does the DRV fry? that's really the million dollar question isn't it?
VESC would be the ESC to end all ESC's if only someone could build it with some sort of DRV protection...
```

---
## \#3 Posted by: rodrigovolkmer Posted at: 2016-11-11T00:19:31.196Z Reads: 61

```
that's all I wish to know... it was  trying to break on the flats, and I was going on lower sppeeds... 

I'm already preparing to protect myself with heatsink glued on the DRV and a little 40mm fan on top. hope it helps
<img src="/uploads/db1493/original/3X/b/0/b084cf2ca25cd9756487884726c932e4e5183e29.jpeg" width="690" height="387">
```

---
