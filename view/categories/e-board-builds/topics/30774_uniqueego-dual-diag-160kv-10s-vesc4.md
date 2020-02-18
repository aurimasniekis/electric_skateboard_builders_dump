# UniqueEGo &#124; Dual Diag 160KV &#124; 10S &#124; VESC4

### Replies: 67 Views: 5362

## \#1 Posted by: scepterr Posted at: 2017-08-16T04:57:32.740Z Reads: 369

```
Hey guys, figured I'd start detailing my first complete DIY build. 
**Components**
**Deck:** Yuneec E-Go 2 Blue/Black, 12mm, eight layered composite wood, Canadian Maple
**Trucks:** Caliber II 50°
**Wheels:** 100mm MBS<img src="/uploads/db1493/original/3X/4/5/45e4dd88601269ea33824a0539251188d09d440e.jpg" width="269" height="250">
**Motor:** 6374 190kv Sealed from https://buildkitboards.com/collections/parts/products/6374-190kv-motor?variant=30211207493 <img src="/uploads/db1493/original/3X/5/3/538cc74ec4263f5c7aec70742ce4bc014331834a.jpg" width="188" height="250">
**Mount:** Carbon Fiber arm + C2 clamp from https://www.electric-skateboard.builders/t/motor-mount-for-caliber-ii-trucks-enertion-clones-aluminum-clamp-carbon-fiber-arm/30286
<img src="/uploads/db1493/original/3X/0/d/0d97bd6a5bfe0d03b01a9310e8fc67f2ca78e2d4.jpg" width="333" height="250">
**Gears:** 15/36 15mm kit from https://www.electric-skateboard.builders/t/15mm-wide-pulley-kits-and-individual-parts-wheel-pulley-motor-pulley-belts-and-hardware/27184
<img src="/uploads/db1493/original/3X/d/1/d109d0ab0742a867a7fb4ca7916dd212304ac67d.jpg" width="666" height="499">
**Battery:** Swappable 7S3P for range and 10S2P for speed, Panasonic 18650PF cells (using stock E-Go2 battery housing)<img src="/uploads/db1493/original/3X/d/f/df94a2d51465628884fff046d3f5033860e4ea5c.jpg" width="333" height="250">
**Remote:** Nano-X
**ESC:** VESC 4.12 with directfets for now and vesc6 shortly
Universal DIY AC&DC CCCV Charger:
<img src="/uploads/db1493/original/3X/a/5/a5da4a69269f675e356d310d8d91b2d58261f686.jpg" width="333" height="250">
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-16T05:09:45.756Z Reads: 321

```
7s3p vs 10s2p will get you similar range, better to just stick with 10s2p so you don't have to change VESC settings. What's the point of going to a Vesc 6 if you're already going to have 4.12's?
```

---
## \#3 Posted by: scepterr Posted at: 2017-08-16T05:12:05.215Z Reads: 308

```
FOC without worry :slight_smile:
I also might be able to fit 12S2P in the same housing :wink:
The 4.12s will eventually go to a couple extra ego2 motors i have once this board is done and I get the 6
I wanna try to make a dual wheel ego2 motor board after this one(diagonal dual) :yum:
```

---
## \#4 Posted by: markyoe Posted at: 2017-08-16T06:24:01.315Z Reads: 290

```
That charger is awesome! Did you build that yourself or just mod one? Can I ask how much it cost you? I'd like to do something like that myself.
```

---
## \#5 Posted by: chuttney1 Posted at: 2017-08-16T06:26:49.133Z Reads: 286

```
I'm more interested in why E-Go used 18650 PFcells rated at 10 amps.
```

---
## \#6 Posted by: scepterr Posted at: 2017-08-16T06:35:51.389Z Reads: 288

```
It's really simple to make, inside is a 42v 2A DC supply (upgraded currently to 5A), and the display is a UCTRONICS Numerical Control DC 6-55V to 0-50V 5A Step Down Stabilized Power Supply Constant Voltage Current Buck Power Converter Power Supply Adjustable Module https://www.amazon.com/dp/B01LWXAC5E/ref=cm_sw_r_cp_apa_sC-KzbRFPQRYZ
I have it wired to also accept a straight DC input and voltmeter on input and output.
One caveat, make sure to use a DC supply with an adjustable voltage pot,you need to bump up 42 to 45ish for the step down to provide 42 for instance, doesn't matter if you just use a 48v supply for instance.
<img src="/uploads/db1493/original/3X/2/6/26da48735612d04852b1308114e2e3cc45767414.jpg" width="333" height="250"><img src="/uploads/db1493/original/3X/a/1/a104f185178696b55af8a7cfa1c7345ddeb39306.jpg" width="333" height="250">
```

---
## \#7 Posted by: scepterr Posted at: 2017-08-16T06:38:45.854Z Reads: 273

```
For the range and high cycle life, stock ego ESC is 15A limited
```

---
## \#8 Posted by: markyoe Posted at: 2017-08-16T06:55:33.139Z Reads: 261

```
Awesome, thanks for the info! Do you have a link to the 42V 5A DC supply? Also, what are the chips on the lid?
```

---
## \#9 Posted by: scepterr Posted at: 2017-08-16T06:59:34.635Z Reads: 258

```
 42v5a http://www.ebay.com/itm/42V-5A-FAST-Charger-For-36V-Li-Ion-Electric-Bike-Bicycle-Ebike-Batteries-/263060085203
