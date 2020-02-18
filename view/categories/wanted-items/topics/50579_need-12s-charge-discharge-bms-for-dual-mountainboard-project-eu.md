# Need 12s charge/discharge BMS for dual mountainboard project *EU*

### Replies: 42 Views: 1520

## \#1 Posted by: Nexo Posted at: 2018-03-29T18:09:18.192Z Reads: 150

```
I am looking for BMS that will protect my lipo packs when riding.

in theory one motor can take up to 65 Amps...but this is maximum :slight_smile:
```

---
## \#2 Posted by: Slak Posted at: 2018-03-29T20:36:22.407Z Reads: 142

```
Pretty sure the BMS is for the battery only, not motors. When the ESC asks 10 amp from the battery, it's not directly 10 amp going to the motor. Amps get "processed" by the ESC ;) I'm only a user of VESCs but i guess it's the same for MTB ESCs.

So to scale your BMS, you need to check the discharge values of your battery, it's in its specs. What kind of lipos do you have in your build ? Any link maybe ?
```

---
## \#3 Posted by: Nexo Posted at: 2018-03-29T21:31:29.668Z Reads: 126

```
3x Multistar High Capacity 10000mAh 4S 10C

https://hobbyking.com/en_us/multistar-high-capacity-4s-10000mah-multi-rotor-lipo-pack.html?___store=en_us
```

---
## \#4 Posted by: Geoalex Posted at: 2018-03-29T21:45:11.072Z Reads: 117

```
Not a big enough c rating for mountain board unless your not going up any hills
```

---
## \#5 Posted by: Namasaki Posted at: 2018-03-29T21:50:04.616Z Reads: 114

```
[quote="Geoalex, post:4, topic:50579, full:true"]
Not a big enough c rating for mountain board unless your not going up any hills
[/quote]


Not really enough C rating for a street board either if you want my opinion.
```

---
## \#6 Posted by: Nexo Posted at: 2018-03-29T21:50:53.850Z Reads: 108

```
10Ah x 10C (100A constant) is not enough? o0
```

---
## \#7 Posted by: Namasaki Posted at: 2018-03-29T21:51:37.022Z Reads: 106

```
It's not really 100a, it is overrated.

All Lipos are overrated except these:
https://www.smc-racing.net/index.php?route=product/category&path=67_152
```

---
## \#8 Posted by: Nexo Posted at: 2018-03-29T21:58:00.952Z Reads: 104

```
well...good to know :slight_smile:

I was also thinking about using Li-Ion cells from electric Volkswagen E-Up!
cells are 25Ah 3,7V each :wink:
```

---
## \#9 Posted by: Namasaki Posted at: 2018-03-29T21:59:50.516Z Reads: 102

```
That is an option however, you'll probably need something like a 12s6p for a EMTB.
You need headroom for amp draw.
If you draw 100a from a 100a battery, you are likely to see some heavy voltage sag.

I think that Li-ions are more suited for long range batteries and Lipos are more suited for short range compact high output batteries.
```

---
## \#10 Posted by: Geoalex Posted at: 2018-03-29T22:04:44.022Z Reads: 98

```
10000mah 10a x 10c should give you 100a charge rating but I bet that pack can’t be charged at 100amps either the charge rating gives you more accurate view of its discharge ability
```

---
## \#11 Posted by: Geoalex Posted at: 2018-03-29T22:07:02.862Z Reads: 93

```
Click the spec tab in that battery from Hobbyking 2a charge and 10a discharge rated
```

---
## \#12 Posted by: Geoalex Posted at: 2018-03-29T22:09:47.618Z Reads: 96

```
https://www.maxamps.com/products/gs-life-12400mah-packs

Trusted and nice warranty
```

---
## \#13 Posted by: Nexo Posted at: 2018-04-05T18:20:56.523Z Reads: 89

```
ok guys, but explain me one thing:

below, you can see my configuration of Focbox, you can see, that max Amp usage from battery is 30A (I am going to lower it anyway, too much power in my opinion :wink: )

that means, that this setup is taking 60A tops

...so how is it in real life according to this battery setup?

![focbox|574x307](upload://5Qd5oSp6gJ4OXJGY2hosFpeXoM1.jpg)

Guys? @Namasaki @Geoalex  @Slak
```

