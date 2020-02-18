# 12s One Plug Charge Tutorial

### Replies: 33 Views: 3750

## \#1 Posted by: mason Posted at: 2016-06-29T03:32:25.584Z Reads: 422

```
I didn't want do have to deal with 4 different ports on my enclosure, so I set out to design a port similar to [this](http://miamielectricboards.com/shop-1/ez) but for 12s. Now thats it's done I can tell you, this is so convenient and easy to use.

**Heres what you will need:**
- [this](http://www.newegg.com/Product/Product.aspx?Item=9SIA0ZX3H71899) $4 and
- [corresponding male](http://www.newegg.com/Product/Product.aspx?Item=N82E16812200388) $7 and
- [this silicone cover which is optional $1](http://www.modcover.com/products/DB25-LPT-Printer-Port-Silicone-Rubber-Dust-Cover.html)
- some 6s balance leads
- deans (or xt60) connectors
- 2x 6s lipos or 4x 3s lipos (like me)

you will be soldering to this horribly draw diagram by me. NOTE: the battery leads (not the balance wires) are 16 gauge wire wired in parallel. one positive & negative per battery. 
<img src="/uploads/db1493/original/2X/4/48870a60033efac27325d79cc4caee7a5dbfb45f.png" width="666" height="500">
how it should look:
<img src="/uploads/db1493/original/2X/a/a31e42d640fd6a9af0173745db27e26e0138ec1d.JPG" width="690" height="388">
<img src="/uploads/db1493/original/2X/a/aa04807cf12b14867293eb4104fedf4eb7fd8ce7.JPG" width="690" height="388">
ultra ghetto looking battery
<img src="/uploads/db1493/original/2X/a/a31e42d640fd6a9af0173745db27e26e0138ec1d.JPG" width="690" height="388">
<img src="/uploads/db1493/original/2X/2/2d0821fe80e1927c78773c386c4304d51f37a678.JPG" width="690" height="388">
deans on the charger side. I'm using 2x iMax B6 chargers
<img src="/uploads/db1493/original/2X/a/a5953e9df7bf7079ea75453f622bf2f104db74d6.JPG" width="690" height="388">
ask questions if you need help/clarification!
I'll sell these if interested.
```

---
## \#2 Posted by: lowGuido Posted at: 2016-06-29T03:45:33.553Z Reads: 372

```
you can cut that connector down from 25 pin to only 13 pins or use a Dsub 15 if you want to double pin the main power rails.
make it more compact.
```

---
## \#3 Posted by: itsmikeholland Posted at: 2016-06-29T08:24:40.850Z Reads: 344

```
so what you're saying is that with this, I can charge 12s in series? I seriously spent all morning looking for a solution to this!
```

---
## \#4 Posted by: Maxid Posted at: 2016-06-29T08:49:37.003Z Reads: 331

```
no it charges two 6S batteries with probably two 6S chargers
```

---
## \#5 Posted by: Bender Posted at: 2016-06-29T11:58:56.300Z Reads: 299

```
Thanks guys I went with [these DB 15's](https://www.amazon.com/gp/product/B014W0UQOS/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1)
I find the 2 rows much easier to solder than the 3 row VGA type
If anybody (US) wants a pair pm me I don't need 10😀
```

---
## \#6 Posted by: mason Posted at: 2016-06-29T13:34:49.544Z Reads: 281

```
15 pins wont be enough for 12s
```

---
## \#7 Posted by: mason Posted at: 2016-06-29T13:35:34.064Z Reads: 265

```
@Maxid 
[quote="link5505, post:1, topic:5305"]
deans on the charger side. I'm using 2x iMax B6 chargers
[/quote]

10 characters
```

---
## \#8 Posted by: Maxid Posted at: 2016-06-29T13:39:39.698Z Reads: 256

```
15 is enough.
Two 6S batteries need 10 pins for the balancing cables and the rest is used for ground and total +.
The balancing ground is the main ground anyway and the balancing cable for the last cell is the total +.

Not sure how @lowGuido can make it with 13pins but 14 should be fine as long as you don't charge with high currents (keep it below let's say 2A). Maybe ground can be used for both batteries thus resulting in 13 used pins?
```

