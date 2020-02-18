# LED switch with Vedders Anti Spark

### Replies: 29 Views: 2004

## \#1 Posted by: florensvb Posted at: 2017-08-05T17:34:02.026Z Reads: 195

```
Hey guys,

So i just purchased this Anti Spark from @Martinsp 

<img src="/uploads/db1493/original/3X/b/b/bb3d17dce4ca332b695911a683f92dec87c20afc.JPG" width="690" height="388"><img src="/uploads/db1493/original/3X/6/d/6d7edb1feb6e57b0c87544833a52e3e58e50a9fd.JPG" width="690" height="388">

And I have this LED from  on/off switch that i just recently fried:

<img src="/uploads/db1493/original/3X/8/c/8ce731f6014cf076e9517062466e1c680fff3466.jpg" width="375" height="500">

Any chance I can make the LED switch work with the Anti Spark, since the LED has 4 cables, but the Anti Spark only has three soldering pads?

Thanks !
```

---
## \#2 Posted by: willpark16 Posted at: 2017-08-05T17:45:41.173Z Reads: 183

```
Short answer is yes
```

---
## \#3 Posted by: willpark16 Posted at: 2017-08-05T17:47:57.946Z Reads: 179

```
<img src="/uploads/db1493/original/3X/d/c/dc3cdcf9042128800df5825c6c8f7b6f54d05418.JPG" width="690" height="387">
```

---
## \#4 Posted by: florensvb Posted at: 2017-08-05T17:52:26.389Z Reads: 171

```
Thanks @willpark16 for your answer!

could you just explain some of the wiring for me? I am assuming you just connected the LED + to the OUT + ?

then you have the switch + - on the left and right pads and the LED - on the center pad?
```

---
## \#5 Posted by: florensvb Posted at: 2017-08-05T17:53:15.470Z Reads: 167

```
Actually that LED switch you posted has 5 wires, but mine only has 4?
```

---
## \#6 Posted by: willpark16 Posted at: 2017-08-05T17:56:51.401Z Reads: 164

```
Is urs only a 4 pin switch?
```

---
## \#7 Posted by: florensvb Posted at: 2017-08-05T17:58:16.127Z Reads: 160

```
Yes it has LED + - and SWITCH + -, resulting in a total of 4 wires
```

---
## \#8 Posted by: willpark16 Posted at: 2017-08-05T18:10:43.365Z Reads: 160

```
Then just that
```

---
## \#9 Posted by: florensvb Posted at: 2017-08-05T18:18:12.688Z Reads: 154

```
Can you explain where to put which wire?
```

---
## \#10 Posted by: Martinsp Posted at: 2017-08-05T18:19:57.149Z Reads: 147

```
Do you have a multimeter?
```

---
## \#11 Posted by: florensvb Posted at: 2017-08-05T18:26:34.457Z Reads: 142

```
no :frowning:
```

---
## \#12 Posted by: Martinsp Posted at: 2017-08-05T18:27:00.103Z Reads: 140

```
I think that the LED is connected to one of the switch pads (negative) internally to the switch therefore you have 4 wires instead of one. but to prove this you need a multimeter.
```

---
## \#13 Posted by: jmasta Posted at: 2017-08-05T18:27:17.041Z Reads: 146

```
Your switch has to have 3 pins. The Fechter/Vedder anti-spark uses a SPDT switch (single pole, double throw). The negative of the LED is wired to the negative of the anti-spark switch

Don't hook up the positive of your LED to the positive of the anti-spark without an appropriately sized resistor, unless the LED is rated for that voltage.  Many of the LEDs in those switches are only 12V or 24V, and can't be hooked up to full pack voltage.  I recently switch to a 220V LED switch, which works well for 12S at ~50V (not super bright, but also not dim)
```

---
## \#14 Posted by: Martinsp Posted at: 2017-08-05T18:29:15.191Z Reads: 141

```
If you dont mind having the regular switch and not the round one. And you care about the LED indicating that the board is on, it would be easier just to wire the LED and a resistor in series to the output of the switch and have the LED as a "separate" unit.
```

---
## \#15 Posted by: florensvb Posted at: 2017-08-05T18:29:35.088Z Reads: 141

