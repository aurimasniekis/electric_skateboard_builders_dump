# Torqueboards 6355 sensored + VESC

### Replies: 21 Views: 3589

## \#1 Posted by: Lizardking0069 Posted at: 2016-08-10T01:27:40.084Z Reads: 357

```
Where does the sensored cable plug into the VESC? Or do I need to solder it on?
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-10T02:02:46.668Z Reads: 354

```
hall sensor port. looking at it straight on with the mosfets facing up, it's on the lower left.
```

---
## \#3 Posted by: Bender Posted at: 2016-08-10T02:10:25.352Z Reads: 352

```
http://vedder.se/wp-content/uploads/2015/01/PCB_Front.png
```

---
## \#4 Posted by: Sboard342 Posted at: 2016-08-10T03:10:39.337Z Reads: 335

```
Do you need to plug the motor wires in a specific order if you use hall sensor? Or does VESC auto detect?
```

---
## \#5 Posted by: Jinra Posted at: 2016-08-10T05:06:43.761Z Reads: 309

```
5v and GND (red and black) cables are important so make sure you dont plug them in wrong. Then there's the temperature cable if applicable, and the 3 hall sensor cables. Order of the hall cables doesn't matter as you set that up in the vesc during detection.
```

---
## \#6 Posted by: Titoxd10001 Posted at: 2016-08-10T06:39:05.635Z Reads: 299

```
@Sboard342 motor wires need to match up correctly only way I know is trying each combo till one works. I didn't see any difference using a hall sensor tbh and I'm over 200lbs. The only time I noticed is when I hit a bump and it hit my motor mount and that shock messed up my sensor somehow and I had to push home because my board wouldn't move from a standstill. Later I realized I could push and then throttle when the hall sensor is bad. I have two sensored motors that I won't be using the sensor because it's just a liability that has little benefit with a vesc.
```

---
## \#7 Posted by: Lizardking0069 Posted at: 2016-08-10T14:45:43.586Z Reads: 281

```
Thanks for the picture @Bender. I'll plug that in tonight after work. I was able to get the motor running on sensorless BDLC and got some slight cogging at start. Hopefully this eliminates cogging altogether.

I also need some heatsinks on this thing. Anyone know of cheap alternative heatsinks. I was about to get chakas but at $15 a pop (x3 Vescs) its expensive for a hunk of aluminum.
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-10T14:56:09.572Z Reads: 269

```
http://m.ebay.com/itm/141865269904
```

---
## \#9 Posted by: Lizardking0069 Posted at: 2016-08-10T15:06:04.471Z Reads: 263

```
Thanks @Jinra !
```

---
## \#10 Posted by: Lizardking0069 Posted at: 2016-08-10T15:07:15.637Z Reads: 260

```
Anyone know if FOC utilizes the hall sensors? I might experiment with FOC to see how it feels.
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-10T15:26:09.727Z Reads: 257

```
you can use foc with sensors, careful not to burn up the drv

https://youtu.be/bYYNbxPXNEU
```

---
## \#12 Posted by: Lizardking0069 Posted at: 2016-08-10T23:30:03.953Z Reads: 246

```
The auto-detect feature should be used with the pulley and gear installed?
```

---
## \#13 Posted by: Lizardking0069 Posted at: 2016-08-10T23:47:30.739Z Reads: 238

```
The torqueboards 6355 sensor cable does not fit the torqueboards VESC. I may have to solder it on.

<img src="/uploads/db1493/original/2X/1/19d99a6880755cb4f3161fecb60bc0307e5686c6.jpeg" width="666" height="500">
```

---
## \#14 Posted by: sl33py Posted at: 2016-08-10T23:53:57.313Z Reads: 232

```
In Vedder's video above he mentions this - you can swap wire for wire to the larger plug and it should work (so he says).  I believe DIYes also has an adapter cable to do this.

GL!
```

---
## \#15 Posted by: Jinra Posted at: 2016-08-11T00:04:49.586Z Reads: 231

```
This will fit.

http://www.ebay.com/itm/JST-2-0mm-PH-6-Pin-Connector-with-Wire-X-10-Sets-TW-/141757606740?hash=item2101696b54:g:W9EAAOSwgQ9V3m4W
```

---
## \#16 Posted by: Lizardking0069 Posted at: 2016-08-11T00:08:39.690Z Reads: 230

```
Thanks for the link.  I will check if there is a supplier closer in the US.
```

---
## \#17 Posted by: Jinra Posted at: 2016-08-11T00:09:56.994Z Reads: 229

```
I have 5pin JST-PH cables from the same seller if you want it. You'll just have to not use the temperature wire. They work prefectly in my build
http://www.electric-skateboard.builders/uploads/db1493/original/2X/6/61f1ed89f798b352ad6f17341c0040527e37c30b.jpg
```

---
## \#18 Posted by: Mrmoonlight Posted at: 2016-08-11T00:18:25.411Z Reads: 223

```
I just hooked up these two heatsinks. 
http://www.ebay.com/itm/381103432358?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

Need some thermal paste too. You can go with the standard stuff or the adhesive kind.
```

---
## \#19 Posted by: Lizardking0069 Posted at: 2016-08-11T01:10:31.439Z Reads: 215

```
Thanks Jinra!! PM sent 🙂
```

---
## \#20 Posted by: paulus_germanus Posted at: 2017-04-25T10:49:53.271Z Reads: 145

```
What AWG are those wires, Jinra? Thx :)
```

---
## \#21 Posted by: Jinra Posted at: 2017-04-25T14:34:07.863Z Reads: 133

```
about 18 or 20
```

---
