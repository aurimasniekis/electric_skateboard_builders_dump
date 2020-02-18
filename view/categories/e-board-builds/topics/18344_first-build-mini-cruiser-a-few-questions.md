# First build mini-cruiser a few questions

### Replies: 47 Views: 3068

## \#1 Posted by: amc Posted at: 2017-02-27T23:26:46.200Z Reads: 196

```
Hey!

Im trying to convert my mini-cruiser from Dusters. I really would like the board to be strong enough
to get up hills in city, not that steep. So I guess a dual is required. Have a look at the images, what do you guys think?

Ive got a list to buy (havent dont' this yet) of all the parts from hobbyking. Im planning to create the
pulley and buy the rest if I can find them in some store.

<img src="/uploads/db1493/original/3X/f/a/fa3e9a64ef2da02910bcd14e9559e84b5ef0d7f5.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/a/b/ab2f556b170f60d007af3f7fe24beee46abb40b3.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/e/7/e7a9dbc83dbff72abe46194b5f55af0da3d39982.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/d/1/d16e3e85b26db5b6e70a3afc01cbd84bee7914b1.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/a/4/a4146a9961a7bf84f0229a23ba7ba5013afbcae1.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/a/3/a3ab5e6cf663803aefbc783c9e3a24f171e29f40.jpg" width="666" height="500">
```

---
## \#2 Posted by: IsTalo Posted at: 2017-02-28T12:22:44.049Z Reads: 163

```
Tell us the parts that you want to buy, and tell me the size of that wheel
```

---
## \#3 Posted by: amc Posted at: 2017-02-28T15:14:17.084Z Reads: 159

```
Hi! Thanks!

Well, these are the parts I think I need. I list both dual and single config. But perhaps a single has 
enough power?

Two motors (dual build): [**Turnigy Aerodrive SK3 - 5055-280kv Brushless Outrunner Motor**](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-280kv-brushless-outrunner-motor.html)

One motors (single build): [**Turnigy Aerodrive SK3 - 6374-192kv Brushless Outrunner Motor**](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html)

Two esc (one for single build):  [**Hobbyking YEP 100A (2~6S) SBEC Brushless Speed Controller**](https://hobbyking.com/en_us/hobbyking-yep-100a-2-6s-sbec-brushless-speed-controller.html)

Rest the same for dual and single motor build.

One splitter: [**XT60 Harness for 2 Packs in Series (1pc)**](https://hobbyking.com/en_us/xt60-harness-for-2-packs-in-series-1pc.html)

Two batteries: [**MultiStar LiHV High Capacity 5200mAh 6S 10C Multi-Rotor Lipo Pack**](https://hobbyking.com/en_us/multistar-lihv-high-capacity-6s-5200mah-multi-rotor-lipo-pack.html)

One remote: [**Quanum 2.4Ghz 3ch Pistol Grip Tx & Rx System**](https://hobbyking.com/en_us/quanum-2-4ghz-3ch-pistol-grip-tx-rx-system.html)

The wheelsize says: 66mm
Depth of the wheels is: 50mm
Trucks (between bearings) is: 120mm
Length between wheels is: 117mm


Thanks!!
```

---
## \#4 Posted by: IsTalo Posted at: 2017-02-28T15:32:06.654Z Reads: 133

```
But U wanna plug that batteries in parallel, right? Use Vesc, Maybe Its better for this motors
```

---
## \#5 Posted by: IsTalo Posted at: 2017-02-28T15:34:09.050Z Reads: 130

```
And I think 66mm is a bit small, I don't know, You need to ask the experts
```

---
## \#6 Posted by: amc Posted at: 2017-02-28T15:36:54.305Z Reads: 125

```
How do you mean parallel? And what is the difference between ESC and Vesc?
```

---
## \#7 Posted by: amc Posted at: 2017-02-28T15:38:34.861Z Reads: 126

```
Also, it seems the dual motor config will not fit two motors
Total Length E(mm): 81.00. Or would it work with my trucks?

....and I don't get these measurments. Its says length 140mm that is very big.
```

---
## \#8 Posted by: IsTalo Posted at: 2017-02-28T15:54:49.980Z Reads: 127

