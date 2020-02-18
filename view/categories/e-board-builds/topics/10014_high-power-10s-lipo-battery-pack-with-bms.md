# High Power 10s Lipo Battery Pack with BMS

### Replies: 725 Views: 56787

## \#1 Posted by: Namasaki Posted at: 2016-09-23T00:42:25.735Z Reads: 2245

```
Looking for more hill climbing power than I could get from my 10s2p with 26650 Lions(it works great on flat ground)
This new project is a 10s1p using Turnigy 2s/5000mah/60c hard packs from Hobby King
5 Packs wired in series is smaller and 2lb lighter than the Lion pack!
<img src="/uploads/db1493/original/3X/1/9/19ebd1deaccdf338b53219f6a7f14d67cda23ed5.PNG" width="281" height="500">
https://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=52279
I used these jst extension wires to extent the balance wires to the bms:
omitting the black ground wire and using only the pos wires from cell 1 and 2 of each pack.
I did this instead of hard wiring to allow for easier testing and replacement of individual cells
http://www.ebay.com/itm/380951841390?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
I attached the packs to the deck with servo tape.
<img src="/uploads/db1493/original/3X/2/9/292469b268f05bf517533e7780cd0aca3c8af775.JPG" width="375" height="500">

Hard wired the packs in series for better power transfer and to reduce bulk.
Using adhesive lined shrink tube and squeezed the ends to close it up.
<img src="/uploads/db1493/original/3X/5/2/520113e16df1f607430e5e3051c3f6ad8a02837f.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/3/5/352c0535d72d42cac9ff6d2306a13693873af626.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/5/f/5f9a3f78286fe859bba959057812bfa92eb2b8c4.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/9/9/99288fb539de97a46f6eec3f5cc1b7c4c6a9cf24.JPG" width="666" height="500">

I decided to keep the balance lead connectors for easier testing and replacement of individual packs.
<img src="/uploads/db1493/original/3X/7/8/78fd8ecb46966cf1cbd22c92f13d298e61a60411.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/9/8/98ca18f83f65a8adb244a09c96d93c82703639e7.JPG" width="375" height="500">

Completed:
<img src="/uploads/db1493/original/3X/e/c/eca7c7147086236632aa737d78b0fb57beb03bf8.JPG" width="375" height="500">

I took it for a quick test ride with only 38v on the pack. Powering up a 12% grade the voltage sag was no more than 1 volt.
More test results to follow...
```

---
## \#2 Posted by: hamminitup Posted at: 2016-09-23T00:57:56.494Z Reads: 1821

```
Very interesting build. This is the first lipo with BMS I've seen. Just curious, how are you going to go about charging? Will there be a power switch?
```

---
## \#3 Posted by: Namasaki Posted at: 2016-09-23T01:34:18.497Z Reads: 1804

```
 The BMS has a built-in power switch. 
I'm charging through the BMS with a 42v laptop style charger.
```

---
## \#4 Posted by: hamminitup Posted at: 2016-09-23T02:18:21.657Z Reads: 1765

```
Ah ok thanks. Do you mind linking where you got the BMS?
```

---
## \#5 Posted by: maxz Posted at: 2016-09-23T02:24:00.182Z Reads: 1734

```
This is exactly what i was thinking about doing, those 2s lipos are thin, are you using a bestech bms??
```

---
## \#6 Posted by: Namasaki Posted at: 2016-09-23T02:28:28.932Z Reads: 1695

```
Yes, bestech 80a 10s bms
```

---
## \#7 Posted by: Namasaki Posted at: 2016-09-23T02:29:07.580Z Reads: 1644

```
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#8 Posted by: maxz Posted at: 2016-09-23T02:29:41.919Z Reads: 1625

```
hmmm that would be the only thing that would kill the price for me, i was thinking about a cheaper bms just for charging
```

---
## \#9 Posted by: Namasaki Posted at: 2016-09-23T03:07:58.227Z Reads: 1564

```
These are very reasonably priced. Only around $60
Or you could use a less expensive charge only bms. Just be careful, some cheap bms's are unreliable.
```

---
## \#10 Posted by: maxz Posted at: 2016-09-23T03:10:05.513Z Reads: 1514

```
just need to buy 2 of them is the only problem and then sent to New Zealand which i would get cause they have a switch built in but finding another buyer for one with NZ shipping fees might be hard.
```

---
## \#11 Posted by: Namasaki Posted at: 2016-09-23T03:13:09.789Z Reads: 1466

```
Just charged the battery to 100% and when for a test ride through the hills.
4.5 miles and the battery only dropped to 84%!
Think I'm gonna get more than the 10mi I was hoping for.
```

---
## \#12 Posted by: michaeld33 Posted at: 2016-09-23T03:18:10.704Z Reads: 1413

```
Wait sorry if I misunderstood, but the lipos are 10S 5000mah? And they're in series? Wouldn't that mean they are 50S 5000mah? I obviously don't think that's what you are trying to do so I just kinda assumed it's 10S 25a?
```

---
## \#13 Posted by: Namasaki Posted at: 2016-09-23T03:49:30.575Z Reads: 1396

```
There are 5 packs in series. Each pack is a 2s/5000mah/60c
So its a 10s1p 5ah 300a discharge.
You may ask, Why in the world would anyone need a battery with 300a discharge?
Point is, very little or no voltage sag when accelerating or climbing hills.
When voltage sag is greatly reduced, You can take the pack lower without tripping the low voltage protection.
And less capacity is needed.

**UPDATE**
The true discharge capability of this battery is more like 90a, NOT 300a.
```

---
## \#14 Posted by: Lukaszlisc Posted at: 2016-09-23T06:59:29.577Z Reads: 1367

```
If you conecting battery in series the discharge is  counting same as Ah? Only voltage doubles.
5x 2s 5000mah 60c in series = 10s 5000mah 60c?
Max amps at 10s (36v) :
60c x 5000mah ÷1000= 300a
Or in paralles capacity and discharge doubles?
5x 2s 5000mah 60c in parallel= 2s 250mah 300c?
Max amps at 2s (7.4v) :
300c x 5000mah ÷1000= 1500a
Am I wrong?
```

---
## \#15 Posted by: Namasaki Posted at: 2016-09-23T12:00:55.378Z Reads: 1332

```
In parallel it would be
7.4v
Voltage would be too low for eskate. 
The C rating doesn't change. 
Only voltage or capacity changes.
```

---
## \#16 Posted by: Namasaki Posted at: 2016-09-23T15:28:35.438Z Reads: 1323

```
You could connect 6 packs in series and parallel 
To make a 6s2p
22v 10ah 60c
```

---
## \#17 Posted by: Namasaki Posted at: 2016-09-23T19:56:26.548Z Reads: 1326

```
Some right some wrong. 
The C rating never changes. 
Series = multiply voltage
Parallel = multiply capacity 
Five 2s/5ah/60c in series =10s/5ah/60c
Five 2s/5ah/60c in parallel =2s/25ah/60c
```

---
## \#18 Posted by: ewalks6 Posted at: 2016-12-10T18:23:17.943Z Reads: 1273

```
Hey, really cool build. Very inspired and wantt to do something similar. Is it possible that you could make a diagram of what you did? I recently joined the community and have been reading a lot to figure out how the BMS works and what not but can't quite understand how you set this up. (I understand the series connections but not the BMS part)
```

---
## \#19 Posted by: pigeonic Posted at: 2016-12-10T18:33:26.146Z Reads: 1267

```
I'm with you on this one. wanting to buy Turnigy 5000mah 2s 20c, but no idea (at least, its 3am where I live my brain might be fried) how to increase cap with those batt packs and increase its voltage?
```

---
## \#20 Posted by: Namasaki Posted at: 2016-12-10T18:38:57.277Z Reads: 1243

```
I'm at work now but soon I will give you more info on the balance wiring as soon as I can.
```

---
## \#21 Posted by: Namasaki Posted at: 2016-12-10T18:40:35.959Z Reads: 1174

```
I highly recommend you get the 60C packs, not 20C. 
With 20c you will have less range because of increased voltage sag.
```

---
## \#22 Posted by: pigeonic Posted at: 2016-12-10T18:44:54.525Z Reads: 1176

```
Found the 60C packs x5, how do you reckon I can increase the cap all while increasing voltage, and sag
```

---
## \#23 Posted by: ewalks6 Posted at: 2016-12-10T20:11:27.076Z Reads: 1201

```
Yeah sounds good. Thanks for the help!
```

---
## \#24 Posted by: Namasaki Posted at: 2016-12-12T03:39:16.323Z Reads: 1225

```
<img src="/uploads/db1493/original/3X/c/9/c915ce9afcad8d0612f358c16462fbff38631258.png" width="665" height="500">
The blue blocks are quick disconnects which makes for easier setup and maintenance.
```

---
## \#25 Posted by: Namasaki Posted at: 2016-12-12T04:04:41.396Z Reads: 1171

```
I used the 2s 5000 60c because they offer high current capability 
while having a very compact footprint.
If space is not an issue, you could use Zippy flight max 8000 30c
I haven't had time to do a full on range test with this setup yet but I have logged about 13 miles without using up a full charge.
```

---
## \#27 Posted by: ewalks6 Posted at: 2016-12-16T15:10:34.180Z Reads: 1134

```
Thanks for the help, great diagram. Two questions- 

1. Does the charge port come with the BMS? I've never used anything like this.

2. Where did you get the E Switch?

Thanks for everything.
```

---
## \#28 Posted by: ewalks6 Posted at: 2016-12-16T15:12:49.071Z Reads: 1098

```
Oh and what are you using for an enclosure? Sorry for all the questions.
```

---
## \#29 Posted by: Namasaki Posted at: 2016-12-16T15:19:35.127Z Reads: 1065

```
Charge port is not included
The E-switch is built in on Bestech BMS
Just add an automotive switch to control it
I'm using psychotiler enclosures
```

---
## \#30 Posted by: brakkeh Posted at: 2016-12-16T18:45:15.411Z Reads: 1074

```
Hey man, 

I don't know how to send a private message so i'm just gonna ask my question here, okay? 

I regularly see people with motors that can pull a max om 80A.
Online once read that the max ampere output of a battery is Ah * C 
So for a lot of people i've seen its 5 * 30 = 150A

What am i missing? 

Thanks, Bram
```

---
## \#31 Posted by: Namasaki Posted at: 2016-12-16T18:55:19.762Z Reads: 1054

```
I answered your question here:
http://www.electric-skateboard.builders/t/killshot-clone-190kv-single-10mah-headlights-usb-charging-volt-meter/13201/8
```

---
## \#32 Posted by: nmagz3 Posted at: 2017-01-20T06:40:17.289Z Reads: 1016

```
I know this is an older post but there is such a wealth of info! Thanks for taking this project on and sharing it with us.  I have (2) 5S 5000 mah Lipos in series and it's such a bitch to charge which I do seperstely for each lipo.  I don't really understand the logistics of a BMS but understand what it does generically.  After more research to come would you mind if I DM you when I feel confident to start the project?  Again, great work here!
```

---
## \#33 Posted by: Namasaki Posted at: 2017-01-20T07:26:27.975Z Reads: 1009

```
Happy to help and answer any questions you might have. 
I have been using this setup for a while now and I am very happy with it. 
I am currently building a second board with the same setup on a different deck and different motor mounts.
```

---
## \#34 Posted by: nmagz3 Posted at: 2017-01-21T09:42:19.905Z Reads: 984

```
I'd like to see how the motors change the ride with the same set up.  Appreciate the help in advice sir :grin:
```

---
## \#35 Posted by: Namasaki Posted at: 2017-01-22T00:31:34.063Z Reads: 986

```
The KV specs of the motor or motors is dictated by the the Vesc and the voltage. 
You want to keep the Erpm at 60k or less. 
60k/7pole pairs =  8571 RPM
When calculating, use full charge voltage, not nominal voltage. 
Example:
10s = 42volts 8571 rpm / 42volts = 204 max motor KV

I've found that 10s and 190kv makes for a very dependable setup with a good balance of torque and speed.
```

---
## \#36 Posted by: mmaner Posted at: 2017-01-22T01:06:03.474Z Reads: 981

```
[quote="Namasaki, post:35, topic:10014"]
10s = 42volts8571 rpm / 42volts = 204 max motor KV
[/quote]

I've never seen that calculation, I don't know how.  You just saved me a shit ton of trouble.  Thanks mate.
```

---
## \#37 Posted by: mmaner Posted at: 2017-01-22T19:10:35.104Z Reads: 971

```
@Namasaki > 60k/7pole pairs = 8571 RPM
How do you know how many poles a motor has?  Specifically I am curious if a [TB 6355 260kv](diy-electric-skateboard-kits-parts/6355-260kv-epower-motor/) is to high of a KV to use on 10s3p.  And if x2 [TB 6355 260kv](diy-electric-skateboard-kits-parts/6355-260kv-epower-motor/) is too high KV to use n 10s3p. 

The reason I am so confused is that my kids board has a x2 5055 280KV motors and 10s3p.

Thanks for the expertise :slight_smile:
```

---
## \#38 Posted by: Namasaki Posted at: 2017-01-22T21:24:52.551Z Reads: 976

```
260kv with 10s is over the limit when using a Vesc. 
7 pole pairs or 14 poles is common for the motors we use including TB's motors. (Although, I'm speaking of 60mm motors and I don't know about 55mm motors.) You may be able overcome this limitation by setting the erpm limit in the bldc tool to 60k. 
And as long as your not going full out at full throttle, you may be ok. 
Is your kids board setup with Vescs?
If yes, then maybe they aren't riding fast enough to exceed the limit.
@chaka may be able to address this question better seeing that he is the expert on this topic and all I know is what I've read in his posts.
```

---
## \#39 Posted by: nmagz3 Posted at: 2017-01-23T01:27:58.321Z Reads: 957

```
Hey there!  I can't stop looking at this diagram and your pictures!  I have (2) 5S 5000 mah Lipos.  If I was to keep my balance leads for the same reason (testing) would you recommend I get a balance lead to connect from the Lipo balance and then take the individual wires (minus the ground) from both Lipos into the BMS?  In my head this is starting to make sense but in practice I feel like their would be some fires :fearful: in my case.  Thanks in advance.
```

---
## \#40 Posted by: nmagz3 Posted at: 2017-01-23T01:41:13.491Z Reads: 951

```
Got another one for ya if you don't mind!  What kind and where did you get the charging port?  Man, this is becoming more and more fisable in my head.  2 months ago I'd never imagine I could even solder let alone understand your post!  Thanks again :sunglasses:
```

---
## \#41 Posted by: Namasaki Posted at: 2017-01-23T05:24:54.788Z Reads: 993

```
http://www.ebay.com/itm/262359346829?_trksid=p2060353.m1438.l2649&ssPageName=STRK%3AMEBIDX%3AIT
The switch is useless but the charge port works fine.
This charge port is the small version and fits the cheaper 42v chargers that are sold on eBay
http://www.ebay.com/itm/222029867724?_trksid=p2060353.m1438.l2649&ssPageName=STRK%3AMEBIDX%3AIT

I used these extensions to connect the balance wires to the bms:
http://www.ebay.com/itm/NEW-12-JST-2S-LIPO-BALANCE-LEAD-EXTENSION-SILICONE-22awg-WIRE-ADAPTER-US-SELLER-/380951841390?hash=item58b27fca6e
They're  really nice because I can quickly disconnect each battery pack from the BMS balance circuit for individual testing, charging or replacement if necessary, although I hard soldered each packs main wires for minimum resistance.
```

---
## \#42 Posted by: nmagz3 Posted at: 2017-01-23T05:43:41.201Z Reads: 927

```
Beautiful and well thought out!  It's like the matrix, I'm starting to see the code!  Thank you bro!
```

---
## \#43 Posted by: Namasaki Posted at: 2017-01-24T22:15:10.341Z Reads: 939

```
[quote="mmaner, post:37, topic:10014"]
How do you know how many poles a motor has?
[/quote]

Open the motor and count the magnets in the shell.
This motor has 14 magnets (poles) or 7 pole pairs
multiply voltage x KV rating to get RPM
multiply pole pairs x RPM to get ERPM
<img src="/uploads/db1493/original/3X/6/c/6c97a33f834585183ff674de5a5d85316654c722.jpeg" width="375" height="500">
```

---
## \#44 Posted by: mmaner Posted at: 2017-01-24T22:20:01.347Z Reads: 886

```
Good info, thank you sir.  I am slowy getting my head around all of this :slight_smile:.
```

---
## \#45 Posted by: Namasaki Posted at: 2017-01-24T22:31:59.159Z Reads: 894

```
Your very welcome, 
About the TB 260kv motors, I used to run those. They are good motors with a good torque and speed.
Their shafts are long enough to accommodate the wider pulleys and belts. They also are well made and come with quality NSK bearings.
I ran them at 12s with Hobby ESC's on 90mm wheels and got 28mph going uphill.(just a slight grade)
When I upgraded to Vesc's I switched to 190kv motors and 10s because I was afraid of causing DRV fault in the Vesc.
But, I think that you could possibly run them at 10s with the Vesc if you turn the max erpm limit down from 100k to 60k in the bldc tool. 
This is only speculation by me for I have not tried it and I am by no means an expert concerning the Vesc.
```

---
## \#46 Posted by: mmaner Posted at: 2017-01-24T22:42:17.469Z Reads: 909

```
[quote="Namasaki, post:45, topic:10014"]
I think that you could possibly run them at 10s with the Vesc if you turn the max erpm limit down from 100k to 60k in the bldc tool
[/quote]

Mine is allready at 60k MAX ERPM, I thought that was the most it should be because of DRV issue?
<img src="/uploads/db1493/original/3X/4/7/47adf97eadd2a27a1e36830ee590f8ab5dd37b7f.jpg" width="529" height="168">

I am running a 6355 190kv right now until my replacement gets here, if I raise it to100k will I get better performance?  It's slllloooooowwwwwww right now :slight_smile:.

Ideally, I would like to run dual 6355's, but I am still waiting on my 10s pack and DIY is out of stock on VESC's for a couple of weeks and I need to get another motor, so Ill probably go with 190kv at that point.
```

---
## \#47 Posted by: Namasaki Posted at: 2017-01-24T22:46:13.755Z Reads: 873

```
I don't think upping the erpm limit will help performance. However, your other settings will. Post screen shots of your other settings in bldc tool and lets have a look.
Also are you running 10s voltage?
```

---
## \#48 Posted by: mmaner Posted at: 2017-01-24T22:50:27.199Z Reads: 916

```
<img src="/uploads/db1493/original/3X/3/a/3ab45f880e89b41fc7281c7818f1d6d3ebfc52f0.JPG" width="690" height="391">
<img src="/uploads/db1493/original/3X/e/0/e01965ecdcd575cfabb89bee466e4b818d6c7328.JPG" width="690" height="390">
<img src="/uploads/db1493/original/3X/5/d/5df723952245a81c222e8f77d0d22d3dfa75d832.JPG" width="690" height="389">
<img src="/uploads/db1493/original/3X/c/0/c054dc75f65ba5414531feca1722646990d4954b.JPG" width="690" height="391">

I am currently running 6s (x2 zippy 8000mah 30c Lipo packs), but I am going to 10s when my new pack gets here.

I am really confused by the math regarding the VESC and Motor KV values, mostly because I'm missing so much of the math for a full understanding.  So if I have this right...

8600 / MAX Voltage = MAX KV
then
8600 / 42.0v (10s) = 204kv
so 204kv would be a theoretical maximum that can be used on the VESC.  But that is dependent on the MAX ERPM limit being at 100k?
```

---
## \#49 Posted by: Namasaki Posted at: 2017-01-24T23:02:20.515Z Reads: 798

```
motor kv means rpm per volt.
So, 200kv means 200 rpm per volt.
So, 200kv x 42v = 8400 rpm
or, 190kv x 42v = 7980 rpm
The max safe erpm for the vesc is 60k
8400 rpm x 7 pole pairs = 58800 erpm
You could safely run 200kv motor at 10s without having to worry about erpm limit.
```

---
## \#50 Posted by: Namasaki Posted at: 2017-01-24T23:07:11.152Z Reads: 834

```
6s voltage is minimum for e-skate and is probably the reason for the lack luster performance.
especially acceleration. Upping the voltage to 10s will make a big difference.
Your motor max (60a) and batt max (60) are plenty high enough.
The only thing, you might try switching from watt control to current control in the PPM settings.
I don't know if you've tried that but it may make a difference.
I run in current mode myself.






<img src="/uploads/db1493/original/3X/b/8/b861b0bcc043f80bee9f403d7c62d214507bdcbb.jpg" width="690" height="391">
```

---
## \#51 Posted by: Namasaki Posted at: 2017-01-24T23:17:26.063Z Reads: 785

```
More on voltage,
I have run 6s, 10s and 12s.
Even the difference between 10s and 12s is very noticeable concerning acceleration.
10s is smooth and manageable.
12s is very snappy and requires much more caution when squeezing the trigger.
6s is the most controllable and is good for crowded sidewalks like the boardwalk at the beach where speed and acceleration is not needed.
```

---
## \#52 Posted by: mmaner Posted at: 2017-01-24T23:17:29.721Z Reads: 777

```
What setting would I change and how to define the value for that setting if I wanted to run 260kv motor or motors at 10s?  Or is that even possible?  Is there a method of including the ERPM limit into the formula **KV * MAX Voltage * 7 = ERPM**?

I have always run 6s up to this point but my range is not great, that's why I wanted to go to 10s on my everyday board.  Eventually I want to run dual motors, but I have some product to buy first.
```

---
## \#53 Posted by: Namasaki Posted at: 2017-01-24T23:20:12.474Z Reads: 765

```
[quote="mmaner, post:52, topic:10014"]
KV * MAX Voltage * 7 = ERPM?
[/quote]

Thats the formula.
KV x V x 7=ERPM
Provided the motor has 14 poles. 
There are some hub motors that have more.
```

---
## \#54 Posted by: Namasaki Posted at: 2017-01-24T23:20:54.041Z Reads: 727

```
have you ever tried running in current control mode?
```

---
## \#55 Posted by: Namasaki Posted at: 2017-01-24T23:23:26.059Z Reads: 742

```
[quote="mmaner, post:52, topic:10014"]
What setting would I change and how to define the value for that setting if I wanted to run 260kv motor or motors at 10s?  Or is that even possible?
[/quote]

I think it is possible but I am not sure. the setting is on the first page and you already have it set at 60k.
Chaka is an expert on the vesc and could probably give a better answer.
```

---
## \#56 Posted by: mmaner Posted at: 2017-01-24T23:25:02.986Z Reads: 770

```
[quote="Namasaki, post:45, topic:10014"]
But, I think that you could possibly run them at 10s with the Vesc if you turn the max erpm limit down from 100k to 60k in the bldc tool.
[/quote]

When I asked about including the ERPM limi, what I meant was how do what is the math to define the ERPM limit for a motor with a higher KV than is supported.  I don't even know if its possible, I'm just trying to figure out if it is.

@chaka, do you have any info that could shed some light on the problem of  how to define the ERPM limit for a motor with a higher KV than is supported?

[quote="Namasaki, post:54, topic:10014, full:true"]
have you ever tried running in current control mode?
[/quote]

I originally ran Current Control Mode until @Ackmaniac released hiw Watt Control Mode. I found I got better performance with WCM on 6s.
```

---
## \#57 Posted by: Namasaki Posted at: 2017-01-24T23:36:35.783Z Reads: 723

```
the motor doesn't have an erpm limit. only the vesc has the erpm limit.
the max erpm that a motor will produce is determined by KV x V x pole pairs
```

---
## \#58 Posted by: mmaner Posted at: 2017-01-24T23:53:03.336Z Reads: 769

```
[quote="Namasaki, post:57, topic:10014"]
the motor doesn't have an erpm limit
[/quote]

I get that.  I was referring to when you said...
[quote="Namasaki, post:45, topic:10014"]
But, I think that you could possibly run them at 10s with the Vesc if you turn the max erpm limit down from 100k to 60k in the bldc tool.
[/quote]

When we were talking about 260kv on 10s.

I am trying to figure out if its possible to run the 260kv motors on 10s by adjusting the ERPM limit.  IF so, whats the math to define what the ERPM limit should be?  If that is possible.

Sorry if Im not being clear, it may not be the ERPM limit that is critical but that's the limit that I am trying to avoid passing so as to not burn up the DRV on the VESC.
```

---
## \#59 Posted by: Namasaki Posted at: 2017-01-25T00:05:29.319Z Reads: 735

```
the erpm limit should be 60k because thats what the vesc can handle.
theres no way to adjust the erpm of the motor except by lowering or raising the voltage supply.
the KV of the motor is set and can't be changed unless you re-wind the motor.
What I was suggesting is that setting the erpm limit in the vesc via the bldc tool to 60k which you have already done might be enough to keep the 260kv motor with 10s voltage from overloading the DRV chip. But I am not sure about this. I haven't tried it so it's only speculation on my part.
I would ask someone like Chaka about this before trying it.
```

---
## \#60 Posted by: mmaner Posted at: 2017-01-25T00:56:34.609Z Reads: 718

```
Cool thanks for letting me bug the crap out of you 😀
```

---
## \#61 Posted by: Namasaki Posted at: 2017-01-25T01:12:14.872Z Reads: 721

```
no problem, I enjoy taking about this stuff
```

---
## \#62 Posted by: miles Posted at: 2017-01-28T21:05:16.581Z Reads: 671

```
Where did you buy your bestech bms? I can't find anywhere to actually purchase online. Their website just has all the info/specs.
```

---
## \#63 Posted by: Namasaki Posted at: 2017-01-28T23:50:06.361Z Reads: 679

```
You email the sales department with your request and they assign a sales rep to work with you and process your order
```

---
## \#64 Posted by: miles Posted at: 2017-01-30T07:32:52.462Z Reads: 685

```
👍 thanks man.
```

---
## \#65 Posted by: Namasaki Posted at: 2017-01-30T12:14:55.526Z Reads: 698

```
For more info look here:
http://www.electric-skateboard.builders/t/first-time-build-never-going-to-start-if-i-dont-post-this/16474/43
```

---
## \#66 Posted by: ewalks6 Posted at: 2017-02-05T01:42:28.504Z Reads: 681

```
Hey,

Just had a quick question. I know battery max output is C * mAh. I ordered the BMS that you suggested and was going to order the batteries you used but then saw a sale for 2S2P 30C 5000mAh batteries. Therefore this means its 10000mAh (I think). Will this affect the BMS I bought at all?
```

---
## \#67 Posted by: i2oadsweepei2 Posted at: 2017-02-05T01:49:33.353Z Reads: 669

```
Those batteries are each made up of two sets of two cells in parallel then together in series for 2s. The output is still the same 2s 5000mah.
```

---
## \#68 Posted by: ewalks6 Posted at: 2017-02-05T02:29:35.339Z Reads: 669

```
Ok. So what's the point of having 2S2P then? (In this situation).
```

---
## \#69 Posted by: Namasaki Posted at: 2017-02-05T04:53:12.304Z Reads: 697

```
I recommend using 2s1p Lipos. that way you are balancing every cell individually.
With a 2s2p Lipo, you would be balancing 2 cell groups as 1cell.
The 2s2p Lipo is made of 4 2500mah cells in parallel and in series. (personally, I would not recommend these for any application)
$125 for 5 2s1p 5000/60-120c packs might seem a little pricey but you get what you pay for. They are high quality packs with low internal resistance. Because of this and their high amp capability, they will be less prone to overheating like some cheaper lipos.
To answer your question, higher mah would not affect the bms as long as you wind up with 10s voltage
```

---
## \#70 Posted by: i2oadsweepei2 Posted at: 2017-02-05T20:54:24.916Z Reads: 688

```
Couldn't have said it any better than Namasaki. This thread is an inspiration for me on a future build.
```

---
## \#71 Posted by: Namasaki Posted at: 2017-02-09T02:27:54.006Z Reads: 824

```
[quote="nmagz3, post:39, topic:10014"]
Hey there!  I can't stop looking at this diagram and your pictures!  I have (2) 5S 5000 mah Lipos.  If I was to keep my balance leads for the same reason (testing) would you recommend I get a balance lead to connect from the Lipo balance and then take the individual wires (minus the ground) from both Lipos into the BMS?  In my head this is starting to make sense but in practice I feel like their would be some fires :fearful: in my case.  Thanks in advance.
[/quote]

This setup will work with five 2s lipos or two 5s Lipos. It's basically the same thing though because you have more balance wires coming for each pack, you need to be all the more careful and find out using a volt meter which cell each of the colored balance wires goes to. Red is always the last cell in each pack. The black balance wire is ground and is not needed with the Bestech BMS. As you can see by the diagram, The pack that supplies the Black power wire to the system is pack 1 Cells 1,2,3,4,5 and the pack that supplies the Red power wire is pack 2 Cells 6,7,8,9,10
Just connect everything correctly and double check it before turning the power on and it will be fine.
```

---
## \#72 Posted by: Namasaki Posted at: 2017-02-27T04:52:10.777Z Reads: 816

```
I have updated my BMS wiring diagram to match the pad and pin locations on the actually BMS.

<img src="/uploads/db1493/original/3X/3/c/3c270d2dac8353fae7063a170cd368936c6170af.png" width="664" height="500">
```

---
## \#73 Posted by: mptrs Posted at: 2017-03-06T22:38:56.580Z Reads: 782

```
Thanks for all the schematics, I learned allot! I ordered the same BMS but I have an anti spark as well. Now I read somewhere that isn't needed with this BMS cause you it has an e-switch. But I'd rather use my anti spark, just to be save. What do I do with the e switch wires?

Drawn up a wiring scheme, hope you can help out what to do with the e switch wires and if everything is in the correct place.

Might want to add some leds as well, what's the best place to connect those?

<img src="/uploads/db1493/original/3X/8/4/843bf67f3402b0177033b1aee4d61b3a8e980f63.JPG" width="375" height="500">

_(the anti spark got a switch, but forgot to draw it)_
```

---
## \#74 Posted by: Namasaki Posted at: 2017-03-06T22:53:45.630Z Reads: 722

```
The built in E-switch has to be on during discharge and charge as well. 
The E- switch is also needed to reset the BMS in the event that one of its protection circuits is activated and shuts the system down. 
There is no easy way to bypass using the built in switch. 
You can use an anti spark switch in addition if you want, you'll have to have 2 switches then. 
I really wouldn't recomend it. Because adding the anti spark switch means more connections which means more resistance across the system and those external anti spark switches are prone to failure and could leave you stranded. 
The built in E-switch eliminates the spark issue anyway and it has been very reliable for me since last summer when I started using it.
```

---
## \#75 Posted by: Namasaki Posted at: 2017-03-06T23:07:30.363Z Reads: 704

```
I would also recommend getting a couple 5s extension cables, plug those into your batteries, cut the plug off the other end of the extension and wire that to your BMS balance cables. 
Then you can quickly disconnect your batteries from the BMS for inspection and maintenance. 
Keep your hobby balance charger for maintenance in case you ever need to replace a pack because you'll  need to manually balance it with the existing pack.
The BMS will keep your packs in balance during charge and discharge cycles but they need to be balanced manually at first because the BMS won't be able to balance them if they are too far out of balance.
```

---
## \#76 Posted by: Namasaki Posted at: 2017-03-06T23:17:08.370Z Reads: 709

```
One more thing. 
When using five 2s packs, the balance wiring is very simple but when using two 5s packs, it can be easy to make a mistake with the balance wires and their correct order. If you get it wrong, you will fry the BMS. So use a voltage meter to determine which cell each wire comes from and double check to make sure it's wired correctly before connecting the main power wires from the battery and powering up the system.
```

---
## \#77 Posted by: mptrs Posted at: 2017-03-06T23:21:11.131Z Reads: 735

```
Aha, can I attach a led switch to the eswitch?
<img src="/uploads/db1493/original/3X/b/9/b99145194dee70e262b1dba6f710016366551886.JPG" width="375" height="500">

Thanks for the extension cable tip. I was hoping for the BMS to do all the dirty work, but some manual won't be too bad.

Any recommendations on the charger or any 42v 5a from aliexpress will do?

And sorry for being such a noob, but how can I check if the balance wires are correct? What makes them correct?


Thanks for all the help, don't want to blow up my BMS (:
```

---
## \#78 Posted by: mptrs Posted at: 2017-03-06T23:26:10.489Z Reads: 719

```
Ok found the order per lipo, is there any order for the bms? OR just keep  12345, 12345

<img src="/uploads/db1493/original/3X/0/4/04a7ad27de6b34c5c46477b0eff6f8ed5116962d.png" width="690" height="398">
```

---
## \#79 Posted by: mptrs Posted at: 2017-03-06T23:29:57.559Z Reads: 705

```
Found this: https://endless-sphere.com/forums/viewtopic.php?f=14&t=52240
So that'll help out!
```

---
## \#80 Posted by: Namasaki Posted at: 2017-03-07T00:27:34.295Z Reads: 737

```
No need to apologize for being a noob.  All of us where noobs starting out.
that's a really nice JST-XH chart. It looks correct but I would still double check my balance wires with a voltage meter.
This BMS does not use the Black ground balance wire from the Lipos as illustrated in my diagram.
The BMS balance jack is numbered on the bottom side of the PCB.
My updated diagram show the bms layout as it is on the real thing.
<img src="/uploads/db1493/original/3X/6/5/65de89abc4d6aa7673bf6e371dd23c1c4f9f7f1c.png" width="690" height="387">
<img src="/uploads/db1493/original/3X/2/c/2cd3a915585b219413390c8da90e711b94862b33.png" width="690" height="387">
There is one more important point that I almost forgot to mention:
These modules are static sensitive so you need to have some type of static protection before you open the bag and remove them.
I use these wireless wrist bands. They seem to work well. They absorb any static charge that is on your body.
http://www.frys.com/product/6932377?site=sr:SEARCH:MAIN_RSLT_PG
```

---
## \#81 Posted by: Xaeron Posted at: 2017-03-07T00:33:22.850Z Reads: 712

```
I have a lot of experience with RC cars but I am new to eskate. After reading a lot I have the feeling that 10s 5000mah lipo performs as good as 10s3p liion and almost like 10s4p.

That shouldn't be that way because 10s4p with Samsung 25NR is twice the mah but in practice this looks true... Anyone else have the same impression???
```

---
## \#82 Posted by: Namasaki Posted at: 2017-03-07T00:42:30.775Z Reads: 699

```
[quote="mptrs, post:77, topic:10014"]
Any recommendations on the charger or any 42v 5a from aliexpress will do?
[/quote]

Those are pretty good, I have one similar that I got from Battery Supports. It charges the pack fairly quick but cant quite charge the pack fully to 42v. It does get the pack up to 41.8 or 41.9 before getting the green light.
The only other option is to use an Adjustable CC/CV  lab power supply. Which is what I use.
I like to get my pack fully charged for maximum performance and range and I am less concerned about their longevity.
```

---
## \#83 Posted by: Namasaki Posted at: 2017-03-07T00:58:40.101Z Reads: 699

```
[quote="Xaeron, post:81, topic:10014, full:true"]
I have a lot of experience with RC cars but I am new to eskate. After reading a lot I have the feeling that 10s 5000mah lipo performs as good as 10s3p liion and almost like 10s4p.

