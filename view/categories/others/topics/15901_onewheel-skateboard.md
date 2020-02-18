# Onewheel skateboard

### Replies: 136 Views: 13812

## \#1 Posted by: littlem39 Posted at: 2017-01-11T12:35:44.167Z Reads: 835

```
I recently stumbled upon Onewheel. Anyone tried to build something similar? https://m.youtube.com/watch?v=XNqOU4jx62I
```

---
## \#2 Posted by: okp Posted at: 2017-01-11T14:21:52.416Z Reads: 792

```
great one ! my reply is a bit off topic as I did not build anything like this yet; but I got the opportunity to try one of these last july and it's a great feeling. You feel a great impression of freedom as you are not using any remote to control. It's smooth, predictable and a lots of fun. Only drawback is the (heavy) weight and miles coverage that kills it. as usual... I did it my way !


https://youtu.be/tljYoVq6rHo
```

---
## \#3 Posted by: littlem39 Posted at: 2017-01-11T16:38:40.756Z Reads: 748

```
That's all i wanted to hear, thanks for your reply :)

I investigated a bit and realised that they use a go kart wheel. Those wheels+tyre+hub+separate bearings can get expensive. So I am considering using two 10'' pneumatic [wheels](https://www.amazon.co.uk/dp/B01CCRN3LQ?psc=1)  with pulley in the middle. I made a quick model in solidworks. <img src="/uploads/db1493/original/3X/c/1/c14db89ca478b0655602b9010ba9e1003b8d80c5.png" width="674" height="454">
```

---
## \#4 Posted by: goldenHusky Posted at: 2017-01-11T19:38:17.730Z Reads: 708

```
memories coming up when I see this haha :joy:
Also made one by myself some time ago.
I built it with an arduino mega + mpu6050 + vesc + 6374 motor with custom planetary gear mounted inside the gokart wheel, 10s4p Sony VTC3 batteries, intelligent led lighting (switched red back and white front light according to the actual driving direction,  including light sensor to determine the needed light), pressure sensitive pads, so the boards knows when you fell off and stops etc.
<img src="/uploads/db1493/original/3X/2/4/24a287ef92df63c24d4f5e9e83e52a89e1d64e73.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/c/4/c447a4e7dacd0de1d84daed3c2fc7f2376c550b7.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/2/4/24bff6b666e3b89038a5a4e971356ce186514754.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/b/7/b7104d25f31fa404828f05529477b6e13f8bc193.jpg" width="666" height="500">

In the end I disassembled the board and sold the components. I needed money for a new project :sob:
```

---
## \#5 Posted by: Hummie Posted at: 2017-01-11T19:40:34.662Z Reads: 667

```
fantastic.   too bad you sold it it looks better than the onewheel.  I see there's another business selling them too now...pretty much an exact copy from the looks but who knows whats inside
```

---
## \#6 Posted by: okp Posted at: 2017-01-11T19:44:06.427Z Reads: 652

```
@goldenHusky insane. do you have any build thread on this ?
```

---
## \#7 Posted by: goldenHusky Posted at: 2017-01-11T19:51:49.320Z Reads: 645

```
@Hummie  Thank you!
@unik Unfortunately not. I built that 3 years ago when I was 16 and didn't discover this forum back then yet.

If anybody wants to build such a thing, I recommend buying a complete tire+ hub motor unit  like this one: http://www.peipeiscooter.com/default/11inch-350w-500w-wide-tire-hub-motor-phub-44

Designing, manufacturing and mounting a custom planetary gear was painful :joy:
```

---
## \#8 Posted by: Hummie Posted at: 2017-01-11T19:55:41.749Z Reads: 619

```
why'd you do a planetary gear and not just direct drive?  seems overkill
```

---
## \#9 Posted by: littlem39 Posted at: 2017-01-11T19:59:02.528Z Reads: 607

```
Probably beacuse outrunners are high kv motors. And in order to have sufficient torque you need reduction (Planetary gear).
```

---
## \#10 Posted by: goldenHusky Posted at: 2017-01-11T20:00:33.949Z Reads: 587

```
ask that the young goldenhusky please :joy:
I was worried that I wouldn't get enough torque to maintain balance when driving very slow/ at startup.
The motor was a 90kv 6374 from alienpower.
```

---
## \#11 Posted by: OskarCastrone Posted at: 2017-01-11T20:14:29.988Z Reads: 577

```
I saw a video on youtube a couple of months ago. This version is actually not tilting forwards and backwards. Instead he is using a remote. Is is deffinetly not as awesome as the original but maybe easier?
Anyway [here](https://youtu.be/B53TV-3KDEM) is a link.
```

---
## \#12 Posted by: littlem39 Posted at: 2017-01-13T08:14:12.739Z Reads: 552

```
@goldenHusky 
can you share with us some more info on your build? i am interested in how you connected the wheel  to the shaft connected to the frame. Your build was really something ! ☺
```

---
## \#13 Posted by: goldenHusky Posted at: 2017-01-14T17:19:04.152Z Reads: 539

```
@littlem39 well I cut the axis into 2 parts, both axis parts were connected to the frame with screws. I used bearings inside the tire to allow it to spin.
So it's like [frame left]--[axis part 1]--[motor]--[gear]--[bearing]--[axis part 2]--[frame right]
```

---
## \#14 Posted by: littlem39 Posted at: 2017-01-15T09:55:29.772Z Reads: 538

```
What do you guys think? <img src="/uploads/db1493/original/3X/3/5/353b53380ef753e567e93b159e60b3bc9f9b49b5.JPG" width="690" height="467">
```

---
## \#15 Posted by: OskarCastrone Posted at: 2017-01-21T12:28:06.812Z Reads: 505

```
Looks pretty sweet! Have you thought about the balancing aspect of the build? :)
```

---
## \#16 Posted by: littlem39 Posted at: 2017-01-21T16:52:57.235Z Reads: 502

```
Sensor + PID regulation in arduino should be good for that, but i would need to test that to tell for sure.  There are many options and space for software development  on this project, unlike on eskate.
```

---
## \#17 Posted by: OskarCastrone Posted at: 2017-01-25T22:35:44.290Z Reads: 494

```
Seems complicated! But cool if you have the means / knowledge to do it! I would love to see more in the future! :D
```

---
## \#18 Posted by: CCU Posted at: 2018-04-04T19:30:48.747Z Reads: 454

```
Any progress on the idea? Because i was thinking about doing the same.
```

---
## \#19 Posted by: littlem39 Posted at: 2018-04-11T21:10:43.127Z Reads: 449

