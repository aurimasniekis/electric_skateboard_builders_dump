# About the Esk8 Electronics category

### Replies: 87 Views: 6160

## \#1 Posted by: onloop Posted at: 2015-07-11T07:00:10.393Z Reads: 890

```
This is where you may discuss any part of the electric skateboard that requires power to function.
```

---
## \#2 Posted by: Braylon31 Posted at: 2015-12-01T13:47:11.234Z Reads: 828

```
Why do I still need a 2s battery to run my reciever is this normal?  Im worried cuase im switching to a wii controller  will i have a problem  pulling wiiceiver power through the vesc?
```

---
## \#3 Posted by: lox897 Posted at: 2016-01-13T20:26:34.878Z Reads: 758

```
@Braylon31 This thread is about the category. Please start your own thread by clicking the new topic button.
```

---
## \#4 Posted by: Jonsme Posted at: 2016-10-10T15:58:30.928Z Reads: 586

```
Hey guys, I have an (Magneto) [Electric Skateboard ](https://magnetoelectricskateboard.com/) and am thinking about installing a VESC. Any recommendations? 

The board is awesome anyway! But getting really into this DIY electric board scene.
```

---
## \#5 Posted by: Randomoddy Posted at: 2016-10-15T05:19:09.392Z Reads: 479

```
Has anyone tried running a Quantum Mt series motor for their E-Board? http://www.hobbyking.com/mobile/viewproduct.asp?idproduct=67027

I'm interested in a dual drive system, and these would leave plenty of space, as they are quite skinny. They only allow for a 6s system, but I could get 4 of them for the price of the Rotorstar motor Im looking at. http://www.hobbyking.com/mobile/viewproduct.asp?idproduct=55435
I know it's a high kV, but I plan on gearing down ~ 6:1 ratio so I dont bog the speedy motor so much. The advantage of the Rotorstar motors is the fact I can run a 12s system. 

Basically, I want to know what would work best for me.

Wishlist-
Dual rear drive
High battery cell count system-6s minimum ideally
High ride time- around 10 miles ideally
Good power- enought to get me up a 30-35% grade
Good braking- for that same 35% grade.

I know I'm asking a lot of the system, but its what I want out of it. It's pretty extreme and, I know, gonna be pricey. I need some input for this since its my first E-Board.
```

---
## \#6 Posted by: darkkevind Posted at: 2016-11-02T14:45:45.838Z Reads: 331

```
Sorry to hijack this thread, but I need to post for some help with my motor but can't see how to create a new thread?
```

---
## \#7 Posted by: lox897 Posted at: 2016-11-03T21:18:33.317Z Reads: 304

```
You need to read for at least 30 minutes and post a few replies.
```

---
## \#8 Posted by: darkkevind Posted at: 2016-11-03T21:20:10.594Z Reads: 308

```
Thank you, I can do it now :slight_smile:
```

---
## \#9 Posted by: Vefond Posted at: 2016-11-11T07:56:04.269Z Reads: 304

```
hey guys, I have a wonderful electric skateboard with hub motor drive, it can be assembled, and the battery can be replaced.<img src="/uploads/db1493/original/3X/9/1/91d254d19e2b038763df6c06df832fca2b7d1504.jpg" width="690" height="477">
```

---
## \#10 Posted by: yumi Posted at: 2016-11-24T03:02:27.191Z Reads: 269

```
I don't know how to post a new topic.:sweat:
```

---
## \#11 Posted by: yumi Posted at: 2016-11-24T08:06:13.470Z Reads: 268

```
I am designing a cheap electric skateboard.

I have played around with various parameters for quite a while until I finally converged towards a specific motor and a specific battery. Lithium batteries are too expensive so I'm going for an AGM motorcycle battery. The problem is that the 0.025Ohm resistance of the motor leads to a huge current (hundreds of amps) up to 10km/hr which is most of my operational range. Other motors do not provide me with sufficient torque, therefore I need to include a current limiter to protect the ESC and maximise the battery capacity. For information, the continuous rating of the ESC I'm using is 60A.

I'm planning on measuring the current with a Hall Effect[ current sensor](http://www.kynix.com/uploadfiles/pdf0125/CSLA1CD.pdf) such as the Allegro modules out there, and an Arduino. Then map the current to a % of the duty cycle to subtract to the setpoint, before sending it to the ESC. For example, up to 30A => 0 feedback, 60A and above => 100% feedback, varying linearly in between. My gut feeling says it's basically a bang-bang controller which should be converging.
```

---
## \#12 Posted by: guillaume772 Posted at: 2016-12-06T14:57:10.940Z Reads: 240