That shouldn't be that way because 10s4p with Samsung 25NR is twice the mah but in practice this looks true... Anyone else have the same impression???
[/quote]

Well, If you buy quality Lipos with high C rating then Li-ions can not compare is performance per pound.
Example:
My packs are 10s 5000mah 60/120c  Thats a rating of  300a continuous and 600a peak
A li-ion 10s3p is only 60a continuous  a 10s4p is only 80a continous
So, some may ask why would you need a 300a battery?
The answer is VOLTAGE SAG.
With a 300a battery, there minimum voltage sag under demanding conditions.
With a 60-80a battery you will see much more sag under the same conditions.
On top of that, the 300a Lipo pack is smaller and lighter than the 80a Li-ion pack.
Some feel that Lipos are too hazardous and I for one have said as much.
But recently I am finding that Li-ion cells can be just as hazardous.
```

---
## \#84 Posted by: Namasaki Posted at: 2017-03-07T01:03:19.276Z Reads: 695

```
[quote="mptrs, post:77, topic:10014"]
Aha, can I attach a led switch to the eswitch?
[/quote]

Yes you can but the bms will not power the light. 
You will need a volt/ohm meter to test continuity and find the 2 poles that connect when the button is on and connect the E-switch wires to those 2 poles.
then find the 2 poles that energize the light when the switch is on and connect those to pos and neg 5v source.
I used an open channel on my receiver to power the light on my switch. It is ultimately powered by the 5v coming for the Vesc.
```

---
## \#85 Posted by: PXSS Posted at: 2017-03-07T01:35:42.720Z Reads: 704

```
Adding to @Namasaki here,
Performance is relative.
Are you measuring performance with range, power output, efficiency, or something else???

If we talk about range, the 10S4P is better as you have more energy. 360Wh vs 185Wh in the LiPo
If we talk about power output, the 10S 5000mAh LiPo is better as they are designed to run at high power conditions, you'll see this in the power ratings. (18650 cells rated between 1.5C-10C, while LiPos are rated between 25C-120C)
The LiPo is smaller (8.4% smaller in volume) and lighter (17.2% in weight), but that is only because it has about half the energy than the 10S4P pack. If you compare two packs with identical energy the LiPo will be much heavier and bigger.

25R cells are pretty terrible cells in my opinion, the only good thing about them is that they're cheap and really they're not that cheap...

I suggest you use 30Q cells.

* They have 3000mAh which means a 10S4P pack will have 432Wh, which is 20% more than the 25R and 134% more than LiPo.
* They have much lower voltage sag than 25Rs which means you can push your board as much as you want without it cutting out on you.
* Can be found under $4 per cell.
```

---
## \#86 Posted by: CaptainMerricka Posted at: 2017-03-07T02:03:16.072Z Reads: 642

```
I am running the same battery pack but a single 6374 and a vedder e-switch+ big hobby charger.  I am wondering what kind of range you are getting on a charge, and how long it takes the BMS to charge from empty to full? Is it charging at like 2A?
```

---
## \#87 Posted by: Namasaki Posted at: 2017-03-07T02:18:50.647Z Reads: 662

```
When I said performance I am referring to power and the ability to deliver high current without excessive voltage sag.
I refer to range as range not as performance.
So, theoretically, a 10s4p li-ion pack will have more range especially with 30q cells capable of 30a per cell.
I did recently built a Li-ion pack using 26650 cells that 4500mah and capable of 30a per cell.
My pack was a 10s2p so 9000mah or 324WH vs my 185wh Lipo pack.
The Lipo pack is smaller and 1 pound lighter than the Li-ion pack.
In demanding conditions with lots of hills, the range of the Li-ion pack was the same or less that the Lipo pack because voltage sag robbed the Li-ion pack of its range.
Granted, on flat ground at moderate speeds the Li-ion pack had much more range. Unfortunately for me, most of my riding is up and down hills.
```

---
## \#88 Posted by: Namasaki Posted at: 2017-03-07T02:21:23.254Z Reads: 618

```
I'm using a 5a charge so it's pretty fast. Bout the same as a hobby charger.
```

---
## \#89 Posted by: PXSS Posted at: 2017-03-07T02:45:19.598Z Reads: 651

```
Performance can be measured based on need. I won't argue how you decide to measure it.

A 30Q 10S4P pack can deliver 1680W of power throughout 91% of it's capacity and 2000W through 83% of it's capacity. I'm using 2.8V as the cutoff when they can really go down to 2.5V. 
The 25Rs on the other hand can only do this for about 50% of their capacity.
So I believe that a 25R pack in a high power environment only had as much range as your LiPo Pack (this is why I think they are crap), the 30Q pack on the other hand would still have twice as much range if you constantly ran it at these power conditions.

My 10S4P pack weighs 4.375lbs including all wires and connectors, according to the link in your first post 5 of your cells weigh 3.46lbs, so lets assume 3.5lbs once all is done. That is 20% lighter than the Li-ion, so 3% off of my initial estimate.
```

---
## \#90 Posted by: Namasaki Posted at: 2017-03-07T03:25:34.306Z Reads: 641

```
My 26650 pack was very disappointing, I had my meter mounted through the deck so I could monitor it while riding and saw my battery drop 30-40% in voltage sag while climbing a 10% grade.
```

---
## \#91 Posted by: PXSS Posted at: 2017-03-07T03:36:42.671Z Reads: 636

```
What cells were you using?
```

---
## \#92 Posted by: CaptainMerricka Posted at: 2017-03-07T03:45:34.754Z Reads: 637

```
I can go 9-10 miles on a charge with identical batteries and different combo.
```

---
## \#93 Posted by: Namasaki Posted at: 2017-03-07T06:08:20.034Z Reads: 633

```
https://liionwholesale.com/products/basen-4500mah-26650?variant=14135870212
```

---
## \#94 Posted by: Namasaki Posted at: 2017-03-07T06:10:41.908Z Reads: 611

```
I'm getting 10 mi with hills. Haven't done the moderate speed flat ground test yet.
```

---
## \#95 Posted by: Xaeron Posted at: 2017-03-07T09:57:46.255Z Reads: 609

```
Yup, your conversation pretty much confirms my theory. A 10s4p has two times more energy but in practice, using it on street, gets pretty much the same range :S
```

---
## \#96 Posted by: Maxid Posted at: 2017-03-07T09:59:48.972Z Reads: 606

```
huh?
10characters
```

---
## \#97 Posted by: Xaeron Posted at: 2017-03-07T10:12:38.553Z Reads: 612

```
After reading many topics on the forum I was feeling that people on 10s 5000mah lipo were having the same range than 10s3p and almost like 10s4p

Namasaki just said that he is getting same range on his 10s3p 9000mah liion than in his 10s 5000mah lipo
```

---
## \#98 Posted by: Maxid Posted at: 2017-03-07T10:17:06.756Z Reads: 621

```
Have you also asked people on their VESC cut-off values?
Liions should be ridden with a VESC cutoff at 3V while Lipos typically are only used until 3.4V.
There is a lot of Energy left if you keep your Lipo settings and just switch to a Liion battery.
```

---
## \#99 Posted by: Xaeron Posted at: 2017-03-07T10:41:58.673Z Reads: 623

```
I have not, as I said it is just an impression that I have and feels weird even to me but what Namakasi said can be true... Liion have a huge voltage sag on high demand of power and that can cut drastically its range
```

---
## \#100 Posted by: Maxid Posted at: 2017-03-07T10:48:36.033Z Reads: 629

```
I had that problem - the right VESC cut off values will solve it though. Liions definitely need the proper cut-offs - otherwise you will sag down too far and the VESC takes away power. A good thing is to look at actual logs - I rode my battery (the one you know about) to 3.5V and already thought that it is at its end since this is below 3.6V and they go down fast at this point. However the log showed only 150Wh used from a potential 270Wh - so quite some juice left. At home I checked with http://lygte-info.dk/review/batteries2012/Samsung%20INR18650-25R%202500mAh%20%28Green%29%20UK.html and saw that 3.5V has still plenty left. If my cut-off would have been at 3.4V I surely would have thought it is empty.
```

---
## \#101 Posted by: PXSS Posted at: 2017-03-07T12:00:08.496Z Reads: 626

```
Boo, I couldn't find discharge curves for those cells...
Based on a similar cell the bestfire inr26650, you should be able to pull 30A per cell sagging 18% up to 3Ah. That means 3600W...

What were your voltage limits set to?
Do you have any of the logging apps?
```

---
## \#102 Posted by: Namasaki Posted at: 2017-03-07T14:38:12.422Z Reads: 608

```
Voltage limits where set lower for my Li-ion pack than for my Lipo pack. The problem was that my Li-ion pack sagged so much and depleted so quickly under high load conditions. 
My first build was with Lipos, charging them with a hobby charger. 
Then I switched to Li-ion thinking they would be safer and more convenient with a BMS and expecting the same or better performance as the Lipos. 
But I was terribly disappointed with there lack luster power and ridiculous voltage sag under load. 
So I went back to Lipos but this time with a BMS. 
Now I have power and convenience. 
And the only time that my Li-ion pack had more range was when cruising the flat boardwalk at no more than 10mph. 
Even though the Li-ion pack had more watt hours, 
It depleted so much faster than my Lipo pack under more challenging conditions  that they even out in range with the Lipo pack delivering more power throughout that range.
```

---
## \#103 Posted by: Maxid Posted at: 2017-03-07T14:45:32.294Z Reads: 606

```
Unles your efficiency changed your statement makes no sense.
Energy is energy - it can't just disappear.
So there must be more to this story: You either used only mediocre cells or had wrong cut-offs.
5000mAh from a Liion HAS to get you as far as 5000mAh from a Lipo (at the same voltage obviously).

Voltage drop is an issue yes - but that would just mean you did not use up all the energy in your liion pack.
How much did you actually charge it?
```

---
## \#104 Posted by: PXSS Posted at: 2017-03-07T14:45:57.683Z Reads: 593

```
The problem is that your voltage should not sag 30-40% ever unless you were drawing like 5kW which is highly unlikely.
That is super weird... Maybe you got bad cells? That's kind of why I only buy Samsung, LG, Sony or Panasonic cells. They got way more to lose if they produce crap cells since they're used in industrial applications.

Do you still have this pack?
Would you like to fix the issues with it? I could probably help you with troubleshooting if you can log data.
If you don't really care for it then, no worries.

E: Check out Kaly's thread, he's got a 12S4P LG pack on his mtb with dual 6374s that he rode 20 miles in just over an hour.
```

---
## \#105 Posted by: Xaeron Posted at: 2017-03-07T14:55:56.368Z Reads: 594

```
5000mah from Liion SHOULD get you as far as 5000mah from Lipo

But in practice you don't get 5000mah of any of them. Part of the energy disipates in heat and a lot of energy is just wasted on drivetrain and so on. When you have a big sag you are wasting more energy. (For example, full throttle for 1km, sag of 1v in one battery and 3v on another battery, the first will be using less energy than the second)

So that is why I said that in practice, Liion seems to be making a lot less range than it should when compared to LiPo, and Namakasi is not the only person having this, there are a couple of threads with a lot of people telling their ranges and people with 6s5000mah lipo are getting unbelievable long ranges.
```

---
## \#106 Posted by: PXSS Posted at: 2017-03-07T15:07:11.750Z Reads: 628

```
Kind of agree but not really.
The issue with @Namasaki's pack is that it's sagging way more than what it should be.
The issue with most others that have this issue is that they use 25R cells which as I explained are not great.

Here is a good comparison from another thread:
[quote="radium, post:23, topic:17296"]
I'll throw my 2c into the ring. I built a 12S5P lithium ion pack using Samsung 18650 30Q for about $300 it could be cheaper depending on 18650 cell and supplier. It's a lot of cells, but it allowed me to configure and arrange them how I wanted and needed to make them fit. The pack has a capacity of 15Ah and 75A continuous discharge rate.

I also have 2 6S Multistar 16Ah batteries that are supposedly 10C max discharge. Realistically for our use, they're about 5C, otherwise the voltage sag is too great. They were about $150 shipped. They are bulky batteries, I had to make a second enclosure just for when I run the Multistars because of their height. I could break them apart and a rebuild the packs, but that negates one of their supposed benefits of out of the box simplicity. They're also heavy.
[/quote]

[quote="radium, post:26, topic:17296, full:true"]
Mine doesn't slow down on a 10-15% grade, and I get over 30 miles on a single charge. My total of $300 included a BMS and an appropriate charger. To get a comparable lipo config outside of the Multistar lineup would probably cost around $300 with a charger that could balance charge the batteries simultaneously.

I haven't had my board working for too long, but in my limited testing I've never pulled more than 107A with 2 6355 motors. It was measured with that in line Turnigy power meter. How many amps are you pulling with Li Ion where you start to notice a slow down going up hills?

Another consideration is that I could probably add another 10-20 cells into my 18650 config if I put it into an enclosure the size of the one required for the Multistar batteries.

Either way, both are definitely useable, my only experience is with Multistar because it offered the most capacity for the right price. I imagine other lower capacity packs don't get as hot.
[/quote]

from this thread:
http://www.electric-skateboard.builders/t/what-is-the-downside-of-single-18650-cells-with-high-higher-ah/17296/

We discuss in detail the pros and cons of LiPo vs Liions.
I suggest you read it.
```

---
## \#107 Posted by: Maxid Posted at: 2017-03-07T15:09:31.288Z Reads: 563

```
[quote="Xaeron, post:105, topic:10014, full:true"]
But in practice you don't get 5000mah of any of them. Part of the energy disipates in heat and a lot of energy is just wasted on drivetrain and so on. 
[/quote]

That is why I said that unless his efficiency changed this is impossible.
voltage drop has nothing to do with this - sure we could assume that the heat generated by the Liion is higher than Lipo but I highly doubt that this happens in meaningful amounts. If we would have to dissipate an additional 100Wh via the battery our enclosures would be HOT and the VESC would shut off due to overheating. Ever touched a traditional 60W light bulb while on?
```

---
## \#108 Posted by: Xaeron Posted at: 2017-03-07T15:33:50.655Z Reads: 560

```
Very interesting reading @PXSS, it's a pity that they are not showing real range 

I guess it all depends on the quality of the cells and lipos.

One thing that I know for a fact after years in rc cars and multirotors is that C rating is bullshit in lipos, so if it is in 18650 too we can only trust real tests
```

---
## \#109 Posted by: Namasaki Posted at: 2017-03-07T16:18:47.632Z Reads: 540

```
I'm at work now so I'll have to resume later
```

---
## \#110 Posted by: PXSS Posted at: 2017-03-07T17:00:24.647Z Reads: 543

```
Most of my posts on that thread are from real tests.
I don't go by ratings.

@Namasaki
Me too :stuck_out_tongue:
```

---
## \#111 Posted by: mmaner Posted at: 2017-03-07T18:37:36.090Z Reads: 546

```
I had the same thing.  Started out using x2 Zippy 3s 30c 5kmAh Lipos in series.  I went to a 10s3p lion pack made with 25r's.  Did not like the loss in torque that resulted in the voltage sag.  So I went back to my lipos.  I am now trying another 10s3p, if I can get the damned thing to fit.  I also have a 30q 10s3p pack in the works.  Im hoping the 30q's prove to be as resilient and beastly as the lipos :).
```

---
## \#112 Posted by: Namasaki Posted at: 2017-03-07T19:05:01.095Z Reads: 523

```
I'm interested in hearing how your 30Q pack compares to your Lipos
```

---
## \#113 Posted by: mmaner Posted at: 2017-03-07T19:06:25.303Z Reads: 524

```
Ill let you know when I get there, still a couple of weeks away at least.
```

---
## \#114 Posted by: radium Posted at: 2017-03-07T19:14:13.305Z Reads: 558

```
Namasaki 26650 cells aren't as good as name brand 18650 cells. A lot more R&D was put into 18650's since they were heavily used in laptops for a long time. 18650 was the only size battery that had enough manufacturing infrastructure already built around it for use in electric vehicles. This is why Tesla chose this size cell. They had the best specific energy, and could be manufactured in larger quantities with tighter manufacturing tolerances more quickly than any other size cell.

The other issue is name brand cells from reputable suppliers vs off brand Chinese or recycled cells. A lot of chinese suppliers take old Samsung, LG, Panasonic etc... cells and clean them up re-wrap them and cell them as new cells. A lot of chinese suppliers also buy cheap knock off 18650 cells from Chinese factories and sell them as legit name brand cells.

The vape community has done extensive testing around 18650 batteries and how much a single cell can handle in terms of current draw and voltage sag. This information is all out there publicly. If you're interested search for posts by "battery_mooch" or maybe "battery_m00ch" on reddit his name is something like that. He's put out a wealth of information about 18650 cells some of which are of interest to us.

The TLDR of my post, 18650 cells produced by Samsung, LG and other name brand companies have spec sheets which are accurate. These figures may be inflated by resellers, but go look at the manufacturing spec sheet for real info. If you buy cells made by someone other than Samsung, Panasonic, LG and Sanyo you can expect the specs to be inflated.

If you buy cells from a disreputable reseller, you can expect there is a good chance they will be re-wrapped chinese or recycled cells not the real cells.

18650's are great for our purposes, but there are a TON of fake resellers of cells. Be careful and know your supplier.
```

---
## \#115 Posted by: Namasaki Posted at: 2017-03-07T19:14:27.435Z Reads: 524

```
[quote="PXSS, post:104, topic:10014"]
Do you still have this pack?Would you like to fix the issues with it? I could probably help you with troubleshooting if you can log data.If you don't really care for it then, no worries.
[/quote]
I Appreciate the offer but unfortunately I had stored it in my safe for safe keeping and my safe was taken during a burglary. How ironic is that?
```

---
## \#116 Posted by: radium Posted at: 2017-03-07T19:15:59.717Z Reads: 507

```
A 10S3P pack is always going to sag some when you pull more than 45-60 amps from it. I'm not sure how much amperage you guys draw, but Zippy's are capable of more amp output.
```

---
## \#117 Posted by: Maxid Posted at: 2017-03-07T19:16:28.207Z Reads: 495

```
They probably had fun when they used a blow torch to open that thing :D
```

---
## \#118 Posted by: Namasaki Posted at: 2017-03-07T19:26:49.608Z Reads: 522

```
Ya, I'm thinking that the Basen 26650 cells where overrated. I went with those because of the 4500mah in an attempt to build a compact battery with good range. And its range was exceptional under very mild conditions but not under more demanding conditions. 

 It's my understanding that Tesla doesn't use just any 18650 but theirs are special.
 From what @PXSS has stated, it sounds like those 30Q cells may be the best available option for A Li-ion battery.
As for me, I'm happy with what I'm getting from my Lipo packs so I'm not looking for other options at this time.
```

---
## \#119 Posted by: radium Posted at: 2017-03-07T19:34:26.314Z Reads: 538

```
The other thing with these batteries is as capacity increases, current draw decreases. Typically a good 2500mAh cell from the same generation as a 3000mAh cell will be able to handle more load with less heat and voltage sag.

I don't know as much about 26650 cells as I do about 18650 cells, but the current generation 18650's absolute top of the line cells for capacity are 3500mAh. Those aren't suitable for our uses though. They might be in something like a 10P config, but realistically for us 3000mAh cells like the Samsung 30Q and LG HG2 are about the best we'll get in terms of capacity.

I'm thinking about either reconfiguring my 12S5P pack or building another 10S6P pack with cells from the same supplier to see if I get more torque because my only experience so far is with my 12S5P pack and 16AH Multistar batteries. People have said the Multistar batteries are lackluster in terms of voltage sag under load and don't give enough torque. Both seem fine to me, I get comparable range and speed from both. The 18650 pack sags slightly less under load.

I've yet to top out either pack. I cruise around at probably 18-22mph top speed. I didn't realize how fast 25+mph would feel on a board when it is that high up. Most of my longboarding experience was on drop throughs or dropped boards. I owned one top mount which I turned into the esk8 and with the angled risers, it's very high up from the road. I might try putting stiffer bushings on it but I like the carvy feeling I have now.
```

---
## \#120 Posted by: Maxid Posted at: 2017-03-07T20:16:05.259Z Reads: 508

```
I am just wondering how manufacturers like Inboard can sell their boards with 12S1P 18650 configs and get away with it. The voltage sag must be HUGE on those packs.
```

---
## \#121 Posted by: Namasaki Posted at: 2017-03-07T21:17:13.489Z Reads: 518

```
I would not even consider building a10s6p or 12s5p battery out of 18650 cells because of the size and weight of it. I mean 60 cells, that's gonna be over 22" long in a low profile configuration. We have tall speed bumps where I live so ground clearance matters. 
What I needed was plenty of power in a compact low profile light weight battery and since my rides are usually 10mi or less, range is not my main concern.
```

---
## \#122 Posted by: radium Posted at: 2017-03-07T21:19:27.969Z Reads: 484

```
I already have one. I do 2x30cell 6S batteries stacked 2 cells high by 15 cells long. Then wire those in series. My board is curved and I mount them as close to the outside of the deck as possible. The way I have them stacked, they're only about 1.3 in tall stacked 2 high.
```

---
## \#123 Posted by: PXSS Posted at: 2017-03-07T22:27:36.998Z Reads: 515

```
Ok, I'll try to reply to all posts in one hahaha. 
I'm building @mmaner's pack. Hopefully it'll only be a weekend or two until I can get to it.

Kinda sucks that your safe got stolen, hopefully it caught fire before they could take anything from it...

Tessa uses Panasonic NCR18650B cells, they're the old gen of the NCR18650GA cell which used to be made by Sanyo (who got bought out by Panasonic who is partly owned by Tesla, I hope you seethe connection now). There is really nothing special about their cell except that they use 7800 of them lol. The secret sauce is their temperature control algorithm and system. 

The 30Q cells are not the best, VTC6's by Sony are, but these cost $6 a cell. I can source 30Q at $3 a cell for like 10% more sag. 

@radium is correct, a lot of research has gone into 18650, other size cells are not nearly as optimized.
```

---
## \#124 Posted by: mptrs Posted at: 2017-03-07T22:33:18.768Z Reads: 504

```
@Namasaki thanks for all the answers! Hope to receive my BMS the coming days and connect it all up. The 5V from the receiver is a nice idea, not tho they will be in the same box. But that's a whole different part of the project hehe
```

---
## \#125 Posted by: Namasaki Posted at: 2017-03-07T22:39:07.156Z Reads: 491

```
You could use an Sbec connected to the output of the BMS and battery to supply 5v if you really want a lighted on/off button.
```

---
## \#126 Posted by: Namasaki Posted at: 2017-03-07T22:58:59.768Z Reads: 486

```
I would pay the $6 per cell to have the better cells. 
I think I paid $7 per cell for my 26650s because I thought they would be awesome.
```

---
## \#127 Posted by: radium Posted at: 2017-03-07T23:11:56.694Z Reads: 480

```
Another problem with VTC 6 is that there are a TON of fakes. Probably more than just about any other 18650 cell. I'm sure counterfeit 30Q exist somewhere, but they're not very common.
```

---
## \#128 Posted by: Namasaki Posted at: 2017-03-07T23:19:51.549Z Reads: 471

```
That's a huge problem and why I wouldn't even think of buying them on Ebay.
```

---
## \#129 Posted by: PXSS Posted at: 2017-03-07T23:31:42.968Z Reads: 497

```
Liionwholesale...
I've never had fakes from them.
I've purchased 300 Sony VTC6, ~1500 Sanyo GA, and 2 of LG HG2, LG MJ1, Samsung 30Q, and Panasonic B cells.
All of them undergo a capacity test by me when we receive them.
```

---
## \#130 Posted by: willpark16 Posted at: 2017-03-08T06:01:31.464Z Reads: 500

```
I second that lg he 2 and Samsung 25r
```

---
## \#131 Posted by: landonkun Posted at: 2017-03-08T07:54:04.825Z Reads: 512

```
[quote="Namasaki, post:126, topic:10014, full:true"]
I would pay the $6 per cell to have the better cells. I think I paid $7 per cell for my 26650s because I thought they would be awesome.
[/quote]

Nooooo stop making me feel so discouraged! I'm about to do my very first build with a 10S2P using the Basens :frowning:
```

---
## \#132 Posted by: Namasaki Posted at: 2017-03-08T16:23:02.998Z Reads: 486

```
10a2p will work for flat ground
```

---
## \#133 Posted by: mptrs Posted at: 2017-03-08T18:54:47.142Z Reads: 492

```
Good one! And I think I have just the thing lying around in the old parts I bought but never used box hehe
```

---
## \#134 Posted by: TheDrYou Posted at: 2017-03-22T18:15:57.160Z Reads: 495

```
Wanted to run this by everyone and @Namasaki  before I order. I was going to get 2 of these https://hobbyking.com/en_us/zippy-flightmax-5000mah-5s1p-20c.html for 5A 10S. This BMS http://www.batterysupports.com/36v-37v-42v-10s-80a-10x-36v-lithium-ion-lipolymer-battery-bms-p-389.html. I gather I can get two of the "BALANCE LEAD EXTENSION" for the two batteries? And need a charger if anyone can recommend one.
```

---
## \#135 Posted by: Namasaki Posted at: 2017-03-22T22:37:39.764Z Reads: 491

```
You will need a 42v charger either 2a or 5a. You can find those easily on Ebay.
The 2a version can be had for less than $20.
The 80a bms you listed will be plenty adequate for charge and discharge.
You will also need an E-switch or an anti-spark loop key.
```

---
## \#136 Posted by: TheDrYou Posted at: 2017-03-23T02:07:46.605Z Reads: 496

```
Charger: http://www.ebay.com/itm/For-Hoverboard-Smart-Balance-Scooter-Wheel-Universal-Charger-42V-2A-adapter-/262623199401?hash=item3d259000a9:g:PtsAAOSw1S9WgOis

Charging Port and Switch: http://www.ebay.com/itm/New-Design-Hoverboard-Charging-Port-Power-Scooter-Repair-Parts-Replacement-/262370357698?hash=item3d167df1c2:g:PpAAAOSwjDZYlB14

With a setup like this how do you know when it's done charing?
```

---
## \#137 Posted by: Namasaki Posted at: 2017-03-23T03:58:37.081Z Reads: 512

```
The charger you listed will work fine. It will automatically stop charging when the battery is full.
The charge port you listed is the same one that I use. The switch that comes with it us useless though because it is a momentary switch.
You will need an E-switch like this:

http://www.electric-skateboard.builders/t/new-directfet-anti-spark-switches-with-onboard-led-circuit/18762
```

---
## \#138 Posted by: TheDrYou Posted at: 2017-03-23T04:22:57.693Z Reads: 493

```
[quote="Namasaki, post:135, topic:10014"]
anti-spark loop key
[/quote]

I don't understand how something as simple as an anti-spark loop key can't be replaced with anything less complicated.
```

---
## \#139 Posted by: Namasaki Posted at: 2017-03-23T04:56:06.065Z Reads: 486

```
The loop key is the only option that is simple
```

---
## \#140 Posted by: Namasaki Posted at: 2017-03-23T05:05:50.304Z Reads: 491

```
If your wanting a push button to turn your board off and on then you will need an E-switch 
Or get a Bestech BMS with a build in e-switch
```

---
## \#141 Posted by: Michaelinvegas Posted at: 2017-03-23T05:50:17.293Z Reads: 501

```
[quote="TheDrYou, post:138, topic:10014"]
I don't understand how something as simple as an anti-spark loop key can't be replaced with anything less complicated.
[/quote]





The problem is that there are few options in terms switches that can withstand the amp loads of esk8 with voltages higher than 6s...check around...pretty much anti-spark loop key or some type of antispark switch are the only choices...regular switches like a light switch can handle 120v, but not the amps a 12s (50.4v) would produce for example.
```

---
## \#142 Posted by: ewalks6 Posted at: 2017-04-02T22:40:12.148Z Reads: 481

```
What's up.

Quick Q. Sold my batteries (the 2S2P ones, shouldn't lose much if not any money so that's good). I am looking at new ones and can't decide between 2S 5000mAh 30C and 2S 5000mAh 40C. I know that you say the higher the C the lower the sag, and the packs max outputs are 150A v 200A, but the second one is about $3 more (x5 = $15). Is it worth it to get the 40C ones?
```

---
## \#143 Posted by: Namasaki Posted at: 2017-04-02T22:42:21.114Z Reads: 476

```
Absolutely worth it especially if its only $3 per pack. Get the 40c for sure.
So what about the 60c like I used? They would be even much better.
```

---
## \#144 Posted by: ewalks6 Posted at: 2017-04-03T00:35:57.725Z Reads: 472

```
Those are about $27, which would be another $30 or so when I am already over budget. I know 60C would be better but I really am trying to keep the price down. Also the hardcase makes the pack a little bigger and I am tight on space.
```

---
## \#145 Posted by: Namasaki Posted at: 2017-04-03T01:07:32.609Z Reads: 460

```
Alright,  they are actually not available in the USA from Hobby King at this time.
So I would highly recommend that you spend the extra $15 for the 40C. 
It's well worth it.
```

---
## \#146 Posted by: ewalks6 Posted at: 2017-04-03T01:34:24.428Z Reads: 462

```
Just bought it. Last part that I need so can start building once they come! Thanks for all the help.
```

---
## \#147 Posted by: Namasaki Posted at: 2017-04-03T01:39:23.556Z Reads: 460

```
do you have a hobby charger?
If yes, it's a good idea to balance charge the packs before putting them together.
If no, check each packs voltage and balance. All cells should be close to same voltage when you put them together.
```

---
## \#148 Posted by: emstr Posted at: 2017-04-30T05:49:16.083Z Reads: 449

```
Do you still need a buyer?? Would totally buy!
```

---
## \#149 Posted by: Iam319 Posted at: 2017-04-30T11:17:17.347Z Reads: 448

```
Hey man, any idea how to find the rpm of hub motors? I haven't been able to find info on it and I'd love to know.
```

---
## \#150 Posted by: Iam319 Posted at: 2017-04-30T11:37:13.458Z Reads: 457

```
How long does it usually take you to charge your 10s board with a 2A charger?
```

---
## \#151 Posted by: Namasaki Posted at: 2017-04-30T20:44:37.513Z Reads: 466

```
[quote="Iam319, post:149, topic:10014"]
Hey man, any idea how to find the rpm of hub motors?
[/quote]


What hub motors are you referring to?
```

---
## \#152 Posted by: Namasaki Posted at: 2017-04-30T20:45:58.295Z Reads: 462

```
[quote="Iam319, post:150, topic:10014, full:true"]
How long does it usually take you to charge your 10s board with a 2A charger?
[/quote]


I usually charge with 5a and I don't usually discharge completely so it's hard to say.
```

---
## \#153 Posted by: Iam319 Posted at: 2017-05-01T01:39:49.413Z Reads: 449

```
I'm going to use the 90mm maytech hub motors. I'm aware they're not the best but my budget doesn't really allow for much else.
```

---
## \#154 Posted by: mptrs Posted at: 2017-05-02T20:09:15.325Z Reads: 437

```
@Namasaki is it possible for you to show how you connected you switch to the BMS?
Bit cautious now cause I blew my switch yesterday hehe. (not connected to the BMS)
```

---
## \#155 Posted by: mmaner Posted at: 2017-05-02T21:19:29.025Z Reads: 439

```
On almost all BMS's the switch wires are either open or closed.  There is no NEG or POS, its simply an open loop for OFF or a closed loop for ON.  Obviously this is for BMS's tat have a switch, some do not.
```

---
## \#156 Posted by: Namasaki Posted at: 2017-05-03T02:37:09.621Z Reads: 438

```
Exactly as @mmaner said. The Bestech E-switch has 2 white wires. When there connected together, the bms turns on.
When there disconnected, it turns off.
All you need is a simple 2-pole automotive switch connected to the wires.
```

---
## \#157 Posted by: mptrs Posted at: 2017-05-03T20:52:55.345Z Reads: 434

```
Thx @mmaner and @Namasaki, was a just to be save question hehe.
Atm I'm mostly using 12AWG wire and 14AWG from the charge port to the BMS. Is this gonna be a problem? Using XT150 for connectors, so that'll be save enough.

VESC came with 12AWG, so thought that would be save enough.

Wiring finally coming together thanks to your diagram and tips @Namasaki. Thanks again!
```

---
## \#158 Posted by: Jinra Posted at: 2017-05-03T21:05:05.416Z Reads: 443

```
12/14 AWG to a charge port is fairly beefy. Since chargers typically charge around 4 amps you can use a thinner cable than that. I think mine is 18/20 awg.
```

---
## \#159 Posted by: mattfink Posted at: 2017-05-04T15:48:26.649Z Reads: 439

```
really like this idea!

I would like to duplicate this approach, but ideally would like to keep the possibility of going to 12S open, if it turns out my build is underpowered on 10S is there a 12S version of the bestech BMS you used? 

if I wired a 12S BMS to a 10S battery initially would you expect that to work?
```

---
## \#160 Posted by: Namasaki Posted at: 2017-05-04T16:13:37.970Z Reads: 428

```
There is a 12s version. 
I don't think a 12s bms with 10s battery will work

If you want Maximum power and range, then 12s
Is the ticket
```

---
## \#161 Posted by: mattfink Posted at: 2017-05-04T23:21:06.347Z Reads: 447

```
Thanks, think i found the 12s version, but also found this one

http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D328.html

Looks like it has a lot of extra features and is programmable for different numbers of cells, worried it might be overly complicated to configure tho' done a few searches and nobody seems to be using it.

I'm new to esk8 and skating in general so 10s seems like a more sensible place to start than 12S, but like the idea if just being able to buy 1 extra cell if i do decide i need the extra volts. Could this BMS be a sensible choice?
```

---
## \#162 Posted by: Namasaki Posted at: 2017-05-04T23:31:20.266Z Reads: 432

```
Those look interesting with their software adjustability. I'm not positive but I think they are rather pricey.
And you will have to buy the optional computer adapter to connect it.

If your just staring out, 10s is probably a better choice seeing that it is easier to manage the power than 12s.
One benefit with the bms that I use is that it has a built in E-switch saving you at least $45 that you would spend on an external E-switch.
And some of it's  parameters are adjustable as well. Only you have to request them when you order it and they are set at the factory.
```

---
## \#163 Posted by: mattfink Posted at: 2017-05-04T23:32:39.726Z Reads: 435

```
Also i was wondering if i could get secure enough and high enough amp connectors that i could plug all the cells together, was thinking i could then unclip to replace cells or make plane legal.

There was a long thread on here about plane legal cells and my understanding is, if they are standard off the shelf cells, correctly rated and under 100kw they are fine, so thinking 5 of these cells once separated would be okay.

