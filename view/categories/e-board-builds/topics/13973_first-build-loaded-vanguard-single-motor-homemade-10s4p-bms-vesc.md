# FIrst build, Loaded Vanguard, single motor, homemade 10S4P, BMS, VESC

### Replies: 48 Views: 4949

## \#1 Posted by: pyttroll Posted at: 2016-11-30T17:07:09.683Z Reads: 432

```
Hi guys,

I recently got interested in esk8 building after having withdrawn my pre-order for a Boosted following their battery issues.
I ordered what I believe is everything I need to assemble my first build, here are the parts:

* Loaded Vanguard 42" deck Flex 2
* Caliber v2 10" Trucks Blackout (50 Degree Baseplate)
* Kegel 83A (a bit hard but I can't get my hands on the 80A) with Loaded Jehu Bearings
* DIY 36T KEGEL Pulley Combo Kit (Motor Pulley: 16T Motor Pulley, Belt Size: 265mm 12mm Wide)
* DIY Electric Skateboard Motor 6355 190KV
* Benchwheel remote
* DIY Single Bolt On Motor Mount Set ONLY (Black)
* DIY Motor Mount Type: 63mm Motor Mount
* DIY VESC BLDC Speed Controller
* DIY On Off Power Switch Electric Skateboard
* 40 x LG 18650 HG2 for custom battery 
* 36V 10S  60A BMS
* Li-ion Li-Po 42V for 36V 37V 10S 2A Wall Socket Battery Charger 
* Bluetooth module for VESC from rpasichnyk

Am I missing anything?

Probably some kind of charing 5.5mm DC female connector..?

Thanks,

Pyt
```

---
## \#2 Posted by: SirDiff Posted at: 2016-11-30T17:38:39.367Z Reads: 398

```
Are you aware of the flex of the deck? People with vanguards usually split the battery and other components in 2 parts (like Boosted) because flat battery packs won't flex, while the deck does, and it could damage the components. You won't be able to put 50 18650s under that board
```

---
## \#3 Posted by: pyttroll Posted at: 2016-11-30T17:48:26.253Z Reads: 378

```
Yeah I'm aware of that, I'm planning on building a 10S4P at first, probably split in 2 parts. I ordered 50 because there was a better bulk price and also in case I destroy a cell while building the battery (planning of soldering).
```

---
## \#4 Posted by: SirDiff Posted at: 2016-11-30T18:07:24.488Z Reads: 364

```
In that case, you should be okay. Which BMS will you use?
```

---
## \#5 Posted by: pyttroll Posted at: 2016-11-30T18:08:58.387Z Reads: 352

```
I ordered this: http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html

Someone recommended in one of the threads.
```

---
## \#6 Posted by: SirDiff Posted at: 2016-11-30T18:11:52.653Z Reads: 347

```
If I'm not wrong, you should be able to get it with a switch soldered on it, this could save you a lot of time. @Jinra may tell you more specifically how to do so
```

---
## \#7 Posted by: pyttroll Posted at: 2016-11-30T18:36:24.337Z Reads: 337

```
Super, thanks for the advice.
```

---
## \#8 Posted by: TranxFu Posted at: 2016-12-01T08:12:47.784Z Reads: 328

```
I am also going for a vanguard build. Do you already have the board ? What's ur weight ? I have the flex 2 but I dunno if I should go for the shorter flex 3... check whiteponys vanguard build. I think that is one of the best out there. He also splitted his 10s4p
```

---
## \#9 Posted by: jujet Posted at: 2016-12-01T09:47:18.454Z Reads: 313

```
Are you in Europe? 

And did you already place your order?

I want a bms as well but they're charging me 20 eur for shipping....
```

---
## \#10 Posted by: pyttroll Posted at: 2016-12-01T12:55:44.876Z Reads: 312

```
Hi @jujet, I'm in Canada, and I already placed my order. Shipping was expensive indeed, China seems to have  logistic problems theses days, I'm still waiting for stuff from aliexpress (non-esk8 related), it's been 2 months...
So they offer this expensive shipping option but guarantee a decent delivery.
```

---
## \#11 Posted by: pyttroll Posted at: 2016-12-01T13:01:08.990Z Reads: 298

