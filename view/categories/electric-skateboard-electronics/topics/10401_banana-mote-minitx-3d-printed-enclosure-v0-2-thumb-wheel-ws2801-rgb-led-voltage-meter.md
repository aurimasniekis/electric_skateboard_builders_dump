# **Banana-mote-miniTX** &#124;&#124; 3D Printed Enclosure V0.2 &#124;&#124; Thumb Wheel &#124;&#124; ws2801 rgb Led Voltage Meter &#124;&#124;

### Replies: 49 Views: 4523

## \#1 Posted by: saul Posted at: 2016-09-30T08:07:54.670Z Reads: 456

```
Remotes have become a popular topic recently since there are so few options.

I've tried to make an enclosure for the gt2b but the board is just **too big**, meanwhile my mini remote has worked well without any major problems. 

A look inside shows amic A7105 transever module similar to [this](http://www.ebay.com/itm/AMIC-A7105-Wireless-RF-2-4GHz-Transceiver-Modules-2400-2483M-3-3V-FSK-GFSK-/280953247359) 3.3v input. and no regulator so I'll have to get some external ones to use a single li ion 18650.

----------
**_Super mini_**
----------
----------


mini remote tx
3.3v regulator
700mah li ion slim battery
attiny85 microcontroller
2 x  ws2801 rgb led (5v)
Voltage meter displayed by leds^.
micro usb charger 1A.
Undecided Compact style thumb or rocker throttle.

Hopefully nano remote size or smaller!
----------
<img src="/uploads/db1493/original/3X/6/c/6c5ae46adec61c4692ea6e4587019f3155943cde.jpg" width="280" height="500">



----------

Deluxe
----------

mini remote tx
3.3v regulator
3000mah 18650
attiny85 microcontroller
3w led + mosfet pwm
3 - 5x ws2801 rgb led (5v)
Voltage meter displayed by leds^.
micro usb charger 1A.
Boosted style thumb wheel (might use orginal steering wheel).
----------

A mock up with an enclosure meant for another project...
<img src="/uploads/db1493/original/3X/d/b/db594495ef1c7a617006fadb1681742643d62f8f.jpg" width="280" height="500">

**v1**
<img src="/uploads/db1493/original/3X/7/2/72f839a53dd2c0cb7c2c6d60f83e24247ea4d761.jpg" width="690" height="387">

**24mm thick. similar size...**
<img src="/uploads/db1493/original/3X/6/1/61b72c3686aa22d447eb0eb54f676d5d85ac3554.jpg" width="690" height="387">

**mini remote  -  nano + nrf - gt2b**
<img src="/uploads/db1493/original/3X/d/3/d3f77ac06884c833b85bce21edb73a942a6f0c32.jpg" width="690" height="387">
```

---
## \#2 Posted by: ThomasRBK Posted at: 2016-09-30T08:50:30.319Z Reads: 409

```
Looks awesome man, would love to have a look at the design in 3D :slight_smile:
```

---
## \#3 Posted by: saul Posted at: 2016-09-30T09:02:33.173Z Reads: 430

```
thanks! I haven't printed the lid yet so heres a look at the cad model.

I'm going to try to cut off the top so I can print it vertical and get a stronger, nicer grip.

<img src="/uploads/db1493/original/3X/d/5/d56f0d96b2c5640f2bd3fa531f6f52240c433c42.png" width="293" height="401">

<img src="/uploads/db1493/original/3X/7/7/77e645846d9f8213cdc25a02da36a468ad223c79.png" width="379" height="490">

<img src="/uploads/db1493/original/3X/0/1/012baea85af55800184c72db85588b991ddd4fb0.png" width="280" height="435">

<img src="/uploads/db1493/original/3X/d/8/d82abffaafefdda96c8e50ed187fa1ebccb00b2a.png" width="631" height="476">

<img src="/uploads/db1493/original/3X/d/a/daffd0b4849680379e47dd1101703d8e431b302a.png" width="658" height="500">

The board has no mounting holes so I will glue it in place...somewhere...
```

---
## \#4 Posted by: ThomasRBK Posted at: 2016-09-30T09:09:14.653Z Reads: 365

```
It really reminds me of the boosted remote, and that's a good thing :)
```

---
## \#5 Posted by: saul Posted at: 2016-09-30T09:28:40.257Z Reads: 381

```
Yes thats kinda what i'm going for, at least for now. 

I finally tried a boosted (v2) a few days ago and the remote was better than i expected but i did keep rolling the wrong way. The torque was nice and smooth too but thats going off topic..



----------
(not mine) boosted remote tear down
----------

<img src="/uploads/db1493/original/3X/5/d/5dec1512bafd8f2038a638d7b3637ce0774878e2.jpg" width="690" height="387">
```