```
Hi, I'm also new to building an electric 
skateboard, and I bought everything for it... except I forgot a charger 
for my battery. I have a 4000mah 5s 20-50c lipo pack, does anyone know 
what charger I should buy?

This is the link to my battery in case I'm not clear enough: https://hobbyking.com/en_us/turnigy-nano-tech-4000mah-5s-25-50c-lipo-pack.html 

Thanks,
Guillaume
```

---
## \#13 Posted by: guillaume772 Posted at: 2016-12-13T21:27:52.222Z Reads: 208

```
Me neither😂
```

---
## \#14 Posted by: guillaume772 Posted at: 2016-12-13T21:28:27.591Z Reads: 203

```
Looks like nobody knows
```

---
## \#15 Posted by: lox897 Posted at: 2016-12-13T21:44:20.184Z Reads: 200

```
Read for at least 30 minutes and comment on some threads. This is not the right place to ask questions about electronics.
```

---
## \#16 Posted by: Fizzy Posted at: 2017-01-14T15:48:33.210Z Reads: 196

```
 My board won't go from a standing position it just shakes a slight roll apply power and your ok any idea what vesc setting needs changing
```

---
## \#17 Posted by: Lucas123 Posted at: 2017-01-14T16:56:58.669Z Reads: 194

```
 hi I've recently received my parts to realize that my space cell pro 3 had an xt60 connector and I was wondering which one is better, xt90 or xt60?
```

---
## \#18 Posted by: BoardfortheLord Posted at: 2017-01-15T00:26:42.206Z Reads: 193

```
xt90 generally because it allows more electricity to flow through it, and its a bit safer

hope this helps
```

---
## \#19 Posted by: BoardfortheLord Posted at: 2017-01-15T00:29:59.981Z Reads: 190

```
I had this same issue, what fixed it for me is by going to the "advanced" tab in the motor config of the bldc tool. There should be a section labeled, "Current control" under that there should be startup boost. Make sure you are in bldc mode and make the number higher. I think the default is 0.010, try making it 0.050 or 0.060. This should get rid of the shaking and give you a gentle start.

Let me know if this helps!
```

---
## \#20 Posted by: Lucas123 Posted at: 2017-01-21T21:16:34.163Z Reads: 175

```
can i use a space cell pro 3 as a power supply to program a vesc
```

---
## \#21 Posted by: kristian Posted at: 2017-01-22T09:34:48.885Z Reads: 149

```
Hi I have a problem with motor. When I am accelering motor doesn't spin
```

---
## \#22 Posted by: Fizzy Posted at: 2017-01-22T18:23:28.344Z Reads: 145

```
That didn't work it's a mountain board so pushing off is tricky (bindings)
```

---
## \#23 Posted by: Joe2020 Posted at: 2017-01-30T22:34:43.577Z Reads: 142

```
How do you create a new thread ?
```

---
## \#24 Posted by: Joe2020 Posted at: 2017-01-30T22:37:07.649Z Reads: 146

```
Hxt90 allows more electricity to flow through, anti spark ones are safest
```

---
## \#25 Posted by: lox897 Posted at: 2017-01-30T22:44:37.470Z Reads: 142

```
You must read for 30 minutes and then click the new topic button
```

---
## \#26 Posted by: Hylke59beare1913 Posted at: 2017-02-03T12:02:55.309Z Reads: 140

```
Ho can help me a have 3 questions

i have the new vesc-x from Enertion but where can i bay the connector cable to the receiver?
And where can i bay the connector plugs there are not on the new vesc.?

On my motor are free cables does it matter how i connect them to the vesc.?
```

---
## \#27 Posted by: moe_lester Posted at: 2017-02-08T21:48:53.128Z Reads: 135

```
FREE VESC SOFTWARE

Does anyone know where to I can get VESC BLDC tool so i can setup my VESCs for my dual motor setup. I bought my VESC from Alien power systems. I been reading for hours and I'm new this all this (VESC/firmware) and I can't seem to find where to download the BLDC tool and is this the only software I need to program the motors??
```

---
## \#28 Posted by: HeRowe Posted at: 2017-02-14T02:03:09.031Z Reads: 131

```
So you have to build up enough reputation to start a thread?
```

---
## \#29 Posted by: Jammeslu Posted at: 2017-02-15T20:50:58.871Z Reads: 133

```
im a beginner on my first build and want to make a easy charge function without needing to take out the batteries each time, running 3s 5200mah x2 on a sk3 249kv single drive setup with vesc. so how do i do and what do I need? a bms thing? what like a laptop charger tho I'm a student and need to carry charge with me. didn't know how to create a thread so just posts this here and would be very happy for answers
```

---
## \#30 Posted by: NICOMUTTER Posted at: 2017-04-10T09:56:28.118Z Reads: 123

