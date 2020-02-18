# Arduino Spot Welder Went Boom

### Replies: 21 Views: 5891

## \#1 Posted by: Fiori Posted at: 2017-10-15T02:22:23.802Z Reads: 374

```
Got my arduino spot welder earlier this week(https://malectrics.eu/product/diy-arduino-battery-spot-welder-prebuilt-kit-v3/). It was working amazing for 100 welds. Then I heard a pop, and saw a flash from the arduino unit. Every time I would place the probes on the nickel strip(or anything that creates continuity) I would get smoke from the unit. 

I immediately disconnected everything. After some inspection I saw this small.... whatever it is on the bottom of the unit burnt. I think it's a diode, I am totally not sure. Was my 12v 100AH battery too much?

Can anyone smarter than me check out the diagram and let me know a suitable replacement for whatever it is I burned. Iv'e looked at the diagram(https://cdn.instructables.com/ORIG/FVN/JRZ1/J70QPQB7/FVNJRZ1J70QPQB7.pdf) but it's just not clear exactly what it is. I'm 99 percent sure its a diode just because of the placement and where it's located. 

Thanks fellers. <img src="/uploads/db1493/original/3X/3/e/3e2af7856cfc0993ddd8a4813e84c45be6e7c7b7.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/f/d/fd153309bc3a076c8aa0d1eee8672f4175107af1.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/6/6/66faaa18d9beb2446b905ae546b1383eb7624f48.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/c/2cf5e2cca73b6435a63dea06f84841c537270c96.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/9/9/999d5f287816199ff2901b28faf312da61d3c1ad.png" width="525" height="500">
```

---
## \#2 Posted by: Fiori Posted at: 2017-10-15T02:44:43.912Z Reads: 338

```
If i'm correct I think it's this one. Is there a stronger one I can buy? It says 400W so I am assuming my 100AH battery pushed it too hard?

http://www.mouser.com/Search/ProductDetail.aspx?R=SMAJ13A-13-Fvirtualkey62110000virtualkey621-SMAJ13A-13-F
```

---
## \#3 Posted by: akhlut Posted at: 2017-10-15T03:03:14.383Z Reads: 341

```
The bom is on github.

https://github.com/KaeptnBalu/Arduino_Spot_Welder_V3?files=1

It points to a through-hole part for that TVS diode. 
http://www.mouser.com/Search/m_ProductDetail.aspx?Vishay-Semiconductors%2f5KP13A-E3-54%2f&qs=sGAEpiMZZMvxHShE6Whpu%252b3Ok0iwlf4Bf801GuCO68c%3d

Check the instructable.  He made a change to replace the smd TVS diode.  http://www.instructables.com/id/DIY-Arduino-Battery-Spot-Welder/

Update 10.2017:
Although the SMD TVS diode has pretty much the same specs as the bigger 
through hole TVS Diode used on the previous Spot Welder versions it seems to struggle with very strong car batteries. There where some fails of the diode reported by users who used 800 CCA or stronger batteries. So i decided to replace the diode with the through hole version, which is a bit more robust.

The BOM was already updated with the new TVS diode.

Here is how to install it to the pcb:

Scratch of the solder stop paint from the ractangle part with the many holes on the pcb with a box knife and add some solder to the blank copper on the scratched area. We need this because the through hole TVS diode is a bit wider than the SMD version.

Bend the through hole TVS diodes legs 90 degrees as close as possible to the diode and cut them short so the diode can be mounted on the pcb. Then put some solder on the legs and solder the diode to the pcb. Solder the left side first. When the diode stays in place solder the right side (scratched pcb side). Make sure to use a powerful enough soldering iron so you dont heat the diode very long. It is necessary to solder the diode directly on the pcb without extension wires. This way it does the best job eliminating the high voltage spikes.
```

---
## \#4 Posted by: Fiori Posted at: 2017-10-15T03:13:26.061Z Reads: 293

```
Thank you I totally missed that update on the page. I ordered it on 9/30 so i must have literally just missed the cutoff for that update. That means it definitely was the larger battery that caused it.   I'll order it and solder it on.
```

---
## \#5 Posted by: Fiori Posted at: 2017-10-15T07:33:16.648Z Reads: 291

```
Got it working.  Ripped up an old power supply and stole the biggest diode I could find. 
<img src="/uploads/db1493/original/3X/3/6/36bf6d79727fb0647a2e6a95f5a5897c6e554796.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/f/0fc62a879be9f19d404266700f5197efe1867736.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/d/8/d81bf6963a633642df1c1ac91e1f70bd9daf31c5.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/9/b/9b515d5535e6f035f17b629be517aeef3e5c4a07.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/2/6/26f92289e177479269223905137e7329c947ffdd.jpg" width="666" height="500">
Working like a champ now. So much faster with probes. Now to cancel my diode order :stuck_out_tongue:
```

---
## \#6 Posted by: scepterr Posted at: 2017-10-15T07:35:37.738Z Reads: 267

```
Haha, nice. 
I would put a dab of hot glue or silicone under the diode, don't want any pixies jumping around 😉

What's the max thickness and material you've been able to weld with this ?
```

---
## \#7 Posted by: Fiori Posted at: 2017-10-15T07:52:09.290Z Reads: 258