---
## \#9 Posted by: itsmikeholland Posted at: 2016-06-29T16:39:28.428Z Reads: 234

```
fuhhh charging 3x 4s batteries is proving to be hugely problematic. no wonder we don't see others using similar configurations very often
```

---
## \#10 Posted by: Maxid Posted at: 2016-06-29T17:00:28.184Z Reads: 221

```
yeah 3 batteries is a pain - you could get an 8S charger - and charge 2 in series in one as 4S maybe
```

---
## \#11 Posted by: mason Posted at: 2016-06-29T17:05:30.927Z Reads: 218

```
4x 3s like I'm doing is still a huge pain in the ass, but I made it (somewhat) easier. I permanently soldered two together in series for 6s, and used a 2x 3s to 6s adapter, aswell as an xt60. now it's just 2x 6s batteries to put in series.
```

---
## \#12 Posted by: itsmikeholland Posted at: 2016-06-29T17:31:25.414Z Reads: 208

```
Do we know what it is that makes a charger only compatible up to 8s or 10s? Is the limitation within the chemistry or just the mechanics? Why can't we just solder some new connectors and make it work? I feel like a 1000w charger should be able to handle my measly 298wh 12s rig, it doesn't seem right that it apparently "can't".

In the meantime I'll probably just buy 3x ~100w chargers and charge each 4S battery individually.

edit: or this one http://www.hobbyking.com/hobbyking/store/__82840__Turnigy_Reaktor_QuadKore_1200W_80A_4_X_300W_20A_DC_Synchronous_Balance_Charger_Discharger.html
```

---
## \#13 Posted by: lowGuido Posted at: 2016-06-29T21:22:11.097Z Reads: 199

```
heres a diagram on how to pinout a balance lead for 12S with a DSUB 15 pin. and thats with double pins on the main power leads. the red and black leads would be 16AWG or similar.

<img src="/uploads/db1493/original/2X/8/8e7e8bf208adcaeee0828d8db326f47d9d637348.JPG" width="690" height="253">

I meant to put it up yesterday but I ran out of time.
```

---
## \#14 Posted by: lowGuido Posted at: 2016-06-29T21:59:07.682Z Reads: 200

```
the charger end would look like this:
<img src="/uploads/db1493/original/2X/9/97575dcea97d9394d4989524a6122ff498e1a384.JPG" width="445" height="500">

you could get it down to 13 pins if you didn't double pin the main power, and perhaps charge at only 2A?
```

---
## \#15 Posted by: Maxid Posted at: 2016-06-29T22:00:13.196Z Reads: 184

```
he does not charge at 12s but 2x6S - that is why I was wondering how you can get it done in 13.
```

---
## \#16 Posted by: lowGuido Posted at: 2016-06-29T22:02:23.357Z Reads: 185

```
can still be done in 13 pins, you would just need to change the charger end to two 6S plugs and two deans connectors.... 
do you really want me to draw another diagram?? LOL
```

---
## \#17 Posted by: Maxid Posted at: 2016-06-29T22:06:24.718Z Reads: 182

```
But they are not in series anymore at 6S - so I think as I have said above you would need 14 pins.
I just don't see it right now so if you actually could draw that I would be happy.
```

---
## \#18 Posted by: lowGuido Posted at: 2016-06-29T22:14:22.529Z Reads: 193

```
<img src="/uploads/db1493/original/2X/7/76454e754b3ced0c17fcc135a85a8a4a033029e9.JPG" width="445" height="500">

sorry this drawing is rough. you wouldn't have enough pins to double pin every charge lead so if I was going to do it this way I would probably not bother double pinning the outer leads and maybe separate pin 12 into two pins instead.
you are starting to compromise on the amount of amps you can charge with. it can certainly be done with 13 pins, but perhaps not a DSUB 15, perhaps something with some higher current pins available.
```

---
## \#19 Posted by: Maxid Posted at: 2016-06-29T22:17:27.788Z Reads: 182

```
so you can actually leave them connected in series and treat them like two 6S packs where you connect the second pack's ground to the 6th cell's positive?
```

---
## \#20 Posted by: lowGuido Posted at: 2016-06-29T22:20:14.196Z Reads: 178

```
it is literally no different to how he currently has it set up.
the cells are connected in the battery
```

