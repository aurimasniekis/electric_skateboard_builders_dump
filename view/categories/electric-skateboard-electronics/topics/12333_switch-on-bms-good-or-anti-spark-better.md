# Switch on BMS - good or anti-spark better?

### Replies: 11 Views: 1421

## \#1 Posted by: oneafrikan Posted at: 2016-11-02T20:14:30.734Z Reads: 265

```
Howdy, quick question for you guys!

I have a Lipo battery connected to a BMS, and the BMS has a switch attached to it... But (I'm pretty sure) every wiring diagram I've seen so far has the switch attached to the main electrics... It's fine but there's no anti-spark so trying to figure that out.

So, should I keep the switch as is, or pull that out (is that possible?) and put in the anti-spark switch??
```

---
## \#2 Posted by: JuniorPotato93 Posted at: 2016-11-02T20:28:25.605Z Reads: 259

```
Well, an antispark switch is really just a electronic switch like the one already in the BMS, in terms of how they operate I mean. It's going to have a transistor that gets turned on opening the circuit just like any antispark switch does. I think the confusion here is that the "antispark" component of the antispark switch comes from the fact that the current does not arc over a small distance when being connected because here we are always connected, but we have a "valve" on it.

I might be a little off in my interpretation if I am someone feel free to correct me, but i think your okay. Only thing I'd be concerned about is do you know how much current your onboard switch is rated for?
```

---
## \#3 Posted by: chinzw Posted at: 2016-11-02T21:12:50.570Z Reads: 242

```
You are correct! Also BMS and Antispark mosfet switches alike use soft on to prevent peak current flow.
```

---
## \#4 Posted by: SirDiff Posted at: 2016-11-02T22:55:18.430Z Reads: 230

```
So if I have a switch on the bms there's no need for another one?
```

---
## \#5 Posted by: Bender Posted at: 2016-11-02T23:11:43.365Z Reads: 220

```
Correct sir
```

---
## \#6 Posted by: mccloed Posted at: 2016-11-02T23:21:50.975Z Reads: 214

```
I concur. BMS switch is sufficient.
```

---
## \#7 Posted by: michaelcpg Posted at: 2016-11-02T23:28:47.841Z Reads: 210

```
Anyone know if there's generally any difference in reliability between a BMS with softswitch and a standalone mosfet switch?
```

---
## \#8 Posted by: jmasta Posted at: 2016-11-02T23:31:47.988Z Reads: 208

```
[quote="JuniorPotato93, post:2, topic:12333, full:true"]
Well, an antispark switch is really just a electronic switch like the one already in the BMS, in terms of how they operate I mean. It's going to have a transistor that gets turned on opening the circuit just like any antispark switch does. I think the confusion here is that the "antispark" component of the antispark switch comes from the fact that the current does not arc over a small distance when being connected because here we are always connected, but we have a "valve" on it.

I might be a little off in my interpretation if I am someone feel free to correct me, but i think your okay. Only thing I'd be concerned about is do you know how much current your onboard switch is rated for?
[/quote]

The high voltage switching is achieved with the mosfets, like you've described.  We stack multiple fets in parallel to achieve the necessary current rating.  But the anti-spark function comes from the capacitor and resistor, which are connecting the gate to the drain.  This slows the inrush of current to the caps on the ESC, arresting the spark.  There is also a Zener diode from the source to the gate, which serves as a flyback diode
```

---
## \#9 Posted by: Namasaki Posted at: 2016-11-03T00:17:44.304Z Reads: 192

```
[quote="michaelcpg, post:7, topic:12333, full:true"]
Anyone know if there's generally any difference in reliability between a BMS with softswitch and a standalone mosfet switch?
[/quote]


I've had 2 stand alone anti-spark switches fail.(one of them in the first 5 min) The soft switch on my Bestech BMS has not failed yet.
```

---
## \#10 Posted by: Ackmaniac Posted at: 2016-11-03T00:34:54.317Z Reads: 186

```
My Vedder Anti Spark switch failed today when i connected the Battery to it. It doesn't switch off anymore and i get a spark. the good side is Esk8.de will take it back. Hopefully they will switch it because i kind of like it. 
I guess it would be better to use a additional xt-90 anti spark to close the connection between the Battery and the Anti Spark Switch. Eats some space but maybe this way they don't brake anymore.
```

---
## \#11 Posted by: rpn314 Posted at: 2016-11-03T03:06:53.385Z Reads: 176

```
[quote="Namasaki, post:9, topic:12333"]
[quote="michaelcpg, post:7, topic:12333"]
Anyone know if there's generally any difference in reliability between a BMS with softswitch and a standalone mosfet switch?
[/quote]

I've had 2 stand alone anti-spark switches fail.(one of them in the first 5 min) The soft switch on my Bestech BMS has not failed yet.
[/quote]

Yeah, hard to go wrong with a Bestech (kinda wish I had one). I'm using @chaka's version of Vedder's anti-spark switch (bought the board on oshpark and soldered it myself). No issues so far.
```

---