```
Unfortunately  i had no funds to go forward with the idea. Still a student, but i have a motor and a vesc that still wait for the better days :) But if you decide to go with the idea and try to make it, i would be happy to discuss it with you
```

---
## \#20 Posted by: sayekim Posted at: 2018-07-12T20:29:59.236Z Reads: 434

```
Has Onewheel simply nailed this?

It seems @goldenHusky is the only one that successfully tried it but disassembled it for money before he found out about the forum. 

I would love to see a standardized complete controller/brain for this for peoples to make their own version. 

Honestly though I do think Onewheel has nailed it and if I ever have the extra dough I’m definitely buying one.
```

---
## \#21 Posted by: Hollan Posted at: 2018-08-02T19:39:15.263Z Reads: 388

```
I'm curious, what pressure sensitive pads did you use?
```

---
## \#22 Posted by: goldenHusky Posted at: 2018-08-02T19:50:26.732Z Reads: 382

```
Velostat @Hollan
```

---
## \#23 Posted by: puuhapet Posted at: 2018-08-16T04:25:53.531Z Reads: 388

```
@goldenHusky
I'm also trying to build my own onewheel clone. Do you have the Arduino code that you used for your onewheel clone build? I'm a total noob when it comes to Arduino code so it would help a lot.
```

---
## \#24 Posted by: goldenHusky Posted at: 2018-08-16T05:13:36.516Z Reads: 383

```
@puuhapet
I'm afraid, I don't have it anymore.
Some other people built their own onewheel aswell and put their code on github, use that as a starting point. Good luck!
```

---
## \#25 Posted by: puuhapet Posted at: 2018-08-16T05:59:18.936Z Reads: 377

```
Ok, thank's anyway. I did a quick search in Github and found one partial code but nothing complete. Have to search more.
```

---
## \#26 Posted by: lock Posted at: 2018-08-17T00:20:45.603Z Reads: 400

```
Just got a call from a local Kart store.... "Just checking you're only after the one tire?". To be fair he already knew about the Onewheel, wished me luck on my new project :joy:

There's not much to it right now; I have a VESC (ESCape), esp32 dev board and 6DOF sensor sitting in a cupboard. Tire + rim are on its way.

Spent a bit of time doing some research; two repos of interest...
https://github.com/schglmnn/VESC-OneWheel

https://github.com/blezalex/WheelBoardMain

It'd be nice to have a VESC with the motion sensor chip for this, and I just read the Unity will come with one. Obviously I don't need a dual motor ESC :tired_face:.

Always assumed Onewheel actually invented the single go kart wheel self balancing skateboard concept, but it turns out [credit should go to Ben Smither back in 2007](http://www.robosys.co.uk/).
https://youtu.be/HGbbag9dklU
```

---
## \#27 Posted by: iKNOWaFATman Posted at: 2018-08-17T01:52:07.879Z Reads: 372

```
Thats nuts if he came up with it and one wheel stole it and ran. Uness he is involved with them....
```

---
## \#28 Posted by: littlem39 Posted at: 2018-08-17T06:43:14.218Z Reads: 364

```
[quote="lock, post:26, topic:15901"]
[/quote]

Have you decided about the motor?
```

---
## \#29 Posted by: lock Posted at: 2018-08-17T07:10:23.108Z Reads: 368

```
Good question.

Will be belt driven. Fairly certain the Onewheel's motor is about 700w, and it probably weighs several kg. Hub options are rather limited, and I'd like to use something lighter and more powerful. Not thinking anything extreme, ideally something around a 6374 size.

With a 11in (280mm) outside diameter the motor will need to be pretty low KV; say 50-70. And even at that low KV it'll still need high'ish (eg; 3:1) gearing. Aiming for a top theoretical speed of 40km/h as it's faster than I'd ever expect to travel... reaching top speed on a self balancing board is not something you want to do.

So basically _sensored_ 6374, 50-70kv, probably from APS as it seems to be the only source. The APS 80mm motors are tempting as some of them have extended axles both sides which would allow a bit more flexibility in pulley mounting.
```

---
## \#30 Posted by: mikenyc Posted at: 2018-08-17T09:39:08.866Z Reads: 352

```
Why not a hub motor?

https://m.aliexpress.com/item/32678163160.html
```

---
## \#31 Posted by: lock Posted at: 2018-08-17T10:07:48.268Z Reads: 356

```
There's certainly some hub options. The one you linked is a little odd sized in terms of go kart wheels. You really need to find something with either a 5 or 6in rim diameter, and a width between 5 and 7in otherwise tires are going to be hard to find. Here's a few options:
[10 inch 10x6.00-5.5 wide tubeless tyre brushless gearless dc wheel hub motor ](http://www.peipeiscooter.com/10inch-10-inch-10x6-00-5-5-wide-tyre-brushless-gearless-dc-wheel-hub-motor-balance-scooter-hub-motor-hally-motor-phub-188)
[11 inch 350w-500w wide tire brushless hub motor](http://www.peipeiscooter.com/11inch-350w-500w-wide-tire-hub-motor-phub-44)

Hub would certainly make the build easier, but I think you'd get better performance and a lighter weight out of a smaller outrunner. As an added advantage you get more accurate motor position sensing due to the reduction (motor turns many times for one wheel revolution), but then a potential disadvantage is that the belt drive introduces backlash/slop a direct drive wouldn't.
```

---
## \#32 Posted by: mikenyc Posted at: 2018-08-17T11:22:22.167Z Reads: 336

```
Hubs are probably safer than belts as well (belt snapping will not be fun at any speed). 

And thanks for finding the correct link. I saw those before, couldn't find them when I searched again.
```

---
## \#33 Posted by: puuhapet Posted at: 2018-08-17T11:57:33.483Z Reads: 328

```
I have one of those 10" hub motors that you linked. I'm also planning to build a clone onewheel. I have one spare VESC 4.12 that I'm planning to use. Good find on the blezalex Github page. I have few old quadcopter flight controllers laying around. Have to check if I can use those in this build. What are your plans to build the frame? I was thinking using U-shaped aluminium for the side rails and maybe 3D-printed parts for the boxes.
```

---
## \#34 Posted by: lock Posted at: 2018-08-17T13:56:23.340Z Reads: 334

