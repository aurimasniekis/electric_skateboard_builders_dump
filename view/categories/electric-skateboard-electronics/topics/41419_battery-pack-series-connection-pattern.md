# Battery pack series connection pattern

### Replies: 9 Views: 660

## \#1 Posted by: thisguyhere Posted at: 2017-12-19T07:35:39.232Z Reads: 129

```
what would be a better design when wiring up a battery pack?

A: this serpentine pattern?

<img src="/uploads/db1493/original/3X/8/7/87bf699dcef2c55767220c5b69e515afa552ed04.png" width="690" height="256">

B: this more linear pattern?

<img src="/uploads/db1493/original/3X/9/e/9e694a19c7da45663634e364507b504c5cbdd2dd.png" width="689" height="234">

i remember seeing somewhere, don't ask me for a source, that additional heat builds up where the u-turn happens in the second diagram.

i've been building all my packs in pattern B this whole time, considering A on the next one.
```

---
## \#2 Posted by: Genghis_Kuan Posted at: 2017-12-19T07:41:33.210Z Reads: 121

```
IMO they are the same, if you think about it on the first diagram if you rotate the first and last two columns of cells straight so you have two columns vertically it would look the same as the second diagram. 

I think it just depends on where you want your positive and negative leads, second diagram you can use less cable.
```

---
## \#3 Posted by: scepterr Posted at: 2017-12-19T07:46:16.278Z Reads: 118

```
I always go B but with main leads on the outside
Also for the U section I use 2-3 pieces of copper braid
<img src="/uploads/db1493/original/3X/2/d/2d97987ae36e8f3c9315d1ad89d095236be013ef.jpg" width="375" height="500">
```

---
## \#4 Posted by: willpark16 Posted at: 2017-12-19T08:35:23.145Z Reads: 96

```
B with the mains on the outside is best
```

---
## \#5 Posted by: TarzanHBK Posted at: 2017-12-19T10:42:05.152Z Reads: 86

```
A - i do it this way. Negativ is that your phase wires are on both side.
B - your chance of shorting the cells is much higher. Happened a few times here, where people don´t insulate enough between the two rows and mess up something.
```

---
## \#6 Posted by: deucesdown Posted at: 2017-12-19T17:16:50.584Z Reads: 73

```
Hm almost all the current is carried on serial connections. If you have a single series connection between p groups, the cells (and nickel) further from the series connections will have more resistance. This is what I believe people call uneven current sharing.

With A, you have a chance to distribute the resistance more evenly. Your diagram already has done this, as you have the series connection in the middle, not at the end, of the p group.

but, you have a chance to do even better with A, at least on the inside series connections, doing like 5 vertical lines between each p group. The outside series can be improved but not so easily.

I'm being fairly pedantic here especially for a 5p pack...

Very curious why the u-turn in B heats up.
```

---
## \#7 Posted by: ducktaperules Posted at: 2017-12-19T17:21:45.609Z Reads: 66

```
i dont think the u turn in B would heat up any more than A. The current through the connections between each parallel group should be the same in both cases.
```

---
## \#8 Posted by: scepterr Posted at: 2017-12-19T17:22:12.363Z Reads: 69

```
Only if you don't have enough current capacity there 
I always put extra material at the furthest points from the output
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-12-19T17:26:54.946Z Reads: 69

```
the single series connection in the diagram is just an illustration, I'd probably use two grounding straps in reality. 

[quote="deucesdown, post:6, topic:41419"]
Very curious why the u-turn in B heats up
[/quote]

I wish I could find the video, it was a thermal camera pointed at a pack on a high current discharge test, like 10a or sumpn, and there was a temperature difference for sure.
```

---
