# Flipsky power switch fix?

### Replies: 15 Views: 634

## \#1 Posted by: Bart_Dood Posted at: 2019-03-20T17:57:09.727Z Reads: 128

```
I have a moderately powered dual VESC board at 40 volts, I've been trying to get a soft switch that works for it, but all the Flipsky soft switches are junk and fail after a few uses and stay on.

Has anyone come up with an actual fix for this yet? last time I looked several months ago it seemed like folks were trying different main power FET's etc to fix it but it wasn't clear if that even worked.

The rainy season is ending and I really want to get my board fixed so I can enjoy it, any help appreciated
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-03-20T17:59:42.232Z Reads: 127

```
It's not worth fixing
```

---
## \#3 Posted by: psychotiller Posted at: 2019-03-20T17:59:47.844Z Reads: 125

```
Loop key. As I'm finding lately. ALL mosfet switches suck it.
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-03-20T18:00:02.603Z Reads: 127

```
Except for if it's precharged
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-03-20T18:01:04.685Z Reads: 124

```
Doesn't the Unity have a good built in switch?
```

---
## \#6 Posted by: psychotiller Posted at: 2019-03-20T18:02:15.301Z Reads: 122

```
unity, and 100a maytech Vescs have built in switches. Pretty much the only way to go if you don't want to Loop key
```

---
## \#7 Posted by: Bart_Dood Posted at: 2019-03-20T18:07:44.407Z Reads: 115

```
Would something like this be robust?

https://flipsky.net/products/antispark-switch-smart-280a?variant=9328420552764&gclid=CjwKCAjwycfkBRAFEiwAnLX5IS_bQx5THVa5_i0SlPVLJLZK2V5r9XnUh6rU7eKs8uQuSDdsxq_B0RoCBC4QAvD_BwE

I guess I don't mind spending some coin if it works ok
```

---
## \#8 Posted by: Sn4pz Posted at: 2019-03-20T18:08:25.806Z Reads: 112

```
this is flimsy as paper, stay away
```

---
## \#9 Posted by: GarrettL Posted at: 2019-03-20T18:27:35.077Z Reads: 108

```
I've got the regular version(not smart) and its been working nicely for several weeks now.
```

---
## \#10 Posted by: Bart_Dood Posted at: 2019-03-20T18:28:15.593Z Reads: 108

```
You have this one?

https://flipsky.net/products/antispark-switch-pro-280a
```

---
## \#11 Posted by: GarrettL Posted at: 2019-03-20T18:29:25.948Z Reads: 104

```
That's the one
```

---
## \#12 Posted by: chrischo1996 Posted at: 2019-03-20T18:45:30.862Z Reads: 97

```
I have the pro as well, no issues so far after hundreds of miles and about 6 months of use at both 10s and 12s.
```

---
## \#13 Posted by: Bart_Dood Posted at: 2019-03-22T17:56:19.634Z Reads: 79

```
I ordered the $39 pro switch, I guess I'll find out if they really improved this thing...
```

---
## \#14 Posted by: DerelictRobot Posted at: 2019-03-22T19:06:55.180Z Reads: 77

```
Antisparks without precharge die a little bit every time you use them. It's just a matter of _when_ they will fail and _how_. I've had them just fail by getting stuck on permanently, and also a bit more spectacularly:

![IMG_20181101_153122|666x500](upload://nnn6HrMXxOwvKXbdfmwSF7He8Sa.jpeg) ![IMG_20181101_153202|375x500](upload://fQRhUN8loW6jMAuFwtNAErApFvx.jpeg)
"Pro" Switch
```

---
## \#15 Posted by: b264 Posted at: 2019-03-22T19:18:38.276Z Reads: 75

```
The way to fix it is to redesign the switch itself, as reviewed here

https://www.electric-skateboard.builders/t/vedder-antispark-design-problem-or-implementation-problem/77967/4?u=b264

But for now, the best way as @psychotiller said is just to use a loopkey.

[quote="psychotiller, post:6, topic:87758, full:true"]
unity, and 100a maytech Vescs have built in switches. Pretty much the only way to go if you don’t want to Loop key
[/quote]

The problem with builtin switches is that the large filter capacitors have a leakage current which is now "always on" so it could drain your battery while turned off if you left it unused for a while.  It's better to put the big filter capacitors after the switch -- which means separate the switch and ESC -- which means for now, loopkey is still the best option if "reliability" and "safety" are two of the factors you're optimizing for.
```

---
