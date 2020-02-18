# Do I need dual anti-spark switches? 100a load

### Replies: 19 Views: 391

## \#1 Posted by: D_Sk8 Posted at: 2018-08-29T03:11:16.727Z Reads: 138

```
I am building a dual Torque Board 6355 with a 12s2p A123 battery that can handle 140a. My intention, though, is to max 50a per VESC = 100a total continuous capable. (maybe 45a x 2 to not stress the VESC's out too much).

If you search online for copper wire ampacity (given, all of the sources I find are for electrical wiring which are longer runs) suggest 12 awg ampacity is only 20a. I think the gauge wire on the anti-spark switch I have from DIY is 12awg (maybe 10awg, but even then I read that 10 awg is only rated to 30a).

I also have Flipsky's anti-spark boards and can build my own switch with 8awg wire, but again, I read 8awg is limited to 40-50a. I need double that.

Do I need to run 2 anti-spark switches? 10/12awg doesn't seem like enough for 100A load.
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-08-29T03:13:19.575Z Reads: 132

```
I doubt that you will draw anywhere near 100a.
```

---
## \#3 Posted by: D_Sk8 Posted at: 2018-08-29T03:29:59.547Z Reads: 130

```
It's my understanding the VESC monitoring application reports the battery and motor current (as well as other stuff). but it's only reporting the load of a single motor. If that't the case, the below video suggests he peaked at 57a per motor. I'm shooting for the same. Or does the VESC app report the current of both motors combined?

![image|690x388](upload://bejRbZprC4eKdL4mCVuMmItER23.jpg)

https://www.youtube.com/watch?v=Bg_7t1sLwhY&t=96s
```

---
## \#4 Posted by: Namasaki Posted at: 2018-08-29T04:05:48.540Z Reads: 115

```
[quote="D_Sk8, post:1, topic:66444"]
If you search online for copper wire ampacity (given, all of the sources I find are for electrical wiring which are longer runs) suggest 12 awg ampacity is only 20a. I think the gauge wire on the anti-spark switch I have from DIY is 12awg (maybe 10awg, but even then I read that 10 awg is only rated to 30a).
[/quote]


You should be using Silicone wire which has much higher current and heat ratings.
Here is a chart for silicone wire
![11%20AM|295x223](upload://2N7M7ZvrubWUCww2e488Sm6gAQe.png)
```

---
## \#5 Posted by: D_Sk8 Posted at: 2018-08-29T04:10:34.183Z Reads: 106

```
Ohh damn, ok. Well, that's the answer to my question then. Thank you. I can work with that. I'll make certain to use 10awg.
```

---
## \#6 Posted by: Namasaki Posted at: 2018-08-29T04:20:03.234Z Reads: 96

```
Silicone 10awg is rated for up to 200F
The insulation is silicone rubber. It is thick yet very flexible.
```

---
## \#7 Posted by: D_Sk8 Posted at: 2018-08-29T04:21:24.635Z Reads: 92

```
I have a ton of 10awg, and even some 8awg, but I know the 8awg is nearly impossible get onto a XT90. Knowing that I can use 10awg is great news.
```

---
## \#8 Posted by: Namasaki Posted at: 2018-08-29T04:22:13.068Z Reads: 91

```
I use 12awg on my builds and never had a problem running dual drives.

But thicker wire is always better because it reduces resistance

You can't go wrong using 10awg Silicone wire

10awg fits perfectly in 5.5mm bullet connectors which I personally prefer over XT connectors.
```

---
## \#9 Posted by: D_Sk8 Posted at: 2018-08-29T04:25:51.958Z Reads: 90

```
Ok, awesome. I really want to push the ESC's to a safe max. I'm 235lbs and there are times i'll be riding in S.F, so I want to get the most out of the board.
```

---
## \#10 Posted by: Namasaki Posted at: 2018-08-29T04:28:32.228Z Reads: 90

```
I would stick with normal size skate wheels like 83mm to 90mm
And gear 36/15 with 83's or 40/15 with 90's

And you will definitely need a dual drive especially if your going up hills.

Dual anti-spark switches, Never thought of doing that. Not sure it will work without causing some side effects or if it will be any advantage over a single switch.
Anti-spark switches have also had a long standing reputation for being unreliable. 
I don't know if there are any available now that have overcome that.
```

---
## \#11 Posted by: Aeroquiv Posted at: 2018-08-29T04:38:49.711Z Reads: 82

```
Ackmaniac's app has the ability to report both vescs, so what you see on @SeanHacker's video is definitely from both vescs.
```

---
## \#12 Posted by: Aeroquiv Posted at: 2018-08-29T04:44:26.406Z Reads: 78

```
At 175lb in the city, I use 40-50A up hills at 15-20 mph. 90mm wheels, 16/36 gearing, and 200kV motors.
```

---
## \#13 Posted by: D_Sk8 Posted at: 2018-08-29T04:55:25.488Z Reads: 77

```
[quote="Namasaki, post:10, topic:66444"]
Dual anti-spark switches, Never thought of doing that.
[/quote]

Yeah, I am not 100% certain whether you can combine two into a single on/off switch, but that'd be nice. I have a feeling that might be a bad idea.
```

---
## \#14 Posted by: D_Sk8 Posted at: 2018-08-29T04:56:09.933Z Reads: 76

```
[quote="Aeroquiv, post:11, topic:66444"]
so what you see on @SeanHacker’s video is definitely from both vescs.
[/quote]

So, that's a combination of both motors, i.e. a total amount of battery current and not just 50%?
```

---
## \#15 Posted by: Aeroquiv Posted at: 2018-08-29T04:56:42.961Z Reads: 73

```
Most likely.
```

---
## \#16 Posted by: D_Sk8 Posted at: 2018-08-29T04:58:03.188Z Reads: 71

```
I assume your 40a/50a is a total amount and not per motor too right? 

I know the motors I have are rated up to 2500 watt, so I wanted to get as close to that as possible. I figure 1800 watt minimum per motor would be a goal.
```

---
## \#17 Posted by: Aeroquiv Posted at: 2018-08-29T04:58:45.508Z Reads: 71

```
yes 40/50A total battery current. Max motors was 50A each, but that was only at low speed acceleration and not actual hill climbing.
```

---
## \#18 Posted by: Chase Posted at: 2018-08-29T21:11:07.732Z Reads: 45

```
5 mosfet switch rates for 100A continuous 

https://www.electric-skateboard.builders/t/vedder-anti-spark-switches-for-sale-from-18/

Push to start switch rated at 100A continuos

http://electricskateboard.repair/index.php?id_product=41&controller=product
```

---
## \#19 Posted by: D_Sk8 Posted at: 2018-08-29T22:14:20.678Z Reads: 31

```
Nice, thank you. I just took a look at the mosfets on the Flipsky board and they are IRFS7730PBF boards, vs the IRFS7530TRL7PP on that board. They seem to be rated similar. But the other one looks pretty amazing. Auto-Off seems like a great idea. Thank you!
```

---