```
Man, When you connect two batteries (ex:6s) in Series (Positive with Positive) it will double the voltage (ex:12s). When you connect in Parallel (Positive and Negative) it will give the double of Mah.

> Vesc

Vesc is a ESC made by Vedder that is the better one for eSK8, It have some features that other don't have, I think the most important is the BLDC tool, that you can ajust the configuration of your ESC. It is a bit more expensive, but it's better. Vesc has Regenerative Breaks, Current Control, Voltage Cut off, and a lot of other features, like the UART port that, with an arduino, you can read the Data of your motor.

> About the trucks

I really don't know, you need to calculate it your self, with the motor mounts you wanna use, and a lot of Trucks have curves, It can be a problem, mine have this problem so I sanded to fit. But let's make a simple calculation, Two Motor that have 55mm lenght, so it's 110mm, just the motor, plus the Motor Mount, something between 2mm and 6mm, and plus the Motor Pulleys. You could Make a dual drive but in differents trucks, one motor on the front, one motor on the back.
 But if you are Light, I think a Single motor would probably work.

> I don't think Quanum is a good remote

Buy GT2B and 3d print BadWolf Enclousure, of Buffalo, you decide, a lot of people don't like Quanum, but you do what you want. I bought Alien Power Remote, everybody says it is good.

## AND AGAIN, READ MORE, I'M NOT A EXPERT
```

---
## \#9 Posted by: amc Posted at: 2017-02-28T17:06:37.236Z Reads: 108

```
Thank you so much for all the info! This is great!

Yes I think I need to start with a single motor, probably cheaper. Later I might put one in the front too. Great about the control, really worth the extra money.
```

---
## \#10 Posted by: IsTalo Posted at: 2017-02-28T17:11:05.238Z Reads: 105

```
You're Welcome, About the battery, with this motor [quote="amc, post:3, topic:18344"]
Turnigy Aerodrive SK3 - 6374-192kv Brushless Outrunner Motor
[/quote] you can run max 10s, or it will burn VESC
```

---
## \#11 Posted by: amc Posted at: 2017-02-28T17:12:14.862Z Reads: 98

```
You mean max 2 of those? 5000mah each?
```

---
## \#12 Posted by: IsTalo Posted at: 2017-02-28T17:25:49.224Z Reads: 91

```
NO man, max 10s, if you buy 2 6s and use the plug that you linked u will burn your vesc, but with 6s you don't have the max power that you could, search for 10s batteries, or two 4s and use that plug, and it will turn a 8s
```

---
## \#13 Posted by: amc Posted at: 2017-02-28T17:31:46.017Z Reads: 86

```
Ok get it! Thanks! Do you have a link to that VESC?
```

---
## \#14 Posted by: saul Posted at: 2017-02-28T18:14:22.571Z Reads: 89

```
whats your budget? range, speed, weight...

a single vesc build can do almost anything but you will spend at least $500-600.

those wheel wont have enough clearance for the motors. you'll want at least 80mm. 90/97mm are smooth af!
```

---
## \#15 Posted by: amc Posted at: 2017-02-28T18:22:40.062Z Reads: 93

```
Hi!

This is my first build so max $500 incl shipping to Sweden.

My weight is 70kg. I would like to get up hills in the city. Stockholm is not that
steep. Speed max 30km/h I guess. The law in Sweden is max 20km/h what I know...but hey....
Range is ok around 15 to 20 km or more would be fantastic.

I like the board I have. Getting new trucks would make it look strange but probably more stable. I guess I would
be able to fit the motor etc.




Thanks!
```

---
## \#16 Posted by: saul Posted at: 2017-02-28T18:34:02.496Z Reads: 93

```
it will be really close, but if you can make some of the parts yourself and find some deals it can be done.

I'm trying to convert because we still use stone age units here....but those number seem very realistic.

[Build guide](http://esk8.today/guides/build-guide/) build #1 is what i'm running now. i need to correct it. is actually does about 26km range. so you could do smaller batteries...
```

---
## \#17 Posted by: amc Posted at: 2017-02-28T18:44:55.281Z Reads: 94

```
Looks great! I will have a look at that.
```

---
## \#18 Posted by: IsTalo Posted at: 2017-02-28T18:57:47.853Z Reads: 91

```
You that is in Europe, Search for sites like Alien Power (I can send you a Coupon) and ESK8.DE
```

---
## \#19 Posted by: IsTalo Posted at: 2017-02-28T21:12:31.213Z Reads: 87

```
You can buy it at, Enertiom, Alien Power Systems, DIY electric skateboard, Miami Boards
```

