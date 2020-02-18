# PCB Max Current

### Replies: 11 Views: 166

## \#1 Posted by: AlanZhou Posted at: 2019-07-30T15:52:52.581Z Reads: 49

```
Couldn't find info on this but, what's the max current a PCB can handle with 1 OZ copper?

![IMG_20190730_115229|666x500](upload://lkuk0P9XBFHGE2kb6DHTOmxzwZ3.jpeg)
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-07-30T16:06:56.573Z Reads: 47

```
@thisguyhere
```

---
## \#3 Posted by: Hummie Posted at: 2019-07-30T16:29:41.979Z Reads: 44

```
not much at all and use multistrand over top for any current that will flow in series.
```

---
## \#4 Posted by: AgressivStreetLamp Posted at: 2019-07-30T17:14:54.020Z Reads: 33

```
This is the same question as "How much water will go through this pipe?"

It really depends on a lot of factors. Width, height, material used, voltage (sorta), ambient temperature, Duration of current application etc.

Use this to get an understanding of the factors and ballpark numbers:
https://www.4pcb.com/trace-width-calculator.html

tl;dr
at 10mm trace width, for 0.05 mm depth: (average ballpark #s based on picture)
10 Amps will get warm over minutes. 100 will melt things in seconds. PCB traces are not meant for large currents.
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-07-30T17:26:26.767Z Reads: 32

```
[quote="AgressivStreetLamp, post:4, topic:99405"]
100 will melt things in seconds. PCB traces are not meant for large currents.
[/quote]

^if thats the case ill just avoid PCB's

was meant for a 10p pack.

All i know about the PCB's are that their 1oz copper and trace is ~15.5 by 88
```

---
## \#6 Posted by: rojitor Posted at: 2019-07-30T17:35:22.637Z Reads: 31

```
I use copper braids on them so it doesn't matter the ampacity of the pcb. I get what I want.
```

---
## \#7 Posted by: AgressivStreetLamp Posted at: 2019-07-30T17:35:23.038Z Reads: 30

```
![image|319x328](upload://eiLB8eUVlpvhA4KxOTZnE0uqSuH.png) ![image|317x327](upload://zJVuevyM6rDoyDviIVKfRBHdBLw.png) 

Half a meter wide and it'll handle 100 Amps. (Continuous, in fairness,)
3" will handle 20 amps

If you add a multi strand wire (looks like solder wick) on top you will be fine.
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-07-30T17:40:28.705Z Reads: 28

```
adding copper braids on top would be hard to do in my case.
```

---
## \#9 Posted by: AgressivStreetLamp Posted at: 2019-07-30T17:42:06.744Z Reads: 31

```
How about nickel strips?
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-07-30T17:43:02.117Z Reads: 28

```
Yea that should work.
```

---
## \#11 Posted by: thisguyhere Posted at: 2019-07-30T19:14:45.568Z Reads: 27

```
it's been addressed but to add, i wouldn't use the copper layer on the pcb by itself.

first, when you spot weld nickel to the copper layer, it takes very little force to pry it off.  you can pull on it lightly and it comes off.

second, not enough ampacity on that thin layer.

so the pcb just acts like a solid backing for the cells and battery making materials to mount up to.

i solder nickel onto the copper layer and use copper strand for series connections.

![image|690x381](upload://kluzVKyE049vHOvenoAY72AnujK.jpeg)
```

---
