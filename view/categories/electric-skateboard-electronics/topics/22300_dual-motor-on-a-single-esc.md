# Dual motor on a single ESC

### Replies: 6 Views: 1096

## \#1 Posted by: bartroosen12 Posted at: 2017-05-03T13:23:04.777Z Reads: 133

```
Hi all,
I was asking should it be possible to connect to motors to one ESC.
ESC: 120A 12S ESC (diy-electric-skateboard-kits-parts/torqueboards-12s-120a-car-esc-opto-hv/)
Motor: SK3 - 149Kv 12S
Battery: 12S 150A max
<img src="/uploads/db1493/original/3X/9/e/9e0df88eb785d1c257670afa850dbbdc2b45fa3c.jpeg" width="666" height="500">
Does anyone ever tested this?
```

---
## \#2 Posted by: rwxr Posted at: 2017-05-03T13:24:12.379Z Reads: 129

```
It has been done, but that was with a VESC. 

https://www.electric-skateboard.builders/t/dual-bldc-single-vesc-works/15193/8
```

---
## \#3 Posted by: JTAG Posted at: 2017-05-03T14:06:53.915Z Reads: 120

```
Yes it is possible if and only if the axis are coupled AND the rotor flux is aligned (the generated voltage on the should be equal). See the pictures in the topic.

:grin:
```

---
## \#4 Posted by: NilsS Posted at: 2017-05-03T17:37:36.493Z Reads: 93

```
Dude i would not do that.
```

---
## \#5 Posted by: longhairedboy Posted at: 2017-05-03T17:41:46.999Z Reads: 92

```
ehhhh... i'll get the popcorn.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-03T18:23:25.712Z Reads: 87

```
Possible on the test bench but it doesn't seem practical for E-board application. 
Wouldn't this reduce motor performance or over work the Vesc?
```

---