The PCB is the back of the voltmeter :yum:
```

---
## \#10 Posted by: jga Posted at: 2017-08-16T07:02:15.164Z Reads: 259

```
I am also working on an EGO 1. I was thinking of changing the enclosure to put a bigger battery but finally I can see with yours it is probably easier to re-use the original enclosure. I'll sacrifice the range a bit.
Did you manage to fit the VESC in the original ESC enclosure? It is very tight.
```

---
## \#11 Posted by: scepterr Posted at: 2017-08-16T07:08:04.836Z Reads: 267

```
The standard fet vesc, not really, but the latest version of the directfet 4.12 vesc ive seen pics of very likely should. 
You should enjoy this pic(though I don't recommend the focbox, any vesc4 will suit it fine in bldc)  <img src="/uploads/db1493/original/3X/8/5/85fc2cdc0196e45a4d708b1fdcd14f26a5d30486.jpg" width="375" height="500">
Personally I find the ego motor and belt cover durability simply unmatched
```

---
## \#12 Posted by: jga Posted at: 2017-08-16T09:57:37.053Z Reads: 238

```
I see you kept the unusual connection to the motor. Did you keep the Yuneec motor as well?
I thought I had read it was difficult to re-use it with another VESC, maybe I'm wrong. I intended to use a new 53XX motor to fit in the motor holder and cover. I believe it is just the electronics that stopped working, motor should be ok,
I may do a small enclosure in ABS for the VESC.
```

---
## \#13 Posted by: scepterr Posted at: 2017-08-16T10:02:52.281Z Reads: 240

```
Stock motor and and yeah I pulled the connector off an extra stock ESC, soldered male MT60 and jst to sensor leads, works in FOC sensored, but bldc is recommended if you don't want to keep fixing your vesc. Im 175lbs, I get 16-17mph,stock motor and battery with vesc with stock settings other than motor detection and batt max 28 min -12. Also your stock esc is very likely fixable if you're interested.
```

---
## \#14 Posted by: scepterr Posted at: 2017-08-17T20:47:26.426Z Reads: 236

```
29T from boardbumpers finally shipped :smiley:
<img src="/uploads/db1493/original/3X/8/e/8ee9f51beee3e16eedf2addf6c92a062d4e9f950.jpg" width="281" height="500">
```

---
## \#15 Posted by: scepterr Posted at: 2017-08-18T05:41:31.731Z Reads: 228

```
I'm curious, why don't I see people using the MT60 connector for phase wire connection?
<img src="/uploads/db1493/original/3X/9/3/93564e71d78b26fbb38a314634c1f2f3339c5c34.jpg" width="250" height="250"><img src="/uploads/db1493/original/3X/b/f/bffb78e4b777f47a0587de31507b5cb87bb57d35.jpg" width="250" height="250"><img src="/uploads/db1493/original/3X/2/4/24b9a76a83a30ab96d202283c9a3b8acbe7a2ef5.jpg" width="250" height="250">
```

---
## \#16 Posted by: AyoJay Posted at: 2017-08-18T12:54:16.903Z Reads: 216

```
Hey scepterr nice setup man! 
Did you remove the motor cover and cooler?
If yes how is it driving in rain?
```

---
## \#17 Posted by: scepterr Posted at: 2017-08-18T18:43:11.191Z Reads: 217

```
@AyoJay covers are all on there

Just got motor in :stuck_out_tongue_closed_eyes: thanks @JLabs
 <img src="/uploads/db1493/original/3X/5/3/538cc74ec4263f5c7aec70742ce4bc014331834a.jpg" width="375" height="499">
```

---
## \#18 Posted by: AyoJay Posted at: 2017-08-18T20:56:44.068Z Reads: 208

```
Alright, do you know if the motor is working in the rain or on wet streets ?
```

---
## \#19 Posted by: scepterr Posted at: 2017-08-18T21:06:33.459Z Reads: 205

```
The ego2 motor I've abused plenty in the rain without issue. Just make sure to properly drain it when you get home :wink:
```

---
## \#20 Posted by: AyoJay Posted at: 2017-08-19T00:08:46.312Z Reads: 205

```
Thanks m8! 
Really appreciate your help!
```

---
## \#21 Posted by: scepterr Posted at: 2017-08-20T13:04:14.894Z Reads: 208

```
Does anybody know of an identical deck to the E-Go 2 deck? Same size, shape 910*240mm
<img src="/uploads/db1493/original/3X/b/8/b899324054cacd7921a7c9f5ae720f704198beec.jpg" width="345" height="199">
<img src="/uploads/db1493/original/3X/0/9/09e2835f79bbad2c7cd9b234670e6fe401a3ccd6.jpg" width="345" height="199">
```

---
## \#22 Posted by: scepterr Posted at: 2017-08-20T18:07:34.775Z Reads: 208

```
Mount came, thanks @thisguyhere
<img src="/uploads/db1493/original/3X/0/d/0d97bd6a5bfe0d03b01a9310e8fc67f2ca78e2d4.jpg" width="666" height="499">
```

---
## \#23 Posted by: jammin Posted at: 2017-08-20T18:11:46.559Z Reads: 204

```
Earthwing superglider looks really similar. idk if they make them anymore
```

---
## \#24 Posted by: thisguyhere Posted at: 2017-08-20T18:12:38.168Z Reads: 203

```
:thumbsup:
```

---
## \#25 Posted by: scepterr Posted at: 2017-08-20T18:35:54.207Z Reads: 210

```
While I wait for my oshpark order,  @akhlut sent me his extra PCBs to use, very awesome of him. 
<img src="/uploads/db1493/original/3X/f/5/f50d6f286a55d36adb5506cc4b3b8eb6dfdb577c.jpg" width="666" height="500">
```

---
## \#26 Posted by: scepterr Posted at: 2017-08-21T00:15:13.375Z Reads: 199

```
@JLabs are these ok for mounting the motor? (You should auto-add bolts to cart when buying motor and make people remove it if they don't need it :wink:  ) Between getting mount and motor, overlooked needing bolts for motor lol<img src="/uploads/db1493/original/3X/b/4/b454ad762ab8aeddd17ae178ecb3d31025a1aa9a.jpg" width="140" height="250">
```

---
## \#27 Posted by: JLabs Posted at: 2017-08-21T00:19:35.150Z Reads: 203

```
PM me and I’ll give you a free shipping code if that’s all you need..

https://buildkitboards.com/products/m4x10-motor-mounting-bolts
```

---
## \#28 Posted by: scepterr Posted at: 2017-08-21T00:23:42.059Z Reads: 197

```
I think you nailed it. Slightly longer tail which is even better, though it seems it's only 5 ply..I think I need more ply than that
<img src="/uploads/db1493/original/3X/3/b/3bf2b8dafa1084c518c6d468c19f78ce47a69bd6.jpg" width="70" height="63">
```

---
## \#29 Posted by: scepterr Posted at: 2017-08-21T02:56:29.808Z Reads: 203

```
Am I crazy for wanting to stick this light on? It can be powered directly from the battery up to 80V, draws 12V2A
<img src="/uploads/db1493/original/3X/7/e/7e0d68141b91fc8e38986ebf8809cb6372da6f4c.jpg" width="140" height="250"> http://www.ebay.com/itm/222230285310
```

---
## \#30 Posted by: JLabs Posted at: 2017-08-21T02:57:22.877Z Reads: 193

```
You should not have posted that.. now I have to buy it and look like iron man
```

---
## \#31 Posted by: scepterr Posted at: 2017-08-21T03:01:27.519Z Reads: 217

```
For $10 saying no is impossible...next thing you know you have one on the front, one on the back, one on your head, two on your shoulders...
```

---
## \#32 Posted by: jammin Posted at: 2017-08-21T18:54:29.050Z Reads: 228

```
I have the 4 ply and it's not _super_ flexy. I think the 5 ply will have some give to it, but be stiff enough too
```

---
## \#33 Posted by: scepterr Posted at: 2017-08-21T23:38:53.762Z Reads: 233

```
Directfet vesc4 PCB, enjoy :wink:
https://drive.google.com/file/d/0B8LrLknwWHGEeFZlaDNIV05PbDg/view?usp=drivesdk
That was quite an ordeal getting it lol
```

---
## \#34 Posted by: JdogAwesome Posted at: 2017-08-22T01:46:59.976Z Reads: 231

```
Looks like an awesome board! Love the DPS5005 Charger! I personally use a DPS5015 as a lab bench PSU and its great! @markyoe If you look up 48V PSU on like eBay or AliExpress you can find them for pretty cheap, I personally use a 24V 20A PSU cause I usually dont do much above 24V. 

@scepterr I have actually seen a person or two use the MT60 connectors for phase leads, there just kind big and out of place compared to sleak bullets. Also that light you listed is looks cool, really big, but cool. Only thing is it seems really inefficient, with a 100W Legit Cree LED you should be getting somewhere closer to 15,000Lm not 3,000, though there obviously a lot more expensive so yeah.
```

---
## \#35 Posted by: scepterr Posted at: 2017-08-22T01:48:38.016Z Reads: 223

```
Could change out the led 😉
```

---
## \#36 Posted by: chaka Posted at: 2017-08-22T13:58:32.381Z Reads: 218

```
Wow you found my files! I was actually looking for your profile so I could send you some updated DirectVESC PCB's. Glad I saw this before contacting you. :wink:

 Posting these files without giving any attribution to what they are our who created them isn't the best course of action if you want people like me to continue creating and modifying files for the community to use. 

FYI, the file you have is not a final version and has some issues. Build at your own risk!
```

---
## \#37 Posted by: scepterr Posted at: 2017-08-22T14:10:11.258Z Reads: 203

```
Yep this is the file mentioned in the first post here 
https://www.electric-skateboard.builders/t/v4-12-direct-vesc-ollinboardco/13104
```

---
## \#38 Posted by: chaka Posted at: 2017-08-22T14:26:05.422Z Reads: 205

```
Yes I know, that was my post. Just know that I took that file down for a reason, you will need to make a few changes to the PCB file if you want a solid build. Have fun and welcome to the community!
```

---
## \#39 Posted by: scepterr Posted at: 2017-08-22T16:20:06.024Z Reads: 209

```
Things not working is half the fun :slight_smile:
Anything specific I should be aware of on the PCB?
```

---
## \#40 Posted by: scepterr Posted at: 2017-08-22T21:11:13.933Z Reads: 211

```
29T drive gear for yuneec motor arrived 😁
<img src="/uploads/db1493/original/3X/5/a/5ab77eef4e89849d9bad9c7693ad77cddac6b994.jpg" width="666" height="500">
```

---
## \#41 Posted by: flywithgriff Posted at: 2017-08-22T21:25:25.687Z Reads: 203

```
Wow! That's pretty cool
```

---
## \#42 Posted by: Randyc1 Posted at: 2017-08-22T21:53:23.343Z Reads: 194

```
Who make those MBS Pulleys?
```

---
## \#43 Posted by: mccloed Posted at: 2017-08-22T23:27:31.593Z Reads: 191

```
I believe this is where they came from: https://www.boardbumpersshop.com/product-page/yuneec-ego-ego-2-29t-drive-gear-upgrade-kit
```

---
## \#44 Posted by: Vampiresquid64 Posted at: 2017-08-22T23:45:09.214Z Reads: 188

```
if I had to guess, I'd say its because that connector only fits on one way so you would have to know which way your motor would spin before soldering, so if u got it wrong you would need to desolder. just a theory. overall I agree with u tho
```

---
## \#45 Posted by: scepterr Posted at: 2017-08-23T01:04:47.140Z Reads: 194

```
Yep it's from boardbumpers. Though I would hold off on ordering for the ego2, I can't seem to get it to line up properly. Waiting for response from BB.

It seems I got version 1 instead of 2 which it was supposed to be...I can't get it setup properly, their support said they'll send me a version 2 next month, but can't really provide specific installation instructions for the E-Go2 atm, which is kinda weird I think.
```

---
## \#46 Posted by: scepterr Posted at: 2017-08-27T16:54:22.097Z Reads: 188

```
Fresh goodies
<img src="/uploads/db1493/original/3X/6/3/63d3174e424d8ed560848c855dc6caf36d1049e3.jpg" width="375" height="499">
```

---
## \#47 Posted by: scepterr Posted at: 2017-09-02T09:01:53.017Z Reads: 182

```
Test fit looks good :grinning:
<img src="/uploads/db1493/original/3X/7/0/705018ad15d8c67ec7320121dfd4802c74807eb7.jpg" width="666" height="500">
```

---
## \#48 Posted by: vap Posted at: 2017-09-02T10:32:17.105Z Reads: 176

```
I'm using MT60, they work great. No problem with 120a escs and heavy vibrations offroad.
I would advise getting black connectors though,MT60s are hard to solder and yellow ones melt.
```

---
## \#49 Posted by: scepterr Posted at: 2017-09-06T00:53:03.151Z Reads: 180

```
Let there be light! :grin:
<img src="/uploads/db1493/original/3X/e/3/e3c81bbbd4959efe9cbb7ac8d48552ff0ca37b5f.jpg" width="375" height="499">
```

---
## \#50 Posted by: scepterr Posted at: 2017-09-06T19:36:26.495Z Reads: 176

```
Nice and tidy
<img src="/uploads/db1493/original/3X/7/a/7ad6ae3672ef1bfe3bde1b23ccbbb0039c0579df.jpg" width="666" height="499">
```

---
## \#51 Posted by: scepterr Posted at: 2017-09-08T00:34:34.907Z Reads: 161

```
I just gotta say WOW, I don't think I need more than 7S at the speed this thing flies.
But now I want dual for better control lol
```

---
## \#52 Posted by: scepterr Posted at: 2017-09-09T01:59:14.382Z Reads: 161

```
Loctite everything :grin:
<img src="/uploads/db1493/original/3X/9/6/9623450cf6bd83a2d0f1dc1de0a140aa184b16f5.jpg" width="666" height="500">
```

---
## \#53 Posted by: Cobber Posted at: 2017-09-22T21:21:37.644Z Reads: 151

```
[quote="scepterr, post:29, topic:30774, full:true"]
Am I crazy for wanting to stick this light on? It can be powered directly from the battery up to 80V, draws 12V2A
[/quote]

How did you go with the light bro? 125w is a lot!
I got one of these I can throw on mine for sessions at the local brewery as it is normally dark when we head home and there are not many streetlights where I live ;)
http://www.ebay.com.au/itm/5INCH-72W-CREE-LED-WORK-LIGHT-BAR-Flood-Spot-OFFROAD-4WD-SUV-ATV-CAR-LAMP-6000K/112543915788?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2648
At 72w I thought I was crazy... :stuck_out_tongue_winking_eye:
```

---
## \#54 Posted by: scepterr Posted at: 2017-09-22T21:24:38.087Z Reads: 150

```
Lol I went with shredlights
<img src="/uploads/db1493/original/3X/e/3/e3c81bbbd4959efe9cbb7ac8d48552ff0ca37b5f.jpg" width="375" height="499">
```

---
## \#55 Posted by: AyoJay Posted at: 2017-09-23T22:44:40.382Z Reads: 139

```
Do you think it’s possible to run 2 motors on the yuneec without changing the esc with 2 yuneec motors ?
```

---
## \#56 Posted by: scepterr Posted at: 2017-09-23T22:45:16.950Z Reads: 145

```
No it's not able to do that
```

---
## \#57 Posted by: scepterr Posted at: 2017-09-27T19:02:50.003Z Reads: 149

```
This build is being converted to dual diag ego2 motors
<img src="/uploads/db1493/original/3X/d/9/d94b06f07850f6c9f6c9f001c34315671fb69121.jpg" width="690" height="315">
Or
<img src="/uploads/db1493/original/3X/6/4/64739466e78af15b95566081449c398a139cbbb4.jpg" width="690" height="274">
```

---
## \#58 Posted by: Eric Posted at: 2017-09-28T18:39:03.678Z Reads: 135

```
What are the specs for your final board? Speed and range as well as what motors, gearing ratio, and correct me if I'm wrong but it looks like you're using a 10s8p
```

---
## \#59 Posted by: jga Posted at: 2017-09-28T20:19:43.261Z Reads: 130

```
I would be surprised if there are 80 cells there...:astonished:
```

---
## \#60 Posted by: Eric Posted at: 2017-09-28T20:55:47.700Z Reads: 130

```
Those are the cheap eBay cells, and each one of those packs is a 10s2p, and he has four of those packs.
```

---
## \#61 Posted by: scepterr Posted at: 2017-09-28T21:02:07.789Z Reads: 130

```
Specs will be updated when it's running,
The motors are 160kv 15/36 gearing 90mm wheels
Pack is 10S8P MF1
```

---
## \#62 Posted by: scepterr Posted at: 2017-10-01T18:23:22.879Z Reads: 122

```
Found an enclosure to fit everything
10S8P, 2 vescs
<img src="/uploads/db1493/original/3X/d/6/d6427b20eea1fae6a40fce35033fd7c2881565fc.jpg" width="690" height="397">
```

---
## \#63 Posted by: Gabriel_Robinson Posted at: 2017-10-24T02:09:46.658Z Reads: 94

```
where did you get that enclosure?
```

---
## \#64 Posted by: GrecoMan Posted at: 2017-10-24T02:15:25.183Z Reads: 90

```
wondering  the same thing...
```

---
## \#65 Posted by: Gabriel_Robinson Posted at: 2017-10-24T02:16:22.885Z Reads: 93

```
I think its an old one that housed Lead acid batteries
```

---
## \#66 Posted by: scepterr Posted at: 2017-10-24T02:40:12.939Z Reads: 97

```
That one came with this blue bomb
<img src="/uploads/db1493/original/3X/3/2/32b99d27942e2b46c9f3bbc311bd3fac6b7f9a41.jpg" width="666" height="500">
Perfect dimensions for the 18650 packs 😉
```

---
## \#67 Posted by: GrecoMan Posted at: 2017-10-24T11:02:41.687Z Reads: 90

```
got an extra?
```

---
