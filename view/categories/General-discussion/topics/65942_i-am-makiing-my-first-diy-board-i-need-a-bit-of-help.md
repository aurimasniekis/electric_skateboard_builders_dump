# I am makiing my first DIY board, I need a bit of help

### Replies: 17 Views: 354

## \#1 Posted by: AfterByte Posted at: 2018-08-24T13:03:35.598Z Reads: 104

```
my budget is as close to 1150 bucks as possible, this is my list, 

Deck : Landyachtz Evo ($135)

Trucks : Torque board 218mm ($65)

Bushings : green 90a  (have already)

Bearings : Zealous ($14)

Wheels : ABEC 11 107mm ($140)

Extra hardware : ($8) (0.25 inch shock pads and bolts)

power kit -  single 6374 and extra parts ($765)
(266 watth battery 12s2p, 15mm wide belts, 14t 40t gear ratio) 

Total cost - $1127 USD

I am 195 pounds and live in a really hilly area, I wish I could afford 2 motors, but I cant, I plan on upgrading in the future. What top speed and range will I get out of this configuration, and is there a way to limit top speed without reducing torque? i want to ease into the board when I first get it, the fastest I have ever gone was 26mph on my backfire g2s. ( I am also trying to keep a low center on gravity on this build wale still having enough clearance)
```

---
## \#2 Posted by: Skunk Posted at: 2018-08-24T13:09:47.535Z Reads: 96

```
@psychotiller just added 107mm superflys for $140  https://psychotiller.com/product/new-abec-11-superflys
```

---
## \#3 Posted by: Lumaci Posted at: 2018-08-24T13:13:33.255Z Reads: 95

```
[quote="AfterByte, post:1, topic:65942"]
I wish I could afford 2 motors
[/quote]

You can, just dont buy that kit.

Buy motors and a dual vesc from flipsky, they charge the same price for two motors that diy do for one almost same goes for their dual vesc you only pay like 30 bucks more for two vescs in one compared to their one vesc if you use their 20USD/20% off coupon code.
```

---
## \#6 Posted by: Skunk Posted at: 2018-08-24T13:19:03.314Z Reads: 87

```
http://esk8.today/2016/12/28/how-far-can-i-ride/#rc
http://esk8.today/2017/01/03/how-fast/

These help alot
```

---
## \#7 Posted by: Skunk Posted at: 2018-08-24T13:21:56.023Z Reads: 87

```
You can get a deck from @Hummie for less and the cutout really helps keep things low profile. 
![9e0ac875acde2fd696fdeaf4bee9ae49b26bf637_1_618x500|618x500](upload://8aN5yMWCDCudRb2dgxrTMYjAGfY.jpeg)
![abb83b69a1385b2b296d4e1ab180c47ccf264962_1_666x500|666x500](upload://9FfRG87UYXrggRHitb5IOT3VRFh.jpg)
```

---
## \#8 Posted by: AfterByte Posted at: 2018-08-24T13:29:37.118Z Reads: 81

```
I actually looked into flipsky, but with 2 6355 motors the build came out to 1360 dollars,(and a single 6374 setup with their vesc is only like 20 dollars cheaper, and it would mean I would have to solder vs the DIY eboard kit that is all plugs, for 20 more dollars I would much rather just have the plugs for easy maintenance and building)    I am also not going with a KIT from DIYeboard, I parted it out as I don't need the bearings and the crappy wheels from the kits. (saves me 25 dollars by avoiding the kit) By parting it out, I was able to use a different gear ratio also for more torque.
```

---
## \#9 Posted by: Lumaci Posted at: 2018-08-24T13:38:19.692Z Reads: 74

```
You just solder bullet connecters onto their vesc, the motor already comes with them.

If you dont know how to solder i would advise you to learn it before you build, and the kit is a bad idea specially since you want to part it out buy from different suppliers and you can get more for the money.


And just do a little research and get some parts from forum (Motor mounts) And its very possible.

For 1200 dollars i made a board for a friend of mine with dual 6374 motors we went with lipos + bms and was able to do a 10s5p pack and went with premium deck enclosures everything great.


Just look up different websites and find the parts you need and compare prices and you will be surprised by how much you can get in your budget.


I just made a board for myself all parts comes down to 1.321USD and its a dual drive 10s3p board and i live in EU so its way more expensive over here due to shipping and import fees.
```

---
## \#10 Posted by: AfterByte Posted at: 2018-08-24T13:41:13.256Z Reads: 70

