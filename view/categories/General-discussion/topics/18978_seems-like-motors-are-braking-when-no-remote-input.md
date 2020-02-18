# Seems like motors are braking when no remote input

### Replies: 8 Views: 930

## \#1 Posted by: headrec Posted at: 2017-03-13T01:54:06.645Z Reads: 80

```
First time using board since fall.  Raptor 1 board and I think I switched to the nano x controller during that time.  Basically I use to be able to push the board with little resistance to get the board going before adding acceleration so I don't have it take off from a stop.  Now it feels like the board has a little bit of the brakes on when I try to push it. I turn the board off and it's like it use to be. 

Wondering if I need to tweak the settings in the VESC and/or if anyone has the same experience and what to look into?
```

---
## \#2 Posted by: makevoid Posted at: 2017-03-13T02:52:43.905Z Reads: 76

```
If you changed transmitter/receiver you need to set its limits, check out http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244
```

---
## \#3 Posted by: headrec Posted at: 2017-03-13T02:58:37.329Z Reads: 75

```
Thank you! I'll check that out tomorrow when I have some more time.
```

---
## \#4 Posted by: headrec Posted at: 2017-03-14T03:49:24.499Z Reads: 47

```
Ok I tried diciking with it tonight and it still the same. bdc is new to me. 

Like I said it's braking hard on a roll. what do i need to do to stop it?
```

---
## \#5 Posted by: Blasto Posted at: 2017-03-14T04:23:41.295Z Reads: 46

```
Like @makevoid is suggesting, sounds like your ppm signal is not centered properly OR its the rolling resistance from the belts.
```

---
## \#6 Posted by: Eboosted Posted at: 2017-03-14T04:42:46.914Z Reads: 43

```
If you have this remote:

<img src="/uploads/db1493/original/3X/f/0/f053356edf204c358a669b1745cb36bbb72d43f6.jpg" width="690" height="388">

Dial the trim with the right side white wheel
```

---
## \#7 Posted by: headrec Posted at: 2017-03-14T11:50:12.853Z Reads: 36

```
It's a nano x remote so no trim selection.

It's definitely more than normal resistance from the belts.

I was having issues getting the vesc to connect to bdc.  I'll try again tonight.
```

---
## \#8 Posted by: headrec Posted at: 2017-03-15T02:15:03.479Z Reads: 21

```
K got it figured out tonight.  Most of the problem was the usb cord I was using wasn't producing a readable COM port.  Just like trouble shooting drone parts.  Helps to have extras of just about everything ha.
```

---
