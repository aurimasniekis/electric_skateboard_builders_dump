# FOCBOX troubleshooting

### Replies: 14 Views: 336

## \#1 Posted by: dimbo Posted at: 2019-01-04T11:52:56.520Z Reads: 110

```
Hi all,

I've been lurking for a while just reading but I think this process is going to go a lot faster if I just ask for a little help :slight_smile:  

I have broken FOCBOX v.1.6 here and would like to try and save it myself. I have basic electronics tools (bench suppy, solder station, heat gun etc.)

I have had a look at the circuit with a cheap microscope and can't see any visible scorching or anything like that. 

I have noticed that both sides of  the diode d101 are connected to GND which doesn't sound ideal to me.

Anyone have ideas on where to go from here ?

Photos attached.

Thanks,

D.

![IMG_20190103_163421|375x500](upload://lbyy9Za7xeoQZyfcjLgPHu38aly.jpeg) ![IMG_20190103_163343|375x500](upload://u2PfX06mdUh8yvhEMVCwKxUTQOO.jpeg) ![IMG_20190103_163505|666x500](upload://rLlChjEThxYJiIYwZDNtdfD8CXm.jpeg) ![IMG_20190103_163331|375x500](upload://nPSbMbOSlYMj3fdIygBg9SHgwX9.jpeg) ![IMG_20190103_163449|666x500](upload://6k77C8uIauLink1yUVnJfpWukIC.jpeg) ![IMG_20190103_163351|375x500](upload://gju4WtzSq8w7kVnhk1e2db1Hlfc.jpeg) ![IMG_20190103_163456|666x500](upload://wn51cb4OsECujJXec2SErYsRpip.jpeg)
```

---
## \#2 Posted by: b264 Posted at: 2019-01-04T11:54:58.713Z Reads: 92

```
[quote="dimbo, post:1, topic:79868"]
I have broken FOCBOX
[/quote]

What are the symptoms? Does it power-on?  Is there a fault code in the terminal?
```

---
## \#3 Posted by: b264 Posted at: 2019-01-04T11:56:42.174Z Reads: 93

```
[quote="dimbo, post:1, topic:79868"]
I have noticed that both sides of the diode d101 are connected to GND which doesn’t sound ideal to me.
[/quote]

If you're certain of this, I would remove the diode and test it out-of-circuit, and then test the pads to see if they both connect to ground.  Photograph which way it was oriented before removing it.

But first complete all troubleshooting that does not require disassembly.
```

---
## \#4 Posted by: dimbo Posted at: 2019-01-04T14:06:23.456Z Reads: 82

```
Hi,

Thanks for replying so quickly. It doesn't power up and no LEDs are on. The focbox was given to me by someone because it doesn't work. I am just formatting a computer to make sure that it won't connect using windows either (I use linux).

I have attached a couple of photos of the diode being tested just in case I'm doing in wrong.

Thanks,

D.

![IMG_20190104_145956|666x500](upload://clvbs14wRrAznpQh0iaJZ167egO.jpeg) ![IMG_20190104_145944|666x500](upload://u7UDuE3bn7Ex2dTGApsGqCCUF0O.jpeg)
```

---
## \#5 Posted by: b264 Posted at: 2019-01-04T14:10:40.606Z Reads: 72

```
I would make a strong guess that someone connected power + and - backwards
```

---
## \#6 Posted by: dimbo Posted at: 2019-01-04T20:08:13.359Z Reads: 65

```
So, I got the diode off. It didn't want to leave the board; it was very effective at sinking the heat away from the solder.

The results:

The diode is good I think: reverse biased 0L and 0.6v when forward biased on diode mode and 16 M ohm when forward biased on resistance mode.

The interesting part was that both of the pads are shorted to ground.....but where to go from here?

As an aside, what would be the recommended method for removal? Mine wasn't optimal by any means...preheat the entire board a bit first? hot air? 
I used the iron with a fat tip but even the solder wick wanted to stay on the board! 

Thanks again for the help :slight_smile:
```

---
## \#7 Posted by: briman05 Posted at: 2019-01-04T20:12:19.886Z Reads: 62

```
There is always @JohnnyMeduse who is a focbox wizard that you could send it to for repair.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2019-01-04T20:17:56.552Z Reads: 61

```
two  Mosfet are probably BLOWN and I'm guessing Q3 and Q4...
```

---
## \#9 Posted by: dimbo Posted at: 2019-01-04T21:10:03.847Z Reads: 58

```
Thanks Johnny...I was secretly hoping that you might chime in here  having seen your previous posts :slight_smile: 
I'll get those mosfets off and see if that's the problem. What technique do you use to get them off without blasting everything in the area with a heat wave?
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2019-01-04T21:18:39.304Z Reads: 59

```
Hot air is basically the best way.
```

---
## \#11 Posted by: b264 Posted at: 2019-01-04T21:27:21.858Z Reads: 56

```
Measure the resistance between each phase wire and batt+ and each phase wire and batt-

Which ones are on?  They should not be on
```

---
## \#12 Posted by: dimbo Posted at: 2019-01-05T21:34:20.198Z Reads: 42

```
I have Q1, Q3,Q4,D101 and R1 off the board currently. Q1 and Q2 have source to drain resistance of 0 ohms (and I destroyed Q3 with too much heat). I assume that those mosfets have died. Is that a correct assumption?
```

---
## \#13 Posted by: dimbo Posted at: 2019-01-05T21:43:08.825Z Reads: 44

```
I'm not sure that the this test will work properly with so many components off the board, but here are the results:

Starting from beside the can bus: 

Bat - to phases .......all have infinite resistance.

Bat + to 2.6 ohm for phase1, 
41.1 kOhm for phase 2
0 Ohm for phase 3
```

---
## \#14 Posted by: b264 Posted at: 2019-01-06T04:34:57.043Z Reads: 30

```
Sounds like two of the FETs are blown

https://www.electric-skateboard.builders/t/focbox-troubleshooting/79868/8?u=b264
```

---
