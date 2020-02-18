# MOSFET antispark switch

### Replies: 11 Views: 1634

## \#1 Posted by: Russell23 Posted at: 2017-06-12T22:41:23.111Z Reads: 226

```
I'm making a MOSFET anti spark switch for my vesc and I was wondering if this diagram would work
<img src="/uploads/db1493/original/3X/7/5/75a9a6adcefdebc329bf9c7f834dbbe7acbb5272.jpg" width="281" height="500">
Parts
MOSFET
 http://s.aliexpress.com/Yj2m2iuQ 
Diode
 http://s.aliexpress.com/fYvYVVNV 
Resistor
 http://s.aliexpress.com/EJrQB7Rz
Led push button
http://s.aliexpress.com/fQjqIZjU
```

---
## \#2 Posted by: chinzw Posted at: 2017-06-13T00:04:04.580Z Reads: 199

```
Why not use the tried and tested diagrams for vedder/fechter anti-spark?
```

---
## \#3 Posted by: Russell23 Posted at: 2017-06-13T06:41:26.237Z Reads: 165

```
Its the same as all the vedder diagram but the layout is different and I'm just wondering if my diagram would work
```

---
## \#4 Posted by: goldenHusky Posted at: 2017-06-13T13:10:00.664Z Reads: 151

```
Hi @Russell23
some thoughts:

- make sure that the trace that's coming from pin 1 of the Mosfet  doesn't bridge your 15k resistor and the zener diode. Pin 1 only should make contact between the 15k resistor and the zener diode

- what is the 400V/3A diode for?

- you will not be able to switch off with this circuit diagram, you will either need a pulldown resistor between gate and source or a SPDT switch. Make sure to choose the correct value for the pulldown or your 12V zener diode will be useless

- I recommend using at least 2 of your Mosfets in parallel and keep the traces and stuff as short and wide as possible.

Edit:
- I also think that 15k is too low, Benjamin uses a 1Mohm resistor, don't know what zener diode you want to use but the current through it might be too high

- your circuit does not have a precharge circuit. I recommend implementing that, otherwise you could kill the Mosfets due to a too high di/dt
```

---
## \#5 Posted by: Russell23 Posted at: 2017-06-13T17:29:02.829Z Reads: 123

```
•The diode lets buildup current flow from the - to the + lead which is the opposite of the way current normally flows, this is because of an electron buildup that can occur and destroy a circuit if a diode is not there to let the electrons flow back.
 •And I'm using 2 15k ohm resistor which makes it 30 ohm
•and for the switch I'm using a led push button
 http://s.aliexpress.com/fQjqIZjU
@goldenHusky
```

---
## \#6 Posted by: goldenHusky Posted at: 2017-06-13T19:00:47.781Z Reads: 116

```
@Russell23 Yea, anyway I doubt it will work, but just try it. Don't use your Vesc at the first try, use an inexpensive high load resistor or something like that instead.
```

---
## \#7 Posted by: Russell23 Posted at: 2017-06-13T21:40:54.533Z Reads: 113

```
It worked for this guy
https://www.electric-skateboard.builders/t/eboard-mosfet-switch/5738
@goldenHusky
```

---
## \#8 Posted by: JdogAwesome Posted at: 2017-06-13T22:17:45.047Z Reads: 103

```
@Russell23 @goldenHusky Hey guy thought I'd drop by and give some insight because I've been building these for a while. 

Russell your design looks ok to start, would be a lot better if it was like an Eagle CAD design or whatever​ but that works fine lol. First off, DONT buy your parts from AliExpress, don't get me wrong AliExpress is great but not for quality electronic components. Almost all of the parts on there are fake or have crappier to WAY shittier specs then there legitimate counterparts. I recommend Arrow.com because there prices are 1/2 of Mouser or Digikey, they offer free shipping and all there items, so far, seem to be of great quality. 

With that out of the way I will address @goldenHusky concerns.  To start I agree that you should make sure none of your traces or wires touch or short, though that's pretty standard with any circuit lol. Second, like Russell said the reverse current diode is a necessary part of the circuit, do not remove it. Third, you definitely need to add a pull down resistor to the gate to make sure it turns off, I use a 10K resistor and that should work fine once you replace your 15K current limiting resistor with a 4.7K one which leads me into point number four. 15K is not to low if anything it's to high because you want to make sure the zener has enough current to stay active. Like I said I personally use a 4.7K res and a 12V zener to make sure that it's above the 10V full saturation​ level and not to high as to shorten the FET life. And about the precharge circuit, it's completely unnecessary in this use case so you'll be fine with out it.

Alright I hope that address everything and if you have any more questions or whatever just through them my way, love helping people out! P.S. please forgive any spelling or grammatical errors I wrote this while walking lol.
```

---
## \#9 Posted by: Russell23 Posted at: 2017-06-13T22:34:49.857Z Reads: 91

```
That circuit is just a quick doddle and I'm gonna make a better one . so I'll just use 2 10k resistors then instead of using 2 15k resistors @JdogAwesome
```

---
## \#10 Posted by: Russell23 Posted at: 2017-06-14T00:37:35.003Z Reads: 92

```
<img src="/uploads/db1493/original/3X/d/d/dd7e93974226580314ee1b22141bb286e2a97df5.jpg" width="281" height="500">
```

---
## \#11 Posted by: goldenHusky Posted at: 2017-06-14T06:21:35.416Z Reads: 77

```
@Russell23 just use the circuit diagram of @JdogAwesome  in the first post of his topic you linked.
```

---
