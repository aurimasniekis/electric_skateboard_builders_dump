# Questions about my first build

### Replies: 16 Views: 2751

## \#1 Posted by: jakobnator Posted at: 2016-01-21T06:31:58.000Z Reads: 113

```
Hi, I am working on my first electric long board build. I have some prior experience with electronics but never have ridden a long board before, however I have high hopes it will be easy due to the fact that I consider myself pretty good at snowboarding, and surfing. Anyways I have purchased a lot of my parts (listed below) and just had a few questions.

Build:
40" blank bamboo deck (had to buy clear griptape) 
amazon trucks/wheels/hardware ki
ebay noname flywheels
Turnigy 6364 245kv 
FVT esc
FVT USB programmer 

I still need to buy batteries, charger, some sort of enclosure, wiiceiver and various connectors/wires. I plan to buy two zippy 5000mah 3S batteries and put them in series, and connect the balancers to an adapter and make it a true 6s battery. Also planning on getting an imax b6 clone for a charger. 

Questions about my drive train, I went with a t17 to t40 (5mm pitch HTD5) reduction because sdp-si didn't have a motor pulley that had an 8mm shaft lower than 17t. Looking back however I probably could have just drilled out the extra 2mm. 

So mathematically speaking I have 83mm wheels, t17 to t40 reduction, 245kv motor and a 6s setup according to the long board calculator website (assuming 90% efficiency) gave me a weighted speed of 20.22 mph. Do you think this reduction is sufficient for me? I don't need crazy hill climbing abilities, but I weigh about 230 lbs and plan to be 245 lbs. I just don't want to put too much stress on the motor. 

Also the belt I got was originally meant for a t15 to t40 gear ratio, does the bigger motor gear make the center distance for the gears too close together? SDP/SI has a center distance calculator that isn't working for me. 

Thanks for your help.
```

---
## \#2 Posted by: torqueboards Posted at: 2016-01-21T06:47:31.080Z Reads: 108

```
eBoard is fairly easy to ride. You shouldn't have any issues.

40T would be cutting it close. 36T would be better 38T if you really need to be.

Should be fine on flat ground. You should kick off though.
```

---
## \#3 Posted by: NNGG Posted at: 2016-01-21T06:55:36.727Z Reads: 110

```
Dont get the imax clone, I've heard bad things about them, I would get a genuine one.
```

---
## \#4 Posted by: Sharkface Posted at: 2016-01-21T07:00:36.409Z Reads: 116

```
[quote="jakobnator, post:1, topic:1067"]
FVT esc
[/quote]

What amp load can this ESC handle? It's a car ESC correct? (not familiar with this brand, sorry)

[quote="jakobnator, post:1, topic:1067"]
connect the balancers to an adapter and make it a true 6s battery
[/quote]
You dont have to do this if you dont want to, just have a balance charger that can do two batteries at once. The charger I am running can do 4 6s batteries at once. Otherwise there is a diagram somewhere on this forums about how to connect those balance wires... make sure you dont get a spark, its a thing.

[quote="jakobnator, post:1, topic:1067"]
t17 to t40 (5mm pitch HTD5)
[/quote]
the [sdp-si calculator][1] isnt working for me either... but that reduction may cause for some belt slippage. If you are not going on any hills you probably wont have any troubles at all. I have a 12T to 36T setup on my 83mm wheels and that reduction doesnt have as many teeth in contact as I should have (much like the 17T to 40T) but it does work, and get me up hills reallllyyy easily... but tear through belts pretty quick in this configuration.

[quote="jakobnator, post:1, topic:1067"]
Do you think this reduction is sufficient for me? I don't need crazy hill climbing abilities, but I weigh about 230 lbs and plan to be 245 lbs.
[/quote]
somebody will have to weigh in on the weight thing and if it will be good enough, but the reduction level is pretty high. The reduction reliability (as discussed above) may need to be scrutinized. If you really want to not worry about your weight go with a 12S battery setup. I have had 30 pounds on my back, i weigh 170 and notice little to no changes when i take that 30 pounds off. Unless im down hill traveling... then all bets are off. Plus running 12S allowed me to get a much higher torque motor.

[quote="jakobnator, post:1, topic:1067"]
does the bigger motor gear make the center distance for the gears too close together?
[/quote]
considering you are trying to put this under a longboard, while a perfect center distance would be ideal, that ideal situation may not coincide with fitting everything under the board. You probably have such a small difference between a 15T and 17T that all will be well in the world.

Good luck with your build!!!
  [1]: http://sdp-si.com/estore/centerdistancedesigner
```