```
[quote="puuhapet, post:33, topic:15901"]
I have one of those 10" hub motors that you linked.
[/quote]

Nice. That one certainly looks like its been made with a Onewheel clone in mind. Is the hub diameter really 6in? The labelling on the pictured tire seems to be a bit off. Normally a tire with a 10x6-5.5 would indicate a 10in outside diameter, a width of 6in, and a hub diameter of 5.5in. I'm of the opinion the width and hub diam have been mixed up.

[quote="puuhapet, post:33, topic:15901"]
What are your plans to build the frame? I was thinking using U-shaped aluminium for the side rails and maybe 3D-printed parts for the boxes.
[/quote]
Not sure just yet, need to think about how much I want to invest into something that may not work. Cheap solution would be U-section or box section aluminium tubing. Some carbon tubing might be nice with some CNC'd attachments to mount the axle, etc. 

There's another option that almost starts to sound like cheating. Go with some [aftermarket Onewheel rails](http://calibratedpower.com/beast-wheel/beast-wheel-rail-set-696mm.html), and maybe even get the OE foot+sensor pads and bumpers from Onewheel direct. Nice thing about this is your DIY would be compatible with a lot of the Onewheel accessories out there.
```

---
## \#35 Posted by: puuhapet Posted at: 2018-08-20T11:28:42.976Z Reads: 339

```
I took some measurements from the wheel. I could only measure the outside edge of the rim. I don't know does this tell anything. Total width measurement is few mm bigger than the caliber max because I had to force the caliber around the tire.

![IMG_20180817_173042|690x388](upload://7LyNYW4ac6NuyaEO8T37E7kfplI.jpg)![IMG_20180817_173156|690x388](upload://nDXamFTziejh7CI7TNCZAdA9WrZ.jpg)![IMG_20180817_173214|690x388](upload://b84vq9Nj6UF5P7UmNFJYU3FH8Cb.jpg)

- Hub diameter 150 mm
- Tyre thread width 132 mm
- Tyre total width 156 mm

Thanks for the suggestions. I haven't finalized my design for the frame yet. First I want get the VESC and balance controller to work together.
```

---
## \#36 Posted by: lock Posted at: 2018-08-21T00:38:35.603Z Reads: 325

```
Thanks @puuhapet

Here's the 5in kart wheel spec ([source](http://www.karting.net.au/media/technical/2016/2016%20DUNLOP%20TYRE%20SPECIFICATIONS.pdf)), haven't been able to find similar for 6in wheels.
![55%20am|690x451](upload://ePlxAB7Y7VjHs0SsCGo3MtUo13l.png)

The corresponding hub diameter dimension you've measured at 150mm is 136.2mm for the 5in wheel, so obviously not a match. If we assume the 6in standard kart wheel adds an inch to this we get 161.6mm (136.2+25.4) which doesn't match up with 150mm either. I guess the labelling on the tire is correct, and that it is actually a 5.5in tire. My only concern with this is that it may limit tire choice.
```

---
## \#37 Posted by: puuhapet Posted at: 2018-08-22T13:10:49.185Z Reads: 312

```
I was able to measure the inside diameter of the hub where the tyre bead sits. Its 139mm. So it's closer to 5.5". Getting a spare tyre in going to be difficult and china might be the only option.

![IMG_20180822_103715_HHT|690x388](upload://yb7BBNfKVL3hMdMEqs85qfIbmZJ.jpg)

Yesterday I started playing around with Eclipse and attempting to build the WheelBoardMain firmware. I copied the git repo to Eclipse but I don't know what to do next.
```

---
## \#38 Posted by: mikenyc Posted at: 2018-08-22T14:17:36.829Z Reads: 305

```
that is awesome. do you think those hoosier tires will fit on this hub?
```

---
## \#39 Posted by: Nick_Talarico Posted at: 2018-08-23T03:34:50.574Z Reads: 298

```
Hi there! I am very curious about possibly making my one DIY one wheel. I was wondering if you'd think the wiring/coding aspects would be too difficult for someone with very limited experience?
```

---
## \#40 Posted by: lock Posted at: 2018-08-23T03:56:49.244Z Reads: 310

```
[quote="mikenyc, post:38, topic:15901"]
do you think those hoosier tires will fit on this hub?
[/quote]

I don't believe so. Hoosier doesn't make a tire for a 5.5in hub, in fact the tire that comes with the hub is the only 5.5in tire I've come across.

[quote="Nick_Talarico, post:39, topic:15901"]
someone with very limited experience?
[/quote]
I think that sums up my level of experience when it comes to electronics/embedded development, and I'm looking at giving it a go. Even if it is a failure, I'm sure there'll be much learnt along the way. There's several DIY implementations out there that seem to work. Unfortunately there's no real support community like what you'll find here when it comes to debugging VESC issues for example. Would be nice to see this grow.
```

---
## \#41 Posted by: puuhapet Posted at: 2018-08-24T04:21:23.928Z Reads: 296

```
The hub motor that I have is 5.5in and requires 5.5in tyre. The tyre that is on my hub is made by Liwang but I can't find that size on their webpage. I found one supplier in Alibaba for the size 11x6-5.5. I need to contact them If I could order just one because they have min order 500 pcs.

I'm also a beginner when it becomes to embedded development. I'm familiar with electronics so that helps. Some progress on the WheelBoardMain firmware. The firmware was created with CoIDE software but the company who has made software doesn't exist anymore. Luckily I was able to find version(1.78) of that software that opened the BalancingController.coproj-file that was in Github. After that I managed to build the firmware and flash it with the same CoIDE software and my SWD adapter. I don't have same hardware as described in github so that requires some changes in the GPIO ports.
```

---
## \#42 Posted by: lock Posted at: 2018-08-28T01:35:25.843Z Reads: 307

```
Well it's a start. 

Tire showed up last week, wheel yesterday. TBH I've never been a fan of tubeless tires, and getting this setup hasn't done much to alter my opinion. Those Youtube videos where the tire just pops on... they lie :joy:

![IMG_2286|447x500](upload://yXee4ggPJpHgl4WINPI0YUEDLzK.png)

Of course none of my installation issues were helped by the fact I don't have an air compressor. Still generous amounts of dishwashing liquid, and a bicycle track pump got the job done. Didn't hold pressure overnight (knew it was leaking at the bead), but soaking it in hot water, breaking the bead, then reseating it with max pressure seems to have fixed it.

It's a [Douglas magnesium wheel](http://dwtracing.com/product/m-series-kart-karting-gokart-dwt-douglas-wheel-rim-cerchio-racing/), with a Bridgestone 11x5-5 tire. Slimmer tire than what the Onewheel uses (and smaller hub diam), as I'll need to mount a drive pulley next to it and hopefully keep the same overall width. Whole thing weights 1.6kg (3.5lbs); lighter than a set of 107 ABECs.
```

---
## \#43 Posted by: mikenyc Posted at: 2018-08-28T02:35:04.981Z Reads: 286

