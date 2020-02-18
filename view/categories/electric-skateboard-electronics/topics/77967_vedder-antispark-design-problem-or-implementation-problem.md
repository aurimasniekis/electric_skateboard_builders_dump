# Vedder antispark, design problem or implementation problem?

### Replies: 26 Views: 1200

## \#1 Posted by: deltazeta Posted at: 2018-12-14T01:11:43.573Z Reads: 153

```
I have a vedder anti-spark currently, and I am moderately shook by the historically poor performance of these things.

![image|509x499](upload://pU8wRVr2OIDJR93nx9QRcl9Wy57.jpeg) 

Besides any obvious user error, I've seen some blaming the initial current being too much to handle for the mosfets, but it seems the vedder design should have a sufficient current inrush limiter. At least the multisim circuit simulation thinks so.
https://www.multisim.com/content/NLP7B94HVyqndpwCyjrKdE/vedder-anti-spark-switch/
 And with the mosfets on my current version rated for 75V and 240A each, those shouldn't be a problem either. 

Is the design itself not robust enough, or are there a lot of cheapo chinese fakes or something?
```

---
## \#2 Posted by: J0ker3366 Posted at: 2018-12-14T01:13:42.003Z Reads: 150

```
&lrm; @b264
```

---
## \#3 Posted by: NAF Posted at: 2018-12-14T01:37:58.903Z Reads: 176

```
Poor shitty ass mosfets on a lot of them.
```

---
## \#4 Posted by: b264 Posted at: 2018-12-14T01:54:14.633Z Reads: 172

```
They blow because they are operating in linear mode during inrush.  It's a design limitation on every one I've seen so far except one.

Imagine a FET is a resistor with a variable resistance.  When it's "off" the resistance is [nearly] infinity and when it's "on" the resistance is [nearly] zero.  That's all fine and dandy until you add capacitors to the load, like the filter capacitors on VESC and other ESCs.  Right when it turns on, it's effectively a momentary short circuit with [not really...] infinite current because the capacitors are empty.  So what the antisparks do is they limit inrush current by turning on not from zero to full blast, but gradually over several milliseconds they ramp from [nearly] infinity to [nearly] zero ohms.  It's this period during the ramp that is the problem, the FET itself is taking almost the entire load due to Ohm's law because the capacitors have effectively zero resistance to inrush.  It's said to be operating in "linear" or analog mode at this point, as opposed to "digital" mode where everything is either on or off with no in-between.  This is extremely stressful to the junctions inside the FET and technically exceeding the design limitations for a very brief period of time.  Each time it's powered-on, it's taking a tiny bit of damage.

The way to ameliorate this is much the same way a loopkey works -- you have a "precharge" circuit where the nonzero inrush-limiting resistance is provided by an *actual discrete resistor* instead of the FET junction itself.  So you have *one FET* with a resistor in series, typically a 5.6 ohm resistor, that is separate from the *one or more FETs* on the main power switch.

So in order of operation, you'd have a single FET turn fully on [nearly] instantaneously (digitally) with a resistor in series to charge the filter capacitors, then once the output voltage approached the supply voltage (meaning the capacitors are nearing full charge) then the main FET(s) turn on [nearly] instantaneously (digitally) to supply high-current power to the system.  This is never operating in "linear" mode but is "fully digital" and will not suffer the incessant failures that plague the inrush-limiting Vedder design.  The power limiting and heating is moved to a discrete resistor instead of burning off the energy inside the FET junction itself, which stays cool during inrush.
```

---
## \#5 Posted by: mmaner Posted at: 2018-12-14T01:54:51.560Z Reads: 148

```
AS switches need a precharhe circuit to not blow the fets. That doesn't exist yet. The best you can do is an XT90-s between the battery and the switch. That won't save it forever, but it helps.
```

---
## \#6 Posted by: mmaner Posted at: 2018-12-14T01:55:14.534Z Reads: 143

```
Or what @b264 said 😀
```

---
## \#7 Posted by: b264 Posted at: 2018-12-14T01:55:49.892Z Reads: 138

```
LoL ninja'd by mere seconds :-)
```

---
## \#8 Posted by: mmaner Posted at: 2018-12-14T01:56:24.405Z Reads: 138

```
Yep, it happens 😀
```

---
## \#9 Posted by: deltazeta Posted at: 2018-12-14T02:02:23.326Z Reads: 132

```
ah great explanation, I didn't realize the fets shouldn't be used in linear mode. I wonder if a traditional current inrush limiter like a thermistor could be used. I guess I would classify that as a design flaw. Time to do more investigating on this, thanks @b264 and @mmaner
```

---
## \#10 Posted by: b264 Posted at: 2018-12-14T02:02:36.006Z Reads: 129

```
[quote]
Vedder antispark, design problem or implementation problem?
[/quote]

So the TL;DR is it's a design problem.  We need digital switches with precharge instead of analog ones with inrush limiting.
```

---
## \#11 Posted by: ervinelin Posted at: 2018-12-14T02:03:02.448Z Reads: 117

```
Do people do this? Install an antisparks XT90 (permanently?) Just before the antispark switch?
```

---
## \#12 Posted by: b264 Posted at: 2018-12-14T02:04:40.904Z Reads: 115

```
[quote="mmaner, post:5, topic:77967"]
The best you can do
[/quote]

You can do better than that -- you can put a momentary pushbutton switch in series with a 5W 10 ohm resistor connected around the antispark on the negative side.  If you push the button right before you turn it on, you won't damage the antispark switch when you do turn it on.

Or even better than that, use loopkeys until you have a fully digital antispark ;-)
```

---
## \#13 Posted by: mmaner Posted at: 2018-12-14T02:04:56.901Z Reads: 114