---
## \#14 Posted by: DeathCookies Posted at: 2018-04-10T12:36:46.238Z Reads: 85

```
You will draw that max amp only when u accelerate hard or drive uphill. While coasting you dont Need much power and while braking you gain a bit.
```

---
## \#15 Posted by: Acidfie Posted at: 2018-04-10T12:37:02.142Z Reads: 86

```
i am looking for a 12S charging only BMS.. so if someone..
```

---
## \#16 Posted by: Slak Posted at: 2018-04-10T13:18:54.381Z Reads: 86

```
As others mentioned before, the "10C" feature from your lipo are overrated. So let's be nice and say the real discharge rating is 5C, then we have 5C * 10000Ah = 50A. It's, in theory, the maximum amount of Amps you can draw from your battery (and when you do, voltage drops so much, you and your board won't like that).

In your settings, if you set 30A as Batt max on each ESC, it will be 60A total, which is above the 50A we calculated (base on my "5C" assumption, but for "7C", it's 70A which is still not really good). Those lipo batteries you linked before are not good for esk8 or MTB (as Geoalex and Namasaki told you already).
You need to look for lipo adapted for our machine's need (25C to 35C for Lipo is good IMO, but it's still overrated ;) ). Problem is not that the MTB won't work at all, it's just that it will be in bad situation on hills, maybe on violent starts, etc...and on the long run, safety of the hardware or yourself can't be guaranteed (if you push your hardware too much, it will rebelled against you one day. Be cool with it.)
```

---
## \#17 Posted by: Acido Posted at: 2018-04-10T13:26:46.392Z Reads: 79

```
like 5ah... its nothing
```

---
## \#18 Posted by: Acido Posted at: 2018-04-10T13:27:24.454Z Reads: 80

```
All lipos are overrated except the pricey ones
```

---
## \#19 Posted by: Slak Posted at: 2018-04-10T13:34:30.997Z Reads: 79

```
Yep I know but I assumed that if OP bought from HobbyKing, he either doesn't have the budget or is not interested in pricey solutions. So I didn't mention it as Namasaki did before already.
```

---
## \#20 Posted by: Nexo Posted at: 2018-04-10T13:46:25.406Z Reads: 77

```
ok guys, I get that, but, at least for now, I ended with 7 Multistar 10Ah 4s batteries. In that case I want to make them useful somehow

So I thought, that it will be good to protect them from overdischarging by using BMS. With a batteries like this it is almost 100% sure that some of cells will sag during riding.
I was going to order 12s 80A Bestech BMS
what do you think?
```

---
## \#21 Posted by: Acido Posted at: 2018-04-10T13:49:55.307Z Reads: 73

```
what are you going to do with 7?
12s3p? you will have one extra cell then
```

---
## \#22 Posted by: Nexo Posted at: 2018-04-10T13:54:39.322Z Reads: 77

```
one on them has puffed 2 cells, but when bulding 12s i will dissasemble it anyway, this is smallest problem

the other option are Volkswagen's E-Up li-ion cells
25Ah 5C (10Cmax)
![liion|375x500](upload://5wZw9TGhvREmqOy4lq3JWdOKZpU.jpg)
```

---
## \#23 Posted by: Geoalex Posted at: 2018-04-10T17:05:16.221Z Reads: 69

```
Interesting how are those vw cells☝🏻
```

---
## \#24 Posted by: Nexo Posted at: 2018-04-10T19:21:07.943Z Reads: 68

```
I found something like this:

Lithium NMC.
nominal voltage 3.6V
weight 700 g
Dimensions:14.7x9x2,5cm
Max Constant discharge 50A
Max peak discharge 100A(15sec)
Max charge current 12A
```

---
## \#25 Posted by: Acido Posted at: 2018-04-10T19:31:13.834Z Reads: 66

```
That seems cool, do you have any?
If so where did you get them?
I might use them for my trampa...
```

---
## \#26 Posted by: Geoalex Posted at: 2018-04-11T01:09:45.087Z Reads: 67

```
Found some I’ll let you know once I test them
Tested at 24Ah from 4.2V to 3V.
150A continuous discharge.
225A peak discharge.
```

