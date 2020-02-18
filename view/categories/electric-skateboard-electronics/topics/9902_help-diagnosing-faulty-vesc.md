# Help diagnosing faulty VESC

### Replies: 29 Views: 2144

## \#1 Posted by: AutoHax0r Posted at: 2016-09-20T20:00:48.777Z Reads: 133

```
Right. Basically, a couple of months ago I received a faulty VESC. To summarize, I was never able to make this thing respond to anything - not even light up. My experience with it ended when the capacitors discharged in an explosive manner. 

Basically, after balance charging my batteries, I attempted to connect to it (w/ antispark connectors) and everything went wrong.

I followed the manual exactly. Shortly after connecting (2-3 seconds) my 8S Li-Po, the VESC got extremely hot and the capacitors on the VESC exploded and flames/smoke exited through the end of the capacitor. The VESC got covered in some form of liquid (probably from the capacitors) and was very warm. The connector and heat shrink also shows this.

Now I'm looking to see if I can get this thing back in shape. Here is a photo. <img src="/uploads/db1493/original/3X/d/1/d125cefeff21d70382610e5c7bdc672f54ca2714.JPG" width="690" height="459">

I took the old broken capacitors of. I'm not sure if the actual VESC-body in functional. I'm under the impression that the capacitors were incorrectly soldered. 

Here is a photo I took while it was in the heatshrink. <img src="/uploads/db1493/original/3X/6/0/60aea4eb305135e916746bf828cc6c2a0fbd4d69.jpg" width="690" height="459">

My question is: Does it appear damaged? Can I test it on PC without capacitors? Any idea on what went wrong?
```

---
## \#2 Posted by: ITman496 Posted at: 2016-09-20T20:05:35.522Z Reads: 125

```
Not very experienced with the VESC but I definitely do not recommend testing without any capacitors.  Any kind of tiny spike on the input could kill the unit.  The caps are there to absorb that.  Do you know why the caps exploded?  It sounds like either they were mounted backwards, or power was fed in backwards.  Both are not a good thing.  Did it smoke anywhere else on it, or only the capacitors?
```

---
## \#3 Posted by: flatsp0t Posted at: 2016-09-20T20:09:52.784Z Reads: 125

```
Can you see any burnt traces on the pcb?
If not, check for solder joints on the legs of the chips., 
if everything seem ok, try connecting a regulated 12v lab powersupply.
do you know if it had the firmware and bootloader flashed already?
If not, you may need an stlink programmer and a VM or a PC with linux
```

---
## \#4 Posted by: AutoHax0r Posted at: 2016-09-20T20:10:20.649Z Reads: 126

```
I'm thinking the polarity was inverted on the capacitors. It certainly looks like it from the wiring diagram. Only the capacitors smoked. 

I have a couple of photos more. 

Right after the ''explosion''. <img src="/uploads/db1493/original/3X/d/7/d779e2a5c5fe6163cc0d6b43b03ae0a04835cca4.jpg" width="690" height="459">



Recent photos. 

<img src="/uploads/db1493/original/3X/6/e/6ee650c0bba376946c0bef22333d959cf8b5c27c.JPG" width="690" height="459"><img src="/uploads/db1493/original/3X/6/8/6809f3d0217f528b4e5923a72a7c3b1a224d65b3.JPG" width="690" height="459">
```

---
## \#5 Posted by: ITman496 Posted at: 2016-09-20T20:12:36.174Z Reads: 118

```
If the caps were inverted then its possible that it could be okay.  I too am dealing with a lifeless enertion VESC that appears to have no bootloader or firmware.  Sigh.  I say put some kind of cap on it for safety and then hook it to a lab supply with current limiting so it doesn't explode again, and see if it lights up.  You should apparently get a blue light and then some kind of flashing red light that turns green.  I'm not getting the second part of that, only blue, signifying that the power is working but nothing else.  If you get neither then there are bigger issues at hand.
```

---
## \#6 Posted by: AutoHax0r Posted at: 2016-09-20T20:14:53.210Z Reads: 115

```
Ah, super annoying dealing with problems. Best of luck to you. Maybe someone with the required technical skills will add their input on here.
```

---
## \#7 Posted by: AutoHax0r Posted at: 2016-09-20T20:17:29.124Z Reads: 116

```
Yes. It did come pre-installed. 

The only burnt parts are around the soldering joints. What do you think about powering it without capacitors?
```

---
## \#8 Posted by: ITman496 Posted at: 2016-09-20T20:18:16.041Z Reads: 116

```
I'd love to post my problems but because I just joined, I can't appear to make a topic yet.  Maybe talking with you here will help push me to the 'tier' that lets me post topics.  

For you, as far as my understanding goes the blue light signifies that the power rail to the microcontroller is alive and well.  Then another light means it is scanning for errors, and it blinks red.  If it keeps blinking red, you have errors, probably with the mosfet driver chip (it seems finicky from what I've been reading and the most likely thing to cause a failure) and if all is well, that red flashing light becomes green and you are good to go. Do you have a bench power supply you can limit to an amp or so to avoid any horrible fires if something is shorted?
```

---
## \#9 Posted by: flatsp0t Posted at: 2016-09-20T20:24:30.468Z Reads: 110

```
If you have access to a lab supply with current regulation/limiting, it should be no problem.
```

---
## \#10 Posted by: AutoHax0r Posted at: 2016-09-20T20:24:45.981Z Reads: 109

```
Sure. I've got a power supply, just hesitant to do anything without recognition from the specialists on here ;).
```

---
## \#11 Posted by: flatsp0t Posted at: 2016-09-20T20:26:03.771Z Reads: 106

```
Then you have to ask @chaka to chime in.
I know it never hurt mine, but just to be sure...
```