---
## \#20 Posted by: amc Posted at: 2017-02-28T21:57:47.039Z Reads: 88

```
Great thanks! I really appreciate your help. Will check esk8.de, was not that cheap what I can see. Gonna look at the rest too.
```

---
## \#21 Posted by: amc Posted at: 2017-02-28T22:23:38.558Z Reads: 85

```
There is really a lot to get into here. I will probably pick:
[Turnigy Aerodrive SK3 - 6374-192kv](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html) (later I might put one in the front) or if there are any similar good at the same price? I feel its pretty expensive.

**Price: $92.29**

For battery two cheap 5000mAH 4s. Cable to connect them. Ive looked at this one, but I really would like a slimmer model. This is 33mm. [ZIPPY Flightmax 5000mAh 4S1P 20C](https://hobbyking.com/en_us/zippy-flightmax-5000mah-4s1p-20c.html)

**Price: $61.44**

Some remote with receiver, Alien Power Remote looks good, saw other models at esk8.de. But there must be cheaper ones somewhere.

The pulley I will try to construct myself. Will grind the trucks somehow...  The motor and wheel drive mechanism, I guess that would be simplest to find somewhere.

Then there are wheels, I guess Ebay might have some stuff?

The only thing that is confusing me is the VESC thing. Which one to pick? It would be great if I could break and regulate speed.
```

---
## \#22 Posted by: IsTalo Posted at: 2017-02-28T22:31:08.205Z Reads: 80

```
Look at this [motor](diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/), you can even buy [The VESC there](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/), they have [great remotes too](diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/), If you buy 300$ there the Shipping will be free. 

About the battery, I really don't know, you could buy at alien, and buy the other parts there too, Because there the shipping will be the same if you buy a cable or if you buy a battery, so buy the many of things you want there. At Ebay you can buy a Charger, search for 8s charger, and some wheels
```

---
## \#23 Posted by: amc Posted at: 2017-03-01T21:33:26.768Z Reads: 74

```
Thank you so much for all your support! Yes, they look good. The $300 is amazing. Well, all this is new to me so I take it slow on the stuff. Just want my first board to be cheap and work "good enough". I will continue my research.
```

---
## \#24 Posted by: mmaner Posted at: 2017-03-01T21:36:11.784Z Reads: 69

```
Not to take anything away from Dexter, the products they sell are great, although I'm not a huge fan of the remote.  I'd take a look at the [MEB Remote](https://miamielectricboards.com/shop-1/handheld-electric-remote).  Its the one I use, in fact I have 3 of them.
```

---
## \#25 Posted by: amc Posted at: 2017-03-01T21:39:30.620Z Reads: 76

```
Hi and thanks!

The most important part for me is breaking and having the ability to regulate speed, slow to faster. Not just press and fast.... If that is possible with the VESC of course. The remote must be able to do this. Or do they all?
```

---
## \#26 Posted by: mmaner Posted at: 2017-03-01T21:45:50.479Z Reads: 74

```
The VESC offers the best torque control of any ESC available.  I doubt anyone would argue with that.  There's still some finesse involved with remotes, no matter how good a remote it is.  I have found the best to be the [Benchwheel remote](https://miamielectricboards.com/shop-1/handheld-electric-remote) like @oriol360 sells.  I am partial to thumb remotes, I find at high speeds, with bumps and carving, that it offers the best control. 

If you want to look at acceleration and break curves checkout the [Extended BLDC-TOOL](http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286) with Watt Control Mode by@Ackmaniac.  There's also the [VESC Data Log Analyzer](http://www.electric-skateboard.builders/t/vesc-data-log-analyzer-vdla/16582) by @DeathCookies.  This combination makes tweaking your VESC settings pretty simple and incredibly accurate.
```

---
## \#27 Posted by: IsTalo Posted at: 2017-03-01T21:55:04.581Z Reads: 72

```
Yeah, but if the shipping pass 60$ would be better to him to buy the remote at DIY
```

---
## \#28 Posted by: mmaner Posted at: 2017-03-01T21:57:09.635Z Reads: 70

```
I was just talking about the remotes brother.  I'm not a huge fan of the nano remote and think its probably a bad idea for a new rider to use as it has had drop-out issues & the travel isn't that great.
```

---
## \#29 Posted by: IsTalo Posted at: 2017-03-01T21:59:51.843Z Reads: 67

