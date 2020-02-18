# EBoard Mosfet Switch

### Replies: 172 Views: 18551

## \#1 Posted by: JdogAwesome Posted at: 2016-07-08T02:25:05.936Z Reads: 868

```
Hello everyone! This is my first post on eSk8 though ive been reading stuff on here for a while now. A couple months ago I wanted a new switch for my board other than my crap-a-tronic fuse switch that was falling apart. So I looked some up and saw a couple very similar devices online from Alien Drive, DIY Boards and a couple other sellers. They were all around $60 and I didn't want to spend that much so I decided to build my own. I looked around a bit online and asked some questions on some forums and got some answers eventually. Currently the switch is built around a IRLB3034 N-Channel MOSFET which is an amazing fet because of its extremely low RDS of only 1.7m Ohm, which in turn makes it extremely efficient and cool running. I tested the switch on  my board which draws around 8-10 Amps cruising normally and ~15 Amps going pretty fast. At any of these speeds the mosfet didnt even get warm, and I was testing this on a 90f degree day. The 3034 fet is great and super cheap, but the problem is it has a max voltage of 40V which will only work with 8S lipos at the most, though dont fret because I found a higher voltage mosfet! The IRFB7530 is another great fet with a rds of only 1.65mOhms and has a max voltage of 60V which means it can work with upto 12S LiPos. Anyways enough with the specs, I am going to upload the schematic for anyone who wants to build there own, but for people who dont want to build one themselves, I would be happy to make and sell them. The circuit would have its own custom PCB and ports for the switch to turn the fet on and off as well as XT60 connectors for power. If anyone is interested in buying one or getting some more info on it im more than happy to help! The couple of pics of the actual circuit was the very first version I made and if I were to do it again it would look far better. 

**DOWNLOAD FOR ALL SCHEMATICS AND BOARD FILES [HERE](http://www.filedropper.com/eboardswitchallversions_1)**

**[HERE](http://www.ebay.com/itm/5pcs-5X-IRLB3034PBF-IRLB3034-HEXFET-Power-MOSFET-TO-220-US-SHIP-/321964625484?hash=item4af6964e4c) is where I purchased the IRLB3034 MOSFET's. The rest of the components you should be able to source your self. I bought everything else on eBay FYI** 

**[IRFB7530](http://www.mouser.com/ProductDetail/Infineon/IRFB7530PBF/?qs=%2fha2pyFaduixAttjbpOXvXaMy%2foIUVggzQUs0Kk54zI%3d) on Mouser.**

**Prices:**
**[IRFB7530](http://www.infineon.com/dgdl/irfs7530pbf.pdf?fileId=5546d462533600a4015364c3d98429c3) ~40A Single FET Switch ~$25**
**[IRFB7530](http://www.infineon.com/dgdl/irfs7530pbf.pdf?fileId=5546d462533600a4015364c3d98429c3) ~80A Dual FET Switch ~$35**
**[IRFB7530-7P](http://www.mouser.com/ds/2/196/irfs7530-7ppbf-937822.pdf) ~100A Dual FET Switch ~$40**
**[IRFB7530-7P](http://www.mouser.com/ds/2/196/irfs7530-7ppbf-937822.pdf) ~50A Single FET Switch ~$30**
**FYI I custom make every PCB so if you need it to fit a certain size requirement just ask and ill try to accommodate it to your needs.**


<img src="/uploads/db1493/original/2X/6/64874b158f8c03d6084226ea0a352d649a592174.png" width="690" height="331">

**NEW VERSION WITH IRFB7530:**
<img src="/uploads/db1493/original/2X/f/f38c1541fcb6e8b5f46db12576df9d4ebaf2266b.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/3/363d7b4d6a69cde10b074308cff4bd1f6bdd0b5f.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/7/761e8bc312c0edb6f72468b0cec843afcde1054a.jpg" width="690" height="388">

Tags: Electric Skateboard Switch, MOSFET Switch, Electric Longboard Switch
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-07-08T03:17:54.955Z Reads: 696

```
Welcome and good first post 🤘🏻
```

---
## \#3 Posted by: Jack Posted at: 2016-07-08T03:19:41.970Z Reads: 686

```
This what your looking for? :slight_smile:

https://github.com/vedderb/SparkSwitch
```

---
## \#4 Posted by: JdogAwesome Posted at: 2016-07-08T03:33:47.651Z Reads: 680

```
That is an interesting design though im not looking for anything I just wanted to share this design, thanks though!
```

---
## \#5 Posted by: treenutter Posted at: 2016-07-08T15:38:42.083Z Reads: 637

```
@JdogAwesome Thanks for sharing this! If you produced a parts list or BOM, that would be a huge help for anyone interested in building your design. If it was a list with links to a vendor like Mouser, that would be even better.
```

---
## \#6 Posted by: lox897 Posted at: 2016-07-09T02:24:26.494Z Reads: 587

```
A BOM would be best. Then we can just import it straight into Mouser and buy it all with a few clicks.
```

---
## \#7 Posted by: JdogAwesome Posted at: 2016-07-09T10:47:30.685Z Reads: 561

```
Yeah ill definitely do that. Personally I just bought the mosfet on EBay, though I had to order like 5 of them, though it was still only like under $10. Then there's the diode which ill link, you can get those on eBay in small bulk packs for like $1-2 and there great to have for any electronics enthusiast. And then just some 10K resistors and perf board to assemble it on, though I would highly recommend just making your own PCB, its actually quite simple and looks beatiful!
```

---
## \#8 Posted by: Astrolite_A15 Posted at: 2016-07-12T01:53:11.808Z Reads: 527

```
Would you still get a spark with this or just when hooking up the battery? Do I need an anti spark connector? Pardon my ignorance, still pre-build.
```

---
## \#9 Posted by: JdogAwesome Posted at: 2016-07-13T23:53:18.050Z Reads: 523

```
Sorry for the extremely late reply I thought I sent this message already! Anyways here us what I meant to send to you: 
No there is 0 spark because your arent connecting any wires with this, it is all controlled internally inside of the MOSFET.

## !!!VERY IMPORTANT NOTICE!!!

