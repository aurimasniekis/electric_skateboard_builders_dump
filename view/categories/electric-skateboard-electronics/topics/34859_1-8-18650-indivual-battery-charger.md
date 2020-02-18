# 1 - 8 18650 indivual battery charger

### Replies: 23 Views: 1959

## \#1 Posted by: D_Sk8 Posted at: 2017-10-05T18:01:09.396Z Reads: 111

```
It's ugly but, for the most part, my first electronics build (experience with soldering). Seems to be working ok. Pretty stoked. I only have an 5v 8a power supply (40 watts), and not certain if the PCB boards actually pull 5v 1a, or 4.2v 1a. In any case, 4.2 volts x 1a = 50.4 watts, and even with 8 of them connected the power supply is a bit warm.

<img src="/uploads/db1493/original/3X/8/2/825e2a1dee96691bd385c84c51d79bc4769f2b27.jpg" width="690" height="388">

I take no credit. Stole the idea from:

https://www.youtube.com/watch?v=KoHtxZG7leQ&t=132s

8 x PCB - $2.40 (when you buy 20)
 
http://www.ebay.com/itm/253068167608
 
4x 18650 Holders x 3 = $3.38
 
http://www.ebay.com/itm/272492989012

5v 8a power supply $14.80

https://www.amazon.com/dp/B0714LKDGS?ref_=pe_2640190_233158860_shiptrack_e_404_dt_1

Other items, 2 sided tape to mount to board.
Board laying around the house or home depot.
wire
solder
electrical tape.
Ability to ignore an ugly job that works.

This will "balance" charge each cell to 4.2v.

I am going to use this to get all cells to max capacity before discharging them to test capacity. The generic B6 charger I have only charges to 4.1v, and I don't know if I trust that even. After charging some show only 4.03, some 4.10. One balance charger says it's charging to 4.2v, and still reads less than 4.10 with a multimeter.

Anyway, enjoy.
```

---
## \#2 Posted by: Davewesh Posted at: 2017-10-05T18:20:52.356Z Reads: 91

```
Looks good! I checked out those TP4056 for my battery design - and pretty much wrote them off as to expensive for a 48 cell battery. 

That being said, I still like this idea for testing, and ultimately keeping my cells charged for my RC-Car since i use LI-ION for servo control and my Nitro Starter. 

Good job on the execution and presentation, time to get a 3d printer and design an enclosure for it!
```

---
## \#3 Posted by: D_Sk8 Posted at: 2017-10-05T19:05:25.733Z Reads: 83

```
Don't tell my wife that. lol, I have seriously been considering buying one. Thanks for the kudos. I haven't done much research but I see people have PCB board printers of some sort. It'd be nice to clean the wiring up on this.

To confirm it worked great:

<img src="/uploads/db1493/original/3X/5/3/53df00e35c6db64a0ae34a380d830d0e1c278235.jpg" width="281" height="500">
```

---
## \#4 Posted by: Davewesh Posted at: 2017-10-05T19:32:33.792Z Reads: 73

```
Good news is that microcenter has a pretty decent lineup of 3d printers if you dont want to go the DIY route, as well they are relatively affordable. The problem with most of them though is that the work space isn't going to be the largest - so you'll likely need to design an enclosure that would be thicker rather than thinner to accommodate everything. 

I've been looking at the PCB routers/printers as well and really haven't found any good "desktop" PCB machine. I have found a few desktop CNC machines that can do simple PCB's but when you start jumping into the multi-layers it seems almost more economical to just contract the board out to a company for a one-off. My biggest interest in getting a PCB printer would be so that I can design my own battery packs and supplemental current delivery - as well as possibly running my own VESC - would be kinda cool but ive not seen any under 5k that can do upwards of 10 layers - as well their conductivity may not allow that kind of power. 

Either way, glad to see it worked my friend! Good Job!
```

---
## \#5 Posted by: D_Sk8 Posted at: 2017-10-05T19:33:44.158Z Reads: 65

```
Ugh, ok. I'll continue with wiring. haha
```

---
## \#6 Posted by: darkkevind Posted at: 2017-10-05T19:47:50.352Z Reads: 65

```
I've already done it.... :smiley:

<img src="/uploads/db1493/original/3X/6/0/60663de4bee4a86d99bd9d35e6830bb712f04039.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/6/7/6752bf9d6ef7991e06b26cf7c40859879a7e4448.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/5/f/5f18dd7763e6f2e11993013c9cfc753e8b47d5a0.jpg" width="690" height="388">
```

---
## \#7 Posted by: D_Sk8 Posted at: 2017-10-05T19:51:15.084Z Reads: 59

