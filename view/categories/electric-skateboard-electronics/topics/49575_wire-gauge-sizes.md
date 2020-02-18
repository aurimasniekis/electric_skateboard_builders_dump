# Wire gauge sizes

### Replies: 15 Views: 1125

## \#1 Posted by: buip Posted at: 2018-03-20T02:08:31.368Z Reads: 195

```
Hey everyone

I'm about to build my battery and electrical system but would like some input before I start buying wires. I've looked at all the other threads but could not find definite answers to these questions. 

1)I am about to solder together a 10S3P Li Ion battery using LG HG2, but was wondering what size nickel strips are recommended or if I should use 10AWG tinned copper [wire](https://www.amazon.com/gp/product/B075891392/ref=ox_sc_sfl_title_6?ie=UTF8&psc=1&smid=A1P2Y1BEUUWGO2)? Or copper rods?

2)Wondering if my wire sizes are adequate for my battery and system, mainly regarding the charging wires. ![electrical schematic|690x250](upload://nNGYbMDS8pAXv6awE5I5oe44jQK.jpg)
```

---
## \#2 Posted by: b264 Posted at: 2018-03-20T02:24:58.954Z Reads: 180

```
2) yes, they are adequate
```

---
## \#3 Posted by: Namasaki Posted at: 2018-03-20T03:20:37.341Z Reads: 168

```
Nice diagram btw.
```

---
## \#4 Posted by: deucesdown Posted at: 2018-03-20T03:29:00.071Z Reads: 167

```
Is the xt90 the load? Gauges look good, even a bit overkill. Get high strand count tinned silicone wire. Check acerracing super worm. Prices are okay, US store, good reputation. Their ebay store may be a bit cheaper.

Don't use copper rod -- I think vibrations will break the joints.

Your pack is specified for 20a per cell (60a, 3p). For nickel I think .20mm x 10mm per series connection will be close to meeting the spec.
```

---
## \#5 Posted by: treenutter Posted at: 2018-03-20T03:29:09.776Z Reads: 163

```
Some helpful info here too:

http://www.electric-skateboard.builders/t/wire-gauge-in-esk8/213
```

---
## \#6 Posted by: buip Posted at: 2018-03-20T03:43:25.311Z Reads: 151

```
thanks for the input
```

---
## \#7 Posted by: buip Posted at: 2018-03-20T03:45:10.563Z Reads: 144

```
thank you namasaki
```

---
## \#8 Posted by: buip Posted at: 2018-03-20T03:50:38.889Z Reads: 137

```
Yes the xt90 is the load. Are you saying the 10AWG and 18AWG are both oversized? What sizes would you recommend? 

Thank you
```

---
## \#9 Posted by: buip Posted at: 2018-03-20T04:00:09.172Z Reads: 128

```
thanks treenutter
```

---
## \#10 Posted by: b264 Posted at: 2018-03-20T04:43:01.567Z Reads: 121

```
For the record, I don't think 10AWG and 18AWG are oversized.  I don't think they are undersized, either.
```

---
## \#11 Posted by: deucesdown Posted at: 2018-03-20T04:48:44.202Z Reads: 116

```
Hm I'm reconsidering. 10awg is good around the battey pack.18awg is good for charge.

I'm going with 10awg wiring to battery, and 12awg to each vesc. Can go bigger, but it's a pain. The wires barely fit the connectors and it's had to route wires.
```

---
## \#12 Posted by: Hummie Posted at: 2018-03-20T04:58:05.533Z Reads: 112

```
you should make your motor wires bigger than your battery wires if you want to have the wire sizes in relation to the amps running within them.   Motor wires will have up to maybe 4x more amps depending on the esc settings.   the amps run circularly through the motor and esc not to the other side with the battery and capacitors.
```

---
## \#13 Posted by: deucesdown Posted at: 2018-03-20T05:27:26.366Z Reads: 102

```
I reread this like 4 times and I'm still lost :slight_smile:
Motor wires are 3 phase AC with PWM. I'm trying to imagine how they actually carry more current. The way current is measured is weird, right?

And most motor wires are quite thin, like the motor side of focbox. Everyone seems okay with this?
```

---
## \#14 Posted by: Hummie Posted at: 2018-03-20T05:35:55.980Z Reads: 98

```
the current is regular standard current.  the real thing.    

 a lot of people are ok with little motor wires and it's the norm but none the less that's where the majority of the amps are.   at least there's 3 phase wires so any of the single phase wires will only experience this higher current for half the time.
```

---
## \#15 Posted by: b264 Posted at: 2018-03-20T06:44:54.910Z Reads: 88

```
[quote="deucesdown, post:13, topic:49575"]
Motor wires are 3 phase AC with PWM. I’m trying to imagine how they actually carry more current.
[/quote]

They carry more current because the capacitors on the VESC absorb the peaks and valleys and draw a more constant load from the battery
```

---