do you think bullet connectors of the type used on the battery work for this?
```

---
## \#164 Posted by: Namasaki Posted at: 2017-05-04T23:44:31.395Z Reads: 431

```
I would trust the 5.5mm bullet connectors for an application like that. They are heavy duty and fit together tightly and they don't come apart with vibration. 
They work well with heavy gauge silicone wire like 12ga and 10ga
And they do not add a lot of bulk to your wiring as other connectors will.
```

---
## \#165 Posted by: mattfink Posted at: 2017-05-04T23:51:15.288Z Reads: 414

```
yeah i've seen them at eu 130 which obviously isn't keep how does that compare to the 10s version you went for?
```

---
## \#166 Posted by: mattfink Posted at: 2017-05-04T23:52:35.201Z Reads: 416

```
Great think i'll give that a try then!
```

---
## \#167 Posted by: Namasaki Posted at: 2017-05-04T23:53:29.807Z Reads: 426

```
The one I use is only $49 plus shipping and PayPal fees.
Total is about $68 ea.
Bestech's order min is 2 bms's

If you don't need 2 or don't want to have a spare, you can sell the extra bms on the forum easily.

Btw, the have a facility in Germany  to service Europe
```

---
## \#168 Posted by: mattfink Posted at: 2017-05-04T23:57:54.191Z Reads: 443

```
So they might actually let me buy the 10s and 12s as a minimum order and it could still work out cheeper? that's worth knowing, i don't really want another board to programme in any case, although the battery level info on the HCX-D328 sound cool.
```

---
## \#169 Posted by: Namasaki Posted at: 2017-05-05T00:02:22.425Z Reads: 471

```
Except, you need to monitor battery level while riding. How you gonna do that with LED's on the bms that you can't see.
Better to have an inline meter mounted through the top of your deck so you can just look down to check the battery.

Like this
<img src="/uploads/db1493/original/3X/a/9/a9134849918321ed8cc4f69e087ed36ca52143d9.jpeg" width="375" height="500">
```

---
## \#170 Posted by: Namasaki Posted at: 2017-05-05T00:04:09.381Z Reads: 455

```
[quote="mattfink, post:168, topic:10014"]
So they might actually let me buy the 10s and 12s as a minimum order
[/quote]


I don't know if they do that or not. I never tried that. It can't hurt to ask them.
```

---
## \#171 Posted by: tonystark Posted at: 2017-05-08T20:17:29.689Z Reads: 453

```
[quote="Namasaki, post:7, topic:10014, full:true"]
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
[/quote]

I cant figure out how to order BMS on bestechpower website. can you suggest how to buy products there please?
```

---
## \#172 Posted by: Namasaki Posted at: 2017-05-08T20:28:39.464Z Reads: 475

```
Bestech sales are done through email.
Send an email to lucy@bestechpower.com requesting to purchase the bms module.
The minimum purchase is for 2 modules.
The cost is $49 ea. plus shipping and PayPal fee.
If you don't want to keep the extra module, they are easily sold on this forum.
Some of the parameters are adjustable at the factory and you will need to specify your preferences during the order process.
I recommend these settings for Lipo batteries,  for Li-ion you could lower the over discharge voltage detection to 2.8v

<img src="/uploads/db1493/original/3X/5/7/57863a69b56052e35845d934938c29706fc495c7.png" width="355" height="499">
```

---
## \#173 Posted by: tonystark Posted at: 2017-05-08T21:01:43.085Z Reads: 448

```
thank you for help. so i just have to tell them that i have 8s3p battery and that is it and what kind bms i want to buy?
```

---
## \#174 Posted by: Namasaki Posted at: 2017-05-08T21:05:49.912Z Reads: 445

```
You need this one:
http://bestechpower.com/296v8spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#175 Posted by: tonystark Posted at: 2017-05-08T21:10:31.376Z Reads: 454

```
yes sir, this is the one. i just emailed her. second bms i will get 10s since majority of people on the form use 10s battery packs. or i will use it for my second elongboard that i want to build if this one will come out good. thank you again for help mate
```

---
## \#176 Posted by: nihliphobe Posted at: 2017-06-02T03:13:38.921Z Reads: 442

```
@tonystark Do you still have that 10s BMS? I'd take it off your hands :)
```

---
## \#178 Posted by: tonystark Posted at: 2017-06-02T06:42:37.384Z Reads: 442

```
No, i ordered from anothere website and you can buy only 1 there
```

---
## \#179 Posted by: zeno Posted at: 2017-06-03T12:32:04.217Z Reads: 445

```
Thanks for the info! :slight_smile:
I'm looking at getting either the exact same batteries, or these softpacks (that are only 19mm thick! :open_mouth: ) :

https://hobbyking.com/en_us/turnigy-nano-tech-5000mah-2s-65-130c-lipo-pack.html 

As far as I can see the c-rating instead of being a solid 60c is 65~130 (weird) but overall specs seem to match the hard case packs. What do you guys think?
```

---
## \#180 Posted by: Namasaki Posted at: 2017-06-03T14:55:03.619Z Reads: 444

```
Those should work fine. 
The 65~130C means 
65C continuous 
130C pulse

The hard packs I used are 60~120C
```

---
## \#181 Posted by: SeanHacker Posted at: 2017-06-17T15:21:26.082Z Reads: 437

```
This is pretty cool @Namasaki . I'm thinking I need to do this as a cheaper alternative to my 10s4p samsung 22r pack that is giving me problems. I have a SuPower 10S 60a BMS (http://www.ebay.com/itm/221769582503?_trksid=p2060353.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT) laying around. Will that work with these batteries? Do you think I can fit this same battery setup in my master cho enclosure? The internal dimensions of the enclosure is about 21x6.5x1.14 but it narrows down slightly toward to ends.
```

---
## \#182 Posted by: Namasaki Posted at: 2017-06-17T15:46:05.455Z Reads: 424

```
The Supower bms will work and it sounds like the batteries will fit in that case.
```

---
## \#183 Posted by: SeanHacker Posted at: 2017-06-17T15:48:16.005Z Reads: 412

```
Awesome! I'm thinking I'm going to try this out then. I'm a total dummy when it comes to batteries so hopefully you're around to answer some questions so that I don't blow myself up! Thanks for the response dude!
```

---
## \#184 Posted by: Namasaki Posted at: 2017-06-17T17:13:31.367Z Reads: 416

```
I'll be around and I check the forum daily and I'm always glad to help if I can.
```

---
## \#185 Posted by: Namasaki Posted at: 2017-06-20T03:33:55.189Z Reads: 430

```
Test run today with hills. 
Data taken from one of 2 Vescs so battery current should be doubled. 
Voltage sag appears to be minimal. 
https://metr.at/r/oyETP
```

---
## \#186 Posted by: Namasaki Posted at: 2017-06-27T02:58:42.078Z Reads: 427

```
Here's another test run in the mission beach boardwalk. Mostly flat with some stop and go and braking for pedestrians. Mild acceleration 
Dual 6355 190kv, 15/40 gears 90mm wheels 

https://metr.at/r/wvwpZ
```

---
## \#187 Posted by: Namasaki Posted at: 2017-06-28T04:17:38.626Z Reads: 416

```
One more test run around the neighborhood with one really steep hill.
42a total battery current with 2v total Voltage sag on that hill.
https://metr.at/r/sRQMX
```

---
## \#188 Posted by: SpeedSloth Posted at: 2017-06-28T12:46:39.833Z Reads: 401

```
How are you getting that log data from the VESC? Do you have to enter the wheel size some where for it to calculate the speeds?
```

---
## \#189 Posted by: Namasaki Posted at: 2017-06-28T13:17:19.019Z Reads: 420

```
Yes, wheel size and gear sizes

<img src="/uploads/db1493/original/3X/2/0/205004aff996725cfff180aa4038ee2c253db7e9.jpg" width="281" height="499">
```

---
## \#190 Posted by: stanl3yy Posted at: 2017-07-06T20:55:04.188Z Reads: 395

```
This setup is perfect for me.
I got the same battery's only differend BMS, one from ebay. I regred not taking the one you ordered because mine doesn't have an e-switch so i bought that sepperately from alienpowersystem.

I am waiting for my vesc to arrive and then I can start my build (enertion vesc).

How many kilometers do you get of an full charge?

Thanks for the info, it helped me a lot!
```

---
## \#191 Posted by: Stef Posted at: 2017-07-06T21:30:30.054Z Reads: 387

```
If anyone is still looking for a 10S BMS, I have a brand new bestech for sale due to the minimum order of two. It has the switch built in and has been working flawlessly on my 2x6355 build. Im located in the US and prefer a US buyer.
```

---
## \#192 Posted by: Namasaki Posted at: 2017-07-07T01:22:49.461Z Reads: 389

```
10-12 miles
14 miles on flat ground if you take the battery down to 32v
But I wouldn't recommend that. I would recommend stopping no lower than 36v.
```

---
## \#193 Posted by: stanl3yy Posted at: 2017-07-08T19:02:56.083Z Reads: 382

```
I only have 1 motor (6374/ 3150W/ 190Kv from torqueboards). Will I get more range?
```

---
## \#194 Posted by: Namasaki Posted at: 2017-07-08T19:36:37.760Z Reads: 383

```
Not really because one motor will be doing 100% of the work. 
Two motors do 50% of the work each. 
Running dual is easier on the motors and Vescs.
```

---
## \#195 Posted by: twan Posted at: 2017-07-08T21:10:12.218Z Reads: 382

```
whats the website you bought from ?
```

---
## \#196 Posted by: twan Posted at: 2017-07-08T21:33:02.893Z Reads: 377

```
Whats a good cheap charger for those 2s lipos @Namasaki
```

---
## \#197 Posted by: Namasaki Posted at: 2017-07-09T02:48:57.524Z Reads: 385

```
Battery supports sells a 5a brick charger for 10s that's only around $50usd
Or you can get a 2a charger for less
```

---
## \#198 Posted by: twan Posted at: 2017-07-09T22:19:12.975Z Reads: 378

```
Hey Ill buy your extra bms
```

---
## \#199 Posted by: Sleepingalex24 Posted at: 2017-07-10T19:21:35.527Z Reads: 383

```
Are you able to turn on the board while charging in order to check voltages and what not?
```

---
## \#200 Posted by: Namasaki Posted at: 2017-07-10T20:29:05.970Z Reads: 379

```
The bms has to be on while charging
```

---
## \#201 Posted by: twan Posted at: 2017-07-18T19:47:51.764Z Reads: 370

```
is it better to solder all the battery packs or just use 4mm bullet wires to connect them in series?
```

---
## \#202 Posted by: Namasaki Posted at: 2017-07-18T20:13:31.083Z Reads: 379

```
Better to shorten the wires and solder them as I did. 
It's more tidy and there's less resistance in the system.
```

---
## \#203 Posted by: twan Posted at: 2017-07-18T23:12:02.199Z Reads: 370

```
so you just balance them with a charger then soldered them up and charged via bms?
```

---
## \#204 Posted by: Namasaki Posted at: 2017-07-18T23:25:16.330Z Reads: 360

```
Yes, I balanced each pack with my hobby charger before putting them together. Then the bms keeps them in balance.
I attach them to the bottom of my deck with servo tape and then solder them together.
```

---
## \#205 Posted by: bmcm Posted at: 2017-07-19T00:05:16.360Z Reads: 351

```
If it's still available and not sold to twan I'll take it. I'm in Atlanta.
```

---
## \#206 Posted by: Stef Posted at: 2017-07-19T00:52:19.274Z Reads: 354

```
Unfortunately it has already been sold. Though something tells me you will seem them being sold on this forum more often, they have an impeccable reputation here.
```

---
## \#207 Posted by: rich Posted at: 2017-07-19T16:44:51.210Z Reads: 366

```
Hey @Namasaki, love your battery pack design!
I also was thinking several times about such a way to make a pack but there's always 2 questions i have.

Isn't it a problem with one short and one long battery lead (in your case the positive lead is long)?
Read often all leads must be the same length and even the distance from one side to the other of your pack is about 23cm, so the positive lead to the controller incl. BMS is min. 30cm, maybe more..... (In my case the positive lead would be 40cm and the negative 15cm). That's why i never did it.

About the BMS, your bestec has over-discharge protection at 2.9V which is quite high but still 2,9V would damage the Lipo cells i think. Most BMS have even lower over-discharge (i have one with 2,5V) because they are maninly made for Li-ion so i don't know why to use a BMS when e.g. one cell is drifting and the BMS starts working when the weak cell reached 2,5-2,9V when it's too late. 

Are there any advantages to use a BMS compared to fuse only and cheap BMS for charging?
I would like to use a BMS for dischgarge in the future, too but i'm not sure if it can really save the lipos......
```

---
## \#208 Posted by: Namasaki Posted at: 2017-07-19T17:58:57.874Z Reads: 358

```
I'm currently using the same bms with the over discharge detection set at 3.0V which is the highest option.
If one cell drifts down to 3.0v the bms shuts everything down. Some Lipos may handle 3.0v without damage others might not. Normally I try not to run my battery lower than 36v and much of the time I don't go below 38v. 
The other advantages of discharging through the bms are short circuit protection.( if a short anywhere in the system occurs, the bms will instantly shut down the entire system.) This happened to me once when I accidentally  shorted the charge port. The bms shut power down so fast that nothing was damaged not even the battery.
People have complained about having problems with Regen braking downhill on a full battery with their vesc shutting down because of over voltage and then being suddenly without any brakes.
I have tested braking down steep hills with a full battery whiled monitoring my battery voltage. The bms would not let the voltage climb higher than 42.8v on my 10s battery and as soon as I stopped braking, the bms quickly pulled the voltage back down to 42v while I was just coasting.
So it seems safe to say that the bms protects against overcharging though regen braking.
```

---
## \#209 Posted by: Namasaki Posted at: 2017-07-19T18:06:36.532Z Reads: 338

```
[quote="rich, post:207, topic:10014"]
Isn't it a problem with one short and one long battery lead
[/quote]


DC current moves in one direction from negative to positive. Therefore I can't see why the positive wire being longer than the negative wire would make any difference at all except that the longer your power wires are, the more resistance you have.
 But it's not a matter of balancing the positive and negative wires.
```

---
## \#210 Posted by: Silverline Posted at: 2017-07-19T18:42:54.962Z Reads: 338

```
Hallo @Namasaki i have the same  BMS on the way for my Trampa 10S build. Nice to hear that the bms is working perfectly fine for you :-) Do the bms needs to be turned on via E-switch, when charging or ?

And oh, what charger are you using ?
```

---
## \#211 Posted by: rich Posted at: 2017-07-19T19:01:05.520Z Reads: 374

```
[quote="Namasaki, post:208, topic:10014"]
The other advantages of discharging through the bms are short circuit protection
[/quote]

Sorry for this stupid question (i'm no electician) but shouldn't a fuse with the same amount of ampere as BMS max doing the same job (beside the fact that the fuse has to be changed afterwards)?
But maybe the BMS is much faster...

I don't have bestec, i have other brand 10s 60A cont./120A max. But this is charging/discharging on different ports where i'm afraid to use it because of regenerative braking. That's why i ordered the same BMS with charging/discharging at the same port which i'll use for my Li-ion pack (build not finished).

I have a second build just finished (MTB with 10s 10Ah Lipo) and you make me wanna use BMS now :wink:
[quote="Namasaki, post:208, topic:10014"]
bms protects against overcharging though regen braking
[/quote]

well that's a good point

Right now i have a cheap bypassed BMS for charging only.
I'm afraid to use my "proper" BMS and send energy back to the discharge port...

[quote="Namasaki, post:208, topic:10014"]
I try not to run my battery lower than 36v
[/quote]

I try it too but when i ride i always forget to watch the voltage. Some days ago i was riding my MTB in the middle of nowhere in the night when my vescs let me know that i've reached 0% (32V) :joy: It was a long way back.....
```

---
## \#212 Posted by: Namasaki Posted at: 2017-07-19T23:33:13.631Z Reads: 382

```
[quote="Silverline, post:210, topic:10014"]
Do the bms needs to be turned on via E-switch, when charging or ?

And oh, what charger are you using ?
[/quote]


Yes, the bms E-switch has to be on during charging.
I have a Battery Supports 5a brick charger for mobile charging and at home I use a CC/CV Lab Power supply to charge.
<img src="/uploads/db1493/original/3X/4/2/4235fbec695102595e74951817d8b9fa603d71d2.jpeg" width="666" height="500">
```

---
## \#213 Posted by: Namasaki Posted at: 2017-07-19T23:47:23.684Z Reads: 364

```
The Bestech bms also has a separate C- (charge only) pad. Still it handles Regen charging coming in through the P-(output) pad.

I recommend locating your voltage meter on top of your board or through the deck so you can monitor your battery while riding.
The BMS over discharge protection should be used as a protection against extreme cell drift and not as a first line defense  or as a fuel gauge.
I also recommend using a voltage readout instead of a percentage readout since that can be deceiving and the voltage is what really matters.
```

---
## \#214 Posted by: Silverline Posted at: 2017-07-20T04:19:44.150Z Reads: 349

```
So the esc's / vesc is on when charging ?


And how kan you se on your lap power supply , when the charge is ready ? The Amp draw in the display shows 0 ? Or
```

---
## \#215 Posted by: Namasaki Posted at: 2017-07-20T04:42:51.146Z Reads: 351

```
The vesc's are on while charging. I don't have a problem with that although a loop key would solve it.
The power supply starts out giving 5a with a voltage a little higher than the battery's current voltage and slowly raises the voltage as the battery charges. This is CC mode and it prevents heating of the cells during charge.
Once the voltage reaches the finish voltage that is set, say 42v the power supply automatically switches to CV mode and the current starts reducing as the battery fills. Theoretically, the current will drop to zero when the battery is full.
I usually stop charging when it gets down around 50ma but since the bms trims the high cells at the rate of 126ma, it seems feasible to let the power supply trickle charge at 50ma and continue to fill low cells while the bms trims the higher cells.
```

---
## \#216 Posted by: rich Posted at: 2017-07-20T07:49:50.856Z Reads: 357

```
[quote="Namasaki, post:213, topic:10014"]
I recommend locating your voltage meter on top of your board
[/quote]


True that's important! That's why i have voltage meter and percentage with backlight top mounted, i just have to look down. But my MTB build is brand new i'm too excited to watch the battery level :joy:. But after my experience i have to change my behaviour.

[quote="Namasaki, post:213, topic:10014"]
The Bestech bms also has a separate C- (charge only) pad. Still it handles Regen charging coming in through the P-(output) pad.
[/quote]

That makes me hope, i think i'll give it a try. But in this case i gonna use the BMS with different ports for Li-ion pack (10s4p charging max. 16A) and the BMS with same ports and charging max. of 60A for my Lipo pack (10s charging max 50A) where i need stronger brakes anyway (MTB).

Do you think an additional fuse is needed when using BMS for discharge as safety?

Many thanks for your help! :grinning:
```

---
## \#217 Posted by: lrdesigns Posted at: 2017-07-20T07:55:35.126Z Reads: 333

```
How many cycles do you think you have put on the pack so far? 
I'm building one similar but 12s and wondering if its worth getting the more expensive packs like nanotech or graphene? They advertise higher charge rates upto 15c and I like to run high regen battery amps. Currently I am running 25 amps on regen but I dont have a logger to know how many amps the system is actually generating during braking. But I wonder if it really matters as its only for a few seconds, its not like your charging the pack from empty at 5c which you would expect it to get warm if you did that?
```

---
## \#218 Posted by: Silverline Posted at: 2017-07-20T08:02:10.375Z Reads: 328

```
On Power Hungry racing quads (mines pull over 100amp on full throttle) Graphene batteries are one of the best batteries to take the abuse. But they are also heavier and bigger. And in a board with less apm pulls, i dont know if graphene is overrated.
```

---
## \#219 Posted by: twan Posted at: 2017-07-20T08:08:39.310Z Reads: 328

```
@Namasaki What button are you using and battery meter on your board? it looks nice!
```

---
## \#220 Posted by: Namasaki Posted at: 2017-07-20T11:58:23.872Z Reads: 354

```
[quote="rich, post:216, topic:10014"]
Do you think an additional fuse is needed when using BMS for discharge as safety?
[/quote]

You don't need a fuse when discharging through the bms because:
1. The bms acts like a circuit breaker that is easily reset by the e-switch in the event of a short. 
2. The Vesc controls current.
```

---
## \#221 Posted by: Namasaki Posted at: 2017-07-20T14:31:46.293Z Reads: 366

```
https://www.amazon.com/dp/B00YS25ZEM/ref=cm_sw_r_cp_apip_XnbbmM93RVOFt

https://www.amazon.com/dp/B00VUUKIMY/ref=cm_sw_r_cp_apip_Zo1jEHCDCf4FH
```

---
## \#222 Posted by: twan Posted at: 2017-07-22T10:08:12.503Z Reads: 360

```
How does the switch work @Namasaki?
My two white wires aren't connected together but when I measure the voltage on the P- terminal there's still a voltage . Isn't it suppose to be nothing ?
```

---
## \#223 Posted by: Namasaki Posted at: 2017-07-22T17:33:22.888Z Reads: 340

```
It will still show 2-3 volts when the bms is off. 
This is normal for the Bestech bms
```

---
## \#224 Posted by: twan Posted at: 2017-07-22T17:47:57.976Z Reads: 349

```
Dam what the heck mine shows like 38 volts :(
```

---
## \#225 Posted by: Namasaki Posted at: 2017-07-23T02:34:55.149Z Reads: 347

```
Do you have the Vescs connected
```

---
## \#226 Posted by: twan Posted at: 2017-07-23T02:48:07.103Z Reads: 364

```
Noo I didnt connect it yet. Does it matter if its connected? This is how it's all currently connected  

<img src="/uploads/db1493/original/3X/4/e/4e3ad684234e0e3f57ee08fc957dc22dec5b8033.JPG" width="375" height="500">
```

---
## \#227 Posted by: flywithgriff Posted at: 2017-07-23T02:52:43.528Z Reads: 343

```
@Namasaki how do you think this would do on a MTB build?
```

---
## \#228 Posted by: Namasaki Posted at: 2017-07-23T04:11:21.037Z Reads: 337

```
Yes it matters, you need a load to drain the voltage down when you turn the bms off.
several others have done the same test as you with the same results. As soon as they connected a load to the output of the bms, it worked correctly.
```

---
## \#229 Posted by: Namasaki Posted at: 2017-07-23T04:12:58.095Z Reads: 337

```
this setup supplies plenty of power with minimum voltage sag so it should perform well on a mountain board.
Range will likely only be 10-12 miles though.
```

---
## \#230 Posted by: twan Posted at: 2017-07-23T04:23:44.104Z Reads: 336

```
ah i just tried it, fixed the problem. thanks so much!
```

---
## \#231 Posted by: flywithgriff Posted at: 2017-07-23T13:18:16.539Z Reads: 337

```
What if I used 4x 3s 8000mah 30c?
```

---
## \#232 Posted by: Namasaki Posted at: 2017-07-23T16:10:09.208Z Reads: 330

```
12s / 8ah
More range, power and top speed
```

---
## \#233 Posted by: flywithgriff Posted at: 2017-07-23T16:45:27.447Z Reads: 328

```
And if i were to do two of those and then wire together that would be 12s 16ah correct?
```

---
## \#234 Posted by: Namasaki Posted at: 2017-07-23T17:44:29.688Z Reads: 330

```
Yes but those packs ar big and heavy. 
For me, the extra range would not be worth  the extra bulk and weight.
```

---
## \#235 Posted by: flywithgriff Posted at: 2017-07-23T17:45:44.217Z Reads: 326

```
I just want a MTB build with a range of at least 15 miles.
```

---
## \#236 Posted by: Namasaki Posted at: 2017-07-23T18:16:05.190Z Reads: 327

```
I think you will exceed 15 miles with 12s/8ah
You might even see up to 20 miles riding flat ground
```

---
## \#237 Posted by: flywithgriff Posted at: 2017-07-23T18:24:48.432Z Reads: 334

```
I can find these batteries but the C rating is only like 10 or 15.
```

---
## \#238 Posted by: Namasaki Posted at: 2017-07-23T21:10:14.573Z Reads: 330

```
10-15C won't cut it in IMO
I would not go below 30C
```

---
## \#239 Posted by: flywithgriff Posted at: 2017-07-23T21:11:34.587Z Reads: 328

```
thats what I was thinking. Trying to find higher rated batteries now.
```

---
## \#240 Posted by: flywithgriff Posted at: 2017-07-26T13:25:16.977Z Reads: 329

```
Am I right in thinking that 5 x 2s 5ah 30c is a 10s1p. But the same setup again but wired together with original setup in parallel would be a 10s2p and should double range?
```

---
## \#241 Posted by: Namasaki Posted at: 2017-07-26T13:34:17.581Z Reads: 330

```
Yes, it would be 10s2p and it should double range and current capability and reduce voltage sag even more.
```

---
## \#242 Posted by: hornet90 Posted at: 2017-07-29T08:01:13.560Z Reads: 330

```
just wanted to say thanks to Namaski for all your help........
```

---
## \#243 Posted by: Moav Posted at: 2017-08-03T06:41:49.638Z Reads: 311

```
What kind of power supply should I need for 5S2P X2 in series with a 10A chrage? 42V 20A?
```

---
## \#244 Posted by: willpark16 Posted at: 2017-08-03T07:08:34.526Z Reads: 312

```
2-5a should suffice I recommend 2a for cell longevity
```

---
## \#245 Posted by: Moav Posted at: 2017-08-03T09:45:41.288Z Reads: 317

```
OK then I'll get lower ampere, but is it 42V? same voltage as the full state of battery? Or could I get a lower V one?
```

---
## \#246 Posted by: Namasaki Posted at: 2017-08-03T11:00:31.360Z Reads: 323

```
You want to match full voltage either charge
5s2p is not 42v though
```

---
## \#247 Posted by: Moav Posted at: 2017-08-03T11:22:32.780Z Reads: 328

```
What I meant is, as I wasn't clear, that there are 4 packs, 2X 5S in series and those two are in parallel to other 2 packs. So 42V ?
```

---
## \#248 Posted by: Namasaki Posted at: 2017-08-03T11:57:32.286Z Reads: 333

```
Ok, that would be a 10s2p and 42v charge. 
Power supplies come either 30v max or 60v max so you'll need a 60v power supply with CC/CV output. 
A 60v 10a  CC/CV power supply would be very expensive. I recommend a 60v 5a which is what I use and it works just fine.
```

---
## \#249 Posted by: Moav Posted at: 2017-08-03T13:02:54.670Z Reads: 338

```
https://www.aliexpress.com/item/Power-Supply-DC-60V-17A-1000W-Switching-Switch-Driver-Transformer-110V-220V-AC-DC60V-SMPS-For/32706061501.html?spm=2114.search0104.3.42.mSbvTe&ws_ab_test=searchweb0_0,searchweb201602_1_10152_10065_10151_10068_10172_10084_10083_10080_10307_10082_10081_10110_10137_10111_10060_10112_10113_10155_10114_10154_10056_10055_10054_10312_10313_10059_10314_10315_100031_10099_10078_10079_10103_10073_10102_10052_10053_10142_10107_10050_10051-10050_10152_10111normal#cfs,searchweb201603_2,ppcSwitch_2&btsid=e3ce1ede-a38b-4a67-8378-be5d06fa1eb5&algo_expid=31be34c5-f35d-466b-b27f-f3b550b26dcd-5&algo_pvid=31be34c5-f35d-466b-b27f-f3b550b26dcd&transAbTest=ae803_1

Is this considered expansive? Or should I stay away from those products at that price point?
```

---
## \#250 Posted by: Namasaki Posted at: 2017-08-03T13:40:00.127Z Reads: 338

```
That's the wrong type of power supply. 


This is what I use. 
Adjustable voltage and current. 
Constant Current/Constant Voltage
https://www.amazon.com/dp/B00G0HAY3U/ref=cm_sw_r_cp_apip_gVQX1iuDemiIz
```

---
## \#251 Posted by: stanl3yy Posted at: 2017-08-03T14:56:09.491Z Reads: 329

```
I use this one for my 10s battery pack:

https://aliexpress.com/item/36V-5A-charger-Output-42V-5A-aluminum-case-charger-Used-for-36V-battery-charging-Hight-Power/1731025899.html
```

---
## \#252 Posted by: Moav Posted at: 2017-08-04T13:19:53.908Z Reads: 322

```
Thank you both, but Stan won for the competitive pricing :slight_smile:

I'm considering charging them in series, I was thinking about making a switch, or perhaps using my anti spark switch if possible to manipulate batteries status from parallel to series. Much like this switch: http://www.instructables.com/id/SIMPLE-ParallelSeries-Select-Switch/

What do you guys think?
```

---
## \#253 Posted by: Moav Posted at: 2017-08-07T10:26:05.049Z Reads: 309

```
Please guys, I need to know if it makes sense so I can purchase the correcr BMS, should I go with 10S BMS and parallel charge or 20S with a higher voltage PSU and a switch, is it safe?
```

---
## \#254 Posted by: Namasaki Posted at: 2017-08-07T12:22:07.502Z Reads: 307

```
[quote="Moav, post:252, topic:10014"]
What do you guys think?
[/quote]

I think a switch like that won't last 1 day if you switch it under power.
```

---
## \#255 Posted by: Namasaki Posted at: 2017-08-07T12:24:08.376Z Reads: 301

```
[quote="Moav, post:253, topic:10014"]
should I go with 10S BMS and parallel charge or 20S with a higher
[/quote]
 12s is the limit for the motors and controllers that we use.
```

---
## \#256 Posted by: Moav Posted at: 2017-08-07T16:03:59.544Z Reads: 293

```
Maybe I didn't explain myself as well as I wanted. This switch is ONLY after I disconnect the batteries from the motors (powering down the system), and it is only for charging, not to be consumed by the motors. A fail safe mechanism may be in order. 10S in parallel when riding, 20S when charging.
```

---
## \#257 Posted by: Namasaki Posted at: 2017-08-07T16:25:49.556Z Reads: 287

```
How do you purpose to balance charge a 20s battery?
```

---
## \#258 Posted by: Moav Posted at: 2017-08-07T20:04:38.048Z Reads: 285

```
With a 20S BMS. It was proposed by Lucy from Bestech.
```

---
## \#259 Posted by: Namasaki Posted at: 2017-08-07T21:13:04.642Z Reads: 286

```
So your going to connect the bms to charge and disconnect it to ride ?
```

---
## \#260 Posted by: Moav Posted at: 2017-08-08T05:41:26.994Z Reads: 294

```
I didn't think about that, you are right, I'd need to disconnect the BMS before powering up the system.
```

---
## \#261 Posted by: Crossfire Posted at: 2017-08-10T09:35:06.723Z Reads: 299

```
For parallel charging the lipos the best and most effective way is to use a nice charger and a good, beefy PSU.
I use the ISDT SC620, 20A charger and a ex-server 500W PSU (small, light and around 40A@12V charging capabilities).
I can charge 2x 4S 5000 mAh in under 30 minutes from like 3.7V per cell to full charge at 4.2V - that's in parallel @ 10A. In case of 3x 4S 5000 mAh setup I'll just ramp the amps up to 15A and get the same charging time.
It's gold.
```

---
## \#262 Posted by: Namasaki Posted at: 2017-08-10T12:31:57.008Z Reads: 298

```
The popular belief is that it's not good to fast charge lithium batteries, especially Lipos.
```

---
## \#263 Posted by: Crossfire Posted at: 2017-08-10T12:57:31.596Z Reads: 302

```
Charging at 1C is not fast charging it's the proper way of charging lipos. 1C for 5000 mAh is 5A while for 2x 5000mAh lipos in parallel is 10A.

I have some experience in FPV and drone racing so I'm quite familiar with proper lipo care and maintainence.
Oscar did a great writeup on parallel charging here: https://oscarliang.com/parallel-charging-multiple-lipo/
Also: https://rogershobbycenter.com/lipoguide/

I've never discharge them below 3.6V per cell. You could feel the difference with drones when the cell voltage fell below 3.8V almost instanly. Between 3.6 and 3.7 they were getting really sluggish. That was a clear sign for a battery change. 
I'm holding to the same habits here in the esk8 hobby as well. 3.7V is preferably the lowest point one should go, 3.6V being a rare exception. Going lower will degrade the performance and can cause bigger risks of damaging the cell...which will over time inflate or even be prone to catch fire. I store my lipos @3.8V per cell.
```

---
## \#264 Posted by: Namasaki Posted at: 2017-08-10T13:23:54.139Z Reads: 285

```
Your right, I wasn't considering the double capacity. 
And I agree with you on the discharge. 
I do my best to not go below 3.6v
```

---
## \#265 Posted by: SilentException Posted at: 2017-08-10T13:37:59.705Z Reads: 288

```
I used to charge my 3S drone packs with 2C without any issues whatsoever. Then I f*ed up (2 times actually) and did a deep discharge to around 2.8-3V. The cells started to puff right after that.

It was similar with my first esk8 build where I was foolish enough to count on the ESC to do a cut-off. But I never even had a chance to charge those (brand new) batteries more than once. The board stopped but it wasn't the ESC. The batteries were at 2V :scream: I've managed to recover the packs but they are quite puffed now and had to remove 2 cells after few more charges because they died.

In my experience, it is the discharge that kills it.  Fast charge away, ain't noone got the time to wait for a ride :) I only slow charge at night.
```

---
## \#266 Posted by: Namasaki Posted at: 2017-08-10T13:44:12.395Z Reads: 276

```
I agree, discharging Lipos to minimum voltage is the worst thing you can do.
```

---
## \#267 Posted by: Crossfire Posted at: 2017-08-10T13:52:17.222Z Reads: 290

```
Exactly ;)
I look at the charging situation like this: we're in a year 2017 and we utilize 2-5A chargers for BMS to fully charge our esk8 in like 3-4 hours? Even electric cars can be charged up quicker...and have times bigger batteries.
Because "it's more convenient" to hook up the board to a charger and then wait 3 hours. I disconnect the batteries in series, connect them in parallel and hook it up to my charger. 1-2 min of work tops. 28 minutes later I'm riding again. 
And if I for example keep another two packs of 2x4S 5000mAh charged (1 hour of charging time for both together) I drop them in my lipo safe bag and then in my backpack and off I go. And when my Drok shows around 65% of charge after like 12km I know I'm close to 3.7 - 3.8 V per cell. I swap the lipos and that way I can theoretically ride for 3x12km and I'm being very, very conservative with my batteries on a single motor setup. That's almost 40 km of range @ around 15km/h average (we have below average quality of asphalt on the city bike trails).
```

---
## \#268 Posted by: oct0f1sh Posted at: 2017-08-11T17:39:00.007Z Reads: 270

```
Would it make any sense to get 5 of these https://hobbyking.com/en_us/zippy-6000mah-2s2p-50c-hardcase-pack.html instead of the 2S1P packs that you linked? I live in San Francisco and I need something that can handle climbing hills while still having a decent range.
```

---
## \#269 Posted by: GunnarK Posted at: 2017-08-11T17:53:58.592Z Reads: 273