```
Hello!
I am seeking some informations about aliens motors... :)
Does anyone know a bit ?
```

---
## \#31 Posted by: schlub Posted at: 2017-05-10T08:20:56.872Z Reads: 105

```
interesting
```

---
## \#32 Posted by: crisonix01 Posted at: 2017-06-02T11:55:20.432Z Reads: 106

```
 need some help here. im building a e-mountainboard but still dont know wich esc to buy im thinking about the Hobbywing Max6 because of the amps or a vesc would be better? For my understanding the vesc is limited to 50 amps and when it comes to a mountainboard you need a lot of torque.
And I also have read that the vesc gets hot. Please help. Im going to be using sk3 6374 149kv by the way.
```

---
## \#33 Posted by: Danny Posted at: 2017-06-02T16:13:48.720Z Reads: 107

```
So I made a template for an electric skateboard, but I'm not sure if it's totally correct. Can someone maybe check if it is correct? <img src="/uploads/db1493/original/3X/3/f/3fbff6bb35e3da62d50fc6df94a6700caef0d04f.png" width="638" height="499">
```

---
## \#34 Posted by: nopro Posted at: 2017-06-11T01:47:57.608Z Reads: 93

```
hi im new to this diy E sk8boarding stuff and need some help, im wanting to build pretty fast sk8tboard like 35-45 kph and i dont know which motor will prowide that cus they all just have some numbers like 190kv 2000kv which does not make sense to me. and does the battery i buy make any diferent to the speed i will get?

so basically which motor and battery do i get?
```

---
## \#35 Posted by: KDA2601 Posted at: 2017-06-20T04:05:42.284Z Reads: 90

```
Hi all, how this this go and is it good idea
Motor- Turnigy Aerodrive SK3 - 6364-213kv Brushless Outrunner Motor (63mm)
Esc- HobbyKing® ™ X-Car Beast Series ESC 1:8 Scale 150A
2x- ZIPPY Flightmax 5000mAh 4S1P 20C (running in series)
Remote- Flysky Gt3b orange

board- Globe cruiser 32" or Landyachtz maple ripper 37"

Will this work and should i spend the extra on the landyachtz or stick with the globe

Thanks
```

---
## \#36 Posted by: louiepi Posted at: 2017-06-20T16:52:16.941Z Reads: 90

```
Where is the new post button. I found it once and when I clicked it said you are not allowed to view the resource.
```

---
## \#37 Posted by: lox897 Posted at: 2017-06-20T20:30:54.552Z Reads: 91

```
You need to read topics for at least 30 minutes. When you go onto the forum home page it will be at the top right
```

---
## \#38 Posted by: TraviskateN00B Posted at: 2017-06-21T04:49:59.392Z Reads: 98

```
Hey everyone, I am new to the e-board realm so go easy :grin:... I have a few questions about what to buy and how to buy.

The current setup I am thinking about is as follows:
1. Dual 270KV 1500w brushless outrunner motors
2. Dual 150A ESC controllers
3. BMS with homemade (2x) 6s2p battery packs
4. Mini 2.4ghz Remote Trans/Receiver
5. Imax b6 charger
6. associated wiring for all components

If anyone can explain if any of this is wrong, please do.
This will be my first build but I want to use this to travel inner city to and from work. Will this do the job? 

Let me know thanks!
```

---
## \#39 Posted by: Damianilcapo Posted at: 2017-06-27T15:59:40.609Z Reads: 83

```
Hi there...where is the new topic button? thanks
```

---
## \#40 Posted by: rakejagland Posted at: 2017-07-16T02:43:48.866Z Reads: 91

```
VESC DETECTION HELP!

Hey! I am new to the DIY electric skateboard community and I'm in the middle of my first build. My set is:
-(2x) 5000mah  4s1p lipo batteries in series
-TORQUE VESC BLDC speed controller
-TORQUEBOARDS 6355 190KV motor

When I first plugged everything in and tested the motor to see if it would spin, everything powered up great and the motor spun, however, there was absolutely no torque. I could put my hand on the wheel and the motor would not spin, it would slip. So, I figured this could be fixed with VESC calibration/configuration. I had to very slightly downgrade my VESC firmware in order to match the latest BLDC tool I could find online. I followed all the videos and forums online on configuring the VESC, but now I can't get any connection. When I power up the board, I no longer get the initial three flashes of the red/pink light on the VESC. I can detect and connect it to my computer and write new configurations, and the radio transmitter even connects to the remote, but I am no longer getting any motor movement at all. Even after I restored to default configuration, I still don't see the three flashing lights and power up and no motor turning. 

Help would be MUCH appreciated! Thank you!
```

---
## \#41 Posted by: richard1983 Posted at: 2017-09-05T19:46:25.384Z Reads: 79

