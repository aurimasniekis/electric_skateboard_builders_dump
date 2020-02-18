# How to build the fasted board possible

### Replies: 26 Views: 1964

## \#1 Posted by: filmerskier97 Posted at: 2017-05-04T22:40:03.867Z Reads: 227

```
If you were a crazy man and wanted to build the fastest possible RELIABLE board that could hit 35-40mph how would you go about it? what parts would you use?
```

---
## \#2 Posted by: Hummie Posted at: 2017-05-04T22:44:51.658Z Reads: 233

```
if its a diy board and you want to do 40 and you want it reliable I think you need to even out all the kinks in whatever parts you chose before you do that 40.   diy and reliable dont go together at first
```

---
## \#3 Posted by: mmaner Posted at: 2017-05-04T23:42:23.970Z Reads: 226

```
12s6p battery pack with 30Q cells, 200kv 6364 or 6374 motors, VESC-X x2, 107mm Abec 11 wheels, BMs for charge only and max the Bat Max and Motor Max in the VESCs.  That should get you close.
```

---
## \#4 Posted by: Jinra Posted at: 2017-05-04T23:52:50.360Z Reads: 220

```
12s 200kv on a vesc is how you fly at 40mph
```

---
## \#5 Posted by: mmaner Posted at: 2017-05-04T23:58:13.325Z Reads: 215

```
18/36 gears on 107mm wheels = 41.15 mph

http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":12,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":18,"wheel-pulley-teeth":36,"wheel-size":107}|
```

---
## \#6 Posted by: Jinra Posted at: 2017-05-05T00:03:22.530Z Reads: 209

```
to clarify, "fly" as in, you broke your vesc by exceeding erpm limits
```

---
## \#7 Posted by: mmaner Posted at: 2017-05-05T00:16:43.198Z Reads: 208

```
Nope...57456 ERPM.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-05-05T00:46:58.369Z Reads: 198

```
The problem with that Calc is that it doesn't calculate with full charge voltage. 50.4v for 12s
```

---
## \#9 Posted by: JLabs Posted at: 2017-05-05T00:52:22.549Z Reads: 189

```
Big wheels, high voltage, and low reduction ratio = the key to speed 🔑
```

---
## \#10 Posted by: Jinra Posted at: 2017-05-05T00:54:49.662Z Reads: 187

```
50.4 x 200 x 7 x .95 =  67032
```

---
## \#11 Posted by: will_manners Posted at: 2017-05-05T01:01:33.757Z Reads: 184

```
Li-ion pack simply won't be at 50.4V under load. There will always be some degree of sag. 

@filmerskier97 If you want a really high reduction ratio use hub motors, 1 to 1 :) 

Link below, the world record uses 4WD hub motors.