---
## \#12 Posted by: ITman496 Posted at: 2016-09-20T20:26:12.764Z Reads: 106

```
Not a bad idea to wait for others input, from my point of view if you don't see anything obviously burned, you have a lab supply, and can find a small cap to tack on there, I'd go for it and see what happens.
```

---
## \#13 Posted by: AutoHax0r Posted at: 2016-09-20T20:35:55.770Z Reads: 102

```
Will have to order the capacitors. The old ones are most definitely dead ;)
```

---
## \#14 Posted by: lowGuido Posted at: 2016-09-20T20:36:54.054Z Reads: 100

```
those caps look like they were in the right way to me.
however it is hard to tell from your photos..
there is no problem using a lab supply to boot up VESC and check BLDC tool without caps.
you only really need them when running a motor.
```

---
## \#15 Posted by: JTAG Posted at: 2016-09-20T22:11:59.695Z Reads: 87

```
Caps only explode on overvoltage or wrong polarity. 

If caps explode but no further sparks / flames on VESC the VESC is most likely still OK. As suggested connect the VESC to either a lab power supply or a 12 isch wall brick and check for LED lighting up. Please try this and reply your findings ^^.
```

---
## \#16 Posted by: zmoney Posted at: 2016-09-21T02:51:33.130Z Reads: 79

```
[quote="JTAG, post:15, topic:9902"]
Caps only explode on overvoltage or wrong polarity.
[/quote]

By looking by the pictures, the polarity on the caps seems to be fine. I'm betting that the caps exloded because of an over-voltage.
```

---
## \#17 Posted by: AutoHax0r Posted at: 2016-09-21T05:52:50.408Z Reads: 72

```
I think the color of the cables were switched, but that obviously doesn't affect anything. I mainly assumed something was up with the capacitors, since they were the only things affected. 

Over-voltage is possible, but I tested with 8s so I think that that is very unlikely.
```

---
## \#18 Posted by: trbt555 Posted at: 2016-09-21T08:35:37.420Z Reads: 68

```
The color of the wires being switched looks fishy to me.
Did you check that the + coming from the battery connector is soldered to the + terminal on the capacitor board ?
```

---
## \#19 Posted by: AutoHax0r Posted at: 2016-09-21T09:28:50.550Z Reads: 72

```
I agree. The wires that go to the LiPo from the capacitor board seem displaced. Black wire goes from +, and red goes from -. But would that interfere?
```

---
## \#20 Posted by: DeathCookies Posted at: 2016-09-21T09:40:33.557Z Reads: 70

```
[quote="trbt555, post:18, topic:9902, full:true"]
The color of the wires being switched looks fishy to me.Did you check that the + coming from the battery connector is soldered to the + terminal on the capacitor board ?
[/quote]

If the cables on the VESC are not switched then everything is alright:
<img src="/uploads/db1493/original/3X/8/5/856041c999f74224b5e8a38002191d106a147a81.jpg" width="442" height="500">
```

---
## \#21 Posted by: JTAG Posted at: 2016-09-21T14:33:51.067Z Reads: 65

```
I checked the design, the capacitors where soldered the right way as well. If I look carefully the caps seems rated at 63V, also OK.

But as you can see here:
http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/6/e/6ee650c0bba376946c0bef22333d959cf8b5c27c_1_690x459.JPG

http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/6/8/6809f3d0217f528b4e5923a72a7c3b1a224d65b3_1_690x459.JPG

The input terminals where swapped (or did I overlook something?).
```

---
## \#22 Posted by: DeathCookies Posted at: 2016-09-21T14:41:45.635Z Reads: 63

```
First picture of your post:
Is the polarity of the capacitor bank alright? I cannot see it like in the second picture
```

---
## \#23 Posted by: trbt555 Posted at: 2016-09-21T16:33:05.837Z Reads: 65

```
This ain't rocket science.
Red goes to (+) and black goes to (-)

The polarity of the wires from the caps to the VESC is OK. The battery wires to the caps look inverted.

Don't hook up the caps and connect the lipo straight to the VESC. As long as you don't run a load, you don't need the caps.
If you don't get a LED to light up, it's fried and you'll have other things to worry about than the caps.
```

---
## \#24 Posted by: AutoHax0r Posted at: 2016-09-21T18:47:52.473Z Reads: 60

```
Just hooked it up my power supply. It lit blue - which is quite nice, as that is the most alive this thing has ever been. So, hook up new caps and get this running? 

Btw, can I hook it up to the PC to check with BLDC without caps and power (only power from USB)

:slight_smile:
```

---
## \#25 Posted by: chinzw Posted at: 2016-09-21T18:50:20.100Z Reads: 59

```
Yes. The caps are there to pevent voltage fluctuations, your power supply should be providing clean voltage.
```

---
## \#26 Posted by: trbt555 Posted at: 2016-09-21T19:33:14.750Z Reads: 59

```
You can't power it from USB, you need an external supply. 
Just use the lipo.
```

---
## \#27 Posted by: zmoney Posted at: 2016-09-22T00:46:21.264Z Reads: 57

```
You can use a lipo, but you should use a lab power supply just to be super careful. Not 100% necessary though.
```

---
## \#28 Posted by: AutoHax0r Posted at: 2016-10-11T14:58:01.334Z Reads: 44

```
UPDATE:

Still not sure what to do. Anybody knows if this thing will run if I try another pair of caps? Can caps be defective?

Thanks guys
```

---
## \#29 Posted by: chinzw Posted at: 2016-10-12T00:07:00.064Z Reads: 38

```
Caps usually bulge when fried. More uncommon but possible is that the caps fried and shorted with no visible evidence. If thats the case removing the caps would also remove the short.
```

---