```
I haven't tried anything above 0.15mm because its all I have. I sold my 0.20mm before i got this(adurrr). 

It does 0.15mm at 6ms with the battery I have been using. I would imagine it could go as thick as you would need. at least up to 0.30mm
```

---
## \#8 Posted by: scepterr Posted at: 2017-10-15T07:56:48.780Z Reads: 244

```
Sounds good, ordered 1 to play with 😁
Will be hooked up to 4S80P 18650 bank, can easily burst 200-300A
```

---
## \#9 Posted by: Fiori Posted at: 2017-10-15T08:02:07.428Z Reads: 245

```
it's going to pull 400A plus. Most places I read suggested not using 18650s.

Also: I would be lying if I said I wasn't having fun with it :stuck_out_tongue: you'll be glad you got it
```

---
## \#10 Posted by: scepterr Posted at: 2017-10-15T08:04:39.494Z Reads: 238

```
It can do more I'll just need to upgrade the connections/wiring. The cells themselves could do 320-400A cont, 800A burst in the bank I'm planning to use. They're all harvested power tool cells, not laptop cells.
```

---
## \#11 Posted by: Fiori Posted at: 2017-10-15T08:10:55.955Z Reads: 230

```
Sounds like a massive beast of a battery. The ease of use is much better than the sunkko. However the sunkko put out some decent welds too.

I'm wondering if the diode I used is going to cause some issues :/ I can't find any info on labeling of diodes. The one I used was similar size/look to the one on the BOM. All it says on it is 680. I am wondering if it's even a TVS diode or not?

It's been fine for the last 75 welds
```

---
## \#12 Posted by: scepterr Posted at: 2017-10-15T08:18:40.278Z Reads: 222

```
I already have the battery modules built just need to layer up and add a couple extra series links

I also got 2 bare PCBs ;)

The 788h is fine but not great for volume
```

---
## \#13 Posted by: scepterr Posted at: 2017-10-26T01:41:23.953Z Reads: 204

```
Got mine in, and just wow, its great 
.20 is no prob at all with a 3s 5ah lipo

@longhairedboy if you don't have one of these, you should

Deff need to beef up lipo wiring, even 10awg gets warm

.20 nickel welded to neg terminal @25ms 3s lipo and pull result...very pleased
<img src="/uploads/db1493/original/3X/6/2/628d97f484c96d7fd014fb64d34cd2852119fe0a.jpg" width="690" height="204">
<img src="/uploads/db1493/original/3X/2/d/2db0a491000fab4674295017ad2eb9d2d7805691.jpg" width="690" height="299">
<img src="/uploads/db1493/original/3X/7/2/72bd30d686e832ed8c722ca4a29d3febce55511f.jpg" width="628" height="500">
```

---
## \#14 Posted by: darkkevind Posted at: 2017-10-26T10:28:38.796Z Reads: 180

```
Just build one of my spot welders and be done with it... Bullet proof!

https://youtu.be/o1NFbchHeM8

https://youtu.be/o4NaDMoEHxU
```

---
## \#15 Posted by: scepterr Posted at: 2017-10-26T10:34:11.067Z Reads: 176

```
I've built a car battery spot welder before, it works but unreliable and uncontrollable. 
I use diff settings for various nickel thickness and depending what it's being welded to. 
Also Auto-weld is awesome.

Ive blown holes in cells with a car battery spot welder lol
```

---
## \#16 Posted by: darkkevind Posted at: 2017-10-26T10:55:03.474Z Reads: 172

```
Lol, I've got the timing down to a tee now, not blown anything yet...
```

---
## \#17 Posted by: longhairedboy Posted at: 2017-10-27T16:19:24.464Z Reads: 163

```
I've blown holes in cells with a Sunkko 788H. They leak a slipery werid smelling clear fluid. 

No way in hell i'm using battery based spot welder without a fuckload of testing and variable current at least.
```

---
## \#18 Posted by: scepterr Posted at: 2017-10-28T21:54:57.181Z Reads: 158

```
Just did a 14S5P pack, just about drained a single 3S 5Ah lipo, definitely faster than with sunkko, much fewer wait periods
```

---
## \#19 Posted by: Jpro Posted at: 2018-04-04T04:04:59.573Z Reads: 133

```
Are you in the U.S.A. ? I am from California and I really want to get this v3 kit for my first battery build how much would it be if you were in us?
```

---
## \#20 Posted by: Fiori Posted at: 2018-04-05T18:44:56.497Z Reads: 120

```
https://malectrics.eu/product/diy-arduino-battery-spot-welder-prebuilt-kit-v3/
```

---
## \#21 Posted by: s3rkan Posted at: 2018-05-27T21:07:01.094Z Reads: 100

```
Hello everyone. I have made a system like this:

https://youtu.be/pQ53sk9ksxQ

I have used 7 Irfb7430 mosfets from AliExpress and a timer module. I have changed the relay on timer module with a PNP mosfet and got a minimum 5msec pulse time. Made the probes with 35mm welding cables.

In short, I have prepared the system perfect as possible as I can do. I have tested the system with an oscilloscope before the welding process. But during spot welding, all the mosfets blown up. I remade the mosfet thing with 8 pcs IRF1404 but again all mosfets blown up. I only made the protection with skotcky diodes. I couldn't make the tvs protection because I couldn't find it in our local markets.

Do anyone have an idea what I am doing wrong?
```

---