---
## \#6 Posted by: Ackmaniac Posted at: 2016-09-30T12:58:34.042Z Reads: 362

```
Are you sure that you need a 3.3v regulator. And which one did you use. I want to run mine also via li-ion.
```

---
## \#7 Posted by: itsmikeholland Posted at: 2016-09-30T16:19:19.529Z Reads: 356

```
Ugh will someone print a ripe banana shaped remote already?
```

---
## \#8 Posted by: saul Posted at: 2016-09-30T22:43:29.601Z Reads: 346

```
The board only has a diode on input voltage, and the module input is 2 - 3.6V so yes.

I was thinking of using a LiFePO4 battery 3.3-3.6v (Perfect) but then i'd have to find a charger..and all that.
```

---
## \#9 Posted by: saul Posted at: 2016-09-30T22:44:34.140Z Reads: 339

```
banana? :banana::banana::banana::banana:




....bbb....
```

---
## \#10 Posted by: itsmikeholland Posted at: 2016-09-30T22:52:43.471Z Reads: 331

```
Im gonna make this a thing. The peel will be the trigger
```

---
## \#11 Posted by: saul Posted at: 2016-09-30T22:56:36.828Z Reads: 324

```
and a hand guard on the other side :joy:

but...but....i don't have any yellow filament! :cry:
```

---
## \#12 Posted by: itsmikeholland Posted at: 2016-09-30T23:00:47.552Z Reads: 310

```
Not yet you dont! How much does that cost? Yellow for the peel and maybe a cream color for the insides...we can paint on some brown spots and blemishes for authenticity
```

---
## \#13 Posted by: saul Posted at: 2016-09-30T23:07:46.661Z Reads: 308

```
about $30 a kg roll :money_mouth:

actually i have some clear that would work for the inside...this design took a pivot.
```

---
## \#14 Posted by: saul Posted at: 2016-09-30T23:20:42.074Z Reads: 322

```
Banana? kinda....5minute attempt...

<img src="/uploads/db1493/original/3X/3/c/3c3ed06bea787106342462b164afae2f61c82cc2.png" width="319" height="500">
```

---
## \#15 Posted by: Pantologist Posted at: 2016-09-30T23:26:53.581Z Reads: 300

```
I really like the feel of a thumb wheel. Do you think you can switch the potentimeter contacts of the wheel and finger trigger to use the wheel for the forward and brake channel?
```

---
## \#16 Posted by: saul Posted at: 2016-10-01T00:28:46.918Z Reads: 287

```
The wheel already works, you just have to connect to ch1 on the rx. :nerd:

I like the wheel too it just needs to be slimmer and centered. coming soon!
```

---
## \#17 Posted by: itsmikeholland Posted at: 2016-10-01T00:47:09.001Z Reads: 289

```
Ohh my gawd its beautiful already! I need to download a program and spend all night on a peeled design. Id rock gt2b banana controller so hard
```

---
## \#18 Posted by: saul Posted at: 2016-10-01T02:50:27.782Z Reads: 300

```
i'm thinking a half peeled design, just not sure how to print that... guess it could work for a gt2b but it would be fat
```

---
## \#19 Posted by: itsmikeholland Posted at: 2016-10-01T04:19:55.833Z Reads: 295

```
Might have to print the peels separately, then glue them to the base. After glueing the joints between the peel and the....shaft?....can be sanded and painted, which saves us $30 of yellow filament since we'll have to paint it anyways. If it doesnt seem like too much of a pain, id totally pay for a fat gt2b banana controller. Ive been dreaming of it since day 1 before i even knew what LiPo stood for lol! Any idea what youd charge for a half peeled fat banana remote?
```

---
## \#20 Posted by: saul Posted at: 2016-10-01T05:25:57.758Z Reads: 304

```
well a roll would be enough for like 20 remotes and I need more anyways...
 I was planning something a bit different...but this would just be a different shell. :thinking:

let me try to print a test and see how it feels...what wold a banana remote be worth to you? :sunglasses:

and does anyone else want one? lol
```

---
## \#21 Posted by: itsmikeholland Posted at: 2016-10-01T05:46:45.461Z Reads: 273

```
I think we should create a new thread for banana remotes :banana: :banana: :banana:. I don't know how much materials cost, is $40 a low ball? $50? 

If it's any help, I found this cad file here, not peeled but seems pretty neat. https://grabcad.com/library/banana-2

I seriously need to learn how to sketch these things up, maybe that's what I'll do this weekend :nerd:
```

---
## \#22 Posted by: saul Posted at: 2016-10-01T08:09:51.775Z Reads: 299

