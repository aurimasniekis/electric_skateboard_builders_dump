# How to build dual motor electric longboard for cheap?

### Replies: 26 Views: 16100

## \#1 Posted by: xPouca Posted at: 2016-05-03T05:40:31.792Z Reads: 408

```
I'm 14 and need a transportation device. I was thinking of getting the Yuneec E-Go but it was kind of expensive and can hardly climb up hills + has low speed. The road from my house to school is 2 miles and has LOTS of steep hills! I need an Indra of what parts to get and these are what I prefer... Climbs up hills easily, good batteries, doesn't over heat as easily, good speeds, and small controller. If anybody can help me out, that'd be amazing. My budget is about $600.
```

---
## \#2 Posted by: MasterCho Posted at: 2016-05-03T05:51:47.970Z Reads: 407

```
https://www.youtube.com/watch?v=6yBgsT65UPg
```

---
## \#3 Posted by: xPouca Posted at: 2016-05-03T17:58:42.596Z Reads: 376

```
Can I use dual motors with that set up?
```

---
## \#4 Posted by: sl33py Posted at: 2016-05-03T18:48:50.116Z Reads: 370

```
cheap transportation = a skateboard (no motor).

For <$600 it's going to be tough to get a good setup.  POSSIBLY a single motor setup on a lower voltage (4-6s) battery and inexpensive ESC.

Motor mounts and gears - unless you have access to a cnc and can d/l the free enertion mounts and have them made, i would buy a full setup/kit that has everything including gears and belts - not just the mount.

GL!
```

---
## \#5 Posted by: longhairedboy Posted at: 2016-05-03T19:11:44.281Z Reads: 353

```
at 14 years old you could probably easily get away with a single, larger motor and therefore spend half as much on your drive train and electronics. And since you only need to go about 5 miles on a charge...

this battery would probably work for you: $60 on sale now
http://www.hobbyking.com/hobbyking/store/__16228__ZIPPY_Flightmax_8000mAh_6S1P_30C.html

this ESC is solid, i've used them a lot: $70
product/single-motor-120a-6s-esc/

All the less expensive but high quality motors (SK3, NTM, Tacon) seem to be backordered at the moment but if you wait a bit you might catch one on sale for around $50 or $60 and then either peice together your drive kit seperately or you can spend a bit more and grab this package that also has the rest of the drive kit, trucks and wheels for $400:
http://www.enertionboards.com/diy-electric-skateboard-kits/single-motor-mount-pro-kit-plus/

bring your own deck for $100 and what you have is a $630ish DIY board plus maybe another $30 or $40 for wires and connectors and maybe a sandwhich box to put it all in. 

Bring your own tools though.
```

---
## \#6 Posted by: xPouca Posted at: 2016-05-03T22:16:45.221Z Reads: 332

```
Ok, I see what you guys are saying now but the reason why I wanted dual motors is because there's a lot of hills in my area. And since watts mean more power (is it?), I'd want equal powers on equal sides. Like it's weird having it on one motor. I was planning on one motor but the one I saw had 1,000 watts and just thinking about it, 1,000 watts on one wheel is weird because that can make it go off balance. I found a set up that I think would be good for me and it's less than $500. The thing is, is it a good one?

Here's the set up 

x2 motors - $67.56
(Turnigy Aerodrive SK3 - 4240-740kv Brushless Outrunner Motor)

x2 batteries - $45.40
(Turnigy 3000 mAh 5s 20C Lipo Pack)

Charger - $17

Wiiceiver- $50
(Diyelectricskateboards)

Trucks and wheels - $60

Deck - $25

VESC - $106
(Enertion)

Pulley Kit - $38

misc cost - $30


TOTAL - $439!
```

---
## \#7 Posted by: eLDoska Posted at: 2016-05-03T22:34:47.409Z Reads: 290

```
740kv is to high. high kv = less torque + overheating
wiieceiver? if you have kama nunchuck you can connect in direct to VESC
1 VESC for 2 motors? bad idea. for 2 motors you need 2 VESCs (+100$)
```

---
## \#8 Posted by: sl33py Posted at: 2016-05-03T22:54:29.428Z Reads: 286

```
Let's break it down:

Motors - 42mm motors are not going to work well.  Minimum of 50mm, or 63mm (better - more powerful).  
KV of motors - shoot for 190-245kv (lower kv helps, but too low has shown to not help!).

Batteries - get 3s or 4s batteries - in series will give you more voltage (2x3s=6s), in parallel will give you more Ah (=range).
You will pay more for higher S batteries (6 and 8s single batteries), AND you will need a special charger usually for over 6 or 8s.  Plus most hobby / RC Car ESC's max out around 6s (some only 4s).  If you are getting a VESC (best option IMO) - be aware of the configuration steps needed to get them working properly.  It's not totally plug and play.  If you can follow steps and be cautious you shoudl be fine.

Charger - you probably don't want the $17 charger.  I would look at the iMax B6v2 as the minimum.  IMO.

Wiiceiver - look at the GT2b and badwolf (and similar) cases.  More reliable than wiiceiver and Nyko. IMO.  I have a couple of each.  The Nyko/Wiiceiver combo is the most prone to dropping and interference.  If you live in a populated area with lots of WiFi - i'd definitely steer clear and go GT2b.

Trucks and wheels - cool

Deck - $25?  hopefully it will hold up - i like nice decks (i'm not 14 and spend far too much on mine - it's all good, but maybe look at a better used deck to start?)

VESC - perfect.  but you need to double the cost, because you need one ESC (or VESC) *per motor*.  One will not control both.

Pulley Kit (need to x2).  AND this doesn't include motor pulley, or motor mounts (x2).  I again would recommend you get a dual motor mount kit - I also am not a fan of printed wheel gears as they simply are not as strong and wear faster than aluminum or steel gears.

Misc costs - heat shrink, soldering iron and solder, an enclosure?

HTH - GL!
```

