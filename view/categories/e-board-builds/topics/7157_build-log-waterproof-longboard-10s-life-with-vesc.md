# Build Log: Waterproof longboard 10s LiFe with Vesc

### Replies: 119 Views: 18688

## \#1 Posted by: ndwallick Posted at: 2016-08-05T05:11:52.454Z Reads: 1153

```
I am starting my second build and I thought I would post all my progress here. :smile:

goals for this build:
1) entirely waterproof, I want to be able to ride it through pouring rain and puddles (anyone have tips for waterproofing?)
2) easy to charge, I want a BMS on board that allows for a 2 wire charger
3) better ground clearance than my last board
4) remote that doesn't try to kill me when it looses connection: :sweat_smile:

Heres what I have so far:

Arbor snowboard style deck
Calliper trucks
Kegel Wheels
Ceramic bearings
Pulley from DIY Electric skateboard
Vesc from Ollin Board Company
170 KV motor from Ollin Board Company
LiFe batteries from Hobby King (5 2s batteries)

<img src="/uploads/db1493/original/2X/c/ccc8264336767c9df0e7dcc1cfaaabd9b43474be.JPG" width="666" height="500">

I also just finished making this MOSFET switch:
http://www.electric-skateboard.builders/t/eboard-mosfet-switch/5738
```

---
## \#2 Posted by: lox897 Posted at: 2016-08-05T05:55:32.384Z Reads: 1039

```
[quote="ndwallick, post:1, topic:7157"]
entirely waterproof, I want to be able to ride it through pouring rain and puddles (anyone have tips for waterproofing?
[/quote]

Maybe some adhesive rubber between the enclosure and board? Also try some silicone as extra protection.
```

---
## \#3 Posted by: JdogAwesome Posted at: 2016-08-05T23:44:45.143Z Reads: 1020

```
Build sounds awesome and that's a beautiful deck you got there! I don't have many tips of waterproofing other than, THATS A GREAT IDEA cause I've had numerous problems with water corroding contacts and messing with other things.
```

---
## \#4 Posted by: ndwallick Posted at: 2016-08-06T00:03:07.871Z Reads: 1027

```
Thanks!

I just bought this fuse today from autozone, its 80 amps and it says its rated for 32 volts, but I read numerous things online that said they will work with higher voltages (I will have a max of 36 volts)
Has anybody tried these fuses, I will probably solder the blades to a connector to attach it.
<img src="/uploads/db1493/original/2X/4/49b753f6892422c908ded8c9b653c9a9c61926f4.JPG" width="375" height="500">
```

---
## \#5 Posted by: Jinra Posted at: 2016-08-06T00:06:16.638Z Reads: 968

```
Why not get a [fuse holder?](https://www.amazon.com/Bussmann-HHX-Maxi--Line-Holder/dp/B000CZ2Z92/ref=sr_1_22?s=automotive&ie=UTF8&qid=1470441879&sr=1-22). Fuses trip by heat, so I imagine putting a soldering iron to it may trip the fuse if heated up for too long.
```

---
## \#6 Posted by: JdogAwesome Posted at: 2016-08-06T05:06:51.302Z Reads: 949

```
Yeah like @Jinra said definelty get a fuse holder, I got some cheap one at AutoZone that works really well for a different project of mine. Also I think an 80A fuse might be a little overkill, I think a 50-60A would work just fine. Oh and with fuses voltage definelty doesn't matter as long as your not exceeding it by a ton, what matters is amperage, that's why people like using 12S2P for example not 6S6P because they need less current from the higher voltage battery.
```

---
## \#7 Posted by: kyo Posted at: 2016-08-06T05:39:09.184Z Reads: 947

```
Maybe this could help with the water resistance 

http://www.electric-skateboard.builders/t/maybe-this-can-help-your-eboard-in-some-wet-situations-neverwet/4833
```

---
## \#8 Posted by: ndwallick Posted at: 2016-08-07T16:31:52.511Z Reads: 900

```
Good point @Jinra and @JdogAwesome I will check autozone for a fuse holder.

Also will try neverwet for the pcb in whatever remote I get. As for the board, I would like to seal it off completely because I don't want to take the heat shrink off my vesc and spray it.
```

---
## \#9 Posted by: racidon Posted at: 2016-08-07T16:49:51.856Z Reads: 891

```
Get an enclosure for your VESC and use SikaFlex (from auto store) to seal up any possible water issues
```

---
## \#10 Posted by: ndwallick Posted at: 2016-08-07T18:56:44.921Z Reads: 951

```
Update:
I just hooked up the sensors on my OM5065 to the Vesc. There is definitely less cogging when I hold the motor still with my hand on my desk.

The only major parts I need to buy now are a remote and a BMS.
Having trouble finding a BMS for 10s LiFe.

I plan on milling my own motor mount for the caliper trucks. I want it to be completely adjustable so I can change pulley sizes and bring it closer to the deck if I add bigger risers, so this is what I designed:
<img src="/uploads/db1493/original/2X/3/3fc6d8421ba22bd3b85859345c0eba3207de4138.jpg" width="386" height="500">
<img src="/uploads/db1493/original/2X/e/ea540483543c7904089502b3e5e91121f8d474a6.jpg" width="386" height="500"
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-07T19:00:50.549Z Reads: 900

```
How about this one http://www.bestechpower.com/32v10spcmbmspcbforlifepo4batterypack/BMS-D270.html

That mount looks pretty swanky. Torqueboard's mount looks pretty good as well if you're considering a commercial one.
```

---
## \#12 Posted by: ndwallick Posted at: 2016-08-07T20:44:00.602Z Reads: 919

```
That one looks like it will work thanks! Just emailed them asking for the price.

I checked Autozone for a fuse holder and I only found ones for the smaller fuses so I gave soldering a shot and it worked surprisingly well. My system still works and it still doesn't trip under load (my hand stopping the motor)
<img src="/uploads/db1493/original/2X/4/416848e2aad163cf3a55ca7657ff08982e32a885.JPG" width="666" height="500">
```

---
## \#13 Posted by: Jinra Posted at: 2016-08-07T21:04:26.181Z Reads: 892

```
Cool! glad it worked out. Seems like it should work fine as long as your fast when soldering. You can get the fuse holder I linked above on amazon for the future, though with an 80A fuse, I doubt you'll ever blow it.
```

---
## \#14 Posted by: ndwallick Posted at: 2016-08-10T05:41:55.382Z Reads: 894

```
I've been emailing back and forth with BesTech and this is the BMS we ended up on. Wanted to post it here before I buy it so I can make sure there are no problems with it. It has a really low discharge rate because I won't be discharging through it, this kept it really small.

<img src="/uploads/db1493/original/2X/c/c810daf4d94544bddd4023f66e69428733237828.jpg" width="353" height="500">
```

---
## \#15 Posted by: ndwallick Posted at: 2016-08-10T22:16:31.470Z Reads: 833

```
So after discovering how hard it will be to get somebody to mill my motor mount/help me mill it, I have decided to buy the one @Jinra recommended: [link](diy-electric-skateboard-kits-parts/single-bolt-on-motor-mount-only/)