```
[quote="mmaner, post:28, topic:18344"]
I was just talking about the remotes brother.  I'm not a huge fan of the nano remote and think its probably a bad idea for a new rider to use as it has had drop-out issues & the travel isn
[/quote]

He could use the Mini remote, and another thing, Miami don't have World Wide shipping
```

---
## \#30 Posted by: mmaner Posted at: 2017-03-01T22:37:37.579Z Reads: 64

```
[quote="IsTalo, post:29, topic:18344"]
He could use the Mini remote
[/quote]

No one said he couldn't, just said its not a great remote, whereas the Benchwheel is.
[quote="IsTalo, post:29, topic:18344"]
Miami don't have World Wide shipping
[/quote]

But with a little bit of searching, its pretty easy to find other options like [this](https://www.aliexpress.com/item/Electric-skateboard-refitting-parts-remote-control-bench-technology/32731985084.html?spm=2114.13010608.0.0.S5hVGU).

This post will tell you a lot about remotes.
http://www.electric-skateboard.builders/t/remotes-commercially-available-options/15162

I don't understand why you are arguing about this, I was just offering an opinion.  One that is based in experience with a lot of remotes, so I figure it might be worth something to someone.
```

---
## \#31 Posted by: IsTalo Posted at: 2017-03-01T22:40:16.597Z Reads: 60

```
[quote="mmaner, post:30, topic:18344"]
I don't understand why you are arguing about this, I was just offering an opinion.  One that is based in experience with a lot of remotes, so I figure it might be worth something to some
[/quote]

I'm not arguing, I just said that he could save money buying at DIY, you said that the remote is not that great, I really don't know if it is or is not great, I bought my controller at Alien, so I really don't know
```

---
## \#32 Posted by: amc Posted at: 2017-03-02T06:47:59.643Z Reads: 60

```
I feel the Benchwheel remote is very good, after watching the video explaining it. Also like that it has a slim receiver. But like IsTalo says its not good if they do not ship worldwide or expensive doing so. Saving money there is no argue that DIY is the best way to go. For me on my budget and first build.

A question about motors. Is everyone that loud?
```

---
## \#33 Posted by: amc Posted at: 2017-03-02T14:42:07.598Z Reads: 60

```
Okay guys i've looked closer on the DIY shop, the motor there 5065 version looks good (dexter recommended it because its consumes less power and still pretty good performance). Also the VESC I could get from there. The nano remote, as mentioned by mmaner, and the issues isn't that promising though. The batteries are superexpensive. Dont get that. So my question, is there any other shop you guys can recommend that has all the stuff? Its really not easy finding all these parts :slight_smile: In some way, maybe pick a few things from hobbyking, like motor and batteries. Then buy the VESC and remote somewhere else? Please, if anyone have a suggestion, for either collect everything from the same shop or pick some other for only remote and vesc. I live in Sweden, so the shop needs to deliver there. Thanks!!
```

---
## \#34 Posted by: amc Posted at: 2017-03-02T15:22:23.131Z Reads: 59

```
Im looking at this stuff now:

**Turnigy Aerodrive SK3 - 5055-430kv Brushless Outrunner Motor**
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-430kv-brushless-outrunner-motor.html

**ZIPPY Flightmax 5000mAh 4S1P 20C** Two of those. Or some cheaper.
https://hobbyking.com/en_us/zippy-flightmax-5000mah-4s1p-20c.html

And then the rest.... The VESC, I have no clue where to buy...and will it work with this motor?
The remote is not easy either, the Benchwheel seems the best. AliExpress sells these but might take
a month to get it delivered, also the reciever is not included, where can I find that part?

Wheels and motor pulley I will find somewhere, the mount I will try to make myself.
```

---
## \#35 Posted by: mmaner Posted at: 2017-03-02T21:06:34.679Z Reads: 52

```
Regarding the benchwheel remote on the Alibaba site just click the 4th pic, that will get you the remote and receiver. 

Get the VESC from DIY, I have a couple from Dexter with no issues and if the shipping is cheap, win win. 

The Zippy batteries you have linked should be fine.  You will have buy a fairly pricey charger to charge them in series, or you can get 6s batteries and charge with a turnigy accucel or IMAX b6, both are inexpensive.
```

---
## \#36 Posted by: amc Posted at: 2017-03-02T21:48:22.247Z Reads: 51