```
Somewhere in this forum @Namasaki talks about this. Saying that it's unwise to go for a 2p pack since balancing the cells of such battery is not completely accurate.
Why?
Because the cells are packed as groups of 2, meaning the balancer sees two cells as one cell.
```

---
## \#270 Posted by: GunnarK Posted at: 2017-08-11T17:56:30.596Z Reads: 279

```
Hi @Namasaki
Just to have an understanding of how to use lipos with a BMS.
When you buy 5 fresh 2s lipos for your 10s build. Do you first have to balance every battery individually using a lipo balancing charger?
Or can you just install all 5 and hook them up to the BMS and let him do the job?
```

---
## \#271 Posted by: Lionpuncher Posted at: 2017-08-11T18:12:59.395Z Reads: 273

```
 @Namasaki is there any ratings I have to be aware of for the E-switch? I have that BMS, can I use the illuminated push button switch that came with my SPS switch?
```

---
## \#272 Posted by: MontPierre Posted at: 2017-08-11T18:15:22.977Z Reads: 267

```
@Namasaki My 10S BMS from Bestech has overcharge protection of 4.28V - as you have same model do you think I can let it charge to this number or keep an eye on voltage meter and disconnect it at around 4.1V? In specs it's says Balance charge 4.2V - does it mean it will start balancing at this voltage only ?
```

---
## \#273 Posted by: Namasaki Posted at: 2017-08-11T20:57:03.523Z Reads: 268

```
You can use any on/off switch. 
Although the bms will not light a lighted switch
```

---
## \#274 Posted by: SilentException Posted at: 2017-08-11T21:13:11.092Z Reads: 282

```
You could always connect the LED on the switch using different ways:

- connect LED pins to the BMS outputs with a resistor in series. Calculate resistor value like this:
R=Vin-2V/I, where Vin is your battery voltage, I is 0.02A
And use closest resistor you can find to the calculated value. You don't have to be extra accurate about it. For example, using 10S pack it would be like R=40-2/0.02=1900Ohm which means 1.8kOhm or 2.2kOhm resistor.

- connect LED to the ESC or receiver 5V outputs. Calculate resistor values using same formula, but use 5V as Vin. Depending on the LED type, it might not light up on 5V. Test it on the bench :)
```

---
## \#275 Posted by: Namasaki Posted at: 2017-08-11T21:13:59.231Z Reads: 272

```
The overcharge protection is set at 4.28 by default to allow some headroom.  Balancing starts at 4.2v
If your cells drift during discharge and then if you undercharge them, the bms will not balance them. 
If you continue this way so that your cells drift too far out of balance, your battery could reach a point where it will not fully charge and the bms will not be able to balance the cells. 
How the bms works is like this:
When your pack reaches 42v and the charger stops charging (green light) the bms will then trim down the highest cells to balance them with the lowest cells ending up with a total voltage below 42v
How much under will depend on how well matched your cells are and how evenly they charge and discharge.
The more balanced and matched(internal resistance) your cells are, the closer you will be to 42v
```

---
## \#276 Posted by: Silverline Posted at: 2017-08-11T21:16:06.825Z Reads: 255

```
How do a charger with only plus and minus connected to the bms/batteries, knows when the batteries is fully charged, and turn on green led ??
```

---
## \#277 Posted by: MontPierre Posted at: 2017-08-11T21:21:35.930Z Reads: 252

```
Thanks! By trimming you mean that BMS will discharged highest cell, voltage then will drop below 42V, charger will come on again to top up missing voltage ( of the lowest cell ?) until all are balanced?
```

---
## \#278 Posted by: SilentException Posted at: 2017-08-11T21:22:29.084Z Reads: 249

```
Chargers do what is called constant current / constant voltage charge.
If empty battery is connected it will start charging using pre set constant current. The battery voltage will slowly rise as the battery charges. When the charger voltage level is reached, it will slowly reduce current and it will go into the constant voltage mode meaning it is charged.
```

---
## \#279 Posted by: Namasaki Posted at: 2017-08-11T21:23:53.580Z Reads: 253

```
I'm glad you asked. 
Voltage is like pressure
Current is like flow 
If the voltage (pressure)  from your charger is greater than the voltage (pressure)in your battery.
The voltage will continue to flow into the battery. 
Once the voltage in the battery is equal to the voltage from the charger then the flow stops because the pressure is equal. 
The the flow stops the green light comes on
```

---
## \#280 Posted by: Namasaki Posted at: 2017-08-11T21:26:40.385Z Reads: 258

```
Yes but best to remove the charger, let the cells balance down and then put the charger back on to fill it up again. 
Better yet though is to leave it below 42v
Bestech designed it that way to help prolong battery life
```

---
## \#281 Posted by: Silverline Posted at: 2017-08-11T21:27:19.532Z Reads: 259

```
So lets say i have a 10s setup. Then when i connect my Charger , it can feel that the voltage is under 42v ? So when it starts to charge , it's start with lower voltage than 42v ? Or starts in 42v, and can feel when the battery level is the same ?
```

---
## \#282 Posted by: Dariks Posted at: 2017-08-11T21:33:44.942Z Reads: 255

```
Hi are you running a hub setup? If not I'm not sure if the batteries will help as much as you would like. Also what esc are you using the vesc tops out at 60amps with cooling.
```

---
## \#283 Posted by: MontPierre Posted at: 2017-08-11T21:37:54.789Z Reads: 250

```
So I can also leave it on and it will do the magic? I guess it wouldn't damage cells - current will be very low at the stage of trimming and balancing. I was under impression BMS is a full package and won't have to be disconnected and connected again after full charge. 

How would I know when cells are balanced ( BMS doesn't have any LEDs) since charge will have green light on even before balancing is finished?
```

---
## \#284 Posted by: Namasaki Posted at: 2017-08-11T21:38:15.652Z Reads: 260

```
I use a lab power supply to charge my batteries. 
It starts in CC mode and continues to raise the voltage keeping it just enough above the battery's voltage for the electrons to flow into the battery. 
Once the power supply reaches the max voltage that I set (42v) it then switches to CV mode. At this point the battery is usually around 41.5v
Then as the voltage in the battery becomes more and more equal to the voltage from the power supply the flow of electrons (current) gradually decreases until the voltage (pressure) in the battery is equal to the voltage(pressure) coming from the power supply. 
I can't say if a $12 charger works the same way or not. 
It would be easy to find out with a volt meter on the output of the charger while charging the battery
```

---
## \#285 Posted by: Namasaki Posted at: 2017-08-11T21:41:05.663Z Reads: 253

```
You'll know the battery is balanced when the total voltage stops dropping
```

---
## \#286 Posted by: SilentException Posted at: 2017-08-11T21:41:57.951Z Reads: 256

```
Yes, it can "feel" it, if you want to put it like that. During CC mode, the voltage will rise as the battery voltage rises, linearly.
Check this page out, third graph.
https://endless-sphere.com/w/index.php/Charging_Lithium_Polymer_batteries
```

---
## \#287 Posted by: MontPierre Posted at: 2017-08-11T21:45:17.234Z Reads: 251

```
How can I tell it is balanced by using "Brick" 42V 5A charger with LED? It doesn't display voltage ... Well I have voltage meter attached to the board ... but I guess I would have to look at it for some time so catch voltage drop. I guess I can't just rely on Green LED on the brick right?
```

---
## \#288 Posted by: Silverline Posted at: 2017-08-11T21:51:30.034Z Reads: 256

```
Thanks guys ...

So in princip. I could charge my 10s pack without a BMS, and my Charger would still show green LED, when the pack have reached 42v (given that without my BMS, the cells would not be in ballance to each other)
```

---
## \#289 Posted by: MontPierre Posted at: 2017-08-11T22:10:59.965Z Reads: 292

```
I have latching LED switch which I would like to disconnect it from Vedder anti spark and connect it to built in Bestech BMS switch to save on space in my enclosure. Here are the schematics of this model.


<img src="/uploads/db1493/original/3X/4/4/44b4e4329a2634eefb4fda953adfa4fb84fd9217.jpg" width="690" height="428">


Based on above is my below connection diagram correct? Switch is rated for 6/12/24 V and max of 3A so might be slightly dimmer than at 6V ( I will bench test it later). I want it to light up when pressed. 

<img src="/uploads/db1493/original/3X/2/9/2937c9f30efcb1e6687883e731cf99f23d0ce508.jpg" width="690" height="381">

I think it looks fine @SilentException... what do you think?
```

---
## \#290 Posted by: SilentException Posted at: 2017-08-11T22:32:15.734Z Reads: 270

```
Yes but you don't want that. Why? Well let's say one parallel group or cell in the series pack is "bad" and it is out of balance. Example of 3S pack:
4.0V 3.8V 4.0V
Charger will charge until pack gets at 12.6V and at this point the pack will be something like:
4.3V 4.0V 4.3V = 12.6V
Some of the cells will be overcharged, not a good idea.
```

---
## \#291 Posted by: SilentException Posted at: 2017-08-11T22:32:31.958Z Reads: 268

```
Momentary switch..not going to work :) You need latching one.
```

---
## \#292 Posted by: MontPierre Posted at: 2017-08-11T22:34:55.938Z Reads: 270

```
I'm sorry, it is latching switch. Not sure why I wrote momentary. It must have been 12hrs shift I have just finished at work :) Would wiring be correct?
```

---
## \#293 Posted by: Silverline Posted at: 2017-08-11T22:35:46.592Z Reads: 291

```
I know. I would never do that. It was just to help me understand how the Charger Works, and how it 'sees' the battery. 
I got it now..
```

---
## \#294 Posted by: SilentException Posted at: 2017-08-11T22:54:07.992Z Reads: 313

```
God, no. I think you might burn something using those connections. Just use a switch part as a switch and LED part as a LED. Simple :)

<img src="/uploads/db1493/original/3X/f/8/f8aeef1109a990c9895b088ff76d1775c48cf9b6.jpg" width="375" height="500">
```

---
## \#295 Posted by: MontPierre Posted at: 2017-08-11T23:08:07.542Z Reads: 287

```
@SilentException Ohh silly me. So + and - on the latching switch are for LED voltage and NO ( normally open) and C ( common) are for the switch! Makes sense :) 

I guess resistor won't be needed - LED can take 3A max and 5V on Vesc is I think 1A max. Thanks!
```

---
## \#296 Posted by: SilentException Posted at: 2017-08-11T23:36:21.813Z Reads: 286

```
[quote="MontPierre, post:295, topic:10014"]
I guess resistor won't be needed - LED can take 3A max and 5V on Vesc is I think 1A max.
[/quote]

This sounds very implausible to me. You might be looking at switch rating and not the LED.
```

---
## \#297 Posted by: Namasaki Posted at: 2017-08-11T23:54:34.709Z Reads: 316

```
Green and blue to E-switch
Red and black to open channel on receiver for 5v


<img src="/uploads/db1493/original/3X/0/c/0cbd6036b0697298afb9e4086690b2fc9eb5bef9.jpg" width="690" height="387"><img src="/uploads/db1493/original/3X/a/9/a9b1d564e6a5f7285ffa319196219542b60b190c.jpg" width="281" height="499">

<img src="/uploads/db1493/original/3X/a/7/a757d4eaf0348f88996de8cd9489b3fb14a28a05.jpg" width="375" height="500">
```

---
## \#298 Posted by: Namasaki Posted at: 2017-08-12T00:06:50.545Z Reads: 316

```
Here is example if charging with CC/CV power supply and bms. 
<img src="/uploads/db1493/original/3X/4/a/4a351effd7978cd44390d721952a82a40c60cbfb.JPG" width="357" height="500"><img src="/uploads/db1493/original/3X/e/b/eb7763c7b14ad7ae546831a09be8cfb88eeb4e9f.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/0/c/0c4b03270a498473330813419f985c8a3a49acdd.JPG" width="374" height="500"><img src="/uploads/db1493/original/3X/b/0/b018fdb798d97e92b3a793c1c4aa43a8795d7be8.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/3/a/3a55538baf16df9bbb449cae347e4400b6f896d5.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/0/9/098f89d18c524e1536e8ab81255a7a224e23e37e.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/1/2/12d8e9af237b3603988df30e7d544cbd54061a82.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/5/f/5fc07a76eeb78259afc9f5cd446ff513f1d21469.JPG" width="375" height="500">
```

---
## \#299 Posted by: Namasaki Posted at: 2017-08-13T01:43:48.575Z Reads: 296

```
[quote="GunnarK, post:270, topic:10014"]
Just to have an understanding of how to use lipos with a BMS.
When you buy 5 fresh 2s lipos for your 10s build. Do you first have to balance every battery individually using a lipo balancing charger?
Or can you just install all 5 and hook them up to the BMS and let him do the job?
[/quote]

Sorry for the late reply.
It would be best to balance the packs before assembling them but if you don't have a hobby charger, then you can get around that as long as all packs are close to the same charge.
I once experienced a problem when I had to replace a pack who's main power cable came loose inside the case.
the new battery was at storage charge and the rest of the pack was somewhere over 4.0v per cell.
In that case the charger stopped before the total pack voltage could reach 42v so the bms balancing was not triggered.
I had to go in and charge the new pack separately to equalize it with the rest of the battery. After that everything was fine.
Frankly, I don't know of any BMS that can balance cells as well as  a good hobby charger can.
```

---
## \#300 Posted by: GunnarK Posted at: 2017-08-13T08:51:15.353Z Reads: 287

```
Thanks for your response!
What margin would be acceptable for the cells?
What voltage is common for 'storage charge'?
```

---
## \#301 Posted by: Namasaki Posted at: 2017-08-13T09:03:46.256Z Reads: 286

```
according to my hobby charger, 3.8v per cell is storage charge.
as far as the maximum acceptable margin for the bms, I really don't have any hard numbers for sure but my best guess is no more than 0.1v per cell.
```

---
## \#302 Posted by: GunnarK Posted at: 2017-08-13T10:51:18.565Z Reads: 281

```
Ok I'll have a look at my batteries when I get them in. If any doubt I'll contact you here in this topic with my measurements, maybe then we can see what is ok as a margin!
Thanks!
This is a really nice topic full of very useful information
```

---
## \#303 Posted by: WawiKirsinger Posted at: 2017-08-30T20:54:38.003Z Reads: 274

```
[quote="Namasaki, post:41, topic:10014"]
The switch is useless but the charge port works fine.
[/quote]

why this switch is useless? the BMS has the E-switch built-in.... i dont understand that :)
```

---
## \#304 Posted by: Namasaki Posted at: 2017-08-31T00:32:01.959Z Reads: 283

```
The electronics for the E-switch are built into the bms. There are 2 wires coming from the bms that have to be connected to a physical on/off switch.

The switch that comes with the charge port is useless because it is a momentary switch, not an on/off switch.
```

---
## \#305 Posted by: mptrs Posted at: 2017-09-16T13:08:29.014Z Reads: 299

```
@Namasaki you helped me out allot so I have another question for you (other may also help, no problem haha).

Is this gonna work or am I going to destroy everything :smile: 

 <img src="/uploads/db1493/original/3X/4/c/4c4e24b28b93dc4e088738ec6b6bad40bc81bf67.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/c/d/cd148d3bfe3290d3ed925d66f863c9ef138c3903.JPG" width="666" height="500">

I connected the BMS to the charger, this way I didn't need to fit it into my board. Connected the C- to the charger -. And the B- is going out the the charger port, so to the - of the lipo. Got the eswitch connected to a simple on/off switch, the one with just two poles, to be able to switch it on and off.
I just need to connect the balance wires, but that something that's always necessary.
There is an anti-spark and switch between the VESC and the lipo's so in theory with the board off there will be no power from the charger that goes to the VESC. Which should make it extra save for the VESC.

This should work, but I haven't seen this before so I just wanted to check. I might have missed something important that ill blow everything up :joy:
```

---
## \#306 Posted by: Namasaki Posted at: 2017-09-16T18:06:06.838Z Reads: 276

```
I can't tell much by the picture. 
Make a diagram and post it and I'll take a look
```

---
## \#307 Posted by: mptrs Posted at: 2017-09-16T19:04:17.959Z Reads: 286

```
In short it's like the image. Only thing missing from the image to keep it simple is the charger port and socket. And the part where the wire from the lipo goes to the anti-spark. (which are coming from the same connector as the wires the charge port uses)

When looking at the diagram I noticed there is nothing different from wiring it directly to the lipo except for the P- not being used. Which in this case is not needed.

<img src="/uploads/db1493/original/3X/c/d/cd04d1111f403f23a098d9e2d06dbc195f7a375f.JPG" width="375" height="500">
```

---
## \#308 Posted by: Namasaki Posted at: 2017-09-16T21:01:54.523Z Reads: 268

```
I need to see everything in the diagram or else I can't say it's good or not. 
And are you bypassing discharge?
And if yes, why bypass with an 80a bms ?
```

---
## \#309 Posted by: mptrs Posted at: 2017-09-16T21:12:29.705Z Reads: 291

```
Ok added the missing pieces.

And I'm not sure what you mean by bypassing discharge. I'm just taking the BMS out off the board and 'into' the charger. (lipo balance wires will be connected to the BMS, but not drawn, BMS has an e-switch)

<img src="/uploads/db1493/original/3X/f/1/f151e47ace4695365de03c406897d9fbfc0875c7.jpg" width="666" height="500">
```

---
## \#310 Posted by: Namasaki Posted at: 2017-09-17T02:04:13.584Z Reads: 282

```
I've never seen a bms used this way but I guess it will work for charging although you will have to have the bms e-switch on while charging and you will need to keep it connected and on after charging to balance the battery
```

---
## \#311 Posted by: mptrs Posted at: 2017-09-17T09:28:21.927Z Reads: 282

```
Yeah that's the problem, I've never seen it before either hehe. But this will save quite some space.

Did some testing and the power is not cut by the e-switch (that's what you meant)
So I think it doesn't need a switch, I can just connect the wires permanently to prevent errors.

Need to print a small enclosure and than I'll use it on my lipos :hushed:

Thanks for the help again.
```

---
## \#312 Posted by: Namasaki Posted at: 2017-09-17T11:56:11.775Z Reads: 260

```
That bms has to be switched on for charging so you will need to connect a switch to it.
```

---
## \#313 Posted by: mptrs Posted at: 2017-09-17T15:57:34.532Z Reads: 262

```
If the wires are always connected it's the same as a switch that is on right? Don't think it knows there is a switch. The circuit is either complete or interrupted, right?
```

---
## \#314 Posted by: Namasaki Posted at: 2017-09-17T16:05:03.081Z Reads: 258

```
You need to be able to turn it off before disconnecting it from the battery. 
And turn it on after the battery is connected.
So you need a switch.
```

---
## \#315 Posted by: mptrs Posted at: 2017-09-17T18:29:59.198Z Reads: 262

```
I will connect the battery before switching on the whole contraption. And pull the plug when everything is recharged.

Still need a switch then? I'm not really sure how the e-switch works then hehe.
```

---
## \#316 Posted by: Namasaki Posted at: 2017-09-17T21:04:35.962Z Reads: 259

```
You should turn the bms off before pulling the plug and disconnecting the balance wires.

Just connect an on/off switch to the 2 white wires.
```

---
## \#317 Posted by: bigben Posted at: 2017-09-19T06:15:40.969Z Reads: 262

```
@Namasaki 
HI, you've inspired me to go with a lipo pack. It looks like you've really looked into this and everyone owes you a great debt of gratitude!
I've plumped for these.https://hobbyking.com/en_us/graphene-5000mah-2s2p-hardcase-w-5mm-female-bullet-connector.html
They were flagged by someone as being a crazy price, what do you reckon? I think they're going to make a pretty usable pack.
Also sent over your bms info to get a quote for 2. If anyone else wants to get one from around the UK area there may be better prices to be had with more orders?
```

---
## \#318 Posted by: Namasaki Posted at: 2017-09-19T12:32:09.429Z Reads: 244

```
I heard the Graphenes are really good and the price is good deal. 
I recommend buying an extra set if you can. 
And thanks for the props
```

---
## \#319 Posted by: bigben Posted at: 2017-09-19T13:20:39.099Z Reads: 251

```
Just ordered the BMSs and two sets of batteries....(10)
Got to have your backup..!
```

---
## \#320 Posted by: Namasaki Posted at: 2017-09-19T17:41:09.196Z Reads: 257

```
Especially at that price. 
They won't be on sale later. 
Just storage charge the extras and put them away. 
I have 5 extra of the batteries that I use.
```

---
## \#321 Posted by: Mobutusan Posted at: 2017-09-19T20:27:23.109Z Reads: 265

```
So, those graphenes look like they don't need balancing and can just use a regular Lipo charger? But how would you set these up with a bms? Would it work to wire them up in series and hook up to a bms as 10s with no balance wires?
```

---
## \#322 Posted by: Namasaki Posted at: 2017-09-19T22:41:41.524Z Reads: 280

```
All lithium multi cell batteries need balance charging.
A bms will not even work if you don't connect the balance wires.
this is how you connect them.
On the graphenes, the center socket is for the cell one balance wire.
Cell 2 balance wire connects to the main positive output.
<img src="/uploads/db1493/original/3X/4/9/49a094677ff3f3637099adf547b6ec690cbeee12.png" width="664" height="500">
```

---
## \#323 Posted by: Mobutusan Posted at: 2017-09-20T01:03:42.508Z Reads: 274

```
Thanks buddy. It all makes sense now. Very helpful schematic too. I'm sooo close to buying a handful of those batteries, since they're down to $22.22/ea now. :scream: 

$111 for 185wh @ 10s with 450A cont./675A burst output + ~$40 BMS sounds pretty sweet. Even if the specs are overinflated.

https://hobbyking.com/en_us/graphene-5000mah-2s2p-hardcase-w-5mm-female-bullet-connector.html?___store=en_us
```

---
## \#324 Posted by: Namasaki Posted at: 2017-09-20T02:42:36.323Z Reads: 278

```
Although Lipo specs are over inflated, when you get them in the 60-90C range, they absolutely Rock!

My 10s 5ah pack with 60C Turnigy Lipos only sags 1/2v when accelerating on slight grades and only 1v when charging up a 10%grade and I'm 195 pounds. They don't swell, they don't overheat.

So imagine how those Graphene 90C packs will perform!!!!
Especially since Graphenes are Turnigy's most high performance battery.
The sale price is crazy. I would buy an extra set just to save for backup.
```

---
## \#325 Posted by: willpark16 Posted at: 2017-09-20T02:54:44.844Z Reads: 270

```
How much range did you get on those again?
```

---
## \#326 Posted by: mmaner Posted at: 2017-09-20T02:59:14.001Z Reads: 276

```
I get about 14 miles out if my setup, which is essentially like the @Namasaki hi-powered 10s pack other than mine are 30c cells.  I still never sag below 1v, even on pretty large grades.  

I just wanna say I wouldn't have thought of constructing a pack like that without @Namasaki doing all the leg work, and I have 2 now, so good on you brother.
```

---
## \#327 Posted by: Namasaki Posted at: 2017-09-20T03:06:49.193Z Reads: 276

```
I maxed at 14 miles on flat ground with dual 6355s,
I haven't tested max range with my 6374s
```

---
## \#328 Posted by: bigben Posted at: 2017-09-24T08:46:49.647Z Reads: 281

```
<img src="/uploads/db1493/original/3X/d/5/d53cd66a5ef1a9e7497dc80a69dc4d499af968ae.JPG" width="666" height="500">
I think these Graphenes are gonna be just fine! Thanks so much for this thread.
<img src="/uploads/db1493/original/3X/2/3/23319458bff4b4be0b24285e2245b0458856f417.JPG" width="666" height="500">
```

---
## \#329 Posted by: TunaTee Posted at: 2017-09-25T15:47:28.552Z Reads: 271

```
Hey, I love your design. Can I pm you some questions?
```

---
## \#330 Posted by: Namasaki Posted at: 2017-09-25T17:34:36.172Z Reads: 271

```
Sure
10 characters
```

---
## \#331 Posted by: TunaTee Posted at: 2017-09-25T20:48:50.505Z Reads: 277

```
I will just ask here since people might want to ask the same questions.
I might go a LITTLE bit above 10 characters lol. 
So, I am purchasing a BMS from bestech, but I still got few questions that I did not get an exact answer from the Bestech representative. 

1. http://www.ebay.com/itm/262359346829?_trksid=p2060353.m1438.l2649&ssPageName=STRK%3AMEBIDX%3AIT
For these charging ports do you have to solder the wires on to the BMS or you just plug it in?

2. I got three 3s1p 5000mah 40C LiPo, will these balance lead work for them?
NEW 12&#034; JST 2S LIPO BALANCE LEAD EXTENSION SILICONE 22awg WIRE ADAPTER...

3. For me to solder something means to let them stay on FOREVER lol. If I solder the batteries together will they be able to charge balancely with the BMS or do I have to uninstall them periodically to balance charge them?

I feel bad to ask about these dumb questions, but I went through your post twice and could not wrap my head around this. You have my gratitude.
```

---
## \#332 Posted by: Namasaki Posted at: 2017-09-25T21:20:36.747Z Reads: 267

```
[quote="TunaTee, post:331, topic:10014"]
I might go a LITTLE bit above 10 characters lol.
[/quote]


You misunderstood, I typed "10 characters" because the system requires at least 10 character for a post.
```

---
## \#333 Posted by: GrecoMan Posted at: 2017-09-25T21:22:17.198Z Reads: 265

```
LOL, @system stops you from posting if it’s below 10 characters, he wrote that so he could get over the limit
```

---
## \#334 Posted by: Namasaki Posted at: 2017-09-25T21:30:24.724Z Reads: 268

```
1: The charge port has to be soldered. The negative wire goes to the bms and the positive wire goes to the main positive of the battery.

2: 2s balance extensions will not work with 3s batteries because they have a different connector.
   2s has a 3 pin connector and 3s has a 4 pin connector

3: The bms will balance the batteries after they are fully charged by trimming the highest cells down to match the lowest cells.
If you ever needed to charge one of the 3s packs individually, you can by connecting the positive and negative charge leads of a hobby charger to the positive and negative wires of the pack you want to charge and connect the balance wires of that pack to the balance port on the hobby charger and use balance charge function. The pack your charging will be electrically isolated from the rest as far as the charge circuit is concerned. You would want to disconnect the balance leads from the bms before performing this operation. And be sure the bms is turned off.
```

---
## \#335 Posted by: TunaTee Posted at: 2017-09-26T00:53:40.900Z Reads: 250

```
lol, sorry totally noob.
```

---
## \#336 Posted by: TunaTee Posted at: 2017-09-26T00:54:20.367Z Reads: 258

```
Thanks for your prompt reply. I will look for some JST 3S balance lead. Appreciate.
```

---
## \#337 Posted by: TunaTee Posted at: 2017-09-26T13:07:15.980Z Reads: 268

```

http://www.ebay.com/itm/2-0A-42V-Charger-For-Terminator-Sting-Spirit-Freedom-959-X-Treme-X-560-E-Scooter/382095075374?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D1%26asc%3D20160908110712%26meid%3D8b5c46ba110a4a0f96b0d823a429c49f%26pid%3D100677%26rk%3D2%26rkt%3D3%26sd%3D142287772773&_trksid=p2385738.c100677.m4598
Hello, will this charger offer too low of an Amp?
```

---
## \#338 Posted by: TunaTee Posted at: 2017-09-26T16:14:17.768Z Reads: 272

```
<img src="/uploads/db1493/original/3X/6/a/6ae7592f95ee479f4e5072780973d13976cba078.JPG" width="666" height="500">
Can you please take a look at my diagram and to see if I got it right? Thank you.
```

---
## \#339 Posted by: Namasaki Posted at: 2017-09-26T16:19:48.636Z Reads: 264

```
2a charge is fine.
```

---
## \#340 Posted by: Namasaki Posted at: 2017-09-26T16:26:54.496Z Reads: 268

```
Your diagram needs more detail concerning the balance wires. Namely, you need to show the numbers of the bms balance socket and 3s batteries will have 4 balance wires. 
Bottom line. Your main connections look good but I can't tell anything about the balance wires and if you get those wrong, you'll fry the bms
```

---
## \#341 Posted by: TunaTee Posted at: 2017-09-26T16:33:56.991Z Reads: 277

```
<img src="/uploads/db1493/original/3X/d/e/de30a0d8eed929408acb6ad7e75736f7191e34da.JPG" width="666" height="500">
Like this?
```

---
## \#342 Posted by: Namasaki Posted at: 2017-09-26T20:09:39.052Z Reads: 269

```
That is not correct
```

---
## \#343 Posted by: Namasaki Posted at: 2017-09-27T00:20:40.057Z Reads: 277

```

You will need to get a 9s bms. The Bestech 10s bms will not work with a 9s battery.

<img src="/uploads/db1493/original/3X/e/a/ea04ded3565cda41b4514abed57b7cb7810bcfaa.png" width="391" height="500">
```

---
## \#344 Posted by: TunaTee Posted at: 2017-09-27T02:25:12.022Z Reads: 261

```
Thank you very much for taking the time and drawing the diagram!
I thought their BMS supports 6s~10s no?
```

---
## \#345 Posted by: Namasaki Posted at: 2017-09-27T02:39:46.909Z Reads: 267

```
They sell bms's for all voltages but you have to order one for the specific voltage your running.

here is a link for the same bms but for 9s battery.


http://bestechpower.com/333v9spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

And your gonna need a 37.8v charger
```

---
## \#346 Posted by: TunaTee Posted at: 2017-09-27T02:47:21.601Z Reads: 258

```
Thank you. Just to be clear, I cannot use a charger that has a higher charging current than my nominal current which is 37.8 Volts?
```

---
## \#347 Posted by: Namasaki Posted at: 2017-09-27T02:50:54.964Z Reads: 268

```
[quote="TunaTee, post:346, topic:10014, full:true"]
Thank you. Just to be clear, I cannot use a charger that has a higher charging current than my nominal current which is 37.8 Volts?
[/quote]


You can not use a charger with higher voltage than the voltage of a 9s Lipo pack at full charge.
Lipo cells at full charge will be 4.2v
4.2 x 9 = 37.8

Just search eBay for  " 37.8v charger"
I ran the search and found at least three 37.8v 2a chargers

Nominal voltage is 3.7v per cell or 33.3v for 9s

You want the charger to match your battery's voltage at full charge or else it will not fully charge the battery.
```

---
## \#348 Posted by: TunaTee Posted at: 2017-09-27T03:18:49.134Z Reads: 256

```
Gotcha. :slight_smile:
```

---
## \#349 Posted by: Blacksheep Posted at: 2017-09-30T01:19:39.687Z Reads: 256

```
Does anyone have a extra bms
```

---
## \#350 Posted by: flywithgriff Posted at: 2017-09-30T01:22:24.697Z Reads: 258

```
What size?
```

---
## \#351 Posted by: Blacksheep Posted at: 2017-09-30T01:22:47.728Z Reads: 260

```
For those Lipo 10s
```

---
## \#352 Posted by: flywithgriff Posted at: 2017-09-30T01:25:05.306Z Reads: 256

```
I have one I have just taken out if a new build. I’m going a different direction and more than likely will not need it.
```

---
## \#353 Posted by: flywithgriff Posted at: 2017-09-30T01:28:16.730Z Reads: 262

```
I also have 10 2s 5ah 30c hardcase lipo packs for sale. They have been made into two 10s lipo packs. They can be used as two separate 10s packs or wired in parallel for a 10s2p 10Ah pack. This is how I used them and they have been used for 3 charge cycles.
```

---
## \#354 Posted by: bigben Posted at: 2017-09-30T06:51:36.537Z Reads: 256

```
I have a new 37.8v charger in the UK that I'm never going to use if you were EU way.
```

---
## \#355 Posted by: nmagz3 Posted at: 2017-10-10T16:50:45.891Z Reads: 260

```
Holy shit @Namasaki since the last time I visited this thread in January you've really had your work cut out for you answering questions!  Thanks so much for your insightful contribution!  I've recently ordered some of my parts now that I've gotten around to some extra cash.

Anyhow, I'm running a single 6375 R-Spec on 10s 8000mah and it works great.  This new battery setup will be used with the R-Spec but will be switched to the new Carvon v4s as soon as I receive it!  My question to you is: would it be better to go with the 12s over this 10s with the Carvon v4's or is that overkill?  Any pros or cons you can kindly point out?  Thanks again brotha!  I owe you a beer :)
```

---
## \#356 Posted by: Namasaki Posted at: 2017-10-10T19:57:53.313Z Reads: 259

```
I think the Carvons will do just fine with 10s. 
I would start with that anyway.
```

---
## \#357 Posted by: nmagz3 Posted at: 2017-10-10T19:59:33.593Z Reads: 266

```
Thanks for the quick reply.  I do feel like 10S (with Lipos) is very safe.  What's questionable is the 12s with Lipos.  I found my motor got pretty hot with a 12s after going up hills.  Thanks for the update sir!
```

---
## \#358 Posted by: esketit Posted at: 2017-10-12T17:25:59.843Z Reads: 279

```
I am trying to build a slim board, so I'm considering using 3S 5Ah lipos in series in parallel to make a 12S 10Ah battery pack that can be split across the top and bottom of the board like boosted.

This is the BMS I intend on using: http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D083.html

<img src="/uploads/db1493/original/3X/3/f/3fdf4e7bdc1492207d2158369cb20361927817b8.png" width="679" height="500">

<img src="/uploads/db1493/original/3X/0/3/034bbc0581984af889c787b643133ad0beb44dd8.JPG" width="494" height="500">
This image shows the wiring of the batteries a little clearer.

Would this setup work for charging and discharging?
```

---
## \#359 Posted by: cryo Posted at: 2017-10-19T18:43:36.796Z Reads: 262

```
hi @Namasaki

Do you know if a BMS is supposed to close off a circuit once cells reach a certain voltage? I left my loop key plugged in for a couple days and came back to 1 LiPo completely unbalanced with one of the lowest cells being 1.4v. My other LiPo seems fine since all cells are at my vesc cutoff voltage. 

I was under the impression that this was what they meant by over-discharge protection
```

---
## \#360 Posted by: Namasaki Posted at: 2017-10-20T01:44:15.439Z Reads: 257

```
can you post a diagram of your wiring?
including the brand and model of your bms
```

---
## \#361 Posted by: cryo Posted at: 2017-10-20T05:12:07.573Z Reads: 268

```
Shitty Diagram: 
https://i.imgur.com/LxS2JtH.png

The BMS product page 
http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html

And also if it matters, how I did my balance connections
https://i.imgur.com/rHPEjfw.png
```

---
## \#362 Posted by: Namasaki Posted at: 2017-10-20T13:41:21.176Z Reads: 246

```
All of your wiring looks correct. However, the over discharge detection for the Supower BMS is too low for Lipo batteries. Once a Lipo cell Falls below 3.0 V it can drop off very quickly. 
 However, the BMS should have shut down when that cell reached 2.9 V
```

---
## \#363 Posted by: cryo Posted at: 2017-10-20T15:34:43.095Z Reads: 242

```
So theoretically, If I left my board on until it ran out of juice every cell should be at 2.9v right?

Guess I just got a defective BMS, any way I can verify?
```

