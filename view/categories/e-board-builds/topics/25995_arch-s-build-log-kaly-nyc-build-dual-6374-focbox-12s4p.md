# Arch_&rsquo;s build log &#124; kaly nyc build &#124; dual 6374 &#124; focbox &#124; 12s4p

### Replies: 14 Views: 3788

## \#1 Posted by: Blasto Posted at: 2017-06-23T14:50:14.522Z Reads: 504

```
This is @Arch build log, thought i'll document the process before the cold malted beverages takes over.

So let's start with the battery. The challenge here to make a battery pack that is as thin and flexible as possible.

This is the initial plan:
<img src="/uploads/db1493/original/3X/a/1/a11636ce50e364faae68be72fde5f8a992a02f8e.JPG" width="374" height="500"><img src="/uploads/db1493/original/3X/2/9/29a0b57652c7717d6ae72cd63a6033ea3870c887.JPG" width="374" height="500"><img src="/uploads/db1493/original/3X/d/6/d6c5ba7b46415b3be3c4090b0b9c11f3104c8cee.JPG" width="374" height="500"> 

so we'll be using a pcb over the top of each // pack, each // pack is spot welded together then soldered on to the pcb. Then each series connection is done from pcb to pcb. Then of course, the sensor wires are bussed down in a nice straigth line.

<img src="/uploads/db1493/original/3X/1/c/1c484aa65737f5a968b84377c11a9d0905aa2ad0.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/1/a/1abdd5e3a11ce88621ac1fe6a31866187b8666f8.JPG" width="374" height="500">
<img src="/uploads/db1493/original/3X/4/7/4728c9f2933f8d62a2261881dc8bdf19598e637f.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/d/7/d7dd057cfe3efca907ace4fd113d11233381c6a0.JPG" width="375" height="500">

Flexible flat 10awg wire was used to do all the series connections

<img src="/uploads/db1493/original/3X/4/a/4a6ddaf131444f70fa6b6fa5c392a68df852e51b.JPG" width="375" height="500">

And a ribon cable for the sense wires...

Result after 6hrs of labouring

<img src="/uploads/db1493/original/3X/9/7/976ba5fb6a93bff679e24141fb6423214f0c6dc8.JPG" width="375" height="500">

Flexible AF, clean straight lines, still need to get the senses to the bms, but thats another post.
```

---
## \#2 Posted by: Randyc1 Posted at: 2017-06-23T15:03:00.099Z Reads: 454

```
Cool Idea !!
```

---
## \#3 Posted by: rpn314 Posted at: 2017-06-23T23:32:02.679Z Reads: 436

```
I was wondering what this was when I saw it in the pictures thread. Looking forward to see this develop!
```

---
## \#4 Posted by: Sander Posted at: 2017-06-25T01:17:09.770Z Reads: 407

```
Cool, how much did the pcb cost and where did you order them?
```

---
## \#5 Posted by: Blasto Posted at: 2017-06-25T01:22:02.039Z Reads: 412

```
Pcbway.com

5$ for 10, did two designs, cell 1 to 6 and 7 to 12. So 10$ usd + 5$ shipping (normally its 25$)
```

---
## \#6 Posted by: Arch Posted at: 2017-06-26T16:22:27.638Z Reads: 391

```
Thanks @Blasto and @JohnnyMeduse. Great idea and sublime execution despite all the booze and 3am end time!
```

---
## \#7 Posted by: Blasto Posted at: 2017-06-28T06:07:20.567Z Reads: 375

```
Few updated pics, 98% done, 100% functional

Needs an opening for the usb, some conformal coating, a tie wrap or two and maybe some glorious hot glue.

<img src="/uploads/db1493/original/3X/e/8/e8ad0730cef1103c04c8e0cf1fab93402c81479f.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/f/9/f95555ab24d7446bdedbd1eac31c4bd3aed35410.JPG" width="666" height="500">
```

---
## \#8 Posted by: rene Posted at: 2017-11-15T10:08:33.777Z Reads: 300

```
WOW!  @Blasto and @Arch !

You guys realized an awesome savety feature to battery builds in general.
A'm blown away!

Now - I need to figure out a way how to materialize those PCBs...
```

---
## \#9 Posted by: deucesdown Posted at: 2018-03-03T18:09:48.904Z Reads: 239