```
I'm attempting to build an Electric Skateboard, I bought a battery from here - https://www.icrfq.com/part/3884479-CSLA1CD.html for my Skateboard. Could you please suggest me this is the correct battery for my skateboard? The battery information is given below or you may check the datasheet of CSLA1CD (datasheet link given above):

* Output - Ratiometric, Voltage - 49.6mV/N
* Voltage - Supply - 8 V ~ 16 V
* Current - Supply - 19mA (Max)
* Sensor Type - Hall Effect, Open Loop
```

---
## \#42 Posted by: cobiispo Posted at: 2017-10-01T07:35:10.048Z Reads: 71

```
apparently you gotta post a few replies to create your own thread so heres my reply
```

---
## \#43 Posted by: maxbicyclemax Posted at: 2017-11-21T10:16:59.791Z Reads: 70

```
Hiya,
Absolute newbie to the forum.
Found it a bit difficult just to create an account on my iphone5.
Now I'm trying to post a question.... am I supposed to introduce myself somewhere or something?
```

---
## \#44 Posted by: maxbicyclemax Posted at: 2017-11-21T10:24:24.030Z Reads: 69

```
How did you go?
Just trying to get started myself.
```

---
## \#45 Posted by: noble Posted at: 2017-12-04T21:11:12.723Z Reads: 69

```
good morning. forgive for my English, I'm from Spain. I bought a skateboard and only cut it so that I could put it on the board I want. When I lengthen the cable, I have this problem.
somebody could help me? I have only extended the cable.

https://youtu.be/WKO3kuqBjgc

Thank you.
```

---
## \#46 Posted by: ElskerShadow Posted at: 2018-02-28T20:03:13.400Z Reads: 60

```
Problem solved ?
```

---
## \#47 Posted by: jcab Posted at: 2018-03-08T22:27:34.363Z Reads: 71

```
VESC not responding to Controller
Using the VESC tool, I updated my 4.12 Flier VESC from 2.54 Firmware to 3.34 Firmware. The update was successful (according to the VESC tool), but now the VESC will not respond to input from the controller. The VESC was communicating fine with the receiver until after the firmware update.  I have tried a few things to troubleshoot this, but no success. 
Transmitter/receiver – 
a.	Redid the binding process – still not communicating
b.	Tried all channels – Still not communicating
c.	Tried using another VESC to insure the Transmitter/Receiver was working correctly – Worked fine on 4.1 hardware/2.18 firmware
d.	All lights on Transmitter/receiver indicate that the connection between the two are active/correct (ie: steady light on both)
e.	Tried a different Transmitter/receiver – still no communication (but this trans/rec works fine on second VESC)
2.	VESC –
a.	 Reapplied Firmware update – still not communication with controller
b.	VESC tool communicates with VESC correctly – can change settings, they are saved and applied
c.	Rebooting VESC after each change – still no communication with Receiver
d.	When using the VESC tool, I can control the motor and it functions correctly (ie: The motor accelerates/brakes/etc. using the arrow keys on the keyboard).
The problem seems to be with the VESC recognizing the receiver. 
Any ideas on what I can do to solve this?
```

---
## \#48 Posted by: Liljpw161 Posted at: 2018-03-09T02:36:43.272Z Reads: 68

```
Need to add an extra battery to an existing board with battery already. I bought this board off amazon. I want the range to be more. How do I add a switch to switch between batteries when one dies?
```

---
## \#49 Posted by: RagingReptar Posted at: 2018-03-12T15:37:02.608Z Reads: 68

```
why cant i make a thread?
```

---
## \#50 Posted by: macncheese Posted at: 2018-03-31T20:13:34.924Z Reads: 77

```
I have the (3) of the batteries below wired in series, providing 36 volts. I want to replace with Lion batteries with **at least double range**. I am using have (2) of the motors below as well. 

I need some recommendations on battery setup. I can buy or build pack.
![20180325_164208|690x388](upload://9YLYhXLOolgvxLlnJnGFqnA3eeH.jpg)![20180331_155553|281x500](upload://A5EvtsfNkQgXwA3v3oN97V1Q8BI.jpg)![20180325_164147|281x500](upload://k7z7EEPJniGJ0AhGH4rjT0m85gL.jpg)
```

---
## \#51 Posted by: tristanrai Posted at: 2018-06-23T16:20:15.580Z Reads: 63

```
so am i, here to create my own replies, that is
```

---
## \#52 Posted by: Tricky1024 Posted at: 2018-09-09T09:29:14.027Z Reads: 47