---
## \#9 Posted by: xPouca Posted at: 2016-05-03T23:29:27.940Z Reads: 247

```
Is this a good motor? Is it 50mm? http://www.hobbyking.com/mobile/viewproduct.asp?idproduct=18126
```

---
## \#10 Posted by: xPouca Posted at: 2016-05-03T23:31:08.353Z Reads: 242

```
And what are the S batteries? This motor http://www.hobbyking.com/mobile/viewproduct.asp?idproduct=18126 Said something about 10s Lipoly
```

---
## \#11 Posted by: barajabali Posted at: 2016-05-03T23:43:35.737Z Reads: 239

```
s means series.  so when you see 10s it means 10 series which are (10) 3.7 volt cells in series giving you 37 volts
```

---
## \#12 Posted by: barajabali Posted at: 2016-05-03T23:44:21.134Z Reads: 238

```
ehh not sure that anyone has experience on here with that. looks to me on backorder anyway
```

---
## \#13 Posted by: sl33py Posted at: 2016-05-04T00:12:46.557Z Reads: 246

```
I'd look at the SK3 63mm motors - you want an 8mm shaft not 6mm (like on the one you linked).  Not only stronger, but the common size for your motor gear.  

Here's a link to one (backordered - seems like most are).  I'd check your local warehouse.

http://www.hobbyking.com/hobbyking/store/__18181__Turnigy_Aerodrive_SK3_6364_190kv_Brushless_Outrunner_Motor.html?strSearch=SK3%2063

Another good option is the Tacon 160:
http://www.hobbypartz.com/96m608-bigfoot160-5335-245kv.html

Also out of stock.  Tough motors to find.  If you are patient they will show up eventually.

Seriously - on a budget build i would get one 63mm motor (one like those linked) and add later if not enough power.  I have a 63mm 200kv motor that moves me along well and i'm probably 2 (or 3) of you.  6'8" 265lbs.  I don't go up big hills on it and it's geared a bit lower for my weight.

Google Lipo batteries series and lipo batteries parallel.  Some education on the reasons for each is needed here xPouca.  It's relatively simple - higher voltage (more power), or more range.  Your VESC can take up to 12s w/ a motor of less than 200kv - 10s with over 200kv motor.  (haven't checked in a while if newest 4.1x VESC has changed this - so someone correct me if wrong/outdated).

Just remember that more power isn't always ideal - you need more expensive batteries, and specialty chargers.  Definitely adds complexity.
```

---
## \#14 Posted by: sl33py Posted at: 2016-05-04T00:24:21.751Z Reads: 227

```
here's my GF's setup w/ a single motor. Moves me along fine...  Nice simple setup and about 13-14lbs iirc. (depending on the 2x3s or 2x4s batteries).

[img]/uploads/db1493/original/2X/8/8109ffc093ab7710b291beef94b6618bcbf562bc.jpg[/img]
Has the wiiceiver - she likes it and the small drops aren't an issue since she goes about 8mph tops.
```

---
## \#15 Posted by: eskateking Posted at: 2016-05-04T18:25:16.890Z Reads: 214

```
All mechanics under the board
http://www.enertionboards.com/diy-electric-skateboard-kits/mono-drive-mechanical-kit - $257

motor
http://www.hobbyking.com/hobbyking/store/__67773__Turnigy_Aerodrive_SK3_6364_245kv_Brushless_Outrunner_Motor_AR_Warehouse_.html - $73

battery
http://www.hobbyking.com/hobbyking/store/__8583__ZIPPY_Flightmax_5000mAh_3S1P_25C.html - $25 x 2 = $50

charger
http://www.hobbyking.com/hobbyking/store/__5548__IMAX_B6_50W_5A_Charger_Discharger_1_6_Cells_GENUINE_.html - $25

remote
http://www.hobbyking.com/hobbyking/store/__31671__HobbyKing_174_8482_HK_GT2B_3CH_2_4GHz_Transmitter_and_Receiver_w_Rechargable_Li_ion_Battery.html - $24

esc
product/single-motor-120a-6s-esc/ - $70

Total: $499

Add 100 dollars for a good deck and thats everything you need.
```

---
## \#16 Posted by: longhairedboy Posted at: 2016-05-04T18:51:27.688Z Reads: 205

