# Bigger Batteries?

### Replies: 14 Views: 684

## \#1 Posted by: SoapyToad Posted at: 2017-07-07T15:10:39.015Z Reads: 85

```
Hi, so I had a question about batteries and the VESC. The VESC is rated for 50A continuous, but is that set by the BLDC tool (battery max) or is it limited by the actual batteries. My current set up is (x2) 5200 mAh lipos at 10c discharge, which I choose because 5.2*10= 52A continuous. I want more range, but am afraid that if I add more batteries it will exceed this limit. I could very well be wrong so please let me know :)
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-07T15:14:08.263Z Reads: 85

```
Current limitation on the VESC is a hardware limitation. Go higher and you're likely to fry something. For your battery, the better the C rating or discharge rating, the better. The discharge rating for a battery is merely the max **potential** output of the pack. You'll never want to pull anywhere near the max discharge on a battery, but it technically can go that high. The reason you want higher C-rate/discharge is because the more potential the less voltage sag will occur under load.
```

---
## \#3 Posted by: SoapyToad Posted at: 2017-07-07T15:17:30.397Z Reads: 79

```
sweet, So i can technically throw whatever size batteries I want in my build as long as i dont program my VESC above 50A?
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-07T15:18:46.929Z Reads: 76

```
Yep, there's a "Battery Max" setting in there. Just don't put anything over 50A and you should be fine. If you're running Li-ion cells, you'll want to make sure your pack has enough discharge potential too. Most Lipo packs should output at least 50A though.
```

---
## \#5 Posted by: SoapyToad Posted at: 2017-07-07T15:20:41.827Z Reads: 71

```
great to know thanks :smile: Now I know what my next upgrade will be! my current setup rides really nice, but I have noticed I cant go really far, maybe like 8-10 miles :(
```

---
## \#6 Posted by: SoapyToad Posted at: 2017-07-07T15:21:26.875Z Reads: 67

```
what are the pros and cons of Li-ion vs Lipo?
```

---
## \#7 Posted by: Jinra Posted at: 2017-07-07T15:24:46.279Z Reads: 56

```
Prismatic lipos have much higher discharge potential at the expense of lower energy density for its weight and a bit more volatile nature. An overcharged/uncharged or physically damaged lipo can have explosive consequences.

Cylinder cell li-ions are higher in energy density per weight and are safer, with some cells having its own internal fuse to avoid catastrophic failure. The cells are also easy to orient in various positions to suit your needs. These benefits, however, come with the cost of much lower discharge potential. For esk8, you're looking at about 20A discharge potential per parallel cell.
```

---
## \#8 Posted by: SoapyToad Posted at: 2017-07-07T15:32:46.436Z Reads: 50

```
So to make a Li-Ion pack, I take N number of cells and just solder them in parallel and series, until I receive my target size/amp. I dont really need to worry about my discharge rate as long as it is strong enough? I cant exceed a max because the VESC controls its max discharge?
```

---
## \#9 Posted by: Jinra Posted at: 2017-07-07T15:50:37.974Z Reads: 49

```
You can solder them, but spot welding is generally regarded as better for the cell. If you're going to solder, make sure your iron is very hot and you don't make contact for more than a couple seconds.  

You do have to worry about discharge rate as you want to have an adequate amount. You can and want to exceed your "battery max" setting on the VESC to minimize voltage sag.
```

---
## \#10 Posted by: SoapyToad Posted at: 2017-07-07T15:53:38.472Z Reads: 49

```
Thanks for the help! I've seen the 18650 batteries used a lot in builds. Is there any reason people choose that one/is there any specific cell you would recommend?
```

---
## \#11 Posted by: Jinra Posted at: 2017-07-07T15:54:37.296Z Reads: 46

```
18650's have a good size to performance ratio which is why they're popular. I use Samsung 25R's myself, but if I were to build a new pack I'd use Samsung 30Q's
```

---
## \#12 Posted by: wafflejock Posted at: 2017-07-07T15:58:27.275Z Reads: 46

```
18650s are used in lots of hand held power tools and laptop battery packs (not  to mention Tesla power walls and cars) so since they're very widely used they also get the benefit of economy of scale, they are widely accessible in this form factor and cheap.  Keep in mind form factor doesn't equal chemistry, you can have a square package with the same chemistry as a cylinder or two cylinders with different chemical make up.
```

---
## \#13 Posted by: SoapyToad Posted at: 2017-07-07T16:01:59.780Z Reads: 47

```
Do Li-Ions have the same properties as LIPOS in terms of cutoff voltage? for example my lipos charge to 4.2v to and stop at 3.5v per cell.
```

---
## \#14 Posted by: Jinra Posted at: 2017-07-07T16:09:55.232Z Reads: 45

```
You have to review the discharge curve of the cell you're looking at. 18650's can typically go as low as 2.5v, but you want to stay away from the voltage cliff (in the discharge curve) in order to prolong cell life.

For example, in the picture below you don't want to go below the voltage at the cliff where the line falls off.

<img src="/uploads/db1493/original/3X/d/d/ddaa0a84ab941f0cf1145657a24a5be663d05c88.png" width="690" height="345">
```

---
