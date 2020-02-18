# 50a enough for dual motors and steep hills?

### Replies: 44 Views: 1356

## \#1 Posted by: Orin635 Posted at: 2018-05-09T15:40:20.697Z Reads: 209

```
Hi guys,

I currently have a pretty weak 6s LiPo battery powering dual 5055 270kv motors and I live in a very hilly area. I want to upgrade my LiPos soon to a better Li-On pack and found the 10s5p Li-On pack from diyeboards. This is a very good price (I think) but the problem I think for me would be is that it only outputs 50a. so would 25a per motor be enough? I know 270kv is quite high so I want to change the 3:1 gearing ratio to 5:1 when I upgrade the battery.

So I'm basically asking would 25a per motor be enough and with a 5:1 gearing ration should I be able to get up steep hills?
```

---
## \#2 Posted by: evoheyax Posted at: 2018-05-09T15:52:07.469Z Reads: 203

```
Depends largely on your weight. Also depends on your definition of steep. Also depends on what your definition of "go up" is. You might get there, but not the fastest.

Some of it will just be trial and error. I always side on the side of more amps. But another big factor is the motor. I can't speak as much on whether this will work or not, since I'm not a belt guy. If I were talking about hub motors, I would say 25 amp per motor is not that great at 10s. But belts can get a bit better efficiency, so you might be able to squeeze a bit more out of them.
```

---
## \#3 Posted by: Orin635 Posted at: 2018-05-09T15:57:51.927Z Reads: 187

```
Thanks for the reply!
I only like to go at 25km/h not even. not sure how to describe the steepness, Im not that heavy im only 16.I think I will probably just have to wing it and hope for the best I would like to get higher amp battery pack but unfortunately diyeboards dont sell anything high
```

---
## \#4 Posted by: professor_shartsis Posted at: 2018-05-09T17:09:23.790Z Reads: 153

```
what’s your tire diameter?
```

---
## \#5 Posted by: Namasaki Posted at: 2018-05-09T17:15:32.837Z Reads: 148

```
I ran some test with an in-line watt meter on a dual drive and my weight being apx 185 lbs going up a hill that was apx 10% grade
Using 12s Opto Car Esc’s and Carvon V2 direct drive motors with 90mm wheels 

Both tests where at apx same speed

12s - 18a total from battery at half throttle 
  6s -  36a total from battery at full throttle 

That should put 10s at apx 27a total 
But as previously mentioned, there are many variables.
```

---
## \#6 Posted by: Orin635 Posted at: 2018-05-09T19:27:03.175Z Reads: 126

```
83mm currently but might soon be 97mm
```

---
## \#7 Posted by: Orin635 Posted at: 2018-05-09T19:28:48.394Z Reads: 122

```
Good info to know! thanks!

I don't think 25a per motors will be enough unfortunately :worried:
```

---
## \#8 Posted by: professor_shartsis Posted at: 2018-05-09T19:47:17.186Z Reads: 110

```
[quote="Orin635, post:6, topic:54915, full:true"]
83mm currently but might soon be 97mm
[/quote]


@Orin635 here is a chart predicting the performance you will get with 25a battery current limit and 80a motor current limit per motor (83mm tire, 3:1 gear reduction, 2 motors, 270kv, 22.8v battery)... top speed looks to be about 19mph (red line, bottom left chart - thrust pounds minus wind drag force) and peak vehicle thrust is roughly 90lbs (yellow line, bottom left chart - vehicle thrust pounds 2 motors):

https://image.ibb.co/b2GjJy/6s.jpg
```

---
## \#9 Posted by: Orin635 Posted at: 2018-05-09T19:54:03.811Z Reads: 93

```
So much information right there its very hard to understand it. Is that a website you got that information from?
```

---
## \#10 Posted by: professor_shartsis Posted at: 2018-05-09T20:03:38.872Z Reads: 93

```
@Orin635 here are some of the formulas involved in the prediction: 

[quote="professor_shartsis, post:309, topic:46485"]
you can start with the ground speed and wheel diameter to get the wheel rpm,

next use the wheel rpm times the gear reduction (wheel teeth / motor teeth = gear reduction) to get the motor rpm.

next use motor rpm / motor kv to get the back emf v,

then use ((pack v * duty %) - bemf v) / winding resistance = motor current

then 60 / (2 * pi * kv) for motor torque in newton meters per motor amp

then motor current times the torque per motor amp for motor torque

multiply the motor torque times the gear reduction for wheel torque

vehicle thrust comes from relationship between the wheel torque and wheel diameter-- (wheel torque in newton meters  * 1000mm) / ((1/2) * wheel diameter in mm) = vehicle thrust in newtons per motor

then you can get the mechanical watts from motor torque in newton meters times motor angular velocity in rad/sec

electical wattage is (pack v * duty %) * motor current = electrical watts

battery current is electrical watts divided by pack voltage

you can calculate the ohmic heating from motor current *  motor current * winding resistance = wattage copper loss & ohmic motor heating

wind drag force in newtons is (1÷2) * 1.225 kg/m^3 fluid density of air * estimated frontal area in m^2 * (velocity in meters per second * velocity in meters per second) * estimated drag coefficient = wind drag force in newtons

wind drag power/wattage is wind drag force in newtons * meters per second = wind drag power/wattage

ignored is iron loss, esc loss, battery loss, drivetrain loss, and rolling resistance.
[/quote]
```