```
thanks that helped alot, I got around 35 miles per hour and about 14 ish miles of range. Whats the best way to limit the speed of the board say I don't want to go above 25 miles per hour when I first get it?
```

---
## \#11 Posted by: Lumaci Posted at: 2018-08-24T13:42:29.444Z Reads: 67

```
Limit it in the vesc tool.

If you get a metr module you can make modes to cap the speed and change on the go.
```

---
## \#12 Posted by: AfterByte Posted at: 2018-08-24T13:52:59.114Z Reads: 61

```
I know how to solder, I work on competition robots at my school, (not small, last one was 6 feet by 4 feet by 5 feet)  I just like the ease of use aspect as its easy to swap out parts and will take less time to build. I will look into other motor mounts on the forum, thanks for telling me that. I know I could get better price to performance if I went with a cheaper deck and other parts, and I probably could get a dual motor in my price point, but I didn't want to get some of the other cheaper parts I was looking into for example pullies/ gearing as the cheaper stuff was all plastic. I want to get metal pulleys. I also could save a lot of money on wheels, but I really liked moving from 80mm to 96mm wheels on my backfire and I even wish the wheels were larger at times (just without the torque loss) I picked parts that fit my design and to what I want my board to be like. That being said, thanks for the info on checking this forum out for motor mounts, will diffidently look into that.
```

---
## \#13 Posted by: AfterByte Posted at: 2018-08-24T13:55:08.818Z Reads: 62

```
thanks for the info, will look into a metr module. (how would i limit it in the vesc tool? what setting is it?)
```

---
## \#14 Posted by: Simonwantstobuildabo Posted at: 2018-08-24T13:56:56.628Z Reads: 61

```

Hi! My dual beast 6355 maytech motor setup, with dual focbox and 12s5p has some issues!
( I use maytech standard remote and reciver )

Also i use VESC TOOL!

One of the motors in “fast mode” shuts down? So i can press full throttle in eco mode, no problem, but when i switch to fast mode it shuts off after a while? Like you can hear 100% Throttle, and after 5,10,20 seconds it goes down to like 60% or even less?

Short version: When pressing full throttle in fast mode, motor start slowing down.

Please help vesc tool gods!
```

---
## \#15 Posted by: Lumaci Posted at: 2018-08-24T13:57:17.432Z Reads: 59

```
You can still get all metal pulleys, the truth about 90% of all esk8 parts sellers is that they get their parts from some where else.

If you go on ebay you can find exactly the same pulley diy sells for half the price, the same motors for half the price heck maybe even the same vesc for 10 - 20 dollars less.

It wont take longer to build by just soldering on 6 bullet connecters and will still be as easy to swap everything out.


I clearly remember building my first board, i spent over 1000 dollars for a single 6374 build from them and today i look back and see how stupid i was for not doing the reserch needed or taking my time.

I can build my same board for half of what i used back then now, take your time and you can get even higher quality parts for less.
```

---
## \#16 Posted by: Lumaci Posted at: 2018-08-24T13:58:48.820Z Reads: 57

```
You limit it with the max amps applied to the motor, if you do like 60 amps you will get full speed but you can limit it to like 40 or something and it will do less or something like that.

Cant exactly remember how to do it since i havent programmed a vesc for lower speeds in ages.
```

---
## \#18 Posted by: rey8801 Posted at: 2018-08-24T14:20:17.963Z Reads: 50

```
Generally speaking you can limit the speed in several way:
-limit the max rpm (you make the calculation based on the wheel diameter and you get the rpm)
-limit the power output as current or watt if you use firmware based on that (@Ackmaniac)
-limit directly the speed through the @Ackmaniac app 

Same things you can do it from your phone, it is actually faster since you create several modes and you can swap them on the road. 
Exemple of mine.
![vescmonitor|281x500](upload://olBxMKqEhu2eoA2PjNseaR8WZOX.jpg)

To do that you can by a HM-10 module, doesn't have to be a metr one, also the cheap one will work. If you want one plug and play I have some. Otherwise buy it on ebay or Aliexpress and wire it :wink:
```

---
## \#19 Posted by: Lumaci Posted at: 2018-08-24T14:21:07.584Z Reads: 42

```
Damn pussy mode hahaha
```

---
## \#20 Posted by: rey8801 Posted at: 2018-08-24T14:21:59.500Z Reads: 43

```
ahaahah for who wants to try it
```

---
