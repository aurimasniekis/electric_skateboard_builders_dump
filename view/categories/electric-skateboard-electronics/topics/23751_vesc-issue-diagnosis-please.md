# VESC issue? Diagnosis please

### Replies: 9 Views: 461

## \#1 Posted by: dedinski Posted at: 2017-05-23T14:49:50.148Z Reads: 52

```
So after normally riding my board for 2 months now I experienced a failure. The board suddenly stopped.

After inspection I found one of the vesc motor wires disconnected. I connected it back, but now i get this red led signal pattern- 2 series of 3 blinks when the remote is pressed (brake or throttle).

Whats the diagnosis docs?
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-23T15:03:37.012Z Reads: 48

```
Plug it in to you computer, get the red blinks, then go to terminal in BLDC tool and type "faults". It should tell you what's wrong. Hopefully it's not a DRV8302 error.
```

---
## \#3 Posted by: dedinski Posted at: 2017-05-23T15:11:29.934Z Reads: 46

```
It is :( damn... is it junk now or?
```

---
## \#4 Posted by: Jinra Posted at: 2017-05-23T15:12:36.354Z Reads: 44

```
What VESC is it? I hear VESC-x can survive a DRV8302. If it's not, then you'll need to replace the chip or the VESC overall.
```

---
## \#5 Posted by: dedinski Posted at: 2017-05-23T15:14:50.561Z Reads: 43

```
It was an enertion standard VESC.. I will contact them to see if something can be done :confused:
```

---
## \#6 Posted by: Jinra Posted at: 2017-05-23T15:15:48.085Z Reads: 41

```
Yea, that sucks. You can send the VESC to @JohnnyMeduse for repair as well.

BTW what motor connectors did you use?
```

---
## \#7 Posted by: dedinski Posted at: 2017-05-23T15:17:38.773Z Reads: 41

```
4mm bullet connectors. Could a bad soldering job to this?
```

---
## \#8 Posted by: Jinra Posted at: 2017-05-23T15:18:58.986Z Reads: 41

```
You mean break the DRV? Probably not, it seems that the disconnected motor wire might have caused it.
```

---
## \#9 Posted by: dedinski Posted at: 2017-05-30T21:22:52.197Z Reads: 16

```
I didnt get a warranty from enertion for my vesc. Any idea where I can get it fixed in eu and approximately the price range Im looking at? Thx
```

---