```
What kind of belt are you going to use on this?
```

---
## \#44 Posted by: lock Posted at: 2018-08-28T03:30:23.832Z Reads: 282

```
Think I've settled on htd8 20mm in the hope it will never skip or break. Obviously the consequences are a little more severe than breaking an esk8 belt.  Don't see any reason to stick with htd5 out of convention; can't see any mechanical esk8 parts fitting in with this build.
```

---
## \#45 Posted by: mikenyc Posted at: 2018-08-28T10:54:34.090Z Reads: 272

```
are you going to be fabricating the gears? maybe you should look at chains
```

---
## \#46 Posted by: lock Posted at: 2018-08-29T08:32:47.710Z Reads: 265

```
Yeah, likely the large pulley will need to be fabricated... maybe even the hub. Should be able to find a small pulley easy enough.

Chains are definitely an option, width would be much lower than a comparable belt.
```

---
## \#47 Posted by: bheijden Posted at: 2018-09-09T09:05:56.816Z Reads: 274

```
I'm considering buying the same hub motor from Aliexpress:

https://nl.aliexpress.com/item/10inch-10-inch-10x6-00-5-5-wide-tyre-brushless-gearless-dc-wheel-hub-motor-balance/32823573279.html?isOrigTitle=true

Which voltage setup do you have and which would you recommend (36V or 48V)?

How would you rate the quality of the motor?

Do you think the motor can be controlled precisely enough to be able to balance the board properly? From what I understand, the motor contains hall sensors right?

Do you think the motor can generate enough torque for a controlled start-up?
```

---
## \#48 Posted by: puuhapet Posted at: 2018-09-10T07:39:11.769Z Reads: 266

```
I have the 48V version. Build quality seems ok but one complaint is the very short air valve. It will need some kind of extension when filling the tyre. The motor has hall sensors and I have rotated it in a test bench with a unicycle controller and it changes direction quickly. But I cannot confirm how the motor will work on the finished build.

I ran in to an issue with the STM32F103 and MPU6000 board. I can't get the I2C to work. I'm a total beginner with programming and debugging so it will take time. I also started playing with Arduino and separate MPU6500 module. I will test that combo within few days and see how it works. The code I'm using is from Github schglmnn/VESC-OneWheel.

Hardware side is work on progress. I have the U-shaped aluminium rails and some steel flatbar for mounting the hub motor in to the rail. Still have to get some wood for the foot pads and abs plastic for battery and electronics enclosures.
```

---
## \#50 Posted by: bheijden Posted at: 2018-09-15T21:57:47.877Z Reads: 280

```
That’s good to know, thank you! I just have two more questionsabout the motor. The title of the Aliexpress-ad says that the hub motor has 600W of power while, further down into the ad in the specification section, it states a “Max output power” of 1280.15W. In the same specification table the power outputted at maximum efficiency is 600W. I thought the convention with motor manufacturers was that they always posted the highest wattage instead of the power where the motor resides in the high efficiency ratio. The reason I am asking is that I want to be sure that the motor has enough power.

I figure that the motor suffices if it can output 600 W efficiently? Compared to the motor that @goldenHusky used (2250W), it is quite low on power… ?

I’m a total beginner when it comes to estimating the required power. I do understand this depends heavily on the things to want to achieve with the board. To give a small overview:

Weight (excl. board) = 85 kg
aimed top speed of 25 km/h
10s/12s setup

Second questions, is it easy to reverse the drive direction and does it perform equally well?

Thank you in advance!
```

---
## \#51 Posted by: pozsy Posted at: 2018-09-28T20:27:42.696Z Reads: 263

```
A little off but i think [this is](https://github.com/doublejosh/emmett/wiki) useful, a little build documentation and a nice collection of successful onewheel projects. (not mine)
I started to work on a onewheel style board now, so thanks for this thread.
```

---
## \#52 Posted by: puuhapet Posted at: 2018-10-01T06:05:18.981Z Reads: 274

```
Have to share what I found. One more DIY Onewheel build.

https://www.facebook.com/ZbLaB/
https://www.youtube.com/watch?v=0dq-1kT_1OI&t=1s
```

---
## \#53 Posted by: Dblaron Posted at: 2018-10-02T04:54:43.585Z Reads: 267

```
So I think I have found the right hub motor. Anyone interested in doing a group buy. I'm going to see how many people I can get. If possible I should be able to get the hub motors around $100 with enough people interested.
```

---
## \#54 Posted by: pozsy Posted at: 2018-10-02T09:21:47.193Z Reads: 265

```
Can you link it please?
```

---
## \#55 Posted by: mikenyc Posted at: 2018-10-02T10:59:16.094Z Reads: 265

```
Hey man how is your progress on this?
```

---
## \#56 Posted by: bheijden Posted at: 2018-10-02T13:59:09.481Z Reads: 271

```
Im possibly interessed! You have a link?
```

---
## \#57 Posted by: Dblaron Posted at: 2018-10-02T21:08:30.618Z Reads: 269

```
Here are the specs of the hub motor. 
Motor tubeless air tire size 254mm
motor tire width 156mm
dropout size 200mm
shaft length 260mm
motor power 48v 800w
max speed 35km/h

Right now I am in talks with the company about quantities. We may need at least 10 people interested. For better pricing. I also am trying to get a sample product for testing and quality control from the manufacturer.
```

---
## \#58 Posted by: Hegemon Posted at: 2018-10-03T20:58:52.811Z Reads: 261

```
Can you send me a Link?
```

---
## \#59 Posted by: lock Posted at: 2018-10-04T02:06:58.396Z Reads: 269

```
Well I've got a whole lot of excuses :smirk:

After ordering from APS a month or two back, it finally arrived. 80x100 12mm motor shaft, pictures don't do it justice, the thing is huge :joy: . There's probably enough parts now for me to be doing more on this than I have time for right now.
```

---
## \#60 Posted by: Dblaron Posted at: 2018-10-09T23:22:33.391Z Reads: 271

```
Ok everyone. I have a price now for an order of hopefully 10 or more. The price qouted was $85 USD to me. So let me know if you are interested and I will keep count for a couple of weeks. Just PM me. I will let you know if there are any shipping costs when I get the next email from the supplier.
```

---
## \#61 Posted by: Dblaron Posted at: 2018-10-09T23:52:11.102Z Reads: 279

```
Here is an image of the wheel that we will be getting. ![SCR10R_jpg-100766-380x380|380x380](upload://eKB1MIImJQcmwf8Dj7jfLVtqxds.jpeg)
```

