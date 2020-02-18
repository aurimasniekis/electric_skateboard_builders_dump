# Nano X signal issues or faulty VESC x

### Replies: 12 Views: 888

## \#1 Posted by: trigger4point7 Posted at: 2017-03-10T07:13:36.094Z Reads: 102

```
I'm back again with another issue. I have only been riding my board for a couple weeks when I started having connectivity issues. The transmitter/reciever seem to pair/connect correctly but the signal is getting lost somewhere between the reciever and VESC. I'm trying to determine which one is at fault? I've found that when I pressed down on the cables on the VESC and shifted them around a bit the signal light would flash and sometimes it would even cause the motor to move. Any suggestions?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-03-10T12:18:00.232Z Reads: 88

```
Sounds like a faulty cable. 
Try a new cable. 
Spend a little extra for quality cable with heavy duty connectors and heavy gauge wires.
```

---
## \#3 Posted by: trigger4point7 Posted at: 2017-03-11T16:33:08.646Z Reads: 69

```
Any suggestions? The nano x didn't come with any (out they forgot) so I threw mine together from some Arduino development cables I had.
```

---
## \#4 Posted by: trigger4point7 Posted at: 2017-03-11T20:47:02.950Z Reads: 63

```
I've also tried a new cable, homemade again, but same/similar issue.
```

---
## \#5 Posted by: Blasto Posted at: 2017-03-11T21:04:55.545Z Reads: 56

```
Take a look at what is going on in the bldc tool, tick the ppm display
```

---
## \#6 Posted by: trigger4point7 Posted at: 2017-03-13T00:00:12.806Z Reads: 55

```
@Blasto how do I go about that? Tick the PPM, I found the page, just not sure what to do once I get there. What will it tell me?
```

---
## \#7 Posted by: Blasto Posted at: 2017-03-13T01:14:09.621Z Reads: 55

```
Well it lets you visualize the ppm signal... is it jumping around or nice and stable
```

---
## \#8 Posted by: trigger4point7 Posted at: 2017-03-13T01:20:46.167Z Reads: 49

```
I'm under App Configuration and the PPM tab, I don't see any charts.
```

---
## \#9 Posted by: trigger4point7 Posted at: 2017-03-13T01:30:06.384Z Reads: 49

```
The motor its self those is very stable when I send it commands to turn to a certain RPM, breaking, all response on the second.
```

---
## \#10 Posted by: Blasto Posted at: 2017-03-13T01:43:45.818Z Reads: 47

```
[quote="trigger4point7, post:8, topic:18860, full:true"]
I'm under App Configuration and the PPM tab, I don't see any charts.
[/quote]

It's just a little bargraph that displays the ppm signal.

edit: sorry wrong thread
```

---
## \#11 Posted by: trigger4point7 Posted at: 2017-03-21T23:24:42.074Z Reads: 39

```
Do you know of any tests I could run to determine if it is a Nano issue or something up again with my VESC?
```

---
## \#12 Posted by: Luke Posted at: 2017-03-21T23:45:34.004Z Reads: 36

```
<img src="/uploads/db1493/original/3X/3/1/3126d0432dddf9b4e293a206794782545025b7db.png" width="690" height="387">
I think these guys meant this bar on bldc tool. When you connect the vesc to your computer and tick "display" it will show you what percentage of throttle is being read by the vesc. this can at least show you if your connection is stable.
```

---
