# I Need Help With My Wiring Diagram &#124; Dual Motor &#124; LiPo SERIES

### Replies: 26 Views: 4709

## \#1 Posted by: Raf Posted at: 2016-07-28T22:46:13.137Z Reads: 311

```
Hey, can you guys help me with my wiring diagram. I've made a start but have gotten stuck and don't want to be making the wrong diagram.

Heres what i got so far...

<img src="/uploads/db1493/original/2X/c/cc0bd8d45ded18f2489fbc9dbbbc6885fb90c736.png" width="690" height="255">


Could you also let me know what i am missing from this?

Thanks
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-07-28T23:03:29.377Z Reads: 310

```
http://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179?u=michaelinvegas
```

---
## \#3 Posted by: JLabs Posted at: 2016-07-28T23:03:35.987Z Reads: 288

```
Are you just curious on how to wire the antispark switch to the VESC's? Everything looks good so far, I am not an expert with the VESC so someone would have to confirm the canbus connection.
```

---
## \#4 Posted by: Jinra Posted at: 2016-07-28T23:05:05.192Z Reads: 279

```
You dont plug both VESCs into the receiver unless your doing a split servo kind of setup. Since he's using the CAN bus he only needs to plug the receiver into 1 (master) VESC.
```

---
## \#5 Posted by: Raf Posted at: 2016-07-28T23:11:54.292Z Reads: 269

```
just curious on how to wire both vescs to the battery source with the watt meter and anti spark switch
```

---
## \#6 Posted by: JLabs Posted at: 2016-07-28T23:20:01.493Z Reads: 258

```
<img src="/uploads/db1493/original/2X/5/5d3e733f51fa1a34d46e7cb3e3411f4e1147d259.PNG" width="690" height="256">

You take the wires from the switch and wire them to an xt60 connector that goes splits to 2 xt60 connectors, I did my best to draw it here (quick)
```

---
## \#7 Posted by: Raf Posted at: 2016-07-28T23:22:38.817Z Reads: 238

```
can i use xt90 connectors?
```

---
## \#8 Posted by: JLabs Posted at: 2016-07-28T23:46:55.741Z Reads: 229

```
Yes, dosnt matter
```

---
## \#9 Posted by: Raf Posted at: 2016-07-29T00:14:25.490Z Reads: 220

```
how do split the wires so that they go to the vesc and watt meter? (sorry for the noob question)

<img src="/uploads/db1493/original/2X/f/f0362c682081a7270def0459fdad6f160fea67ca.png" width="164" height="129">
```

---
## \#10 Posted by: Jinra Posted at: 2016-07-29T00:22:05.069Z Reads: 208

```
cut away some of the silicone insulation and solder on the wires, make sure to reinsulate.
```

---
## \#11 Posted by: JLabs Posted at: 2016-07-29T00:35:15.776Z Reads: 208

```
Yes exactly what @Jinra said
```

---
## \#12 Posted by: Raf Posted at: 2016-07-29T00:47:08.485Z Reads: 207

```
To wire the two vescs I can use a "xt90 y harness" right?

http://www.hobbyking.com/mobile/viewproduct.asp?idproduct=25662
```

---
## \#13 Posted by: JLabs Posted at: 2016-07-29T00:59:27.952Z Reads: 204

```
Yes would work perfectly
```

---
## \#14 Posted by: Raf Posted at: 2016-07-29T13:46:58.645Z Reads: 196

```
@Jinra 

Okay so i have updated the diagram. After doing some further research i noticed another style of wiring. Could you please let me know which one is correct?


Verseion 1
<img src="/uploads/db1493/original/2X/5/5754dac14a2d1502a34f77b1b32f811b9f9567ed.png" width="690" height="388">

Version 2
<img src="/uploads/db1493/original/2X/5/5ab7a4cce39ee31e7f9146ca8a0b373a4efcfc54.png" width="690" height="387">
```

---
## \#15 Posted by: Jinra Posted at: 2016-07-29T13:58:33.175Z Reads: 181

```
Depends what type of switch/anti spark you have. If you have a xt90 anti spark plug from hobby King then the second diagram is what you want. If you have something like a vedders anti spark switch or torqueboards switch, the first diagram is for that.

Also you probably don't need the LED since the watt meter will turn on when the board is on anyway
```

---
## \#16 Posted by: JLabs Posted at: 2016-07-29T14:00:33.765Z Reads: 174

```
You are going to want version 1
```

---
## \#17 Posted by: Raf Posted at: 2016-07-29T14:01:01.896Z Reads: 175

```
okay thanks, I am planning on using vedders antis spark. And as for the watt meter i think i am just going to use it to configure the settings so i can decide the max/min watt/amp/volt output and once i have it all figured out i will probably take it out
```

---
## \#18 Posted by: Raf Posted at: 2016-07-29T14:04:26.593Z Reads: 171

```
another question i have is how do i wire the meter. It has two wires coming out of each side (2 red 2 black). Do i just wire on red and one black from one side and the leave the other two?

https://www.amazon.co.uk/Vollter-Analyzer-Display-Precision-Electronics/dp/B01853CJAW/ref=sr_1_1?s=kids&ie=UTF8&qid=1469195183&sr=1-1&keywords=Wattmeter+130A
```

---
## \#19 Posted by: Jinra Posted at: 2016-07-29T14:06:24.534Z Reads: 163

```
That's an inline watt meter. You basically snip the red and black wires on your diagram and throw the meter in between, similarly to your vedder switch.
```

---
## \#20 Posted by: Raf Posted at: 2016-07-29T14:12:56.359Z Reads: 163

```
so like this....

<img src="/uploads/db1493/original/2X/f/fbd686b3fda3ef58ba515fe50d233012fe108596.png" width="690" height="298">
```

---
## \#21 Posted by: Jinra Posted at: 2016-07-29T14:13:22.146Z Reads: 162

```
yep yep

 10 chars
```

---
## \#22 Posted by: PDXroses Posted at: 2017-04-28T23:58:44.724Z Reads: 114

```
I'm pretty new at this so excuse the simple question. To reduce bulk, I'd like to eliminate the two XT90's that go into each VESC and replace it by soldering the wires. Is that a safe option?  Thanks!
```

---
## \#23 Posted by: mmaner Posted at: 2017-04-29T01:32:14.712Z Reads: 111

```
The main reason to leave the XT-90s is for quick connect/disconnect. There's no reason why you couldn't or shouldn't solder it directly.
```

---
## \#24 Posted by: Busk8 Posted at: 2018-03-23T14:38:17.712Z Reads: 66

```
did it work?
```

---
## \#25 Posted by: PDXroses Posted at: 2018-03-23T21:53:16.609Z Reads: 63

```
It worked wonderfully until I needed to unplug the motor. Then it was a nuisance. But seriously, how often would you need to do that anyway?
```

---
## \#26 Posted by: OBone Posted at: 2019-04-18T03:40:32.522Z Reads: 12

```
Hi all. Noob question again. 

Please explain more about the receiver? I understand the concept of using a master VESC and slave VESC. But how do you connect the two exactly? Isn't CANbus something in a car? 

Thanks
```

---