---
## \#62 Posted by: littlem39 Posted at: 2018-10-11T18:04:50.202Z Reads: 268

```
You are from EU or US?
```

---
## \#63 Posted by: zack1 Posted at: 2018-10-18T23:48:51.354Z Reads: 264

```
Would be interested in a hub wheel..depending on shipping costs, current shipping costs is the same price of the hub wheel.
```

---
## \#64 Posted by: Battosaii Posted at: 2018-10-19T00:02:38.477Z Reads: 263

```
I wonder how 4 of those hub wheels would do on an electric go kart
```

---
## \#65 Posted by: mikenyc Posted at: 2018-10-19T00:44:06.518Z Reads: 264

```
I believe they're from a go kart
```

---
## \#66 Posted by: Dblaron Posted at: 2018-10-22T00:18:01.258Z Reads: 259

```
I would be doing this mainly for US residents. If I get enough people I can think about shipping to EU. So send me a private message if you are interested. Along with that put the country you are from so I can get a feel for who's looking.
```

---
## \#67 Posted by: zack1 Posted at: 2018-10-22T01:27:30.435Z Reads: 256

```
Not sure if 18 inch is too big https://www.peipeiscooter.com/18inch-450w-to-1000w-brushless-non-gear-dc-hub-motor-with-disc-brake-for-electric-scooter-phub-88.html
```

---
## \#68 Posted by: sayekim Posted at: 2018-10-22T15:36:09.656Z Reads: 251

```
That’s what she said
```

---
## \#69 Posted by: milanteubel Posted at: 2018-11-07T14:04:35.784Z Reads: 253

```
Is it to late to get my name in for a hub motor? I would be interested if the group buy is still open.  Also, I love the direction this thread is going!  I would love to have a Onewheel but can't justify the price.  It would be so cool if enough people built one that we can have a rough design plan for others that would be interested.  I really appreciate all the input so far, lets make this happen!
```

---
## \#70 Posted by: Flexo Posted at: 2018-11-08T15:03:39.752Z Reads: 250

```
@goldenHusky Do you remember what kind of pressure sensitive pads you used? I can't really find any I'm happy with :/
```

---
## \#71 Posted by: Remieknaapen Posted at: 2018-11-09T17:35:17.209Z Reads: 243

```
I would be interested in one depending on the price and if you are willing to ship to Europe (Neherlands).
```

---
## \#72 Posted by: goldenHusky Posted at: 2018-11-09T18:48:41.709Z Reads: 252

```
[quote="Flexo, post:70, topic:15901"]
Do you remember what kind of pressure sensitive pads you used? I can’t really find any I’m happy with :confused:
[/quote]

Selfmade with aluminium foil and velostat @Flexo
```

---
## \#73 Posted by: Flexo Posted at: 2018-11-11T01:43:38.731Z Reads: 245

```
Thanks :smiley:  I made one and it works, but I'm having trouble trusting it to be reliable in high speed situations. Did you do anything to make sure it wouldnt fail on you? @goldenHusky
```

---
## \#74 Posted by: fafi.azucar Posted at: 2018-11-11T04:03:09.459Z Reads: 239

```
so in a nutshell, what parts do i need to build one? asking for a friend
```

---
## \#75 Posted by: Flexo Posted at: 2018-11-11T20:39:19.884Z Reads: 250

```
@fafi.azucar I haven't made one yet, but I am planning my parts list. What I have planned to make/buy so far is

- Accelerometer
- Arduino (mega I think)
- VESC
- Gokart wheel with hub motor
- Led lights for the front and back
- Batterypack
- Aluminium rails
- Pressure sensitive pads
- Wooden plates for both ends
- Griptape
- On/off button
```

---
## \#76 Posted by: pozsy Posted at: 2018-11-12T09:01:33.903Z Reads: 240

```
Check the popular links at the top, there are quiet a few build descriptions in there. Those helped me a lot to start off this project.
```

---
## \#77 Posted by: Remieknaapen Posted at: 2018-11-16T11:04:18.050Z Reads: 242

```
@ [Dblaron](https://www.electric-skateboard.builders/u/Dblaron), i'm not able to send you a PM, but i'd love to join the group buy if that's possible!

I also managed to find spare tyres for this type of wheel.
https://www.peipeiscooter.com/dc-hub-motor.html?product_list_limit=30

What kind of voltage would do you guys prefer to use and why?
```

---
## \#78 Posted by: m303625 Posted at: 2018-11-18T08:48:08.363Z Reads: 244

```
The hoverboard hack is brilliant, the self balancing hardware and software is all done and it even has a pair of escs , just add motor and done, well with a couple of hiccups, escs are rated for 6.5inch 350w hoverboard motor the inventer only got theoretical 700w motor by combining both motors and using both escs, These hoverboard mainboards are cheap what about overvolting them to 12s vs 10s and possibly upgrading fets to run the single aliexpress hub motor?? you would only use one of the escs and one of the gyro boards with no other modification 
any opinions?
```

---
## \#79 Posted by: m303625 Posted at: 2018-11-18T11:03:43.802Z Reads: 283

```
ok just found some more info on the cheap hoverboard main boards
they should handle up to 13s which will increase both speed and torque, so 20+ should be no problem best to upgrade fet heatsinks for extra insurance, standard fets should be ok but check ratings as they vary depending on what they can get their hands on!
this is all with standard firmware (propriety)
or another option is to use electric unicycle mainboard
https://www.aliexpress.com/item/FREE-SHIPPING-Electric-unicycle-controller-self-balancing-electric-unicycle-motherboard-electric-unicycle-accessories/32822691199.html?spm=2114.search0104.3.201.8fd85934bWfMjo&ws_ab_test=searchweb0_0,searchweb201602_4_10065_10068_10130_10547_319_317_10548_10696_10924_453_10084_454_10083_10618_10920_10921_10922_10307_537_536_10131_10132_10133_10059_10884_10887_100031_321_322_10103,searchweb201603_51,ppcSwitch_0&algo_expid=5c502d18-fedd-4c62-95cc-28aeed8f13b5-30&algo_pvid=5c502d18-fedd-4c62-95cc-28aeed8f13b5
 probably very similar but these are rated around 60v, not sure how the larger 14+inch wheel size will affect things though?
```

---
## \#80 Posted by: puuhapet Posted at: 2018-11-18T16:35:53.570Z Reads: 276

