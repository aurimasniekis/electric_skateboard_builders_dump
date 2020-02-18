# First Build- An Attempt at Performance on a Budget

### Replies: 48 Views: 5518

## \#1 Posted by: Penny_Pincher Posted at: 2017-06-03T05:51:27.156Z Reads: 477

```
Ok so I've been doing a fair bit of research for the past week or so but I'm a newbie and could use some input. The goal is to have a board that I can use to commute to and from home to the gym/train station/work. I'd like it to be able to go up some pretty decent hills (I weigh 180lbs) and preferably go at least 20mph. Here's the parts list that I've come up with. Please give me any suggestions that you have. Much appreciated. 

Motor: 5065 1820W 270KV Brushless Motor, sensorless (X2)
ESC: Maytech Dual ESC 
Battery: four 5S 18.5V 6000mAh 50C Li-po wired into a 10s2p battery pack
Motor mount: Ebay motor mount (see link)
Trucks: 180mm paris trucks
wheels: 90mm flywheels

_Links:_ 
**Motor mount:** http://www.ebay.com/itm/Electric-Longboard-Skateboard-Motor-Mount-for-5065-5055-6374-6364-Motor-New-/252797338872?hash=item3adbe544f8:g:8C8AAOSwuxFYyPia

**Motor:**http://www.ebay.com/itm/N5065-5065-270KV-Brushless-Motor-For-DIY-Electric-Skateboard-Scooter-Multicopter-/401293060506?hash=item5d6eee299a:g:cCkAAOSw4A5YzNaf

**ESC:**https://www.aliexpress.com/item/Maytech-Free-Shipping-electric-longboard-dual-motor-speed-controller-dual-hub-motor-skateboard-ESC/32810420455.html?spm=2114.01010208.3.22.0Q9cuJ&ws_ab_test=searchweb0_0,searchweb201602_2_10152_5010012_10065_10151_10130_10068_10136_10137_10060_10138_10155_10062_437_10154_10056_10055_10054_10059_303_100031_10099_10103_10102_10096_10052_10053_10107_10050_10142_10051_10084_10083_10080_10082_10081_10178_10110_519_10111_10112_10113_10114_10182_10185_10078_10079_10073_10123_10189_142,searchweb201603_13,ppcSwitch_5&btsid=52a83181-c58b-4086-aed3-c99bc4f4df02&algo_expid=0f4f7224-a833-4771-bb53-2fe785fb6473-3&algo_pvid=0f4f7224-a833-4771-bb53-2fe785fb6473

**Battery:**https://www.aliexpress.com/store/product/New-18-5V-6000mAh-50C-Max-55C-5S-5Cells-18-5Volt-RC-LiPo-Li-Poly-Battery/909108_725738546.html?spm=2114.12010612.0.0.7vLmVa

**Trucks:** http://www.ebay.com/itm/Blank-Pro-180mm-Reverse-Kingpin-Longboard-Trucks-10-Axle-Black/140892408040?_trksid=p2045573.c100033.m2042&_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D41451%26meid%3Def21fef8e74b44698d8749404a9bfa72%26pid%3D100033%26rk%3D2%26rkt%3D8%26mehot%3Dpp%26sd%3D322382503804
```

---
## \#2 Posted by: saul Posted at: 2017-06-03T06:09:29.673Z Reads: 436

```
your name really says it all....

 I don't think it makes sense to build a dual on a budget. A single drive with vesc and 63mm motor will outperform it anyways. 20mph is easy!

and there are more than a few issues with these parts. I've never used any of them but to start the mounts need turned trucks like these
http://www.ebay.com/itm/Paris-7-trucks-for-electric-longboard-skateboard-and-trucks-turning-service-/322382503804?var=&hash=item4b0f7e9f7c:m:mjDWqt3IHG7rizUboRW-qng

next up, you can not fit 2x 5065 on a single truck so you'd have to run diagonal.
 pretty sure that esc wants sensored motors!! even still 270kv on 10s is not a good match.

you're also missing wheel/motor pulleys, belts,...and a remote.
```