---
## \#364 Posted by: Namasaki Posted at: 2017-10-20T15:40:47.100Z Reads: 245

```
[quote="cryo, post:363, topic:10014"]
So theoretically, If I left my board on until it ran out of juice every cell should be at 2.9v right?
[/quote]

That's not exactly how it works. The Bms should shut down if even just one cell drops to 2.9 V. 
For example, if you have one cell that falls out of balance and goes lower than the rest. You could have nine cells at 3.0v+ and one cell at 2.9v. 
 At that point the BMS should shut down. 
You could possibly have a faulty BMS.
```

---
## \#365 Posted by: rich Posted at: 2017-10-29T14:22:52.782Z Reads: 241

```
Hey @Namasaki, finally I order my 12s BMS form bestech and have a question about overcharge settings. Your BMS has 4.28V detection voltage and 4.08V release voltage. Would it be possible to set the release voltage to 4.2V or ist it only possible with 0.2V difference? Because if the BMS would shut off due to regenerative braking with full battery the BMS stays off until the battery reaches 4.08V, or am I wrong?
```

---
## \#366 Posted by: Namasaki Posted at: 2017-10-29T15:53:18.020Z Reads: 243

```
You can request a different overcharge detection at the time you order the bms.
I just went with the default setting.
I did a full battery down hill braking test.
The results where:
As I was braking downhill with a full battery, the battery voltage climbed steadily until it reached 42.8 volts.
At that point the voltage stopped climbing and held at 42.8v 
Apparently the bms blocks the charge current at that point.
When I reached the bottom of the hill and released the brakes, the bms trimmed the voltage back down to 42v
The bms did not shut down even at 42.8v, it just blocked the charge current. 
It may be possible that if braking down a very long hill with a full battery so that 42.8v is maintained for a long duration that the bms may overheat and shut down.
When I ran my test, I was only at 42.8 for a very short duration. Probably 1 min or less.
I am running dual vescs with min bat current set at -10a so thats -20 total regen. At that setting, the voltage climb is still not too fast.
I assumed that since 4.28v overcharge detection was the factory default setting, that if was an acceptable amount.
After running my test, there was no noticeable damage to the battery.
I mean we are only talking about less than 1/10 of a volt per cell.
```

---
## \#367 Posted by: rich Posted at: 2017-10-29T16:10:38.155Z Reads: 240

```
[quote="Namasaki, post:366, topic:10014"]
The bms did not shut down even at 42.8v, it just blocked the charge current.
[/quote]

That's great info! Good 2 know, thank you!
```

---
## \#368 Posted by: bigben Posted at: 2017-10-29T17:20:36.678Z Reads: 244

```
I think we have a heartbeat.. 
Big thanks to @Namasaki !<img src="/uploads/db1493/original/3X/a/5/a5f4009bf118b7acfed424c58a13337673c5246d.JPG" width="375" height="500">
```

---
## \#369 Posted by: Namasaki Posted at: 2017-10-29T22:21:08.654Z Reads: 239

```
Let me explain with a little more detail. when my battery reached 42.8v I continued braking but the voltage never went over 42.8v
So My assumption was that the bms blocks the charge current at that point.
```

---
## \#370 Posted by: uigiroux Posted at: 2017-10-29T22:31:58.312Z Reads: 247

```
I am looking to do a build with the Carvon V4's also, but I'm going to go 4WD.  I had originally planned on building a 12s4p using the Samsung 30Q's, but I think I want to use the graphene batteries to do a 12s battery.  What would the stats be for that and what BMS would I need to use?
```

---
## \#371 Posted by: rich Posted at: 2017-10-29T23:02:22.974Z Reads: 246

```
[quote="Namasaki, post:369, topic:10014"]
So My assumption was that the bms blocks the charge current at that point.
[/quote]

That makes sense, I like the fact that it didn't shut off. But that would mean that even a overcharge setting of 4.2V would be better if the BMS just stops the charge and doesn't power off. But I read  threads about problem with BMS which shut off above overcharge limit. I think I go with 4.25V for safety :sunglasses:
```

---
## \#372 Posted by: uigiroux Posted at: 2017-10-30T00:11:04.856Z Reads: 228

```
Also would I want to go with the 2s*6, 3s*4, 4s*3, or 6s*2, and why?
```

---
## \#373 Posted by: Namasaki Posted at: 2017-10-30T00:12:34.163Z Reads: 259

```
The thing to remember is that if the bms stops the charge current, It most likely is going to cause heat. And if the heat goes too high, the bms will shut off. Although the Bestech bms is less likely to overheat than others.
Most other bms's do not have heatsinks on the FET's. The Bestech does.
The Bestech has a balancing discharge current of 126ma
Most other bms's balancing discharge current is only around 60ma. Including the Battery Supports brand.
```

---
## \#374 Posted by: Namasaki Posted at: 2017-10-30T00:32:50.104Z Reads: 277

```
[quote="uigiroux, post:370, topic:10014, full:true"]
I am looking to do a build with the Carvon V4's also, but I'm going to go 4WD.  I had originally planned on building a 12s4p using the Samsung 30Q's, but I think I want to use the graphene batteries to do a 12s battery.  What would the stats be for that and what BMS would I need to use?
[/quote]


30Q's are good batteries and a 12s4p pack with a good bms would probably do well especially in terms of range.
The drawback to using Li-ion cells, besides the size and weight of a 12s4p is that building such a battery requires more equipment and expertise because a poorly built Li-ion battery will not only be problematic but can be down right dangerous.
There have been at least 2 cases that I know of where boards using Li-ion packs have caught fire and burnt to the ground.
Several builders are using more advanced construction techniques such as cell lever fusing to improve safety and dependability.

http://www.electric-skateboard.builders/t/ollinboards-cell-level-fuse/7392
http://www.electric-skateboard.builders/t/fishpaper-and-cell-level-fusing-use-it/35026
```

---
## \#375 Posted by: Namasaki Posted at: 2017-10-30T00:36:27.160Z Reads: 247

```
[quote="uigiroux, post:372, topic:10014, full:true"]
Also would I want to go with the 2s*6, 3s*4, 4s*3, or 6s*2, and why?
[/quote]

It just depends on how thick you want the battery to be.
I used 2s to have the thinnest battery
```

---
## \#376 Posted by: uigiroux Posted at: 2017-10-30T01:11:25.418Z Reads: 237

```
So in terms of performance there is no difference?  I also want the thinnest setup, so I guess that means the 2s's then.
```

---
## \#377 Posted by: Namasaki Posted at: 2017-10-30T02:50:56.354Z Reads: 249

```
The performance will only depend on the total number of cells, the capacity and the C rating.
It is always recommended to get batteries with the highest C rating possible regardless of capacity however a combination of high C rating and high capacity is best.
Be aware that C ratings are a not a reliable measure of actual discharge current capability.
That is to say that a 5ah battery with 60C rating cannot really handle 300a
The Idea of multiplying capacity and C rating to determine actual discharge current is simply false.
As far as I know, there is only one distributor of Lipo batteries that states real discharge current capability for their packs.
http://www.smc-racing.net/index.php?route=product/category&path=67_97
```

---
## \#378 Posted by: uigiroux Posted at: 2017-10-30T03:13:13.460Z Reads: 248

```
How would that compare to the graphene one that was discussed earlier?

https://hobbyking.com/en_us/graphene-5000mah-2s2p-hardcase-w-5mm-female-bullet-connector.html?___store=en_us

That's what I'm leaning towards making a 12s setup from now.
```

---
## \#379 Posted by: Namasaki Posted at: 2017-10-30T03:16:57.657Z Reads: 248

```
I have heard that the Graphene's are good batteries.
My Turnigy 5ah 60C batteries do well and sag very little so the Graphene 90C should do really well.
```

---
## \#380 Posted by: Namasaki Posted at: 2017-10-30T03:24:20.671Z Reads: 249

```
I think these are a better deal though and they are in stock.
http://www.smc-racing.net/index.php?route=product/product&path=67_152&product_id=412
```

---
## \#381 Posted by: uigiroux Posted at: 2017-10-30T04:27:38.122Z Reads: 253

```
True, though I was just looking at their inventory, and I think getting four of these would be a better idea than the 2s, and they're in stock, and they would be just $60 roughly more than the ones you linked.
https://hobbyking.com/en_us/graphene-5000mah-3s-65c-w-xt90.html?countrycode=US&gclid=CjwKCAjw-NXPBRB4EiwAVNRLKragEW_5vr3bD1aI6f_oeGFEnb81lYF9hwoAPVUFHwupRVOFcMvSYhoCI5oQAvD_BwE&gclsrc=aw.ds
```

---
## \#382 Posted by: Namasaki Posted at: 2017-10-30T12:51:12.389Z Reads: 248

```
The 3s would be a good option just thicker than 2s
```

---
## \#383 Posted by: uigiroux Posted at: 2017-10-30T16:39:06.906Z Reads: 251

```
What kind of BMS would I need with the 3s, and is there a hobby charger that would work with the graphene battery as well?
```

---
## \#384 Posted by: Wilsonliang777 Posted at: 2017-10-30T20:49:20.036Z Reads: 264

```
I read this threat many times and I am ready to connect my 3s 7000 mAh into a 10s lipo back.   I just want to made sure I got it right before I begin.  I have 3x 3s lipo packs and salveraged another broken 3s pack to get a 1s 7000mah battery.   So.  3x 3s + 1x 1s= 10s 7000mah lipo.      Any advice and suggestion would be appreciated because I don't want to burn my house down or damage $120 of  lipo.  <img src="/uploads/db1493/original/3X/7/0/70af4a1aa1e2c115c51f3d48f1302d1746d184ae.jpg" width="375" height="500">
```

---
## \#385 Posted by: bigben Posted at: 2017-10-30T21:25:48.868Z Reads: 254

```
Graphene charges the same as lipo as far as I can work out. At least I hope it does because thats how i storage charged my graphene batteries.
<img src="/uploads/db1493/original/3X/4/b/4bc782512655bbbc313a52227b3bef9df8f353f2.JPG" width="375" height="500">
```

---
## \#386 Posted by: Namasaki Posted at: 2017-10-30T21:44:08.193Z Reads: 246

```
The Graphene is a Lipo battery
```

---
## \#387 Posted by: Namasaki Posted at: 2017-10-30T21:48:17.743Z Reads: 248

```
[quote="uigiroux, post:383, topic:10014, full:true"]
What kind of BMS would I need with the 3s, and is there a hobby charger that would work with the graphene battery as well?
[/quote]


The graphene is basically a Lipo battery. You can use a hobby charger.
If you are thinking of making an E-board with 3s voltage, forget it. You need at least 6s voltage.
I recommend the Bestech bms. the Model that I use and is featured in this thread is available for 6s to 12s
```

---
## \#388 Posted by: Namasaki Posted at: 2017-10-30T22:03:40.088Z Reads: 247

```
[quote="Wilsonliang777, post:384, topic:10014"]
Any advice and suggestion would be appreciated because I don't want to burn my house down or damage $120 of  lipo.
[/quote]


Your wiring diagram checks out.
There is very little chance of your batteries catching fire with this type of setup. 
The situations that would make your batteries catch fire would be
1. shorting them out long enough to make them ignite.
2. trying to charge them with too high voltage. ( example: using a 48v charger on a 10s pack with no bms.)
3. exposing the internals of the cell pouches to air or water while they are fully charged can cause explosive fire.

NOTE:
I would highly recommend that you consider batteries with higher C rating because they will suffer less voltage sag and will last longer.
7ah batteries with 25C will work if that's what you have already.
```

---
## \#389 Posted by: Wilsonliang777 Posted at: 2017-10-30T22:36:16.469Z Reads: 245

```
Thanks for the replay and advise.  Yes.  I should buy batteries with higher c rates but I can not afford new batteries now.      One more question.  I attached a diagram of my battery system that I want to bypass the bms on discharge.    Does the diagram look ok?  <img src="/uploads/db1493/original/3X/f/f/ff030322683b9be5231bc3e6f2aa25766b2a33ac.jpg" width="375" height="500">
```

---
## \#390 Posted by: uigiroux Posted at: 2017-10-30T22:58:37.064Z Reads: 231

```
I though I could use 6 of the 2s graphene batteries for a 12s6p setup..?  I know others have used five if the 2s lipo for a 10s setup.
```

---
## \#391 Posted by: uigiroux Posted at: 2017-10-30T22:59:19.440Z Reads: 230

```
Which batteries are you using exactly?
```

---
## \#392 Posted by: Brycehoosiers Posted at: 2017-10-30T23:02:34.048Z Reads: 230

```
If you use 6 2s batteries that equals a 12s1p, a 12s6p would be 36 batteries
```

---
## \#393 Posted by: bigben Posted at: 2017-10-30T23:13:15.363Z Reads: 246

```
https://hobbyking.com/en_us/graphene-5000mah-2s2p-hardcase-w-5mm-female-bullet-connector.html?___store=en_us
These ones. They were on special a while back so I bought two sets. This build is for a mate and not yet run it. I think it should have a bit of punch.
```

---
## \#394 Posted by: Namasaki Posted at: 2017-10-30T23:16:38.233Z Reads: 241

```
I prefer not to advise on bypassing. I do not recommend bypassing.
And I am curious as to how you would control the regen charging when it goes straight into the battery and not through a bms.
```

---
## \#395 Posted by: uigiroux Posted at: 2017-10-30T23:30:13.291Z Reads: 234

```
That's exactly what I was originally going to build for a 12s setup, but then for space sake I thought I would go with four of the 3s's, but I'm being told now that wouldn't work?  I'm not sure why exactly... It still makes a 12s setup...?
```

---
## \#396 Posted by: uigiroux Posted at: 2017-10-30T23:47:03.121Z Reads: 246

```
How much more power could I get if I was to use this 2s battery?

https://hobbyking.com/en_us/graphene-7500-mah-2s2p-hardcase-w-5mm-female-bullet-connector.html

What could I expect, more range, better acceleration, top speed, etc...?
```

---
## \#397 Posted by: Namasaki Posted at: 2017-10-31T00:35:42.367Z Reads: 238

```
[quote="uigiroux, post:396, topic:10014"]
What could I expect, more range, better acceleration, top speed, etc...?
[/quote]

Less voltage sag which means more power, range and even speed
```

---
## \#398 Posted by: uigiroux Posted at: 2017-10-31T04:43:39.840Z Reads: 243

```
I was just looking at some battery enclosures and came across Enertion's SPACE battery packs, which seem exactly what I'm looking for, but it seems like they stopped making them...?  Is this what happened?  If so, is there another company that makes professional looking battery packs out there?  Hopefully in the 12s series..?  I saw Enertion only did 10s, so... Yeah any help would be awesome!
```

---
## \#399 Posted by: Wilsonliang777 Posted at: 2017-10-31T05:05:57.268Z Reads: 258

```
I get your point.   I will try to get a bms that can handle the discharge amp.   How many amp should I get?   45amp discharge enough or 60amp or 80amp.  I am  runing  dual motor  1650w each.  10s  7000mah 25c battery.  ESC Max discharge is 2400w.  I am 150lb.  I am looking at a bms what spec below.  <img src="/uploads/db1493/original/3X/0/3/031835b138ac9182245910789d396faa047d5208.png" width="243" height="500">
```

---
## \#400 Posted by: bigben Posted at: 2017-10-31T07:20:24.671Z Reads: 246

```
People use 10s to be kinder to the vesc. 12s was thought to be living on the edge and has been connected to failing vescs.
Where in the world are you? It'll help to know where you are so people could offer up battery building services.
```

---
## \#401 Posted by: uigiroux Posted at: 2017-10-31T08:03:31.329Z Reads: 252

```
I'm in Omaha Nebraska.  I have no problem building any kind of battery I completely understand how to do that, I just would prefer something that looks professional... Though since it seems that getting a battery like that isn't likely, I'm now looking into building a longboard from wood and carbon fiber / Kevlar and building in a spot for everything so it'll be as thin as possible and look just how I want it. I've got experience with building things like that so this will just add one more way I can fully customize my build!
```

---
## \#402 Posted by: uigiroux Posted at: 2017-10-31T22:21:24.477Z Reads: 257

```
Ok forgive me in advance, but I also have a motorcycle and I want to build a battery for it.  The battery I am trying to replace is:

https://earthxbatteries.com/shop/ETX18B

I want to use one of these battery blocs from :

http://www.batteryblocs.com

to build it.  What setup would I need to get something comparable?  I have a single cylinder 650 cc engine btw.  I was thinking either the 6p2s or 8p2s, but I'm not sure.  Assume I'll use Samsung 30Q's also.  Thanks for your help!
```

---
## \#403 Posted by: uigiroux Posted at: 2017-10-31T22:28:48.986Z Reads: 246

```
They normally use the A123 26650 batteries to make the batteries, usually 6, maybe 8, so I figure I could make a comparable one using these much less expensive 18650's.
```

---
## \#404 Posted by: uigiroux Posted at: 2017-11-01T01:37:54.850Z Reads: 259

```
I was just looking at some Trampa boards and came across their VESC V6.1

http://www.trampaboards.com/vesc-6-complete--vedder-electronic-speed-controller-trampa-exclusive-p-24166.html

and it seems like it's very different, and from what they're saying it's the best one you can get, by far...?  Has anyone read up on these things?
```

---
## \#405 Posted by: GunnarK Posted at: 2017-11-02T13:58:10.109Z Reads: 270

```
Hi guys,

Having a 'little' problem here
I was recently working on my battery because the negative end had come loose of the BMS.

Now I managed to create some sparks from shorting by letting the negative battery lead touch one of the 'thingies' on the BMS. (see picture) the middle lug of the 'thingy' has the most 'damage'.

This caused some colouring on the solder, but worse is probably that it seems to be the cause of my BMS not fully charge the battery anymore (stops around 68%)...
<img src="/uploads/db1493/original/3X/a/4/a4e8aaf1ef6df596e34497b3328e1ff088ad839a.jpg" width="666" height="500">

Could this easily be fixed? Or could it be the case that more hardware is affected?
I don't have a voltmeter yet to test things, but maybe you can give some direction in the matter!

Thanks

EDIT: I created a new topic on the matter but thought it would be good for people to have a sense of where to go to if they face the same problem as me
http://www.electric-skateboard.builders/t/bms-replace-part-or-just-broken-ruined/37176?u=gunnark
```

---
## \#407 Posted by: GunnarK Posted at: 2017-11-02T14:15:16.727Z Reads: 253

```
@MattHarder This is a question that is not directly related to the topic. I would suggest you to create a new topic.
This can be done on the homepage in the upper right corner you find a button 'create new topic'.

To answer you're question nonetheless;
Money vs. quality is your factor now. Cheaping out on batteries is not the best thing though, I would advise to get a 30C rated battery as a minimum to not stress the batteries as much. A BMS is something you need to consider as well
A bestech bms will help prolong the life of your batteries, keeping them balanced while discharging (lipos tend to go out of balance).
But a cheap bms can also be used albeit only for charging (NB not 'discharging') and could go for like 10 bucks, 1/8th of the price for a Bestech BMS.
I would suggest the Bestech BMS and see it as an investment that you'll be glad for making
```

---
## \#408 Posted by: MattHarder Posted at: 2017-11-02T14:53:21.065Z Reads: 244

```
@GunnarK Thank you so much! That helps me a lot. Sorry about posting this here I am new to the forums and didn’t know how to post anything by itself. Thanks so much
```

---
## \#409 Posted by: Juiced Posted at: 2017-11-06T20:47:25.410Z Reads: 239

```
Is there any way you can post your vesc settings with this build?
```

---
## \#410 Posted by: Namasaki Posted at: 2017-11-06T22:00:46.683Z Reads: 252

```
[quote="Juiced, post:409, topic:10014, full:true"]
Is there any way you can post your vesc settings with this build?
[/quote]

Dual Motor Settings

<img src="/uploads/db1493/original/3X/f/c/fcd7f9bb046818a4c4839f5c0277096a93e5bdc4.png" width="690" height="363">

<img src="/uploads/db1493/original/3X/c/8/c86fcf7410b6c58bfa2d0b800b6678e2750a1556.png" width="690" height="363">
```

---
## \#411 Posted by: Juiced Posted at: 2017-11-06T22:59:26.486Z Reads: 222

```
Thanks! What would you recommend for a single drive? I'm setting up as we speak
```

---
## \#412 Posted by: Namasaki Posted at: 2017-11-07T00:06:17.067Z Reads: 222

```
The only thing I would change for single drive is the battery min current.
with this battery build and a single drive, you could run the battery min current at -20
```

---
## \#413 Posted by: ryan_pogi Posted at: 2017-11-08T04:42:23.535Z Reads: 227

```
@Namasaki, is it possible to run 10 packs of 2s/5000mah/60c (to a 10s2p setup) and use a 10s bestech bms?
```

---
## \#414 Posted by: Namasaki Posted at: 2017-11-08T11:58:40.712Z Reads: 236

```
I haven't tried this but I guess it's doable. 
It would be better to get high capacity, high discharge packs and keep it simple.
```

---
## \#415 Posted by: mmaner Posted at: 2017-11-08T18:50:30.899Z Reads: 252

```
[quote="ryan_pogi, post:413, topic:10014"]
is it possible to run 10 packs of 2s/5000mah/60c (to a 10s2p setup) and use a 10s bestech bms?
[/quote]

It is I have done it.  

<img src="/uploads/db1493/original/3X/2/e/2e1dad479b80ea26687a9f4da341b30451c7c4c7.jpg" width="156" height="500">
```

---
## \#416 Posted by: ryan_pogi Posted at: 2017-11-08T19:07:49.587Z Reads: 241

```
This is great news for me.
Thanks, @mmaner.
```

---
## \#417 Posted by: Namasaki Posted at: 2017-11-08T22:18:19.525Z Reads: 240

```
You must be getting close to 30 miles range with that setup.
```

---
## \#418 Posted by: mmaner Posted at: 2017-11-08T22:38:11.952Z Reads: 235

```
If I could stay out of the throttle I would 😀.  I get about 22 to 24.
```

---
## \#419 Posted by: Namasaki Posted at: 2017-11-08T23:08:23.207Z Reads: 233

```
Still some serious range.
```

---
## \#420 Posted by: mmaner Posted at: 2017-11-09T01:38:52.244Z Reads: 232

```
Yeah, it's fun. I take it out if town alot, because I know I won't have to charge often. I really haven't ridden it much lately. With the Jet Spud 29 & now the Evo on 6 Shooters I'm having fun 😀
```

---
## \#421 Posted by: Gynpe Posted at: 2017-11-09T03:08:11.500Z Reads: 238

```
Hey @Namasaki I'm thinking of going 12s, and also want to swap the wheel pulley from 36 to 32 which I have laying around.

I understand speed will increase.

Is there anything (aside from speed and safety) that I should worry about? Or is this perfectly fine with my single 170KV + FocBox build?

@ryan_pogi @mmaner  I was thinking about doing the same exact thing the other day. Glad to know it is possible.
```

---
## \#422 Posted by: ryan_pogi Posted at: 2017-11-09T19:05:47.460Z Reads: 244

```
Questions, @mmaner, @Namasaki.  
1.) So battery #1 and #6  balance wires go together, right? Is it better to solder them, then heat shrink? or a butt connectors will do?
2.) yellow wire is at balance port #1 and red is at balance port #2, then eliminate/ isolate the black wire.  Is this correct?
3.) So I will be using 10 packs of 2s/5000mah/60c LiPo's.  Will a 42v 2ah Lithium battery charger (hoverboard charger) be sufficient for charging?

Thanks.
```

---
## \#423 Posted by: mmaner Posted at: 2017-11-09T23:53:18.232Z Reads: 241

```
1 > Correct. Yes solder, no butt-splice = very very bad.
2 > I'm not sure about the colors, mine are different.  You need to use a multimeter to define which is cell 1 and which is cell 2.  Yes, you will isolate the negative.
3 > That charger should be fine, you could use a 5a charger thought o charge faster.
```

---
## \#424 Posted by: ryan_pogi Posted at: 2017-11-10T00:08:19.054Z Reads: 232

```
Sorry, how do you define which is cell #1 using a multi-meter on yellow and red wire?
One should give you a reading and the other does not?
```

---
## \#425 Posted by: Namasaki Posted at: 2017-11-10T01:25:48.638Z Reads: 234

```
Rule of thumb for 2s Lipo balance wires. 
Black wire on edge of connector is ground
Red wire on opposite edge is cell 2
Wire in middle of connector is cell 1
On Lipos that are 3s to 6s, the balance wires are always in succession and cell 1 is always next to the black ground wire. 
The red wire on the edge is always the last cell in the pack. 
The black wire on the edge is always ground.
```

---
## \#426 Posted by: ryan_pogi Posted at: 2017-11-10T01:28:53.636Z Reads: 234

```
Got it, thanks.
```

---
## \#427 Posted by: ryan_pogi Posted at: 2017-11-10T22:18:31.485Z Reads: 263

```
Normally, I just buy batteries pre-packed, or pre-made.  Cause I'm one of those guys you call lazy, sadly.
This is my 1st attempt to make my own.  Starting the the least expensive ones, the LiPo's.

Learned from some articles and videos that LiPo's are some scary sh!t.  One of the most dangerous batteries around.
No wonder hard packs are nice, for extra battery protection. With BMS (assuming in good working condition), will, somehow, eliminate over charging and make it safer.  But still, it does not mean you will let your battery charging unattended.

Anyway, I just got my 4 pack of 10 (2s/5000mah/7.4v 60c LiPo) from hobbyking and will start solder them in series.
So I used my multi-meter to test the balance wires (for curiosity sake).
The cell #1 reads 3.7v, while cell # 2 reads 7.5v. 
So the conclusion is, the lowest voltage reading is the cell #1, and adds up till you reach 37v, which is cell #10.
Since I'm doing the parallel, I'll just match-up the balance wire with the same voltage reading.
Thanks to @mmaner 's crystal clear diagram, I know now where to connect the volt meter, and charger.
Thank you too @Namasaki.
```

---
## \#428 Posted by: Namasaki Posted at: 2017-11-10T23:11:03.005Z Reads: 267

```
It's a really good idea to balance charge each pack before soldering them together. Especially if your connecting them in parallel.
anytime you connect multiple cells or packs in parallel, they will auto balance themselves quickly with high current transfer that can damage the cells involved.

I have been using Lipos for years, first in helicopters and now in Eboards. I have never had a problem with them catching fire or exploding.
Just use quality Lipos and balance charge them either with a good hobby charger designed for Lipos or a bms and brick charger with the correct voltage output.
Since I've been into Eboarding, I have not seen anyones lipo build catch fire but I have seen 2 builds with Li-ion batteries burn to the ground.
When you stop and think about it, the Lipo build is somewhat flexible.
The welded Li-ion pack is more rigid and consequently, more susceptible to vibration and road shock.
The pics below are both Li-ion builds that just caught fire. The top one for no apparent reason. The bottom one ignited after riding over a very rough road.

<img src="/uploads/db1493/original/3X/f/d/fda395299c20141371207d0d4ab58d9b653abe51.png" width="281" height="500">

<img src="/uploads/db1493/original/3X/f/f/ff2846ce445faeae63d2d0ac0375c4bc9b7273bb.jpg" width="690" height="387">
```

---
## \#429 Posted by: GunnarK Posted at: 2017-11-15T17:59:24.028Z Reads: 249

```
Battery min at -20 for a 5ah battery?
Thought one shouldn't go beyond 2c, meaning -10 in this case.
```

---
## \#430 Posted by: Namasaki Posted at: 2017-11-15T18:51:02.444Z Reads: 246

```
The Lipo packs that are featured in this thread are rated for 5C charge or 25a
I bench charge them at 5a 
They have been doing fine with regen brakes batt min at -20a total
```

---
## \#431 Posted by: GunnarK Posted at: 2017-11-15T20:51:21.851Z Reads: 243

```
Nice!
Mine are rated 3C charging. Best to leave it at 10 instead of 15?
```

---
## \#432 Posted by: Gynpe Posted at: 2017-11-17T03:36:44.123Z Reads: 242

```
Hey!

Currently hooking up the 10s battery to the 10s BMS... Before I did so, I measured all cells, and later the total for the pack which was 41.6v (I actually screwed up the batteries a little bit from charging carelessly, and now 41.6v is the maximum it charges) at any rate... All cells are balanced...

When I check the voltage THROUGH the BMS it reads 40.8v, that's 0.8 less volts. 

Is it normal for the BMS to "eat" up some voltage?
```

---
## \#433 Posted by: Namasaki Posted at: 2017-11-17T18:55:34.872Z Reads: 233

```
I've never known the bms to eat any voltage. 
Where are you measuring the voltage?
Try waiting about 5 seconds after turning it on before measuring. 
If your batteries are balanced but not charging to full 42v then the problem most likely is with the charger your using.
That is, if your using the BMS and settings featured in this thread
```

---
## \#434 Posted by: Gynpe Posted at: 2017-11-18T17:41:31.104Z Reads: 235

```
Hey, I was measuring the voltage without turning the BMS on.

Once I turned it on it gave the proper reading.

Side note, I installed the charge port to the -C on the BMS and the positive to the positive that comes out of my battery. As it was charging I turned on the BMS and the charger blew up.

Smoke... Fear... Fun.

So, I advise not to do that to future builders.
```

---
## \#435 Posted by: Namasaki Posted at: 2017-11-18T20:00:26.568Z Reads: 234

```
Your charger did not blow up because you turned the bms on. 
The bms is supposed to be on while charging per the manufacture's instructions.
I usually turn my charger on first and then turn the bms on immediately and nothing has ever blown up.
```

---
## \#436 Posted by: Gynpe Posted at: 2017-11-18T20:18:02.368Z Reads: 240

```
Oh crap...

I remember I plugged in the charger to the charging port, and the charger seemed to be making some sort of sound (which I can't recall) then I turned on BMS and just smoke everywhere. I nearly soiled myself.

Anybody know what it can be due to? I'm not sure I should plug another charger in...

BTW used the same batteries, same BMS, a 24 euro 42v 2a charger, and I think even the same charging port for segways, and the connections I'm 99.9% sure they are right.
```

---
## \#437 Posted by: Namasaki Posted at: 2017-11-18T20:48:44.885Z Reads: 239

```
Double check the polarity of the charger and your charge socket on the board. 
It sounds like you got the polarity wrong.
```

---
## \#438 Posted by: Gynpe Posted at: 2017-11-21T05:23:01.252Z Reads: 253

```
It was indeed a polarity problem. Everything seems to be connected properly now, except...

This is the charger connected only to the plug in my house <img src="/uploads/db1493/original/3X/3/7/37803550f0897a55a35753f447418dbee9ed8bb2.jpg" width="281" height="500">
As you can see the light on the charger turns green.

And this is what happens when I connect the other end to the board <img src="/uploads/db1493/original/3X/a/f/af18c2f098d8e6c36583d0c91950cebb84bf9c9e.jpg" width="281" height="500">

You can bearly tell, but it powers up my focbox, and the light on the charger goes from green to red, and that's with the bms off.

I'm afraid to turn it on, and there aren't any instructions that come with these chargers. Should I just switch on the bms?

Sorry for the shit pictures.
```

---
## \#439 Posted by: Gynpe Posted at: 2017-11-21T10:27:52.267Z Reads: 241

```
Quick update, I left the charger on without turning on the BMS and saw that the voltage was going up... Meaning the battery was being charged, so I manned up and turned on the BMS.

Battery is fully charged. The joy is unexplainable... It only charges to 41.6v, but still... I'm happy as hell.

Thanks for enduring my constant noobness @Namasaki.

Will open up a thread with my build and pictures when I get the chance!

Thanks again!!
```

---
## \#440 Posted by: GunnarK Posted at: 2017-11-21T16:17:15.937Z Reads: 248

```
Your Bestech BMS should automatically turn on when you plug in the charger. If this is not the case than I think something is wrong with your wiring.
I can confirm this since I have a battery indicator connected between the pos and neg ports coming out of the BMS
http://www.electric-skateboard.builders/t/my-monodrive-6374-10s-bamboo-eboard/33460/31?u=gunnark

As to the 41.6v of charge: just because your charger says 42v on the enclosure doesn't mean it will actually charge to 42.0v
A charger or higher quality might, but a 24 bucks charger almost certainly won't.

Cheers
```

---
## \#441 Posted by: mmaner Posted at: 2017-11-21T16:23:09.094Z Reads: 235

```
None of my BesTech BMS's automatically turn on when I connect the charger, I have to turn them on to charge.  That's one of the characteristics of the BEsTech BMS that it does not allow any traversal unless the ON/OFF circuit is completed.  I haven't bought one in about 3 months, so it might be different now, but of the 4 that I own none auto turn on.
```

---
## \#442 Posted by: GunnarK Posted at: 2017-11-21T16:25:05.093Z Reads: 232

```
Hmmm interesting.
Mine also turns automatically off as soon as the charging has completed, or so it seems.
Probably the charger that stopped charging resulting in the BMS turning off
```

---
## \#443 Posted by: mmaner Posted at: 2017-11-21T16:30:51.410Z Reads: 235

```
Ahhhh you meant the charger, I thought you meant the board electronics.  I was trying to say that to charge I have to have the BMS switch on, when its off it doesnt charge.
```

---
## \#444 Posted by: GunnarK Posted at: 2017-11-21T16:43:39.311Z Reads: 235

```
Nope haha
I really mean my BMS automatically turns on the moment I plug in my charger. I don't have to touch my e-switch at all!

Then, when I unplug the charger I can see the voltage dropping because of the indicator wired in between and the whole systems turns off.

Before I bought the BMS I read I had to switch on the board before plugging in the charger. Forgot that once and my board magically turned on!

Really like it this way. Now I can spot across the room if it is done charging 👌
```

---
## \#445 Posted by: Namasaki Posted at: 2017-11-21T18:35:31.230Z Reads: 229

```
The bms only appears to turn on when you plug in the charger because the charger supplies power to the output side of the bms. 
This is why your Vesc turns on and your meter lights up. 
You still need to manually turn the bms on to charge or it will not work correctly.
```

---
## \#446 Posted by: GunnarK Posted at: 2017-11-23T14:15:02.933Z Reads: 227

```
Definitely gonna check that out! 
I thought I shorted some things which caused it to not charge over 69%...
Fingers crossed what you describe is the culprit!
```

---
## \#447 Posted by: Muke Posted at: 2017-11-28T17:18:11.622Z Reads: 235

```
@Namasaki I think I will copy your battary/bms system for my first build. Will this BMS work with an 8s pack too?
I would love to start with 8s and upgrade to 10s later on (need to cut cost).

Thanks for all your work in this forum, your replies have helped me out a lot already! :slight_smile:
```

---
## \#448 Posted by: mmaner Posted at: 2017-11-28T17:51:34.596Z Reads: 239

```
[quote="Muke, post:447, topic:10014"]
Will this BMS work with an 8s pack too?
[/quote]

You will need to get an 8S BMS, unless you use the @raphaelchang BMS which is adjustable IIRC.
```