```
hi all, I have been building my project for a while now and managed to kill 2 x VESC controllers. 1 of them I know I powered up with no motor and went full throttle. (don't know my I did it :smile:), I know this causes the DRV ERROR so I will be replacing the DRV chip next week. but the other is somewhat of an unknown so I am hoping someone can help.

I have:
12s 6Ah power pack
Flipsky Antispark
13s BMS (China)
Flipsky VESC 4.12 50A Cont.

I setup the VESC as normal, configured for the remote and setup the motor FOC sensored 60A for all except 20A regen.

Motor tested and setup with no issues, I could use the motor from the remote also with no issues, but then I went full throttle and BANG!! VESC has popcorned the DRV chip. and by popcorned I mean there is a hole in it.! When this blew it also took at the Anti-Spark board. (great :pensive:)

I know FOC is not recommended but my test rig before building this was FOC with this controller but no BMS, Anti-Spark and only 6s 6Ah battery pack.

I will also repair this VESC but I need to try and understand what and why it happened. please can I ask for views on this?
```

---
## \#53 Posted by: Regens Posted at: 2018-09-27T17:50:37.886Z Reads: 48

```
Hello, first of all you somebody doesnt have time then skip this post because im asking this for a friend who doesnt speak english but has a problem. recently his skateboard broke up and the decided to build a custom one 
using focbox 3.30 FW and engine sk3 6374 192kv and 6s acumulators li-pol but the problem is that the vesc tool FW is so overhelming to him that he doesnt really know where to begin, sites in our languages are very limited in information about that since electric skateboards are not very popular here.
It does work but the the skateboard is very sluggish. The top speed is ok but accelerating from standing position is very slow making it difficult to drive on the streets (red lights etc).

i would really appreciate if somebody patient could help us solve it as Vesc tool FM looks very confusing. 
I will post any additional info if needed ofc.

Thanks in advance
```

---
## \#54 Posted by: Dougz Posted at: 2018-10-04T08:59:53.755Z Reads: 46

```
Hobby king do a cheap charger that will charge up to 6s, that will do you unless you want to charge 10s 12s you need something like the graupner 18s.
```

---
## \#55 Posted by: evanlanz Posted at: 2018-10-09T22:50:20.539Z Reads: 47

```
commenting so I can make a thread
```

---
## \#56 Posted by: jojamcha Posted at: 2018-10-15T21:03:21.715Z Reads: 44

```
Hello everyone! I am completely new to skateboard building and have a few questions to ask. I recently unboxed my new VESC, motor, receiver and batteries and I am putting them all together now. I am using the VESC BLDC tool to configure the VESC, remote and motor. Unfortunately, when I try to configure the motor settings something interesting happens. When I try to run the motor detection test. nothing happens for a few seconds, then a message pops up in the message box that says "detection failed", and in the bottom right corner, outlined in red, "bad connection result received". Also, now my VESC in flashing pink in sets of two flashes, not three. I honestly have no idea what is going on! Please help! :grimacing:
```

---
## \#57 Posted by: Brasstackzach Posted at: 2018-10-20T13:28:02.240Z Reads: 42

```
hi I am very new to the esk8 world, but i recently built my first board, I am running a 12s 2p battery from torque boards with there 6374 190kv motor ....its a single setup,i have ridden it a few times it starts out super strong and kinda crazy fast but seems like at about 70% batt life i get a power drop off is that normal? seems strange to me but with nothing to compare it to not really sure will say for example  it goes from speeds of  25mph+ to toping out at maybe 20 or less at 70% battery then after parking the board for a bit (with turned off ) when i turn it back on the battery display says 90% with being plugged in..... not sure what thats about.
```

---
## \#58 Posted by: Brasstackzach Posted at: 2018-10-20T13:30:00.289Z Reads: 36

```
hi I am very new to the esk8 world, but i recently built my first board, I am running a 12s 2p battery from torque boards with there 6374 190kv motor …its a single setup,i have ridden it a few times it starts out super strong and kinda crazy fast but seems like at about 70% batt life i get a power drop off is that normal? seems strange to me but with nothing to compare it to not really sure will say for example it goes from speeds of 25mph+ to toping out at maybe 20 or less at 70% battery then after parking the board for a bit (with turned off ) when i turn it back on the battery display says 90% with out being plugged in… not sure what thats about.
```

---
## \#59 Posted by: zturmam Posted at: 2018-10-29T01:03:38.387Z Reads: 33

```
Hey anyone know what I can do to swap out DIYeboard.com’s esc for the 10s5pdual belt motor kit ? I ordered it about a month ago and have been replacing parts as they fail which has been rediculously quickly. But as I put almost 30 miles a day on it I kinda figured as much. Anyway any ideas on what esc would work and hold up to the miles I put on it?
```

---
## \#60 Posted by: Doodles Posted at: 2018-11-12T20:45:55.836Z Reads: 34