---
## \#27 Posted by: Geoalex Posted at: 2018-04-11T01:12:11.702Z Reads: 70

```
Cell size
5 7/8inch (148mm) long.
1 1/16 inch (27mm) wide.
3 9/16 inch (91 mm) tall.
4 7/16 inch (113mm) tall with terminals.
```

---
## \#28 Posted by: Nexo Posted at: 2018-04-11T04:42:04.704Z Reads: 68

```
I will get 12 of those cells on Monday

I will test them and let you know

those are second hand cells from norwegian auction website

total cost for 12 cells is, more-less, 250$
```

---
## \#29 Posted by: Acido Posted at: 2018-04-11T11:22:47.152Z Reads: 66

```
Thats super cheap! Let me know how it goes
```

---
## \#30 Posted by: Geoalex Posted at: 2018-04-11T22:38:18.388Z Reads: 68

```
![image|552x500](upload://b226OzVLQVMjVaTDaa02DcMxazj.jpeg)
Power disconnect or anti spark key any thoughts on it

Got 12 for Monday delivered 😂
```

---
## \#31 Posted by: Nexo Posted at: 2018-04-12T15:22:02.525Z Reads: 65

```
i have something like this on my boat :smiley:
it can handle up to 150A as far as I can remember
```

---
## \#32 Posted by: mmaner Posted at: 2018-04-12T15:23:29.867Z Reads: 62

```
they are massive and it will likely vibrate loose.
```

---
## \#33 Posted by: Acido Posted at: 2018-04-12T16:03:42.415Z Reads: 60

```
yea those are switches for the lead acid battery...
```

---
## \#34 Posted by: Acido Posted at: 2018-04-12T16:04:10.557Z Reads: 61

```
Nah they stay firm in place, they look ugly AF but should work
```

---
## \#35 Posted by: Nexo Posted at: 2018-04-13T21:33:17.032Z Reads: 62

```
ok guys, but...do you have any final thoughts about BMS for that set?
80A? 100A? how to think about what BLDC tool says? Should I think more about motor max x2 or battery max x2?

2x FOCBOX
2x 6374 3550W @65A each
```

---
## \#36 Posted by: Geoalex Posted at: 2018-04-13T23:07:21.354Z Reads: 58

```
I’m ordering 150a 12s BMS if you want me to order you extra one
```

---
## \#37 Posted by: pat.speed Posted at: 2018-04-13T23:23:58.336Z Reads: 61

```
I think a 100a bms would be sufficient, well unless your @Nowind then you might need a 5000a bms lol
```

---
## \#38 Posted by: Nowind Posted at: 2018-04-14T10:10:40.910Z Reads: 58

```
Hehe yeah well we will see what we can do with the A200S .......:grimacing:
```

---
## \#39 Posted by: Nexo Posted at: 2018-04-17T16:33:44.559Z Reads: 52

```
update:

battery is at home already :wink:

it is a serious brick, but 12s 25Ah is worth it :smiley:  

I paid for it 257$ shipped free by a kind man :smiley:

![30739623_1571072239606820_5213870201744916480_n|690x388](upload://kXQVY60JF83YSls7DDM1RVEaUfB.jpg)

I will try to load it, then unload it to check how are they doing, they came loaded to 3,7V so everything seems to be normal, originally setup was 6s2p but I will change it to 12s1p, I dont need 50Ah :stuck_out_tongue:

BTW: 12s BMS still needed! :open_mouth:
```

---
## \#40 Posted by: Geoalex Posted at: 2018-05-04T04:00:04.662Z Reads: 44

```
Get BMS yet?
```

---
## \#41 Posted by: Geoalex Posted at: 2018-05-06T04:32:09.770Z Reads: 41

```
![image|375x500](upload://xRYKY8CCsLnQdFRo0ZAprdPXpNZ.jpeg)![image|666x500](upload://dvPanHkk6gZVK3pbAmO95wz1Bq4.jpeg)
```

---
## \#42 Posted by: Acidfie Posted at: 2018-09-20T21:06:24.839Z Reads: 25

```
who needs 150 Amps, wtf.. are you building a car?
```

---