---
## \#3 Posted by: Jinra Posted at: 2017-06-03T06:09:57.100Z Reads: 397

```
You'll likely be unable to fit both motors on a single truck so you'll have to do dual diagonal. Any ideas on what pulleys you're going to use?
```

---
## \#4 Posted by: Rinzler Posted at: 2017-06-03T10:33:12.374Z Reads: 388

```
If you want to penny pinch, here is a cheaper motor :wink: https://de.aliexpress.com/item/New-Arrival-Brushless-Outrunner-Motor-N5065-270KV-1665W-For-DIY-Electric-Skate-Board/32793728617.html?spm=2114.010208.3.44.xuSbRx&ws_ab_test=searchweb0_0,searchweb201602_2_10152_10065_10151_10068_5010013_10136_10137_10060_10138_10155_10062_437_10154_10056_10055_10054_10059_303_100031_10099_10103_10102_10096_10052_10053_10142_10107_10050_10051_5030013_10084_10083_10080_10082_10081_10110_519_10111_10112_10113_10114_10179_10182_10185_10078_10079_10073_10123_10189_142,searchweb201603_9,ppcSwitch_5&btsid=c06cc9c4-740e-49eb-8fb3-acebac881f8c&algo_expid=f0a61d97-1986-41f1-b4e7-e49b248336b4-6&algo_pvid=f0a61d97-1986-41f1-b4e7-e49b248336b4
```

---
## \#5 Posted by: Penny_Pincher Posted at: 2017-06-03T14:45:09.688Z Reads: 363

```
@saul @Jinra I'll link the remote, gears, and pulleys that I plan to use. The motor gear has 20T and the wheel gear has 60. Also, if I wanted to fit two motors, what type do I need? and if you really think a single motor build is better.... what components do you suggest?

Gears/Belt: https://www.aliexpress.com/item/Maytech-electric-skateboards-pulley-and-belt-system-with-1pcs-NSK-f608zz-bearing/32770135067.html?spm=2114.01010208.0.0.uBffm7

Remote: http://www.ebay.com/itm/2-4GHz-Radio-Remote-Controller-Receiver-Binding-Plug-For-Electric-Skateboard/262779892776?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D41451%26meid%3Da6ae4bac9dee45189a43b12c995e976b%26pid%3D100005%26rk%3D3%26rkt%3D6%26mehot%3Dpp%26sd%3D232284516689
```

---
## \#6 Posted by: aigenic Posted at: 2017-06-03T15:25:41.374Z Reads: 331

```
Just dont do it like this...you will end up buying better and reliable parts...I tried something similar with my first build, and all the parts I tried to make cheaply are today gone, I replaced them with more reliable ones...

At least spend more money on the mechanical part...so caliber trucks, motor mount from a member of this forum (from 22$, just search), 3d printed wheel pulley (12$ also from forum), motor pulley + belt from ebay and it will not be pain in the ass...

The electronics...if you want cehap setup, you can go 6s on 240 - 270kv motor with Car ESC, it is cheap and good solution...But I higly recommend VESC
```

---
## \#7 Posted by: Rinzler Posted at: 2017-06-03T15:28:02.082Z Reads: 313

```
They are saying a single motor build is better because you dont need a dual drive for your performance demands, if you go dual with cheap components things will break and the quality of the components will be quite low. But if you build a single drive you are using less components for the same price so they can be better, better quality.
```

---
## \#8 Posted by: aigenic Posted at: 2017-06-03T15:29:38.734Z Reads: 303

```
@Rinzler Absolutely true
```

---
## \#9 Posted by: Penny_Pincher Posted at: 2017-06-03T16:20:04.050Z Reads: 313