[Fastest speed record on an electric longboard set at 102.9 km/h](https://www.youtube.com/watch?v=Hi3icPBURUA)

[Esk8 Calc; 12S, 170kv, 97mm, Gear ratio 1:1](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":12,"motor-kv":170,"system-efficiency":70,"motor-pulley-teeth":1,"wheel-pulley-teeth":1,"wheel-size":97}|)
```

---
## \#12 Posted by: Jinra Posted at: 2017-05-05T01:16:01.254Z Reads: 180

```
doesn't have to be, with a little decline, there's suddenly low load and you'll be hitting the rpm limit
```

---
## \#13 Posted by: Hummie Posted at: 2017-05-05T01:28:08.004Z Reads: 178

```
<img src="/uploads/db1493/original/3X/8/9/8909709f354e64b35291c1725fbe4b1ef595421f.jpeg" width="666" height="500">I didn't do math but I do 30mph on 90kv hub motors with 81mm wheels and I think u could hit 40 mph with just 120kv hub motors. I can wind you that and Ive got new motors in a couple weeks that match these abec11 centrax 83x78 wheels.

http://www.abec11.com/products/abec11/abec-11-77mm-centrax-77a-80a-83mm-centrax-77a-80a
```

---
## \#14 Posted by: lowGuido Posted at: 2017-05-05T01:37:04.605Z Reads: 171

```
I think I would build an uneven drive board if I was looking for crazy top speed. Have a 170kv and a 200kv on 12S would probabaly be crazy enough.
Or maybe even 280kv and 430kv on 6S...
```

---
## \#15 Posted by: Namasaki Posted at: 2017-05-05T01:51:44.873Z Reads: 171

```
This setup got my 185lbs up to 33mph.
12s Lipos TB 12s ESC's and Carvon 145kv hubs
Maybe with Vescs, I could have got close to 40mph
(Vescs seemed to be much more efficient than those car ESC's)
However, I doubt I would have the courage to go that fast.
Even 30mph was out of my comfort zone.
Note: the blue wheels are 97mm
I did 33mph with my yellow 90mm wheels.
<img src="/uploads/db1493/original/3X/8/f/8fc3e558a79bc584f60ecd5c478b5eb5ae053026.JPG" width="374" height="500">
```

---
## \#16 Posted by: Namasaki Posted at: 2017-05-05T01:57:39.486Z Reads: 169

```
Check this out, 55mph with a dual belt drive.
https://youtu.be/Fm-0SgVSyD8
```

---
## \#17 Posted by: Jinra Posted at: 2017-05-05T01:59:59.151Z Reads: 166

```
While also illegal, testing on a live road like that seems supremely stupid. Who knows what debris or pot holes there are on there, not to mention if you wipe you can easily get run over.
```

---
## \#18 Posted by: Namasaki Posted at: 2017-05-05T02:05:13.366Z Reads: 163

```
Ya, pretty crazy alright. Definitely not for me.
I like to skate in my comfort zone.
```

---
## \#19 Posted by: mmaner Posted at: 2017-05-05T02:14:10.884Z Reads: 160

```
39.65 mph with lipo 10s, 18/32 gears and 107mm wheels.

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":18,"wheel-pulley-teeth":32,"wheel-size":107}|
```

---
## \#20 Posted by: paragon Posted at: 2017-05-05T03:34:19.401Z Reads: 154

```
fastest != 40mph

If you want the fastest, you'd probably want: 
a 2 speed transmission (one for a torquey start, one for a high top end) dual drive with 60+ mm motors (you can go dual diagonal with 80100 motors) 
or you can go quad drive with higher kv motors so you'll have better top end speed (this route is mechanically simpler, but a lot less efficient)
stiff deck with a wide wheelbase
high c lipos or lifepo4 cells (the size of a li-ion pack that could put out the needed amps would likely be impractical)
kelly controller (if going above 12s)
lots of $$$

this is diy; reliability depends on your math, attention to detail, and the quality of the parts you pick
otherwise, just go for the tried and true...
```

---
## \#21 Posted by: Sourcecode Posted at: 2017-05-05T04:46:33.309Z Reads: 139

```
My setup is quite fast - I'm on 12s with 2 vesc-x and 192kV motors, 2 - 6s  lipo's in series, im 100kgs and i easily hit 50-60kmh every day with the 60000 erpm limit. it is a mountain board tho 😊
```

---
## \#22 Posted by: Namasaki Posted at: 2017-05-05T04:58:12.646Z Reads: 136

```
7" wheels ?
```

---
## \#23 Posted by: Sourcecode Posted at: 2017-05-05T05:06:31.100Z Reads: 131

```
I think it's 8" wheels
```

---
## \#24 Posted by: BigBoyToys Posted at: 2017-05-05T06:48:32.668Z Reads: 125

```
https://youtu.be/_5iQlEIksqs

I used 130kv hubs, 12S3P battery and 2 Vesc's which were all from Dexter. Hit 39mph on my first top speed attempt. My V2 Carvon's  hit 35 pretty easy at 12S voltage too.

He's selling competes that already go that fast on his site last time I checked.
```

---
## \#25 Posted by: GhettoFab.rictation Posted at: 2017-11-07T05:43:54.825Z Reads: 64

```
I had no issues with 97mm wheels hitting 40 mph (sorry I'm American) now I'm Makin changes because I fried my 149kv and ate shit lol wasn't too bad but I'm taking that risk going that fast I'm switching to mountain wheels and having hard time finding balanced wheels to go fast enough so I'm going to try the green ada tires and if those don't work it's the tubes. I need a different motor and settings on my vesc though<img src="/uploads/db1493/original/3X/c/c/cc7101036fff56e319905c20aad74baa4eb1875b.jpg" width="690" height="388">
```

---
## \#26 Posted by: GhettoFab.rictation Posted at: 2017-11-07T05:45:29.408Z Reads: 62

```
You guys like my work table haha
```

---