---
## \#11 Posted by: Orin635 Posted at: 2018-05-09T20:07:28.454Z Reads: 76

```
So what sort of information does the diagram give me? I dont really understand it
```

---
## \#12 Posted by: Hummie Posted at: 2018-05-09T20:08:36.727Z Reads: 77

```
[quote="professor_shartsis, post:10, topic:54915"]
you can start with the ground speed and wheel diameter to get the wheel rpm,

next use the wheel rpm times the gear reduction (wheel teeth / motor teeth = gear reduction) to get the motor rpm.

next use motor rpm / motor kv to get the back emf v,

then use ((pack v * duty %) - bemf v) / winding resistance = motor current

then 60 / (2 * pi * kv) for motor torque in newton meters per motor amp

then motor current times the torque per motor amp for motor torque

multiply the motor torque times the gear reduction for wheel torque

vehicle thrust comes from relationship between the wheel torque and wheel diameter-- (wheel torque in newton meters  * 1000mm) / ((1/2) * wheel diameter in mm) = vehicle thrust in newtons per motor

then you can get the mechanical watts from motor torque in newton meters times motor angular velocity in rad/sec

electical wattage is (pack v * duty %) * motor current = electrical watts

battery current is electrical watts divided by pack voltage

you can calculate the ohmic heating from motor current *  motor current * winding resistance = wattage copper loss & ohmic motor heating

wind drag force in newtons is (1÷2) * 1.225 kg/m^3 fluid density of air * estimated frontal area in m^2 * (velocity in meters per second * velocity in meters per second) * estimated drag coefficient = wind drag force in newtons

wind drag power/wattage is wind drag force in newtons * meters per second = wind drag power/wattage

ignored is iron loss, esc loss, battery loss, drivetrain loss, and rolling resistance.
[/quote]

and the load is assumed more I guess with the larger amps used
```

---
## \#13 Posted by: professor_shartsis Posted at: 2018-05-09T20:09:00.027Z Reads: 66

```
[quote="Orin635, post:11, topic:54915, full:true"]
So what sort of information does the diagram give me? I dont really understand it
[/quote]

the yellow line on the bottom left chart shows how many pounds of thrust you have at different speeds with those settings.
```

---
## \#14 Posted by: professor_shartsis Posted at: 2018-05-09T20:10:06.276Z Reads: 65

```
[quote="Hummie, post:12, topic:54915"]
and rider weight right?
[/quote]


if you want to calculate acceleration in m/s^2 then you need rider weight, but it isn't a factor in calculating vehicle thrust or wind drag force on flat ground.
```

---
## \#15 Posted by: Orin635 Posted at: 2018-05-09T20:11:33.732Z Reads: 66

```
so at 20mp/h i'll have 0 pounds of thrust?
```

---
## \#16 Posted by: Hummie Posted at: 2018-05-09T20:11:50.944Z Reads: 67

```
50amps and 12s works good for me doing steep hills.  enough.  im 155lbs.  especially with a pulley setup should be even less an issue
```

---
## \#17 Posted by: professor_shartsis Posted at: 2018-05-09T20:13:18.172Z Reads: 70

```
[quote="Orin635, post:15, topic:54915, full:true"]
so at 20mp/h i’ll have 0 pounds of thrust?
[/quote]

right, notice how the back emf voltage produced by the spinning magnets on the rotors (which opposes the battery voltage - red line top left chart - back emf voltage) increases with speed and surpasses the maximum pwm effective voltage of your battery/controller right below roughly ~20mph (yellow line, top left chart - effective pwm voltage).
```

---
## \#18 Posted by: Orin635 Posted at: 2018-05-09T20:14:16.679Z Reads: 70

```
There's no 12s option from diyeboards and if I was making it myself or buying from a battery builder I would just get a higher discharge cells
```

---
## \#19 Posted by: Orin635 Posted at: 2018-05-09T20:15:49.165Z Reads: 72

```
Yes I see that
```

---
## \#20 Posted by: Orin635 Posted at: 2018-05-09T20:18:01.465Z Reads: 70