```
I always put an XT90-S on my battery packs. I can't prove it helps, but it doesn't hurt and I 'think' it helps. 

I mean, it's 3 bucks for a little insurance.
```

---
## \#14 Posted by: Pedrodemio Posted at: 2018-12-14T02:41:45.359Z Reads: 115

```
so a cheap simple solution would be to use a 555 timer as a delay for the main MOSFET's  to turn on?
```

---
## \#15 Posted by: deltazeta Posted at: 2018-12-14T03:54:32.434Z Reads: 113

```
designs where the mosfets are placed very close to the esc and after the large capacitors, i.e. integrated solutions (unity, flipsky 6.6), would mostly likely not have to deal with very much inrush current and as a result be much more robust
```

---
## \#16 Posted by: b264 Posted at: 2018-12-14T03:58:53.137Z Reads: 116

```
The cheapest and simplest solution is to use an XT90S loopkey.

If roll-to-start is something you absolutely must have, I would use an MCU like the [ATtiny25](https://www.digikey.com/product-detail/en/microchip-technology/ATTINY25-15ST/1611-ATTINY25-15STCT-ND/6833095), a tiny [regulator](https://www.digikey.com/product-detail/en/ZXTR2005K-13/ZXTR2005K-13DICT-ND/4279448/?itemSeq=266929706), and some logic-level low-Rds MOSFETs, but this will involve some low-level code writing and specialized hardware to write the firmware to the MCU.
```

---
## \#17 Posted by: b264 Posted at: 2018-12-14T04:06:41.751Z Reads: 119

```
[quote="deltazeta, post:15, topic:77967, full:true"]
designs where the mosfets are placed very close to the esc and after the large capacitors, i.e. integrated solutions (unity, flipsky 6.6), would mostly likely not have to deal with very much inrush current and as a result be much more robust
[/quote]

Correct; If the e-switch is on the ESC side of the filter capacitors instead of the battery side, then an analog inrush limiter or no inrush limiter at all will be sufficient.  However, then you have the leakage current of the filter caps as a constant draw even while powered-down, disconnecting power from the ESC to work on something does not power it down (i.e. it can still shock you), and if any one of the 3 devices break, you have to replace all 3.
```

---
## \#18 Posted by: b264 Posted at: 2018-12-14T04:18:43.410Z Reads: 115

```
Also in lieu of roll-to-start, you can just leave your board on.  It could probably idle for months or more on a full charge.  (If there aren't lights and stuff on, just the ESCs and receiver)  Turning it off would be prudent if it were to be stored or something.  You could turn the remote off instead.
```

---
## \#19 Posted by: lrdesigns Posted at: 2018-12-14T04:19:38.829Z Reads: 114

```
The FatBoy antisparks have a pre charge. Not heard of anyone breaking one yet. 

https://shop.3dservisas.eu/collections/fatboy-antispark-switches/products/fatboy-mini-sparky-switch-50a-200a-100v-pre-charged-anti-spark-switch-with-push-to-start?variant=12506550894685
```

---
## \#20 Posted by: b264 Posted at: 2018-12-14T04:19:57.096Z Reads: 113

```
[quote="lrdesigns, post:19, topic:77967"]
The FatBoy antisparks have a pre charge. Not heard of anyone breaking one yet.
[/quote]

[quote="b264, post:4, topic:77967"]
It’s a design limitation on every one I’ve seen so far except one.
[/quote]


That's the one I was referring to above ;-)
```

---
## \#21 Posted by: deltazeta Posted at: 2018-12-14T04:20:51.509Z Reads: 106

```
Was actually looking to buy one, but sadly its out of stock :pensive:
```

---
## \#22 Posted by: DeathCookies Posted at: 2018-12-17T02:52:42.032Z Reads: 91

```
[quote="b264, post:20, topic:77967"]
It’s a design limitation on every one I’ve seen so far except one.
[/quote]

The problem of hyped products sold at the perfect moments... :see_no_evil: So many broken FlierSwitches and so on.....
```

---
## \#26 Posted by: pjotr47 Posted at: 2018-12-17T21:34:49.800Z Reads: 89

```
I broke 2 antisparks in one week :confused:
```

---
## \#27 Posted by: deltazeta Posted at: 2018-12-19T08:31:40.211Z Reads: 87

```
I've been thinking about some ways of solving this issue, and this one i'm particularly fond of.

![image|690x388](upload://xVP1VrQoScmTrcQbzrKATwy8yML.png) 

The momentary switch connects a resistor in series and precharges the vesc caps, while a secondary cap gets charged to turn on a latching output for the mosfet, which would turn on as fast as possible. After a certain amount of time, the circuit latches and is considered on and the momentary button can be released. Similarly the button will need to be held for the circuit to turn off.

The diagram is a bit off, since i haven't figured out how to use the right mosfet in the simulator.

@b264 any opinions? or more importantly anything that screams wrong?
```

---
## \#28 Posted by: deltazeta Posted at: 2018-12-29T23:21:47.875Z Reads: 72

```
https://www.youtube.com/watch?v=1qRWBkrcnAM
This is a great video about the linear region operation. The standard irfs7730 fets can't even handle a single amp safely until the voltage difference across the drain and source drops to 20V. Its no wonder the fets blow so easily with typical high voltage packs.
```

---
## \#29 Posted by: deltazeta Posted at: 2018-12-30T04:23:01.036Z Reads: 69

```
actually looking at the simulation of the switch, the inrush current is actually adequately small for the fets, so I'm at a loss again as to why the fets blow. I'll throw my switch under an oscilloscope later to verify the current really is low enough.
```

---