```
@Blasto @Arch thank you guys. I keep coming back to this thread every few weeks, and although sparse on words, there's so much nuance and detail. I'm comparing to the other pcb designs, and this is what I'm picking up on this round of examination.

- actual 10awg flat braid wire, not grounding strips of whatever diameter that _should_ be 10awg equivalent
- The connection between cells and PCB _not_ nickel strip. It's 10awg flat braid, presumably soldered to the nickel on the cells. Because using 10awg instead of nickel for this connection, the fact that the high current contact does not extend to the 4th cell does not matter.
- but there is actually some soldering that heats up the cells. Unless the 10awg was soldered on before spot welding.
- there are 2 different pcbs! the difference is the silk screening, 1-6s and 7-12s.
- pcbway is actually really really cheap for this?

2 questions. :slight_smile:

Can you share the pcb files? It'd be nice to have the link in this thread. I understand if not. This would be a fun thing to learn anyway.

Do you remember what you used for the ribbon cable?
```

---
## \#10 Posted by: rene Posted at: 2018-03-04T07:35:34.876Z Reads: 219

```
https://www.electric-skateboard.builders/t/building-18650-battery-holder-connector-pcb/38651
```

---
## \#11 Posted by: Blasto Posted at: 2018-03-06T03:36:46.610Z Reads: 201

```
Hey thanks for your interest

[quote="deucesdown, post:9, topic:25995"]
The connection between cells and PCB not nickel strip. It’s 10awg flat braid, presumably soldered to the nickel on the cells. Because using 10awg instead of nickel for this connection, the fact that the high current contact does not extend to the 4th cell does not matter.
[/quote]

The cells were spot welded in groups of 4 with nickel strip, then glued on the pcb. used the 10AWG flat braid to bring the high current path on the PCB (soldered on the top of the nickel strip, I have a good iron, took less than a second of heat)

![image|246x187](upload://bMHyTHCRSdXR0iW1H01UbzPFqNn.jpg)

[quote="deucesdown, post:9, topic:25995"]
there are 2 different pcbs! the difference is the silk screening, 1-6s and 7-12s.
[/quote]

yes, 2 reasons, to make it look peeerdy and with pcbway, a single design under 10X10cm is 5$ for 10 pieces (20$ for 20 pieces) so i had to justify sending 2 "different" design so i would end up getting both for 10$ for 20 pieces

[quote="deucesdown, post:9, topic:25995"]
Can you share the pcb files?
[/quote]
TBH, i was not 100% satisfied with the design, too much track cutting and it was somewhat labour intensive. I would not feel comfortable with sharing a design that I am not ready to back up. 

Besides, there's a few guys that got inspired by this thread and that are selling their pcbs.

[quote="deucesdown, post:9, topic:25995"]
Do you remember what you used for the ribbon cable?
[/quote]

just some normal 100mil ribbon cable

[example of ribbon cable](https://www.digikey.ca/product-detail/en/molex-llc/0250010802/WM08-02A-ND/857950)
```

---
## \#12 Posted by: deucesdown Posted at: 2018-03-06T04:19:48.906Z Reads: 190

```
[quote="Blasto, post:11, topic:25995"]
TBH, i was not 100% satisfied with the design
[/quote]

Thanks for responding. There are a few outstanding forum members who really know their shit. And people who really know their shit are bothered by the little things, the subtleties, learned through years of agonizing over the details.

Okay enough fluffing. What didn't you like?

[quote="Blasto, post:11, topic:25995"]
too much track cutting
[/quote]

Sorry for being noob, this means cutting on the pcb with a knife? The photos look so good. What was it?

[quote="Blasto, post:11, topic:25995"]
10X10cm is 5$ for 10 pieces
[/quote]

This means 1 oz copper, right? Is it enough for 4 x 30q worth of current, potentially 80a? I know the wires are almost touching on the pad.
```

---
## \#13 Posted by: Blasto Posted at: 2018-03-06T04:43:11.238Z Reads: 184

```
[quote="deucesdown, post:12, topic:25995"]
Sorry for being noob, this means cutting on the pcb with a knife? The photos look so good. What was it?
[/quote]
![image|581x500](upload://2HKe14c4OiAdAxdSzogvhPOwN5h.png)

the "cell" selection is done by cutting the pcb track, i debated by doing this or using a zeros ohm resistor. turns out it was more a pita to cut the track i did not want than to use a zeros resistor. It's a very small cut, barely visible.

![image|257x500](upload://dPxepTbRDxK1KXqm2Dt0oCC1IdP.png)

[quote="deucesdown, post:12, topic:25995"]


This means 1 oz copper, right? Is it enough for 4 x 30q worth of current, potentially 80a? I know the wires are almost touching on the pad.
[/quote]

yeah 1oz is more than enough, by soldering the flat braid to the pcb and tinning, it's adding a lot of "weight" to the pcb. Also, the  flat braids is very close to each other, so the pcb is carrying the current for 1 or 2mm (engorged with solder)
```

---
## \#14 Posted by: Arch Posted at: 2018-03-13T21:13:36.262Z Reads: 170

```
Barely visible cut and a bitch to make! LOL
```

---