```
At first I was going to use a unicycle main board. The biggest problem was that the the board had to be mounted vertically like in the unicycle on the side of the wheel. Could not find a different firmware where the gyro axis would be swapped.

I ended up using a VESC 4.12 and an old Naze32 flight controller board from a quadcopter. Here is the link to Alex B's code that I used. https://github.com/blezalex/WheelBoardMain. Still have some work tweaking the PID's but I can ride the board for short trips.
```

---
## \#81 Posted by: m303625 Posted at: 2018-11-18T21:48:26.960Z Reads: 278

```
good work, are you going to further develop the code?
I threw out all my old naze32 boards!! all f4 now
I am good with electronics hardware but my coding sucks, am interested though done a little with arduino using their IDE any advice where to start? eg what IDE to use and how do you compile and upload to the board?? written in some version  of C I assume?
```

---
## \#82 Posted by: puuhapet Posted at: 2018-11-19T07:05:09.242Z Reads: 266

```
I'm also not good with coding. Learned enough to get my board working. Alex B helped me to get his code working on my Naze32 board. You have to use CoIDE, compile and flash his firmware. 

If you want to use arduino+MPU6050 board check this https://github.com/schglmnn/VESC-OneWheel. I got this working also but I was not happy with it.
```

---
## \#83 Posted by: Sindre Posted at: 2018-11-19T19:46:57.312Z Reads: 263

```
![46458674_271080610419354_3395996667755888640_n|279x500](upload://qWjqzN5HYFyeyiZma13xjCVuU9L.jpeg) !

Working on my own one wheel atm, was trying a weekend build.
Everything is done, just need the controller. Diddent have a gyro laying arround so trying to use a microbit, but dosent have my hopes up
```

---
## \#84 Posted by: mikenyc Posted at: 2018-11-19T20:03:44.218Z Reads: 255

```
![image|279x500](upload://mxX27vwWmWoLj6U9Zh2p4S7mj5T.jpeg)
```

---
## \#85 Posted by: m303625 Posted at: 2018-11-24T04:44:33.733Z Reads: 253

```
why not try using a hoverboard esc mainboard, they are cheap and the firmware is good to go ?
eg https://www.aliexpress.com/item/Universal-for-6-5-8-10-Inch-2-Wheels-Self-Balancing-Electric-Scooter-Parts-Hoverboard-Motherboard/32796726976.html?spm=2114.search0104.3.1.cf092d13h4Dosg&ws_ab_test=searchweb0_0,searchweb201602_4_10065_10068_10130_10547_319_317_10548_10696_10924_453_10084_454_10083_10618_10920_10921_10922_10307_537_536_10131_10132_10133_10059_10884_10887_100031_321_322_10103,searchweb201603_51,ppcSwitch_0&algo_expid=7ad6e412-a68c-4998-85d7-3bca2d02bb4a-0&algo_pvid=7ad6e412-a68c-4998-85d7-3bca2d02bb4a
```

---
## \#86 Posted by: Remieknaapen Posted at: 2018-11-24T22:28:44.042Z Reads: 246

```
Looks really nice i must say! What type of motor do u use, what voltage and how many Watt?
And how many Cells are u using?
```

---
## \#87 Posted by: fafi.azucar Posted at: 2018-11-30T22:27:05.079Z Reads: 238

```
can u put up the parts u used? maybe the links too? it would be helpful😊
```

---
## \#88 Posted by: Sindre Posted at: 2018-12-01T20:10:42.415Z Reads: 241

```
https://www.aliexpress.com/item/10inch-10-inch-10x6-00-5-5-wide-tyre-brushless-gearless-dc-wheel-hub-motor-balance/32823573279.html?spm=2114.search0104.3.1.6db95eb8nGaR6K&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10068_319_10059_10884_317_10887_10696_100031_321_322_10084_453_10083_454_10103_10618_10307_537_536,searchweb201603_51,ppcSwitch_0&algo_expid=ac48397c-2d43-42b2-b1b5-d8754150122c-0&algo_pvid=ac48397c-2d43-42b2-b1b5-d8754150122c

Im running it on 12s vesc6 with 20-30A
It peaks on 1600w or so, and seem to really strong. I programed a microbit since i diddent have an gyro breakout laying arround, but the microbit wasent fast enuff and also did software imlement ppm. This made it unstable and lagg. This was supposed to be a weekend project, but im stuck with exams for now. Il make an propper build thread and post source code and parts in late desember. Im using 12s 3p from old laptop cells 18650.
```

---
## \#89 Posted by: Sindre Posted at: 2018-12-01T20:11:26.277Z Reads: 235

```
Im working on building my own vesc6 that are really small. Il post a propper thread when im finished with them
```

---
## \#90 Posted by: fafi.azucar Posted at: 2018-12-01T22:27:50.174Z Reads: 228

```
waaah. i'm very excited i'll wait for that thread😍😍😂 goodluck on your exams boi✌
```

---
## \#91 Posted by: mikenyc Posted at: 2018-12-01T23:56:37.185Z Reads: 231

```
Are you going to include the imu?
```

---
## \#92 Posted by: m303625 Posted at: 2018-12-02T05:38:14.522Z Reads: 238

```
Great looking fwd to the build thread, which gyro are you planning to use? and what are you basing the firmware on? 
would be good to develop the code to add features as they come up!
```

---
## \#93 Posted by: m303625 Posted at: 2018-12-07T21:26:10.287Z Reads: 246

```
found this firmware which uses a naze32 flight controller and VESC to run the board
https://github.com/blezalex/WheelBoardMain
there is also a youtube video showing it working
https://www.youtube.com/watch?v=4-E7deaGyFs
```

---
## \#94 Posted by: m303625 Posted at: 2018-12-08T06:33:01.398Z Reads: 239

```
ok I got the CoIDE and toolchain setup and can compile the AlexB's code just waiting on motor and vesc
have ordered a naze32 rev6 as that is all i could find on ebay, there is some SWD pads on the back of the board, is this where you attach the stlink programmer? I assume some of these pads trace back to the F1 chip (swio and swclk) is this the same board you used?![naze32Back|690x459](upload://yiJB7HixxTHKnInhIzjCEoZJEjM.jpeg)
```

---
## \#95 Posted by: puuhapet Posted at: 2018-12-08T20:44:18.878Z Reads: 231

```
The board looks the same as I have. Those pads should also have GND and VDD. Use a multimeter to find out which pads are connected. If that board is the same as I have you will need to modify Alex B's code because he used Flip32 board and the I/O-ports are different. I can share my code so it should work ok. Alex B used two force sensing resistors in the footpads. I only have one pushbutton switch in one footpad. I'm going to build a footpad sensor with Velostat then it will behave almost the same as force sensing resistor.
```