Should I get the one designed for 50 mm motors or 63 mm motors? @torqueboards 
I have a 50mm OM5065, but I have seen 50 mm motors with smaller bolt spacing. My motor bolt spacing is about 38 mm or 27 mm depending on how you measure.
```

---
## \#16 Posted by: Jinra Posted at: 2016-08-10T22:17:56.311Z Reads: 818

```
His mount does **not** fit chaka's motors FYI. He's working on getting one that does, but it currently will not fit. I'm using Enertion's mount right now and it fits perfectly.
```

---
## \#17 Posted by: torqueboards Posted at: 2016-08-10T22:30:36.215Z Reads: 826

```
@ndwallick - what @jinra said. @chaka is difficult wanted to use some odd motor mount spacing :slight_smile: 

I do have some v3 motor mounts which will fit Chaka's mount but the latest v4 motor mount doesn't.
```

---
## \#18 Posted by: ndwallick Posted at: 2016-08-10T22:46:07.908Z Reads: 829

```
hhhmmm good thing i didn't buy the 50 mm one yet haha. How much for a V3 mount? also what do they look like? Can I see some pictures? @torqueboards
```

---
## \#19 Posted by: jrpwit Posted at: 2016-08-11T05:04:01.502Z Reads: 838

```
In my opinion the enertion mount is best for chaka's motors at the moment but... cause u asked here the v3 mount. BANG! 
<img src="/uploads/db1493/original/2X/e/ef98219b4381b1b30b2b9564b194e55b3e22f5ae.jpg" width="275" height="183">

I love my v4 mount tho!
```

---
## \#20 Posted by: Mrmoonlight Posted at: 2016-08-11T05:33:54.599Z Reads: 829

```
Besides sealing the deck so it's waterproof, have you thought of a way to keep your bearings dry? I know a lot of heavy grease would help. Maybe a hub cab like some of the hub motors have, but without a hole in the center.
```

---
## \#21 Posted by: ndwallick Posted at: 2016-08-11T06:17:03.819Z Reads: 783

```
@jrpwit  Oh yaaaa I remember seeing that mount before. Looks like the V4 is a big improvement. I wish it worked with my motor. It looks like the Enertion mount would be the best for me, but the blue will throw off my color scheme. Maybe I can paint it.

