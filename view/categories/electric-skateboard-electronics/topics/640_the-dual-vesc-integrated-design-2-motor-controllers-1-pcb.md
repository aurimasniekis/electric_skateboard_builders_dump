# THE DUAL VESC &#124; Integrated Design - 2 Motor Controllers 1 PCB

### Replies: 22 Views: 5844

## \#1 Posted by: jacobbloy Posted at: 2015-12-03T06:48:57.363Z Reads: 448

```
 Introducing the dual VESC made for simplicity.
This is a twin ESC designed and based off of the VESC 4.10.
Benefit:
compact design when compared to wiring 2 vesc to gether
Less soldering and wiring
Batteries input is shared between both ESC
Capacitors are pcb mountable at 45 or 90deg
Both ESC connected via can bus
1 USB input
Built in nrf24l01 footprint ready for nunchuk control
Reduced componants by
Both ESC share 3v and 5v power rail 
Both share the 1 set of LEDs
And again 1 USB and reduces the need for installing jst plugs meaning a small componant reduction.

Foreseen problems:
3v and 5v Power rails not supplying enough amp
Batterie input traces not handling required current
Added cost of 6 layer pcb
(Please add more)

Ways we have tried to fix:
Made pcb 6 layer to allow 3layer thick power traces

Thread started for all positive and negative feed back please!

<img src="/uploads/db1493/original/2X/a/acb303d11c0c6cdaa6011cf16ab839c5792c8769.png" width="281" height="499"><img src="/uploads/db1493/original/2X/f/f30370289ee2ff91e1d0e9b5ed5b2d1d180cf18d.png" width="690" height="387">
```

---
## \#2 Posted by: onloop Posted at: 2015-12-03T07:07:47.168Z Reads: 411

```
FUCKING GAME CHANGER!!!... can't wait to get my hands on this little biatch!
```

---
## \#3 Posted by: akira Posted at: 2015-12-03T08:27:30.197Z Reads: 405

```
Very nice !!
Are you already testing one ?
```

---
## \#4 Posted by: Wanderer Posted at: 2015-12-03T08:35:40.333Z Reads: 392

```
This is the last piece of the puzzle for all wheel drive on my beast!
Hurry up and finish so I can give you my money!!
```

---
## \#5 Posted by: lowGuido Posted at: 2015-12-03T09:06:11.665Z Reads: 358

```
thats nice. a move in the right direction. I like that the power tabs are on the edge of the board now. thats heaps better.
```

---
## \#6 Posted by: onloop Posted at: 2015-12-03T10:18:26.458Z Reads: 350

```
In 7 days will have the first one & can start testing to ensure its functioning as expected.
```

---
## \#7 Posted by: trbt555 Posted at: 2015-12-03T10:45:57.733Z Reads: 343

```
Nice !
This can't be coincidence after @chaka mentioned a compact dual VESC in another thread ;-)

A dual VESC will need to be cheaper than two single ones for this to work.
Quality control and testing will also become more important because failure of one side will render the whole board practically useless.

I don't know if this is feasible electronically but ideally you'd have one MCU controlling 2 independent sets of power MOSFETS. **EDIT - strike that, it won't work.**
```

---
## \#8 Posted by: Blasto Posted at: 2015-12-03T19:04:52.612Z Reads: 325

```
Very nice work guys,

Here are my observations:

-5V rail, use both buck converters connected together with 2 diodes, small voltage drop but worth it if the the extra power is needed
-keep the led independent, very useful to know which DRV is sending the error code
-line up all of the fets bodies, to be able to stick a nice long heatsink on there, include heatink mounting holes?
-the power input tabs stick out like a sore thumb, directly put a XT60 connector footprint?

How will the USB detect both mcu, or is it just detecting one mcu and the second one is directly programmed by CAN? The issue I foresee is that we cannot control each motor independently... which is very handy in robotics, but maybe your not aiming for this market. Add some 0 ohm resistors on the CAN bus, because i am assuming they are connected together, add the second usb footprint as a place holder (vertical mount?)?

-inquire for 3-4oz copper on outter layers, can be less expensive than adding internal layers

-add some via stitching on the power track if you thing your tracks are to small, but i think your power tracks are superimposed, if it is the case, adding a stitch can be tricky/

-add solder mask on the no longer needed legacy power landings, unless you add some solder to those tracks
```