```
Is this diagram for a 10s battery? or 6s?
```

---
## \#21 Posted by: professor_shartsis Posted at: 2018-05-09T20:19:24.812Z Reads: 66

```
[quote="Orin635, post:20, topic:54915, full:true"]
Is this diagram for a 10s battery? or 6s?
[/quote]

6s -- assumed was 3.8v per cell * 6 cells in series = 22.8v battery
```

---
## \#22 Posted by: Orin635 Posted at: 2018-05-09T20:20:39.319Z Reads: 65

```
Ok so the diagram for what Is for my current setup?
```

---
## \#23 Posted by: professor_shartsis Posted at: 2018-05-09T20:21:06.436Z Reads: 63

```
[quote="Orin635, post:22, topic:54915, full:true"]
Ok so the diagram for what Is for my current setup?
[/quote]

yes-- with 25a battery limit & 80a motor limit per motor.
```

---
## \#24 Posted by: Orin635 Posted at: 2018-05-09T20:23:17.885Z Reads: 64

```
Ok, i think there was some confusion. The diagram is a mix between my current setup and what I want it to be/upgrade it to
very sorry
```

---
## \#25 Posted by: skatardude10 Posted at: 2018-05-09T21:16:14.703Z Reads: 62

```
For reference, whatever value this may be...

My gearing is heavily bias towards speed over torque, at 20/32 on 90mm flywheels.

I run 30A each vesc and have *plenty* of torque to get up steep hills, and I weight 200 lbs, and my board weighs quite a bit too. 

I have a feeling, with 25A to each vesc, not weighing much, and geared for torque, you probably won't be lacking the torque you need to get you up hills.
```

---
## \#26 Posted by: skatardude10 Posted at: 2018-05-09T21:18:13.416Z Reads: 59

```
Hey, have you shared this Excel / spreachsheet calculator by chance? 

Id love to play with it to run some numbers.
```

---
## \#27 Posted by: Pedrodemio Posted at: 2018-05-09T21:25:11.280Z Reads: 57

```
I run dual 5055 190Kv with 14:34 gearing on 80mm wheels, I can keep 30km/h up to 15% grade with 30a total battery current and 40a each motor, more than that I can climb up to 24% at 17km/h

I wouldn’t run more than 40a on 5055 motors since even with that they can get pretty hot
```

---
## \#28 Posted by: Orin635 Posted at: 2018-05-09T21:29:16.619Z Reads: 56

```
thats great to hear I really hope your right :joy:
```

---
## \#29 Posted by: Orin635 Posted at: 2018-05-09T21:30:30.501Z Reads: 54

```
also good to hear. some say it'll work some say maybe not. I will probably go with it now. still hard to decide
```

---
## \#30 Posted by: Orin635 Posted at: 2018-05-09T21:30:44.476Z Reads: 54

```
yes i'd love to aswell
```

---
## \#31 Posted by: skatardude10 Posted at: 2018-05-09T21:38:45.987Z Reads: 54

```
I do run dual 6374, but with a 5:1 gear ratio, even with the reduced torque from 5055 motors at 270kv, you should be in a very good place torque wise. 

One thing to look out for though, is that with 10S and 270kv, your ERPMs at max RPM are 68K, well above the 60K limit. I'd suggest going down with your motor kv... Maybe around or under 230kv, and not going so high with your gearing... Maybe 4:1 with 230kv motors. 

If you stick with 270kv and 10S, just know that at top speed you really do risk burning a DRV chip or two and faceplanting because of it. You can try limiting max ERPM in firmware configuration, but I don't know how reliable that is, because if you coast over that going down a hill I'm pretty sure you are still screwed unless you set it to brake at a certain speed. 

I just wouldn't go there, and wouldn't drop a 10S in place of a 6S when running 270kv. I'd make other changes, like motors to ensure you don't even have the potential to go over 60K erpm on full throttle.

Calc.esk8.it
```

---
## \#32 Posted by: Orin635 Posted at: 2018-05-09T21:47:45.795Z Reads: 54

```
I wont be changing my motors for a long time I need to upgrade other parts first. I dont even have vescs yet. I currently use the eBay ESC which has been doing very well for me. aswel. someone told me to limit the ERPM to around 55k and in real world test I probably wont even reach that only if you use full throttle with wheels in the air
```

---
## \#33 Posted by: Pedrodemio Posted at: 2018-05-09T22:00:40.259Z Reads: 47

```
What’s your wheel size? And 10S right? I have a spread sheet that is simple to understand. 4:1 is hard to do since you have low  clearence and/or low teeth in mesh on the motor pulley

You could reconnect you motor in Star to lower the Kv by sqrt(3) factor
```

---
## \#34 Posted by: Orin635 Posted at: 2018-05-09T22:06:09.271Z Reads: 50

