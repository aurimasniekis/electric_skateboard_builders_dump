# Info about battery pack

### Replies: 28 Views: 3531

## \#1 Posted by: KungFuPanda Posted at: 2016-04-02T21:31:05.799Z Reads: 143

```
HI everyone!

In the past few days I've read a ton of guides about how to build esk8 and I've got a project in my mind...there's just one problem, battery.
I want to build something that won't catch fire and that I can bring with me everywhere, I cannot use Lipo batteries and Lifepo4 are just too big (and also not 100% safe), also I cannot afford the enertion space pack right now if I have to buy all the other parts.
What can I do? This thing is driving me crazy, also I'd like to be able to charge the eskate without having to pay too much attention to the charger...is there any way I could build or buy a BMS?
```

---
## \#2 Posted by: lox897 Posted at: 2016-04-02T23:03:48.175Z Reads: 141

```
There are a ton of 18650 build threads on here. Check them out for some inspiration. I am building a pack with A123 26650 Lithium Iron Phosphate cells soon. I just need to gather some tools and stuff to build it.
```

---
## \#3 Posted by: lox897 Posted at: 2016-04-02T23:04:37.256Z Reads: 142

```
BMS can be bought from Battery Supports. They are supposed to be pretty good quality.
```

---
## \#4 Posted by: JLabs Posted at: 2016-04-03T00:23:12.770Z Reads: 134

```
Check these two links out.. One is a battery template I put together with a parts list an wiring diagrams.. The second is a link to a group buy that just recently finished up and some people will be doing build threads when they can do one.. Here you go
http://www.electric-skateboard.builders/t/18650-group-buy/2015/156

http://www.electric-skateboard.builders/t/custom-18650-battery-pre-build/2014
```

---
## \#5 Posted by: KungFuPanda Posted at: 2016-04-03T10:57:22.829Z Reads: 118

```
Thank you everyone!

So basically I can buy 10 1cell 18650 and connect everything to the 38$ BMS right? That sounds awesome, it's not even that expensive!
```

---
## \#6 Posted by: lox897 Posted at: 2016-04-03T11:00:02.027Z Reads: 110

```
How many volts do you want and how many mah? If you are doing a 10S1P then yes 10 cells is right. If you want more range increase the amount of batteries in parallel.
```

---
## \#7 Posted by: KungFuPanda Posted at: 2016-04-03T11:11:13.510Z Reads: 104

```
It's a 1 motor build, it's better if I do 5000mha ad 12v or 10000mha at 6v? I'm worried that 6v it's not enought but it's a normal skateboard, not a longboard
```

---
## \#8 Posted by: lox897 Posted at: 2016-04-03T21:05:37.496Z Reads: 98

```
You need at least 22.2 volts.
```

---
## \#9 Posted by: KungFuPanda Posted at: 2016-04-03T21:51:22.380Z Reads: 93

```
Oh well, in that case I need to buy a lot of batteries D: I should build like 7-8 packs of 4x2500mah 3.6v right?
```

---
## \#10 Posted by: lox897 Posted at: 2016-04-03T21:56:06.498Z Reads: 106

```
How many volts and mah do you want? I will design a configuration for you. Volts must be at or above 22.2v. What cells will you use? Samsung? LG? Sanyo?
```

---
## \#11 Posted by: KungFuPanda Posted at: 2016-04-03T22:11:32.287Z Reads: 109

```
If I can achive around 10km range with 5000mah it would be enought for me

On my local amazon I can get a good deal on this
Samsung ICR18650-26F Li-Ion 18650 3.7V 2600 mAh

Otherwise I can get the samsung 25r or the lg LG HE4 18650 2500mAh 20A 3.7v
```

---
## \#12 Posted by: lox897 Posted at: 2016-04-03T22:25:56.957Z Reads: 107

```
You could probably get that with 8S but do you want a higher voltage so you can go a bit faster?
```

---
## \#13 Posted by: KungFuPanda Posted at: 2016-04-03T22:41:11.852Z Reads: 110

```
I don't now how fast I can go with 22v, I've seen that the standard speed with 1 motor is 25-30km/h, I won't need go any faster than that...also I'm only 60kg
```

---
## \#14 Posted by: lox897 Posted at: 2016-04-03T23:03:29.811Z Reads: 106