---
## \#96 Posted by: kmorgan Posted at: 2018-12-08T23:54:07.883Z Reads: 232

```
Have you ordered a wheel yet? Or you still looking for people interested?
```

---
## \#97 Posted by: m303625 Posted at: 2018-12-10T10:05:19.371Z Reads: 226

```
can you please share your code?
thanks
```

---
## \#98 Posted by: puuhapet Posted at: 2018-12-10T10:22:43.554Z Reads: 229

```
I have it on my old laptop. I will uploaded it today to my Google drive. I will share the link here.
```

---
## \#99 Posted by: puuhapet Posted at: 2018-12-10T19:10:22.419Z Reads: 223

```
Here is the link for the code

https://drive.google.com/drive/folders/1QKhA-TFG5KrmGJzb5k4WjjoFu8RLj9_o?usp=sharing

Original files can be found here
https://github.com/blezalex/WheelBoardMain
```

---
## \#100 Posted by: Remieknaapen Posted at: 2018-12-11T20:32:00.256Z Reads: 207

```
Is it possible for you guys to make a small write-up on how you managed to upload the code to the Naze32?
```

---
## \#101 Posted by: brenternet Posted at: 2018-12-11T20:34:15.097Z Reads: 210

```
[quote="sayekim, post:68, topic:15901, full:true"]
That’s what she said
[/quote]

This is the most underrated comment of 2018
```

---
## \#102 Posted by: sayekim Posted at: 2018-12-11T21:02:47.497Z Reads: 213

```
I know right what the hell.

I’d totally jump on that... 

That’s what she said.
```

---
## \#103 Posted by: m303625 Posted at: 2018-12-13T02:20:44.116Z Reads: 212

```
still waiting for my naze to turn up but from what i understand here is the procedure
get CoIDE to compile the code
use cheap stlinkv2 dongle and software from st microelectronics to upload to board
use the swd pins on the back of the naze rev6 board, foot sensor pads connect to ppm input 1 & 2 and output for vesc is maped to motor one pin (use puuhapet's code and a naze32 rev6)
```

---
## \#104 Posted by: puuhapet Posted at: 2018-12-13T18:51:35.867Z Reads: 205

```
You can compile and flash with the CoIDE. No need for other software. Windows might need some drivers to discover the stlink dongle.
```

---
## \#105 Posted by: b4ng4r4ng Posted at: 2018-12-15T18:47:50.344Z Reads: 204

```
@Dblaron, I'm interested in the group buy if you are still considering. US resident. Please keep us posted! Thanks!
```

---
## \#106 Posted by: Sindre Posted at: 2019-01-06T23:21:41.673Z Reads: 204

```
Do you still have the firmware for this?
```

---
## \#107 Posted by: Sindre Posted at: 2019-01-06T23:50:27.649Z Reads: 204

```
https://www.electric-skateboard.builders/t/onewheel-build-guide/80129
```

---
## \#109 Posted by: Fungineers Posted at: 2019-03-17T08:48:41.957Z Reads: 179

```
Wow! This is quite a thread. Unfortunately looks like not many people succeeded. So, I am going to take a jab at it. I have a YouTube channel by the name of 'Fungineers' and I have built Skateboards, battery packs, and stuff with Arduino. However, this seems like quite some work (needs a lot of time and money). 
I will try to post updates here, but mostly on my channel. Anyone else still working on this project?
```

---
## \#111 Posted by: Fungineers Posted at: 2019-03-17T18:36:59.832Z Reads: 173

```
Hey @Sindre nice build. 
So you used the Naze32 and it works ok? Why not an Arduino+gyro?
```

---
## \#112 Posted by: Fungineers Posted at: 2019-03-17T18:44:42.530Z Reads: 171

```
@goldenHusky awesome build man! Too bad you dont have it any more. Why Arduino mega tho? Isnt a Nano or Uno enough for the IO?
```

---
## \#113 Posted by: goldenHusky Posted at: 2019-03-18T13:26:12.175Z Reads: 163

```
@Fungineers  Thanks! The mega has more processing power, I thought it would be useful, it was just a single onewheel so I made no cost improvements.
```

---
## \#114 Posted by: StefanMe Posted at: 2019-03-18T13:57:18.999Z Reads: 164

```
Holy shit... why have I opened the thread. 

🤦🏻‍♂️
```

---
## \#115 Posted by: Fungineers Posted at: 2019-03-18T14:29:07.817Z Reads: 164

```
@goldenHusky thanks for replying. So did Arduino+gyro work flawless? Did you write your own code?
Also please can you give me the dimensions of the aluminium rails. They look exactly like the real deal. How the hell did you get them made?
```

---
## \#116 Posted by: goldenHusky Posted at: 2019-03-19T08:39:02.106Z Reads: 165

```
@Fungineers  Yes, it worked, I oriented myself at various projects on github to get an idea on the PID loop and other stuff, the alu rails are standard sizes you can purchase in any metal shop, I don't remember the exact dimensions but it was a multiple of 5mm, something like 40x20
```

---
## \#117 Posted by: antonyo Posted at: 2019-03-31T07:31:27.230Z Reads: 153

```
so has anyone gotten the dimensions on the rails yet?
```

---
## \#118 Posted by: ervinelin Posted at: 2019-03-31T08:01:16.875Z Reads: 163

```
Which GitHub repository did you use in the end?
```

---
## \#119 Posted by: goldenHusky Posted at: 2019-03-31T16:09:38.588Z Reads: 160

```
A mixture of multiple.
```

---
## \#120 Posted by: Remieknaapen Posted at: 2019-04-17T20:25:53.494Z Reads: 154

```
Hi Puuhapet,

I received my st-link programmer and naze32 today.
What outputs on the st-link do i need to use to connect it to the naze32?
And what input pins do i need to use on naze32?
```

---
## \#121 Posted by: antonyo Posted at: 2019-04-19T05:20:55.958Z Reads: 144

```
how does this compare to a onewheel?
```

---
## \#122 Posted by: Remieknaapen Posted at: 2019-04-25T12:30:47.732Z Reads: 145

```
Did you 
get the naze32 programmed with the st-link ?
```

---
## \#123 Posted by: Fungineers Posted at: 2019-05-12T08:14:26.714Z Reads: 137

```
Hi guys. Been a while! 
It looks like many people have initiated their own builds, which is great! 
Here's my progress: Built myself a VESC. Blew it! So built another one, and am gonna program it with stlink. 
The Omniflight f4 flight controller just arrived in the mail. Perfect timing. So time to tinker with the flight controller. I think this is the most difficult bit right here. @Remieknaapen did you make any headway? Also, Im confused: why would you need to flash firnware on your Naze? If you bought it it should come preinstalled with firmware. What am I missing? 
Also, anyone has any ideas/ schematics on connecting the flight controller to the VESC and setting up the PIDS, etc.? Any help is appreciated. 
Thanks!
Fungineers.
```