---
## \#449 Posted by: Muke Posted at: 2017-11-28T18:27:36.961Z Reads: 236

```
Ok thank you!
```

---
## \#450 Posted by: PredatorBoards Posted at: 2017-11-28T18:35:02.264Z Reads: 253

```
Ayyy! I've used those same styled hard case batteries (4S1P) for my Duce 

12S1P + onboard charger 
<img src="/uploads/db1493/original/3X/7/8/78cff2b2a7c15f5223ca1e9b9c3af79cd83524db.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/1/e/1eaf949d84573c1a7db3a7c7d8eed2e348616389.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/6/1/610709b040ab8e7f6c17c03583a484a91303dad0.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/2/d/2d5508d64bdb03caac3c8e52b445027ab56c8268.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/8/3/8397b5625ea7cbea82b3d38a0a05c10968f557a0.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/6/8/6859405543329015e640d5d1b5aa9d3568eb6d41.JPG" width="666" height="500">
```

---
## \#451 Posted by: GunnarK Posted at: 2017-11-30T18:47:41.615Z Reads: 236

```
Hi Namasaki,

What about this BMS?
http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D336.html
Heard from from a guy from Belgium this one costs around 30 euros a piece while the D223v1 costs about 50 euros.

Would love your opinion or maybe you can shine some light on why this BMS isn't as expensive as the D223V1.
That 10amp discharge difference does not bother me
```

---
## \#452 Posted by: Namasaki Posted at: 2017-11-30T18:52:51.297Z Reads: 223

```
Looks ok to me. It appears to have a built in E-switch but they don’t say so I would ask them to make sure.
```

---
## \#453 Posted by: GunnarK Posted at: 2017-11-30T18:54:20.864Z Reads: 216

```
The guy who referred me to this BMS has ordered these before and confirms it has an e-switch.
```

---
## \#454 Posted by: Namasaki Posted at: 2017-11-30T18:58:09.969Z Reads: 214

```
I’d say go for it then. 
It’s a good deal at the price you mentioned.
An external E-switch alone would cost more.
```

---
## \#455 Posted by: GunnarK Posted at: 2017-11-30T19:03:20.663Z Reads: 220

```
Exactly!
I was a little stunned because of the price difference and the little specs difference there is.
Only main differences are:
-size
-max discharge

All others are adjustable.

Only reason for this price difference I could think of is the manufacturing since it is not a "sandwich bms" and the slightly lower discharge level
```

---
## \#456 Posted by: Namasaki Posted at: 2017-11-30T19:54:12.608Z Reads: 212

```
[quote="GunnarK, post:451, topic:10014"]
D223v1
[/quote]

The D223v1 seems to have better heat sinks but that might not be an issue.
```

---
## \#457 Posted by: GunnarK Posted at: 2017-11-30T20:02:56.202Z Reads: 205

```
Not really I guess. Though I can recall the D223V1 warming up my enclosure.
Nothing extreme but definitely warm
```

---
## \#458 Posted by: Namasaki Posted at: 2017-11-30T20:08:05.192Z Reads: 207

```
I’ve never noticed that running 10s. 
Are you running high regen current?
Batt min. 
I run my total Batt min at -20a
Or -10 per Vesc.
```

---
## \#459 Posted by: GunnarK Posted at: 2017-11-30T21:20:14.388Z Reads: 205

```
Oh forgot to mention: later I discovered one of my 2s packs had started to swell slightly (the one closest to my BMS) so I think that is where the heat came from. Not sure though.
Will look into the packs this weekend

Batt max is set to 40
Batt min is set to -10
```

---
## \#460 Posted by: hornet90 Posted at: 2017-12-01T04:14:30.195Z Reads: 210

```
Looks good
```

---
## \#461 Posted by: ivanflo Posted at: 2017-12-03T00:08:23.911Z Reads: 212

```
am looking to purchase this BMS, What overcharge/over discharge voltage setings would be appropriate?

I will be using a similar battery setup as used in this thread.
```

---
## \#462 Posted by: Namasaki Posted at: 2017-12-03T00:48:09.744Z Reads: 214

```
I went with the factory default on over charge 4.28v
and the highest available setting for over discharge  3.0v
```

---
## \#463 Posted by: Hankbull Posted at: 2017-12-03T10:48:52.969Z Reads: 231

```
Hey man,  thanks heaps for this post. I just finished my first build following your build. I hope to find someone with a computer so I can set it up. Thanks again for such a detailed build log and answering everyone's questions. Cheers
```

---
## \#464 Posted by: Torcn Posted at: 2017-12-22T21:57:58.486Z Reads: 234

```
Hey guys!!! I’m planning to build a battery pack inspired on those. I’m in canada for what I have been looking is harder to get parts specially battery’s, shipping cost is crazy plus duty’s.

VESC is 60A max so do you think 60A bms is safe? I already went down trought all thread and you guys are using 80A bms. 

https://www.amazon.ca/gp/aw/d/B00WQCTQL4/ref=mp_s_a_1_3?ie=UTF8&qid=1513979796&sr=8-3&pi=AC_SX236_SY340_QL65&keywords=lipo+battery&dpPl=1&dpID=51nK7JjST1L&ref=plSrch

This on amazon are good deal for me, free shipping. Any thoughts?
```

---
## \#465 Posted by: Namasaki Posted at: 2017-12-22T22:12:18.343Z Reads: 227

```
I have not personally used Gens Ace but I have read that they are good quality.
A 60a bms should be fine for discharge.
Other important factors are short circuit protection and balance current. Some bms's offer up to 126ma balance current while others can be as low as 42ma
Also important to know that most bms's have an over discharge detection of 2.8v per cell which is fine for Li-ions but too low for Lipos.
```

---
## \#466 Posted by: Torcn Posted at: 2017-12-23T01:32:45.435Z Reads: 219

```
I’lol go with those. HobbyKing shipping doesn’t worth it. Didn’t knew that, still don’t know which bms will pick. Where did you get your voltage indicator? I got one similar but only shows me percentage
```

---
## \#467 Posted by: Lospalaz Posted at: 2017-12-23T02:46:41.613Z Reads: 213

```
I went with this from Aliexpress:

[10S 80A active bms 2017 new Li-ion smart bms pcm with android Bluetooth app UART correspondence bms wi software (APP) monitor](https://www.aliexpress.com/item/10S-80A-active-bms-2017-new-Li-ion-smart-bms-pcm-with-android-Bluetooth-app-UART/32839468266.html?ws_ab_test=searchweb0_0,searchweb201602_3_10152_10065_10151_10344_10068_10130_10345_10342_10547_10343_10340_10548_10341_10541_10084_10083_10139_10307_10539_10312_10059_10313_10314_10534_100031_10604_10603_10103_10605_10594_10596_10142_10107,searchweb201603_12,ppcSwitch_2&algo_expid=1487dff9-f2f1-4913-8704-d55142dd30c3-5&algo_pvid=1487dff9-f2f1-4913-8704-d55142dd30c3&rmStoreLevelAB=4)

It's still in the mail...
```

---
## \#468 Posted by: Namasaki Posted at: 2017-12-23T02:53:16.051Z Reads: 218

```
There is a mod you an do to make it display voltage

http://www.electric-skateboard.builders/t/diy-battery-pack-using-basen-26650-hi-drain-li-ion-cells/4973/324?u=namasaki
```

---
## \#469 Posted by: Torcn Posted at: 2017-12-23T13:25:13.552Z Reads: 214

```
Looks interesting with the app. Do you know if there is a 6s version?
```

---
## \#470 Posted by: Torcn Posted at: 2017-12-23T13:27:48.340Z Reads: 213

```
Will try to do it. Voltage reader is must have if bms only cuts off at 2.9v.
You said usually only discharge to 3.6v? Why? Is it better for battery’s? Can’t you go to 3.2?
```

---
## \#471 Posted by: Lospalaz Posted at: 2017-12-23T15:48:19.726Z Reads: 211

```
Nope, the fun begins at 10s! (And goes to 30s.)
```

---
## \#472 Posted by: Namasaki Posted at: 2017-12-23T19:06:50.102Z Reads: 216

```
With Lipos, the less you drain them the better. 
This is probably true for Li-ions as well although they can go lower than Lipos. 
The thing is that unless every cell is perfectly matched including internal resistance, they will not discharge evenly. So if your monitoring total pack voltage instead of individual cell voltage while discharging, you should allow a margin of safety.
```

---
## \#473 Posted by: Lospalaz Posted at: 2017-12-23T22:54:35.815Z Reads: 223

```
...
...

...Let's say that _someone_ did something inadvisable like buying five 15-30c 5.2a lipo (like _[these](https://www.genstattu.com/tattu-5200mah-7-4v-15c-30c-2s1p-lipo-battery-pack-with-deans-plug.html)_), would adding a cap pack (like _[this](https://emperformanceproducts.com/cap-pack/)_...) be able to make up the c rating?

(...Or at least discourage puffy batteries T_T)
```

---
## \#474 Posted by: Namasaki Posted at: 2017-12-23T23:55:20.862Z Reads: 227

```
The GensTattu’s are said to be good quality. 
And using a Capacitor pack is something that I have not tried but it sounds like a good idea. 
@PatRocks is using a cap pack with Tattu Lipos. 
Maybe he can check in and give his opinion.
```

---
## \#475 Posted by: PatRocks Posted at: 2017-12-24T01:55:59.811Z Reads: 234

```
The batteries you choose will have pros and cons, and in many cases, the deciding factor is cost (don't make that mistake). For me, as well as @Namasaki the decision to go LiPo is discharge capability. As you may already know @Lospalaz the C-rating of a lipo is the manufacturer's claimed max. sustained-current output without causing damage to a cell's chemistry. Depending on how you ride, you may very easily exceed 78 Amps at times, but probably not often. If you are planning on smaller capacity packs, GO HIGH C-RATING, or wish you had later. 

A capacitor pack will not mitigate voltage-sag, at least not for any sustained period. They are more for smoothing out the current spikes associated with switched DC motors (brushless motors). The Cap-pack you linked above is the one I bought, and it's awesome. It will increase performance, but not necessarily in a way that you will feel. What it WILL do is increase the life-span of your ESC, clarify your RF signal, look awesome, and give you more instant-power! 

So my opinion: Capacitors? - get some! 5200mAh 15c LiPos? you should reconsider, but they may be suitable for you... 

Patrick
```

---
## \#476 Posted by: Lospalaz Posted at: 2017-12-24T04:52:51.436Z Reads: 217

```
[quote="PatRocks, post:475, topic:10014"]
5200mAh 15c LiPos? you should reconsider, but they may be suitable for you...
[/quote]

*slumps forward in chair, holding head in hands*
"B-but they were on sale, and they look so nice in my bookshelf as I wait patiently for other parts of my eboard arrive"

Agh.  The manufacturer's claimed constant is 15c and max discharge is 30c.  I'm going to trust it (#famouslastwords) and see how a hill-climb goes.

As for the capacitors, I'll let that be the next upgrade!
```

---
## \#477 Posted by: PatRocks Posted at: 2017-12-24T05:41:42.115Z Reads: 211

```
Oh my bad, I didn't realize you already have them😅
They'll be good batteries for sure! I like them crazy as hell, and forget that's not for everyone. Or necessary lol. Are you doing a single motor?

At the very least, those tattu batteries will last a long time. They have a great reputation for quality
```

---
## \#478 Posted by: Lospalaz Posted at: 2017-12-24T06:31:43.436Z Reads: 208

```
Okay, battery manufacturer with stellar reputation, check.
[quote="PatRocks, post:477, topic:10014"]
Are you doing a single motor?
[/quote]


Dual motor build. (Do not tell me that my highly-regarded batteries are not okay for a dual motor build...! T_T)
```

---
## \#479 Posted by: PatRocks Posted at: 2017-12-24T06:39:18.923Z Reads: 210

```
You'll draw the same amount of power each way, with dual motors each does half the load
```

---
## \#480 Posted by: Lospalaz Posted at: 2017-12-24T07:00:15.482Z Reads: 212

```
Wrapped up in battery paranoia I completely forgot about that =P.  Okay, I'm much better than I was 8 hours ago, thanks!
```

---
## \#481 Posted by: Namasaki Posted at: 2017-12-24T15:56:28.198Z Reads: 213

```
[quote="PatRocks, post:479, topic:10014, full:true"]
You'll draw the same amount of power each way, with dual motors each does half the load
[/quote]
True,
With dual drive, each motor/vesc handles 1/2 the wattage needed however the maximum wattage potential is theoretically doubled.
This allows you to climb steeper hills with dual motors.
@Lospalaz 
If you fear that your battery can't handle the potential maximum then all you have to do is reduce the battery max amps setting in the Vesc tool.
```

---
## \#482 Posted by: Lospalaz Posted at: 2017-12-24T17:04:02.807Z Reads: 218

```
[quote="Namasaki, post:481, topic:10014"]
reduce the battery max amps setting in the Vesc tool.
[/quote]

VESC...
Ahh... 
About that...
I bought [this](http://www.diyeboard.com/upgraded-v21-dual-belt-motor-sine-wave-foc-esc-speed-controller-p-599.html). dual esc from diyeboard.

(I... I told myself that I wanted simplicity... T_T)

But I'm sure my batteries can handle the amps.
```

---
## \#483 Posted by: Torcn Posted at: 2017-12-25T03:21:26.524Z Reads: 211

```
Thanks for your tips!! Already got the batteries will buy bms and try to connect everything together, let’s see how it goes, I’m dummy when it comes to batteries
```

---
## \#484 Posted by: Namasaki Posted at: 2017-12-25T03:30:31.841Z Reads: 208

```
If you have any questions, we are here to help.
```

---
## \#485 Posted by: Torcn Posted at: 2017-12-27T02:20:40.730Z Reads: 218

```
Thank you. I’ll share my experience when I get all the parts to start :slight_smile:
```

---
## \#486 Posted by: DevinG Posted at: 2017-12-28T12:33:50.502Z Reads: 212

```
do you have volt cap tester coming off the bms? where does this usually get attached electricly?
```

---
## \#487 Posted by: Namasaki Posted at: 2017-12-28T16:41:26.758Z Reads: 210

```
I have my volt meter on the output side of the bms
The positive lead goes to the battery positive and the negative lead goes to the bms P-
```

---
## \#488 Posted by: DevinG Posted at: 2017-12-29T01:53:28.927Z Reads: 216

```
Im just trying to confirm is whether or not I can come off my series adapter just before the esc since im not using a bms atm.
Also if l am likely to get accurate readings.
```

---
## \#489 Posted by: gogomrrobot Posted at: 2017-12-29T19:56:04.174Z Reads: 237

```
@Namasaki or anyone:
 
Does bestech BMS 223V1 tend to lose about 0.8V in overall efficiency? Have the spec sheet.

Battery should be 50.3 but instead oscillating between 49.4 and 49.5V

<img src="/uploads/db1493/original/3X/8/9/8937c72a03961e1d4687d5b5e2010f59c1adb57e.JPG" width="375" height="500">
```

---
## \#490 Posted by: Namasaki Posted at: 2017-12-29T19:59:00.831Z Reads: 231

```
Did you check the battery voltage where the battery connects to B- on the bms?
You know the bms e-switch wires have to be connected and the bms on when charging or testing voltage right?
```

---
## \#491 Posted by: gogomrrobot Posted at: 2017-12-29T20:06:46.233Z Reads: 231

```
Nope I didn't have the eswitch wires connected. Doing that now.

Lol... voila!!! It works... thanks so much !!!
```

---
## \#492 Posted by: nenecossais Posted at: 2018-01-08T08:59:08.292Z Reads: 229

```
Hello All
Many Thanks Namasaki for this BMS project 10s1p using Turnigy 2s/5000mah/60c.
As far as I understand you reach 16 miles range with 2 motors ?

I am curious to know How evolve board can reach 50 km range... and I would like to build an 30km range board.
My eskate is 1 motor 6374 3.2kW (from alien) 1 Vesc and 15*36 gear ratio.
With 2 batteries Zippy 5S 8000mAh in serial I get around 16km range.

Does anybody ever build battery system to get 30km range ?
I am thinking to build such Namasaki battery system with 10s2p (4batteries 5S 8000mAh) connected to bestech ?
```

---
## \#493 Posted by: Namasaki Posted at: 2018-01-08T12:56:50.100Z Reads: 231

```
My actual tested range is 14 mile max on flat ground. 
That’s running my pack down to 33v and running dual 6355s. 
Mileage will vary depending on rider weight, wind conditions and riding style. 
Stop and go vs constant cruising. 
I also have a build with same batteries and with dual 6374s. It gets less mileage because the larger higher torque motors draw more current. 
I don’t have a single drive for actual comparison but my theory is that mileage will be similar with a single or dual because the load is the same. 
Your just working a single Vesc and motor twice as hard as each Vesc and motor with a dual drive. 
Unless you increase the load beyond the limits of a single Vesc and motor.  Like climbing hills that are too steep for your single drive.
```

---
## \#494 Posted by: nenecossais Posted at: 2018-01-08T13:47:24.582Z Reads: 237

```
Thanks for info, for sure range depend on weight, flat ground, wheel, wind, straigh road ..

1 or 2 motor should be sligtly the same, I think you even get more range with 1 motor because of electrical switching lose, thermal and coupling lose. 
As example Buffalo board seems to switch long range mode by deactiving one motor.
```

---
## \#495 Posted by: TeslaAlex Posted at: 2018-01-29T15:29:49.288Z Reads: 248

```
Hi! This thread has been the inspiration for my own battery build, 4 x 3s 8000 mah 30C Lipos with a 12s 80A Bestech BMS. Everything has arrived at my house, and after a lot of reading Im quite sure about what to do next. I used your wiring diagram and converted it to 12s (the male/female part are 5.5mm bullet connectors). 

![12s Bestech BMS Wiring|690x459](upload://rhRQguPkABN16LW8CZu0vJBjdhM.png)


Having done this, I do still have a couple concerns. I read trough the whole thread and these are the questions I still wonder about. I would really appretiate if you could help me out! :slight_smile:

1. Should I configure my Focbox before connecting the BMS? 

2. At what voltage should the individual batteries be at when connecting to the BMS? At the moment, they are charged to "storage voltage" = 3.8V

3. How do I check the voltage of each individual cell, in the best way? Do I simply unconnect one lead at a time from the balance lead connector (after having connected the batteries in series) and use a voltmeter?

4. In what order should the components be connected to the BMS? Should the battery positive and negative be connected before the balance leads? Should the focbox be connected before the battery? 

Thanks a lot! 

/Alex
```

---
## \#496 Posted by: Namasaki Posted at: 2018-01-29T16:08:23.008Z Reads: 226

```
I’m at work now but I will answer your questions this afternoon when I get home.
```

---
## \#497 Posted by: gigoy Posted at: 2018-01-29T16:32:42.492Z Reads: 229

```
Very interesting. You should definitely do a video of this for reference/tutorial! Good luck!
```

---
## \#498 Posted by: Namasaki Posted at: 2018-01-30T01:51:02.327Z Reads: 237

```
Nice diagram!
**1.Should I configure my Focbox before connecting the BMS?**
It doesn't really matter.

**2.At what voltage should the individual batteries be at when connecting to the BMS? At the moment, they are charged to “storage voltage” = 3.8V**
3.8v is fine, 4.2v is fine, the important thing is that they are all the same voltage. But that should be done before putting the battery pack together.

**4.In what order should the components be connected to the BMS? Should the battery positive and negative be connected before the balance leads? Should the focbox be connected before the battery?**
First make sure the bms is turned off at the on/off switch connected to the E-switch wires.
Then connect the balance wires from the battery to the bms.
Then you can connect the Battery neg to B- pad and the Focbox neg to the P- pad and the charge port neg to the C- pad
Then connect the battery pos to the focbox positive and the charge port positive.
Once everything is connected, double check your wiring and make sure it's right.
Then turn the bms on to power up the Focbox for an initial test.
After the focbox finishes booting up, turn the bms off and connect the usb cable to the vesc and your PC and then turn the bms on again.
After the focbox boots up, open your Vesc tool or BLDC tool which ever you have and program the vesc.
Remember to turn the bms on when charging.

**Oops, I missed number 3.**

**3.How do I check the voltage of each individual cell, in the best way? Do I simply unconnect one lead at a time from the balance lead connector (after having connected the batteries in series) and use a voltmeter?**
You could first Turn the bms off, then unplug the balance wire connectors from the bms and check the battery voltage at the pins of the balance wire connector coming from the battery.

neg probe on battery neg main and pos probe on pin for bal wire 1 to measure cell 1
neg probe on pin for bal wire 1 and pos probe on pin for bal wire 2 to measure cell 2
neg probe on pin for bal wire 2 and pos probe on pin for bal wire 3 to measure cell 3
follow this pattern all the way to cell 12.
This is one way that you can check individual cell voltages with a multimeter. 
The pins are very close together so be very carful no to touch the neg and pos probes together while testing or you will cause a short.
```

---
## \#499 Posted by: mmaner Posted at: 2018-01-30T02:07:22.819Z Reads: 215

```
Good tutorial @Namasaki.  I was gonna do the same today but ran out of time.
```

---
## \#500 Posted by: TeslaAlex Posted at: 2018-01-30T06:04:35.328Z Reads: 216

```
This is amazing! Thank you for taking your time, everything just got a lot easier for me! This forum is the best! :grinning:
```

---
## \#501 Posted by: riva_00 Posted at: 2018-01-30T09:20:58.679Z Reads: 218

```
If only Namasaki had a tip jar......
```

---
## \#502 Posted by: Blitz Posted at: 2018-02-22T14:04:40.550Z Reads: 216

```
I was Reading This topic filled with knowledge for half an hour Cant get to the bottom maybe some other time :joy: Great topic Bruh. I've bought 3 (3s 8000mah 30c) zippy lipos for 81euro was that a good deal for range and power? I will run mono (190kv 2kw motor)

after reading this I got the Li-on's are better out of my head! I thought I was cheaping out :stuck_out_tongue_closed_eyes: Is my setup better than 9s3p q30?
```

---
## \#503 Posted by: mmaner Posted at: 2018-02-22T14:06:12.087Z Reads: 215

```
[quote="Blitz, post:502, topic:10014"]
Is my setup better than 10s3p q30?
[/quote]

It's close, the MAH is still a little bit lower, the amp delivery should be better, as always the charge cycles are less with LIPO's
```

---
## \#504 Posted by: Blitz Posted at: 2018-02-22T14:20:58.916Z Reads: 210

```
I get what your saying but The big question is, 240A 8ah Vs 45a 9ah  could the higher Amps make the range near the same?

Edit: changed 10s3p to 9s3p so comparison can be easier.
```

---
## \#505 Posted by: anorak234 Posted at: 2018-02-22T14:47:01.364Z Reads: 209

```
The debate between li-ion and Lipo continues...
(Btw lion is better XD)
```

---
## \#506 Posted by: mmaner Posted at: 2018-02-22T14:56:40.756Z Reads: 216

```
The more amps the less sag, the less sag the more you stay out of the throttle...so it 'could' equal, I dont know if it will but the difference is minimal, shouldnt be an issue.
```

---
## \#507 Posted by: Blitz Posted at: 2018-02-22T15:02:38.571Z Reads: 216

```
I just think that Lipo has a lot to offer on a lower price making it perfect for someone like me.
(FYI lipos are better):P
```

---
## \#508 Posted by: Namasaki Posted at: 2018-02-22T18:06:47.112Z Reads: 207

```
Me two.......
I like the high current output in a compact, light weight, inexpensive and easy to build solution where long range isn’t needed.
```

---
## \#509 Posted by: Blitz Posted at: 2018-02-22T18:33:21.473Z Reads: 215

```
Wait what my 8000mah lipos can't go far?
```

---
## \#510 Posted by: madlemgw Posted at: 2018-02-22T19:34:05.757Z Reads: 217

```
I have been reading this thread for a few days now and I'm thinking my mind has been changed.  I'm looking at building a MTB board with dual drive (190 kv 6364 motors) and I was going to use Li-on batteries but I'm now thinking of using Lipos.  I'm going to be using the board in a non-conventional way, on a golf course.  So I don't need speed (10-15 mph) and distance 10-15 miles should be plenty.  The course is rather flat a few good sized hills I would have to go up.  Do you think this setup with get me what I'm looking for?  I'm about 215 lbs and maybe another 15 lbs for my gear.
```

---
## \#511 Posted by: Namasaki Posted at: 2018-02-22T22:03:31.713Z Reads: 223

```
Better to go with 6374’s for low speed hill climbing. 
They have lots of torque. 
And Use large wheel pulleys
```

---
## \#512 Posted by: bloke900 Posted at: 2018-03-02T01:29:08.184Z Reads: 226

```
This thread has actually been inspiration for my first build. Thanks heaps Namasaki for putting the details up here - and an even bigger thanks for staying active in the thread! 

I originally had selected 5x Zippy 2s 8000mah 30c batteries, but seriously considering the 60c 5000mah even with the hit ill take to range. Would it make that much noticable difference to sag or general punch? 60c batteries would be up to 300a discharge, 30c would be 150a. In the real world on mostly flat ground, would this make much of a difference to the feel of the board to a 115kg skater? What would you choose? 5000mah 60c  (theoretical 16km range) vs 8000mah 30c (theoretical 27km range) 

Are the hardcase batteries physically strong enough to provide protection if they were not covered by an additional enclosure?  My gut is telling me dont even risk it, but I need to ask the question.
```

---
## \#513 Posted by: Namasaki Posted at: 2018-03-02T03:25:43.298Z Reads: 223

```

8ah x 30C is 240a but neither that or the 300a for my packs is truly accurate. They are overrated as are all Lipo packs on the market.

Still, My 60C packs work really well on hills and even better on flat ground and though I have not used the Zippy flight max, they should work well especially if your just riding on flats.
The Flightmax are a lot larger than the Turnigy 5000/60C which is why I didn't use them on my builds. I considered them but they where just too big.
The Turnigy's are very compact and the hard case is very strong. I tried to break one open once and had a hard time doing it. 
You may get a substantial increase in range with the Zippy 8000's especially on flats so if you need more range and have room for them, I would give them a try.
```

---
## \#514 Posted by: bloke900 Posted at: 2018-03-11T01:50:47.721Z Reads: 216

```
Thanks for your help.  The sizing really is quite different on those 2 batteries. I hadn't realised quite how much before now.
```

---
## \#515 Posted by: ltlderek Posted at: 2018-03-19T19:31:26.005Z Reads: 212

```
Forgive my ignorance: 

In my setup, I have two 4C 5000mah batteries in series. Basically, instead of connecting my  main + & - to the VESC , those will go into the BMS , and then go to the VESC, and my balance ports will (or can) go independently into the BMS, depending on the model...? or am I going to have to determine a certain pin out from there? I have these in an XT90 connection setup currently, but the batteries are barrel - XT90 converted (if that matters)
```

---
## \#516 Posted by: monny Posted at: 2018-03-23T08:56:22.729Z Reads: 201

```
would it be a problem doubling your battery pack ?

i mean using 10 pieces instead of five 5000mah 2s lipos (serial & parallel) to get 10000mah 10s
```

---
## \#517 Posted by: Namasaki Posted at: 2018-03-23T11:58:57.858Z Reads: 208

```
I believe it has been done
```

---
## \#518 Posted by: riva_00 Posted at: 2018-03-23T13:06:51.856Z Reads: 219

```
Read this m8y: -

http://www.electric-skateboard.builders/t/wiring-and-charging-advice-please/26839

I'm still currently charging my batteries through a balance wire splitter to a balance charger (charging 4~6 5s batteries at once), as I'm waiting for a BMS designed on here to be complete.

You can do it, but make sure you do it safely.
```

---
## \#519 Posted by: TeslaAlex Posted at: 2018-04-01T10:22:44.312Z Reads: 206

```
Just got my battery pack connected and ready to go. In what order should everything be connected and turned on when charging? Do I plug the charger in the board and then turn the charger on, and then the board? 

Thanks for your help! :grinning:
```

---
## \#520 Posted by: telnoi Posted at: 2018-04-01T11:35:32.439Z Reads: 206

```
If you have 4x, they work fine under any conditions.
In winter it has 0.8v voltage sag on a hill where my dual focbox craps out before I reach the top. Should be better once the Temps go up.
```

---
## \#521 Posted by: Namasaki Posted at: 2018-04-01T15:08:56.362Z Reads: 216

```
[quote="TeslaAlex, post:519, topic:10014"]
Do I plug the charger in the board and then turn the charger on, and then the board?
[/quote]

Yes, that sequence works best
```

---
## \#522 Posted by: dg798 Posted at: 2018-04-17T13:18:52.207Z Reads: 207

```
That’s a nice enclosure. Do u sell those and would it fit 6 of the 2s batteries and a single vesc and bms?
```

---
## \#523 Posted by: bigben Posted at: 2018-04-17T18:58:58.302Z Reads: 211

```
Hi,
I do sell them. Should be no problem with another 2s pack in there.
Here is my instagram for a few more pics.
https://www.instagram.com/bbenclosures/
The enclosure you were looking has 545mm internal length.
```

---
## \#524 Posted by: DevinG Posted at: 2018-04-20T00:40:28.764Z Reads: 206

```
Could I do something like 2 3s lipos in series with both packs having another in parallel?
Am I understanding that as 6s2p? 

I'm just trying to wrap my head around this for future upgrades.
```

---
## \#525 Posted by: Namasaki Posted at: 2018-04-20T01:00:59.471Z Reads: 202

```
Ya, that would be 6s2p and double capacity
```

---
## \#526 Posted by: webst Posted at: 2018-04-20T09:48:08.799Z Reads: 205

```
[quote="Namasaki, post:83, topic:10014"]
My packs are 10s 5000mah 60/120c  Thats a rating of  300a continuous and 600a peak
[/quote]
I don't know if anyone straighten this up yet (I haven't gone through all thread) but I believe this is not correct. You're using 2s battery so serial connecting 5 of them does not make it capable of putting 5 times the current through one of them. Only the voltage goes up. Current limits stay the same.
```

---
## \#527 Posted by: Jumpman Posted at: 2018-04-20T10:30:08.976Z Reads: 203

```
Each lipo is theoretically capable of 300A/600A, so he is correct.
```

---
## \#528 Posted by: Namasaki Posted at: 2018-04-20T11:58:14.095Z Reads: 209

```
@Jumpman 
I multiplied 5ah x 60c to get 300a. 
Some time later I learned that this formula does not equate the true current capability of Lipos. 
The true current capability of my battery is more like 80-90a. And that is just a guesstimate.
```

---
## \#529 Posted by: webst Posted at: 2018-04-20T13:29:35.926Z Reads: 206

```
My bad, I mixed C with Amps. You were right. So 7P of 30Q should give similar current to what you estimate your lipo has?
```

---
## \#530 Posted by: Jumpman Posted at: 2018-04-20T15:15:05.512Z Reads: 209

```
Thanks for the clarification.  I also don’t trust those figures, that’s why I said theoretically, but maybe I should have used a different word.
```

---
## \#531 Posted by: Jps224psu Posted at: 2018-04-24T02:02:30.653Z Reads: 213

```
![IMG_6905|666x500](upload://uddeMSsXcXAGOWYXHqhXzu4nUbn.JPG)

Here is my very artistic attempt at 12S LiPo schematics.   I hope it is close to right was wondering if folks can take a look and let me know where i went wrong.

list of stuff
Battery (3): Gens Ace 4s 7200mah 70C 
Jst extension wires: NEW 12" JST 4S LIPO BALANCE LEAD EXTENSION SILICONE 
BMS Bestech BMS with E-switch 12s  80a
Power switch: The BMS has a built-in e switch power switch use automotive switch to control it 
Charge port: power button for port
Charger: 44.4v laptop style charger 5A for mobileand/or (CC/CV lab power supply for home…Amazon.com: KORAD KA6005D -Precision Variable Adjustable 60V, )
Anti static wrist strap- 
can cable
10awg
5.5 bullets
4 bullet for motor cables (as vesc 6 has 4mm) (APS 8072S)

was thinking of Photon Remote plus app so didn't need any LCD on board...does it cover everything? if not get: 

Battery voltage meter-  DROK DC8-63V 12V/24V/36V/48V LCD Lead-acid Battery Capacity (amazon)
Switch for voltage meter- Amazon.com: E Support 16mm 12V 3A Car Green Light Angel Eye Metal Push Button Switch Socket: Automotive

few questions: i don't need loop key b/c i have e-switch?
is there anything else folks would add for protection or a nice to have? 

Thanks,
Justin
```

---
## \#532 Posted by: Namasaki Posted at: 2018-04-24T05:47:59.640Z Reads: 193

```
I don't see anything wrong on the diagram. The battery orientation and balance wires all look correct to me.
Great choice of batteries btw.
I have the Lab Power supply you mentioned, It works really well.
```

---
## \#533 Posted by: Hariboisawesome Posted at: 2018-04-24T06:12:06.219Z Reads: 202

```
Similar situation. I’m stuck at the balance wires. 2 6s setup. ![image|375x500](upload://yl1kjOfX2wsuiQvwRpv8G2XZhOM.jpg)
```

---
## \#534 Posted by: Jps224psu Posted at: 2018-04-24T18:26:50.264Z Reads: 193

```
Thanks @namasaki do you agree that i don't need any voltage meter/battery indicator if i have a remote that displays it?  Or you think its a good idea to put in? Thinking photon remote will be able to display all that is necessary and app can record my data while riding. Also for the Lab power supply...dumb question here but if i have a female DC charging port (5mm x 2.1mm) in board do i just manufacture a male cable to go from lab power supply to board? thx
```

---
## \#535 Posted by: Namasaki Posted at: 2018-04-24T21:02:39.279Z Reads: 195

```
It has been my experience using the metr Bluetooth module and app that it does not report accurate battery voltage. 
I contacted the seller and app creator about this and he said that the Vesc 4.12 does not report voltage to the module correctly. 
My module and app usually reports voltage about one half volt higher than actual voltage. 
So  you can use the remote to monitor but compare with a multimeter for a reference
```

---
## \#536 Posted by: Jps224psu Posted at: 2018-04-24T21:19:05.120Z Reads: 201

```
![image|371x500](upload://lACm47b4x2XVjwUyVwJ9xTQDeSz.jpeg)

Search some of those keywords from that post looks like plenty out there on 6s2p. Gotta sift through the garbage to find the good stuff. In my experience many of the answers are out there. If you want people to tell you how to do it answers dont come in too often. Its a friendly atmosphere but not that friendly. 🤟
```

---
## \#537 Posted by: Jps224psu Posted at: 2018-04-24T21:22:15.299Z Reads: 178

```
Thanks dude. Appreciate it. Wonder if they fixed w vesc 6 will do aome research. Prob opting out of display on board less electronics soldered in less problems. Was i right on the lab charger? Just create male dc from charger to board? Or better way to do it?
```

---
## \#538 Posted by: rich Posted at: 2018-04-24T23:01:17.792Z Reads: 176