---
## \#5 Posted by: jakobnator Posted at: 2016-01-21T19:09:51.232Z Reads: 94

```
It's a 120a car esc did some research and people have said good things about it on other forums.
http://www.amazon.com/FVT-120A-Brushless-Sensored-Sensorless/dp/B00LWH3YIA/ref=sr_1_2?ie=UTF8&qid=1453402717&sr=8-2&keywords=fvt+esc

As for the 6s battery I plan on using one of those adapter cables. I don't see the problem since it's basically two 3s balancing plugs plugged into a 6s balancer. For sparking I was going to wire a xt-90 anti-spark in series and make it a "key" instead of having a switch.

I was looking into a voltage meter/ buzzer for lipos apparently you arent supposed to leave them in is there a way I can make a permanent battery meter/buzzer?

Also if I went and got a 15T is it ok if the width is much wider than the 9mm wide belt because they are much cheaper on ebay just a lot wider. 

Lastly what wire gauge would you recommend I plan on using the same gauge for everything just to make it simpler (except for the really small stuff).

Here is a rough mock up of my wiring diagram if you could just double check everything.
http://imgur.com/H5FnQI5
```

---
## \#6 Posted by: EnertionSupport Posted at: 2016-01-21T19:16:17.034Z Reads: 95

```
Welcome to the forum!

Here is a good thread about wiring two 3s batteries together:
http://www.electric-skateboard.builders/t/charging-2-x-3s-lipos-in-series-please-look-over-my-schematic/734/17
```

---
## \#7 Posted by: Randyc1 Posted at: 2016-01-23T05:17:58.986Z Reads: 86

```
Why are you tearing through Belts on 12T 36T ??
```

---
## \#8 Posted by: Sharkface Posted at: 2016-01-23T05:34:52.531Z Reads: 88

```
I have more torque on this motor (149kv SK3 6374) than I can shake a stick at and I am riding up hills with multiple laptops and a spare battery. With a 36T to 12T you are getting as much torque as you are going to be able to get on an 83mm wheel, but not enough teeth will be in contact with the belt on the motor side of things to properly accommodate for the strength of the belt. Think of it like two really evenly paired arm wrestlers. One wrestler is my weight going up hill, while the other is the massive torque behind the motor. While they will put up a good fight, eventually one side will win. In this case, the motor pulley always wins because its putting more pressure on the belt and having less teeth in contact than the wheel pulley. With a low number of teeth in contact, combined with the inevitable stretching of the belt, teeth slip and with this slippage comes tearing of teeth. Eventually all the teeth are torn off and you are walking the rest of the way home.

On the other side of the spectrum I am running a 36T to 20T setup and this gets me an amazing top speed, as well as a LOT of teeth in contact with the belt on the motor pulley. Since there are so many teeth in contact the belt will not slip, but now you have to contend with a heavy stretching factor. Eventually instead of all the teeth getting torn up you are snapping the belt, and again, walking your happy self on home.

They key is to find that happy medium that will allow for enough teeth to be in contact that the belt doesn't slip, but not so many teeth in contact that the belt stretches much faster than intended. I have yet to confirm for myself, but I hear rumors that 36T to 16T is a really really happy sweet spot.  Soon I will be preaching the amazingness of the 63mm brushless motor lol
```

