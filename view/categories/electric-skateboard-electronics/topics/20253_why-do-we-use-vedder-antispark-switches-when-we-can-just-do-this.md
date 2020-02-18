# Why do we use Vedder Antispark switches when we can just do this?

### Replies: 29 Views: 2345

## \#1 Posted by: Aborn Posted at: 2017-04-04T12:08:44.471Z Reads: 435

```
<img src="/uploads/db1493/original/3X/c/5/c5177b2ad8ff5115addd430f84df978e809ed584.jpg" width="375" height="500">
```

---
## \#2 Posted by: Maxid Posted at: 2017-04-04T12:25:43.923Z Reads: 419

```
so a mosfet switch? that's what the vedder is
```

---
## \#3 Posted by: Aborn Posted at: 2017-04-04T12:45:30.390Z Reads: 419

```
<img src="/uploads/db1493/original/3X/2/9/29097132817268b832fd8ffb688054aec385ce57.jpg" width="665" height="500">

It just seems overcomplicated and overpriced then?
```

---
## \#4 Posted by: Stevemk14ebr Posted at: 2017-04-04T12:52:36.075Z Reads: 407

```
It's not complicated, it's 3 mosfets in series because you will have trouble finding a single switch able to handle the current and voltage. Someone explain to me what r2 and c1 are for though
```

---
## \#5 Posted by: Aborn Posted at: 2017-04-04T12:53:21.416Z Reads: 401

```
All my questions have been answered, thank you. :slight_smile:

Wait, so a "inrush limiter" is not a inrush limiter but rather just a mosfet switch? ?
```

---
## \#6 Posted by: Stevemk14ebr Posted at: 2017-04-04T12:55:06.600Z Reads: 395

```
I think the resistor and cap might be there for inrush limiting but you'd have to ask someone better at EE, I'm just a little programmer
```

---
## \#7 Posted by: Maxid Posted at: 2017-04-04T13:29:27.261Z Reads: 382

```
It's not and it's not.

you have multiple mosfets in parallel to be able to use high currents and some additional parts to allow a range of voltages and safety features to keep the mosfets healthy.

The switch is like 30 bucks with the most expensive parts being the mosfets and the PCB.
a mosfet like this is a couple bucks each so that adds up.

You can make the switch out of breadboard if you want to save a couple bucks.
```

---
## \#8 Posted by: Aborn Posted at: 2017-04-04T13:49:21.281Z Reads: 349

```
Thanks you for clearing things up for me :slight_smile:
```

---
## \#9 Posted by: jmasta Posted at: 2017-04-04T15:17:25.343Z Reads: 335

```
[quote="Stevemk14ebr, post:4, topic:20253, full:true"]
It's not complicated, it's 3 mosfets in series because you will have trouble finding a single switch able to handle the current and voltage. Someone explain to me what r2 and c1 are for though
[/quote]



[quote="Aborn, post:3, topic:20253, full:true"]
<img src="/uploads/db1493/original/3X/2/9/29097132817268b832fd8ffb688054aec385ce57.jpg" width="665" height="500">

[/quote]

The Zener diode injects a forward voltage of 12V, so the difference between the Gate and Source voltage is independent of the battery voltage

R2 and C1 in combination are the so-called "current inrush limiters"

* R2 limits the current to C1

* C1 is a capacitor and therefore it takes a finite time to charge and discharge. When first activating the switch, C1 slowly "fills up" until the Drain voltage reaches is high enough to open the mosfet.  If you have a voltage meter installed on your board, you'll notice it takes a second or two to reach full pack voltage (i.e., not instantaneously)

This is what prevents the spark and activates the circuit... or so I understand it.  But I'm a mechanical/aerospace guy, not an electrical engineer :wink:
```

---
## \#10 Posted by: Aborn Posted at: 2017-04-04T18:07:49.587Z Reads: 273

```
Very good explanation, but is the current limiting necessary?

Will using only the mosfet wear it out?
```

---
## \#11 Posted by: jmasta Posted at: 2017-04-04T19:20:07.184Z Reads: 265