```
Well done @Namasaki :clap::sunglasses:
Just wanted to say this is really a great thread full of information and I appreciate your support to help others (including me). And 28.6k views is truly impressive!

Keep it up!
```

---
## \#539 Posted by: Namasaki Posted at: 2018-04-24T23:46:46.724Z Reads: 201

```
[quote="Jps224psu, post:537, topic:10014"]
Just create male dc from charger to board? Or better way to do it?
[/quote]


Yes, just make a charge cord to plug into the Power supply and your charge port.
Two other points of interest.
1: use a multimeter to check the output of the Lab power supply. Just to insure the accuracy of charge voltage.
2: I have found that when charging with the power supply and the Bestech HCX-223V1 bms it works better when you follow these steps.
1. Plug the power supply in and turn on the main power.
2. Adjust the voltage and current on the Power supply, check it with a multimeter.
3. Connect the charge cord from the power supply to the charge port.
4. Turn on the output of the power supply then immediately turn on the bms.
The power supply will begin in CC mode with the voltage staying just a little above the pack voltage.( this reduces battery heat during the charge process).
Once the battery gets close to the set voltage, the power supply will automatically switch to CV mode and stay at set voltage while the current will steadily drop until the battery is fully charged.
Note: The power supply will not shut off when the battery is fully charged but it's output will decrease to about 50ma. At that time you simply turn off the power supply output (NOT THE POWER BUTTON)
Then turn the bms off and disconnect the charge cord.
Note: If you turn the bms on before the power supply, it has a tendency to confuse the power supply.

Main power button ![15 PM|134x101](upload://f8xWUg8ybe3PNvCVnzG8VphCQLk.png)

Output on/off. ![27 PM|85x59](upload://jFqRFKAqnCEl59syZTdjBRfZZpQ.png)

![42 PM|382x500](upload://lBwUaId1toCx81GXb5ubWAhudQw.png)
```

---
## \#540 Posted by: Jps224psu Posted at: 2018-04-25T01:24:06.683Z Reads: 180

```
Really appreciate it @Namasaki. Looking fwd to getting this thing up and running.
```

---
## \#541 Posted by: Hariboisawesome Posted at: 2018-04-25T07:34:53.730Z Reads: 181

```
I've actually spent about 4 hours reading various post about BMS and lipos together. Tried a couple of different ways that I thought I understood to be correct. Turns out that I'd misunderstood because my BMS started to get pretty hot for a split second. That's what lead me to post. I'm not asking for anyone to do work for me. Thanks again for the images though
```

---
## \#542 Posted by: Jps224psu Posted at: 2018-04-25T12:33:03.998Z Reads: 192

```
Our friend Lucy @bestech came back on the BMS I was going to order one i had found many people in forum have used before and she said that one is no longer available but she has an upgraded one. hcx-d528v1 It has e-switch as well and spec sheet seems to be ok outside the short circuit protection at 480a.  Does anyone have experience with this BMS? Regardless of what i order I will most most likely have an extra one due to the min 2 order. so will post if folks are interested.  hcx-d528v1 ![hcx-d528v1|690x335](upload://1gDhwHacjxg5YOeISxvvIo1eFg5.png)
```

---
## \#543 Posted by: Namasaki Posted at: 2018-04-25T12:50:14.651Z Reads: 190

```
Tell her the short circuit detection is too high and needs to be lowered.
```

---
## \#544 Posted by: Jps224psu Posted at: 2018-04-25T13:27:43.794Z Reads: 183

```
Thanks @Namasaki what "a" would you recommend i ask her to lower to given my set up?  Also i am not sure how to wire this based on not having a C- but i guess i can figure that out later.  I also went back to ask if there were any more HCX-D223V1 avail....seems to be the one everyone likes...
```

---
## \#545 Posted by: Namasaki Posted at: 2018-04-25T14:24:55.580Z Reads: 174

```
Short circuit detection should be close to the over current detection, maybe even the same.
```

---
## \#546 Posted by: Jps224psu Posted at: 2018-04-25T14:31:13.233Z Reads: 174

```
thx assuming the second over current protection (240A+-40A)
```

---
## \#547 Posted by: Namasaki Posted at: 2018-04-25T14:35:11.669Z Reads: 182

```
No, I would have it set with the 1st detection value and I would have them lower the 2nd value. 
I’m not even sure why they have dual over current detection.
```

---
## \#548 Posted by: Jps224psu Posted at: 2018-04-26T12:24:39.665Z Reads: 171

```
FYI- still going back and forth with Lucy.  She mentioned they cannot set values on the hcx-d528v1 the same so i asked for 160 (1st)/170 (2nd) /180 (Short).  She came back saying that many people use this PCB for eks8 as is, I informed her many members think those values are too high so she is checking with her engineers to see what can be done.  Its too bad they don't carry the older (seem to be better) versions.  Anyone have any other suggestions on model #'s w eswitch?
```

---
## \#549 Posted by: Jps224psu Posted at: 2018-04-27T11:53:52.554Z Reads: 175

```
I guess I am just going to go with it for now despite numbers not being great....here is message from Lucy so everyone has transparency:

Hi Justin, 
  
I got news from our engineer, it's suggested over charge detection current (1) 160A+/20A, over charge detection current (2) 225A+/40A and short circuit detection current 450A+/40A. 
  
Awaiting for your feedback soon.
```

---
## \#550 Posted by: Namasaki Posted at: 2018-04-27T11:57:18.506Z Reads: 170

```
Tell her that our application doesn’t run that high current and the wiring can’t handle 200a let alone 450a
```

---
## \#551 Posted by: Jps224psu Posted at: 2018-04-27T12:03:55.891Z Reads: 172

```
@Namasaki....done.  Will let you know...i also asked if there is another BMS model w eswitch that fits our requirements (maybe not on website as her email suggests " We have more than 30,000 different PCM/BMS designs, we cannot upload all to our site, please email us if you can not find what you need on our site.")
```

---
## \#552 Posted by: skatardude10 Posted at: 2018-04-29T04:40:51.982Z Reads: 183

```
Well, I just read through this thread... great stuff!! Right now I am just doing some research to see if it would be feasible to setup a 12S2P setup with lipo batteries. 

First, there aren't many posts on doing 2P with BMS... what would be the best way to do this? Can you really only truly balance 1P setups? Would a 12S2P lipo setup be (WAY) too bulky? I don't mind having quite a bit of bulk if it means more range and more available power.

Second question... with an 80A discharge BMS, this limits me to 40A on each vesc, correct? What if I wanted to run each VESC at 60A, would I need a 120A BMS? Or do I have this wrong, and I could use a 12S 80A BMS?
```

---
## \#553 Posted by: Namasaki Posted at: 2018-04-29T06:04:07.030Z Reads: 180

```
I run my Vescs at 50a batt max in a dual setup and have never had a problem.
The Bestech 80a can handle 80a continuous and  peaks up to 240a.
On a street board with 90mm wheels, it's doubtful that you would every pull even 80a total with a dual drive regardless of what you set the batt max at.
On a EMTB with large off road wheels and tires, it might be a different story.

I ran a test once with12s going uphill at 1/2 throttle using an inline watt meter in between the batteries and the ESC's and I was pulling only 18a from the batteries. That was total current draw with a dual drive.

Then I switched my batteries from series to parallel and ran the sane test on 6s at full throttle and pulled only 36a total.
```

---
## \#554 Posted by: skatardude10 Posted at: 2018-04-29T06:17:35.721Z Reads: 184

```
According to my logs, when I had my battery max set to 40 on each vesc, I would pull 60+A continuous (75A total when full acceleration dropping to 60-65A continuous) very often due to my gearing, all the time accelerating really. I love the power, but my lions sag a bit too much pulling 80A total. Limited to 60, they sag muuuuuch less, but still I pull 60A pretty much all the time accelerating.

I'd love to be able to up my settings to 60A each vesc. I think the amp draw has to do with the fact that I go full throttle often, weight 90+ kg, board weighs quite a bit (numbs my hand after a minute of holding it, lol), and it's geared for 38mph... But 30A per vesc doesn't get me there *ultra quick*. 40A per vesc is a bit quicker, but I'd love to accelerate faster than 40Ax2 does. I tried a few other gear ratio setups, and acceleration wasn't immensely better and top speed was reduced drastically. 

If I can keep my gearing or even lower it more and let loose with the extra amps lipos can provide for all the more power, I'd be in love.
```

---
## \#555 Posted by: webst Posted at: 2018-04-29T10:38:57.081Z Reads: 192

```
[quote="skatardude10, post:552, topic:10014"]
First, there aren’t many posts on doing 2P with BMS… what would be the best way to do this? Can you really only truly balance 1P setups?
[/quote]

Batteries balance themselves parallely so don’t worry about it. BMS is used for series balancing as this doesn’t occur by itself.

Here, I’ve drawn something that should make it easier to grasp the concept:

![image|566x500](upload://durUPrT0xYKvcrbFcoWVwYhHn0T.jpeg)
```

---
## \#556 Posted by: sayekim Posted at: 2018-04-29T13:54:24.552Z Reads: 198

```
Damn this really shows what an extra 20 kilos does to batt amp demand. 

Not sure I can compare it really well but I only pull 46 amps for dual hub motors and I weigh 72 kilos and have batt amps set to 25 for each focbox. 

https://metr.at/r/iu356

You have a metr log for comparison?
```

---
## \#557 Posted by: Namasaki Posted at: 2018-04-29T18:09:19.270Z Reads: 185

```
Nice illustration @webst
It’s so simple when you think of electrons  as water. 
Voltage is like water pressure 
Current is like flow
```

---
## \#558 Posted by: Jps224psu Posted at: 2018-04-30T13:27:01.647Z Reads: 182

```
for those interested....reply from Lucy over wknd 

 "Hi Justin, 
  
According to your requests, the short circuit current is 360A we have so far. "

Obviously some interference in the communication lines but 360a is not much better....I have gone ahead and ordered the HCX-D223V1 bestech BMS from alien power systems.  Although bestech says they dont make that model anymore APS claims to have them. So not sure if they are avail or not from bestech or you have to buy through APS.  I am getting railroaded on the price and shipping to US.
```

---
## \#559 Posted by: Jps224psu Posted at: 2018-05-08T00:27:46.500Z Reads: 179

```
Aps came through with the HCX-D223V1 bestech BMS ....delivered today. I spoke w Bruno at APS he said they just ordered them and had not heard they stopped making them. So for the timebeing you can get them there, it cost a bit much but better than your board burning to the ground with these “upgrades” Lucy is recommending. Last pc of puzzle is photon remote then i can get to building. Im sure ill be back w some questions.
```

---
## \#560 Posted by: webst Posted at: 2018-05-08T10:11:18.697Z Reads: 181

```
@Namasaki what is the lower voltage limits you set with your LiPo pack? I asked HobbyKing staff about [this](https://hobbyking.com/en_us/graphene-7500-mah-2s2p-hardcase-w-5mm-female-bullet-connector.html) battery and been told that 3,7V is safe lower limit which seems pretty high for me. I still have to measure how many Ah can I get from them within this voltage range soon and post here. @uigiroux you might be interested if you still consider this pack.
```

---
## \#561 Posted by: Namasaki Posted at: 2018-05-08T12:01:54.876Z Reads: 179

```
I’m still using this battery build on both of my boards. 
I monitor voltage while riding and usually go no lower than 3.6v
I did go as low as 3.3v for a max range test once. 
But I would not do that on a regular basis.
```

---
## \#562 Posted by: moon Posted at: 2018-05-08T12:38:17.928Z Reads: 176

```
I think the batteries are out of stock now :frowning:
```

---
## \#563 Posted by: Namasaki Posted at: 2018-05-08T15:04:51.688Z Reads: 176

```
Keep an eye on it. They most likely will get more or you can get them on eBay. Ebay price is higher though.
```

---
## \#564 Posted by: Jps224psu Posted at: 2018-05-14T15:36:48.158Z Reads: 176

```
Hi all,

had a couple quick Q:

1) I assume the eswitch wiring doesnt matter (no + or -) as you are just creating loop?

2) Balance cable wiring- I noticed on primary battery pack (+) you start off the balance cable wiring with the red wire in slot 12 for a 12s set up.  I noticed on my diagram and @Namasaki on the last battery the red wire is going to BMS (while ignoring all the grounds) on other set ups i see people skipping the last battery red wire and then using the last ground to run to BMS?  A little confused by this.

thx.
```

---
## \#565 Posted by: Namasaki Posted at: 2018-05-14T17:15:34.969Z Reads: 176

```
Answers 

1.  That is correct

2. The first cell in series provides the negative main. 
The last cell in series provides the positive main. 

The balance wires start at the first cell and count up to the last cell.
```

---
## \#566 Posted by: Jps224psu Posted at: 2018-05-14T22:12:04.200Z Reads: 179

```
![image|375x500](upload://ytddUMBQ1cBrcbCSdeUpwpfNQSy.jpeg)

So here is what i came up with. Starting from left to right first red is b12 then b11-b9 (skip last black wire from battery grnd? Also since jst ext is 5s i would skip the last two black wires and then start the next battery red wire in b8 same thing to b5 then last battery red wire b4 and same thing down to b1. Do any of the balance wires go to b- on the bms or just the main neg from battery?
```

---
## \#568 Posted by: Namasaki Posted at: 2018-05-15T00:19:33.637Z Reads: 167

```
The red wire is always the last cell in series of a pack.
So the cells count down from the red wire but the last wire or the wire furthest from the red wire is always ground.
```

---
## \#569 Posted by: Jps224psu Posted at: 2018-05-15T01:24:44.610Z Reads: 163

```
Thanks @Namasaki. I think I have it now, sorry my description wasn't too great.  I am skipping all the grounds on the lipo (furthest from red) as well as the 6th cable on jst ext.  Red (+) wires will be on b4, b8, b12.  Last question (sorry appreciate the help don't want to screw this up) I don't need the final ground to go to b- on bms right?  Just the negative of battery to bms not both.  I saw mixed ways of doing on youtube.
```

---
## \#570 Posted by: Namasaki Posted at: 2018-05-15T01:43:51.602Z Reads: 163

```
It depends on what bms your using.

Ok, I see your using the same bestech that I used.
With that bms, you don't need to use any of the balance ground wires.
Just run the main ground cable from the first battery pack in series to the B- pad
as shown in my diagram.
That bms uses the main ground instead of the balance ground wires.
```

---
## \#571 Posted by: Jps224psu Posted at: 2018-05-15T02:00:04.626Z Reads: 163

```
perfect..thx dude!
```

---
## \#572 Posted by: Muke Posted at: 2018-05-16T14:39:27.384Z Reads: 174

```
[quote="Namasaki, post:280, topic:10014"]
remove the charger, let the cells balance down and then put the charger back on
[/quote]

So am I right to conclude that if I leave my board on with the charger unplugged it will balance the battery at a lower voltage than 42V? (for example also at 39V for a 10s setup?) 
If yes, how long do you leave the board on?
You said ''let the cells balance down'', does that mean the voltage of the whole pack will drop slightly when the BMS balances the cells?

And another question: do you trust the switch to turn off the board completely or do you still plug out the battery over night?
```

---
## \#573 Posted by: Namasaki Posted at: 2018-05-16T17:02:14.473Z Reads: 177

```
Your batteries really should be balanced before connecting them in series to the bms.
The bms trims high cells down to match the lower cells when balancing.
From my experience it appears to do this even when the bms is off.
As far as balancing the cells when the total voltage is below 4.2v per cell, I have not done a conclusive test to prove it however it does appear to do so.

The built in E-switch is adequate for turning the whole board on and off.
I have left my board's sitting in the closet with the battery connected and the E-switch off for more than a week without adding charge to the battery but checking them periodically  and they are holding their charge very well.
```

---
## \#574 Posted by: Jps224psu Posted at: 2018-05-24T15:38:10.622Z Reads: 175

```
This is an awesome thread and just wanted to thank @Namasaki for all his help both in this forum and directly through PM. I have one last issue i am trying to resolve been talking to jens @Nowind as well. Dont see a great forum for this and too many new topics started so figured i would ask here. Hoping someone can help. I will share a video want to get your thoughts of what noise could be. In bench test it seems to be coming through both motors so I am not thinking defective but maybe you can lead me in right direction. Noise happens about 1/2 throttle or more and also when coasting from time to time. 

Set up:
12s1p
Dual vesc 6 in bldc hybrid mode
Settings are well below what motor can output
Checked for loose screws etc

Nothing so far. 

Youtube link:

https://youtu.be/DE93rrBXcmM
```

---
## \#575 Posted by: Jps224psu Posted at: 2018-05-24T17:13:30.257Z Reads: 167

```
Other thought is could it be the chain and maybe too tight?
```

---
## \#576 Posted by: trampa Posted at: 2018-05-24T17:19:13.795Z Reads: 162

```
Try FOC. FOC will eliminate noises from the motor. Thos way you can see if the noise is mechanical noise from the drive train.
```

---
## \#577 Posted by: Jps224psu Posted at: 2018-05-24T17:52:37.694Z Reads: 164

```
thanks Frank but FOC wont work at all...i have tried to configure at least 10 times (no exaggeration)  each time wiping vesc w firmware update and starting from scratch... the behavior is bizarre.  Sometimes, only master vesc will work and inverts direction of wheel, other times both wheels spin in right direction but just go full throttle and lose connection.  ThenI  have to wipe vesc and go to BLDC hybrid to get to work again.  If it try to go back without wiping vesc crazy stuff happens in BLDC mode as well.  FOC seems totally unstable for some reason. Just talked to my motor head friend who works on motorcycles he suggests 

Chain too tight causing lateral torque
check bushings/inner motor for vibration/markings
check motor mount and cog/gear alignment using laser
balance tires on a spindle

so guess i will try that.  If anyone can explain the FOC madness happy to listen and try again.
```

---
## \#578 Posted by: webst Posted at: 2018-05-24T17:59:25.397Z Reads: 152

```
[quote="Jps224psu, post:577, topic:10014"]
Sometimes, only master vesc will work and inverts direction of wheel, other times both wheels spin in right direction but just go full throttle and lose connection.
[/quote]

It inverts direction because one motor is pointed to the left and one to the right. There is option in vesc tool to invert it so both go the same way. Try to go FOC one more time, invert one motor, configure CAN, properly configure remote and tell us what happened.
```

---
## \#579 Posted by: trampa Posted at: 2018-05-24T18:02:34.899Z Reads: 147

```
Do single motor, single VESC first. Test each VESC with each motor.
```

---
## \#580 Posted by: trampa Posted at: 2018-05-24T18:05:00.269Z Reads: 150

```
And try without the sensors plugged in.
```

---
## \#581 Posted by: Jps224psu Posted at: 2018-05-24T18:11:53.416Z Reads: 159

```
Thanks @webst I def know of the inverted option i have to click it each time in BLDC hybrid for the slave to invert.  I have Photon remote so I cant config per se.  I set to UART, 115200, in nunchuck tab control mode= current w no reverse then i config in remote itself. remote hasnt been an issue at all in bldc once i  got it up and running so shouldnt be that.  @ trampa i have always done one vesc at a time and they both work that way.  Problem is when i connect them either both spin in right direction at full speed then dies out or only master spins i can usually control for a few brakes/revs then that revs up and dies out.  I do not have CAN connected until the slave config.  I have not tried without sensors connected.
```

---
## \#582 Posted by: Jps224psu Posted at: 2018-05-24T18:15:28.958Z Reads: 152

```
how exactly would i do w/o sensors should i still select hall sensors during motor wizard despite them being unplugged and I would assume the motor resistance and flux linkage do not need sensor to calc?  When do i plug in sensors and what settings would i manually update in config.
```

---
## \#583 Posted by: trampa Posted at: 2018-05-24T18:22:10.849Z Reads: 164

```
Only CAN L and CAN H connected I guess. Some managed to connect all four pins... 

I would do the detection with very loos chain. I would compare the values the same VESC measures for both motors. Then do the same with the other VESC. Especially the resistance and Lambda are of interest.

This way you can see if one motor or VESC has a problem. 
Bench tests do not give a lot of feedback, since VESC use current control.
```

---
## \#584 Posted by: webst Posted at: 2018-05-24T18:22:26.044Z Reads: 158

```
Just unplug sensors and omit them in motor detection wizard. Do not plug them now and tell us if it's working.
```

---
## \#585 Posted by: Jps224psu Posted at: 2018-05-24T18:30:26.354Z Reads: 158

```
Will do.  I only have the two pins connected removed 5V and grnd. Will check settings in wizard and without sensors (omitting them as well) will report back.  I have this one problem in the way called work...ugh.  @webst when your picture is small I see Jesus, when it gets larger nothing but the dude of life. I will refer to you as "His dudeness, duder, or el dudorino"  Thanks for the help.
```

---
## \#586 Posted by: Jps224psu Posted at: 2018-05-24T18:34:58.215Z Reads: 153

```
oh yeah if it does work when do i plug sensors back in? Just in case no one is around later.
```

---
## \#587 Posted by: webst Posted at: 2018-05-24T18:39:59.345Z Reads: 159

```
I changed it when somebody called me dude for being the janitor here. If it works then try to ride sensorless for a moment and check if it doesn't come back. Just push the board a little when at zero speed.
```

---
## \#588 Posted by: Jps224psu Posted at: 2018-05-24T23:49:28.659Z Reads: 160

```
Took it all apart. Happening without wheels and chains. Trying to set up foc. Makes noise and fails on flux linkage. Thats a new one. Updated vesc tool to .94
```

---
## \#589 Posted by: Jps224psu Posted at: 2018-05-24T23:50:32.504Z Reads: 169

```
![0af26423ceabd6735524eeaa757de11e2756fdb6|666x500](upload://25UsPjV1F7FXXAtT0PNqTvx24W5.jpg)
```

---
## \#590 Posted by: Namasaki Posted at: 2018-05-25T00:24:37.607Z Reads: 176

```
BLDC motor noise is normal and varies between different motors.
These are all sensorless. The last video is Carvon V2 with car esc's.

https://youtu.be/w_bjUQyZIqo

https://youtu.be/xY2gTAUL5IQ

https://youtu.be/eSeTWe-GI8U

https://youtu.be/B2-BbF6I8E4
```

---
## \#591 Posted by: Jps224psu Posted at: 2018-05-25T00:28:56.224Z Reads: 166

```
Thanks im ok w a little noise but something is up now. I wiped and installed fiemware on vesc it wont detect in bldc or foc for either motor. Running vesc tool .92 and .94 failed in both
```

---
## \#592 Posted by: Namasaki Posted at: 2018-05-25T00:30:02.158Z Reads: 168

```
Are you doing detection with drive train on?
If yes, try disconnecting the drive train.
too much load on motors might cause detection fail.
You also might try replacing the bearings in the motors. They can cause a lot of noise.
```

---
## \#593 Posted by: Jps224psu Posted at: 2018-05-25T00:32:57.725Z Reads: 173

```
https://youtu.be/iDt37Zpdzf8
```

---
## \#594 Posted by: Jps224psu Posted at: 2018-05-25T00:39:57.097Z Reads: 169

```
Cover your ears for that. And i try on unmounted motor too w/o jens adapter for 80mm same shit
```

---
## \#595 Posted by: Namasaki Posted at: 2018-05-25T00:42:18.448Z Reads: 168

```
You see how noisy my Alien HEV 6374's are.
My Alien HEV 6355's are a lot quieter.
Some motors are just louder than others.
Don't know why it keeps failing detection though.
```

---
## \#596 Posted by: Jps224psu Posted at: 2018-05-25T00:44:52.574Z Reads: 170

```
Yeah this is another level loud. Iphone not doing justice and why are cant figure out why they both failing detection now in both bldc and Foc? The original noise came and went like grinding. So it wasnt a natural motor sound from what i can tell. Now im just straight up stuck.
```

---
## \#597 Posted by: Jps224psu Posted at: 2018-05-25T01:09:14.818Z Reads: 176

```
https://youtu.be/EekzA727k3c
```

---
## \#598 Posted by: Jps224psu Posted at: 2018-05-25T01:09:50.764Z Reads: 172

```
This is the other vesc and bldc mode failing on both vescs now and both motors. Wtf
```

---
## \#599 Posted by: Namasaki Posted at: 2018-05-25T02:24:48.538Z Reads: 164

```
Could be that those motors are just very loud.
My APS 6374's are much louder than my APS 6355's
```

---
## \#600 Posted by: Namasaki Posted at: 2018-05-25T02:26:11.082Z Reads: 166

```
what voltage are you using to do motor detection?
if your using 12s, that might be the problem with failing detections.
Maybe a stab in the dark but sometimes you gotta look under every rock to find a problem.
```

---
## \#601 Posted by: Jps224psu Posted at: 2018-05-25T03:30:39.223Z Reads: 168

```
Yep 12s. It worked everytime before today who knows though i have an old lipo lying around i can try. 5.5hrs and im in a worse spot then before. I can get foc to recognize now by changing detection values. Same prob as before though once its all hooked up one push of remote and it goes haywire and cuts out thats with or without sensors. Now when i try to go back to bldc even with clearing firmware and changing to same values that works with foc i get bad detection error. Give up for today. Thanks for help everyone.
```

---
## \#602 Posted by: trampa Posted at: 2018-05-25T18:27:44.510Z Reads: 165

```
When you say wiped the FW, did you use VESC-Tool or an ST-Link?
```

---
## \#603 Posted by: Jps224psu Posted at: 2018-05-25T18:31:10.248Z Reads: 175

```
I used vesctool and reinstalled fw. I cant get bldc to connect and remote works fine when it was in bldc. I contacted @Wajdi who thinks it may be vesc. Was working w @Ackmaniac for awhile trying to trouble shoot. In bldc i get bad detection reult detection failed. Tried different usb cables, computers, diff versions of vesc tool, you name it. Im 10 hrs deep now. I can get it to connect in foc but it just revs and dies. No fault codes.
```

---
## \#604 Posted by: Jps224psu Posted at: 2018-05-25T18:32:52.862Z Reads: 178

```
![image|666x500](upload://8Lv7ZKLoPAT3SAgsmbAOXjVqGWj.jpeg)
```

---
## \#605 Posted by: Jps224psu Posted at: 2018-05-25T18:34:16.626Z Reads: 170

```
Foc only works when i reduce i c w. If i try that in bldc just fails no matter what values i put in there also tried lowering motor and battery current max for purposes of detection. That failed too
```

---
## \#606 Posted by: trampa Posted at: 2018-05-25T18:41:52.006Z Reads: 171

```
Since you have a problem with two ESCs, it's a bit funny. The chance to have two faulty devices is close to zero.
```

---
## \#607 Posted by: Jps224psu Posted at: 2018-05-25T18:51:53.112Z Reads: 169

```
I dont know what it is but any idea why bldc mode wont detect motor any work arounds? Software?
```

---
## \#608 Posted by: Jps224psu Posted at: 2018-05-25T19:10:12.059Z Reads: 169

```
I dont know what it is but any idea why bldc mode wont detect motor any work arounds? Software?
```

---
## \#609 Posted by: webst Posted at: 2018-05-26T11:51:50.728Z Reads: 170

```
Considering all the strange behavior and both motors and vescs having the same problems I’d suggest to try to find someone near you with working setup and cross check everything. I know this is barely a solution but considering the facts and that you already contacted pretty experienced guys I don’t see better solution.
```

---
## \#610 Posted by: Jps224psu Posted at: 2018-05-26T21:35:20.579Z Reads: 162

```
Thanks man. Still trying.....
```

---
## \#611 Posted by: Jps224psu Posted at: 2018-05-27T00:01:14.502Z Reads: 165

```
Getting closer and convinced its a software issue. I had changed the original master to a slave despite loading new firmware many times. When i went back and made the original master the master again i got bldc to connect only on the old master vesc. The slave wont connect. Trying foc and using original master but it could def have something to do with it.
```

---
## \#612 Posted by: Jps224psu Posted at: 2018-05-27T01:31:02.390Z Reads: 165

```
Got foc to run again but cuts out. Just like before. Tried bldc wont detect motor w or w/o sensors.
```

---
## \#613 Posted by: webst Posted at: 2018-05-27T06:35:53.803Z Reads: 166

```
Measure both motor coils impedance. It should all measure the same.
```

---
## \#614 Posted by: DevinG Posted at: 2018-05-27T16:32:30.636Z Reads: 182

```
Im gonna try and build a setup like this thanks @Namasaki
```

---
## \#615 Posted by: Jps224psu Posted at: 2018-06-01T02:11:59.544Z Reads: 186

```
Hey everyone. 20 hours later there were two issues that i think may be solved. The first was setting up master on one vesc and then changing master to other vesc and despite using vesc tool to clear it, it never really forgets setting @trampa said to use stlinkv2 to flash and seemed to fix the software issue. (Thanks Frank) Next issue photon remote receiver. Even after flash it would rev up and shut off. Was about to lose hope but my man @namasaki sent me a mini rc remote and it paired and worked for 20 min flipping power to board on and off many times. No issues. Have to take a test run to declare it fixed but looking good for anyone who gave a sh*t. Thank you everyone who helped me through this certainly some really good trouble shooting tips for future sufferers. Cracking beer to celebrate what seems to be fixed.
```

---
## \#616 Posted by: Gandinator Posted at: 2018-08-05T11:14:40.159Z Reads: 175

```
Hi,

I know this is a year later but I'm making my board now. I have a similar 10S set-up however, I was planning to buy a BMS from ebay with 60A over discharge. There is no e-switch though. My plan was that I connect the balance cables to the BMS. Then the negative wire of the charging port to the C or CH port on the BMS. Then this guy I saw on youtube (https://www.youtube.com/watch?v=_yrYG5skwvs&t=1043s --- 9 minutes in) has some "extension cable" which has +/- wires connected to xt90s (apparently used to be JSTs). One end of the xt90 goes into the series adapter xt90 from the 2 batteries (2x 5s) and the other end of the xt90 goes into a ON/OFF switch (then VESC).

As for the added +/- wires on this "extension cable", as said before the positive wire connects to the positive of the charger port and the negative goes to the B- port of the BMS. 

I also wanted a monitor so if i connect the negative lead of the monitor to the B- port and the positive lead to where the positive wire of the charger port and "extension cable" positive wire had joined. 

I would really appreciate your comments on this. I would be very grateful.

thanks
```

---
## \#617 Posted by: Namasaki Posted at: 2018-08-05T23:07:34.099Z Reads: 163

```
The Supower 60a bms is a good choice and can be used with an external E-switch or a Loop Key to turn your board on and off.
I personally would not use a low amp bypass bms like the one shown in the video you posted.
My reason is that when you bypass the bms during discharge, you cancel it's ability to protect the battery from over discharging and from short circuiting.
Sure you can use the vesc to protect against over discharge but the Vesc can only monitor the battery as a whole.  A bms monitors each and every cell or cell group individually.

I also believe that the fewer high current connections you have, the better.
I solder my packs together in series and the main ground from the battery is also soldered to the B- pad on the bms with no connector in between.
```

---
## \#618 Posted by: Gandinator Posted at: 2018-08-06T09:14:00.841Z Reads: 152

```
Hi Namasaki,

Thanks for the help. I saw the diagram you posted about connections with the BMS. It may have been on a different thread. I'll follow that too but what I said in my previous comment about the connections, does that seem fine in terms of proper connections. I think negative "extension cable" that goes to the VESC should go to the P- port but is everything else seem good?
Thanks
```

---
## \#619 Posted by: Namasaki Posted at: 2018-08-06T14:54:17.623Z Reads: 153

```
I’m having a little trouble visualizing your description. 
Better if you draw a diagram and post that. 

Bottom line, my advice is to keep the wiring as simple as possible with as few connectors as possible.

And I’m not sure if your aware of this but you can’t just use any old switch on the high current circuit. 
You’ll need an antispark loop key or an antispark E-switch
```

---
## \#620 Posted by: b.sk8 Posted at: 2018-08-06T16:41:33.589Z Reads: 153

```
@Namasaki Could you suggest a BMS for 12S-10000mAh-25C Lipo ? I will use it for dual setup ( 2 flipsky 6.6)  I am not sure if you would need more details.  Even better if you have a tutorial or diagram for 6x 2s Lipo with BMS.  Thank you for all your efforts in the forum!
```

---
## \#621 Posted by: Namasaki Posted at: 2018-08-06T19:02:41.659Z Reads: 159

```
The bms used in this thread is also available for 12s. 
Follow the 10s diagram posted in this thread and just add 2 more cells.
```

---
## \#622 Posted by: Gandinator Posted at: 2018-08-06T19:59:52.090Z Reads: 169

```
Hi Namasaki,

Your help once again is grately appreciated. 

I agree I need to keep the wiring as simple as possible.
I am also aware I can't use any switch. Though expensive I was going to use one of those high amp switches available on torqueboards or something. 
This is my plan below

Is it ok?

![IMG_20180806_205647|690x388](upload://kBHGzYaHQ4KsmUGVhVjzoabncLR.jpg)
```

---
## \#623 Posted by: Namasaki Posted at: 2018-08-07T02:02:00.274Z Reads: 162

```
your diagram is not correct. 
The wiring to the bms is not correct. 

First thing you have to do is decide exactly which bms you will use because they are not all the same and are not all wired the same.
```

---
## \#624 Posted by: Gandinator Posted at: 2018-08-07T08:42:07.603Z Reads: 157

```
Thanks for your help I'm such a noob.
I've got this BMS https://m.aliexpress.com/item/32839578059.html?trace=wwwdetail2mobilesitedetail&productId=32839578059&productSubject=10S-36V-Lithium-Battery-Protection-Board-BMS-with-balance-Waterproof-18650-lipo-Li-ion-16A-25A&spm=a2g0s.9042311.0.0.69d35c0f3TnTBZ

I have chosen the one with 60A with separate port so I'm hoping that it will come with three ports. B- P- C- ports.

Also I was thinking now im not going to have the on/off switch and just have an antibiotic spark loop key because it's so much cheaper.

Could you help a bit with the wiring if possible.

Thanks so much again.
```

---
## \#625 Posted by: Namasaki Posted at: 2018-08-07T12:01:50.373Z Reads: 153

```
A loop key is also more dependable. 

Post a pic of your battery’s balance connector so I can see the wires attached to it. 

I’ll make a diagram for you today after work
```

---
## \#626 Posted by: Gandinator Posted at: 2018-08-07T14:28:32.026Z Reads: 162

```
Thanks so much man. I really would be screwed with your help.

Pic ![Screenshot_20180807-151915__01|678x500](upload://7Dn1QEqRLXWHlwPSB0nz7KOqAkH.jpg)
```

---
## \#627 Posted by: Namasaki Posted at: 2018-08-08T00:49:57.629Z Reads: 158

```
Note:
You can leave the balance ground wire on Battery 2 disconnected. It is not necessary to connect it anywhere.
Clip it short and make sure the end is insulated.
Another important point is to make sure you cut balance wires one at a time or else you will short the battery.
```

---
## \#628 Posted by: Namasaki Posted at: 2018-08-08T00:50:38.450Z Reads: 165