---
## \#9 Posted by: NNGG Posted at: 2016-01-23T06:44:41.755Z Reads: 84

```
yea cant wait for my vesc and run my 16/36 149kv. 
 How many S? do you run yours on?
```

---
## \#10 Posted by: Randyc1 Posted at: 2016-01-23T16:04:04.509Z Reads: 78

```
I will be trying 14T 36T with a 6364-245kv on a 15mm wide belt.
```

---
## \#11 Posted by: Sharkface Posted at: 2016-01-23T17:47:44.200Z Reads: 84

```
[quote="NNGG, post:9, topic:1067"]
How many S? do you run yours on?
[/quote]
This is my first/beater build so I am rocking 12S on Torqueboards ESC. So that 36T to 20T config gets me a wonderful top speed of like 28mph or some crap lol

[quote="Randyc1, post:10, topic:1067, full:true"]
I will be trying 14T 36T with a 6364-245kv on a 15mm wide belt.
[/quote]
If @jakobnator uses that 40T wheel pulley and you use the 36T wheel pulley, both yall will have close to the same motor. Would be cool to see ya'lls builds side by side on a run or two.
```

---
## \#12 Posted by: jakobnator Posted at: 2016-02-07T18:26:20.110Z Reads: 76

```
Alright I am starting my build I have everything now except the motor mount welded. First thing I started with is attaching the gear to the wheel and I am having a REALLY hard time getting the holes in the washer perfectly spaced. I don't have access to a drill press but getting the holes 90 degrees isnt the problem. Anyone have any tips, I am really scared to drill holes in the gear after this many mistakes on the washers. 
<img src='/uploads/db1493/original/2X/f/f780dcc15c6c6f5293cd8c34970951b7bdbe345d.jpg'>
```

---
## \#13 Posted by: psychotiller Posted at: 2016-02-07T19:54:36.853Z Reads: 77

```
You really, REALLY need a drill press. Then before you drill anything you should make a jig to set your washers and pulley on so that you can accurately turn your part to be drilled in each location. 

To make a jig, I've used a piece of flat wood, a socket that specifically fits the washer and another socket to fit the pulley. A long bolt and washer to secure the socket. Then just use clamps to secure the jig to your drill press. Make sure everything is tight so that you have no movement.

Use the jig to mark your hole too! If you don't the time to do it right your build isn't going to be safe or fun to ride.
```

---
## \#14 Posted by: lowGuido Posted at: 2016-02-10T04:46:42.375Z Reads: 72

```
true story.
go find a drill press. someone must have one you can use. neighbor, school, maker space, someone had got to have one you can use.
```

---
## \#15 Posted by: jakobnator Posted at: 2016-02-21T04:34:43.654Z Reads: 66

```
Alrighty, I have my own 3d printer and realized that there are 3d printed solutions!
<img src='/uploads/db1493/original/2X/f/fa6a7759cea72dcb4d68ac3d700d8aba2f84ddf0.jpg'>

Next question, what is the best way to jig the motor mount so it is square with the truck when welding. Also what is the best way to determine the angle the mount should be?
```

---
## \#16 Posted by: wieg16 Posted at: 2016-05-11T17:07:57.936Z Reads: 56

```
What I did was I loosed my trucks to what I would ride them on, and I took a video from different angles showing how the board turned so I would know how much room I had, after analyzing it I made a rough guess where I should put it. I turned the board upside down and held the motor mount where I wanted it. I then proceeded to flex the trucks to see if it would touch (loosing your trucks will help when doing his step so that you don't have to push as hard) once everything looked good I clamped it down and everything fit perfectly! Not the best way but it worked<img src="/uploads/db1493/original/2X/a/aaa7ecaba25490c5631a212090ccb653232e0fa0.png" width="281" height="499"><img src="/uploads/db1493/original/2X/9/9915856e7a4b40971eb4fb9a4369378e1f3aa900.png" width="281" height="499">
```

---
