# How to not fry my step down

### Replies: 21 Views: 1263

## \#1 Posted by: GhettoFab.rictation Posted at: 2017-11-25T11:19:46.372Z Reads: 148

```
I have a cheap little step down converter that can handle fifty volts but it never stated watts or amps it could handle. The voltmeter on the unit went out and it's a shame but useless really so no big deal but it still works and I connect it to 25v 6s no issue. But what can I place in front of it that will help it out a little? Or could I run a step up converter to the 12v lights shown? I would use the vesc 5v supply to step up on either the receiver or other plugs( not sure what they are called the white ones with 5v and 3.3v). Please help everyone! I have a switch with two mosfets on the way and feel comfortable after that but idk can anyone help suggest the step down converter in series or step up converter from vesc??? <img src="/uploads/db1493/original/3X/4/6/46b1153998ee3fd31b375797548a2c986f198437.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/5/b/5b6ea424fadb0ff3e3155f38e4066f822c948329.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/4/a/4ad5acec37dc20342e2f5a783e666c17e17eea68.jpg" width="281" height="500">
```

---
## \#2 Posted by: darkkevind Posted at: 2017-11-25T12:47:05.672Z Reads: 119

```
It doesn't matter what wattage or amp rating your battery is, the volt meter will draw as much current as it requires, the current draw from your ESC has no affect on it....
```

---
## \#3 Posted by: GhettoFab.rictation Posted at: 2017-11-25T12:50:46.805Z Reads: 117

```
The volt meter on the step down fried. Idk why because it states ok up to 50v but doesn't state the watt or amp limit. I have the other voltmeter I'm using. But the step down or step up converters are the question. Run 12s to the step down converter in series, or run a step up converter from the vesc?
```

---
## \#4 Posted by: krloz Posted at: 2017-11-25T13:12:23.006Z Reads: 106

```
Don't step up the vesc power. it is rated for a maximum of 1 amp so if you need more than 0.2 or 0.3 amp after stepping up you will damage the vesc
```

---
## \#5 Posted by: darkkevind Posted at: 2017-11-25T14:02:36.737Z Reads: 96

```
It doesn't state it because there is no watt/amp limit. Like I said, it draws as much current as it needs...
```

---
## \#6 Posted by: GhettoFab.rictation Posted at: 2017-11-25T14:35:19.835Z Reads: 83

```
I'm talking about the purchased step down. Doesn't state when I purchased it the limits. The voltmeter was ON the step down. So I'm talking about the converter as a whole handling the v w and amp
```

---
## \#7 Posted by: vishal_tejwani Posted at: 2017-11-25T15:23:11.535Z Reads: 70

```
If you have a bms , use step down converter for led lights

And connect your Batteries directly to esc , i do the same no problems yet
```

---
## \#8 Posted by: GhettoFab.rictation Posted at: 2017-11-25T20:35:51.519Z Reads: 64

```
No bms. No monies and bms seems complicating
```

---
## \#9 Posted by: Quezacotl Posted at: 2017-11-25T21:12:38.715Z Reads: 65

```
That step-down converter you have appears to be the popular LM2596-based module, which is rated about 3A. I use the same for my lights and many projects.
```

---
## \#10 Posted by: egzplicit Posted at: 2017-11-25T23:47:49.994Z Reads: 55

```
Does it work for 42v (10s fully charged)? Everywhere I’ve seen this step down they never rate it at more than 35-40v
```

---
## \#11 Posted by: Quezacotl Posted at: 2017-11-26T07:19:56.544Z Reads: 47

```
Yes it does. You can find all info on the datasheet. Anytime you don't know about some module, just search for the part's datasheet.
```

---
## \#12 Posted by: GhettoFab.rictation Posted at: 2017-11-26T10:37:20.644Z Reads: 44

```
Yes this is true. It seems to barely handle 12s though as I bought a set of four and I'm down to two with the volt meters blown on the other two they completely blew out.
```

---
## \#13 Posted by: egzplicit Posted at: 2017-11-26T10:40:38.446Z Reads: 47

```
[quote="Quezacotl, post:9, topic:39238"]
LM2596
[/quote]

http://www.ti.com/lit/ds/symlink/lm2596.pdf This shows 40v max so giving it has some safety margins, 10s should be ok but 12s is a stretch.
```

---
## \#14 Posted by: GhettoFab.rictation Posted at: 2017-11-26T10:46:51.294Z Reads: 49

```
It says 50v on it idk here it a more clear pic <img src="/uploads/db1493/original/3X/4/9/4902e2ff7addf53ea02cc855d9f225a07462b294.jpg" width="281" height="500">
```

---
## \#15 Posted by: egzplicit Posted at: 2017-11-26T11:02:41.826Z Reads: 46

```
50V on the capacitor, but the step down module (LM2596) is only rated at 40v:

> • 3-A Output Load Current
> • Input Voltage Range Up to 40 V

See the linked PDF from above.
```

---
## \#16 Posted by: GhettoFab.rictation Posted at: 2017-11-26T11:10:10.530Z Reads: 47

```
I checked pdf no complete picture to verify it's the same I saw circuit board looked little different on one page but it was just breezing through it. I'm going to probably buy different step down
```

---
## \#17 Posted by: GhettoFab.rictation Posted at: 2017-11-26T11:12:26.147Z Reads: 48

```
https://www.amazon.com/DROK-Converter-Transformer-Inverter-Automotive/dp/B01739WR7O/
```

---
## \#18 Posted by: Quezacotl Posted at: 2017-11-26T17:09:54.767Z Reads: 40

```
"Absolute max supply voltage = 45V" says on LM2596 datasheet.
```

---
## \#19 Posted by: GhettoFab.rictation Posted at: 2017-11-27T04:14:40.847Z Reads: 31

```
Yeah need that step down shown :confused: thank you guys though for including information!!
```

---
## \#20 Posted by: SkaterBoy58 Posted at: 2017-11-27T04:58:37.825Z Reads: 29

```
Guys - I have experienced these converters blowing up ( literally) on 42V input when data sheet says 40V max input  . ( thought it would have a  bit of tolerance)
Easiest way is just to add 4 diodes in series on +ve input to always have voltage <40V 
Cheers
```

---
## \#21 Posted by: GhettoFab.rictation Posted at: 2017-11-27T21:29:25.209Z Reads: 26

```
What kind of diodes? And if I buy the 55v buck down no need for them
```

---
