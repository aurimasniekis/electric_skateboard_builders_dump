# Do I *need* a loop switch?

### Replies: 17 Views: 1237

## \#1 Posted by: brandon Posted at: 2016-10-24T02:33:42.782Z Reads: 190

```
If my ESC has a built in switch, do I really *need* a loop switch or some other high current switch in line with my batteries? Is anti spark really important?

Also, do I need to unplug my batteries from my esc to charge, or is turning the ESC off with the built in switch enough to allow charging?
```

---
## \#2 Posted by: chinzw Posted at: 2016-10-24T02:48:38.141Z Reads: 187

```
You need some sort of anti-spark, the caps on the ESC get charged even when its off, and this is what causes the spark. If you dont use an anti-spark you will ruin your connectors and maybe fry something else in the process. If you dont want to spend money you can use XT90S connector, or if thats still expensive (5$) you can buy a resistor and a momentary switch and make your own antispark for about 1-2$

edit: you can charge your batteries while connected to the ESC, just make sure its off.
```

---
## \#3 Posted by: treenutter Posted at: 2016-10-24T02:56:10.765Z Reads: 174

```
@brandon no, you don't absolutely need one. The main risk is to your connectors, which are very inexpensive to replace.
```

---
## \#4 Posted by: chinzw Posted at: 2016-10-24T03:01:12.691Z Reads: 171

```
Well, a pack of 5 x XT90 connectors is 6$ and 2 XT90S are 6$, if you do the math, just buy the XT90S
```

---
## \#5 Posted by: saul Posted at: 2016-10-24T03:39:28.368Z Reads: 156

```
by built in switch i guess you have a car/flier esc, so theres no risk of spark when connecting power like on a vesc(always on).

**but I would still have a loop switch close to the battery as a _failsafe_**. in case the esc fails to on, or something, always good to have a way to quickly disconnect power!
```

---
## \#6 Posted by: chinzw Posted at: 2016-10-24T03:46:47.507Z Reads: 153

```
[quote="saul, post:5, topic:11779, full:true"]
by built in switch i guess you have a car/flier esc, so theres no risk of spark when connecting power like on a vesc(always on).

**but I would still have a loop switch close to the battery as a _failsafe_**. in case the esc fails to on, or something, always good to have a way to quickly disconnect power!
[/quote]

Most ESC have caps, which is what causes the spark, its not a VESC only thing.

<img src="/uploads/db1493/original/3X/f/2/f280fe9b0e265e0a6651de43eacf8371c1dc1836.jpg" width="375" height="500">
```

---
## \#7 Posted by: saul Posted at: 2016-10-24T03:50:44.365Z Reads: 147

```
all esc have caps :wink:
but yes you're right, the high inrush current to "fill" the caps with charge is what causes the spark, but if the switch if off, this won't happen right?

vesc on the other hand do not have a built in power switch(and usually higher voltage), so aniti-spark is more important.
```

---
## \#8 Posted by: chinzw Posted at: 2016-10-24T05:32:31.088Z Reads: 140

```
The caps are before the switch, so you will get the same effect as with the VESC
```

---
## \#9 Posted by: Alfred Posted at: 2016-10-24T11:46:26.335Z Reads: 117

```
hello from Vienna . 
I have a question regarding charging without separating the vesc.
Can damage the Vesc if it is not separated during charging.
(11 S 36V / 10Ah A LIFEPO battery from HEADWAY charger 36 V 5 Ah).
I would like to have only one external jack and no other switch can be forgotten.
THX Alfred
```

---
## \#10 Posted by: mattdig Posted at: 2016-10-24T12:50:33.781Z Reads: 104

```
I'm just using a regular metal switch from the hardware store wired between the battery and the ESC. 
http://www.dhresource.com/260x260s/f2-albu-g1-M01-DD-57-rBVaGFaAW42AUzseAAFPqecMaE8339.jpg/heavy-duty-toggle-flick-switch-12v-on-off.jpg
```

---
## \#11 Posted by: Maxid Posted at: 2016-10-24T13:01:10.508Z Reads: 100

```
:scream: What current is that switch rated for?
```

---
## \#12 Posted by: mattdig Posted at: 2016-10-24T13:03:06.286Z Reads: 98

```
Like 20A (at 220V). It's fine. Safety 3rd. Honestly I've been using it for 2 years, and I've measured peak  amps in the 90s through it, no problem.
```

---
## \#13 Posted by: brandon Posted at: 2016-10-24T13:14:20.022Z Reads: 95

```
So loop switches are ugly as hell, I'd prefer something a little more black and non-obstrusive. Any suggestions?

Sounds like my solution will be to leave the ESCs built in switch on all the time and switch power directly from the batteries.
```

---
## \#14 Posted by: TarzanHBK Posted at: 2016-10-24T14:20:31.047Z Reads: 87

```
if you like it more black paint it! :monkey:

if you want a more elegant way, go for a antispark switch, where you can choose what switch stile you like
```

---
## \#15 Posted by: chinzw Posted at: 2016-10-24T16:41:44.145Z Reads: 80

```
As i said before, you can charge your batteries while connected to the ESC, just make sure its off. You dont need the loop key to be visible, just use the XT90S as a normal connector so that when you connect your batteries you dont get sparks. 
And please dont use one of those 20A mechanical switches! @mattdig safety is always first, if you dont care for your safety thats ok, but dont promote unsafe practices to other people (specially newbies)
```

---
## \#16 Posted by: mattdig Posted at: 2016-10-24T17:09:01.082Z Reads: 76

```
You're right, and I'm sorry.
```

---
## \#17 Posted by: Okami Posted at: 2016-10-24T18:54:37.919Z Reads: 69

```
I also use mechanical switch. I had the option to solder 1 wire to 2 terminals at once,  it was 4 pole, single throw switch. At 115V it says 20A. So far it has holded up great. My only concern is that it might have increased resistance compared to connectors or a smart switch. Should, probably, check one day is it significant or not.
```

---