```
I can’t make one either. I think you need to read a certain amount but I’m not sure.
```

---
## \#61 Posted by: Jake50 Posted at: 2018-11-14T17:49:41.483Z Reads: 31

```
Can anyone help me find a supplier that sells Onan X2 batteries /chargers/remote controls?
```

---
## \#62 Posted by: BobTheBuilder Posted at: 2018-11-22T13:37:58.377Z Reads: 34

```
Hey I have a benchwheel eskate that works but the battery lasts for 20min and max speed 12mph. It really can't go any hills etc. 
Anyways I was wondering if you would know if its possible to add a second motor + change the battery. I'm quite new in these so any help is appreciated. Do I have to change the esc at the same time. Or if u have any ideas to make it more quick feel free to tell. This is my board.
https://www.benchwheel.com/collections/single-motor/products/300w-power-four-wheel-electric-skateboard
![skate|281x500](upload://kO09scSKxbWOe9t9ju9cbxeUOk1.jpeg)
```

---
## \#63 Posted by: fastasmix Posted at: 2018-11-25T00:40:58.196Z Reads: 34

```
Hey guys,
some context...
First time posting here. I just built an electric skateboard. I started off with a cheap motor controller off eBay for $40 that got the job done surprisingly well but had a 12mph speed limit for some reason and whenever I braked standing on the board the belt connecting my motor would skip. This proves the motor and battery work fine. Given these two I upgraded to a Flipsky VESC off of Amazon and downloaded the VESC Tool because the motor would only activate in short bursts. I started the motor setup wizard and it could not complete a motor detection cycle. It showed a Detection Failed and I saw on another forum that I should go into terminal and enter faults. I did that and it said Undervoltage. Anybody know how I could fix this? 
Here are the specs:

10s2p custom lithium-ion battery at 38v fully charged w/ BMS
270kv sensorless motor
Flipsky VESC

And some screenshots of the issue in VESC tool:

![Screenshot%20(11)|690x388](upload://wTV4aeHv8TYE6WfUpRPkvCpGz0X.png) 
![Screenshot%20(12)|690x388](upload://xIWLiNWHKytR3XZj8cguBrPreF1.png) 

There are pages of faults that all read like the first two brackets with slightly different numbers.

Finally, a picture of my board. It is on an Earthwings deck. Everything is stored inside a fiberglass shell I fabricated that is not on the board at the moment but sitting to the side. My battery, battery monitor, powerswitch, and charger are attached. 

![unnamed|375x500](upload://rvjh7WIaPo5JDftApWIiqdo8Jtr.jpeg) 

Anything would help! I tried multiple duty, erpm, and amp values for the detector with no success. 

Thanks!
```

---
## \#64 Posted by: Oli172 Posted at: 2018-12-15T09:03:06.444Z Reads: 26

```
Hi
Did you get any advice on battery packs as far as best for range and power?  I am struggling to find solid facts.  I am also looking at hobby king and want to use their outrunner motors.  So far I am thinking about finding a relatively high voltage and connecting 2 lots of 2 batteries in series and then joining them together in parallel to get better amps.
```

---
## \#65 Posted by: macncheese Posted at: 2018-12-15T13:38:31.210Z Reads: 24

```
Look at the bettery section in this forum. How long do you want it to last?
```

---
## \#66 Posted by: Felipesosadiaz Posted at: 2018-12-17T05:02:30.221Z Reads: 27

```
I dont know how to post a new one so here it goes!!
I recently bought a escooter in really bad shape and want to make a new one. The only.parts i took from the old ones were the wheels and the motor... now my problem! I bought a speed controller YK31C of 24 v. Connected it like everyone says on internet..and doesnt work!

I connected the battery, the on/off switch together, the throttle (positives, negqtices and signal respectevly) and even the brake light. 

I found out the brake light, the battery indicator light and swith on/ off are working but the motor wont move when i push the throttle. 

 I tested the motor directly to the battery and works. I tested with a multimeter controller the red and black output of the thorotlle and gives 5v. And tested the output of the throttle and gices a range from 0.4 to 6v when pushed. So whay am i doing wrong!! Why is the motor not moving. I bought another controller yk31c and still the same.problem. any thoughts? I attach pics.(you can see the clambs touching but when o tested they are actually not touching each other). The green wires are an extension of the controllers throttle![20181216_231741|281x500](upload://mwkQlGVNctKIu7bBTYxXbymaUbE.jpeg)
```

---
## \#67 Posted by: Felipesosadiaz Posted at: 2018-12-17T05:03:33.722Z Reads: 32

```
Another pic![20181216_231841|690x388](upload://8es8wxSaHX6oht5H579EF9zPUgs.jpeg)
```