```
Put in please 97mm wheel size, 10s and im not sure for gearing ratio. according to this calculator http://calc.esk8.today/ 1:4 give me a top speed of 45km/h which I wont get close to. preferably I would like a 1:5(to give me 36km/h top speed) but then as you say I would have little teeth on the wheel pulley. maybe I could add a idler pulley?
```

---
## \#35 Posted by: Orin635 Posted at: 2018-05-09T22:07:24.781Z Reads: 45

```
Then again for a 1:5 ratio I would need a 60t pulley
```

---
## \#36 Posted by: Pedrodemio Posted at: 2018-05-10T01:26:45.529Z Reads: 48

```
The problem is not even teeth in mesh, this you solve with an idler as you said, but lower than 14T the diameter of the pulley is too small, the belt in bent more than it should and it will last a lot less

Here's 1:4, looks good, top speed wise is the same gearing I use on my board, BUT the pulley sits a 4mm from the ground, even less if you consider belt thickness, unless where you live the road is pristine and no little rocks exist, you can't use that

With 1:5 the wheel pulley would be bigger than the wheel 

![image|280x500](upload://iv9aQ7MqDYIlWV57KhUs3Uuu0F1.png)

The best you can do with these motors is 1:3,14

![image|280x500](upload://uO3zouEQZu1qD47mlK9re07wqCn.png)
```

---
## \#37 Posted by: lrdesigns Posted at: 2018-05-10T03:19:11.946Z Reads: 42

```
You can't really go bigger than 48 tooth on 97mm wheel with M5 pitch belts. The pulley is just too low to the ground. 48 is already kinda bad. 

If you switch to M3 pitch belts then you can get a better ratio, but that introduces other problems. Almost no one uses M3 pitch.

Also to your main question, 25a per vesc should be enough torque for hill climbing with the right ratio and considering your not that heavy / not a top speed addict.
```

---
## \#38 Posted by: Orin635 Posted at: 2018-05-10T12:48:10.794Z Reads: 40

```
My dual esc has 3 speed controllers. Maybe if I just leave it on the lowest speed and pop it on to highest speed or middle going up a hill. I think I will leave my gears and everything for now and buy the new battery's over summer
```

---
## \#39 Posted by: professor_shartsis Posted at: 2018-05-10T16:46:14.594Z Reads: 40

```
[quote="Orin635, post:38, topic:54915"]
I think I will leave my gears and everything for now and buy the new battery’s over summer
[/quote]

it looks like with 10S, 80a motor limit, 25a battery limit per motor on a vesc, you can reach roughly ~32mph (red line, bottom left chart, net thrust pounds, thrust minus wind drag force 2 motors)...

here is a comparison of 6S (22.8v -- 19mph) vs 10S (38v -- 32mph):

https://image.ibb.co/hDCGiy/6s_vs_10s.gif
```

---
## \#40 Posted by: Orin635 Posted at: 2018-05-10T17:03:01.653Z Reads: 36

```
So if im reading it correctly I wouldn't get that big a boost for climbing hills?
```

---
## \#41 Posted by: professor_shartsis Posted at: 2018-05-10T17:25:55.456Z Reads: 36

```
[quote="Orin635, post:40, topic:54915, full:true"]
So if im reading it correctly I wouldn’t get that big a boost for climbing hills?
[/quote]


and here is a comparison of 10S -- 5:1 vs 4:1 vs 3:1 vs 2:1 gear ratios (25a bat limit per motor, 80a motor limit):

https://image.ibb.co/hmv0bJ/2_3_4_5.gif

(if you switch to 10S, then gear it at 5:1, I believe you'll get a significant boost -- not in top speed but peak vehicle thrust, that said 2:1 @ 10S gives ~40mph top speed...)
```

---
## \#42 Posted by: Orin635 Posted at: 2018-05-10T18:43:19.573Z Reads: 34

```
I'm thinking a 4:1 ratio, it'll have plenty of speed and quite a lot of torque and that means i'll only need a 48t pulley on the wheel which should be ok
```

---
## \#43 Posted by: Orin635 Posted at: 2018-05-10T18:50:37.469Z Reads: 33

```
Just half read this post https://www.electric-skateboard.builders/t/gearing-ratio-for-torque/34348
seems he was trying to do bout the same as me. I think I will get the new battery and then try everything out then 3D print pulleys and see how well it does. maybe even add a cover for the wheel pulley depending on if I want to keep the higher wheel pulley
```

---
## \#44 Posted by: Pedrodemio Posted at: 2018-05-10T22:56:36.876Z Reads: 30

```
It’s close to the ground, but if the places you ride are relatively clean it should work

You will know if your belt start to look like a Swiss cheese
```

---