```
[quote="xPouca, post:6, topic:2844"]
I was planning on one motor but the one I saw had 1,000 watts and just thinking about it, 1,000 watts on one wheel is weird because that can make it go off balance
[/quote]

1) torque steering isn't really as much of an issue as some people might make it out to be. The motors I use in dual drives are rated at 2400 watts each and the single drive motors i use are rated at 3200 watts. ooooh 3200 watts on one wheel sounds serious! but its not. It doesn't yank you to one side as much as people think it will, especially if you have it heel side like you should. 

2) That doesn't mean that either of those motors are ever going to see over 2000 watts even in a single drive config where one is doing all the work on one wheel. They most likely won't. They're just able to handle that if you cold even fit that much battery pack on them. 3200 watts is 4.2 horsepower for fucks sake. You'll never see that coming out of your pack. 

3) you want the fattest motor you can get and you want it on a lower KV somewhere roughly around 180-200 if you're worried about hills, and those rspecs can handle 6S just fine, so they're not going to burn up from the heat even at their lower kv. but there's nothing stopping you from going 12S on the cheap and charging your packs separately on a dual 6S charger if you want a higher more efficient voltage.
```

---
## \#17 Posted by: xPouca Posted at: 2016-05-05T04:37:53.809Z Reads: 181

```
Are drive kits good? And I saw a reply by eskateking listing everything out but I still feel like I want equal motors (dual). I don't know, I just feel that one motor will yank me. Links and prices will also be amazing. But thanks!
```

---
## \#18 Posted by: outsider Posted at: 2016-05-05T09:38:36.290Z Reads: 180

```
Thanks for all the information. Generally will 190kv always beat out a 245kv motor? Just deciding which one to go for :)
```

---
## \#19 Posted by: eskateking Posted at: 2016-05-05T15:31:00.166Z Reads: 180

```
You truly don't need dual drive. Not at 14. It will not yank you. Enertion drive kits are very reliable.
```

---
## \#20 Posted by: xPouca Posted at: 2016-05-05T17:40:22.502Z Reads: 176

```
One of the motors that I was looking at said something about 10s voltage. Does that mean I need to buy 10s lipo batteries? And how would I connect 2 ESCs to the batteries because all I on YouTube was just 1 ESC soldered to the battery or something like that?
```

---
## \#21 Posted by: eskateking Posted at: 2016-05-05T17:53:13.312Z Reads: 167

```
10s voltage means that that is the maximum you can have. 6s would be fine for that. Also, 2 esc would connect together via a canbus connector such as this one. http://www.ollinboardcompany.com/product/canbus-connector-for-vedder-s-motor-controller
You won't need it though.
```

---
## \#22 Posted by: eskateking Posted at: 2016-05-05T21:01:22.987Z Reads: 162

```
You would connect the master to the batteries that are connected in series, and then slave esc would connect via can-bus to the master.
```

---
## \#23 Posted by: xPouca Posted at: 2016-05-06T04:50:54.812Z Reads: 155

```
Is http://www.hobbyking.com/hobbyking/store/__67773__Turnigy_Aerodrive_SK3_6364_245kv_Brushless_Outrunner_Motor_AR_Warehouse_.html good? It seems like the motor is a bit too much for one wheel. I'm starting to actually get into that 1 motor or none idea. Is 3200W too much for one wheel? Will it yank a 119 pounds guy? Should the motor be on heel side or toe side? And does it have enough torque to climb up steep hills? And if I were to want to upgrade to dual, is it enough room?
```

---
## \#24 Posted by: makepeace Posted at: 2016-05-08T15:50:59.720Z Reads: 162

```
Heel side/toe side is all about preference really. It's more of a matter of whether you feel more comfortable leaning back or forward under acceleration. That being said, heel side has totes more pressure on the drive wheel, which means more friction and thus more traction.

What is very important to note is that the turning effect of having one motor is very very small, in comparison to the weight of your body and how you apply that on your boards gas pedals. Boards have a very long wheelbase, and a very short axle length. This means that the turning torque about the pivot point somewhere in the centre of the board is very small, so the 'yanking' turning force is always going to be small, in comparison to the yanking force forward (or backward on your body). Negligible, in fact. You won't even feel it, cognitively, as your body will naturally react to oppose it to get you to go straight.

So, long and short of it, that motor would be fine for you, you will just need to set the acceleration at a comfortable level so as not to be yanked backwards and fall off the board in that way.

As regards hills, depends how steep. That motor will be fine for you for most common grades.

As regards adding another motor, you won't have enough space with that motor to do a dual rear drive, but there is nothing wrong with putting it on the front. I actually find dual diagonal way more comfortable and agile than dual rear. But if you want to powerslide, go dual rear, and in that case you should be looking for a 6355 or there abouts motor.
```

---
## \#25 Posted by: willpark16 Posted at: 2016-05-09T03:11:24.702Z Reads: 157

```
Have u done any reading on this yet? Everything ur asking is covered on this forum just look it up.
```

---
## \#26 Posted by: woxishashou Posted at: 2017-02-13T02:43:34.673Z Reads: 99

```
Do you want DIY?
Or buy a piece of dual motor electric longboard?
600$ Enough to buy http://www.gearlab.us/electric-board.html
```

---