```
Hi @TranxFu, I'm 80kg, I was gonna go for the Flex 3 but in this [thread](https://endless-sphere.com/forums/viewtopic.php?f=35&t=80808&sid=208700882768b18eda2a334b3c8814c5)@whitepony highly recommends going for the Flex 2.

> cant stress enough that I think that the flex 1 and flex 2 vanguards are much better carvers than the smaller flex 3+ models that boosted is using. the 2 42" flex versions allow your feet to stand comfortably far away from the trucks, giving you really great damping and a really awesome springy return ... and at the same time, the larger wheelbase makes for a more stable ride.
```

---
## \#12 Posted by: TranxFu Posted at: 2016-12-01T14:27:27.566Z Reads: 298

```
Thanks buddy ! Just what I needed to hear :D... I'm 85kg and lets say add a backpack(5kg). Flex 2 should be fine then. I was just worried about the extra 10cm... I'll go with nearly the same setup as yours. Just minor differences in motor and drive train... How are you planning to make your split enclosures ? And are you sure about soldering the 18650 ? Theres cheap ways to make a DIY Spotwelder
```

---
## \#13 Posted by: pyttroll Posted at: 2016-12-01T14:48:35.966Z Reads: 294

```
Glad I could help @TranxFu, I'll go for split enclosures indeed, I'm waiting for 3d files from this [thread](http://www.electric-skateboard.builders/t/custom-enclosures-for-sale-design-your-own/7485), or I'll print [these](http://www.thingiverse.com/thing:1834035).
For the battery, I've done some research and there should not be a problem with soldering as long as you're fast, I don't want to get into the trouble of building a spot welder. I also read that spot welding does not create a contact surface as good as traditional soldering, but I could be wrong.
```

---
## \#14 Posted by: Eboosted Posted at: 2016-12-12T04:01:55.882Z Reads: 278

```
Do you know how you are going to connect the VESCs with the battery?, for my build, which is technically the same as yours, I'll use flat braided tinned copper wires and a wood router to connect the electronics from the top, after that I'll have to cover the cable with epoxy and cover it later with grip tape.

I went with the 38" Flex 3 Vanguard as I'm looking for some flex but not as much, I plan to stand near the tracks to get maximum control at high speeds, looking to get 23MPH (38km/hr) on my build, and stand a little bit more in the center for carving intensive rides and get the springy benefit of the deck. With the 42" you only have the option to stand in the center for carving, but the added weight would hurt braking ability and turning reaction would be diminished at high speeds, on the other hand the bulkiness of a 42" would not be good for carry it around.

Please share pictures of your work and parts, whenever you can, I'm triying to follow all Vanguard threads in order to help me when I receive my parts, your build will be awesome LOL
```

---
## \#15 Posted by: grovestreetparty Posted at: 2016-12-12T09:30:14.490Z Reads: 267

```
Haha looks like youguys will be the testers for my eventual vanguard build. I myself am thinking about using a vinyl wrap underneath the deck, which might serve as a solid place to run the wires so I don't have to go above the deck or drill through. 
Please document as much as you can! As much as I've learned, I feel like everybody is still leagues ahead of me on this.
```

---
## \#16 Posted by: pyttroll Posted at: 2016-12-12T11:51:08.058Z Reads: 291

```
I'll use a router on the top of the deck to create 2 channels and regular 10 gauge wire for the connection to the VESC.
Like you, i'lol use epoxy to fill the holes and black grip tape after.

The Vanguard comes with transparent grip, I'm not sure if it's tape though, so I don't know how difficult it's going to be to remove.

I'm mostly focusing on range and less on speed, I probably won't be carving as juch as you so the flex does not bother me.

Good luck with your build, looking forward to see how it turns out.
```

---
## \#17 Posted by: pyttroll Posted at: 2016-12-13T03:52:05.416Z Reads: 299

```
Here is my 10S4P layout, it is inspired from the battery made by @barajabali for @Eboosted:

<img src="/uploads/db1493/original/3X/3/7/370d4214e6feeba5d59691b2056c13083cd0b3d6.jpg" width="374" height="500">
```

---
## \#18 Posted by: Eboosted Posted at: 2016-12-13T04:32:07.724Z Reads: 291