## Please read post number 67 about the gate resistor values!
```

---
## \#10 Posted by: JdogAwesome Posted at: 2016-07-14T05:13:39.290Z Reads: 501

```
Also I found this [MOSFET](http://www.mouser.com/ds/2/196/irfp7718pbf-936343.pdf), its the IRFP7718PBF and its capable of handling 75V or a 17S LiPo Pack! So if anyone was planning on making a 17S pack, then yeah I guess you could do that, though good luck finding an ESC capable of running 75V.
```

---
## \#11 Posted by: JdogAwesome Posted at: 2016-07-14T18:24:25.087Z Reads: 510

```


**OUTDATED SCHEMATIC NEW VERSIONS BELOW**

Here is a schematic I designed for the switch, in the example it uses an IRFB7530 mosfet, and is designed for 12S, though you can change that out for a different kind of mosfet. The circuit image and and .Zip download are below. Note that the LED resistor must be at least a 1/2W resistor but I would recommend a 1W so it doesn't get to hot. **IMPORTANT!** The thick traces for the + and - rails are not thick enough to handle high amperage, you have to add a layer of solder on the top or a wire that runs along it to handle the higher amperage. 

<img src="/uploads/db1493/original/2X/f/fe76cefca6280753e01b2d44e3734ccc56aeee30.png" width="648" height="500">

 **And you can download the .zip with the schematic and board [HERE](http://www.filedropper.com/eboardswitchv2_1).**
```

---
## \#12 Posted by: ndwallick Posted at: 2016-08-03T20:06:19.048Z Reads: 443

```
This is awesome it's exactly what I need, I am about to make it, does anybody know what the diode is for?
```

---
## \#13 Posted by: Maxid Posted at: 2016-08-03T21:10:44.474Z Reads: 441

```
you know there is a better one right?
https://github.com/vedderb/SparkSwitch/
```

---
## \#14 Posted by: JdogAwesome Posted at: 2016-08-03T22:13:22.367Z Reads: 436

```
Hey ndwallick the diode is an essential part of the circuit. The diode lets buildup current flow from the - to the + lead which is the opposite of the way current normally flows, this is because of an electron buildup that can occur and destroy a circuit if a diode is not there to let the electrons flow back. Anyways, its a very important part of the circuit and if you were asking to see whether or not you need the diode, the answer is a definite yes, lol. Though thank you for asking the question so now others will know!
```

---
## \#15 Posted by: JdogAwesome Posted at: 2016-08-03T22:28:28.539Z Reads: 424

```
Hello Maxid, at the time of me needing a new switch for my EBoard, I had no idea the Vedder switch even existed, if I had I would have most likely used that design. When I created this thread I still had no idea the Vedder switch existed and it was only until someone told me about the Vedder switch because of how similar my switch is and the Vedder one were that I found about it. I still think that it cant hurt having more than one design for a MOSFET switch out there and this is my version of it, I know this one is very similar but still I don't think it can do anybody any harm having this one out there.
```

---
## \#16 Posted by: VladPomogaev Posted at: 2016-08-04T10:14:42.533Z Reads: 407

```
Your through-hole components have the traces on the top of the board. I believe that you need to either flip the components, or flip the traces (make them blue).
```

---
## \#17 Posted by: Astrolite_A15 Posted at: 2016-08-04T10:18:53.279Z Reads: 397

```
After I click the link, I have no idea what I'm looking at. Easier for me to just copy this one.
```

---
## \#18 Posted by: JdogAwesome Posted at: 2016-08-04T15:03:01.485Z Reads: 404

```
That's a good point but if you noticed how I'm using the heatsink flange for the mosfets drain, I have to have the components on the top side with the traces on the top side as well. Though you could definitely have just the mosfet on the top side and the other things like resistors and the diode on the bottom side.
```

---
## \#19 Posted by: JdogAwesome Posted at: 2016-08-04T15:13:06.300Z Reads: 402

```
Yeah that github link is kinda confusing but below is the real post on endles sphere about the switch. I highly recommend you take a look at both of these designs and just use whatever works better for you, or you like more. 
Thread: https://endless-sphere.com/forums/viewtopic.php?f=31&t=73800
```

---
## \#20 Posted by: VladPomogaev Posted at: 2016-08-04T15:52:34.343Z Reads: 399

```
Yes, but literally all of your other components need to be on the other side of the board then, especially your LED and pin header, which you won't be able to solder on (unless your via is already made there).
```

---
## \#21 Posted by: JdogAwesome Posted at: 2016-08-04T16:33:04.172Z Reads: 375

```
That's true but even if you did that it would still work, it wouldn't be the prettiest thing but it would work. Also you could mount all the components on the opposite side and just bolt the FET through the PCB onto the large contact for the drain. In fact that might actually work pretty well and I may do that my self.
```

---
## \#22 Posted by: VladPomogaev Posted at: 2016-08-04T16:46:57.159Z Reads: 371

```
I think that's sort-of what I've been saying :)
```

---
## \#23 Posted by: ndwallick Posted at: 2016-08-05T04:36:10.261Z Reads: 398

```
Just finished building it! I thought I'd show everybody here.

I left out the LED.
I tested it on a 15 volt power supply and it works.
Time to test it on my 10s LiFe batteries.<img src="/uploads/db1493/original/2X/d/da9a783efec9c5a40f7204dd5db531b5df7f8651.JPG" width="666" height="500"><img src="/uploads/db1493/original/2X/c/cdabed98a82efea333878b4990a5ea40b00c5d9c.JPG" width="666" height="500">
```

---
## \#24 Posted by: ndwallick Posted at: 2016-08-05T04:48:37.424Z Reads: 361

```
Works perfectly on 33 volts too
```

---
## \#25 Posted by: JdogAwesome Posted at: 2016-08-05T23:32:56.961Z Reads: 364

```
That's so cool that you actually built the design! Thank you it means a lot! That's great to hear that its working well, did you use the same IRFB7530 MOSFET or did you use another type? Also I would recommend that you maybe shrink wrap the entire thing or wrap it in electrical tape, if you haven't already done that lol.
```

---
## \#26 Posted by: ndwallick Posted at: 2016-08-05T23:40:10.372Z Reads: 353

```
Of course! I used the IRLB3034 cause it was cheapest and my batteries will stay under 40 volts. I definitely plan on insulating it with something. Wish I had some large clear heat shrink.
```

---
## \#27 Posted by: JdogAwesome Posted at: 2016-08-05T23:49:05.278Z Reads: 359

```
Yeah the 3034 is what I'm using in my board and it seems to work very well. Did you buy the 3034 on EBay from some cheap seller or did you buy them from a trusted retailer like Mouser? I'm just wondering because you might wanna be careful running them near there limit if there cheaper non legit versions. I'm using some cheap ones off of eBay though they work fine for me and don't get warm whatsoever at 6S ~15A cointinous.
```

---
## \#28 Posted by: ndwallick Posted at: 2016-08-05T23:55:30.795Z Reads: 349

```
I got the ones off eBay that you linked in your first post, it's been working fine so far just testing on my desk with no load. I guess I'll find out how it works with load once I complete my board haha.
```

---
## \#29 Posted by: Astrolite_A15 Posted at: 2016-08-06T01:15:10.631Z Reads: 350

```
I'll test these on a 6S when they come in:
http://www.ebay.com.au/itm/10Pcs-IRLB3034PBF-IRLB3034-HEXFET-Power-MOSFET-TO-220-/191736128497?hash=item2ca45d23f1:g:PH8AAOSw5VFWIMaw

Will be using these on my own stuff though:
http://au.rs-online.com/web/p/products/8208833/?cm_mmc=AU-PPC-_-google-_-3_AU_EN_M_SEMIS_Broad-_-international_rectifier%7Cmosfet_transistors&mkwid=sFxbMWOKY_dc%7Cpcrid%7C82233297603%7Cpkw%7C%2Birfb7530pbf%7Cpmt%7Cb%7Cprd%7C

When I etch my board I'll post pics. Thanks for sharing this with us.
```

---
## \#30 Posted by: ndwallick Posted at: 2016-08-06T02:30:22.944Z Reads: 342

```
Can anyone with more electronics knowledge answer this question?

Suppose this switch is off and I am kicking my board. I'm assuming the Vesc will be on because it is being powered from the motor spinning. If I send a brake command to the vesc will the batteries charge? (because mosfets do not block current going backwards)
```

---
## \#31 Posted by: JdogAwesome Posted at: 2016-08-06T04:55:25.335Z Reads: 331

```
Well first off I heard some people talking about almost exactly this in another thread, I'm not sure where but ill try to find out. Though eventually they decided that pushing the board along with it being off was a very bad idea, and they are very right. If the switch is off then it won't allow current to flow either direction which means you'll have an electron buildup which could, and will, lead to either killing a your VESC MOSFET or other components connected to the circuit. And I don't even think peddling would supply enough current to keep the VESC on. But if it did and it tried letting current flow to the batteries, obviously the MOSFET switch but be in between and would then either kill the fet or the VESC. @ndwallick
```

---
## \#32 Posted by: JdogAwesome Posted at: 2016-08-06T05:02:06.890Z Reads: 317

```
Hey Astro! The ones you linked on EBay I'm sure will work, but they won't be as good or as trustworthy as legitimate versions from a trusted retailer like the other MOSFET you linked. Also you can get the exact same IRFB7530PBF on Mouser for only $3.33 so there a couple $$$ cheaper. And Mouser is definitely a legitimate vendor.
```

---
## \#33 Posted by: Astrolite_A15 Posted at: 2016-08-06T05:40:16.947Z Reads: 322

```
Do they ship free to AUS? (edit) Just saw 'Free shipping for orders over $60' not sure if thats int. though.
```

---
## \#34 Posted by: JdogAwesome Posted at: 2016-08-06T06:06:26.725Z Reads: 328

```
Have no clue you might wanna just check yourself by checking out and getting far enough to see shipping rates. I ordered 10 IRFB7530 on Mouser for $2.83 A piece and they seem to be of good quality and shipping was right around $5 but that was in the US.
```

---
## \#35 Posted by: Astrolite_A15 Posted at: 2016-08-06T06:07:29.842Z Reads: 321

```
Thanks, might get my hands on both and compare them for the Aussie users.
```

---
## \#36 Posted by: JdogAwesome Posted at: 2016-08-09T03:39:54.100Z Reads: 338

```
VladPomogaev was saying that I should also have the MOSFET on the opposite side of the board like most PCB's are and have a bolt go through the board and that was definitely the right idea. Anyways I redesigned a small part of the schematic to accommodate the MOSFET being mirrored on the opposite side of the copper traces. So if you plan on doing that please use this design instead.

**And you can download the .sch and .brd [HERE](http://www.filedropper.com/eboardswitchv3)**

<img src="/uploads/db1493/original/2X/a/a3b863de76064306c2e1a0bc20b2d2e96319972d.png" width="648" height="500">
```

---
## \#37 Posted by: JdogAwesome Posted at: 2016-08-09T05:27:50.694Z Reads: 325

```
You mentioned wanting some large heat shrink and I found a bunch of different sizes on Aliexpess, I just ordered [THIS](http://www.aliexpress.com/item/2Meter-64mm-Width-PVC-Heat-Shrink-Wrap-Tube-Blue-for-AA-Battery-Pack/32616421465.html?spm=2114.13010608.0.56.y8mgPv) for $2.20 and ill see how it works once it gets here. [HERE](http://www.aliexpress.com/wholesale?catId=0&initiative_id=SB_20160808212648&SearchText=PVC+Heat+Shrink) is a search that brings up a ton of different sizes of heat shrink on AliExpres. Just make sure to put how large you want it in mm.
```

---
## \#38 Posted by: Jinra Posted at: 2016-08-09T05:30:18.284Z Reads: 315

```
Wow that is CHEAP. Ali's a good place to get stuff from if you don't mind waiting a couple weeks. I got two pairs of bushings for $2 as well.
```

---
## \#39 Posted by: JdogAwesome Posted at: 2016-08-16T17:22:08.426Z Reads: 345

```
I finally finished making the circuit and it turned out ok! I tested it at 15V and it works fine though I'm going to be testing it at 24V soon. I'm aware that my soldering skills are complete crap, but hey it works lol. For the XT60 leads I used some awesome high strand super flexible 12 AWG wire and the mosfet is the IRFB7530PbF for a 12S build. I still have to shrink wrap the entire thing to give it some protection but I will do that when it arrives.

P.S. I got my 12AWG Wire off of Amazon, but I found some on Aliexpress for $4 a meter, which is pretty good in my opion if you don't mind waiting a month. [LINK](http://www.aliexpress.com/item/1-METER-Red-1-METER-Black-12AWG-14AWG-16AWG-22AWG-24AWG-Heat-proof-Soft-Silicone/32555643416.html?spm=2114.01010208.3.68.kLita6&ws_ab_test=searchweb201556_10,searchweb201602_1_10057_10056_10037_10055_10049_301_10059_10033_10058_10032_10017_106_105_104_10060_103_10061_102_10062,searchweb201603_2&btsid=d73e2c52-f1ba-4710-9b0d-f63bede90b29) 

<img src="/uploads/db1493/original/2X/2/26a5cc50e8ba22124b034d312f571542738e7377.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/9/9fed5e32c2fcc2458ea561d9c92a01d83e6a5d57.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/3/38f1d8e1c426085dc6e83aaeeffd8b82f2f51abb.jpg" width="690" height="388">
```

---
## \#40 Posted by: Nordle Posted at: 2016-08-16T17:26:57.965Z Reads: 324

```
Just don't order cheap fets or caps from Aliexpress
```

---
## \#41 Posted by: VladPomogaev Posted at: 2016-08-17T05:33:14.164Z Reads: 309

```
Ah! You run the current through the bolt and nut! I understand now. Are you thinking of ever putting some more MOSFETs on in parallel?
```

---
## \#42 Posted by: JdogAwesome Posted at: 2016-08-17T05:36:01.268Z Reads: 313

```
[s]I dont think it will ever be necessary to put 2 or more in parallel but you never know :)[/s]
```

---
## \#43 Posted by: JdogAwesome Posted at: 2016-08-19T01:06:52.021Z Reads: 330

```
Here is the finished product, shrink wrapped and ready to be shipped out! Tested it on 24V and it worked well without any temp increase though I guess ill see how it works in the 52V 12S system it will be in. 

<img src="/uploads/db1493/original/2X/1/11e6b8b94522565a316ab1ac81a1beb2d9d6f148.jpg" width="690" height="388">

<img src="/uploads/db1493/original/2X/7/7a242ccca5abf014e701edac601ac15e700f44cf.jpg" width="690" height="388">

<img src="/uploads/db1493/original/2X/8/83b291292ed70ed25b7f09fd900477a44dd79283.jpg" width="690" height="388">
```

---
## \#44 Posted by: JdogAwesome Posted at: 2016-08-20T02:03:06.448Z Reads: 314

```
[quote="JdogAwesome, post:42, topic:5738"]
I dont think it will ever be necessary to put 2 or more in parallel but you never know :slight_smile:
[/quote]

Actually I've changed my mind completely lol. Yes I think there would be reason to put 2 or more fets in parallel for a higher current application, in fact im working on designing a PCB that is very similar to the original design, except it accommodates two TO-220 MOSFET's instead of one for an upto ~60A system. I also may work on a schematic using the IRFS7530-7P which is pretty much the same fet that the VESC uses, because of its lower RDSON and lower C/W rating.
```

---
## \#45 Posted by: JdogAwesome Posted at: 2016-08-20T03:49:23.377Z Reads: 319

```
I mentioned in the post above about creating a board that would have two MOSFET's in parallel, well I finished designing it and its obviously extremely similar to the original single fet design though it will work if you ever need to pull somewhere around 40-60A continuous. I also still plan on making a design around the IRFS7530-7P when I have time to do so.

**.Zip with Brd and Schm files [HERE](http://www.filedropper.com/eboardswitchv4)**

**NEW IMAGE WITH SEPARATE RESISTORS FOR GATES:**
<img src="/uploads/db1493/original/2X/3/3f1ca98645484e5918794a4a5dd914460447b853.png" width="587" height="449">
```

---
## \#46 Posted by: JdogAwesome Posted at: 2016-08-20T18:18:11.148Z Reads: 306

```
Here is the IRFS7530-7P I was talking about. Obviously very similar to the other ones but it accommodates a D2PAK 7-P package MOSFET. Its not done yet I think theres some things I would change but yeah. And this would obviously have a strange mismatch of SMD and normal components, which would mean the fet would be on one side and everything else on the other. Also it took me a while to find a D2PAK lbr file for Eagle but [HERE](https://github.com/triffid/BLDC/blob/master/D2PAK-7.lbr) is the link to the Github file if your interested.

**EDIT: UPDATED IMAGE**
<img src="/uploads/db1493/original/2X/7/796e4c6e561f157502deb12323804b8ace595409.png" width="489" height="500">
```

---
## \#47 Posted by: JdogAwesome Posted at: 2016-08-21T00:53:52.828Z Reads: 303

```
I also made a schematic with 2 D2PAK MOSFET's in it, cause why not. Below is an image of the 2x D2PAK schm and in the file there is the single D2PAK schm as well.

**.Zip Download [HERE](http://www.filedropper.com/eboardswitchv5v6_1)**

**NEW IMAGE WITH SEPARATE RESISTORS FOR GATES:**
<img src="/uploads/db1493/original/2X/1/1107dc3df7641d953b9da54d93349ebdbfa5624e.png" width="497" height="500">
```

---
## \#48 Posted by: JdogAwesome Posted at: 2016-08-24T05:27:33.019Z Reads: 291

```
Managed to make the original switch WAY smaller, now it comes in at only 48mm x 28mm! 

<img src="/uploads/db1493/original/2X/c/cad40263c5e45be783387244daac7cf1a1970114.png" width="630" height="405">
```

---
## \#49 Posted by: JdogAwesome Posted at: 2016-08-24T06:03:59.759Z Reads: 286

```
And obviously re-did the IRFB7530-7P board as well. And its even smaller than the previous one!

<img src="/uploads/db1493/original/2X/8/8da1a26f3d35282b478e9a1c9766f1362012d963.png" width="525" height="315">
```

---
## \#50 Posted by: DeathCookies Posted at: 2016-08-24T06:17:28.811Z Reads: 271

```
Why does it only handle about 30-60A ? The FET is rated to 295A.
What do i am overlooking?
```

---
## \#51 Posted by: JdogAwesome Posted at: 2016-08-24T06:31:41.707Z Reads: 275

```
Lol, so the max rating on a MOSFET is usually COMPLETE AND UDDER BULLSHIT. By that i mean like the TO-220 package leads will melt at around 75A so that's out the window right there. And doing the math at 30A your going to see around a 94C degree temp rise on the 7530 which is fine but much higher and its gonna start to get sketchy. I heard that they literally COOL the IC's in non conductive boiling liquid to test the max amperage, so yeah unless your planning on doing that, then don't even worry about the supposed "max amperage" for the MOSFET, do the heat calc your self and figure out a safe operating amperage, or Google it and you'll figure out the true max safe amperage.
```

---
## \#52 Posted by: DeathCookies Posted at: 2016-08-24T06:39:40.342Z Reads: 275

```
I am just curious because the "[Vedder Anti Spark Switch](https://github.com/vedderb/SparkSwitch)" is kinda standard but no one said that it is maxed to 60A... So the Vedder Switch cannot handle more than 60A? Somehow i doubt it but i am glad if somebody can enlighten me ;)
```

---
## \#53 Posted by: JdogAwesome Posted at: 2016-08-24T06:48:58.335Z Reads: 274

```
Well this [Vedder Switch](http://www.electric-skateboard.builders/t/anti-spark-switch-kit-extras-for-sale-vedders-v1-3/384) which is another great one and I highly recommend you take a look at, uses a 40A fuse on the positive rail which pretty much means, a 40A limit for the switch. I think it could possibly handle ~45A without a heat sink but I wouldn't risk. And like I said just do the heat calculations because that is your main problem, heat generation and dissipation.
```

---
## \#54 Posted by: lowGuido Posted at: 2016-08-24T06:54:18.373Z Reads: 267

```
295A rating?? LOL did they get hobbyking to do their data sheets?

50A MAX
```

---
## \#55 Posted by: DeathCookies Posted at: 2016-08-24T07:00:04.274Z Reads: 275

```
Mhm... how much does a heatsink help?
What else can i do to increase the amperage rate of the switch?


**EDIT:** i am a fool.... yeah it can handle 50A max at 12S (or whatever voltage) so the rate is more than enough. Correct?
```

---
## \#56 Posted by: lowGuido Posted at: 2016-08-24T07:01:57.414Z Reads: 266

```
im fairly sure vedders switch uses 2 FETS so that makes a theoretical 100A max
```

---
## \#57 Posted by: JdogAwesome Posted at: 2016-08-24T07:07:05.177Z Reads: 268

```
Well yeah 50A would be definitely near its limit and it would be getting damn hot though I think it would work (haven't done the equation, I'm tired.)  anyways most EBoards don't draw 50A continous so its not a big deal and if you did need to draw 50A cont, you'd be better off using 2 fet's in parallel like my dual fet schematics. Also heatsinking does help a lot though its still not fixing your under lying problem of drawing to much current from your fet.
```

---
## \#58 Posted by: DeathCookies Posted at: 2016-08-24T07:22:19.946Z Reads: 272

```
I just had a wrong calculation... The motor can pull up to 80A so i thought this switch wont work but i forget that the battery does not provide 12S @ 80A!

Thank you very much ;)
```

---
## \#59 Posted by: JdogAwesome Posted at: 2016-08-24T09:27:35.390Z Reads: 260

```
Yeah no problem. The motor can draw upwards of 100A+ on its first start up though that is for an extremely small amount of time and the switch could handle that perfectly.
```

---
## \#60 Posted by: DeathCookies Posted at: 2016-08-24T11:24:28.019Z Reads: 284

```
I am still confused somehow....

The battery provides 44,4V  (12S) with a rather low amperage. Thus it will not melt the 40A fuse.
Now i remembered that @hummie and @devin have measured some data:

[quote="devin, post:56, topic:6753"]
46.92V average
44.1 amps peak
4.92 amps average
[/quote]

This is the part where i get confused. The wattmeter is between the battery and the ESC so the amps peak should have blown a AntiSparkSwitch!?

It would be alright to setup the VESC battery max = <40A and the motor to 80A?
It would be the same acceleration/torque if battery max is at 40A instead of 80A?

Thanks in advance for enlighten me!
```

---
## \#61 Posted by: mason Posted at: 2016-08-24T12:23:40.898Z Reads: 251

```
I got parts for 3 of these and am having issues with all of em. I'll keep diagnosing.
```

---
## \#62 Posted by: JdogAwesome Posted at: 2016-08-24T12:35:12.156Z Reads: 256

```
Parts for 3 Vedder Switches? If you figure out what's wrong make sure to drop that in the Vedder thread to benefit others. Also a good place to deal help would be that thread as well.
```

---
## \#63 Posted by: JdogAwesome Posted at: 2016-08-24T12:39:51.798Z Reads: 262

```
Personally I don't have a VESC, wish I did though, so I can't tell you exactly how the VESC would behave but, escalating the max amperage can give you more torque because like I said when the motors first start up they draw a lot of current and the VESC may limit that because you set it to 40A max so it would be better to set it higher in that case. Though like I said I don't know to much about the VESC so I'm not the right person to ask sorry. And the reason the fuse doesn't blow is because its drawing that current for a very short amount of time so the fuse doesn't have enough time to heat up and break.
```

---
## \#64 Posted by: JdogAwesome Posted at: 2016-08-24T12:53:06.676Z Reads: 272

```
I was reading more about paralleling MOSFETS  and you can't use one resistor for the same gates of the MOSFET's because they will "fight" over the voltage for the gate capacitance so I have to go and change that on the dual fet circuit's. 

EDIT: Updated images, schm and brd files to accommodate this change.
```

---
## \#65 Posted by: mason Posted at: 2016-08-24T16:09:14.900Z Reads: 272

```
Yep! Will do.
```

---
## \#66 Posted by: JdogAwesome Posted at: 2016-08-28T01:40:17.258Z Reads: 294

```
Dual IRFB7530 version with 12V LED push button integration.

<img src="/uploads/db1493/original/2X/5/56fc3fc48aecd1899c0300cb1d8c3dcd33ccdc5a.png" width="595" height="460">
```

---
## \#67 Posted by: JdogAwesome Posted at: 2016-09-07T22:06:44.509Z Reads: 290

```
## **!!!VERY IMPORTANT NOTICE!!!**

The gate resistors for the MOSFET('s) can not always be just 10K resistors! I was originally doing this and its wrong! The 2 resistors act as a voltage divider for the gate but you have to make sure the voltage is not over the Vgs max of the MOSFET. For a 12S build you will need a 24-32K Ohm resistor on the positive side and a 10K on the negative side of the voltage divider. For a 10S build 18-25K Ohm on positive side and 10K on negative. For an 8S build 2x 10K's would be fine but a 12K on the positive side would be better. 6S Build two 10K's are fine as well. You can also use a mismatch of different resistor values using a [Voltage Divider Calculator](http://www.ohmslawcalculator.com/voltage-divider-calculator) to calculate the required values, just don't use any resistors under ~1K Ohms. I put an example below so you can get a better understanding.

USING A 12V ZENER DIODE TO DRIVE THE GATE WOULD BE BEST! Using a 12V Zener would mean the gate always gets 12V no matter what the voltage is, as long as it's above 12V obviously.

<img src="/uploads/db1493/original/3X/2/a/2aa1db2dd74cc9ba5b09acd0be0a439594f5a960.jpg" width="690" height="363">
```

---
## \#68 Posted by: Chicagojoshua Posted at: 2016-09-08T19:24:05.953Z Reads: 274

```
Dude I am totally interested in one of these. I have a 13s 3p lithium battary pack that I made myself for a single drive motor. What is my cheapest option for one of your switches?
```

---
## \#69 Posted by: sl33py Posted at: 2016-09-08T19:41:02.179Z Reads: 271

```
@Chicagojoshua - 13s is going to be tough to find an ESC that will work.  Most max at 12s.  Not sure if the mosfet switch will also be limited to 12s max?
```

---
## \#70 Posted by: JdogAwesome Posted at: 2016-09-08T19:44:22.882Z Reads: 275

```
Hey @sl33py my switch uses the IRFB753PPbF MOSFET which has a max voltage of 60V so you could technically use a 14S battery. Also most components that have a max of 12S can probably handle 13S-14S just because not many parts have a max voltage of above 50.4V(12S full charge) and below 60V so usually there max is 60V, not much in between.
```

---
## \#71 Posted by: Chicagojoshua Posted at: 2016-09-08T19:56:15.270Z Reads: 264

```
Ok, 

    So which switch do you recommend and how much will it cost me for the LED push button version you make?
```

---
## \#72 Posted by: JdogAwesome Posted at: 2016-09-08T19:58:48.072Z Reads: 259

```
Well its up to you on which one you want. Either one will work for your single drive setup though the dual MOSFET one that's $35 instead of $25 will future proof you more because you'll be able to use it with a dual drive setup if you ever decide to go that route. If you want the LED Pushbutton its an additional $10 so for the single FET switch it will be $35 and the dual would be $45 though like I said my prices are negotiable.
```

---
## \#73 Posted by: Chicagojoshua Posted at: 2016-09-08T20:56:18.634Z Reads: 252

```
I will purchase two... one a single drive and another for a future dual drive both with the push button LED. Whats the best price you can quote me?
```

---
## \#74 Posted by: 2-alex-2 Posted at: 2016-09-08T21:18:36.967Z Reads: 251

```
How much for just a blank pcb posted to uk ? Single 6s setup
```

---
## \#75 Posted by: JdogAwesome Posted at: 2016-09-08T21:21:16.247Z Reads: 273

```
A blank PCB for one of the switches? No components just the PCB right? I guess I could send one to you, ive never shipped internationally before so I dont know how much it would be though. I custom make all my PCB's using a laser printer but you could try using the Toner Transfer method to make one yourself and it would be quite a bit cheaper.
```

---
## \#76 Posted by: dstnceswmer Posted at: 2016-11-17T04:45:16.703Z Reads: 252

```
I was wondering if someone could double check me on my switch drawing. Should be essentially the same as @JdogAwesome made.

<img src="/uploads/db1493/original/3X/3/2/32f9f928ea70bc8be618b494a7ed86d23b851252.png" width="690" height="485">
```

---
## \#77 Posted by: JdogAwesome Posted at: 2016-11-17T05:05:00.056Z Reads: 237

```
Looks good though you'd be a lot better off using a 12V Zener Diode's to drive that MOSFET gate as it's more stable at different voltages, other than that looks great!
```

---
## \#78 Posted by: dstnceswmer Posted at: 2016-11-17T14:36:59.843Z Reads: 235

```
Cool, appreciate the tip! Also I believe you may have told me a while back But I'm still confused on the purpose of the diode (1N5404) I believe you (or maybe it was someone else) said it had to do with the regenerative breaking? But how does it help / what exactly does it do?
```

---
## \#79 Posted by: Blasto Posted at: 2016-11-17T15:50:22.712Z Reads: 238

```
[quote="JdogAwesome, post:14, topic:5738, full:true"]
Hey ndwallick the diode is an essential part of the circuit. The diode lets buildup current flow from the - to the + lead which is the opposite of the way current normally flows, this is because of an electron buildup that can occur and destroy a circuit if a diode is not there to let the electrons flow back. Anyways, its a very important part of the circuit and if you were asking to see whether or not you need the diode, the answer is a definite yes, lol. Though thank you for asking the question so now others will know!
[/quote]

@dstnceswmer he is using it as a flyback diode

https://en.wikipedia.org/wiki/Flyback_diode
```

---
## \#80 Posted by: dstnceswmer Posted at: 2016-11-17T18:57:23.792Z Reads: 235

```
So here is an updated pic with a zener diode being used, and two schottkey diodes added in line with the charger to prevent any possibility of a reverse polarity charger damaging anything. Also made the picture more accurate in that there is a barrel plug for the charger. Everything looking good? <img src="/uploads/db1493/original/3X/7/a/7aba1f138d132c420bf3ff1701030f2f3a49c2dd.png" width="690" height="485">
```

---
## \#81 Posted by: jmasta Posted at: 2016-11-17T20:08:09.298Z Reads: 211

```
A single 7530 MOSFET is not going to be enough for 60A continuous 

In addition, most anti-spark switches have a capacitor and resistor in series, connecting the gate to the drain. It's my understanding that this is what limits the inrush of current to the ESC's caps, preventing the spark
```

---
## \#82 Posted by: dstnceswmer Posted at: 2016-11-17T20:13:08.481Z Reads: 216

```
? The data sheet I have says that it is rated at 195A Continuous drain current at a 10V Vgs. So why wouldn't one be enough?

http://www.infineon.com/dgdl/irfs7530pbf.pdf?fileId=5546d462533600a4015364c3d98429c3
```

---
## \#83 Posted by: jmasta Posted at: 2016-11-17T20:21:28.108Z Reads: 237

```
<img src="/uploads/db1493/original/3X/7/7/779c6801159594b2f79e41341d2bfb5000a0b049.png" width="597" height="500">

You want to keep the power dissipation to around 1 W per FET.  With a single 7530, you would be dissipating 4-5 W at 60A.  A single 7530 should really only be used up to 30A continuous, and even that is pushing it a bit.  Otherwise you need to incorporate passive or active cooling
```

---
## \#84 Posted by: JdogAwesome Posted at: 2016-11-17T20:28:40.497Z Reads: 222

```
@jmasta @dstnceswmer A single FET is fine for your use. Your board only draws around 20A nominal with peaks UpTo around 80A but that's for a very short amount of time and it can handle it fine. @jmasta about the capacitor resistor on the gate to limit inrush current thing, no you should not do that. I was talking to some very smart electricians on Stack Exchange and they were saying it isn't healthy for FET's. Also inrush current doesn't matter because it's a MOSFET so there is no sparking and they can handle extremely brief high inrush current no problem.  Also I've been using a single 7530 FET as a switch for my board for a while and it works, so yeah.
```

---
## \#85 Posted by: dstnceswmer Posted at: 2016-11-17T20:30:58.710Z Reads: 217

```
Ok, I was just going to say the same thing regarding not needing 60A continuously, just wasn't sure how much I'd actuall be drawing. How exactly did you figure approximately 20A? Just curious as to what calculations would be used.
```

---
## \#86 Posted by: dstnceswmer Posted at: 2016-11-18T04:55:09.584Z Reads: 208

```
Also, looking at barrel jacks for the charging port. Only problem is they seem to be all rated for only 12V. Will this be a problem?

ie. https://www.digikey.com/product-detail/en/mpd-memory-protection-devices/EJ501A/EJ501A-ND/2439531
```

---
## \#87 Posted by: JdogAwesome Posted at: 2016-11-18T05:27:20.470Z Reads: 221

```
No it shouldn't be a problem. Im using [this](http://www.ebay.com/itm/381603862436?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT) connector because it comes with a waterproof cover which will be very useful. And for the male connector im using [this](http://www.ebay.com/itm/371462338310?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT).
```

---
## \#88 Posted by: wuwica Posted at: 2016-11-22T04:30:36.908Z Reads: 233

```
Hey, long time forum lurker here, gotta thank you for the schematic for the switch - it was a ton of fun building.  Two things though, I want to double check a few things with the switch i built:

1st, is it even right?  I don't have much experience with circuits and a second pair of eyes always helps.

2nd is this where I should solder on those zener diodes? 

<img src="/uploads/db1493/original/3X/3/2/324e64ce108343ce594a3d61915915270ef86ffe.jpg" width="500" height="500"><img src="/uploads/db1493/original/3X/8/3/835c0a889e4a233d194ac03eef4ad786c6fbb578.jpg" width="500" height="500">

please excuse my crummy soldering job :sweat:
```

---
## \#89 Posted by: JdogAwesome Posted at: 2016-11-22T05:09:08.485Z Reads: 226

```
Hey @wuwica your circuit looks great especially for a perfboard one lol. Its a little hard to tell what exactly is going on in the pics just because of the nature of it being a perfboard circuit but as long as it follows the same principles and has the same connections as my circuit below it should work just fine. 
<img src="/uploads/db1493/original/3X/c/a/ca3003d4441cccea0bf0751c06c84ac293b77bd5.jpg" width="681" height="500">
```

---
## \#90 Posted by: JdogAwesome Posted at: 2016-11-22T05:15:13.343Z Reads: 217

```
Heres another pic of an actual board I made for a customer that uses that same circuit I posted above.
<img src="/uploads/db1493/original/3X/7/e/7eb5f9a0020c6eb537d3b0886e778bebb92ec613.jpg" width="690" height="388">
```

---
## \#91 Posted by: kyo Posted at: 2016-11-22T07:34:51.715Z Reads: 208

```
Hi, love your drawing, Does it work? did you actually do it? and is the battery indicator on when you charge your board( while the SPDT switch is off) ??
```

---
## \#92 Posted by: JdogAwesome Posted at: 2016-11-22T11:40:22.585Z Reads: 209

```
@kyo I can at least tell you that when it is charging the battery monitor will not be illuminated because it comes after the MOSFET in the circuit.
```

---
## \#93 Posted by: dstnceswmer Posted at: 2016-11-22T16:45:12.554Z Reads: 208

```
@kyo Thanks :), I am in the process of building it at the moment and testing it. Still waiting on a few parts to come in from digi key. I'll update when I have a few results.
```

---
## \#94 Posted by: JdogAwesome Posted at: 2016-11-22T17:44:16.340Z Reads: 206

```
@dstnceswmer hey for the MOSFET's I actually just bought them from a website called Arrow and there half the price of Mouser or Digi-Key. They also ship from within the US and shipping is free! It was $16 for 10 FET's. https://www.arrow.com/en/products/irfb7530pbf/international-rectifier
```

---
## \#95 Posted by: kyo Posted at: 2016-11-23T01:58:50.707Z Reads: 207

```
Hey guys, @JdogAwesome , @dstnceswmer thanks for your input. I am thinking ab a senario that battery indicator will be turned on or off accordingly to the switch and charging port. What i mean is that when turn on or off the board by the switch, batt inducator turns on off accordingly, we can do this already, and when we charge the board by plug in a charger, can the battery indicator turns on or off accordingly ?? Can we do that?
```

---
## \#96 Posted by: dstnceswmer Posted at: 2016-11-23T02:15:03.334Z Reads: 211

```
my switch in the drawing should only be on when the board is turned on (when motor/VESC is connected to the battery). When the board is switched off the battery monitor will also be off. This is because the negative lead of the monitor is connected to the drain of the fet, same as the motor. So when the FET is off there is no connection of the negative  wire in either the motor or batt monitor to the ground of the battery.
```

---
## \#97 Posted by: wuwica Posted at: 2016-11-23T02:16:53.526Z Reads: 218

```
Cool, you've been a great help
<img src="/uploads/db1493/original/3X/5/b/5ba84dc7f7eb2286b1d44eca835c0acd7988fdc0.jpg" width="500" height="500">
 I just gotta plug the ESC and wire in a charging port.

Thanks again ☺
```

---
## \#98 Posted by: dstnceswmer Posted at: 2016-11-23T02:20:07.924Z Reads: 209

```
dang wish I saw this earlier lol. I actually just ordered 5 from digi key today for like $20 :(. I did go with a slightly cheaper one than the 7530'standard though.  I went with IRFB7534PBF. The specs seen nearly the same as the 7530's. Also I'm gonna be putting two in parallel just to err on the side of caution
```

---
## \#99 Posted by: wuwica Posted at: 2016-11-23T21:31:27.418Z Reads: 209

```
I set up a push switch before my battery indicator, and I'd just press the button whenever I want to check the charge. I'd imagine it'd be doable if you have a 3 pin dc connector (tip, sleeve, shunt) and a transistor to check when the dc jack is plugged in.  
http://i.stack.imgur.com/tcQ8n.png

pin 3 disconnects when a jack is plugged into the connector.

My knowledge of electronics is only ankle deep so I cant really think up a schematic for it :disappointed_relieved:.
```

---
## \#100 Posted by: dstnceswmer Posted at: 2016-11-23T22:21:43.401Z Reads: 194

```
Oh didn't realize @kyo also wanted to have in indicator turn on based on the charging plug. In that case, yes @wuwica that sort of connector would do the trick.
```

---
## \#101 Posted by: kyo Posted at: 2016-11-24T02:37:14.587Z Reads: 194

```
@wuwica , @dstnceswmer, thanks for the input but It is not that easy, I've already looked into this, and dont know how to do it, that's why i asked in the first place.

@wuwica    this kind of dc jack is mostly used for radio that use both plug in dc power and battery but not at the same time.  reason this dc jack can not be used for my purpose  :  when plug in, tip2 would bend out a bit just enough for tip3 lost contact at that black arrow(ur pic above). but we need contact to get the voltage, so this is not gonna work. Unless we use something similar to e-switch, i think.

btw, my knowledge of electronics is very short too. Maybe i missed something. 

<img src="/uploads/db1493/original/3X/1/d/1df84411736485efde10527bd45fa996783e708a.png" width="240" height="92">
is this pic right with the label?
```

---
## \#102 Posted by: wuwica Posted at: 2016-11-24T04:54:00.351Z Reads: 190

```
Yea that picture is labeled right, and I meant to use the transistor gate to take in a connection from the tip shunt.

When a dc jack is plugged into the connector the tip shunt will disconnect and will allow the drain/source to be connected.  I was only assuming this would work so I just brought up the possibility.  I'd use the transistor as a switch.
```

---
## \#103 Posted by: kyo Posted at: 2016-11-24T05:11:02.316Z Reads: 191

```
yeahh that's what i had in mind too, it's a e switch all over again, but this time is for battery indicator :D
```

---
## \#104 Posted by: JdogAwesome Posted at: 2016-11-24T05:35:36.575Z Reads: 192

```
@kyo @wuwica @dstnceswmer I feel like your guys are making it to complicated lol. I think what would be easier is just having a push button connected to you battery so you can check your battery whenever you need.
```

---
## \#105 Posted by: dstnceswmer Posted at: 2016-11-24T15:43:22.998Z Reads: 190

```
Agreed. I just plan on having my indicator turn on with the board as per my original drawings. not sure why you would care if it's on when the charger is plugged in?
```

---
## \#106 Posted by: DeathCookies Posted at: 2016-11-28T13:25:44.878Z Reads: 187

```
It would be nice if you could update your first post:

- download url (newest version)
- post 67 (gate resistor)
```

---
## \#107 Posted by: JdogAwesome Posted at: 2016-11-28T13:40:35.385Z Reads: 182

```
I wish I could, it's been to long since I posted it for me to edit it sorry.
```

---
## \#108 Posted by: DeathCookies Posted at: 2016-11-28T13:42:14.109Z Reads: 185

```
hahaha :smiley:
that's nasty...
```

---
## \#109 Posted by: dstnceswmer Posted at: 2016-11-29T00:12:54.632Z Reads: 175

```
Is that 47k resistor just a pulldown from the Gate I assume?
```

---
## \#110 Posted by: JdogAwesome Posted at: 2016-11-29T00:30:20.347Z Reads: 178

```
Exactly, just makes sure the gate drains when you power down the circuit. And the reason its such a high value is so it doesn't affect the gate voltage as a voltage divider.
```

---
## \#111 Posted by: dstnceswmer Posted at: 2016-11-29T00:31:43.349Z Reads: 185

```
Ok, yeah I had built most of my switch and was just contemplating why I didn't have a pull down for that exact reason, thanks!
```

---
## \#112 Posted by: JdogAwesome Posted at: 2016-11-29T00:34:05.886Z Reads: 204

```
@dstnceswmer Also, an update on my order for the 10x IRFB7530 MOSFET's from Arrow they just arrived today and at first glance they look very nice, but the packaging was a bit overkill lol.

<img src="/uploads/db1493/original/3X/d/4/d4d887817d61c6863420a5da3ae50d4674da6c75.jpg" width="690" height="299">
<img src="/uploads/db1493/original/3X/8/b/8b3505f277eac4daccb4580ee3c567ada988a7e9.jpg" width="690" height="388">
```

---
## \#113 Posted by: dstnceswmer Posted at: 2016-11-29T19:36:52.000Z Reads: 199

```
@JdogAwesome If your switch is 12V rated how is it ok to be using in your configurations? the way I see it (even at 10s) the potential across the switch is (Vbatt-12V) = (42-12)=30V > 12V
```

---
## \#114 Posted by: JdogAwesome Posted at: 2016-11-29T19:51:28.535Z Reads: 199

```
The switch is rated at 12V because the LED has the proper current limiting resistor for 12V that's the point of the two 4.7K resistors is to add to that current limiting resistor. Just because a switch says it can handle 12V doesn't mean it can't handle higher voltages, to an extent.
```

---
## \#115 Posted by: dstnceswmer Posted at: 2016-11-30T17:10:07.443Z Reads: 205

```
So I've been running a few simulations in LTspice and from what I can tell, the led in my rocker switch is going to be screwing with my gate voltage on my FETs. Best I can guess is that inside the switch is an led in series with a 500ohm resistor (that would make it 12V tolerant) the cathode end of this is tied to the switch ground while the anode is connected to the center tap. Problem is that this small 500 ohms negates the affects of my zener and acts as a voltage divider with my current limiting 10k, effectively giving me a smaller than desired gate voltage. Below is the schematic I have been simulating. Any thoughts?

<img src="/uploads/db1493/original/3X/b/e/be9a40fe289590fb34b8c3ed6fea204e53253c61.png" width="690" height="208">
```

---
## \#116 Posted by: JdogAwesome Posted at: 2016-11-30T17:40:53.205Z Reads: 192

```
Your definetly right that the LED would affect the gate voltage. Though you shouldn't be running anything off the gate anyway. The way I have it setup is so the LED terminals have there own channel with the two 4.7K resistors. Though with your rocker switch your saying there connected to the terminals right? The switch I use has separate terminals for the LED light, and terminals for the contacts.
```

---
## \#117 Posted by: dstnceswmer Posted at: 2016-11-30T17:48:08.535Z Reads: 197

```
> Though with your rocker switch your saying there connected to the terminals right?

Yup that's exactly what I was saying. It's just an automotive rocker w/led. I can see how having the led on a separate terminal would work. looks like my options are:
1. See if I can crack open the switch and re-route the led anode
2. Buy a new switch with broken out separate terminals
3. Use some sort of 12V step-down regulator as gate/LED power supply instead of zener diode (prob. over complicating things)
```

---
## \#118 Posted by: JdogAwesome Posted at: 2016-11-30T18:00:25.122Z Reads: 195

```
1. I'd say thats nearly impossible to do without just destroying the switch.
2. I'd recommend you do that, link below is the switch I use and it works very well.
3. Yeah I think that's definetly over complicating things.

https://www.amazon.com/gp/aw/d/B00ZR7MMXO/ref=yo_ii_img?ie=UTF8&psc=1
```

---
## \#119 Posted by: dstnceswmer Posted at: 2016-11-30T18:50:00.872Z Reads: 196

```
1. so actually quite easily popped off the top of the switch and was able to seperate the led annode from the switch center tap. just as I suspected, was just a 500ohm res/led in series. So that's a viable option. 
2. I do however like the look of the switch you linked (thanks)
3. yeah not doing that :stuck_out_tongue:
```

---
## \#120 Posted by: ayospringroll Posted at: 2016-11-30T20:18:38.350Z Reads: 198

```
Hey, this is a nice thread! 
I dont know if I missed it while reading this but is using one mosfet like in this diagram enough to power off/on a 6s 22.2V circuit on my board? Also if it is do you mind sharing a link where I can download the printout to try and make my own PCB? 
Thank you!
```

---
## \#121 Posted by: JdogAwesome Posted at: 2016-12-03T05:53:21.137Z Reads: 181

```
Hey @ayospringroll a single FET is definitely enough to tun a 6S build, I am personally running 6S and I only use a single FET. [Here](http://www.filedropper.com/eboardswitchsinglemosfet) is a link to download the .brd and .sch files to open in Eagle.
```

---
## \#122 Posted by: PXSS Posted at: 2016-12-23T07:09:53.624Z Reads: 180

```
Is your switch on a pcb or perf board??? Interested in buying a 50A one or the kit to solder myself
```

---
## \#123 Posted by: JdogAwesome Posted at: 2016-12-23T07:40:43.540Z Reads: 180

```
My switches come on PCB's, if your interested in buying one PM me. I will have nice OSH Parks boards hopefully within the next week as well.
```

---
## \#124 Posted by: IsTalo Posted at: 2017-02-05T15:45:35.090Z Reads: 175

```
Hello, could I use this [Mosfet](http://br.mouser.com/ProductDetail/STMicroelectronics/STP60NF06/?qs=RC432zO33OoItaZuWNLfaw%3D%3D) ?
```

---
## \#125 Posted by: JdogAwesome Posted at: 2017-02-05T16:32:09.948Z Reads: 180

```
No, that MOSFET has a very high RDSON of 16mOhms compared to the 7530 of around 1-2mOhm.
```

---
## \#126 Posted by: IsTalo Posted at: 2017-02-05T16:40:21.961Z Reads: 179

```
Ah Okay, Can you explain to me what is a gate button? I'm from Brazil and It's a bit difficult to me to understand everything
```

---
## \#127 Posted by: anoop54 Posted at: 2017-03-06T21:08:58.634Z Reads: 166

```
Hey I saw your schematic for this and wanted to ask why we use a diode parallel to a mosfet, Is this to protect the mosfet from any voltage coming back from esc? or well current.
```

---
## \#128 Posted by: JdogAwesome Posted at: 2017-03-06T21:47:47.232Z Reads: 167

```
Hey @anoop54, yeah you've pretty much got it, the diode is to protect against reverse voltage and current spikes resulting from the magnetic field collapsing in the coils/windings of the motor. Anyways, short story is yeah you definetly need a diode to protect the FET.
```

---
## \#129 Posted by: Jammeslu Posted at: 2017-03-08T20:13:04.678Z Reads: 161

```
Just a quick question, why won't it work to put a high amp breaker 50A at the very end of a xt90 antispark cuz in that way you just switch the toggle to turn on with no spark
```

---
## \#130 Posted by: respy66 Posted at: 2017-04-18T13:03:52.368Z Reads: 157

```
@JdogAwesome hey could you help me with a little bit simpler layout im a bit confused but if you made a clearer diagram I would appreciate that 
Thank in advance
```

---
## \#131 Posted by: JdogAwesome Posted at: 2017-04-19T00:10:49.336Z Reads: 157

```
Hey @respy66 yeah I'll try making a clearer diagram,. It if you could let me know what exactly your finding confusing that would be great! It's a pretty simple circuit pretty much just 2 MOSFETs in parallel that are turned on and off via a switch. All the other zeners and resistors are for driving the gate at 12V.
```

---
## \#133 Posted by: respy66 Posted at: 2017-04-24T16:24:12.869Z Reads: 150

```
@JdogAwesome colud you give me a design of the pcb with only the routing and pads I'd like to etch my own pcb
```

---
## \#134 Posted by: chapatte Posted at: 2017-04-25T08:29:45.708Z Reads: 147

```
Hey @JdogAwesome congrats on your work for the switch !
  I'm also trying to put together a switch for a 6S setup with two IRLB3034 -N in parallel, Would you mind uploading the PCB design so that I (we) can etch a PCB.

Second question is : since I'm building the switch for a 6s setup, Should I swap the 2.2k and 47k resistors at the gate with a 10kand use 4.7k to power the led, the button and the butten LED?

Thanks A LOT !

PS: I know its my first post, but i'm a loooong time lurker on this forum !
```

---
## \#135 Posted by: JdogAwesome Posted at: 2017-04-25T20:28:01.019Z Reads: 144

```
@chapatte @respy66 hey guys thanks for your interest in my switch! Currently I dont have a good board design for the TO-220 package but I do have a schematic, which you can use to design your own board. I do however have a D2PAK design if you plan on using all SMD parts which ill upload as well. Just let me know if you'd like any more info or help! Download the files [HERE](https://drive.google.com/file/d/0BzLpefQ-7x-gd0xFY2lCT3h3Mms/view?usp=sharing).
```

---
## \#136 Posted by: chapatte Posted at: 2017-04-26T10:08:44.039Z Reads: 143

```
Thanks ! Unfortunately I kinda sucks at PCB design and I already have the parts for an "old" version of the PCB.
Do you still have the files for PCB pictured in post #89 ?
```

---
## \#137 Posted by: ryny24 Posted at: 2017-04-26T16:06:24.374Z Reads: 139

```
I'm confused on why there are two part numbers for the diode. 1N4004 & 1N5404. I purchased both, but which do I use?
```

---
## \#138 Posted by: JdogAwesome Posted at: 2017-05-04T00:17:28.423Z Reads: 138

```
@chapatte @ryny24 Hey guys sorry for taking so long to reply, for some reason I didnt get a notification via email which I normally do so I didnt notice your replys. 

@ryny24 About the diode mix up, you can use either of those diodes, however the 1N5404 can handle more current though its also a lot bigger, physically. 

@chapatte Hey yeah I do, but just make sure you use the resistor values from the other schematic I linked before and make all the high current traces a lot larger. Link [HERE](https://drive.google.com/file/d/0BzLpefQ-7x-gQ2ZNR0NBWERXVVU/view?usp=sharing)
```

---
## \#139 Posted by: chapatte Posted at: 2017-05-04T08:19:11.928Z Reads: 136

```
Exactly what I was looking for, thank you !
```

---
## \#140 Posted by: ryny24 Posted at: 2017-05-05T20:14:48.700Z Reads: 143

```
Thank you @JdogAwesome! My switch just arrived so I can play. Post #89 is a little hard to follow the left side, which I think is mostly a voltage divider for the switch LED?  I drew it out in a way I could read it easier. Does this look correct?<img src="/uploads/db1493/original/3X/9/e/9ebdd16fd8cd608a10e7d8f9e0b35f98ef02f9e7.png" width="690" height="310">
```

---
## \#141 Posted by: JdogAwesome Posted at: 2017-05-06T12:42:10.754Z Reads: 141

```
Hey Ryan, your schematic is correct except for the LED voltage divider. In my design there isn't a voltage divider, just a 4.7K or 6.8K current limiting resistor.
```

---
## \#142 Posted by: tonystark Posted at: 2017-05-08T22:02:43.865Z Reads: 133

```
hi, i have alot of IRF3205 laying around. data sheet says that it can deal with 80-110 Amps and 55Volts. I am using 8s3p battery pack.just want to make sure this fet will be fine?
```

---
## \#143 Posted by: tonystark Posted at: 2017-05-08T22:40:55.588Z Reads: 134

```
i am trying to open these links that you share but every time it takes me to a home page and there is no option to download something, only to upload. any suggestions? thanks
```

---
## \#144 Posted by: ryny24 Posted at: 2017-05-14T00:43:02.993Z Reads: 135

```
It works!!!!!!!! It actually works!!!!<img src="/uploads/db1493/original/3X/9/9/99b4f8d756fe5aa3d700d5b72e730ec1eead8752.jpg" width="375" height="500">

I owe each of you a beer. Thank you!
```

---
## \#145 Posted by: JdogAwesome Posted at: 2017-05-14T12:23:13.560Z Reads: 129

```
Looks great! Just make sure to put some heatshrink around it or something to give it a bit more protection. Also love that purple led!
```

---
## \#146 Posted by: dstnceswmer Posted at: 2017-06-14T21:56:13.939Z Reads: 126

```
could you elaborate more on this? I'm failing to see the issue using 1 zener+current limiting resistor to provide 12v gate voltage for both Fets.
```

---
## \#147 Posted by: lowGuido Posted at: 2017-06-14T23:19:40.424Z Reads: 123

```
@ryny24 can you tell me how much it cost you to build in components?
```

---
## \#148 Posted by: JdogAwesome Posted at: 2017-06-14T23:19:45.082Z Reads: 122

```
Hey @dstnceswmer to elaborate, from what I understand it's more of a issue with the gate capacitance and how you want the MOSFET's to turn on at around the same and they have trouble doing that drawing from a small supply, like a resistor. In this use case scenario I think you would be fine just using a single resistor zener combo, but having two separate gate drivers like that also gives you a failsafe in case one zener dies or something, would hate for your board to die whilst going down a hill. In any case you'd be fine just using a single zener. Hopefully that helps you out, if you have any other questions just let me know!
```

---
## \#149 Posted by: JdogAwesome Posted at: 2017-06-14T23:23:55.602Z Reads: 131

```
Yeah I actually have an entire spreadsheet of my prices for different switch combos, I'll drop that below. Also all my FET's and important components like diodes I get from Arrow.com so that I know there legitimate and have good specs. Things like resistors, zeners and LED'S I just get from eBay or whatever because there pretty basic components. 

Dual TO-220 Package
IRFB7530PbF: $3.10
PCB Cost: $5
12AWG Wire: $1
XT60: $.0.50
Small Parts: $0.50
Labor: My sanity

Total: $10.10
Profit from $35 Sale: $24.90
Profit from $30 Sale: $19.90

-------------------------------------------------

Dual TO-220 Package (WITH SWITCH)
IRFB7530PbF: $3.10
LED Pushbutton: $4
PCB Cost: $5
12AWG Wire: $1
XT60: $.0.50
Small Parts: $0.50
Labor: My sanity

Total: $14.10
Profit from $45 Sale: $30.90
Profit from $40 Sale: $25.90

-------------------------------------------------

Dual D2PAK-7
IRFS7530TRL7PP: $4.38
PCB Cost: $5
12AWG Wire: $1
XT60: $.0.50
Small Parts: $0.50
Labor: My sanity

Total: $11.38
Profit from $35 Sale: $23.62
Profit from $30 Sale: $18.62

--------------------------------------------------

Dual D2PAK-7 (WITH SWITCH)
IRFS7530TRL7PP: $4.38
LED Pushbutton: $4
PCB Cost: $5
12AWG Wire: $1
XT60: $.0.50
Small Parts: $0.50
Labor: My sanity

Total: $15.38
Profit from $45 Sale: $29.63
Profit from $40 Sale: $24.62
```

---
## \#150 Posted by: dstnceswmer Posted at: 2017-06-16T13:57:29.281Z Reads: 127

```
Ah ok yeah that makes sense, I'll prob go with two diodes for redundancy's sake as you suggested. I have been running my switch made up on perf board with just one gate voltage supply for a little while now, but am in the process of drawing up my schematic for a new pcb in kicad now. One other thing that I'm not totally clear on was your choice of using a 6.8k resistor for the LED in your lighted switch. I am getting one of those lighted PC latching switches as well and from what I can tell:

From switch specs: LED +12v, 15mA

My calculations show:
R = (+12v - Vd) / 0.015A
R+R' = (50.4V - Vd)/0.015A
(+12v - Vd) / 0.015A + R' = (50.4V - Vd)/0.015A
R' = [(50.4V - Vd)/0.015A] - [(+12v - Vd) / 0.015A]
R' = (50.4v -12v -Vd +Vd) / 0.015A
R' = 2560 ohms for 15mA @50.4V
R' = 2.2k should give about 17mA

So why so high with the 6.8k resistor on there?

here is a link to the switch I bought:
https://www.amazon.com/gp/product/B017KP67FY/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
```

---
## \#151 Posted by: JdogAwesome Posted at: 2017-06-16T16:15:21.812Z Reads: 123

```
[quote="dstnceswmer, post:150, topic:5738"]
I have been running my switch made up on perf board with just one gate voltage supply for a little while now
[/quote]

That's to funny I'm still running one of my very first single FET 3034 designs and it's been working great for me, lol. So pretty much the LED is rated at 12V at 15ma, MAX. Which means running it any higher than that will kill it eventually. Even if you ran the LED at like 2 ma it would still light up just not as bright. The problem with running it at 15ma from a 50V supply is that the resistor would need to dissipate around 800mW of power which means you would need a relatively beefy resistor and it would also just generate a lot of unnecessary heat. To be honest if your using a 10-12S setup I'd just use a 10K resistor, but because people using my switch designs use all different voltages I wanted to make sure it would still be relatively bright at the lower spectrums like 6S, so I chose 6.8K.
```

---
## \#152 Posted by: JdogAwesome Posted at: 2017-06-16T16:24:08.088Z Reads: 122

```
Also the switch you bought looks nice I use a very similar one. Pretty much you just want to use the C (common) and NO (Normally Open) contacts as normal switch contacts and then the + and - for powering the LED inside the switch. Just make sure to connect the - of the LED to the drain of the FET so it only turns on when the switch is on. Also in case you wanted to calculate how much heat your MOSFET will produce under load use this calculation. I simplified it and just labeled every value pretty much so just replace parts in it with your FET's values. 

Heat generation: 
20² * 0.009 = 3.6W at 20A

0.009 - Miliohm RDSON found on datasheet
20² - amperage squared
3.6W - heat generated in watts

Above Ambient Calc
0.68 * 62 = 42°C

0.68 - heat generation value in wattage from above calc.

62 - C/W - JUNCTION thermal resistance to ambient, found on MOSFET datasheet

42°C - Above Ambient temperature


175-42 = 133°C (271°F)

175 - Max package temp (also found on datasheet)

42 - Above ambient from previous equation

133°C (271°F) - max ambient air temp
```

---
## \#153 Posted by: dstnceswmer Posted at: 2017-06-16T16:32:19.547Z Reads: 116

```
Ok, yeah that makes sense, thank you for clarifying that for me :) Also I was curious, had you ever considered adding a 3rd led/zener to just drive that led on the switch at 12V? Seems to me that this would be another viable option, although again you may need a decently high rated resistor (~0.5W), possibly get away with a 1/4 W
```

---
## \#154 Posted by: JdogAwesome Posted at: 2017-06-16T16:35:15.362Z Reads: 122

```
Theoretically you could, but I see no point to doing so as a resistor would server the same purpose and you would need a big wattage zener. Also if you were thinking of using it as a small 12V source, no just no lol.
```

---
## \#155 Posted by: dstnceswmer Posted at: 2017-06-19T15:24:06.327Z Reads: 124

```
Cool again thank you for the advice. Below is the schematic for my switch. I will be using all SMD's except for the FET's which will be through holes as well as the barrel plug and through holes for soldering in battery/motor wires etc... Was wondering if someone could just give me a quick double check on this?
<img src="/uploads/db1493/original/3X/b/7/b78c47d7fbea4388a7d2d3f25c83a23c34f1ac3b.png" width="690" height="278">
```

---
## \#156 Posted by: JdogAwesome Posted at: 2017-06-19T17:55:17.104Z Reads: 114

```
Yeah everything looks good with your schematic, id just recommend changing the 47K pull downs to 10K, but you dont have to.
```

---
## \#157 Posted by: dstnceswmer Posted at: 2017-06-19T18:04:26.260Z Reads: 116

```
Awesome! thanks for the quick feedback. BTW I am also going to be designing a pcb for taking in CH1 and CH3 from the GT-2B and output LED headlight and underglow control via an on-board arduino. Again, I currently have it all working on my board now but it's a perfboard hodge podge mess with a rat's nest of wiring. I'll post some pics and schematics soon if anyone is interested.
```

---
## \#158 Posted by: JdogAwesome Posted at: 2017-06-19T18:09:15.444Z Reads: 115

```
Sounds awesome! Definitely post some pics and documentation about it, Ive heard of a lot of people interested in that kinda thing. Let me know if you need any help with either the Arduino Programming or any schematics, love that kinda stuff lol.
```

---
## \#159 Posted by: dstnceswmer Posted at: 2017-06-19T21:21:38.658Z Reads: 123

```
Will do. I'll probably post them in a different thread and link it in here (Keep this on topic with the switch). I already have the code pretty much sorted out, have been trying it on my board I am finishing up not and works quite nicely. Though I did have to upgrade the onboard regulator and shunt capacitor on the arduino pro-mini as the output from my 12v step down buck regulator (https://www.amazon.com/DROK-converter-Regulator-Modified-Transformer/dp/B00CGV5NT4/ref=pd_rhf_gw_p_img_1?_encoding=UTF8&psc=1&refRID=GZM7G94KRQWYH6ZEVCP5) was too noisy at turn on that it kept frying Arduinos. 

Also modified my schematic a bit, wen to SB5200TA for both my flyback diode and charger reverse polarity protection. I did this simply for ease of ordering 2x of the same component as opposed to having many different components. This shouldn't be a problem as it is rated at 200V and 5A correct?
http://www.digikey.com/scripts/DkSearch/dksus.dll?Detail&itemSeq=231034655&uq=636334845351356541

Also switching my pull down resistors to 20k and using 2x 20k parallel resistors for my switch LED current limiting. I chose to parallel the two 20k's in order to halve the power consumption by half on each one so that I could use 1/4W resistors and still have a decent safety margin on them, does this sound right? 
below is the updated schematic.
<img src="/uploads/db1493/original/3X/d/4/d42963d4df38237e7d21626ac84f2802f2c3a624.png" width="690" height="263">
```

---
## \#160 Posted by: dstnceswmer Posted at: 2017-06-27T13:52:54.496Z Reads: 113

```
@JdogAwesome 
Been working on my pcb layout and from what I've seen looking at some online calculators and such, the high current traces need to be massive to handle even 20A of current. I was wondering what kind of trace widths and copper weight you used in your pcb?
```

---
## \#161 Posted by: JdogAwesome Posted at: 2017-07-02T05:39:27.655Z Reads: 111

```
Hey Justin (I'm also a Justin lol) just now getting around to answering DM's and messages been really busy lately. I always use 2oz copper from Osh Park and I'm not sure exactly what my traces sizes are but using a calculator should give you a rough estimate, just remember to bump the ambient temperature rise to about 25C or else itll give a larger trace size. Also if you want to have smaller traces you could just have no solder mask on the traces and put a layer of solder on top of them to make them thicker. And your schematic from your last reply looks good!
```

---
## \#162 Posted by: Tomer Posted at: 2017-07-02T09:07:46.028Z Reads: 104

```
Hey @JdogAwesome, could you please re-upload the schematics and board files?
http://www.filedropper.com/eboardswitchallversions_1 seems to resolve to a blank page.

Thank you.
```

---
## \#163 Posted by: encore1906 Posted at: 2017-07-04T17:32:16.740Z Reads: 105

```
Hi I'm looking to purchase one of your connectors?  I would like one that looks like the one from Torqueboards but actually works...lol  How much do you charge @JdogAwesome  Do you have a website to order from?
```

---
## \#164 Posted by: JdogAwesome Posted at: 2017-07-04T17:53:22.075Z Reads: 113

```
Hey @Tomer [HERE](https://drive.google.com/file/d/0BzLpefQ-7x-gaEt1MFlhdXRPQWs/view?usp=sharing) is the link to my newest designs the "New Compact Switch" folder is my newest design which I will be selling. 

@encore1906 hey Encore thanks for your interest in my switch, which I think is what you mean by connector right? Anyways if you are, my switches cost $35 a piece and are the most compact on the market, from what I know. They also come with a blue LED push button as well as XT60's, just DM me if your interested! ATM the PCB's are still being fabricated so it could still be 2-3 weeks before I have them in stock. Pic below is what the finished PCB will look like if your interested. <img src="/uploads/db1493/original/3X/a/5/a5e414823640463c8706c3e68e5a8dc5a24d9a72.png" width="690" height="334">
```

---
## \#165 Posted by: encore1906 Posted at: 2017-07-04T18:07:28.498Z Reads: 111

```
@JdogAwesome I'm new to this platform and I don't see an option to be able to DM you.  Here is the type of setup I'm looking for.  Hope this helps.  What would be the total cost of this one.  I had a Torqueboard one but the power just stays on and won't shut off which is now not allowing me to plug things in without sparks. I'm needing a bullet connectors on one end and a XT90 connector on the other end like the images below.  Can you do this?<img src="/uploads/db1493/original/3X/7/e/7edfa220cfabce3c1c24898115773f77d553fdfa.jpeg" width="375" height="500">
```

---
## \#166 Posted by: encore1906 Posted at: 2017-07-04T18:08:05.350Z Reads: 110

```
@JdogAwesome <img src="/uploads/db1493/original/3X/3/b/3b631c3e94497e49dd74e606c13fb14d0f5cf477.jpeg" width="375" height="500">
```

---
## \#167 Posted by: encore1906 Posted at: 2017-07-04T18:09:10.325Z Reads: 115

```
@JdogAwesome <img src="/uploads/db1493/original/3X/d/e/de7cca367963ac887b699bf4eff66e62ee453c6b.jpeg" width="375" height="500">
```

---
## \#168 Posted by: Kaly Posted at: 2017-07-04T18:27:15.440Z Reads: 109

```
Hi 
Will this work on a 12S system ?
```

---
## \#169 Posted by: JdogAwesome Posted at: 2017-07-04T18:55:09.092Z Reads: 112

```
@encore1906 if you click on my name there should be a button that says "message" just click that. Anyways yeah I suppose I could do XT90's and bullets but id have to charge you like a small fee like $5 for the extra parts if thats ok. Also what size bullet connectors?

@Kaly Yup my switch should work from 6-12S LiPos, technically it could work with upto 14S (60V) but I wouldn't risk it, and not many people use batterys above 12S.
```

---
## \#170 Posted by: encore1906 Posted at: 2017-07-05T18:02:55.122Z Reads: 125

```
@JdogAwesome thats what I figured but I didn't see any Message button this is what I see.  That's fine I'm okay with the $5 extra for the parts. What is the max Battery Cell yours can take...10S, 12S??? But anyways I would like to go ahead and purchase your Power On/Off Switch with XT90 connector on the Out (+/-) side and 5mm bullet connectors on the In (+/-) side. So my total I'm looking around $40 correct? You can email me I'm ready to purchase.  I'll also give you a shout out on my YouTube channel (YouTube.com/CKid86)<img src="/uploads/db1493/original/3X/2/2/223ad6f3512b41c049219c64a50fbbd792817c2b.jpg" width="690" height="494">
```

---
## \#171 Posted by: JdogAwesome Posted at: 2017-07-05T18:27:05.034Z Reads: 130

```
Pic below should be how to message be, but anyways my switch can handle upto 12S technically 14S but I wouldn't push it that far. You said XT90's on the output and you mean the same type your old switch had on the pic you took? And ill put 5mm bullets on the inputs. Ill email you with some more info, also like I said my PCB's are still being manufactured so it could be 2-3 weeks before the switches are ready.  
<img src="/uploads/db1493/original/3X/b/c/bcfe07e398dbed5de39b4e1e0bf0476256fb7505.jpg" width="690" height="454">
```

---
## \#172 Posted by: encore1906 Posted at: 2017-07-05T18:40:17.733Z Reads: 130

```
@JdogAwesome okay sounds good...send me an email and we can discuss further there about payment...etc.  But yea you have the right idea about my setup I'm wanting. Send me an email and lets continue this convo.
```

---
## \#173 Posted by: JdogAwesome Posted at: 2017-07-07T19:51:24.068Z Reads: 117

```
**-------THREAD MOVED-------**

**Please leave questions and replys on this new thread from now on, thanks!**

**[LINK](https://www.electric-skateboard.builders/t/boom-jda-ebsc-switch-pre-order-boom-35-compact-eboard-switch/)**
```

---
