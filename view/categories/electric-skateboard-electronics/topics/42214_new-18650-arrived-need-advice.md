# New 18650 Arrived Need Advice

### Replies: 18 Views: 1193

## \#1 Posted by: ZackoryCramer Posted at: 2017-12-29T18:19:22.804Z Reads: 201

```
Hey everyone! I bought 26 18650 LG HG2's and just arrived this morning.<img src="/uploads/db1493/original/3X/f/b/fb618dc7b401dec1f77aebcb71efeafed4fce8ab.JPG" width="666" height="500"> I am planning a 13s2p battery pack with 48v 6ah and 40amp constant output. I'll organize them in this orientation.<img src="/uploads/db1493/original/3X/0/c/0c7d1307b44a426ca4912b6ab801095eeaea7a99.JPG" width="666" height="500"> But I don't have a spot welder, so I am planning to just solder on the battery caps. Is that really bad? I have done a lot of soldering jobs and I guess you just need to minimize the contact time of the solder to prevent cell damage? If anyone built their own li-on packs before, please tell me how you did so and if there's anything I would need to proceed. The BMS and cell brackets are coming this afternoon.
```

---
## \#2 Posted by: Sebike Posted at: 2017-12-29T18:39:21.441Z Reads: 191

```
This would be the ideal occasion of using the search button. Plenty of discussions and info on these topics. Good luck!
```

---
## \#3 Posted by: chsknight Posted at: 2017-12-29T18:53:43.562Z Reads: 187

```
Start here...

https://www.electric-skateboard.builders/t/soldering-iron-for-18650-packs/18626/31
```

---
## \#4 Posted by: barajabali Posted at: 2017-12-29T19:11:56.351Z Reads: 181

```
I can spot weld them for you for a small fee and shipping. 

Other wise soldering cels should only be done with a powerful iron 70+Watts. And minimal length of soldering.

Heat ruins the cells, mostly the negative terminal
```

---
## \#5 Posted by: Namasaki Posted at: 2017-12-30T02:51:38.131Z Reads: 147

```
did you know that 13s will be 54.6v fully charged?
Next question, why 13s, why not 12s 50.4v  or 10s 42v?
```

---
## \#6 Posted by: Sk8Board Posted at: 2017-12-30T03:40:30.404Z Reads: 135

```
use anti corrosive rosin flux and really high heat (I did 855 F but you could do more, more heat only if you need to decrease contact time)
```

---
## \#7 Posted by: overint Posted at: 2017-12-30T07:00:12.630Z Reads: 120

```
Would be interested to know what ESC you are going to use with 13S.
```

---
## \#8 Posted by: FredrikHems Posted at: 2017-12-30T10:07:26.184Z Reads: 110

```
Probably Focbox or similar
```

---
## \#9 Posted by: overint Posted at: 2017-12-30T10:20:59.127Z Reads: 109

```
Doesn't focbox only do 12S?
```

---
## \#10 Posted by: FredrikHems Posted at: 2017-12-30T10:42:41.501Z Reads: 104

```
No. In fact, it is rated for up to 63v or 15s. But you should always leave some headroom for electronics, and not push it to their abselout maximum.
```

---
## \#11 Posted by: darkkevind Posted at: 2017-12-30T11:16:26.163Z Reads: 99

```
Make my spot welder and spot weld them yourself ;)

https://youtu.be/b_kGgPVrcCI
```

---
## \#13 Posted by: ZackoryCramer Posted at: 2017-12-30T18:37:46.455Z Reads: 80

```
Thanks everyone for responding. To answer some poeple's questions, VESC supports up to 60v which is a bit higher than 14s charged(58.8) and I said 48v as the nominal voltage, fully charged would be 54.6v. I just finished soldering them last night(PT). What I did was damping the taps with solder then sandwiching the tab and a short coil of soldering between the 18650 and soldering iron with the damped solder heating the tab and the sandwiched solder melting and sticking to the surface. I did a strength check every time I finished a join and they all seemed fine. Once I finished the parallel joints, the pack because warm for about 20 mins then cooled down. Here's what the pack looks like, sorry I didn't take a picture of the joint.
<img src="/uploads/db1493/original/3X/b/8/b8e6fda2fa78f95076f75c66d289aa319c8d30df.png" width="378" height="499"><img src="/uploads/db1493/original/3X/7/b/7bb1dbca18309357540b54214ecf5f5f8738120c.png" width="595" height="500">
However, once I plugged the xt90 to the Vedder Spark Switch(I soldered myself), there was a light emitting out of the green portion of the female plug and it sparked(ironic right?) and smoked, but only the male connector was badly damaged for some reason. I am now scared to plug the XT90 in again. I haven't tried to directly plug into the VESC but I have check to voltage to be 46.8v which is lower than a fully charged 12s lipo pack I tested earlier.
<img src="/uploads/db1493/original/3X/d/a/da90328cb7949b26bc4cdb1f909e2d927f10d65c.png" width="607" height="500"><img src="/uploads/db1493/original/3X/f/9/f9c0397e7b7f98a67caa2e07c814b7b397a12c1b.png" width="357" height="339">
```

---
## \#14 Posted by: Betsy Posted at: 2017-12-30T19:36:01.942Z Reads: 73

```
You may want to recheck every battery for a burnt connection/solder joint. One of those batteries may have a sign of puffiness. All wired connections must be spot on down to the xt90. I use shrink tube around the xt pos/neg posts. I prefer ec3 or ec5 depending on the amps/voltage. 
Good luck
```

---
## \#15 Posted by: ZackoryCramer Posted at: 2017-12-30T22:59:13.083Z Reads: 69

```
Thanks but I figured out that the problem was the XT-90 anti-spark connector. Just an advice to everyone else, don't use 12s or higher voltage on anti-spark connectors, you will damage both female and male plugs.
```

---
## \#16 Posted by: Acido Posted at: 2017-12-30T23:15:45.203Z Reads: 66

```
You could also use a propane powered soldering thing idk the name just touch it and its connected
```

---
## \#17 Posted by: Betsy Posted at: 2017-12-31T04:15:08.419Z Reads: 57

```
Right on. Be safe ride safe. Happy new year
```

---
## \#18 Posted by: ZackoryCramer Posted at: 2017-12-31T17:40:48.968Z Reads: 51

```
Don't worry, I blaze my 90mm's at 25mph const.
```

---
## \#19 Posted by: florensvb Posted at: 2017-12-31T18:03:47.856Z Reads: 50

```
http://www.electric-skateboard.builders/t/new-single-build-for-my-brother/34155/55?u=florensvb

some information in there as well as here

http://www.electric-skateboard.builders/t/soldering-a-10s2p-samsung-30q/35247
```

---