```
Ohh damn, you made your own static balance charger, haha. That's pretty sick. I'm going to use a BMS, this is just to get the batteries to 4.20v so I can test capacity with IMAX B6 charging units, so I can build a proper 12s5p battery pack.
```

---
## \#8 Posted by: scepterr Posted at: 2017-10-05T19:54:02.592Z Reads: 59

```
Make sure the tp4056 at the end of the string are getting enough current, you might need to run power leads to both ends. Check www.diypowerwalls.com for dozens of diff multi tp4056 setups, from 5 to 40-50
```

---
## \#9 Posted by: D_Sk8 Posted at: 2017-10-05T19:55:57.923Z Reads: 58

```
That's a good point. That's probably why I am seeing some strange behavior. It's getting the current, but I am only using 8 of 12. But I just noticed some odd behavior when I had on in space 12, then filled spaced 1-7. (2 different 18650 battery types). I had to unplug the charger and plug it back it for it to register. Seems to have charged the batteries fine after that though.
```

---
## \#10 Posted by: D_Sk8 Posted at: 2017-10-05T19:56:25.767Z Reads: 55

```
Awesome site. I'm gonna bookmark that, thank you.
```

---
## \#11 Posted by: darkkevind Posted at: 2017-10-05T19:57:11.050Z Reads: 51

```
If anything they need to be over-volted, something like 5.5 or 6v...
```

---
## \#12 Posted by: D_Sk8 Posted at: 2017-10-05T20:01:14.578Z Reads: 47

```
I have a 300 watt DC to DC converter and 90 watt laptop power supply I can use. It's a bit easier finding higher volt power supplies with higher watts than 5v ones.
```

---
## \#13 Posted by: scepterr Posted at: 2017-10-05T20:01:29.421Z Reads: 48

```
Run a copper bus bar thick enough to not drop voltage for positive and neg across the top and then connect each tp4056 to it. 
Computer PSU are good, just make sure to hook up something(a fan) to 12v to get full power on 5V
```

---
## \#14 Posted by: darkkevind Posted at: 2017-10-05T20:02:39.529Z Reads: 48

```
You can't go too high with the input voltage... 6v is probably max. Check the specs on your TP4056's
```

---
## \#15 Posted by: scepterr Posted at: 2017-10-05T20:03:31.068Z Reads: 48

```
There's no need to overvolt, the right capacity bus bar will hold 5V across it
```

---
## \#16 Posted by: scepterr Posted at: 2017-10-05T20:06:04.407Z Reads: 50

```
This is one of my many, many tp4056 rigs 😉
<img src="/uploads/db1493/original/3X/2/0/203f52492c3733a4f72b4e8a4486f16f2191bd33.jpg" width="690" height="393">
I have since replaced the rprog resistor with a pot for variable charge current. It can do up to 1.2A if you put a tiny heatsink on the ic or have a fan blowing across them
```

---
## \#17 Posted by: D_Sk8 Posted at: 2017-10-05T20:11:14.592Z Reads: 50

```
Ohh, I see. I think I saw some battery packs that had contacts under the holder that could connect to a bar. I'll check into those. Might be easier to work with the bar on.

https://youtu.be/vryHAt8liMs?t=113
```

---
## \#18 Posted by: D_Sk8 Posted at: 2017-10-05T20:11:43.404Z Reads: 47

```
That's awesome.
```

---
## \#19 Posted by: scepterr Posted at: 2017-10-05T20:14:08.521Z Reads: 49

```
Also if you using the B6 for Mass charging I prefer the series method over parallel, and you can still parallel on top of the series. I made 6S cradles using the 18650 holders so I can balance charge 6 at a time, or 12,18 etc if 2P,3P<img src="/uploads/db1493/original/3X/1/e/1e300f6fe4962bb445bb90b7789a239ae006d2d0.jpg" width="690" height="372">
```

---
## \#20 Posted by: D_Sk8 Posted at: 2017-10-05T20:15:14.071Z Reads: 48

```
I can't even get 4.20v charge via the B6. I am just going to use the B6 to check capacity at this point. I am finding the fake ones I got are not consistent and not certain I should even trust the capacity testing.
```

---
## \#21 Posted by: scepterr Posted at: 2017-10-05T20:17:28.361Z Reads: 45

```
Manually set the vmax on the b6, sometime it needs that
```

---
## \#22 Posted by: D_Sk8 Posted at: 2017-10-06T16:18:46.100Z Reads: 38

```
Anyone have any idea's on reverse polarity protection? lol. Oops. 1 down 11 to go.
```

---
## \#23 Posted by: scepterr Posted at: 2017-10-07T06:08:01.412Z Reads: 28

```
It doesn't have reverse polarity protection that you can rely on, only if it's a nearly dead battery and you're quick to get it out, I think it's only up to 2A, then it'll pop
```

---
