# \[SOLVED\] GT2B ChoZen Remote Battery Meter Gauge

### Replies: 15 Views: 1215

## \#1 Posted by: Mikenopolis Posted at: 2017-11-28T04:44:50.475Z Reads: 219

```
[SOLVED] ignore the picture on this post and ignore the diagram drawn on that printout. Solution is to leave the battery as is. You only need to solder two wires in total from the battery meter to controller PCB as seen on the last picture I posted a few posts below. Use a bit more wire than I did as you need room to move the meter to align with the hole you make, align it then use hot glue to keep it in place. Apply electrical tape between the two boards to prevent short, then put everything back together. This [battery gauge was found on eBay](https://www.ebay.com/sch/sis.html?_itemId=null&_nkw=1S+Single+Cell+Lipo+Battery+Voltage+Status+LED+Indicator+Gauge+Module) for like $7 shipped 



................................................................................................
So I'm trying to add a battery indicator on my GT2B mod. Got the idea from @FLATLINEcustoms' remote. After I solder what I think was correct the meter's LEDs turned on but it's always on. Does anyone know what I did wrong here?

<img src="/uploads/db1493/original/3X/d/6/d6b133fc4b74f79a7baa9851578a16e5bce196a3.jpeg" width="666" height="500">
```

---
## \#2 Posted by: Titoxd10001 Posted at: 2017-11-28T04:52:39.463Z Reads: 197

```
Think it draws so little power it's meant to stay on. Haven't done the meter mod myself
```

---
## \#3 Posted by: lrdesigns Posted at: 2017-11-28T04:55:02.297Z Reads: 190

```
I think you need to tap the battery power, after the power switch, not directly from the battery. Or the minus to the battery and positive after the power switch.
```

---
## \#4 Posted by: ShutterShock Posted at: 2017-11-28T04:56:50.667Z Reads: 182

```
That seems like it would be right.  I should do this mod to my gt2b, looks pretty cool.
```

---
## \#5 Posted by: Mikenopolis Posted at: 2017-11-28T05:36:38.868Z Reads: 169

```
I'm following the image that was provided and posted by flatland as well....I'm not fully understanding the pcb's two sets of + & - contacts I guess
```

---
## \#6 Posted by: wafflejock Posted at: 2017-11-28T05:41:23.292Z Reads: 163

```
Looks like just two outputs and two gnd in case you need them can check for continuity on those holes without any power running into the board.  Also like @lrdesigns said just need to put the switch on one of the battery leads between the battery and the meter so you cut off power to the meter itself along with the power it passes through.

Can see the traces from VCC just run around the edge of the board and gnd is hooked right to the battery gnd in the traces.  Looks like the chip controls the gnd opening/closing for the LEDs to turn on based on the voltage it's reading.
```

---
## \#7 Posted by: jmasta Posted at: 2017-11-28T06:00:24.519Z Reads: 155

```
[quote="Titoxd10001, post:2, topic:39502, full:true"]
Think it draws so little power it's meant to stay on. Haven't done the meter mod myself
[/quote]

This is what I remember as well. Flatlinecustoms has his on all the time

If you look through that thread someone figured out how to make the power meter switch on/off with the controller.  There was also something about replacing a resistor to make the LED brighter (which in turn draws more current, making the switch more necessary)
```

---
## \#8 Posted by: Mikenopolis Posted at: 2017-11-28T06:04:17.904Z Reads: 144

```
Interesting. I was thinking about adding another switch to turn the meter itself on and off. Which means I would have flick TWO BUTTONS to turn on the remote 🤔
```

---
## \#9 Posted by: jmasta Posted at: 2017-11-28T06:07:59.419Z Reads: 152

```
You just need to solder on the LED positive wire to the 5V switched source on the back of the PCB, if I remember correctly.  You could find it with a multimeter.  Or go searching through that thread. Someone posted a picture of which solder point you need
```

---
## \#10 Posted by: Mikenopolis Posted at: 2017-11-28T06:41:54.097Z Reads: 155

```
Thanks @jmasta. Figured it out. This is the solution. The meter remains off when remote is off and turns on along with remote. <img src="/uploads/db1493/original/3X/4/2/42a918df480a705b7af6fdcbe5ff78465f6bf43b.jpeg" width="666" height="500">
<img src="/uploads/db1493/original/3X/3/1/31b57b3b0278366f4f45c1d8c524a8f94709702d.jpg" width="375" height="500">
```

---
## \#11 Posted by: FLATLINEcustoms Posted at: 2017-11-28T12:29:54.605Z Reads: 136

```
They use such little power they stay on. Someone did the math and it was a long long long time to drain the battery. I wire mine straight to the battery. Very convenient to look at the remote and see how much power it has. 

Joel
```

---
## \#12 Posted by: clistpdx Posted at: 2018-05-05T17:49:42.506Z Reads: 98

```
I'm looking to buy this cheap battery meter guage on ebay. Does anyone know if the correct one is "1S" or "1S, 2S, 3S"?
https://www.ebay.com/sch/sis.html?_itemId=null&_nkw=1S+Single+Cell+Lipo+Battery+Voltage+Status+LED+Indicator+Gauge+Module
```

---
## \#13 Posted by: Mikenopolis Posted at: 2018-05-05T18:55:22.726Z Reads: 95

```
1s is the one I used
```

---
## \#14 Posted by: Battosaii Posted at: 2018-05-05T18:56:47.066Z Reads: 90

```
Is there enough space to add this to a winning version 2 or a Nano x remote?
```

---
## \#15 Posted by: Mikenopolis Posted at: 2018-05-06T02:00:54.329Z Reads: 76

```
I don’t know. The winning most likely not. But I think the nano-x might have enough surface area. Just have to figure out if there’s enough space to add the thickness. This thing is a pain to take apart and put back together so I can’t check
```

---