---
## \#68 Posted by: Mountainboard83 Posted at: 2018-12-24T05:46:45.368Z Reads: 30

```
Hi First post not sure if this is the correct spot to enter it. Im building an MBS Core94 Moutainoard with Dual 6374 190kv motors on 12s with dual Vesc master/slave with cam bus. I ran thru the vesc tool motor and controller setup everything appears to work, motor hums then spools and all green, controller show full throttle, center and brake at 100% saved settings to vesc and copied to slave but after disconnecting nothing happens when i give it throttle. ran through setup 4 or 5 times re charged battery and checked all connections, must be a setting in vesc tool im missing? setting up in FOC if that matters.
```

---
## \#70 Posted by: yonahsadeh Posted at: 2019-02-10T14:39:41.349Z Reads: 28

```
Hello all, I am embarking on my first electric skateboard build and need some help making sure all of my components will work BEFORE buying them. I also want to know if something is not needed/I need to replace it with something else.

The following is a list of all of the components that I have put together. Do I need a BMS for the 2x 5s lipo batteries? How and where would I attach the charger to the batteries? (I want to use one of those three prong chargers because I don't want to have to remove the batteries to charge them) Do I need a switch in order to have a battery indicator and power button?

Thanks,
-Yonah

https://textuploader.com/1a89t
```

---
## \#71 Posted by: carinthia Posted at: 2019-02-11T07:25:30.727Z Reads: 29

```
Hi newbie here trying to put together my first electric skateboard build. After some basic research I've come up with the following electronic set up. 

ESC: http s://hobb yking.c om/en_us/aerostar-advance-120a-esc-opto.html
Battery: http s://hobb yking.c om/en_us/turnigy-high-capacity-battery-8000mah-4s-12c-drone-lipo-pack-xt90.html (two of these, planning to connect in series to make an 8s pack)
Motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html
(I put spaces in between the 'c' and 'o' in "com", the 'b' and 'y' in "hobby" and the 'p' and 's' in "https" due to new user link resrictions)

Ive also looked into a balance charger for the batteries as I know Lipo batteries can be dangerous when charged uncautiously

Balance charger:  https://hobbyking.com/en_us/ecube-e4-with-us-plug.html

Am I missing anything glaringly horrid with this setup or is this a reasonable start point? ANy advice as to what changes I should consider?

Thanks :)
```

---
## \#72 Posted by: Fede6686 Posted at: 2019-03-01T09:24:43.619Z Reads: 26

```
I'm new to esk8 building. I would build a 10s4p li-ion pack with the possibility of upgrading to 12s4p in future. Is it possible with one of this BMS?

https://it.aliexpress.com/item/Smart-7-S-per-20-S-Lifepo4-li-ion-Bordo-di-protezione-Della-Batteria-BMS-400A/32966608058.html?spm=a2g0s.13010208.99999999.271.76963c00irqn8t

https://it.aliexpress.com/item/12-S-44-4-V-Al-Litio-intelligente-li-ion-sistema-di-bordo-di-protezione-della/32966069150.html?spm=a2g0y.search0204.3.30.6c4c2572csOjr1&transAbTest=ae803_4&ws_ab_test=searchweb0_0%2Csearchweb201602_7_10065_10068_319_317_10696_10084_453_10083_454_10618_10304_10307_10820_10821_537_10302_536_10902_10843_10059_10884_10887_321_322_10103%2Csearchweb201603_60%2CppcSwitch_0&algo_pvid=78734044-cf66-44f2-b544-c21819ff38e9&algo_expid=78734044-cf66-44f2-b544-c21819ff38e9-4
```

---
## \#73 Posted by: sevolon Posted at: 2019-03-05T00:43:02.253Z Reads: 24

```
Same! I am new to this website and have some problems with my new e-board that I would like to discuss!
```

---
## \#74 Posted by: zed Posted at: 2019-04-09T18:46:33.531Z Reads: 26

```
Hello everyone,

I would like to buy 
turnigy sk3 6374 149kv.
But this one is without sensors or should I buy thisone? 
https://hobbyking.com/cz_cz/turnigy-sk8-6374-149kv-sensored-brushless-motor-14p.html

Will this one work well with míní direct helical and Vesc6 ? 

Thanks for help
```

---
## \#75 Posted by: Jake25 Posted at: 2019-04-28T12:09:54.678Z Reads: 22

```
Hey guys, 

I was wondering if you guys can help me with my dual motor evolve skateboard. What I'm asking for is how can I control the motors separately if it's possible.
```

---
## \#76 Posted by: BearBoi Posted at: 2019-05-08T07:42:42.416Z Reads: 24

```
I am in the exact same situation :P I'm new here. I also have a problem with my motor funny enough. I guess I'll wait patiently until esk8 lets me post :D
```