```
It was a design @jackw and I put together, @barajabali made the idea physically together

The wiring looks great @pyttroll, what BMS are you going to use? Batteries Support's? 

The battery pack should be in Peru by this weekend, as soon as I have it with me I'll take the final measures and print the 3D enclosure together, hope the board looks visually appealing with it bolted on.
```

---
## \#19 Posted by: pyttroll Posted at: 2016-12-13T12:57:09.027Z Reads: 284

```
I'm using the exact same BMS as yours.
Looking forward to see that enclosure printed.
```

---
## \#20 Posted by: TranxFu Posted at: 2016-12-13T14:39:15.897Z Reads: 277

```
The grip tape on the vanguard is sprayed on. So you'll have to sand it down
```

---
## \#21 Posted by: pyttroll Posted at: 2016-12-13T19:09:15.254Z Reads: 272

```
Thanks for the info :)
```

---
## \#22 Posted by: pyttroll Posted at: 2017-01-31T00:25:44.233Z Reads: 287

```
Here is a quick update.

I received my batteries late december, 50 x LG HG2.

<img src="/uploads/db1493/original/3X/6/6/668473772b579ffb7020229795bce96f84c75f36.jpg" width="375" height="500">

That's a lot of boxes...

<img src="/uploads/db1493/original/3X/c/6/c657487f408be1eabeba54b5c6a31b04c3302285.jpg" width="375" height="500">

I checked them all for voltage consistency.

<img src="/uploads/db1493/original/3X/6/7/675e7005010717c2d173eed12db4b6fac6181f4d.jpg" width="375" height="500">

I initially was going to build a 10S4P so I selected the 40 HG2s with the closest voltage. I built at 10S5P in the end...

<img src="/uploads/db1493/original/3X/0/8/0829653143a626560e342079b6287044f4d92e98.jpg" width="666" height="500">

Added more insulation on the positive side.

<img src="/uploads/db1493/original/3X/4/d/4d9ce8a47b78f6a7fdec715ddcf8bf73f034a76e.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/b/b/bb1612a41f8b280e3366e8529a0e19e8f990cae6.jpg" width="666" height="500">

Hot glued cells of 5 HG2s.

<img src="/uploads/db1493/original/3X/4/9/49d0ceb307fcb1fc14ba3693bc188f29894ebebe.jpg" width="666" height="500">

And spot welded them.

<img src="/uploads/db1493/original/3X/8/b/8b036d51acdb8971ac2304979a983ad7ea2dc31e.jpg" width="666" height="500">

Plugged everything to test out the wiring.

<img src="/uploads/db1493/original/3X/3/1/312d639380b402b0dbfc16d9a686b95fae987ac4.png" width="690" height="387">
https://youtu.be/L0eZw7f6Az8

Slow-mo.

<img src="/uploads/db1493/original/3X/8/1/814b1805cb068091f62f2970e78a0422c26df9b6.png" width="690" height="384">
https://youtu.be/feWFi75SpRU

Vaccuum formed some enclosures.

<img src="/uploads/db1493/original/3X/9/f/9ffbd90c96394c40dbadddbc514c2a427a6d3401.jpg" width="375" height="500">

Added a vinyl wrap on one of them (second one is pending completion).

<img src="/uploads/db1493/original/3X/e/1/e1f1292c79259d61be4af520099f98510ad5d0a1.jpg" width="375" height="500">

Drilled some holes and added inserts.

<img src="/uploads/db1493/original/3X/4/b/4b91457c9f6317aca8b945ab6597dd59acf02525.jpg" width="666" height="500">

Screwed the back enclosure to the board, waiting on some washers to arrive...

<img src="/uploads/db1493/original/3X/1/d/1d43abfc7940629e3b6d0963a3c1d509d53c39d0.jpg" width="375" height="500">

The other enclosure mounted, needs vinyl wrapping...

<img src="/uploads/db1493/original/3X/7/5/7573348a700e76cf0fb2d533e38122a31bebf9b5.jpg" width="375" height="500">

Routed channels for the main wires.

<img src="/uploads/db1493/original/3X/c/3/c39dd08e71301f6ce7c069effba2af86c1702221.jpg" width="666" height="500">

And then for the balancing wires.

<img src="/uploads/db1493/original/3X/6/5/6507b278f34cacd051fda0a9c0b1671d1954f4dc.jpg" width="375" height="500">

Flex test. Enclosure can take the bounce.

<img src="/uploads/db1493/original/3X/4/1/41b4dc3f7bacba15a08d13d0a69bf0ede4bb5039.png" width="690" height="345">
https://youtu.be/ICKvel-OdWM

Pushing it.

<img src="/uploads/db1493/original/3X/1/8/1870a34090b696d33136393488b827d2f12e77bd.png" width="690" height="387">
https://youtu.be/J0QkZn93cgw

I'm almost done with the project, a few hours left to finish the wiring and cut holes for the anti-spark switch and charging port.
```

