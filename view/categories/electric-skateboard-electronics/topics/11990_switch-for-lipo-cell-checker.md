# Switch for lipo cell checker

### Replies: 8 Views: 844

## \#1 Posted by: ninja Posted at: 2016-10-27T06:21:19.912Z Reads: 78

```
Hi builders! I put a cell checker (up to 8s) on my board. I have 2x 4s in series lipos, so i want one cell checker per both lipo packs. I connected JST-XH connectors like in diagram, it's working, cell checker reads all 8S. But i want to put a switch for that cell checker. Where i should put a switch in there? Here is diagram:
<img src="/uploads/db1493/original/3X/6/7/672b674314388d33198484118eab537c3eba7df8.png" width="507" height="500">
```

---
## \#2 Posted by: smudgeUK Posted at: 2016-10-27T07:53:23.418Z Reads: 66

```
I was thinking about this recently after reading the cell checkers drain voltage when always plugged in. I personally would just break the 0v
```

---
## \#3 Posted by: chinzw Posted at: 2016-10-27T07:57:01.076Z Reads: 65

```
Yep, cutting the ground would work.
```

---
## \#4 Posted by: smudgeUK Posted at: 2016-10-27T08:02:39.832Z Reads: 64

```
In fact, now I think about it, is it not the only one that will work?!
Any others would just drop one cell from the readout?
```

---
## \#5 Posted by: ninja Posted at: 2016-10-27T16:33:30.700Z Reads: 49

```
Which one is ground wire?
```

---
## \#6 Posted by: mmaner Posted at: 2016-10-27T16:36:26.977Z Reads: 48

```
if you put a 2 pole switch in between the ground, you will be good.  the ground is the black wire on the far left.
```

---
## \#7 Posted by: chinzw Posted at: 2016-10-27T16:47:40.676Z Reads: 42

```
Yeah, that's right. Depending on how the cell checker is wired tough. Since if you cut the GND, then 1st cell becomes ground, which could feed back through the inputs and power the circuit anyways.
```

---
## \#8 Posted by: ninja Posted at: 2016-10-27T21:27:25.148Z Reads: 34

```
Thank you guys, i just did it it's working perfect!
```

---