---
## \#21 Posted by: Bender Posted at: 2016-07-04T12:58:38.520Z Reads: 171

```
Am I correct in thinking that you'd have to charge one 6s pack at a time and not 2 in parallel with this setup?
```

---
## \#22 Posted by: lowGuido Posted at: 2016-07-05T04:00:47.058Z Reads: 163

```
@Bender you definitely can't parallel charge this setup. You would need 2 chargers.
```

---
## \#23 Posted by: longboardshort Posted at: 2018-04-08T16:43:11.507Z Reads: 92

```
Been searching and can’t find any pre-built permanent charging options I would possibly buy and I bet many others would eventually.. maybe) a pre-soldered/setup charging port solution allowing for permanent battery mounting. I’d be especially interested in 10s and 12s lipo ports. 

I’m guessing a d-sub connector that would mount to enclosure panel with balance connector or harness to plug individual batteries into. Ideally it would come with the external harness to plug into the charger. Even if it would require two charging ports. 

Is there any sort of rendition to his that exists and is available? Thought i remember Miami offering something similar to this, but then when I checked later it wasn’t available/offered any longer. I’m hoping my search ability is less than adequate and there is. If not I will be adding this on my long to do list.
```

---
## \#24 Posted by: lowGuido Posted at: 2018-04-10T19:26:52.655Z Reads: 86

```
these days I just have one or two balance connectors coming out of the box and I just charge off them.
```

---
## \#25 Posted by: Hummie Posted at: 2018-04-10T20:22:34.747Z Reads: 84

```
That seems a nice solution w nothing needed in the board yet still balancing and also electronically simple.  If it were all hooked up with a 13 prong plug be great
```

---
## \#26 Posted by: Acidfie Posted at: 2018-04-10T20:27:49.176Z Reads: 76

```
please keep in mind that most D-SUBS have about 100 plug in&out cycles before something dies..
```

---
## \#27 Posted by: longboardshort Posted at: 2018-04-11T16:24:58.526Z Reads: 75

```
Can you recommend any D-subs that have a better lifetime?  I don't mind paying for them, as I have a couple sets of batteries that i'll likely be switching.. more and more I think about it I feel like I should just buy a BMS.. but do they accomodate for different batteries?  ie 12s vs 10s vs 6s.. so are there universal ones I suppose is the question?
```

---
## \#28 Posted by: philvanzu Posted at: 2018-04-11T18:50:32.071Z Reads: 69

```
@toleg is building a real beauty of a board with external BMS, he uses a DIN connector.
Pics visible [here](http://e-sk8.fr/forum/viewtopic.php?f=7&t=2417&start=181)
```

---
## \#29 Posted by: longboardshort Posted at: 2018-05-17T15:58:42.343Z Reads: 55

```
Can you charge them without removing your enclosure?
```

---
## \#30 Posted by: lowGuido Posted at: 2018-05-18T05:35:43.721Z Reads: 52

```
Yes. Always
```

---
## \#31 Posted by: longboardshort Posted at: 2018-05-18T17:15:15.906Z Reads: 48

```
Could you please shed me a little insight prease?  I am currently trying to install I guess a very close to identical setup as this (I have two 6S VGA adapters soldered up and ready to install) but am reluctant to still because Im not sure how to lay it out exactly for long term charging option w/o enclosure removal.  

Please and thank you brudda
```

---
## \#32 Posted by: lowGuido Posted at: 2018-05-19T03:07:00.586Z Reads: 44

```
These days i just poke a balance lead out the side.
Keeps it simple.
![20170804_161036|690x388](upload://a77JEshJMhBVJeakjF49LroqOAs.jpg)
```

---
## \#33 Posted by: longboardshort Posted at: 2018-05-20T04:58:12.438Z Reads: 39

```
Ok hopefully this is my last question on this topic. So would this setup work:

Dual 6s lipos, each going to a custom VGA adapter along with the balance leads. The + of bat1 and - of bat2 will form the series 12s connection. 

There will be a removable loopkey between the common wire between the two 6s batteries going from + of one to - of the other which I will remove for charging. Then the 12s series connection will go to another (main power) removable loopkey then to escs and rest of electronics. 

Does anyone see any issues with this setup? Thanks in advance!
```

---
