# \[Anti-Sparks\] Is This Possible?

### Replies: 18 Views: 804

## \#1 Posted by: Proxy Posted at: 2017-12-08T11:05:10.971Z Reads: 193

```
I'd plan to follow this guy's <a href="https://www.youtube.com/watch?v=lvhfwkFXgRQ">YouTube </a> tutorial on anti-sparks but it seems like i need a lot of adapters. So i thought, is it possible to snip the end part off of a <a href="https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html">XT90 Battery Harness</a> and then solder on a Anti spark plug that plug it straight into the vesc? 

**Here is a diagram of what im talking about:**
   https://imgur.com/lBMtoDb
<img src ="https://imgur.com/lBMtoDb">
```

---
## \#2 Posted by: lasplaner Posted at: 2017-12-08T12:29:05.895Z Reads: 175

```
From what I understand, yes it is completely possible.

Placing the 2 batteries in series will effectively give you a battery with the same amount of amp-hours, but double the voltage (assuming you use the same two batteries).

So soldering this XT-90 Anti-Spark on the series connector is essentially soldering the Anti-Spark onto a single voltage source, as the series connector combines the voltages from both batteries forming a higher voltage pack. However some people prefer to use an anti-spark switch key, which works like this. 

<img src="/uploads/db1493/original/3X/0/7/078416810d75c5dfdb6315e6c461db0aae7db30a.png" width="225" height="250">
[quote="Proxy, post:1, topic:40449"]
Here is a diagram of what im talking about:
   https://imgur.com/lBMtoDb
[/quote]

In the end it is your descision but your design in this diagram should work. That being said, now I need to try it out for myself!

-lasplaner
```

---
## \#3 Posted by: PXSS Posted at: 2017-12-08T12:32:57.311Z Reads: 156

```
Yes. It's possible. 
Just make sure you use the female on the battery. You had them backwards in your picture
```

---
## \#4 Posted by: tung Posted at: 2017-12-08T14:38:03.075Z Reads: 138

```
why does spark even occur? how often does it occur?
im planning to build and didnt know i would need an antispark till i see this
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-12-08T14:55:32.812Z Reads: 125

```
cause we are running “high voltage”. the spark is a rush of correct going to the connectors, which degrades them
```

---
## \#6 Posted by: Namasaki Posted at: 2017-12-08T15:01:47.734Z Reads: 126

```
Forgive me for nitpicking but in your diagram, the battery supplying negative to motor should be battery 1
And the battery supplying positive to motor should be battery 2
```

---
## \#7 Posted by: lasplaner Posted at: 2017-12-09T00:50:00.415Z Reads: 103

```
I think it’s got to do more with the VESC’s high voltage capacitors. They hold small amounts of charge to smooth out the waveform of the DC battery signal, but a sudden inrush of current from the batteries when plugging them in means that they spark. The antisparks introduces a resistor, which lessens the current entering the capacitors.

@Namasaki why is this true? Is it because current flows from one terminal to another? If so, how would current flow in a circuit kept open by a disconnected antispark?
```

---
## \#8 Posted by: Hummie Posted at: 2017-12-09T01:13:48.570Z Reads: 99

```
the drawing looks fine and you can have the plug either way with the green side on the battery side or the esc side no problem.  
I've heard of someone just adding vasaline on connectors instead
```

---
## \#9 Posted by: Namasaki Posted at: 2017-12-09T01:13:48.875Z Reads: 96

```
Because the cell count goes from the negative end to the positive end like this:

<img src="/uploads/db1493/original/3X/4/9/49a094677ff3f3637099adf547b6ec690cbeee12.png" width="664" height="500">
```

---
## \#10 Posted by: Proxy Posted at: 2017-12-09T04:12:33.303Z Reads: 77

```
vasaline? Wot....
```

---
## \#11 Posted by: Hummie Posted at: 2017-12-09T06:01:18.953Z Reads: 73

```
https://en.wikipedia.org/wiki/Paschen's_law

surprised to read this:

"With a constant pressure, the voltage needed to cause an arc reduced as the gap size was reduced but only to a point. As the gap was reduced further, the voltage required to cause an arc began to rise and again exceeded its original value."


 vasline  with higher resistance than the air so if maybe a 50v arc would be at .3mm then if you have connectors that have no metal .3mm apart while youre able to connect them through the insulator then no spark.  the details of what would happen i don't know..or if it would even work and waiting for you to do it.
```

---
## \#12 Posted by: b264 Posted at: 2017-12-09T08:22:05.767Z Reads: 68

```
The spark is from the capacitors on the ESC charging-up.  (The 2 or 3 cans at one end)  Without those, you would never need an anti-spark.  However those are needed for responsiveness.  Technically, you could take them and the anti-spark off but I do NOT recommend it.
```

---
## \#13 Posted by: PXSS Posted at: 2017-12-10T12:13:57.197Z Reads: 58

```
[quote="Hummie, post:8, topic:40449"]
you can have the plug either way with the green side on the battery side or the esc side no problem.
[/quote]

No. You should never put the male plug on a battery. That's just asking for a short to happen.
```

---
## \#14 Posted by: Hummie Posted at: 2017-12-10T19:00:10.247Z Reads: 48

```
looking the plug it looks to me as if ironically the female has more exposed connectors and probably easier to short than the male
https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html
  I like the male on the battery because when these things do eventually fail, and I find i'm getting a spark, my battery leads are longer and easier to solder than the small wires I have off my vescs.
```

---
## \#15 Posted by: PXSS Posted at: 2017-12-10T20:10:28.865Z Reads: 39

```
Just in case...
Which one do you think is the female?
```

---
## \#16 Posted by: Hummie Posted at: 2017-12-10T20:22:48.078Z Reads: 38

```
   For some people maybe "female" can be different things but for me it's always the hole that I stick it into
```

---
## \#17 Posted by: PXSS Posted at: 2017-12-10T20:37:40.905Z Reads: 36

```
The female is the one with the female bullets...
```

---
## \#18 Posted by: Hummie Posted at: 2017-12-10T22:00:39.384Z Reads: 33

```
ok then looking at it from that deciding what sex my plug is I've got it like you and  I stick my green one, femaie, on the battery.  looking at it now the bullets are pretty safely down in there for the battery.
```

---