```
the newest gt2b printed enclousure is $25 just for the shell...i've seen completed mods for $100...

anyways heres a scaled print of the test. not yellow but the shape is pretty nice..

one of the nicest prints in a while! 

<img src="/uploads/db1493/original/3X/9/b/9bf6baa34cf377561b4fef2dbe160481f9398e3c.jpg" width="280" height="500">
<img src="/uploads/db1493/original/3X/2/4/2475da2a75237e7f98211c145026c3c6840b513c.jpg" width="280" height="500">
<img src="/uploads/db1493/original/3X/f/1/f12cf92fb69ac8fc5e7f4b7eb2c11c4c798db40e.jpg" width="280" height="500">
```

---
## \#23 Posted by: saul Posted at: 2016-10-05T08:11:58.602Z Reads: 285

```
Got some translucent yellow filiment, it reminds me of hi viz yellow! 
Its going to work well with the leds! which are also done.

just waiting on the buck/boost converters....

Left is a more accurate color
----------


<img src="/uploads/db1493/original/3X/4/c/4c0893d2168e4bffdc8825a3074f68ef38db7ca3.jpg" width="280" height="500"><img src="/uploads/db1493/original/3X/a/4/a47db1f19c3f4ac6c5e74f89765aae6c75bd4476.jpg" width="280" height="500">
```

---
## \#24 Posted by: TheRedPanda Posted at: 2016-10-05T12:02:06.303Z Reads: 272

```
Do you have an IRL banana for scale? :grin:
```

---
## \#25 Posted by: flatsp0t Posted at: 2016-10-05T12:10:40.312Z Reads: 265

```
I just fell over this a few days ago, maybe it is possible to use it.
http://lifepo4wered.com/lifepo4wered-usb.html
https://www.tindie.com/products/xorbit/lifepo4weredusb/
```

---
## \#26 Posted by: saul Posted at: 2016-10-05T14:02:09.579Z Reads: 281

```
@TheRedPanda just ate the last one :banana::sob: i'll get one for scale when i print the other half!

@flatsp0t those look really cool, i'll keep them in mind.
 but I went with the [mcp1700](http://www.digikey.com/product-detail/en/microchip-technology/MCP1700-3302E-TO/MCP1700-3302E-TO-ND/652680), it gives 3.3v at 250ma with input 2 - 6v So works perfect for a single li ion which are cheaper, come in more sizes, and have higher capacity.
  
and i can still drive all the leds on the liion directly, not sure if the rgbs would work on <3.5v....
```

---
## \#27 Posted by: saul Posted at: 2016-10-14T00:24:57.835Z Reads: 273

```
The banana was too fat, but I will go back to it soon.

Here is the super mini I've been working on. printing now.... :sleeping:

<img src="/uploads/db1493/original/3X/5/1/51ee512c6b2231971a1ce0aa2f3c02ea6f557c5b.png" width="392" height="500">
<img src="/uploads/db1493/original/3X/8/5/85b821bdf225434adb77da8018409e6d395dc6c9.png" width="216" height="500">
<img src="/uploads/db1493/original/3X/a/a/aa654ae128e872ea015a8150c8632763ba231d9a.png" width="322" height="500">
<img src="/uploads/db1493/original/3X/d/7/d751ab559e68d165e87f9bca3b8c411ee1d4b7da.png" width="387" height="481">
```

---
## \#28 Posted by: Kaly Posted at: 2016-10-14T01:59:36.829Z Reads: 244

```
this is great work Man  !!!!  :-) :-) :-)

i've have a couple of mini remotes around,I was thinking on a mod for the enclosure but you are already way ahead of what i was thinking. 

Are you thinking on sharing the stl files or going to sell the enclosure ?
```

---
## \#29 Posted by: saul Posted at: 2016-10-14T03:22:08.085Z Reads: 246

```
Thanks! I've notice these remotes were getting popular and I've been using it since day one with no issues!
Just annoyed it doesn't fit in a pocket well...

i'm still not sure what i'm going to do, need to get this fully assembled and tested then i'll see what the demand is like...

i'll probably sell a few to help support this whole esk8 building habbit :money_mouth:
this version is also no just a plug and play mod, it requires some addtional parts...since its switching to rechargable!
```

---
## \#30 Posted by: i2oadsweepei2 Posted at: 2016-10-26T22:21:06.043Z Reads: 222

```
Hello Saul, just wondering if there are any updates on this mod. 

Thanks,
Kevin
```

---
## \#31 Posted by: saul Posted at: 2016-10-26T22:30:00.970Z Reads: 231

```
Haven't had time to work on this for a bit, But i will finish it soon.
switched to 18650, small battery version wasn't small enough to be worth it.

If anyone has a 3d printer and would like to _beta test_ an enclosure let me know!

<img src="/uploads/db1493/original/3X/d/a/da9bbe7b9e204bf51b2e72c4f8e707b2ea232834.png" width="356" height="500">
<img src="/uploads/db1493/original/3X/2/a/2a7e59dc8fe79f237ef55559ac3f756d1780370c.png" width="376" height="498">
```