```
Ok so in that case- What do you suggest my build should look like in terms of components? I had also considered buying maytech or lofty ambition hub motors to eliminate the complexity of belts and gears... I was thinking that going with hub motors may allow for a more low maintenance setup, and I would of course need VESCs for that setup since the hub motors would be sensored. The only reason I was turned off by that route was over concern that the hub motors may not be able to take abuse from rough pavement. Any thoughts? I'll link the hub motors i'm talking about below. I would be hooking these up to the same battery setup, which in theory should give me a fair bit of power. Thoughts? 

https://www.alibaba.com/product-detail/Maytech-wireless-receiver-remote-and-90mm_60596635246.html?spm=a2700.7724838.0.0.XvXIX7
```

---
## \#10 Posted by: Rinzler Posted at: 2017-06-03T17:14:07.092Z Reads: 298

```
Nobody tested those hub motors, trust me if your on a budget you dont want to be the first. Most of the builds in the community are the mostly the same, because we know what works and what doesnt :wink:
I advise you to use the search function of the forum and search for builds that have the same things you are sure about etc.you are going to use a 10s lipo pack.

Here is it, have a read, find a board that performs good, maybe ask a few questions to the builder of the board and just copy, copy, copy because you are quite new here and on a budget and experimentation leads to trial and error which costs :cry:
https://www.electric-skateboard.builders/search?expanded=true&q=10s%20lipo%20%20%23e-board-builds
```

---
## \#11 Posted by: Penny_Pincher Posted at: 2017-06-03T21:07:27.144Z Reads: 292

```
Which motor is better for a single motor build? 

Option 1: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html?___store=en_us

Option 2: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html?___store=en_us

Option 3: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html?___store=en_us


I've started to sort out my other components. I was looking into the Alien power systems motor (i'll link it below) but I couldn't find gears that would fit the 10mm shaft.

Alien Power motor: http://alienpowersystem.com/shop/brushless-motors/alien-6374-sensored-outrunner-brushless-motor-170kv-3200w/
```

---
## \#12 Posted by: smurf Posted at: 2017-06-03T21:40:14.600Z Reads: 275

```
Option 5:
http://www.ollinboardcompany.com/product/om-6085-200kv
```

---
## \#13 Posted by: saul Posted at: 2017-06-03T22:04:12.191Z Reads: 266

```
i've been really tempted to get one of these, good price. 190kv is perfect for 10s.
https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html
```

---
## \#14 Posted by: Penny_Pincher Posted at: 2017-06-03T23:02:13.960Z Reads: 260

```
@saul @smurf have either of you built with the motors you suggested? and it looks like I can get pulleys for the Alien power systems motor which is rated for 3200W and 170Kv which I think would give me plenty of torque and speed. Would a 190Kv, 2000W motor get me up hills and going fast?
```

---
## \#15 Posted by: Penny_Pincher Posted at: 2017-06-03T23:35:42.531Z Reads: 263

