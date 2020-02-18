# 18650 battery pack question

### Replies: 12 Views: 663

## \#1 Posted by: Ishayc Posted at: 2017-09-27T05:34:47.211Z Reads: 109

```
Hi,

I can get a good deal on Samsung ICR18650-26J 2600mAh batteries.
I'm planning on building a 10s6p pack.
My question is - will a 31.2 discharge current be enough for dual Tacon 160 motors?

Ishay
```

---
## \#2 Posted by: darkkevind Posted at: 2017-09-27T06:28:48.636Z Reads: 102

```
What do you class as a 'good deal' for 60 of those cells?
```

---
## \#3 Posted by: jrpwit Posted at: 2017-09-27T06:28:52.275Z Reads: 102

```
Yes it would work but battery would sag. Maybe up the voltage to 12s?

Also tacon is great for the money however because of its higher kv of 245 this will want to draw more current 
further contributing to a sagging battery.

I would recommend saving for other cells like the 30q or 25r. 

One think I have learned is to not short cut and just get the right stuff if I want good performance.
```

---
## \#4 Posted by: Ishayc Posted at: 2017-09-27T06:43:11.466Z Reads: 90

```

@jrpwit Yup, The tacons are awesome. I'm now running them with 6s lipos.
If I limit each vesc to 15 amps will the sag be that bad?
@darkkevind not sure yet but very cheap :)
```

---
## \#5 Posted by: jmasta Posted at: 2017-09-27T07:08:00.282Z Reads: 87

```
It will work as long as you keep it under 5A/cell (30A total).  Pulling 30A on a 10s6p pack made from 26J cells, will have 3.5V sag or more, but that's not too bad for li-ion packs.  With 6 in parallel (6p @ 5A/cell), it would have less sag than a Samsung 25R with 3 in parallel (3p @ 10A/cell)

You could even do 7A/cell (42A total), but the cells will start getting pretty hot, which is bad for battery life.   Should be fine for bursts though


_**Samsung 26J:**_
http://lygte-info.dk/pic/Batteries2012/Samsung%20ICR18650-26J%202600mAh%20(Pink)/Samsung%20ICR18650-26J%202600mAh%20(Pink)-Capacity.png


_**Samsung 25R:**_
http://lygte-info.dk/pic/Batteries2012/Samsung%20INR18650-25R%202500mAh%20(Green)/Samsung%20INR18650-25R%202500mAh%20(Green)-Capacity.png
```

---
## \#6 Posted by: darkkevind Posted at: 2017-09-27T07:31:10.947Z Reads: 72

```
Cheaper than this?

<img src="/uploads/db1493/original/3X/f/4/f447bd6b8d5885799a7eb99472a7cb72da028bbb.jpg" width="281" height="500">
```

---
## \#7 Posted by: Ishayc Posted at: 2017-09-27T07:41:30.583Z Reads: 67

```
Much cheaper
```

---
## \#8 Posted by: darkkevind Posted at: 2017-09-27T07:42:13.355Z Reads: 68

```
Nice! 😁 . . .
```

---
## \#9 Posted by: scepterr Posted at: 2017-09-27T08:11:23.009Z Reads: 67

```
I hope people aren't actually running cells at max cont discharge current...unless they plan on replacing them yearly. 
30Q for instance
<img src="/uploads/db1493/original/3X/c/f/cf17da110b2d8ec6637d929e1d4ffc9b9634a4af.jpg" width="281" height="500">
```

---
## \#10 Posted by: darkkevind Posted at: 2017-09-27T09:30:20.962Z Reads: 54

```
That's why I run LG HG2's 4p...
```

---
## \#11 Posted by: Acido Posted at: 2017-09-27T10:16:31.383Z Reads: 51

```
what is that site?
us or eu?
```

---
## \#12 Posted by: darkkevind Posted at: 2017-09-27T10:20:01.387Z Reads: 53

```
It's my site. It's a filter tool for Nkon.nl where you can price up your pack... Nkon is based in NL so it's in Euro's.

http://kevindark.co.uk/PublicServices/NkonFilter
```

---
