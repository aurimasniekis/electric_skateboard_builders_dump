# Dual motor setup with one 6355 and one 6374?

### Replies: 9 Views: 723

## \#1 Posted by: cwazy1 Posted at: 2017-08-28T21:05:09.614Z Reads: 131

```
Has anyone done this? I started with a 6355 single build, planning on making it a dual, but I regret going with the 6355 to start since I have 218mm hangers. Would I be able to run one 6355 and one 6374? Then ultimately switch over to two 6374's?
```

---
## \#2 Posted by: psychotiller Posted at: 2017-08-28T21:13:53.989Z Reads: 126

```
Yup! No problem. Ask @lowguido as this is his forte.
```

---
## \#3 Posted by: lowGuido Posted at: 2017-08-29T00:09:12.695Z Reads: 112

```
yeah it works fine, probably the only thing I would say is that if you use DRV cookers dont use canbus, instead split the PWM wires.
```

---
## \#4 Posted by: Deckoz Posted at: 2017-08-29T01:34:34.986Z Reads: 90

```
Can you elaborate? Why no canbus?
```

---
## \#5 Posted by: cwazy1 Posted at: 2017-08-29T02:08:28.938Z Reads: 84

```
What do you mean by drv cookers? 6374 motors?
```

---
## \#6 Posted by: lowGuido Posted at: 2017-08-29T02:11:32.422Z Reads: 82

```
well if you are using 2 different motors that will have different RPMs for any given throttle position I would think it best to keep the electronic parts as seperate as possible.
while it *may work with canbus you would defininently want to disable any traction control feature. 

DRV cookers = VESC
```

---
## \#7 Posted by: cwazy1 Posted at: 2017-08-29T02:19:13.315Z Reads: 80

```
Ohhh. Okay. I'll go with dual 6355s then.
```

---
## \#8 Posted by: lowGuido Posted at: 2017-08-29T02:32:44.875Z Reads: 76

```
why? go 6374
```

---
## \#9 Posted by: PatRocks Posted at: 2017-08-29T02:43:23.021Z Reads: 72

```
That's what I am running!<img src="/uploads/db1493/original/3X/c/a/ca60583a50c60b138b5ca14be09b9a6dde67d789.jpg" width="666" height="500">
```

---