---
## \#9 Posted by: onloop Posted at: 2015-12-03T21:54:30.195Z Reads: 297

```
[quote="trbt555, post:7, topic:640"]
A dual VESC will need to be cheaper than two single ones for this to work.
[/quote]

Ideally yes... but that's not as easy as you would think, at least not yet, I think one of the biggest cost increases was the 6 layer PCB. This is somewhat countered by not having a separate PCB for the Caps.

So in the end there is really no reduction in cost. Which is fine by me.

The most exciting thing is its simplicity, Less soldering! As a builder of complete electric skateboards, I know that time is money, this could save 30-40mins per build which I will gladly pay a few dollars for that.... For a one man band any time saving is extremely valuable.
```

---
## \#10 Posted by: cmatson Posted at: 2015-12-04T04:41:30.791Z Reads: 285

```
[quote="onloop, post:9, topic:640"]
So in the end there is really no reduction in cost. Which is fine by me.
[/quote]

but then besides soldering, what would be the advantage? if it died, you have two dead VESC's instead of one...

it seams like it it costs around the same as two VESC's, then there really isn't a reason to get it: but that's just my opinion :wink:
```

---
## \#11 Posted by: lowGuido Posted at: 2015-12-04T05:30:42.098Z Reads: 257

```
I just noticed that you ditched half the caps in this design. any reasons?
```

---
## \#12 Posted by: rutxbikecron Posted at: 2016-01-05T11:07:31.084Z Reads: 227

```
This is a super good PCB design it simplifies a lot of electronics.
```

---
## \#13 Posted by: mikehan Posted at: 2016-01-06T07:31:35.320Z Reads: 228

```
I am currently building a board
 I can wait to try this dual VESC
where can i get one?
```

---
## \#14 Posted by: lowGuido Posted at: 2016-01-06T08:42:28.707Z Reads: 224

```
Just buy two singles for now.
```

---
## \#15 Posted by: psychotiller Posted at: 2016-01-06T13:08:49.340Z Reads: 219

```
You can get a dual vesc right now from ollinboardcompany.com. pm chaka
```

---
## \#16 Posted by: longhairedboy Posted at: 2016-01-06T13:43:29.393Z Reads: 223

```
I have two dead dual ESCs on my bench right now. Both of them have one side that works. 

If one side of this fails, can i just cut it in half?
```

---
## \#17 Posted by: psychotiller Posted at: 2016-01-06T14:12:07.450Z Reads: 227

```
Unrepairable damage? When you update the duals are they plugged in as one?
```

---
## \#18 Posted by: longhairedboy Posted at: 2016-01-06T14:53:30.078Z Reads: 255

```
They're the old Flier style ones from Enertion's late 2013 collection. I saved them so that one day i could maybe start replacing parts on them, but i haven't yet. They're monsters when they perform correctly.  

But right now they're dead and that's leaving a nasty taste in my mouth where integrated dual ESCs are concerned.
```

---
## \#19 Posted by: chaka Posted at: 2016-01-06T15:23:36.644Z Reads: 273

```
Building on the original PCB design is still the most compact for a dual VESC. It needs to be fitted with vertical usb ports to make it work but only measures 80mm wide. 

Here is a photo of a quad VESC with an extended base for mounting purposes. You would want the capacitor boards in their usual configuration on a dual VESC but it gives you a good idea of what you would see on a custom dual VESC.

<img src="/uploads/db1493/original/2X/1/1b864e954198b58262321fda59ec27631e8398f3.jpg" width="641" height="500">
```

---
## \#20 Posted by: Money Posted at: 2017-01-17T23:47:04.708Z Reads: 127

```
<img src="/uploads/db1493/original/3X/3/c/3c9370e2707786ba1bc00085102da802c2a1a9af.JPG" width="690" height="345">

Can someone please confirm if this is a VESC board or not? I was told it is, but i havent seen anything else like it online.

Thank you very much

Edit: sorry, i didnt realize this thread was a year old. On my phone it just said Jan 16, and not the year.
```

---
## \#21 Posted by: Pantologist Posted at: 2017-01-17T23:52:00.589Z Reads: 125

```
Doesn't look like a vesc. Different mosfets and no drvs.
```

---
## \#22 Posted by: Money Posted at: 2017-01-17T23:53:41.282Z Reads: 122

```
Thank you. I appreciate your input. Thanks a lot! I didnt think it was either.
```

---