```
Thanks @mmaner! 

Sorry, cannot find the remote with receiver on AliExpress or Alibaba site. Please can just give me a link?
```

---
## \#37 Posted by: IsTalo Posted at: 2017-03-02T22:00:27.153Z Reads: 51

```
Man, use the "@" when you want talk to us, because if not I can't receive notifications... about the vesc, there all good places, also on AliExpress, I think you could buy at Ebay somethings, they have a lot of Free Shipping things
```

---
## \#38 Posted by: amc Posted at: 2017-03-02T22:01:33.523Z Reads: 50

```
Ok cool @IsTalo  :)
```

---
## \#39 Posted by: IsTalo Posted at: 2017-03-02T22:05:53.984Z Reads: 54

```
First, this motor will blow your Vesc, High Kv, and also, it would work if you use 4s but your speed will be crap... So do what is written in this forum, use a 6s, It's simple, cheap and have enough power, and is easy to find a charger for it. Motor, lower than 250kv, some people says "Lower than 300kv" but it depends on your gear ratio, so 245kv is nice (I think), @mmaner correct if I'm wrong, Don't try to purchase a cheap motor, cheap motor=cheap magnetics, so no way... , any question, ask me and mike
```

---
## \#40 Posted by: mmaner Posted at: 2017-03-02T22:11:08.788Z Reads: 60

```
This is where I got it, but I can't tell which one to get on my phone.  The Alibaba site kinda sucks.  

https://www.aliexpress.com/item/Electric-skateboard-refitting-parts-benchwheel-diy-remote-control-bench-technology/32731985084.html?spm=2114.13010608.0.0.8qEz7i
```

---
## \#41 Posted by: mmaner Posted at: 2017-03-02T22:15:09.237Z Reads: 58

```
@IsTalo You are correct, too high JV and your VESC will be toast.  You can solve that by limiting the ERPM but you will sacrificing speed and torque that way.  

@amc Having used from 190kv to 280kv I prefer a 260kv on 6s single motor boards.  It's fast enough and good torque for a single drive. If you think you will eventually upgrade to dual motors you might think about getting a 190kv motor, 2 of those is pretty damned lush 😀.
```

---
## \#42 Posted by: amc Posted at: 2017-03-02T22:22:44.679Z Reads: 54

```
Great info from both of you!
This will really help a lot. Sorry, to eager to get this running. I will have some more look on this forum. Might have some questions later on though :) 
Thanks guys!
```

---
## \#43 Posted by: mmaner Posted at: 2017-03-02T22:42:16.037Z Reads: 64

```
No worries.  We all get/got excited for our first build.  I have really looked too hard at shipping costs because I buy mostly from DIY, MEB & Amazon.  

If you can buy $300 worth from DIY you can get free shipping.  I think that is free worldwide, but check with @torqueboards to be sure.   

If you buy a single motor mechanical kit, 260kv motor and VESC you should be good.

diy-electric-skateboard-kits-parts/torqueboards-single-motor-mechanical-kit/

diy-electric-skateboard-kits-parts/6355-260kv-epower-motor/

category/electric-skateboard-parts/electric-skateboard-electronic-speed-controller/

After that all you need is a remote, battery(s), deck, enclosure and some wire & other bits.
```

---
## \#44 Posted by: torqueboards Posted at: 2017-03-02T22:47:42.196Z Reads: 58

```
Yeah, it's worldwide free shipping. No 260KV in stock. We'll have 5065 260KV in a few weeks.
```

---
## \#45 Posted by: amc Posted at: 2017-03-03T08:02:06.653Z Reads: 55

```
Thanks!

Found this pulley stuff very cheap. http://www.ebay.com/itm/Electric-Skateboard-Parts-Kit-Pulleys-And-Motor-Mount-For-72-70MM-Wheels-DIY-/332125756292?hash=item4d543cdb84:g:t~IAAOSwB-1YonJp
```

---
## \#46 Posted by: amc Posted at: 2017-03-03T22:29:24.107Z Reads: 50

```
Is this worth it? Or just plain crap? @mmaner 

http://www.ebay.com./itm/322382536122?ssPageName=STRK:MESELX:IT&_trksid=p3984.m1555.l2649
```

---
## \#47 Posted by: mmaner Posted at: 2017-03-03T22:38:01.773Z Reads: 47

```
I don't know, never used them.
```

---