---
## \#23 Posted by: Eboosted Posted at: 2017-01-31T08:03:00.180Z Reads: 264

```
That looks amazing, congrats!

My friend and I are building two Vanguards, the forst one if already done, I'll do mine as soon as i finish the final details Never Summer Reaper.

[img]http://i.imgur.com/9Su9Dus.jpg[/img]
```

---
## \#24 Posted by: pyttroll Posted at: 2017-01-31T11:39:48.327Z Reads: 256

```
Congrats to you too, these look awesone!
```

---
## \#25 Posted by: jimbosays Posted at: 2017-02-08T05:58:00.904Z Reads: 244

```
Any updates on this build? Looks sweet and I'm curious to know the top speed with your setup!
```

---
## \#26 Posted by: pyttroll Posted at: 2017-02-08T12:40:31.103Z Reads: 242

```
I have to make a new enclosure for the back, I can't fit my VESC, BMS and anti spark switch in there. I have to find time, and being a dad with a small kid does not leave you much time : )
Plus I need to wait for the snow to melt.
I'll keep you posted.
```

---
## \#27 Posted by: pyttroll Posted at: 2017-03-07T13:54:57.621Z Reads: 249

```
Finally got to get the board to a very close to final state.
I had to redo the rear enclosure about six times, it was initially too small, then I had some issues with the motor mount touching it when turning. I guess that's what you get trying to fit 50 cells on a Vanguard...
In the end I'm pretty happy with the result, not as clean as I would have liked it to be but good enough.

Took it for a spin and I have to say it has tons of torque, not sure why I'd put a second motor on it, I'm using @Ackmaniac firmware and it helps smoothing the acceleration. 

Next step would be to install rear lights and use carbon fibre vinyl on the enclosures.

<img src="/uploads/db1493/original/3X/4/3/436cc227b29cecf84ff4f42054de34370b7dd105.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/b/8/b80d88884787e9a0275eca3caca002a15bd0e1af.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/c/8/c85f5e62191d1e833dff1f3e6d13f29e23b583cd.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/2/b/2bd4052df89dcf4dd45a4b7f151fb7b2003ce3bc.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/5/8/587a9c7f1e8be39a87cd362cea54160aebd3bc2f.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/f/9/f91788077ab89159576faeb167ccd91549c7ffcc.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/c/f/cfc153b82d4ddffa656ccc5164883b3623832443.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/9/1/91ad5af4bc7344a99a0d0c6abd32331cff54542b.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/8/6/8624fb6b8bf3c717fdf8d2540af7a3d38c768561.jpg" width="375" height="500">

More pics I did not post before:

<img src="/uploads/db1493/original/3X/5/2/52bb8d4cbb64786f3ebcab43d4812f2354075ee2.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/2/a/2a6c5803bbb5fb28fbd798a3284a9381ec20e9fe.jpg" width="666" height="500">
```

---
## \#28 Posted by: TranxFu Posted at: 2017-03-07T20:13:02.881Z Reads: 220

```
Is it regripped on top ? These holes look so painful :D How did you split up the Pack ? I assume one side is VESC + Switch/BMS + cells and the other side is cells only ?
```

---
## \#29 Posted by: pyttroll Posted at: 2017-03-07T20:17:33.680Z Reads: 216

```
Yeah the top has been regripped (see first pic in last post) so you won't see the holes :slight_smile:
I have 30 cells in the front, and in the back I have the other 20 along with a BMS, the VESC, a buck converter for the lights, and Vedder's antispark switch.
```

---
## \#30 Posted by: michaelcpg Posted at: 2017-03-07T20:36:39.015Z Reads: 215

