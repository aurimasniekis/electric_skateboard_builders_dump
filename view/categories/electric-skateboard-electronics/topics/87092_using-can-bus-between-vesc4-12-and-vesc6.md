# Using CAN bus between vesc4.12 and vesc6

### Replies: 7 Views: 136

## \#1 Posted by: xilw3r Posted at: 2019-03-13T21:27:20.356Z Reads: 60

```
hey guys,

the title says it all really- is it safe to connect 4.12 vesc and a vesc 6 (flipsky variant to be exact) by can bus? I tried searching for this, maybe i just missed it, sorry if so.

big thanks
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-03-13T21:29:27.058Z Reads: 59

```
I doubt it, not to mention if you ran them together you'd likely have thermal throttling on the 4.xx, while the 6.xx would just be chilling

Also, I don't think  4.xx HW can run the FW meant for  6.xx HW
```

---
## \#3 Posted by: trampa Posted at: 2019-03-13T21:58:14.890Z Reads: 50

```
You CAN do that as long as you power up both units simultaneously via same battery connection.
Just make sure both ESCs run the latest or same FW. It doesn't matter if you hook up different devices via CAN. HW 4.xx can be controlled via a master HW 6.xx and VS.
```

---
## \#4 Posted by: spei Posted at: 2019-03-13T21:59:35.687Z Reads: 49

```
If Im not mistaken, I've head somewhere that it is possible, as long as all the settings from both motors for both different VESC's are the same (ermp and such)
```

---
## \#5 Posted by: trampa Posted at: 2019-03-13T22:00:57.621Z Reads: 49

```
The lowest rated device sets the limits....
```

---
## \#6 Posted by: spei Posted at: 2019-03-13T22:01:41.795Z Reads: 49

```
[quote="trampa, post:5, topic:87092, full:true"]
The lowest rated device sets the limits…
[/quote]

Exactly this thing!
```

---
## \#7 Posted by: trampa Posted at: 2019-03-13T22:03:55.647Z Reads: 50

```
You can run two different motors on two different HW versions and set different current ratings for each device. The design is very versatile....
```

---