---
## \#124 Posted by: Remieknaapen Posted at: 2019-05-12T20:07:31.820Z Reads: 143

```
Hi Fungineers!

The new code for the naze32/flip32 is a dedicated onewheel code and makes it possible to use footpad sensors to start the onewheel. I don't know i you can use the stock drone software that comes installed on the control board.
If you are interested, in the following topic someone is building a code to use an arduino with MPU6050, Still figuring out the code and get it to work, you can see the progress over here https://www.electric-skateboard.builders/t/onewheel-build-guide/80129/51

I made some progress myself and managed to upload the new code to my naze32. Also my velostat sensor are working but i can't seem to the get my naze32 with the new code armed or activated by pressing the footpad sensors. The esc output does work though, so my guess is that I need to tweak to code in someway.
```

---
## \#125 Posted by: Fungineers Posted at: 2019-05-14T06:52:01.159Z Reads: 138

```
Do you know if the firmware for the NAZE will also work on my OMNIFLIGHT? I mean it should, since the processor is the same (ARM).
I will try to upload the firmware on the Omniflight and see if it works. Could you please advise how you flashed the firmware? Did you supply external power or power from the stlink? How were your connections?

Thanks
Fungineers
```

---
## \#127 Posted by: dawn Posted at: 2019-06-18T12:59:07.532Z Reads: 118

```
hi,it is beautiful one wheel skateboard.if you want do it,we can provide these hub motor wheel.:face_with_hand_over_mouth:
```

---
## \#128 Posted by: dawn Posted at: 2019-06-18T13:00:19.895Z Reads: 115

```
hello,i am Dawn from peipeiscooter,we can provide many kinds hub motor wheels,contact me.:smiley::smiley::smiley:
```

---
## \#129 Posted by: StefanMe Posted at: 2019-06-18T20:55:45.360Z Reads: 115

```
I try to buy a hub motor from your side (over AliExpress), your response is horrible. First order U just delivered nothing (but give a delivery Garantie within 8 days) and my new order a few days ago is still „the seller is processing your order“ . A little bit strange when u take 55€ for delivery. 

At the moment I cannot recommend your store. But let’s see how the quality of there’s motors are.
```

---
## \#130 Posted by: s.white432 Posted at: 2019-06-22T22:35:33.941Z Reads: 102

```
This peipeiscooter hub motor has a 15x6.00-6 tyre:

https://www.aliexpress.com/store/product/15inch-15-inch-widen-tire-15x6-00-6-tyre-BLDC-brushless-non-gear-hubwheel-motor-for/1470068_32824407612.html?spm=2114.12010612.8148356.69.f8422286up9YmM

The FM Onewheel has a 11.5 X 6.0-6. I'm wondering whether the 15 inch tyre could be replaced with a standard 11.5 or 11.0 inch go-kart tyre or is the hub geometry likely to be incompatible?
```

---
## \#131 Posted by: Surfer Posted at: 2019-06-23T08:14:17.669Z Reads: 101

```
Maybe it fits but just the weight is 9 kilo 🤪 from the specs on the link.
There is some ow motors on sale, not super crazy expensive but they run 58~63 volts, 14s-15s then vesc will not work
```

---
## \#132 Posted by: Fungineers Posted at: 2019-06-26T19:13:06.900Z Reads: 97

```
Hey guys, been working hard these past few weeks.
The mechanical assembly is almost done. 
The hard part is the code which Im working on. 
@Remieknaapen and @MaxGoldenson are also working on the same thing so might have one soon!
![IMG_20190625_190700|666x500](upload://ovy8YKEgpxGbqLpftv2IhZGrRfu.jpeg) 
Im gonna post updates on the YouTube channel regularly:   
https://youtu.be/65Tv4kycUSg
```

---
## \#133 Posted by: Surfer Posted at: 2019-06-26T19:17:29.541Z Reads: 92

```
I would like to give more likes :slight_smile:
The code for what are you guys working is for vesc 4.12 or vesc 6?
```

---
## \#134 Posted by: Remieknaapen Posted at: 2019-06-26T20:39:23.852Z Reads: 93

```
Nice introduction Fungineers!! Keep up te good work.

I will post some information and pictures of my build next week!
```

---
## \#135 Posted by: Fungineers Posted at: 2019-06-27T10:25:57.014Z Reads: 85

```
Thanks @Surfer 
Im working on 4.12, but it shouldnt matter as the communication protocol is the same for both version as far as I know. I could be wrong though.
```

---
## \#136 Posted by: Hegemon Posted at: 2019-07-03T22:37:05.268Z Reads: 79

```
Doing a 12S Setup. Should I get a 48V or 60V Motor at 600W? I'm assuming the 48V should be good enough since the voltage will drop and there should be enough of a safety margin on the components but I just wanted to get some more opinions.
```

---
## \#137 Posted by: Fungineers Posted at: 2019-07-31T18:31:02.167Z Reads: 62

```
48 should be good.
```

---
## \#138 Posted by: Fungineers Posted at: 2019-07-31T18:32:07.311Z Reads: 61

```
Progress: 
I did run the whole setup on the bench successfully. Waiting for the rails to be painted and come back!

https://youtu.be/RZwWWSBSPQk
```

---
## \#139 Posted by: Bionic24 Posted at: 2020-02-09T22:28:42.255Z Reads: 17

```
Older posts already but perhaps someone can help with this. I have been trying to flash the Mainwheel repository from @blezalex to a Naze32 Rev5 board. Flashing succeeded with Betaflight configurator, but there is no data coming through on the app when I connect it with my phone. first boot shows a solid blue LED and a fast blinking red light. hot reboot only gives solid Blue on the flightcontroller.

Is see people here are using ST-link programmer to flash the board. Is this because the original bootloader needs to be replaced? Someone that succeeded with this and that can help me out?

[edit] I soldered DIO/GND/CLK to the bottom pads and flashed the hex file with my ST linker. Flashing and verification runs smooth and without errors but the outcome is the same? Perhaps it is a baudrate thing?

@Remieknaapen I see you are from the Netherlands as well, perhaps we could get in touch?
```

---
## \#140 Posted by: Fosterqc Posted at: 2020-02-10T05:06:40.937Z Reads: 15

```
hey buddy! we just need to get your level up then you can PM
```

---