```
Yes. The purpose of this circuit is to (1) switch on/off the high current lines, and (2) limit the inrush of current to the capacitors on the ESC to suppress the spark.   Without the current inrush limiter, you have just made an electronic switch.  And C1 & R1 are the cheapest components on the board. You're talking less than a dollar. It doesn't limit the current of your system - just slows the influx of current on initial contact.  

0...10...20...30...40V, instead of 0...40V [spark!]
```

---
## \#12 Posted by: Aborn Posted at: 2017-04-04T19:33:56.364Z Reads: 255

```
[quote="jmasta, post:11, topic:20253"]
0...10...20...30...40V, instead of 0...40V [spark!]
[/quote]
Thanks for the dummy explanation XD

I just didnt think a mosfet could make a spark, but hearing it's that cheap, i'll just include it :p thanks a lot for your help.
```

---
## \#13 Posted by: pennyboard Posted at: 2017-04-05T03:13:41.428Z Reads: 234

```
I've been using this on my 12s setup for about 2 months, and I used for 4 months on an 8s setup before that. Never had any problems, and it cost like $5 from Lowe's. All I did was solder it into the wire between my batteries and my VESC.
<img src="/uploads/db1493/original/3X/1/4/1445541ec51fcdb82eec8e786640ff5f2d3321e3.jpg" width="375" height="500">
```

---
## \#14 Posted by: benwong Posted at: 2017-04-05T03:28:50.123Z Reads: 218

```
@pennyboard how many Amps this switch can handle?
```

---
## \#15 Posted by: pennyboard Posted at: 2017-04-05T14:41:08.559Z Reads: 208

```
@benwong  I've been running 50 amps at 44 Volts with no problem.
```

---
## \#16 Posted by: mmaner Posted at: 2017-04-05T14:42:07.482Z Reads: 210

```
I would love to know the make & model of that switch.  I've seen single throw switches that claim to handle that many amps, but they are huge.
```

---
## \#17 Posted by: benwong Posted at: 2017-04-05T14:56:15.467Z Reads: 207

```
i got this switch too. 
they claim that can handle 50amps too. i haven try to connect yet. 

<img src="/uploads/db1493/original/3X/7/9/794734d30ba00a964a6f83731e49acb311f54ad1.jpg" width="337" height="500">
```

---
## \#18 Posted by: pennyboard Posted at: 2017-04-05T16:18:55.342Z Reads: 189

```
Here's a picture of the packaging. Like I said, I bought it at Lowe's. It's rated for 20A at 125 volts, and since the determining factor in whether or not the switch is burns out is determined by the power dissipated in the wiring of the switch (I think), dividing 125 volts by the 44 volts that 12s runs gives 2.84, so the switch can handle 2.84*20 amps at 44 volts, which is about 55 amps, and like I said, it has yet to fail me after almost 9 months.
<img src="/uploads/db1493/original/3X/f/b/fb2d24b475ae804f45617378f9fdf4c7fc3f45ea.jpg" width="375" height="500">
```

---
## \#19 Posted by: mmaner Posted at: 2017-04-05T16:26:22.107Z Reads: 185

```
very cool, Ill have to check into that.
```

---
## \#20 Posted by: Maxid Posted at: 2017-04-05T16:31:37.912Z Reads: 181

```
[quote="pennyboard, post:18, topic:20253, full:true"]
It's rated for 20A at 125 volts, and since the determining factor in whether or not the switch is burns out is determined by the power dissipated in the wiring of the switch (I think), dividing 125 volts by the 44 volts that 12s runs gives 2.84, so the switch can handle 2.84*20 amps at 44 volts, which is about 55 amps
[/quote]
That is not how that works
the only reason the switch did not get destroyed by now is because 20A is fairly high and you have probably been cruising at a lower current most of the time. You still have a spark when connecting so that switch will wear out at some point.
```

---
## \#21 Posted by: pennyboard Posted at: 2017-04-05T16:48:59.810Z Reads: 162

```
Alright, good to know. And by spark, you're referring to a physical spark within the switch when it is thrown, I'm assuming? Also I've done fairly long, steep, uphill climbs (over a mile at greater than 15 degree incline), and I'm pretty sure I was pulling more than 20 Amps there for a long time, so the switch must more robust than advertised I guess. As long as it keeps working, I'll keep using it and then when it does blow out, just replace it with another $5 switch. Much better in my opinion than spending $60 on a switch.
```