---
## \#77 Posted by: Gvido Posted at: 2019-06-17T23:12:39.690Z Reads: 20

```
Hello everybody!
```

---
## \#78 Posted by: Mazer Posted at: 2019-06-23T15:48:56.522Z Reads: 19

```
Does that work?
```

---
## \#79 Posted by: Sparkmatic Posted at: 2019-07-18T19:08:41.284Z Reads: 18

```
Hello, I have been lurking for some time now, But recently me Yuneec EGO has started have a problem with having smoke coming from the motor... I know it is from lubricant/oil getting into the motor but I now need to clean the winding. Does anyone know how to remove the stater from the motor? Pictures would be super helpful if you have any. Thanks
```

---
## \#80 Posted by: benha Posted at: 2019-07-19T20:20:09.619Z Reads: 18

```
Hello!  I'll be asking an electronics question soon, but for now I'm submitting a reply to this thread to see if that helps accelerate the pace with which I'm allowed to post a new thread ;-)
```

---
## \#81 Posted by: Jonisonvespa Posted at: 2019-07-26T09:55:39.250Z Reads: 17

```
Hello,
Can someone pleaze help, read all the fqas, i am struggling where to buy from, im from the uk and i but from ebay, and from china alli express ect, 
So far
```

---
## \#83 Posted by: Th0mas Posted at: 2019-08-09T08:33:32.752Z Reads: 14

```
Hi all, I wanna asking some question about battery. Generally, Three brands of the battery on the market which is used to build skateboard: LG, Samsung, and Sanyo. there are many model about  each brands. I wonder how I can distinguish about those model of Samsung.Such 30Q, 35E. What is it?
```

---
## \#84 Posted by: MikelNight Posted at: 2019-08-09T19:10:28.439Z Reads: 13

```
Hey Esk8 builders i have a question. 

After Finishing My new Setup wich is 10s3P, with bms, vedders antispark and vesc 4, i disconnected the on/off button from the antispark to cut Out the holes for the enclosure. After that i See the vesc turned on. Plugged Out everything to turn OFF the vesc. (I know now, that this wasn‘t good at all) 

But anyway, now the vesc will Not turn on again. Do i burnet my vesc with that move? Plugged in the vesc directly to the battery, Same thing, it wont Go on. No blinking, nothing.

Thanks for your help.
```

---
## \#85 Posted by: Lincon Posted at: 2019-08-28T06:57:15.300Z Reads: 9

```
Hello guys,,
I had this same issue, what fixed it for me is by going to the “advanced” tab in the motor config of the bldc tool. There should be a section labeled, “Current control” under that there should be startup boost. Make sure you are in bldc mode and make [dkt test](https://www.easydrivingtest.com.au/driver-knowledge-test) the number higher. I think the default is 0.010, try making it 0.050 or 0.060. This should get rid of the shaking and give you a gentle start.
```

---
## \#86 Posted by: malJohann Posted at: 2019-09-30T10:42:34.587Z Reads: 7

```
More esk8 electronics being developed at e&ZeroWidthSpace;sk&ZeroWidthSpace;8&period;n&ZeroWidthSpace;ews
```

---
## \#87 Posted by: ScootyP Posted at: 2019-10-19T23:51:36.552Z Reads: 5

```
Hey guys, recently I created my own Li-ION battery pack 10s4p to use on an electric scooter I am building. I also attached a balancing BMS with over/under charging protection and everything. I then got a 42V 2A charger for the pack and the charger itself was rated to come with battery protection circuitry. After testing it out tho, the charger seems to stop charging when the pack reaches only 37V, which is the nominal voltage of the pack since ~3.7V times 10 in series is 37V. But shouldnt the charger go all the way to around 42V since that is the true fully charged capacity of the pack. Has anyone dealth with something like this? Thanks
```

---
## \#88 Posted by: Arcadepcnut Posted at: 2019-10-28T17:25:02.150Z Reads: 5

```
ok so im not as old as i thought. i cant figure out either how to post a topic and figured i was just to darn old for these forums. i have an important question to ask... :(
```

---
## \#89 Posted by: chopper698 Posted at: 2019-11-17T04:01:56.979Z Reads: 4

```
Finishing up my first esk8 build and Im up to setting the parameters for the flipsky dual 6.6. I downloaded the vesc app to my android and got the bluetooth. Theres not much info on youtube, flipsky has a tutorial,  its so fast and the guy is speaking chinese so its useless. I got through some of it I dont even know if its the right info I put in. My remote is the VX2 from flipsky and its not showing mph when the wheels turn, amps and battery life of the board. It also feels like its has only 1 speed HIGH with no transition. I know I set the wheels, pulley, and cells of the battery.
```

---