```
OK here's what I've come up with in consideration with the suggestions you all have given me. Let me know if this seems like a compatible build. If I've understood everything I've been reading, these parts should be compatible and give me a board that should go up hills and relatively fast. What do you all think? let me know. thanks. 

Motor: Turnigy Aerodrive SK3 - 6364-190kv Brushless Outrunner Motor
Battery: four 5S 18.5V 6000mAh 50C Li-po wired into a 10s2p battery pack
ESC: Maytech VESC
Remote: 2.4 ghz controller & receiver
Gears/ Belts: 15T on Motor, 36T on Wheel 15mm belt (From Ebay)
Wheels: 90MM flywheels
Trucks: Getting a pair from Ebay to fit the motor mounts which are also from Ebay. See links below. 

_Links To Everything_ 
**Motor Mount:**http://www.ebay.com/itm/Electric-Longboard-Skateboard-Motor-Mount-for-5065-5055-6374-6364-Motor-New-/122382295648?hash=item1c7e8da260:g:eA0AAOSwCU1YulzI

**Trucks:**http://www.ebay.com/itm/Paris-7-trucks-for-electric-longboard-skateboard-and-trucks-turning-service-/322382503804?var=&amp;hash=item4b0f7e9f7c:m:mjDWqt3IHG7rizUboRW-qng

**Gears and Belt:**http://www.ebay.com/itm/DIY-Electric-Skateboard-ABEC-Flywheel-Pulley-Kit-15mm-Wide-Belts/272671900207?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D41451%26meid%3D16907880bd2b4d059ae210ee1b53795a%26pid%3D100005%26rk%3D4%26rkt%3D6%26sd%3D272671887289

**Remote:**http://www.ebay.com/itm/2-4GHz-Radio-Remote-Controller-Receiver-Binding-Plug-For-Electric-Skateboard/262779892776?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D41451%26meid%3Da6ae4bac9dee45189a43b12c995e976b%26pid%3D100005%26rk%3D3%26rkt%3D6%26mehot%3Dpp%26sd%3D232284516689

**Motor:**https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html?___store=en_us

**ESC:**https://www.aliexpress.com/item/Maytech-ESC-RC-VESC-for-outboard-motor-remote-control/32735966588.html?spm=2114.01010208.3.8.vSz4N8&ws_ab_test=searchweb0_0,searchweb201602_2_10152_5010012_10065_10151_10130_10068_10136_10137_10060_10138_10155_10062_437_10154_10056_10055_10054_10059_303_100031_10099_10103_10102_10096_10052_10053_10107_10050_10142_10051_5030013_10084_10083_10080_10082_10081_10178_10110_519_10111_10112_10113_10114_10182_10185_10078_10079_10073_10123_10189_142,searchweb201603_16,ppcSwitch_5&btsid=1f92bb8d-3fdd-4330-ab5d-a8869fe8b31d&algo_expid=da4569bd-0fe5-46b1-a2a4-09a9a1e2afed-1&algo_pvid=da4569bd-0fe5-46b1-a2a4-09a9a1e2afed


**Wheels:**http://www.ebay.com/itm/90mm-80a-Gel-Soft-Longboard-Wheels-Neon-Green-/182602253222?hash=item2a83f143a6:g:GfUAAOSwKOJYG73k
```

---
## \#16 Posted by: aigenic Posted at: 2017-06-04T07:55:29.391Z Reads: 224

```
If you bay Maytech VESC you will probably have to upload the frimware...
```

---
## \#17 Posted by: TehAtheist Posted at: 2017-06-04T08:56:33.366Z Reads: 231

```
How do you mean exactly? Is that a difficult process that involves a sepperate PCB or is that just plug and play with a usb cable and clicking a button?
```

---
## \#18 Posted by: WSB Posted at: 2017-06-04T09:20:35.347Z Reads: 225

```
No, it works fine without the need to upload any firmware.
```

---
## \#19 Posted by: aigenic Posted at: 2017-06-04T09:59:14.232Z Reads: 223

```
Anyway, it will be better if you ask the vendor if the firmware is uploaded...
```

---
## \#20 Posted by: Penny_Pincher Posted at: 2017-06-04T12:49:07.941Z Reads: 214

```
I have programmed ESC and receivers before, so using the BLDC tool and updating the ESC is something I should be able to do fairly easily if I have to. Other than that- does everything look good? I am thinking of ordering everything today.
```

---
## \#21 Posted by: aigenic Posted at: 2017-06-04T13:00:46.668Z Reads: 195

```
I think it is OK, the only thing I am not szre about is the center distance of the motor mount...I think it will be OK, in the worst scenario you will have to buy shorter or longer belts...
```

---
## \#22 Posted by: aigenic Posted at: 2017-06-04T13:02:47.606Z Reads: 202

```
And also the batteries wouldgive you about 40kms of range, the  10S1P might be enough for you, it depends on your personal attitude
```