---
## \#32 Posted by: Pantologist Posted at: 2016-10-26T22:34:38.618Z Reads: 210

```
I have a 3D printer! I also have a TB Mini remote that needs to be shrunk. I also have extra 18650 cells. Just don't have a voltage regulator or lithium charger yet. Just send me the STLs :D
```

---
## \#33 Posted by: saul Posted at: 2016-10-26T22:51:26.950Z Reads: 217

```
I still need to make some small changes and do a test print. 

if you want to see the older version, its about a 4hr print.
I couldn't fit a decent size battery in this yet, so moved back to 18650...

**Not ready for use -- for cosmetic purposes only**
https://drive.google.com/open?id=0B4_1KKUphqtDYm4wNzJqWHFFZGM

if you use a lifepo4 18650 you can get away without a regulator.

also I only recommend if you have a spare mini remote. I don't think its ready for everyday use.
```

---
## \#34 Posted by: Pantologist Posted at: 2016-10-26T23:16:56.565Z Reads: 205

```
Let me know when the next version is done. I'll print that.
```

---
## \#35 Posted by: saul Posted at: 2016-10-26T23:20:06.739Z Reads: 199

```
ok, i'll probably get back to it in a couple days... unless I get inspired :sleeping:
```

---
## \#36 Posted by: Pantologist Posted at: 2016-10-26T23:22:07.084Z Reads: 198

```
So there is an opening on one side of the remote? 

Is it possible to make a shell design? All you have to do is create screw holes and then split the part in two.
```

---
## \#37 Posted by: saul Posted at: 2016-10-26T23:27:45.080Z Reads: 205

```
yes its open side, with a screw on cover.

I started with halfs like gt2b...but i don't really like the feel. and the seam...

Unibody design, with vertical print feels really nice! strong. lots of details....

it also helps to prototype this way instead of 2 2-3 hour prints you get 1 4 hour and 1 10 minute ;)
```

---
## \#38 Posted by: Pantologist Posted at: 2016-10-26T23:33:46.864Z Reads: 201

```
Ahh okay. I didn't have that part so I was not sure. 

I'll be waiting for that remote design ;) I want to do some testing this weekend so if you could get it done before then, I might be able to actually test it while riding.
```

---
## \#39 Posted by: saul Posted at: 2016-10-26T23:41:02.370Z Reads: 204

```
i'll see what I can do! 
motor mount have taken most of my attention lately....
```

---
## \#40 Posted by: Pantologist Posted at: 2016-10-26T23:41:55.549Z Reads: 206

```
Yeah you've been busy I can tell! I almost forgot you designed those motor mounts as well. You must be a MechE?
```

---
## \#41 Posted by: saul Posted at: 2016-10-26T23:45:47.737Z Reads: 190

```
Yea things have sort of snowballed....
actually I studied cs, but physics hasn't changed :nerd:

All of my designs are written in openscad, geometric/logic based code.
```

---
## \#42 Posted by: Kaly Posted at: 2016-10-27T09:51:24.499Z Reads: 184

```
I will like to print one of this ;-) 
Can you share the beta file when ready ?
```

---
## \#43 Posted by: ajaynagra Posted at: 2016-10-29T16:07:23.802Z Reads: 182

```
I would also like to print :)
```

---
## \#44 Posted by: ajaynagra Posted at: 2016-12-06T16:16:11.395Z Reads: 156

```
Any updates on this?
```

---
## \#45 Posted by: saul Posted at: 2016-12-06T17:45:58.978Z Reads: 157

```
sorry nothing yet. been very busy.

I will have something soon.
```

---
## \#46 Posted by: saul Posted at: 2016-12-09T05:17:29.650Z Reads: 145

```
Just curious. would you guys prefer rechargable (needs more components) or a small 2AA version?
```

---
## \#47 Posted by: i2oadsweepei2 Posted at: 2016-12-09T11:34:09.993Z Reads: 138

```
I wouldn't mind either. If I knew you were working on a 18650, 18350 or small lipo version I would totally wait for rechargeable. It's winter here though... So I will happily await the outcome. Thanks for doing this.
```

---
## \#48 Posted by: scepterr Posted at: 2017-11-12T09:13:38.184Z Reads: 94

```
Hey @saul anything new with this?
Got a printer coming Monday and a virgin mini...😉
```

---
## \#49 Posted by: saul Posted at: 2017-11-18T10:21:14.622Z Reads: 77

```
[quote="scepterr, post:48, topic:10401"]
anything new with this?
[/quote]

I abandoned the mini remote completely.. .it works fine but

I should have something with more features and same/smaller size soon.
```

---