---
## \#22 Posted by: Maxid Posted at: 2017-04-05T16:51:22.075Z Reads: 166

```
to destroy you will probably need quite a high current - i mean it needs to melt :scream: - but it will also not be efficient. On that climb you "lost" quite a lot of energy in heat.
```

---
## \#23 Posted by: pennyboard Posted at: 2017-04-05T16:55:40.928Z Reads: 165

```
Ah that makes sense. Although I've touched the switch several times after riding and it wasn't even warm. Also, now that I think about it, I think my explanation of why the switch can handle 50 amps may be correct. Because after all what causes the switch to melt is heat dissipation, which is determined by the power through a component, and power is v*i, so reducing voltage reduces the power, allowing an increase in current before the limits of the component are exceeded. I'm not trying to start a massive debate/argument, just trying to get to the bottom of this.
```

---
## \#24 Posted by: Maxid Posted at: 2017-04-05T17:34:35.185Z Reads: 164

```
The heat dissipation is P=R*I²
Only the current is important and the resistance of the switch. The squared current is also why higher currents are so damn annoying
```

---
## \#25 Posted by: pennyboard Posted at: 2017-04-05T21:36:16.644Z Reads: 158

```
Ah, okay, I was confusing the voltage drop across the switch with the voltage coming out of the batteries, which is why I used the wrong equation. Thanks for explaining that to me.
```

---
## \#26 Posted by: XBoard0 Posted at: 2017-04-06T01:34:47.365Z Reads: 163

```
I'm an electrical engineer and came across this post. I thought I would better explain how the current limiter works.

You are all correct with saying the current limiting comes from the resistor and capacitor network. However, it is R1 and C1 doing all the work, R2 is basically irrelevant.

When the switch is in the off position Vgs (gate-source voltage) is being shorted to zero. All the FETs are in cutoff and not conducting (since Vgs is less than the threshold voltage Vtn, Vtn is roughly 5V). Additionally, the voltage across C1 is at your pack voltage. If you don't understand why, think of the load across controller + - as a very small resistor. C1 is then effectively connected between ground and Pack+ through a 1K resistor.

Now lets throw the switch...

The voltage across a capacitor can not change instantly, so there is still the pack voltage across C1. This effectively keeps Vgs at ground (the FETs are still off). C1 starts to discharge through R1, R2, and the load. Current actually starts flowing backwards through controller as C1 discharges. As C1 continues to discharge, the voltage across the cap decreases, raising Vgs. Once Vgs surpasses the threshold voltage Vtn (~5V) the FET's start to conduct (they enter the saturation regime) and current flows through the controller in the correct direction and the voltage across the controller lines gradually increase, slowly turning on the controller. 

Note, that in the saturation regime the current flowing through the FETs are roughly proportional to Vgs^2, so the current given to the controller ramps up quadratically with Vgs. At some point the voltage across C1 goes to zero and then C1 starts charging in the opposite direction (hence why C1 must be non-polar). As we said the current the FETs pass is related to Vgs, but Vgs is controlled during switching transients by the voltage across C1. Since C1 is charged up very slowly through the giant resistor R1, the FETs turn on very slowly. Finally, once C1 is fully charged, the FETs are fully on and the controller can can use as much current as it likes.

As for R2, pretty sure all it does it prevent a spark across across the switch when turning it off due to C1 discharging. The zener diode just clamps Vgs so it can never rise above 12V, otherwise it would reach your pack voltage and many fets have a max Vgs of ~20V.
```

---
## \#27 Posted by: Aborn Posted at: 2017-04-06T11:24:09.469Z Reads: 147

```
That was your first post? Wow, and welcome to the community. Great to have an expert clear things up :)
```

---
## \#28 Posted by: JeffS Posted at: 2017-04-06T11:42:06.493Z Reads: 143

```
Noob question: Without the inrush current limiter, where do you see the spark?
```

---
## \#29 Posted by: Aborn Posted at: 2017-04-06T11:49:39.434Z Reads: 138

```
When you connect your battery

That could be using a connector or a switch.
```

---