---
## \#23 Posted by: Penny_Pincher Posted at: 2017-06-05T23:45:37.127Z Reads: 199

```
I've decided to switch two things: I will be going with a 170kv 6374 maytech motor because it has a sensor, and mainly because it it sealed, which I hope will help with keeping it protected from water/sand/etc, and I will only be going with 10s1p (2 5s batteries wired together) since I want to keep things simple and I should still get about 10 miles of range out of those batteries. I will probably be ordering all my components tonight. Now I have to wait almost 3 weeks until everything arrives...
```

---
## \#24 Posted by: vadimkovalev99 Posted at: 2017-06-14T06:13:08.963Z Reads: 195

```
you should upload pics and update on how good it works....
```

---
## \#25 Posted by: Penny_Pincher Posted at: 2017-06-14T17:48:31.404Z Reads: 207

```
Currently waiting for the last few parts to come in! I will upload pictures once I start building the board.
```

---
## \#26 Posted by: Penny_Pincher Posted at: 2017-07-01T23:50:36.600Z Reads: 223

```
OK! The last of the parts arrived on Friday, and I spent Friday evening putting the final build together. I had put together an "intermediary" build that was pretty sketchy but now everything is pretty much final as of now. If you have any questions about the parts or anything, I'll try my best to answer them.

**Performance:** While I have not been able to measure the percent grade of the hills I have climbed, I can say that it easily goes up hill that are difficult to climb on a bike. I was able to final feel comfortable going to full throttle today and I peaked at 25mph, although that was on a very slight downhill. Going back up that slight downhill, I reached a max speed of just over 23mph, which is faster than I ever really need to be able to go. As far as range goes, based on calculations it should be just under 10 miles, but I have not tested this yet.

**Notes:** The most difficult parts of building the board were mounting the gear to the wheel so that it was properly centered (it's still not perfect, but good enough) and also getting the belt not to rub up against the wheel since the gear on the wheel was seated a little too far into the wheel. I solved this by melting down the side of the wheel with  a soldering iron a little bit and adding two extra speed rings on the axel between the truck and the wheel. This causes the belt to have a little bit of overhang on the gear, which may affect the lifetime of the belt. I don't think it will, but we'll see. The total distance I do every day is around 4-5 miles, and it varies from open road- good and bad pavement- to sidewalks. This thing has 90mm wheels which I specifically chose so that it could handle cracks in the pavement and going on sidewalks. Despite the size of the wheels, riding on sidewalks for too long is a pretty rough ride, uncomfortable, and feels like I'm abusing the board. So far it has handled everything well, although I had to apply a liberal amount of loctite threadlocker to every single screw and bolt on this thing to keep it from self-disassembling. Overall, I spent a lot of time planning this out ahead of time and the whole project seems to have gone fairly smoothly. I should mention that while this thing is very fun, it is also quite dangerous, and that everyone who decides to build one of these should test their boards incrementally and regularly check on every component for any signs of failure. Also you should wear a helmet at all times.

**Pictures:** Here's what the final build looks like. I have the stickers on there for one reason: I take this on the train, and people these days get scared when they see bulky boxes strapped to objects with wires coming out. These stickers are an attempt at making the board look more friendly, and it has worked very well- I get a lot less stressful looks from strangers now. This is not something I had initially considered when making the board, but it should definitely be a part of the planning process unless you want to find yourself on a watch list somewhere. Thanks to everyone who helped!

<img src="/uploads/db1493/original/3X/1/3/1324edd184ffca0d6c88923f1b93207503205f2a.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/4/3/43a38cd618b46425c8a526823034cc4525cb7702.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/6/5/651c02bc12025d322ada78c480505145998e398f.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/4/8/48b422464ef6f05269b88588b4655a611d5c53d4.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/2/8/28d0552b1d132a194c5620a3348a77713075887d.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/9/f/9f456faabad83706ce60b9b0eec6e59ffa160e0f.jpeg" width="666" height="500">
```

