# Balance charging 3 - 2S lipo&rsquo;s as one 6S Lipo?

### Replies: 12 Views: 2319

## \#1 Posted by: LAVAMAN Posted at: 2016-12-18T21:38:41.731Z Reads: 143

```
Hello,
I am new to this forum as of yesterday. I am building an E board and will be using 3 - 2S Lipo batteries wired in series to power the board. I have a Traxxas battery charger that will charge up to 6S Lipo. My question is how to build a balance harness so that I can connect to my charger so I can charge as one 6S battery. I want to make charging and balancing as easy as possible. Please see my diagram (attached) and fill in the blanks if you know how.

<img src="/uploads/db1493/original/3X/f/0/f00de968e0675b1c5ab1eb079c7564eb11e9e2c3.jpg" width="388" height="500">
```

---
## \#2 Posted by: Esrapp21 Posted at: 2016-12-18T21:40:20.099Z Reads: 136

```
Are you wondering where to solder to a JST balance connector?
```

---
## \#3 Posted by: LAVAMAN Posted at: 2016-12-18T21:45:29.714Z Reads: 133

```
I think a 6S balance plug has 7 pins? How do I connect all 3 2S lipo's into 1 6S balance plug so my charger thinks it is 1 6S Lipo?
```

---
## \#5 Posted by: Esrapp21 Posted at: 2016-12-18T21:48:44.151Z Reads: 130

```
Here is a diagram I made of what you want to do: 

<img src="/uploads/db1493/original/3X/6/1/61955f17b3b9a1a9744fff3832ddd2aa0af7c509.PNG" width="598" height="500">
```

---
## \#6 Posted by: LAVAMAN Posted at: 2016-12-18T22:01:13.724Z Reads: 117

```
This is what I was looking for! 

So the blue, orange & green wires go to the small center banana plugs and the pink & brown wires come off the series wires. I assume you have done this before? My charger will think I am charging one 6S battery and balance all cells evenly. Thanks for the information. I appreciate it. One step closer.
```

---
## \#7 Posted by: Esrapp21 Posted at: 2016-12-18T23:00:05.369Z Reads: 106

```
Each of the colored wires coming directly from a battery are connected to a single cell from it, and all the series connections combine 2 cells to one, so the basic idea is that for every cell, there is a wire. This allows the balance charger to know how much to charge each cell. Good luck on the board!
```

---
## \#9 Posted by: Namasaki Posted at: 2016-12-18T23:26:48.750Z Reads: 104

```
I'm pretty sure that it is unessesary to patch in the black balance wires from pack 2 and 3.
They are already connected when the main wires are connected in series.
you only need to connect the black ground balance wire from the first pack in the series.
Think of the 3 packs as 1 pack when connected in series.
A 6s pack will only have 1 ground wire and 1 wire from each cell's positive side.
<img src="/uploads/db1493/original/3X/2/1/21667d1252a8a730e7910dc864a2c165f85853dd.png" width="644" height="485">
```

---
## \#10 Posted by: Esrapp21 Posted at: 2016-12-19T01:44:18.558Z Reads: 91

```
My bad, and you're right. Good catch
```

---
## \#11 Posted by: LAVAMAN Posted at: 2016-12-19T16:54:32.727Z Reads: 85

```
Thanks for the correction! I will follow this diagram.
```

---
## \#12 Posted by: lollystimler Posted at: 2018-09-03T13:04:48.352Z Reads: 30

```
I want to do the same but with connecting 4 2s Lipos to make a 8s battery, would this be the correct configuration?![image|375x500](upload://zJv6C3zMOJJRTV7Wb9dW9qlLq3R.jpg)
```

---
## \#13 Posted by: PXSS Posted at: 2018-09-03T13:08:04.015Z Reads: 27

```
That is correct.
```

---
## \#14 Posted by: Namasaki Posted at: 2018-09-03T13:50:51.429Z Reads: 23

```
I can’t be sure unless you number the pins on the balance connector to match the bms you’re using.
```

---