```
on the led it says

_Ui:36VDC lth: 1A_
_ZLQ-B48V_
```

---
## \#16 Posted by: florensvb Posted at: 2017-08-05T18:31:28.485Z Reads: 133

```
hm thats an interesting approach, as the led switch is kinda hard to press down with the thumb.. not too practical. but i dont have a resistor
```

---
## \#17 Posted by: Martinsp Posted at: 2017-08-05T18:32:41.711Z Reads: 132

```
I will throw that in the package for you both the LED and the resistor of appropriate value. :) Just tell me what battery pack you are using so I can calculate the value
```

---
## \#18 Posted by: florensvb Posted at: 2017-08-05T18:39:21.798Z Reads: 129

```
Wow you're amazing. I have an 8S battery with 8000mah
```

---
## \#19 Posted by: Martinsp Posted at: 2017-08-05T18:40:22.409Z Reads: 123

```
It is like 10 cents :D Hopefully karma sees this :D :D (joke)
```

---
## \#20 Posted by: jmasta Posted at: 2017-08-05T18:40:36.768Z Reads: 126

```
Your LED switch will work natively with full pack voltage then
```

---
## \#21 Posted by: florensvb Posted at: 2017-08-05T18:42:32.692Z Reads: 117

```
thank you @Martinsp @jmasta @willpark16 !
```

---
## \#22 Posted by: Martinsp Posted at: 2017-08-05T18:43:37.172Z Reads: 114

```
The switch would work, it is within the specs pretty much. But unfortunately @florensvb does not own a multimeter so we are not able to figure out how to wire it correctly.
```

---
## \#23 Posted by: florensvb Posted at: 2017-08-05T18:45:17.399Z Reads: 113

```
Wait but we dont need to figure it out anymore, right? I'll just use your plain black switch with the 3 wires and then hook up the LED + and - to the leads that go OUT of the anti spark?
```

---
## \#24 Posted by: Martinsp Posted at: 2017-08-05T18:47:10.618Z Reads: 114

```
Yes that is another option.
```

---
## \#25 Posted by: florensvb Posted at: 2017-08-05T18:48:26.551Z Reads: 108

```
haha wait then what were you suggesting? :D

Or you're still trying to make the black switch obsolete and use the led switch the proper way? 

I am still interested if that could work of course
```

---
## \#26 Posted by: Martinsp Posted at: 2017-08-05T18:51:02.226Z Reads: 108

```
I just asked the employee about this on DIY website. :D I will notify you once they reply :D
```

---
## \#27 Posted by: florensvb Posted at: 2017-08-05T18:54:34.757Z Reads: 108

```
you're a legend
```

---
## \#28 Posted by: Martinsp Posted at: 2017-08-05T18:58:00.752Z Reads: 116

```
<img src="/uploads/db1493/original/3X/f/4/f4284000e0b82c23c01df1c5f0389e0794ae3fd4.png" width="380" height="500">
OK so as expected they said they cant give me the design files of their switch and the pinout of the push button switch :D I am pretty sure that they were either laughing or crying in the office because of me asking such a stupid question. :D just like asking "hey can you give me design files of your product so that I can copy it and sell for cheaper?" :D 

Seems like the external LED is the only option now.
```

---
## \#29 Posted by: torqueboards Posted at: 2017-08-05T21:30:48.443Z Reads: 105

```
Finding the pinout of the push button switch is as simple as searching the on/off switch on ebay or google. You can also cut the heatshrink and read the pinout.

<img src="/uploads/db1493/original/3X/5/5/55f0faacd3f0cd77643353745974298cf0c3656d.png" width="500" height="*">

Finding the pinout for the on/off button is as simple as flipping over the switch and reading the PCB.

<img src="/uploads/db1493/original/3X/2/4/240d45b0e57dec5bd7c2b322ae9866694e2f66df.png" width="600" height="*">

If I remember correctly the vedder switch as jmasta has already mentioned uses an SPDT switch. The Vedder switch doesn't use an LED switch. They're two different styles of switches. Can't remember why but your probably better off buying a SPDT type switch instead of trying to re-use that LED one as the two switches are different.
```

---