```
![00%20PM|690x433](upload://s8G3BekoRgMME747D2h7Sr0ZJMA.png)

@Gandinator 
**WARNING**
Be very careful with this type of setup at least until the characteristics of this bms are known.
For example, braking on a full battery especially down hill.
Or durning hard acceleration.
The bms could shut off leaving you with a sudden loss of power and no brakes.
```

---
## \#629 Posted by: Gandinator Posted at: 2018-08-08T09:52:29.462Z Reads: 159

```
Thanks so much.

I've seen on other videos that they connect Battery 1's balance cable positive first (at the bottom of your diagram in this case) and they cut the positive wire on Battery 2. 
However, I assume its different for every BMS right? I've seen my BMS's diagram and see how it relates to yours. 

If i do have a separate port for charging, I just connect the negative of the charge port to the C- right?

Lastly, If I were to have a monitor for the battery percentage where would I connect that.

Cheers man,
```

---
## \#630 Posted by: Namasaki Posted at: 2018-08-08T11:56:54.738Z Reads: 165

```
I named the batteries 1 and 2 in relation to the sequence of cells 1-10. 

It’s not really necessary to name them at all. 
What is important is that the pack supplying the main black cable is cells 1-5
And the pack supplying the main red cable is cells 6-10
It is critical that the balance wires are connected in this sequence because if they are not correct, the bms will smoke.

There doesn’t appear to be a C- pad. 
When there is no C- pad, the charge neg hos to P-

I will add a meter to the diagram when I get home from work. 
It should go like this
Meter red between loop key and Vesc 
Meter black between bms P- and Vesc 
Then the meter will only be on when the loop key is connected
```

---
## \#631 Posted by: adrienfeve Posted at: 2018-08-08T19:52:47.370Z Reads: 158

```
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/69?u=adrienfeve

Could you explain a bit more?
I don't really understand why this is the case. On a simple 2S cell, how is it possible to balance each cell individually when the current flowing through both has to be the same?

Is this diagram correct:
![20180808_204848|690x366](upload://iRNMSCSc5AEW1CsMvQsenNlK9Tx.jpg)

I am designing my first esk8 and want to go with 10s. I was going for 2 x 5S cells. Except space, is there any disadvantage in doing so compared to 5 x 2S ?

Thanks!
```

---
## \#632 Posted by: adrienfeve Posted at: 2018-08-08T20:18:25.441Z Reads: 158

```
OK I found the answer in that video which is great:
https://www.youtube.com/watch?time_continue=658&v=wIbHLacozFo

However, I still don't see why there can be an issue when you have 2 cells in parallel on the balance lead. They are in parallel so they have to be at the same voltage and will balance one another. Is this correct?
```

---
## \#633 Posted by: Namasaki Posted at: 2018-08-08T22:46:14.589Z Reads: 157

```
In a perfect world, cells in parallel will automatically balance each other. The bms will see how ever many cells you have in parallel as one cell.
If the cells in parallel are not matched in terms of true capacity and internal resistance, then they will probably  not charge and discharge evenly.

It is my opinion that a 1p battery is the best scenario for balancing.
This is one of the reasons that I prefer Lipos to Li-ions.
```

---
## \#634 Posted by: Namasaki Posted at: 2018-08-08T22:49:11.538Z Reads: 147

```
I have added a battery meter to the diagram.
```

---
## \#635 Posted by: adrienfeve Posted at: 2018-08-09T05:28:15.694Z Reads: 148

```
Yes OK this makes sense if capacity and internal resistance are not a perfect match in the parallel branch. Thanks!
```

---
## \#636 Posted by: Gandinator Posted at: 2018-08-09T12:43:02.138Z Reads: 150

```
Thanks so much man. You really helped me out a lot. Never thought people would take so much out of their time to help. Cheers. BIG UP NAMASAKI
```

---
## \#637 Posted by: Jellybean Posted at: 2018-08-10T21:54:10.521Z Reads: 155

```
If you prefer 1P, how do you go about getting more range? Just bigger/more expensive batteries or individually balance charge each battery every couple discharges? I would like to put 4x 5000mah 6S LiPos into a 2S2P configuration for 12S 10Ah. Is BMS still usable? Thanks for all the help
```

---
## \#638 Posted by: Namasaki Posted at: 2018-08-11T02:29:24.339Z Reads: 167

```
I'm ok with with medium range of 10-12 miles so a 10s 5ah battery works for me.
People who build for maximum range usually use Li-ion cells.

I believe it is better to use Li-ion cells for a multiple P battery because with Li-ion cells, all the the Parallel connections are made before the Series connections. This simplifies the balancing process because all cells in parallel automatically balance themselves and the bms will see each group as one cell.
And each P group will automatically and continuously balance itself even when the board is off.

With four 6s Lipos, the series connections are made before the parallel connections. 
This rather complicates things. 
You can parallel the low current balance wires.
But you can not parallel the high current connections between each and every cell.
There have been some who have done this but I'm not sure how well it worked out over time.

Gens Ace Tattu makes some high capacity Lipos that are very good but not cheap.
https://www.amazon.com/Tattu-10000mAh-22-2V-Battery-Multirotors/dp/B01G8FUWMG


Or if you want some ridiculous range and power and don't mind the heavy price:
https://www.amazon.com/Tattu-22000mAh-22-2V-Battery-Multicopter/dp/B017NJTHJU/ref=sr_1_4?s=toys-and-games&ie=UTF8&qid=1533954092&sr=1-4&keywords=Tattu+22000mAh+22.2V+25C+6S+LiPo+Battery+Pack

@PatRocks uses the 22ah Tattu's with amazing results.
```

---
## \#639 Posted by: Jellybean Posted at: 2018-08-17T01:50:21.838Z Reads: 161

```
Thanks for the help @Namasaki
```

---
## \#640 Posted by: Gandinator Posted at: 2018-08-30T14:41:50.134Z Reads: 157

```
I'm just wondering when does the BMS begin to balance the voltages in each cell. Does it automatically do it when connected to everything or only when in discharge and charge?
```

---
## \#641 Posted by: Namasaki Posted at: 2018-08-30T15:12:00.626Z Reads: 160

```
Can’t say for sure. Theoretically, it’s supposed to start balancing when the pack is fully charged. 
However from what I’ve seen, it appears to balance all the time, even when turned off. 
I have not done any tests to confirm this.
The balancing current on bms’s is minimal and varies depending on brand and model. 
Some balance at 126ma some only 60ma
These are the top brands. Bestech and Supower. 
 Cheaper brands could be even less.
```

---
## \#642 Posted by: Gandinator Posted at: 2018-08-30T17:18:00.311Z Reads: 160

```
So you can't really know if the cells are balanced or not unless you measure it right? 
I've heard some have like LED's which light when it's fully balanced after charging but if you dont have that how would you know when to take the plug out?
```

---
## \#643 Posted by: AxelF Posted at: 2018-08-30T20:13:33.115Z Reads: 160

```
Whats your opinion on the batteries? Thinking about going 12S (4x3S), ZIPPY Compact 5800mAh 3s 60c (70C burst) to be specific. Maybe a 10s setup with the batteries linked by @Namasaki is better because of the higher burst (120C)?

In theory (Im aware of the fact that manufactures overestimate C number ALOT) my suggested 12S setup would be able to deliver 348A cont. and 406A burst. Can't really compare this directly to the 10s setup as 12S wont need as much current draw for the same power delivery...
```

---
## \#644 Posted by: Namasaki Posted at: 2018-08-30T20:31:03.007Z Reads: 153

```
I think the true current rating will be no more than 1/3 of what the C rating suggests
```

---
## \#645 Posted by: Namasaki Posted at: 2018-08-30T20:34:00.779Z Reads: 158

```
If the batteries get too far out of balance, they won’t fully charge with a bms and brick charger
```

---
## \#646 Posted by: AxelF Posted at: 2018-08-30T20:40:48.840Z Reads: 158

```
With that assumption Id still get 116A cont. Should be fine with a single 6374 motor (80A marked max)... Hmmm... decisions...
```

---
## \#648 Posted by: Blitz Posted at: 2018-10-03T20:30:49.526Z Reads: 156

```
[quote="Namasaki, post:24, topic:10014"]
The blue blocks are quick disconnects which makes for easier setup and maintenance.
[/quote]

Great idea! I think I'll copy you on that and get these.
I definitely want to keep a close eye on how my batteries are doing.

https://hobbyking.com/en_us/jst-xh-3s-wire-extension-20cm-10pcs-bag.html
```

---
## \#649 Posted by: dg798 Posted at: 2018-12-04T14:10:17.626Z Reads: 144

```
I’m building kinda of the same concept pack as this just with 4 3s I series for 12s. Instead of hardwiring it for series connection can I just use bullet connectors to connect them in series?
```

---
## \#650 Posted by: Namasaki Posted at: 2018-12-04T20:11:22.999Z Reads: 136

```
You can use connectors. 
Hard wiring just makes a cleaner setup and a more sure connection for maximum dependability and minimum resistance. 
Note: that it is still possible to check and even charge packs individually while they are connected in series. 
I have done this with mine. I disconnect the bms when testing and charging individual packs using a hobby balance charger with charge cables that have alligator clamps.
```

---
## \#651 Posted by: dg798 Posted at: 2018-12-04T21:08:59.821Z Reads: 130

```
Will using connectors decrease speed or acceleration to the resistance or is it very minute that it’s nothinn I should worry about?
```

---
## \#652 Posted by: slybarman Posted at: 2018-12-04T21:15:27.378Z Reads: 134

```
Provided the connectors are appropriately sized and soldered correctly, You won't notice any difference.
```

---
## \#653 Posted by: dg798 Posted at: 2018-12-04T21:15:51.078Z Reads: 136

```
5.5mm connectors for 10awg wire
```

---
## \#654 Posted by: slybarman Posted at: 2018-12-04T21:22:58.967Z Reads: 140

```
rated for 150 amps.  With bullet connectors we used to use male on one battery wire and female on the other to prevent accidentally plugging them in wrong and heat shrink on the females to prevent accidental shorting.  That was 10-15 years ago - not sure if that is still best practice.
```

---
## \#655 Posted by: dg798 Posted at: 2018-12-04T21:38:40.734Z Reads: 144

```
Ok thx for the info
```

---
## \#656 Posted by: Namasaki Posted at: 2018-12-05T03:21:30.033Z Reads: 148

```
5.5 bullets are my favorite and what I use on any connections that are not hard wired.
For shrink tube, I recommend using the overlapping mod detailed here:
https://www.electric-skateboard.builders/t/bullet-connector-shrink-tape-mod-how-to/9416
```

---
## \#657 Posted by: JBev Posted at: 2018-12-06T21:16:34.997Z Reads: 144

```
I plan on making a similar setting using either 5 or 6 of these in series with a bestech bms.
https://hobbyking.com/en_us/zippy-compact-5000mah-2s-60c-lipo-pack.html 
I plan on running one of torque boards' 6380 motors and an Ollin vesc. It is my first time building an esk8, and I think I might need the power from a 12s setup because I live in a very hilly area, but I'm not sure if one motor would be able to handle it. Should I go with the 10s or the 12s?
```

---
## \#658 Posted by: JBev Posted at: 2018-12-06T21:19:31.569Z Reads: 139

```
Also, will running 12s improve the range?
```

---
## \#659 Posted by: Itsmedant Posted at: 2018-12-06T21:30:40.789Z Reads: 138

```
The difference between 12s and 10s is mainly going to be a voltage difference. Voltage is more like "horse power"

The second numbers (3p, 4p, 5p, etc.) is your capacity. Think more of "gas tank".

I know this isn't the exact definitions for both of these, but thats the easiest way to get what changing around your batteries will do.
```

---
## \#660 Posted by: Itsmedant Posted at: 2018-12-06T21:50:53.101Z Reads: 138

```
So if you went from 10s4p to a 12s4p, you may see a bit of range increase, but if you went from a 10s4p to a 10s5p you would actually see a much larger increase.

The main reason you'd see an increase in range going from 10s to 12s is that you have more voltage "headroom" to play with. The sag that you will inevitably see won't hit you as fast as a 10s battery would.
```

---
## \#661 Posted by: Customesk8 Posted at: 2018-12-08T06:38:29.639Z Reads: 137

```
@Namasaki hey man looks awesome, pretty much exactly where i'm heading but i'm worried it wont fit under my short board length wise do you have the total measurements of this set-up?
```

---
## \#662 Posted by: Namasaki Posted at: 2018-12-09T02:20:32.879Z Reads: 137

```
The total enclosure length including the flanges is 23"
```

---
## \#663 Posted by: Customesk8 Posted at: 2018-12-09T02:23:39.433Z Reads: 141

```
![image|498x171](upload://vsD35zwNk33nOCINrNqpZqozX2h.png) 

Only got 420mm :(

Still need to do some research to determine if 8s or 6s will do the job for me so i can fit it all in
```

---
## \#664 Posted by: Namasaki Posted at: 2018-12-09T02:29:11.283Z Reads: 141

```
[quote="JBev, post:658, topic:10014, full:true"]
Also, will running 12s improve the range?
[/quote]


Running 12s will increase power and can also increase range because range is determined by voltage and capacity.
For example:
6s/10ah will theoretically  have about the same range as 12s/5ah.

Although as @Itsmedant mentioned, going from 10s to 12s is not likely to make a big difference in range but will supply more power for hill climbing.
Keep in mind however that higher voltage can be harder on electronics. Make sure you run heat sinks on your vescs.
And really if your planning on building a hill climber, better plan on a dual drive. A couple of 6374s will supply plenty of torque.
```

---
## \#665 Posted by: Namasaki Posted at: 2018-12-09T02:32:40.198Z Reads: 135

```
[quote="Customesk8, post:663, topic:10014"]
Only got 420mm :frowning:

Still need to do some research to determine if 8s or 6s will do the job for me so i can fit it all in
[/quote]


Keep in mind that I have a rather large bms and I allowed a lot of room for the bms and Vescs.

The Actual battery pack is only about 9-10" long
```

---
## \#666 Posted by: Customesk8 Posted at: 2018-12-09T02:34:22.948Z Reads: 132

```
Yeah true I'm studying that photo to see how much space i can recover, maybe minus 1 battery it'd be doable but then i don't know enough yet as to whether 8s will power dual motors well enough
```

---
## \#667 Posted by: Namasaki Posted at: 2018-12-09T02:35:35.091Z Reads: 134

```
Have you considered a longer deck?
```

---
## \#669 Posted by: Customesk8 Posted at: 2018-12-09T06:39:02.613Z Reads: 138

```
Yeah I have a longer one but want to use this short deck. 

Think I've figured out how I can do it - basically doing exactly the same as you but to cut down on size and fit it under the board going with 6s either that or ditch the BMS (yet to decide actually) but leaning towards going with 6s

Your work looks great man thanks for sharing
```

---
## \#670 Posted by: Customesk8 Posted at: 2018-12-16T11:54:58.279Z Reads: 131

```
what to do if they are not close enough and you don't have a balance charger?
```

---
## \#671 Posted by: Namasaki Posted at: 2018-12-16T22:18:13.302Z Reads: 133

```
if your talking about the voltages, how far off are they?
```

---
## \#672 Posted by: Customesk8 Posted at: 2018-12-16T22:18:54.732Z Reads: 135

```
sorry more hypothetical i dont have the batteries yet but incase they come out of balance

i gather hooking them up to the bms will sort it?
```

---
## \#673 Posted by: Namasaki Posted at: 2018-12-16T22:23:29.678Z Reads: 131

```
They should come with all cells at 3.7-3.8v
Check every cell before putting them together.
If any pack has a very low voltage, it is suspect as defective

update:
I just wanted to add that it is possible to get a bad pack right out off the box when buying Lipos.
I have experienced this first hand so I strongly recommend to anyone using Lipos to check new packs before doing anything with them.
```

---
## \#674 Posted by: Customesk8 Posted at: 2018-12-16T22:37:41.149Z Reads: 131

```
i've ordered the exact same batteries as you. 

so as long as they're around 3.7-3.8 i can connect them all together and to the BMS (i'm just getting an ebay charge only BMS) and from thereon it should be fine?
```

---
## \#675 Posted by: Namasaki Posted at: 2018-12-17T01:31:11.810Z Reads: 127

```
Theoredically but I can't vouch for cheap bms's sold on eBay.
That is, I can't promise you that it will be fine.
```

---
## \#676 Posted by: venom121212 Posted at: 2018-12-28T23:42:11.500Z Reads: 123

```
Wow so much knowledge in this thread. Thank you. Are there any pros / cons between 5 X 2s packs vs 1 x 10s lipo pack of equivalent ratings? The only one that comes to mind is number of connections but I figured you might know best.
```

---
## \#677 Posted by: Namasaki Posted at: 2018-12-29T04:51:50.793Z Reads: 120

```
five 2s vs one 10s

Size constraint is the main factor however there is also the matter of maintaining the overall battery.
So if you have five 2s packs and one cell goes bad, you have to replace two cells.
If you have two 5s packs and one cell goes bad, you have to replace five cells.
If you have one 10s pack and one cell goes bad, you have to replace ten cells.
Because when one cell goes bad in a Lipo pack, the whole pack is done.
```

---
## \#678 Posted by: JBev Posted at: 2019-01-02T15:46:24.140Z Reads: 118

```
I finally finished my board. I used one motor and 5 2s 60c lipos in series for the battery. I found that I lost traction when climbing hills. I use 100mm crossover wheels. Does anyone have a suggestion for how to improve traction without a second motor? Would 6.5 inch pneumatic wheels work?
```

---
## \#679 Posted by: JBev Posted at: 2019-01-02T20:40:12.623Z Reads: 115

```
i just switched the motor to the front wheel and the traction improved so much! It still isn't perfect though. It still slips when braking down big hills.
```

---
## \#680 Posted by: Customesk8 Posted at: 2019-01-02T22:44:16.827Z Reads: 113

```
How big are the hills?
```

---
## \#681 Posted by: Sn4pz Posted at: 2019-01-02T22:47:03.422Z Reads: 115

```
I would think it's your wheels, maybe a nice uniform surface would grip better

Or pneumies bc pneumies
```

---
## \#682 Posted by: J0ker3366 Posted at: 2019-01-02T22:50:41.292Z Reads: 125

```
Try putting more of your weight I've the motor when braking or accelerating. Then again, it could just be the surface you're riding on. I have the mbs all terrains and I don't get that problem unless its wet. Pictures of your build?
```

---
## \#683 Posted by: JBev Posted at: 2019-01-03T00:26:12.069Z Reads: 124

```
![IMG_20190102_191128|690x388](upload://b6MirVCkUezZuZYAneOWxnAp1EE.jpeg) 
My roads are pretty rough. They paved them cheaply (by putting down gravel and pouring tar over it) so there are a lot of loose pebbles. As you can see in the picture, the drive wheel has worn down a lot from only 3 hours of riding. I was able to climb a 35% grade hill today, but wasn't able to get down without skidding. Yesterday I wasn't able to get up the same hill. I think the bigger contact patch from the worn down wheel and front wheel drive helped. Also, this is my first board, so it took some time to get used to riding  it. The more I rode the board, the less it skidded.
```

---
## \#684 Posted by: Namasaki Posted at: 2019-01-03T06:28:25.243Z Reads: 118

```
I'm betting that some soft abec 11's would give you a lot more traction than those wheels.
Then again, if your roads have a lot of loose gravel, I don't know if anything will help.
```

---
## \#685 Posted by: b264 Posted at: 2019-01-04T00:06:53.523Z Reads: 116

```
[quote="JBev, post:683, topic:10014"]
putting down gravel and pouring tar over it
[/quote]

Ugh, that's the worst.
```

---
## \#686 Posted by: JBev Posted at: 2019-01-04T20:55:31.005Z Reads: 117

```
Ok, now I'm choosing between using trampa superstars or abec 11s. The setup with superstars would cost around 150 dollars more, but I think it's worth it because my roads are really bad.
```

---
## \#687 Posted by: bigben Posted at: 2019-01-04T20:58:24.870Z Reads: 117

```
[quote="b264, post:685, topic:10014"]
> putting down gravel and pouring tar over it
[/quote]


My street is apparently being resurfaced next week... I bet this is what happens.
```

---
## \#688 Posted by: JBev Posted at: 2019-01-11T01:50:08.598Z Reads: 120

```
I got my bms today! I am using a charge only bms.![IMG_20190110_204655|690x388](upload://byPriP6cvaOWkWqDVppFew3NSbL.jpeg) 
Will it spark when I plug in the charger? Do I need something like an anti spark loop key that I can plug in to start charging after the charger is already in?
```

---
## \#689 Posted by: Namasaki Posted at: 2019-01-11T04:52:15.792Z Reads: 118

```
Try connecting the charger to the bms before plugging it into the wall socket.
```

---
## \#690 Posted by: JBev Posted at: 2019-01-11T15:42:12.437Z Reads: 119

```
Ok, will try that after I finish soldering the connections today.
```

---
## \#691 Posted by: rsalmon Posted at: 2019-01-11T15:49:11.384Z Reads: 119

```
I have this same BMS in charge only setup. It does not spark when I plug the charger in.
```

---
## \#692 Posted by: JBev Posted at: 2019-01-17T02:29:47.563Z Reads: 116

```
@Namasaki
@bigben
@b264
@rsalmon
I just made a new topic for my build.
```

---
## \#693 Posted by: ryansinatra Posted at: 2019-01-26T23:32:58.814Z Reads: 106

```
Instead of hard wiring the packs, I could also just use xt60 series connectors, correct?
```

---
## \#694 Posted by: Indiangummy Posted at: 2019-01-26T23:40:28.351Z Reads: 114

```
Yes or bullet connectors. Either would work but hard wiring is best for power delivery.

Edit: @ryansinatra check out @lrdesigns build. He used bullet connectors.
```

---
## \#695 Posted by: ryansinatra Posted at: 2019-01-27T01:55:46.154Z Reads: 113

```
Good call! Thanks for the info.
```

---
## \#696 Posted by: Friskies Posted at: 2019-01-27T03:11:54.244Z Reads: 115

```
@Namasaki. I've been thinking about doing a compact travel build that I can go travelling. Yhis basically removes li-ion from my options - what I normally build with. What cell would you recommend for something as close to travel safe as possible that will still give 10/12s and wouldn't matter too much if I had to leave it an an airport.
```

---
## \#697 Posted by: Namasaki Posted at: 2019-01-28T00:22:30.088Z Reads: 114

```
Go with the highest C rating you can find because the capacity will need to be low for air travel.
But then, I always recommend the highest C rating possible regardless of capacity.
```

---
## \#698 Posted by: yonahsadeh Posted at: 2019-02-10T22:00:19.377Z Reads: 109

```
For my build, I am trying to figure out how to wire my two 5s batteries together and how to get them hooked up to a power button and 3 pin charge port. What plugs would I need, and would I need a power switch for the button?
```

---
## \#699 Posted by: Namasaki Posted at: 2019-02-10T22:07:46.269Z Reads: 106

```
Read through this entire thread and most if not all of your questions will be answered.
```

---
## \#700 Posted by: Bobby Posted at: 2019-02-10T22:13:38.153Z Reads: 105

```
Would you say graphene packs are closest to their listed c rating... im planning on making a bigger lipo battery and was hoping for 25+ miles with no sag... Im hoping 6 5s packs will be enough
```

---
## \#701 Posted by: Namasaki Posted at: 2019-02-10T22:28:42.865Z Reads: 106

```
Graphene's have a reputation for being good but I have never used them.
I doubt that there is a Lipo battery in existence that will deliver what it's C rating suggests.
I also doubt that you can eliminate voltage sag completely  with a battery that will have a reasonable size and weight for an Esk8.
The only thing you can do is try to reduce voltage sag as much as possible.
Lipos are good for short to medium range with maximum power and minimum sag in a relatively small package.
Li-ions are the usual choice for long range batteries.

5s packs are thick and using 6 of them for a 10s3p is gonna be a very bulky and heavy battery.
My very first build used 2 6s packs for 12s1p 5ah which got me about 10 miles.
I had an enclosure that I could open to swap batteries out quickly.
So I carried extra batteries in my back pack and had a total range of 30 miles.
I used a hobby charger to charge my packs outside the board.
That's just another option if you don't have the resources to build a Li-ion battery.
```

---
## \#702 Posted by: Bobby Posted at: 2019-02-10T23:06:51.356Z Reads: 102

```
Makes more sense. My lipo can be short commutes and the li ion for the long ones.... i know zero is unachievable but its a lot less with a high discharge lipo right? Which lasts longer in terms of cycles?
```

---
## \#703 Posted by: Indiangummy Posted at: 2019-02-10T23:14:28.913Z Reads: 100

```
Yes that's correct. The closer you're battery can get to providing the amps you demand the less voltage sag you will have.
```

---
## \#704 Posted by: PatRocks Posted at: 2019-02-10T23:37:53.565Z Reads: 104

```
The graphene Panthers (75c) and the older 65c generation are tested thoroughly on the rcgroups forum, and the verdict is they are **"TRUE"** 55 and 50c capable respectively. Meaning that not only can they do a full 55/50-C discharge, but they can do that repeatedly for their service life. Extremely impressive
```

---
## \#705 Posted by: Bobby Posted at: 2019-02-10T23:38:24.478Z Reads: 105

```
How long can i keep the lipos unused before i have to put them in “storage mode”. Does that only matter when you dont use them for an extended amount of time?
```

---
## \#706 Posted by: Bobby Posted at: 2019-02-10T23:38:57.344Z Reads: 105

```
So the graphene panthers are the newer ones?
```

---
## \#707 Posted by: Indiangummy Posted at: 2019-02-10T23:40:28.199Z Reads: 109

```
You can keep them for a few months or even longer  at 3.7-4.0 V. 
I left mine at the Voltage they came as, from the factory for two months with no problems. If your cells are at close to full charge I would discharge them to storage levels after two weeks of no use.
```

---
## \#708 Posted by: Namasaki Posted at: 2019-02-10T23:45:29.113Z Reads: 115

```
[quote="Bobby, post:705, topic:10014"]
How long can i keep the lipos unused before i have to put them in “storage mode”.
[/quote]


When you buy them, they will come at 3.7-3.8 per cell for shipping.
When you get them, you need to check the voltage of each cell individually.
It is possible to get a battery with one or more cells that are under minimum voltage.
It happened to me twice buying zippy lipos.
If you get a battery like that, the seller should replace the pack.
```

---
## \#709 Posted by: noi Posted at: 2019-04-15T16:10:27.207Z Reads: 101

```
There is plenty of usefull stuff here, thanks a lot @Namasaki. 
I´m on my first build and would like to get the wiring confirmed. 

![IMG_5643|666x500](upload://qTZ5sfiL61m6SW4qvqKaljsVjrH.jpeg) 

My batteries and balance wires are a bit different. I will put 5x 2S2P in series to get 10S. I´m confused with the balance wires, the batterie has one more connection in the middle, what is it?

![IMG_5642|666x500](upload://gi421m298ofuy7eIxNKDBguM28k.jpeg) 

Also my 10S BMS has 11 wires, one is black. I´m not 100% sure where it goes. Is it right to have it on the negative of the first batterie? All the other negatives are not connected, right?

![IMG_5644|375x500](upload://wsBZisCFSOLrZOqbjMd9mYfyKy9.jpeg) 

Would be very appreciated if someone can have a look and confirm, that it is right like that. Thanks a lot.

Three more questions:
1) Does I have to disconnect the loop key while charging?
2) The BMS doesn´t have a on/off switch, will it drain the batteries over time? Should I place the loop key somewhere else?
3) Does I need a inline fuse somewhere or is it enough to have overcurrent protection in the BMS
```

---
## \#710 Posted by: Namasaki Posted at: 2019-04-15T17:12:08.009Z Reads: 94

```
I’m at work now but will get back to you as soon as I can
```

---
## \#711 Posted by: noi Posted at: 2019-04-15T19:15:55.839Z Reads: 97

```
No worries, thank you very much anyway.
```

---
## \#712 Posted by: Namasaki Posted at: 2019-04-15T20:30:32.899Z Reads: 102

```
The orientation of your balance wires and main wires is correct.
Removing the loop key during charge cycle will stop the esc from powering on and is not a bad idea.
I'm not familiar with your BMS or the amount of drain it will impose on your battery.
You could put a 2nd loop key on the battery negative main and run a jumper from the B- pad to pin 0 of the balance socket if the the 2 are not already connected in the PCB.
Then you could disconnect the bms by removing the key.
```

---
## \#713 Posted by: noi Posted at: 2019-04-15T21:19:00.089Z Reads: 104

```
Awesome, thank you very much for your time.
What do you mean with "run a jumper from the B- pad to pin 0 of the balance socket"? Pin 0 is the black one on right? With jumper do you mean to connect them? What is it doing if I connect it? Maybe instead of the Loop Key I could just pull the main negative out of the battery if I wanna store it for a longer period of time.

Like this (added green wire)?:

![IMG_5643|666x500](upload://r2oIATCBIZORUrm9gYCSp9K6Bl2.jpeg) 

I have this BMS: https://de.aliexpress.com/item/10-S-13-S-36-V-48-V-40A-60A-Lithium-Batterie-Schutz-Bord-Elektrische-Fahrrad/32888307335.html?spm=a2g0s.9042311.0.0.6b934c4du4VM0E
```

---
## \#714 Posted by: Namasaki Posted at: 2019-04-16T00:39:42.990Z Reads: 102

```
Yes, Like that.
That way you can stop all current flow through the bms when you pull the key.
Now I can't say for sure that the jumper is necessary. It depends if there is continuity between the B- pad and pin 0 through the pcb.
It may be that pin 0 is an optional ground used when bypassing the bms for discharge so that you wouldn't have to use the B- pad at all.

You could (with all battery wires disconnected) test for continuity between the B- pad and pin 0 with a multimeter.
If the meter beeps then they are on the same ground and you can omit the jumper.
```

---
## \#715 Posted by: noi Posted at: 2019-04-16T07:01:16.418Z Reads: 102

```
Thank you very much. I will do all the wiring and see how it goes.
```

---
## \#716 Posted by: gucio0 Posted at: 2019-04-30T09:16:17.450Z Reads: 97

```
Hey. @Namasaki If I was to buy this HCX-D223V1 BMS in 13S variant. but use it only in 12S, would that be a problem?

That's why I'm asking:
https://www.alibaba.com/product-detail/battery-management-system-bms-for-e_60292861212.html?spm=a2700.7724838.2017115.23.3471310aR3w4WU

I wanted to use these in 12S 

https://hobbyking.com/en_us/turnigy-battery-nano-tech-5000mah-2s-65-130c-lipo-pack-xt-90.html
```

---
## \#717 Posted by: Namasaki Posted at: 2019-04-30T11:57:29.253Z Reads: 94

```
[quote="gucio0, post:716, topic:10014"]
If I was to buy this HCX-D223V1 BMS in 13S variant. but use it only in 12S, would that be a problem?
[/quote]

Yes, it would be a problem. These bms’s are specific so you have to get a 12s bms for 12s battery
```

---
## \#718 Posted by: gucio0 Posted at: 2019-04-30T14:26:16.637Z Reads: 96

```
Thanks a lot for a clarification @Namasaki,  now I'm tempted to go all out with 16s but it sound ridiculus...
Not sure if I'd ever need that and How I'd charge it. Plus I have to buy two and have no clue about what to do with another BMS, electrify a bike?
```

---
## \#719 Posted by: gucio0 Posted at: 2019-05-02T08:21:16.778Z Reads: 94

```
I have one more question, do you know of any other way or source of purchasing that particular type of BMS in 12S config? Or is Alibaba my best shot and I should just stay patient and wait?
```

---
## \#720 Posted by: Namasaki Posted at: 2019-05-02T11:59:40.451Z Reads: 89

```
You can order directly from Bestech or create 
a thread in the items wanted category to see if there is one available from a forum member
```

---
## \#721 Posted by: gucio0 Posted at: 2019-05-07T05:44:53.060Z Reads: 85

```
Thanks a lot.
```

---
## \#722 Posted by: direct_drive Posted at: 2019-05-07T08:47:56.834Z Reads: 84

```
Just a heads up, bestech arent answering emails... i must have tried 5 or 6 times over the past couple of weeks, from different email acounts, and to their info@ and sales@ accounts = nothing :roll_eyes:

If anybody has any ideas on how to get them that would be great
```

---
## \#723 Posted by: Indiangummy Posted at: 2019-05-07T22:36:22.475Z Reads: 79

```
Try http://litechpower.com/BMS/ it's a little longer ship time but there is no minimum qty required. 

Bestech and litech are the same company.
```

---
## \#724 Posted by: direct_drive Posted at: 2019-05-08T06:41:24.774Z Reads: 82

```
[quote="Indiangummy, post:723, topic:10014"]
Try [http://litechpower.com/BMS/ ](http://litechpower.com/BMS/) it’s a little longer ship time but there is no minimum qty required.

Bestech and litech are the same company.
[/quote]

Thanks man!
```

---
## \#725 Posted by: gucio0 Posted at: 2019-05-15T12:43:55.054Z Reads: 75

```
Hi, I've got one more question. Is this BMS: 
http://litechpower.com/product-detail/HCX-D596LF12S.html

going to work fine with a pair of these:
https://www.rcdetails.info/en/details/11204

also is it possible to receive guidance on how to connect it to vesc6 and BMS
```

---
## \#726 Posted by: Namasaki Posted at: 2019-05-15T17:29:36.692Z Reads: 77

```
There is plenty of information and guidance in this thread. 
Please read through this entire thread and if there’s something you don’t understand, we are here to answer your questions.
```

---
## \#727 Posted by: ivanflo Posted at: 2019-05-25T22:50:12.735Z Reads: 65

```
The simplicity and bang for buck of this setup is really amazing. I was able to use this setup with the 8000 Flight max to make a highly flexible build with range well beyond what I would generically use in one session.

Gearing up towards my second build and I still come back to this setup as the only one easily made flexible and essentially as thin as a 18650 battery pack. Thinking about LiPo's at 2200 for an ultralight commuter.
```

---
## \#729 Posted by: mattyB Posted at: 2019-09-04T12:45:37.798Z Reads: 49

```
can someone explain to me what will happen when i connect 5 X 2s 3700mah Lipos in series. I know that it will create a 10s battery but what i don't understand is what will happen to the current. Will i end up with a 18.5Ah battery so therefore pretty good range, like what will happen?
```

---
## \#730 Posted by: Namasaki Posted at: 2019-09-04T23:10:37.760Z Reads: 45

```
Series increases voltage

Parallel increases current/capacity

In series you’ll have a 10s 3.7ah battery

With Lipos  the C rating is very important 

A 10s 5ah battery can deliver decent range and power if the C rating is high enough. 
I run 10s 5ah 60/120 C and it delivers good power and 10-14 miles depending on many factors.
```

---
## \#731 Posted by: mattyB Posted at: 2019-09-05T10:01:41.993Z Reads: 45

```
The batteries are 70c 3700mah
```

---
## \#732 Posted by: Namasaki Posted at: 2019-09-08T20:50:40.356Z Reads: 40

```
70c is good
```

---