---
## \#27 Posted by: solarcross Posted at: 2017-07-29T17:32:15.306Z Reads: 191

```
So.....How are the sealed motor .....any-issues..
-is it really water-tight....
thankyou
```

---
## \#28 Posted by: Penny_Pincher Posted at: 2017-09-05T01:36:17.481Z Reads: 180

```
Sorry for the late reply- so far no issues with the motor. I’ve gone through small puddles and it has gotten wet but it still works perfectly. I did damage it slightly at first since I had the belt tension way too tight which caused the shaft of the motor to be pulled in towards the wheel at all times. Because of this I had to replace a C-clip on the motor shaft but otherwise the motor is still going strong. Would reccommend.
```

---
## \#29 Posted by: Penny_Pincher Posted at: 2017-09-15T19:14:02.118Z Reads: 176

```
UPDATE: The motor motor mount, which is held onto the truck using three screws with point to dig into the aluminium, don't seem to be a great solution. I have ridden this setup for about four months straight almost daily, but now the motor mount is coming loose and is rotating around the truck. I don't have the time right now but I am planning on drilling three holes into truck at the position of the screws, and I will get longer screws so that they go down into the holes in the truck. This should be a permanent and solid solution, although drilling the holes at the correct locations and angles will likely prove to be difficult. I will keep this thread updated if there is interest.
```

---
## \#30 Posted by: pat.speed Posted at: 2017-09-16T05:58:11.199Z Reads: 162

```
Yeah same thing happened and I stuffed up the hole alignment by a few mm so now the belt rubs on the wheel a bit
```

---
## \#31 Posted by: BenL Posted at: 2017-09-17T03:25:04.760Z Reads: 155

```
Did you end up using that ebay transmitter/receiver that you linked? What is it's behavior when it loses signal or loses power (can test by flipping the board upside-down and removing the battery or walking to another room)? How do you like it? 

I'm looking for an alternative to the Nyko Kama which doesn't have a fail-safe if it loses power- it just keeps doing exactly what it was doing when it had connection. Thanks!
```

---
## \#32 Posted by: Clonkex Posted at: 2017-09-18T05:32:11.459Z Reads: 143

```
I'm certainly interested. Keep us updated! :)
```

---
## \#33 Posted by: Penny_Pincher Posted at: 2017-09-19T18:48:41.804Z Reads: 145

```
No, I did not end up using the linked remote. I decided to change to one that was smaller and would fit in my pocket easily. The one I am using I will link below. It is good and has never lost connection with the board while i’m riding it although in the city (probably due to interference) if I do not touch the throttle on the remote at all for about 30 seconds, the motor begins to ‘twitch’ a little bit but nothing more. Also, if the board is plugged in and the transmitter is turned off, instead of staying neutral or braking, the board goes full throttle which is a little scary. However, I have had no problems with the transmitter or receiver and I ddo think it is a better alternative to many of the options currently out there. 

https://www.aliexpress.com/item/Wholesale-New-arrival-2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32678995218.html?spm=2114.search0104.3.72.NgPleg&ws_ab_test=searchweb0_0,searchweb201602_4_10152_10065_10151_10130_10068_10344_10342_10343_10340_10341_5560011_5550020_10307_10137_10060_10155_10154_10056_10055_10054_5470020_10059_100031_10099_5460020_10338_10339_10103_10102_440_10052_10053_10107_10050_10142_10051_10324_10325_5380020_10326_10084_513_10083_10080_10082_10081_10178_10110_10111_10112_10113_10114_143_5570011_10312_10313_10314_10078_10079_10073,searchweb201603_6,ppcSwitch_5&btsid=1619b284-9803-4a64-90ef-d990f5406dbc&algo_expid=6bcfb6d9-9aa2-4b8a-9a23-2db24b32af2d-9&algo_pvid=6bcfb6d9-9aa2-4b8a-9a23-2db24b32af2d
```