```
The speed also depends on the motor kv. Well, here is an 8s pack design I did for you. If you wanted to go less just take or add on a group of cells.<img src="/uploads/db1493/original/2X/7/7160c42f3d4b09c36ba8215269173caf7cc16225.jpg" width="690" height="487">

You would also put balance leads on the positive, negative and series connections.
```

---
## \#15 Posted by: laurnts Posted at: 2016-04-03T23:14:51.069Z Reads: 91

```
@lox897 I think this design is more like 4s4p in my opinion, as I can only see big groups of 4 batteries connected in series and each of this group of big batteries is 4 cells in the inside. Correct me if I am wrong.
```

---
## \#16 Posted by: lox897 Posted at: 2016-04-03T23:16:30.364Z Reads: 89

```
No. There are two cells that are connected in parallel and then in series. Same happens on the outer area of the cells.
```

---
## \#17 Posted by: lox897 Posted at: 2016-04-03T23:17:37.784Z Reads: 90

```
It's like @whitepony 's design except smaller and not 4p.
```

---
## \#18 Posted by: laurnts Posted at: 2016-04-03T23:18:52.596Z Reads: 92

```
Ohh yes my bad the two cells are connected in series. you're right :smiley:
```

---
## \#19 Posted by: lox897 Posted at: 2016-04-03T23:19:31.724Z Reads: 87

```
I see how you got confused though. It looks a bit confusing.
```

---
## \#20 Posted by: KungFuPanda Posted at: 2016-04-04T22:14:33.021Z Reads: 83

```
Thank you very much :) 

Now I have to decide If I want to spend around 150€ and build that pack or wait a bit and get di space cell...
In the meantime I could buy like 3 of these http://www.hobbyking.com/hobbyking/store/__14076__ZIPPY_Flightmax_1800mAh_9_9V_5C_LiFePo4_TX_Pack.html
and put them in series to get 30v just for trying the esk8
```

---
## \#21 Posted by: lox897 Posted at: 2016-04-04T22:18:53.688Z Reads: 79

```
You can't use those. They've got a 5c discharge rating. That's 9amps discharge, not enough to start your board. Get some lipos.
```

---
## \#22 Posted by: lox897 Posted at: 2016-04-04T22:20:32.040Z Reads: 77

```
Remember, if you are just trying to get stuff for cheap to get your board working, your board will fail. False economy.
```

---
## \#23 Posted by: KungFuPanda Posted at: 2016-04-04T22:37:33.614Z Reads: 79

```
Yeah I know! That's why I'm buying the vesc and other parts on the enertion site, I'd like to avod lipos because there fire friendly but there's no other choice, probably I'll get the zippy 5000mah then if I really like the esk8 i'll get the space cell or I'll make the 8s2p you designed :)
```

---
## \#24 Posted by: lox897 Posted at: 2016-04-04T23:14:29.860Z Reads: 74

```
Good plan. Lipos are fine as long as you know how to take care of them. There are plenty of videos and articles online, I recommend reading a few so you get some knowledge on how to use them correctly and safely. Also, pretty much everyone who has built an esk8 has used lipos. We all know how to use them well.
```

---
## \#25 Posted by: KungFuPanda Posted at: 2016-04-05T22:02:03.008Z Reads: 75

```
Sorry to bother you but I've got an idea!

Is it possible to use just 8 cell in series to get 1 2500mah battery with 8x3.6v? And how can I balance charge everything?

I was thinking to get just 8 cell to test the esk8 and then buy another 8 in the future to put them in parallel and get 5000mah if needed
```

---
## \#26 Posted by: lox897 Posted at: 2016-04-05T22:20:47.104Z Reads: 77

```
In lithium ion? Yes you can. You would use a BMS to balance charge.
```

---
## \#27 Posted by: KungFuPanda Posted at: 2016-04-06T23:05:16.449Z Reads: 79

```
but I've seen this build
http://www.electric-skateboard.builders/t/vanguard-orange-10s-sk3-i-vesc/1337/13
 where this guy doesn't use a BMS, I would like to build something similar so I can use the samsung 25r cells keeping the total cost down
```

---
## \#28 Posted by: lox897 Posted at: 2016-04-06T23:40:49.183Z Reads: 71

```
You could but you will need to buy an 8S compatible charger.
```

---