```
Nice work :) I'm about to put 60 cells on my Vanguard so will be interesting to see how that goes... :p
```

---
## \#31 Posted by: pyttroll Posted at: 2017-03-07T20:47:36.748Z Reads: 209

```
You're a brave man :)
```

---
## \#32 Posted by: jujet Posted at: 2017-03-08T09:31:30.788Z Reads: 203

```
Nice build. Your enclosures look so good, have you thought about making more and selling some for the community ? :slight_smile:
```

---
## \#33 Posted by: pyttroll Posted at: 2017-03-08T16:26:09.202Z Reads: 203

```
Thanks, unfortunately I don't have much spare time these days and I don't feel that the quality of the enclosures is good enough to be sold to third parties.
```

---
## \#34 Posted by: pyttroll Posted at: 2017-03-14T19:38:31.336Z Reads: 205

```
Test rode the board and got a bit of a scare when I lost the brakes, VESC threw an OVER VOLTAGE error. This was caused by the battery being 100% full and using the BatterySupport BMS.
I'll probably rewire the BMS for charge only... I'd rather lose a battery than my life...

Anyway, the board is super fun to ride, here's a vid of my neighbor, he came running out when he saw me, I think he's hooked.

https://youtu.be/0GrX1WYJCrw
```

---
## \#35 Posted by: Blasto Posted at: 2017-03-14T20:07:56.633Z Reads: 202

```
What's your max input voltage on the vesc? Should be 57V
```

---
## \#36 Posted by: pyttroll Posted at: 2017-03-14T20:15:03.507Z Reads: 198

```
Yes, it's 57V.
```

---
## \#37 Posted by: pyttroll Posted at: 2017-06-09T17:46:00.145Z Reads: 170

```
FYI, today I've hit my max top speed on the build, 46 kph, I'm currently running 90mm ABEC and 16/36 gearing. I'm also getting a range of about 60km.
```

---
## \#38 Posted by: Eboosted Posted at: 2017-06-09T19:29:00.474Z Reads: 171

```
46 kph? Damn! that's fast. 

Be careful and wear a helmet
```

---
## \#39 Posted by: pyttroll Posted at: 2017-06-09T19:40:29.237Z Reads: 176

```
<img src="/uploads/db1493/original/3X/3/a/3a0c7b6b3948b428ab50040c93726b9d0f30c400.jpg" width="375" height="500">
```

---
## \#40 Posted by: sMATTEr Posted at: 2017-06-09T20:11:35.909Z Reads: 166

```
This gives my ideas for my next build, wifey will not be pleased..  😆 Nice work!
```

---
## \#41 Posted by: Eboosted Posted at: 2017-06-09T20:43:41.894Z Reads: 157

```
I'm waiting on that helmet from the GB, it might take a while to get it though

Where did you buy it and how much did you pay for it?
```

---
## \#42 Posted by: Blucas Posted at: 2017-06-09T20:56:00.211Z Reads: 158

```
Hold up. 60km?!?!
```

---
## \#43 Posted by: pyttroll Posted at: 2017-06-09T21:30:20.371Z Reads: 167

```
Local skate shop, 288.15$ Canadian + tax
```

---
## \#44 Posted by: Eboosted Posted at: 2017-06-09T21:57:28.452Z Reads: 166

```
Would you please take a picture with the visor lifted?
```

---
## \#45 Posted by: pyttroll Posted at: 2017-06-10T17:05:27.367Z Reads: 161

```
<img src="/uploads/db1493/original/3X/d/8/d8d720931b5c00d70d811b000334f214396d0914.JPG" width="375" height="500">
```

---
## \#46 Posted by: pyttroll Posted at: 2017-06-10T17:06:33.741Z Reads: 164

```
<img src="/uploads/db1493/original/3X/3/4/345c72fbdef733976ab5761ca2ebd1f1e859aa3c.JPG" width="375" height="500">
```

---
## \#47 Posted by: Eboosted Posted at: 2017-06-11T08:41:39.737Z Reads: 159

```
Wow it looks amazing! Best sun glasses ever!
```

---
## \#48 Posted by: pyttroll Posted at: 2017-06-11T12:38:21.660Z Reads: 144

```
Snapchat Spectacles :slight_smile:
```

---
