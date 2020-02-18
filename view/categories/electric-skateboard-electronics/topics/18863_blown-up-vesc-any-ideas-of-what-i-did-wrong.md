# Blown up vesc, any ideas of what i did wrong?

### Replies: 8 Views: 882

## \#1 Posted by: Marcello Posted at: 2017-03-10T12:20:14.380Z Reads: 133

```
i used my vesc normally for about 1 week and next morning i turn it up and a spark comes out. any ideas of what went wrong?
<img src="/uploads/db1493/original/3X/d/e/de92420ad70d98d08690b6a3614aef4e4f346bf4.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/f/f/ff583b5c62005347ba5aa9de5344db04d6afd2d2.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/9/c/9c8a58a6da619a7c922e0a9fad9a6bb545f9fbfb.jpg" width="281" height="500">
```

---
## \#2 Posted by: Montiey Posted at: 2017-03-10T15:03:13.561Z Reads: 111

```
You've shorted the 5V and GND on the PPM input. If you got a spark, then separating the pins is a start, but it won't work right until you replace the components that were damaged- and the damage surely isn't limited to C33… The regulator is probably toast, and you might've burnt a trace or two. Check the schematics if you can and see what other components are connected to the 5V rails, and look them over, too.
```

---
## \#3 Posted by: rpn314 Posted at: 2017-03-10T19:28:39.421Z Reads: 97

```
Looks like you blew C33.
Yeah, definitely want those pins separated further, at all times. I believe that 5v comes from the buck converter in the DRV chip...
```

---
## \#4 Posted by: Montiey Posted at: 2017-03-11T14:27:14.750Z Reads: 75

```
Uh oh. If the DRV is blown then it's going to be allot harder to fix than just a 4 pin regulator. :o
```

---
## \#5 Posted by: rpn314 Posted at: 2017-03-11T18:14:19.156Z Reads: 61

```
[quote="Montiey, post:4, topic:18863, full:true"]
Uh oh. If the DRV is blown then it's going to be allot harder to fix than just a 4 pin regulator. :o
[/quote]

Yes it is. You'll need a hot air rework station to replace the DRV chip
```

---
## \#6 Posted by: Journ Posted at: 2017-03-11T20:13:41.163Z Reads: 55

```
Any advice on preventative measures to keep this from happening? Or is this question too tangential for this thread and if so i can delete it.
```

---
## \#7 Posted by: flatsp0t Posted at: 2017-03-11T20:24:14.946Z Reads: 51

```
Use an empty plug (no wires crimped in) to cover the pins, so you cant accidentally press them together.
```

---
## \#8 Posted by: Montiey Posted at: 2017-03-12T14:24:47.917Z Reads: 38

```
Same. If I hadn't left them covered by heat shrink previously this year, I would have put a "dummy" plug on my VESC's pins. But now I use a GT2B, and so there's a real connector on the pins now.
```

---