---
## \#34 Posted by: Clonkex Posted at: 2017-09-19T23:01:23.469Z Reads: 126

```
You need to set the failsafe on your VESC so that if the controller disconnects you don't accelerate at full throttle. Read this thread: http://www.electric-skateboard.builders/t/board-got-stuck-on-full-throttle-with-no-brakes-what-could-cause-this-related-story-slid-my-e-skate-for-the-first-time/26314
```

---
## \#35 Posted by: Aurhoxx Posted at: 2017-09-23T09:10:44.513Z Reads: 119

```
Hello, i am building my first build.
here are the parts:
turningy aerodrive sk3 6374 149kv
3 zippy 5000mah 3s 45c batteries
xcar beast 120amp esc
2.4ghz remote
i have all the connectors and mounts/pullys
How fast should i go and how far will i go?
```

---
## \#36 Posted by: Aurhoxx Posted at: 2017-09-23T09:12:24.836Z Reads: 130

```
oh it is also in series
```

---
## \#37 Posted by: Deakbannok Posted at: 2017-09-23T10:02:40.383Z Reads: 146

```
i cried after read the first paragraph of the first post.
```

---
## \#38 Posted by: GrecoMan Posted at: 2017-09-23T10:27:11.992Z Reads: 149

```
You could pick up one of my mounts 😉
http://www.electric-skateboard.builders/t/new-circular-truck-motor-mount-survey-posted/33609/28
```

---
## \#39 Posted by: pat.speed Posted at: 2017-09-23T12:37:15.608Z Reads: 147

```
That will not work. An Xcar beast esc can only handle 6s not 9s
```

---
## \#40 Posted by: Aurhoxx Posted at: 2017-09-23T20:59:09.590Z Reads: 136

```
oh sorry i meant 2 of them lol
```

---
## \#41 Posted by: pat.speed Posted at: 2017-09-23T23:14:36.930Z Reads: 120

```
Ahhh ok looks fine. You will not go very fast at all probably around 20kmh. If you haven't bought the parts yet I would suggest the 245kv motor from HobbyKing as it will increase your speed to around 35km/h and it is also cheaper
```

---
## \#42 Posted by: Aurhoxx Posted at: 2017-09-25T01:03:39.224Z Reads: 93

```
ok i have changed plans
6347 192kv, 2 6s 5000mah lipo battery, Talon 120a 12s esc, 90mm wheels, 12t motor pulley/36t wheel pulley how fast and is the range on this board will be?
```

---
## \#43 Posted by: Clonkex Posted at: 2017-09-25T03:35:32.660Z Reads: 84

```
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":192,"system-efficiency":85,"motor-pulley-teeth":12,"wheel-pulley-teeth":36,"wheel-size":90}|
```

---
## \#44 Posted by: Aurhoxx Posted at: 2017-09-25T21:34:36.200Z Reads: 74

```
what is the range?
```

---
## \#45 Posted by: GrecoMan Posted at: 2017-09-25T21:51:42.631Z Reads: 74

```
Depends on your riding style and environment
```

---
## \#46 Posted by: Aurhoxx Posted at: 2017-09-25T22:09:38.873Z Reads: 73

```
just the normal flat ground with an average a bout like 15mph
```

---
## \#47 Posted by: Clonkex Posted at: 2017-09-25T22:38:45.982Z Reads: 73

```
Should be _very roughly_ 22km, using this super approximate calculation:

12S = 44.4v (using nominal cell voltages)
5000mAh = 5Ah
44.4 * 5 = 222KWh (kilowatt-hours)
222 / 10 = 22.2km

You could get a lot more, could get a lot less.
```

---
## \#48 Posted by: Aurhoxx Posted at: 2017-09-25T22:42:35.897Z Reads: 73

```
Thank you! ordering parts today😁
```

---