@Mrmoonlight I've solved that problem with these [ceramic bearings](https://www.amazon.com/gp/product/B00KQPJUKA/ref=od_aui_detailpages00?ie=UTF8&psc=1).
```

---
## \#22 Posted by: Mrmoonlight Posted at: 2016-08-11T06:52:45.954Z Reads: 772

```
Nice, what are the races made out of? Aluminum? Stainless? Might have to get me a set.
```

---
## \#23 Posted by: ndwallick Posted at: 2016-08-11T15:33:47.579Z Reads: 788

```
Not sure, I just know they are know for working well with water. I'm curious too now what the rails are made of,  guessing stainless.
```

---
## \#24 Posted by: ndwallick Posted at: 2016-09-20T01:43:15.687Z Reads: 798

```
I finally got my motor mount machined!
<img src="/uploads/db1493/original/3X/8/7/87637a900bf7dab8a6fc0200a7f87871294156f4.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/1/1/111093dac4920de66b90000c21af022858e2491f.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/3/0/3060cb1af49190d1f87ec7d5991808f7a2f47bad.JPG" width="375" height="500">
```

---
## \#25 Posted by: ndwallick Posted at: 2016-09-23T07:14:49.905Z Reads: 752

```
Now that I have all the major parts for my build, the next step is an enclosure, or 2 enclosures. I bought this [kydex](http://www.ebay.com/itm/Kydex-T-Plastic-Sheet-1-8-x-24-x-36-Calcutta-Black-/141935594480) on ebay and I'm going to thermoform it similar to how @stealth71 did [here](http://www.electric-skateboard.builders/t/thermoforming-a-kydex-battery-enclosure/8642/17). I just want to completely seal it up by adding a rubber material around the perimeter and using waterproof epoxy wherever wires or anything comes out.
<img src="/uploads/db1493/original/3X/d/8/d845fc913c2306ec6ef82bb6030b29f97cc813c8.JPG" width="690" height="372">
```

---
## \#26 Posted by: stealth71 Posted at: 2016-09-23T13:32:09.310Z Reads: 743

```
I look forward to seeing how it comes out.
```

---
## \#27 Posted by: Luke Posted at: 2016-09-24T20:25:56.756Z Reads: 741

```
If you have an unlimited budget for bearings then these full ceramic ones ought to help 
http://www.vxb.com/Set-of-8-608-2RS-Full-Ceramic-Skate-8x22x7-p/fullceramic608-2rs.htm
If you don't want to spend that much I recommend zealous bearings as they incorporate a high tech grease to minimize corrosion. 
Also you're going to have issues with traction in the rain, especially with that drive wheel. If you have access to a lathe or I suppose the motor does a similar job you can do this to give you avoid aqua plaining 
http://www.telusplanet.net/public/gary2a/CS/rainwheels/rain.jpg
```

---
## \#28 Posted by: ndwallick Posted at: 2016-09-24T22:42:46.978Z Reads: 705

```
wow those are expensive bearings! I'll probably stick with the cheap ceramics I have for now. Good idea for the grooves in the wheel. I'll try to rig something up to cut those using the motor to spin the wheel.
```

---
## \#29 Posted by: chuttney1 Posted at: 2016-09-25T00:19:53.993Z Reads: 702

```
Nice grooves, but I'll have to say these are terrible in riding through water even though the purpose of putting groves is giving water a way to move through urethane. Putting groves are terrible because it kicks up so much water while riding on wet pavement.
```

---
## \#30 Posted by: Luke Posted at: 2016-09-25T00:23:54.415Z Reads: 731

```
[quote="chuttney1, post:29, topic:7157"]
ice grooves, but I'll have to say these are terrible in riding through water even though the purpose of putting groves is giving water a way to move through urethane. Putting groves are terrible because it kicks up so much water while riding on wet pavement.
[/quote]

To be honest I've never done it myself, only seen other longboarders do it. They did not report water kicking up but they may not have been looking out for it or been too worried about it with non electric boards
https://www.youtube.com/watch?v=1fWt1PyqMJY
Found that video of some commercial wheels with grooves, they dont seem too bad
```

---
## \#31 Posted by: ndwallick Posted at: 2016-09-28T08:30:56.772Z Reads: 727

```
Alright so I finally got a chance to attach everything temporarily and ride it for the first time.:grinning:
<img src="/uploads/db1493/original/3X/1/e/1ebe72cb38a7452836dcb1fb18fbe3360b3f20f8.JPG" width="666" height="500">
It's a great feeling when you can finally use something you've been working for a while. My winning remote works great. The vesc works surprisingly well sensorless when starting from 0. I probably won't use the sensors for the sake of waterproofness. I wouldn't want water to short out the sensors in the motor and ruin the vesc.

The only problem is it only goes 17 mph. My last board I calculated to go 20 mph and it went 18 mph, so I assumed that since I calculated this one to go 22 mph it would go about 20. But it went 17.

I just recently found out that LiFe batteries have a voltage sag when under load so I hooked my multimeter up to the batteries and rode at full speed. The voltage dropped from 33.4 volts to 32 volts. So that must not be the only reason it goes so much slower that calculated.

How big is everyone else's difference from calculated speed and actual speed?

Anyway to fix this problem I will probably have to increase my motor kv to 200. This will give me a calculated speed of 25.7 mph so it should really go 19 to 20. (then if I want a little more speed I can up the gear ratio (it's already pretty high at 15:36))

Hey @chaka can I send you my OM5065 170 kv motor and exchange it with a 200 kv one?:relaxed: I barely used it, it still looks brand new.

I also just got the Kydex I ordered and I will soon start making an enclosure.
```

---
## \#32 Posted by: chaka Posted at: 2016-09-28T13:54:06.639Z Reads: 699

```
Yeah, go ahead and send it back. I can use it on a campus cruiser prototype. The VESC runs at 95% max so you need to calculate for that when running numbers.
```

---
## \#33 Posted by: ndwallick Posted at: 2016-09-29T23:44:52.286Z Reads: 746

```
Thanks @chaka! I just mailed it, it should be there on Monday
```

---
## \#34 Posted by: ndwallick Posted at: 2016-10-04T02:16:26.719Z Reads: 784

```
I just finished the forming part of my kydex enclosure using @stealth71 s method [here](http://www.electric-skateboard.builders/t/thermoforming-a-kydex-battery-enclosure/8642). It turned out great :grinning: . I used the 1/8 inch kydex which is the thickest I could find and it was very difficult to form but it's extremely strong.

First I made this wood piece to simulate the shape of my batteries:
<img src="/uploads/db1493/original/3X/5/5/5556e957e26dc4fb1b289902ca81145b05b9dda1.JPG" width="666" height="500">
I glued it to the deck and laid the hot kydex over it and clamped it with foam for about 15 minutes. The corners weren't very well defined at all at this point:
<img src="/uploads/db1493/original/3X/d/c/dcbcdf4f66ee1cf8a13aefcc1b472e6693412f70.JPG" width="666" height="500">
Then after a lot of using the heat gun and pushing the corners in with a paint stick, then lots of sanding, I got this:
<img src="/uploads/db1493/original/3X/b/d/bd0abad2f0b5d9140e9703a7ce36a91707e681c1.JPG" width="666" height="500">

This was pretty much an all day job with how hard the 1/8 inch kydex is to form, but it's well worth the extra strength for me. Next I just have to drill some holes and find the right hardware.
```

---
## \#35 Posted by: stealth71 Posted at: 2016-10-04T12:12:29.401Z Reads: 735

```
Nice work!!
```

---
## \#36 Posted by: Jebe Posted at: 2016-10-04T12:22:14.744Z Reads: 743

```
Am waiting on this deck from the nile myself ! The walnut looks awesome
```

---
## \#37 Posted by: ndwallick Posted at: 2016-10-05T21:12:44.155Z Reads: 763

```
Finally got the hardware in. I countersunk all the bolts to be flat with the top of the board and it looks super clean :grinning:
<img src="/uploads/db1493/original/3X/d/9/d95889d363b13f4df560a88044ad0ebeeb768797.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/a/1/a1b760c50bc14a80ad40a631d59fb12b0658d57b.JPG" width="666" height="500">

@stealth71 thanks! 
@Jebe good choice it's a nice deck
```

---
## \#38 Posted by: Jebe Posted at: 2016-10-05T21:51:53.876Z Reads: 736

```
nice work on that kydex :thumbsup:
```

---
## \#39 Posted by: Stevemk14ebr Posted at: 2016-10-05T21:54:33.473Z Reads: 731

```
why so many bolts? The enclosure looks great.
```

---
## \#40 Posted by: ndwallick Posted at: 2016-10-05T22:22:30.631Z Reads: 738

```
haha I knew somebody was gonna ask that, for watertightness. I'm gonna put some kind of rubber sheet between the kydex and the board and I just wanted to make sure the entire perimeter is tight against the rubber.
```

---
## \#41 Posted by: Kaly Posted at: 2016-10-05T22:58:59.290Z Reads: 710

```
@ndwallick you can use thin double sided tape and pvc sheet to waterproof that enclosure
```

---
## \#42 Posted by: Jebe Posted at: 2016-10-05T23:31:43.296Z Reads: 744

```
Look what turned up today ! :slight_smile: got a spare enclosure handy ? :stuck_out_tongue: 
<img src="/uploads/db1493/original/3X/1/7/173dc8e1c23d1a771ff712bbcbb90f564838c171.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/4/2/426e846be5fd328fca449e2896d5545ee2f4ba8d.jpg" width="281" height="500">
```

---
## \#43 Posted by: ndwallick Posted at: 2016-10-05T23:38:38.485Z Reads: 690

```
Awesome! and nope I've only made that one enclosure
```

---
## \#44 Posted by: tueboard Posted at: 2016-10-06T13:38:24.908Z Reads: 685

```
how many degrees celsius and time you need to mold the kydex with the heat gun?
```

---
## \#45 Posted by: ndwallick Posted at: 2016-10-06T14:32:04.142Z Reads: 727

```
I put it on a sheet of cardboard In a convection oven and set it to 330 farenheight (166 Celsius). It was probobly in there for 10 minutes. I just kept feeling it with gloves to see how flexible it got then took it out when it was soft enough.

Then after molding it I used a heat gun to finish off the corners. I had to use the low setting on it cause the high setting makes the surface too hot and messes up the texture.

I just heated a certain area (keep the heat Hun moving a bit) then held it onto position with some cardboard while it cooled.

Good luck!
```

---
## \#46 Posted by: ndwallick Posted at: 2016-10-07T00:09:39.065Z Reads: 744

```
I can confirm that a yoga mat works very well as a watertight seal. I put this piece of one between my enclosure and deck, filled the enclosure with water before I bolted it on, shook it around and no water comes out at all! If water can't get out then it can't get in. I just have to cut the mat to the right shape now.
<img src="/uploads/db1493/original/3X/8/3/83f9f6f185ef162f0ed9a6620b5828b993fce69c.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/9/19f656873da04f788a68c3c833517e855eb46abc.JPG" width="666" height="500">'

If anyone's gonna do this I suggest a thin yoga mat with not a lot of texture on it.
```

---
## \#47 Posted by: ndwallick Posted at: 2016-10-07T23:57:25.246Z Reads: 735

```
just got everything squeezed into the battery enclosure, it's a really tight fit. I am using parts of a yoga mat on all sides of the battery to hold it in place and to dampen vibrations. I used corrosion X on the BMS (its under the fuse, hard to see in the pic) just in case water gets in and I used Loctite marine adhesive sealant to seal the holes where the power wires and the charging port come out.
<img src="/uploads/db1493/original/3X/e/7/e7031cbb5e540ee19e84703ad44fbbdffca346da.JPG" width="375" height="500">
```

---
## \#48 Posted by: stealth71 Posted at: 2016-10-10T14:02:42.257Z Reads: 721

```
Looking good!
```

---
## \#49 Posted by: brandon Posted at: 2016-10-10T15:22:58.136Z Reads: 716

```
What kind of connectors are you using for charging?
```

---
## \#50 Posted by: ndwallick Posted at: 2016-10-10T20:53:43.655Z Reads: 727

```
I'm using xt60 connectors for charging. Here's what the outside of the enclosure looks like:
<img src="/uploads/db1493/original/3X/c/3/c39db32d47e4e05b9d4a85501e787758d85fc042.JPG" width="375" height="500">
I'm gonna make a cover for the charging port on the board to keep it from shorting out.

and here's my charger: (I just bought it without a connector on it and soldered that one on)
<img src="/uploads/db1493/original/3X/4/9/4907b070cba1b034215c73d3e73aa34280c421b7.JPG" width="666" height="500">
```

---
## \#51 Posted by: ndwallick Posted at: 2016-10-10T20:56:05.726Z Reads: 691

```
Also shoutout to @chaka for letting me exchange my 170 kv motor with a 200 kv one! I just got it a couple days ago. Happy I went with his motor instead of a HK one.
```

---
## \#52 Posted by: IDVert3X Posted at: 2016-10-10T21:05:02.647Z Reads: 695

```
How are you going to seal the XT60 on the outside of the case?
I found some rubber covers on eBay but they doesn't seems to be waterproof.
```

---
## \#53 Posted by: ndwallick Posted at: 2016-10-10T21:13:39.724Z Reads: 705

```
I'm gonna use a male xt6 connector with some hot glue over the places you normally solder to. Water may still be able to touch the terminals but it won't get into the enclosure because of all the sealant I put on the inside around the connector.

<img src="/uploads/db1493/original/3X/1/d/1df7fa1834e54dc29ccca168c60ebcbaea4577b1.JPG" width="690" height="442">

It won't be a super big deal if water shorts the terminals (as long as it's not salt water) because water isn't that conductive. Same reason you can spray a car engine down with a hose and the battery will be fine even though the connectors are exposed.

Water mainly causes problems with circuitboards that are very sensitive to being shorted just a little bit. But also I will put some Corrosion X on the terminals just to be safe.
```

---
## \#54 Posted by: IDVert3X Posted at: 2016-10-10T21:27:13.461Z Reads: 688

```
On the battery terminals, you have 42V.
The resistivity of the drinking ( not salt ) water is 2-200 Ohms at 20C ( according to Wikipedia ).
In the worst case, 42V/2R=21A which is not a big deal for our battery packs.
But 21A*42V=882W of energy wasted. How much heat is that? :D
```

---
## \#55 Posted by: ndwallick Posted at: 2016-10-10T22:05:45.159Z Reads: 702

```
Very good point, my batteries are actually ~33 volts so that's about 16.5 amps if water bridges the terminals. Those terminals are connected the the BMS which I know has some kind of over current protection. But that still would be bad. I wouldn't want my BMS to keep shutting them off and back on. Sooooo that's what the Corrosion X is for :grinning: 
https://www.youtube.com/watch?v=s4z8QMgTEA4

Also I'm sure the resistivity of water changes based on distance and the "thickness" of the water bridging the terminals. I wonder exactly how many ohms it will be in this situation.

I'm going to do a little experiment on this I'll post it here when I'm done.
```

---
## \#56 Posted by: ndwallick Posted at: 2016-10-10T22:40:27.406Z Reads: 687

```
Alright i just did the experiment. Here's what I did:

I took some spare lipos I had (22.2 volts total) and hooked them up to my multimeter in amp mode and a female xt60 connector. I then dipped the connector into tap water from my sink and checked the amperage. I sprayed Corrosion X on the female xt60 connector and I dipped it again.

results:
without corrosion x: 0.015 amps
with corrosion x: 0.003 amps

This is how many amps the water allows with the connector fully submerged, so I think it will be pretty safe on the bottom of my board with water just spraying on it. :grinning:

Amps will be a little higher on my 33 volt batteries but should be pretty close.
```

---
## \#57 Posted by: IDVert3X Posted at: 2016-10-11T05:59:02.619Z Reads: 662

```
Thats interesting. That would mean the water has resistivity of around 1500Ohms. Anyway, good to hear it works fine to you.
```

---
## \#58 Posted by: ndwallick Posted at: 2016-10-20T02:38:21.811Z Reads: 698

```
The second enclosure is done!
This one was actually a lot harder to form because the kydex had to stretch and compress more because if the smaller size. But it still turned out pretty good.
<img src="/uploads/db1493/original/3X/a/9/a9a56d4218461abec43243fdddae372cfdd5605c.jpg" width="666" height="500">

Got all the electronics in it and sealed all the holes with loctite marine epoxy. I also used a yoga mat again between the board and the deck.
<img src="/uploads/db1493/original/3X/d/9/d9e68867395f2bccd77540f36231cc0a602abebf.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/0/3/037208ef0663f376f90fb4e372e947db0717d678.jpg" width="666" height="500">

And here's the (mostly) completed board!
<img src="/uploads/db1493/original/3X/7/f/7f7c7b865d6453db6df6b6464031ea324e956ace.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/b/e/be53b5b004629e7f439cdc5c0aab1124f8c453fc.jpg" width="666" height="500">
```

---
## \#59 Posted by: LivingLongboard Posted at: 2016-10-21T17:19:30.360Z Reads: 670

```
That looks sick with the LED light
```

---
## \#60 Posted by: ndwallick Posted at: 2016-10-22T22:37:51.055Z Reads: 697

```
My board is officially complete! :grinning:
Here are some pictures of it:
<img src="/uploads/db1493/original/3X/b/e/be53b5b004629e7f439cdc5c0aab1124f8c453fc.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/4/5/451ef1cc7ad39534ef4c04a7ab13e2d02df9ad78.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/0/3/03599603b288101ddbaa8329ea1ac586a0f04ad4.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/5/7/571f8ef8d8672af292a8844f3171c52dae5576fe.jpg" width="666" height="500">

Here are the measured specs:
top speed: 20 mph
range: 11 miles (farther than I expected)
charge time: about an hour (charging at 1C)
weight: only 15 pounds

I meet all the goals I set for this build. It's (most likely) completely waterproof. I've only rid it through puddles so far but it's been doing fine. It's easy to charge with the BMS. The batteries are a safe chemistry (LiFe) so they shouldn't ever catch on fire. The ground clearance is great, and the winning remote is working pretty well for me (I've only had a few drop outs when I'm pulling lots of amps. I am gonna try more loops around the ferrite ring).

Also I haven't posted anything about my Arduino battery meter here yet. I wanted an easy way to see how much battery life I had left so I made this:
<img src="/uploads/db1493/original/3X/3/a/3a4c889381ea1a1a8dc89fd05b3ee0a3af6ecc31.jpg" width="666" height="500">
This circuitboard has @JdogAwesome's [mosfet switch](http://www.electric-skateboard.builders/t/eboard-mosfet-switch/5738?source_topic_id=7157) and an arduino that I've programmed to read the battery voltage and display it on 5 LEDs on the outside of the board.

I've found that just reading voltage isn't the best way to monitor LiFe batteries because their voltage goes up and down a lot depending on load but it works good enough. :grinning:

I'd like to thank all these people for making this board possible: :slight_smile:
@JdogAwesome for the mosfet switch
@torqueboards for the wheel pulley kit
@chaka for the vesc and motor
Benjamin Vedder for designing the vesc
@stealth71 for the [kydex enclosure idea](http://www.electric-skateboard.builders/t/thermoforming-a-kydex-battery-enclosure/8642)
@onloop for making this forum possible
and everyone else here for posting their builds and ideas.



Some things I still want to add in the future:
a headlight for seeing the road better at night
a handle
change from 9mm to a wider belt
a gps tracker (any ideas for this?)
```

---
## \#61 Posted by: ThomasRBK Posted at: 2016-10-22T23:00:14.408Z Reads: 628

```
Board looks really clean man, love it!
```

---
## \#62 Posted by: JdogAwesome Posted at: 2016-10-23T01:43:04.355Z Reads: 620

```
Wow this board is beautiful! Im happy you liked the design of my switch and I hope it fits your needs!
```

---
## \#63 Posted by: torqueboards Posted at: 2016-10-23T02:11:36.689Z Reads: 626

```
Nice :)  We have 12mm Kegels now btw. They are a much nicer/durable fit than the previous versions.
```

---
## \#64 Posted by: ndwallick Posted at: 2016-10-23T23:08:10.240Z Reads: 674

```
I've had a few people ask me how I did the Arduino battery meter so here's how I did it: :grinning:
I'm writing this assuming basic arduino programming knowledge and goodish math knowledge.

This is how the Arduino reads the battery voltage:
<img src="/uploads/db1493/original/3X/9/1/914b8c28814f2a965f3e9fac18cd797605ea09d6.jpg" width="666" height="500">
The Arduino analog pins can read anything from 0 to 5 volts so I just used resistors to drop the main voltage down before connecting to an analog pin. The voltage will still be proportional to the main voltage.

So now that the arduino can read the battery voltage it just needs to know what voltage correlates to what capacity. Since my LiFe batteries don't discharge linearly I had to find an equation for the discharge curve. To do this I charged my battery fully then rode my board until it died, checking the battery voltage with a multimeter every mile and writing it down (I used the app Strava to know how many miles I had gone).

Once I had a table of data (distance traveled and voltage) I put the data in my calculator and used the calculators built in quartic regression to find an equation for the curve:
<img src="/uploads/db1493/original/3X/4/9/49d25e8ae1f8ab0f0273a78592a16a97084584f2.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/d/1d6af1532d7f32e68747431a200262a16420549a.jpg" width="666" height="500">

I put 5 LEDs on my board so I decided my battery meter would have 6 states: (1 means LED on and 0 means LED off)

<img src="/uploads/db1493/original/3X/f/6/f6f3d22c2442db6443b88b5b7b2752301d2e497f.jpg" width="666" height="500">

Then I just had to use the equation to find out what the battery voltage would be at every increment. 
<img src="/uploads/db1493/original/3X/5/0/504a1d4ce009d0de373076f915157f66cdfa1feb.jpg" width="417" height="500">

The arduino analogRead() function doesn't directly read the voltage. It only reads a fraction of the voltage determined by the resistors used in the first picture. It also doesn't return the value of the voltage, it returns a number 0 through 1023 (0 being 0 volts and 1023 being the reference voltage(the reference voltage is really close to 5 volts)).

So now I had to find an equation that relates the battery voltage to the number the arduino analogRead() function returns. This is way easier than the last equation because it will be a linear one. I just needed two data points:

first data point:
battery voltage: 0
analogRead(): 0

second data point:
battery voltage: 33.6
analogRead(): 748

To find the second data point I just measured the battery with a multimeter and used the arduino serial monitor to display the results of analogRead().

Then I plugged these into my calculator and used linear regression to find an equation. I used that equation to translate all the battery voltage increments into what analogRead will say at those voltages:
<img src="/uploads/db1493/original/3X/5/5/55ba92ae04b991f6af96eda5baf823e5e60e2a22.jpg" width="375" height="500">

So now I know what increments to change the LEDs at, time to program the ardiuno! The ardiuno code is really simple, here it is:

//longboard battery meter code
//Nick Wallick 10/20/16

int delayTime = 100;
int battery;
int flashingTimer = 0;

void setup() {
  // put your setup code here, to run once:
  pinMode(A7, INPUT);
  pinMode(8, OUTPUT);
  pinMode(9, OUTPUT);
  pinMode(10, OUTPUT);
  pinMode(11, OUTPUT);
  pinMode(12, OUTPUT);

  startupAnimation();
  startupAnimation();
}

void loop() {
  //reads pin attached to resistors and battery
  battery = analogRead(A7);

  //BATTERY AT 5 BARS///////////////////////////////
  if (battery >= 750){
    digitalWrite(8, HIGH);
    digitalWrite(9, HIGH);
    digitalWrite(10, HIGH);
    digitalWrite(11, HIGH);
    digitalWrite(12, HIGH);
  }
  //BATTERY AT 4 BARS///////////////////////////////
  if (battery < 750){
    if (battery >= 741){
      digitalWrite(8, LOW);
      digitalWrite(9, HIGH);
      digitalWrite(10, HIGH);
      digitalWrite(11, HIGH);
      digitalWrite(12, HIGH);
    }
  }
  //BATTERY AT 3 BARS/////////////////////////////////
  if (battery < 741){
    if (battery >= 737){
      digitalWrite(8, LOW);
      digitalWrite(9, LOW);
      digitalWrite(10, HIGH);
      digitalWrite(11, HIGH);
      digitalWrite(12, HIGH);
    }
  }
  //BATTERY AT 2 BARS///////////////////////////////
  if (battery < 737){
    if (battery >= 734){
      digitalWrite(8, LOW);
      digitalWrite(9, LOW);
      digitalWrite(10, LOW);
      digitalWrite(11, HIGH);
      digitalWrite(12, HIGH);
    }
  }
  //BATTERY AT 1 BAR///////////////////////////////
  if (battery < 734){
    if (battery >= 724){
      digitalWrite(8, LOW);
      digitalWrite(9, LOW);
      digitalWrite(10, LOW);
      digitalWrite(11, LOW);
      digitalWrite(12, HIGH);
    }
  }
  //BATTERY AT FLASHING///////////////////////////////
  if (battery < 724){
    if (battery >= 683){
      if (flashingTimer > 2000){
        digitalWrite(8, LOW);
        digitalWrite(9, LOW);
        digitalWrite(10, LOW);
        digitalWrite(11, LOW);
        digitalWrite(12, LOW);
      }else{
        digitalWrite(8, HIGH);
        digitalWrite(9, HIGH);
        digitalWrite(10, HIGH);
        digitalWrite(11, HIGH);
        digitalWrite(12, HIGH);
      }
      flashingTimer = flashingTimer + 1;
      if (flashingTimer > 8000){
        flashingTimer = 0;
      }
    }
  }
  //BATTERY AT FAST FLASHING///////////////////////////////
  if (battery < 683){
    if (flashingTimer > 500){
      digitalWrite(8, LOW);
      digitalWrite(9, LOW);
      digitalWrite(10, LOW);
      digitalWrite(11, LOW);
      digitalWrite(12, LOW);
    }else{
      digitalWrite(8, HIGH);
      digitalWrite(9, HIGH);
      digitalWrite(10, HIGH);
      digitalWrite(11, HIGH);
      digitalWrite(12, HIGH);
    }
    flashingTimer = flashingTimer + 1;
      if (flashingTimer > 1000){
        flashingTimer = 0;
      }
   }
}




void startupAnimation() {
  digitalWrite(8, HIGH);
  delay(delayTime);
  digitalWrite(8, LOW);
  digitalWrite(9, HIGH);
  delay(delayTime);
  digitalWrite(9, LOW);
  digitalWrite(10, HIGH);
  delay(delayTime);
  digitalWrite(10, LOW);
  digitalWrite(11, HIGH);
  delay(delayTime);
  digitalWrite(11, LOW);
  digitalWrite(12, HIGH);
  delay(delayTime);
  digitalWrite(12, LOW);
  digitalWrite(11, HIGH);
  delay(delayTime);
  digitalWrite(11, LOW);
  digitalWrite(10, HIGH);
  delay(delayTime);
  digitalWrite(10, LOW);
  digitalWrite(9, HIGH);
  delay(delayTime);
  digitalWrite(9, LOW);  
}

The code just reads the A7 pin and turns the right number of LEDs on depending on what A7 returns.

When writing the code I decided to add fast flashing, in addition to normal flashing, if the battery gets way too low so I know to turn it off. I also added a startup animation just cause it looks cool :slight_smile: .

Hopefully this helps some people figure out how to make a battery meter!

Also here's my full electrical drawing of the circuitboard I soldered the arduino to. The wires going up on the right go to the LEDs. This circuit board also has this [mosfet switch](http://www.electric-skateboard.builders/t/eboard-mosfet-switch/5738?source_topic_id=7157).
<img src="/uploads/db1493/original/3X/1/3/13d2ee8c10db06e221b5ff7f90d19075501269be.jpg" width="666" height="500">
```

---
## \#65 Posted by: Stef Posted at: 2016-10-23T23:51:19.405Z Reads: 569

```
This is one of the most beautiful builds I've seen with external enclosures.Your enclosures along with buttons and leds just look professional. The builds I love the most are the stealth builds with a hollow wooden deck, but you have the added advantage of leaving some flex in the board for comfort! 

The only thing I think you should do make it actually waterproof is getting rid of the connector between the enclosure, and making an enclosure/spray-shield for your motor so water doesn't spray in to it. I'm also going to do a waterproof build so yours will definitely serve as inspiration!
```

---
## \#66 Posted by: ndwallick Posted at: 2016-10-24T01:30:49.694Z Reads: 560

```
Thanks so much! It would look better without the connector between the enclosures but I kinda need it for ease of maintanence. It should be fine getting wet though.

A splash guard for the motor would be good to protect the motor bearings from water. Or I can change the motor bearings with ceramic ones.
```

---
## \#67 Posted by: LivingLongboard Posted at: 2016-10-25T03:50:06.158Z Reads: 539

```
Do you have a complete list of all the parts you used?
```

---
## \#68 Posted by: JdogAwesome Posted at: 2016-10-25T06:07:47.339Z Reads: 555

```
Hey @ndwallick I love the schematic for the board and how you implemented everything, only thing I would suggest is using a small buck converter instead of the Linear one because they are 100x more efficient. Also I purchased [these](http://m.ebay.com/itm/12V-10W-LED-Round-Car-Daytime-Running-Light-DRL-Head-Lamp-Eagle-Eye-White-Light-/371422062600?txnId=873566006024) for headlights and they seem pretty bright, though I haven't tested them on my board in real conditions yet. And for the GPS thing, I've had an idea in dev for a little while now which would have a GPS module as well as UART communication with the VESC and connect via BT to your phone to get accurate info on your VESC as well as GPS based info, but don't expect anything any time soon lol.

EDIT: you may also want to slightly bump your positive side MOSFET gate driver voltage divider resistor a little, like 12K ohms because ATM gate is being given 17V which is a little closer to the max of 20V for the 3034. You should be fine at 17V but if you wanna make sure I'd go with 12K resistor. And if you really want to perfect it you could use a 12V Zener instead to give it a constant 12V.
```

---
## \#69 Posted by: ndwallick Posted at: 2016-10-25T07:14:53.558Z Reads: 546

```
Here you go @LivingLongboard I meant to post this earlier. All the parts I bought and their prices:
https ://docs.google.com/spreadsheets/d/1z52R29VjZmLlpdBmYNeP7w5TYLwirt2lKW2v7VQmexs/edit?usp=sharing

Edit: just remove the space after https. The link was causing problems

@JdogAwesome I do plan on switching to a buck converter. At first I thought a linear voltage regulator would be fine cause it is only powering an arduino but it does get pretty warm. Il also switch to the newer higher voltage mosfets that you suggested in your post and I'll change out the resistors according to whatever those mosfets need.

I'll probably just make a whole new circuitboard with all the changes and add whatever circuitry for headlights I may need. Il definitely check out those headlights they're super cheap.

Also looking forward to your GPS module!
```

---
## \#71 Posted by: Bataleon Posted at: 2016-11-04T11:18:49.019Z Reads: 494

```
Fantastic build, @ndwallick!

I'm looking at getting the same deck and 5065-200kv motor. Have you found the flex of the deck to be a problem? Also, how hot does the motor get during a riding session?

In hindsight is there anything you would've done differently with this build?

Thanks
```

---
## \#72 Posted by: ndwallick Posted at: 2016-11-04T22:17:48.405Z Reads: 482

```
Thanks! The deck has a medium flexiness to it. When I attached the kydex it definitely got stiffer but the flex didn't cause any problems.

The motor gets pretty warm but never too hot to touch.

The main thing I changed since I finished the board is upgrading to [this](diy-electric-skateboard-kits-parts/36t-kegel-pulley-combo-kit/?attribute_motor-pulley=16T+Motor+Pulley&attribute_belt-size=255mm+12mm+Wide) 12mm pulley kit because I already had a 9mm belt break.

Good luck with your build
```

---
## \#73 Posted by: Bataleon Posted at: 2016-11-04T22:30:41.120Z Reads: 464

```
Great, thanks for the info. What range are you getting with your 10S2P LiFe pack?
```

---
## \#74 Posted by: ndwallick Posted at: 2016-11-04T22:35:26.706Z Reads: 460

```
Right when I finished the build I did a range test and got 11 miles, but I was likely not pushing it very hard since I was still getting used to it. I also live in an area with no hills. So I'd guess a little less than that. The board only weighs 15 pounds so there's definitely room for more battery.
```

---
## \#75 Posted by: laikiux Posted at: 2017-01-31T19:04:39.549Z Reads: 433

```
Hi! what type of mounting hardware you are using? Can you share the site, where you bought it?
```

---
## \#76 Posted by: osbor Posted at: 2017-01-31T20:14:02.378Z Reads: 441

```
general waterproofing question
i've always wondered, are outrunner motors inherently waterproof? do you just need to watertight and insulate the connections coming off of them?
```

---
## \#77 Posted by: SageTX Posted at: 2017-01-31T20:31:51.370Z Reads: 445

```
That is correct.
```

---
## \#78 Posted by: ndwallick Posted at: 2017-02-05T04:01:46.705Z Reads: 465

```
@laikiux I designed the motor mount myself and got a friend with a machine shop to machine it for me. Here's the [design](http://www.electric-skateboard.builders/t/build-log-waterproof-longboard-10s-life-with-vesc/7157/10) and here's the [final product.](http://www.electric-skateboard.builders/t/build-log-waterproof-longboard-10s-life-with-vesc/7157/24) It turned out pretty good, I just had to cut off a corner with a saw after to get more ground clearance.

@osbor Outrunners are inherently waterproof. I believe even if the connections coming off of them get wet it will be fine. Regular water isn't conductive enough to screw them up electricaly. The motor bearings could rust though if they aren't ceramic. Water mostly causes problems with sensitive smaller electronics like circuitboards and possibly sensors on an outrunner (haven't tried those wet yet). Salt water however is more conductive and could cause problems. Here's a good [video](https://www.youtube.com/watch?v=s4z8QMgTEA4) on the topic.
```

---
## \#79 Posted by: laikiux Posted at: 2017-02-05T07:16:05.421Z Reads: 446

```
Sorry, but I asked for enclosure mounting hardware :D
```

---
## \#80 Posted by: ndwallick Posted at: 2017-02-06T03:10:29.298Z Reads: 440

```
Ohhhh I used M5 bolts that are 25mm long (threads + head) with a flat head for countersinking. Then I used M5 washers and M5 nylon lock nuts on the other side. I got everything at ace hardware. Hope that helps!
```

---
## \#81 Posted by: BpaoIce Posted at: 2017-05-05T21:08:21.573Z Reads: 421

```
Hello "first time trying to build electric longboard"
Im wondering about something, those measurements of yours, are those in mm? or?  I have a friend that have acces to cnc machine, but he could not quite understands the measurements of yours, like whats R.5250 ? appreciate if you have time to answer :smiley:
```

---
## \#82 Posted by: ndwallick Posted at: 2017-05-05T21:20:00.256Z Reads: 396

```
They are in inches. I should have had that on there, and the R.5250 means the radius is 0.525 inches. Also that circle with a line through it means diameter.

Also part A I had made on a laser edm machine. It may be kinda hard to machine with a cnc but probably possible. Good luck!
```

---
## \#83 Posted by: BpaoIce Posted at: 2017-05-05T21:32:38.709Z Reads: 377

```
Thanks for the quick reply :smile:
```

---
## \#84 Posted by: ndwallick Posted at: 2017-05-06T03:33:37.920Z Reads: 403

```
I haven't modified this build very much since I finished it, so I though it was time for some improvements.

I just replaced my vesc firmware with [Ackmaniac's](https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286) so I can have more control over the vesc with this [app](https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888). Just have to wait for a bluetooth transmitter in the mail.

Also I have some really cool plans for a headlight.
```

---
## \#85 Posted by: Conor Posted at: 2017-05-08T20:06:42.983Z Reads: 394

```
What unit of measurement is that?
```

---
## \#86 Posted by: BpaoIce Posted at: 2017-05-08T23:26:12.386Z Reads: 420

```
Another question, what kind of motor are you using on that motor mount? i have read earlier on the topic that you used a 50mm OM5065-170KV but later changed to a 200KV. Are you still using the new motor on the same motor mount? And is it possible for me to use a 50mm or 63mm motor from Turnigy SK3 series on this motor mount?
Thanks for the reply
```

---
## \#87 Posted by: ndwallick Posted at: 2017-05-08T23:55:49.174Z Reads: 445

```
@BpaoIce I am still using the 200kv OM5065 on the same mount. I just had to saw a corner off for more clearance with the deck.
<img src="/uploads/db1493/original/3X/9/9/99288f4d6bff6894cdd700d22ce3021b66c1591a.jpg" width="666" height="500">
The OM5065 has an unusual bolt spacing. Regular 50mm motors and 63mm motors have different bolt spacings.

If you're going to use a OM5065 then this mount will work but If you want a different motor I would find the bolt spacing (by emailing the manufacturer or looking it up here) then just adjust my design a little bit. It should be an easy adjustment.

@conor Not sure what you mean?
```

---
## \#88 Posted by: Bataleon Posted at: 2017-05-15T18:48:52.124Z Reads: 405

```
How's your OM5065 been holding up, @ndwallick? :) Do you often ride in the wet/rain?
```

---
## \#89 Posted by: ndwallick Posted at: 2017-05-17T01:19:38.699Z Reads: 402

```
It has been holding up really well! I dont ride it in the rain very often but It's certainly gotten wet a few times. I don't have the sensors hooked up, not sure how the rain would affect those.
```

---
## \#90 Posted by: lrdesigns Posted at: 2017-07-04T07:24:32.464Z Reads: 381

```
[quote="ndwallick, post:89, topic:7157"]
I don't have the sensors hooked up, not sure how the rain would affect those.
[/quote]

I opened mine up and epoxied over the exposed contacts as I intend to do some wet ridding and want to use the sensors. 

How is the board going? No water issues?
```

---
## \#92 Posted by: FinnishSnowmobiler Posted at: 2017-08-09T23:28:27.323Z Reads: 379

```
Great looking build. The outcome is outstanding! The only question I have about this build is that don't you get your pants really wet and dirty when driving in moist conditions? Mine isn't even near waterproof but I've played with the idea of adding some sort of mudguards to the board.

Cheers!
```

---
## \#93 Posted by: ndwallick Posted at: 2017-09-09T23:30:58.599Z Reads: 357

```
@FinnishSnowmobiler Ya riding is the rain is pretty messy!

@lrdesigns I haven't had any water issues but I recently have had some motor overheating issues. I am going to start a new thread about it.
```

---
## \#94 Posted by: Cobber Posted at: 2017-09-10T00:12:07.197Z Reads: 349

```
Looks good bro :ok_hand:
enclosure came out nice and not too hard or messy

[I'd use sugru for stuff like this](https://sugru.com/), even the mounting around the plug i'd use it there to unless your budget is super tight ;)
```

---
## \#95 Posted by: ndwallick Posted at: 2017-09-11T02:08:54.199Z Reads: 331

```
Never heard of sugru, I will have to try it!
```

---
## \#96 Posted by: ndwallick Posted at: 2017-10-02T16:52:23.671Z Reads: 331

```
I recently had my motor overheat and stop working. It was probably because I've been riding it with a backpack, and going up hills in the AZ heat. So I just bought a larger [motor](http://www.ollinboardcompany.com/product/om-6085-200kv) and a new [mount](collections/featured-items/products/single-bolt-on-motor-mount-set-only-black). I will post pics here when I have it all installed. It will be nice to have a little more power too!
```

---
## \#97 Posted by: ndwallick Posted at: 2017-10-06T15:22:26.282Z Reads: 354

```
After kicking my board for 2 weeks, I finally installed the OM6085 motor last night! It feels way more powerful than my old motor and a lot smoother too. I should have started with a 60mm motor! 

Evan after riding up a hill in 80 degree F weather, it did not get too hot to touch. I will have to see how hot it gets when it's hotter out.

<img src="/uploads/db1493/original/3X/f/f/ff4f61f0462cdee92b9774f5281e3d33c4ede121.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/c/0/c0d5c71bcb8c972fad608c013d0142b296570aa6.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/7/b/7bd39867a578074c61a45e5efcc8ad585d178d9d.jpg" width="666" height="500">
```

---
## \#98 Posted by: chaka Posted at: 2017-10-06T16:05:16.264Z Reads: 319

```
Looks nice! Let me know when you are ready for 90mm wheels. We will have some in a few weeks. http://www.ollinboardcompany.com/product/ollin-popoca-longboard-wheels-90mm-78a

Should be a perfect fit for that wheel pulley.
```

---
## \#99 Posted by: ndwallick Posted at: 2017-10-06T23:03:55.173Z Reads: 316

```
I will need some wheels soon, those look nice, I could use some softer wheels! Mine are 83A 

I rode with the new motor in 96 degrees F a little bit ago and I could still touch it without burning my hand.

Looks like my top speed is up from 20mph to 22mph!
(My theoretical top speed for both 200kv motors is 27.5mph)
(I'm guessing the biggest cause if it being lower is the vesc efficiency and the LiFe voltage sag)

I also noticed that I have full braking all the way until a full stop. :grinning: With the old motor, once I got going really slow the brakes would not brake with as much force and I would have to put my foot down. Now I can hold the brake down and come to a complete stop without my feet.
```

---
## \#100 Posted by: ndwallick Posted at: 2017-10-23T05:49:31.967Z Reads: 291

```
My old mount is for sale! I know it's hard to find mounts for the spacing on OM5065s. http://www.electric-skateboard.builders/t/for-sale-used-custom-adjustable-motor-mount-for-om5065/34993
```

---
## \#101 Posted by: Trans-amers Posted at: 2017-11-06T09:23:35.529Z Reads: 274

```
Did you use an oven or heat gun/hair dryer to heat up kydex?
```

---
## \#102 Posted by: ndwallick Posted at: 2017-11-08T18:26:52.326Z Reads: 279

```
An oven, if you scroll way up in this thread, I wrote about it, and I put a link to the turorial I watched
```

---
## \#103 Posted by: ndwallick Posted at: 2017-12-08T02:21:17.319Z Reads: 270

```
Starting an Instagram for pics of my board and other things I invent/build!
Go check it out!

https://www.instagram.com/nickwallick/
```

---
## \#104 Posted by: VAEsk8 Posted at: 2018-01-06T03:08:22.478Z Reads: 239

```
Hi man! Awesome build! 
What deck are you using? A link would be appreciated :)
```

---
## \#105 Posted by: VAEsk8 Posted at: 2018-01-06T03:10:30.361Z Reads: 236

```
Whats the name of that deck? Is it flexy? Link please :)
```

---
## \#106 Posted by: faithfulpuppy Posted at: 2018-01-06T05:36:40.290Z Reads: 235

```
i believe its an arbor axis. I don't know what length though 
http://arborcollective.com/skateboards/products/
```

---
## \#107 Posted by: Jebe Posted at: 2018-01-06T06:33:30.564Z Reads: 228

```
Yep. Arbor axis 40. Is a bit flexi.
```

---
## \#108 Posted by: ndwallick Posted at: 2018-02-02T22:49:30.832Z Reads: 225

```
@VAEsk8 hey! sorry I haven't been on here in a while, yup it's an Arbor Axis, I got it here: https://www.amazon.com/dp/B014R179O2/ref=cm_sw_su_dp
but it looks like they are sold out at that link right now, and it is slightly flexy, not nearly as flexy as a boosted board deck though.
```

---
## \#109 Posted by: ndwallick Posted at: 2018-07-20T19:26:21.384Z Reads: 200

```
Here is a quick update on my board since I haven't posted on here in a while.
My motor broke so I got this new [motor](https://psychotiller.com/product/sensored-6365-200kv-motor).
![IMG_1230|666x500](upload://A4gFLLYfyyksnMdsexGE6hyEyQ2.jpg)
I didn't want my black controller to look like a gun anymore so I painted it red with Plasti Dip. It also matches the motor quite well.
![IMG_1234|375x500](upload://xWdiLAizogGcqLY0lncclOBJxzj.jpg)
After I did these upgrades this happened:
![IMG_0929|375x500](upload://iCywoaUPSHbx7rLnZqBAi2mbdHM.jpg)
I was riding on a dark sidewalk and hit a huge crack. The board just snapped and I went right into the ground.

Here is my temporary fix for the deck which got me to class for the last 2 weeks of my semester:
![IMG_0933|375x500](upload://fsvdfs90ADc4xUAox0Jc8JazINw.jpg)

I bought a new deck and I just need to drill all those mounting holes again :sweat_smile: I will post pics here once the new deck is on. It's the same style deck but with a different pattern on the bottom and better grip tape.
```

---
## \#110 Posted by: ndwallick Posted at: 2018-07-27T03:49:28.245Z Reads: 192

```
Here is my new deck and some pics fo the board with it installed!
![IMG_1235|666x500](upload://4HCR1pSz67dfQju9ILQChw8WbAm.jpg)
![IMG_1240|666x500](upload://tm4QFydKA3d2xNAIi20cjnrBltg.jpg)
![IMG_1239|666x500](upload://31X8A6nS5Y2necS3Xrbq1Xa9X9X.jpg)
```

---
## \#112 Posted by: TiMMaTTie Posted at: 2018-08-11T20:12:55.418Z Reads: 175

```
you're not using the drop-through for your trucks, wouldn't you prefer a deck without those huge holes and have a bit more strength?
```

---
## \#113 Posted by: Skunk Posted at: 2018-08-11T21:09:38.471Z Reads: 171

```
How's your motor holding up riding ing in wet weather?
Did you take your motor apart and coat anything or change the bearings?
```

---
## \#114 Posted by: ndwallick Posted at: 2018-10-31T20:08:12.419Z Reads: 148

```
@TiMMaTTie You're right, a deck without the holes would add a lot of strength, but my current enclosures only fit the exact shape of that deck. I will probably go with a different deck for my next build.

@Skunk I haven't done anything to the motor and it has been holding up great! I don't ride it in the rain very often though. It doesn't rain much in AZ, but I did ride a few miles through the pouring rain a month ago and it worked well.
```

---
## \#115 Posted by: lrdesigns Posted at: 2018-11-02T07:41:29.381Z Reads: 143

```
Nice work on the Mcgiver fix!!

You should consider a reinforcing plate that goes and inch or two towards the center of the deck so you don't snap this one in the same spot.
```

---
## \#116 Posted by: ndwallick Posted at: 2018-11-08T03:41:27.939Z Reads: 137

```
@TiMMaTTie and @lrdesigns you guys called it lol. This just happened a couple days ago. It was the back part this time. I think I am going to get another of the same deck so that I don't have to remake my enclosures then reinforce it with steel this time.
![IMG_1662|375x500](upload://kUtVVkHRv8tb4e5ORGl4DAziBzn.jpeg) 

Also the MayTech motor got rammed into the sidewalk and slid for a good few seconds till I stopped. It still works great. None of the electronics got damaged.
```

---
## \#117 Posted by: lrdesigns Posted at: 2018-11-08T03:46:47.906Z Reads: 136

```
I can see the future man, the FUTURE! bhahaha. 

3rd deck is the charm they say. :stuck_out_tongue_closed_eyes:

If you can tie the plate into the bolts you already have for the enclosure that could be a good method without having to drill any extra holes. 

![image|690x339](upload://l2afiznWZWg0TaOxGGoQ9ExlCEv.jpeg)

I had a drop through that started to crack in the same spot, I did this. 
![image|541x500](upload://odqCDDopoJyE6SHOqr4zSWrisRb.jpeg)
```

---
## \#118 Posted by: ndwallick Posted at: 2018-11-08T05:59:09.150Z Reads: 128

```
@lrdesigns I like the drawing! I will definitely try to do something like that. What material is your plate and where did you get it?
```

---
## \#119 Posted by: lrdesigns Posted at: 2018-11-08T06:07:18.539Z Reads: 129

```
Its just 2mm Aluminium plate. I just cut it by hand with hacksaw. I got it at metal shop, they may have offcuts this size if you ask.
```

---
## \#120 Posted by: arne200 Posted at: 2018-11-27T06:44:29.736Z Reads: 114

```
But will aluminium give enough strength? Presume steel is too heavy though.
```

---
## \#121 Posted by: ndwallick Posted at: 2019-01-12T06:02:45.191Z Reads: 79

```
I just put new deck on and here's what I came up with for reinforcements. They are 1/4 inch aluminum plates. I didn't reuse the enclosure bolt holes because my enclosure is starting to crack and that would put extra stress on it. Instead I just used one thick bolt on each plate. I think this deck is gonna hold up for a while now. @TiMMaTTie @lrdesigns 
![a573a682-7ef9-4988-90d2-9307fa49e248|472x354](upload://pQQMr5tB8MPcdfrJ0SapE0Yo1Cw.jpeg) 
![b1b97723-5501-43b6-97db-69eb1998e52e|666x500](upload://hpBiYRLlOUZK64LTbILIucXoPDP.jpeg) 
![b25196de-be08-4f92-aa84-317751490d66|666x500](upload://xlQ63cB4w7ddWMg8UGfAGfpy7He.jpeg)
```

---
## \#122 Posted by: lrdesigns Posted at: 2019-01-14T02:20:26.029Z Reads: 66

```
Nice work, I hope it has a long life now. :ok_hand: :grinning:
```

---
