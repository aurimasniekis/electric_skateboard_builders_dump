# Bestech D190 BMS doesn´t charge to full 4.20V per Cell

### Replies: 25 Views: 285

## \#1 Posted by: noi Posted at: 2019-06-17T19:48:35.776Z Reads: 85

```
I just received the Bestech D190 BMS and connected it. It stops charging at 40.8V (10S). Normally it should charge to 42V (4.2V per cell). Have you experienced something similar? what could be the problem? Is the BMS faulty?
```

---
## \#2 Posted by: MannyM0E Posted at: 2019-06-17T22:40:37.302Z Reads: 73

```
Does your charger turn green or is it still red when charging ?
```

---
## \#3 Posted by: noi Posted at: 2019-06-18T07:13:03.702Z Reads: 66

```
It turns green. I left it on for another hour, but nothing changed on voltage. My cells are charged to 90% only and are not balanced. Not sure what's going on. With the old BMS the charger could charge it to 100%. It´s a 4A 42V charger. I think the problem is the BMS.
4.08
4.09
4.06
4.09
4.08
4.09
4.06
4.09
4.07
4.10
```

---
## \#4 Posted by: Namasaki Posted at: 2019-06-18T11:33:08.104Z Reads: 59

```
The problem is more likely the charger especially if it’s a cheap brick charger.
I have had similar issues using cheap brick chargers. 
Now I use a Labratory power supply and have no problem getting full charge.

Check the output of your charger under full load. If it’s less than 42v, it will not fully charge the battery. 

Also if your cells are too out of balance, this can hinder the operation. 
But from the numbers you posted, I don’t think that’s the problem.
```

---
## \#5 Posted by: noi Posted at: 2019-06-19T08:49:25.802Z Reads: 45

```
Thanks for the reply. I use this charger https://de.aliexpress.com/item/32887667488.html?spm=a2g0s.9042311.0.0.3c804c4dbHqO8l. I also charged the cells with my hobby charger, which balanced them perfect to 4.19 / 4.20V. After this I connected the BMS again and the BMS got very hot, I think it tried to discharge the cells, because it thought the voltage is to high. Then I was riding with the board and tried again to charge it with the BMS and it charged to 41.5V, what's good enough, but still disappointing. I was riding again and put it on the charger with the BMS and it stopped again at 40.8V. I disconnected it and plugged the charger in again after 30 minutes and it charged to 41.3V. The cells voltage are now:
4.14
4.14
4.12
4.15
4.14
4.14
4.12
4.14
4.13
4.15
It doesn´t look well balanced to me. Not sure what's going on here. I´m very disappointed, I thought I´m buying a good BMS, but it looks like it´s not working as it should. Maybe something is wrong on my setup, but I can´t figure out what. The BMS should charge to 4.20V and balance the cells to 4.20V. I left the charger connected for hours, but nothing changed on voltage.
```

---
## \#6 Posted by: Namasaki Posted at: 2019-06-19T15:02:58.718Z Reads: 33

```
That looks like a quality charger.  
What bms are you using and what are the specs?
```

---
## \#7 Posted by: noi Posted at: 2019-06-19T15:25:31.616Z Reads: 35

```
The Bestech D190 https://litechpower.com/product-detail/HCX-D190LI10S10A-06.html. It should load to and balance to 4.20V. Same thing today, it charged to 40.9V and after I waited a while and connected the charger again, it charged to 41.4V. Could the cables have an influence on the charging voltage? I can´t explain, why the BMS cuts the charging so early. Maybe a fault on the BMS.
```

---
## \#8 Posted by: thisguyhere Posted at: 2019-06-19T15:30:12.189Z Reads: 37

```
take voltage readings of each cell.  i bet one's out of balance.  i noticed when variance is greather 0.1v it never kicks into balance charge.

https://medium.com/@esk8life.orders/checking-and-correcting-voltage-drift-in-a-battery-pack-616e139d2e3b
```

---
## \#9 Posted by: noi Posted at: 2019-06-19T16:07:00.636Z Reads: 35

```
The cells are very close, it´s not perfect balanced, I would expect more from the BMS, but it´s also not to bad. I don´t think the BMS cut off the charging because of a bad cell. I measured to your instruction: 0.25 4.14 8.26 12.37 16.45 20.7 24.8 28.9 33.0 37.1 41.3 Why is the first one 0.25V and not 0? Are my cables so bad? I also measured directly on the battery pack as well: 4.14 4.12 4.14 4.11 4.13 4.13 4.14 4.11 4.13 4.13 so the lowest is 4.11 and the highest 4.14, do you think this is a problem for the BMS? I also balanced the cells perfectly with the hobby charger before and still the BMS had problems.
```

---
## \#10 Posted by: noi Posted at: 2019-06-19T16:16:32.530Z Reads: 31

```
Did I wire the BMS correctly? B- goes to the minus on the first pack and then B1 and B2 to the middle and plus balance cable and then B3 and B4 to the middle and the plus balance cable on the next pack and so on. B10 is then on the last plus of the last pack.
```

---
## \#11 Posted by: thisguyhere Posted at: 2019-06-19T16:36:48.710Z Reads: 30

```
[quote="noi, post:9, topic:96814"]
I also measured directly on the battery pack as well: 4.14 4.12 4.14 4.11 4.13 4.13 4.14 4.11 4.13 4.13 so the lowest is 4.11 and the highest 4.14
[/quote]

looks like it's balanced, so cells are good.

[quote="noi, post:10, topic:96814"]
Did I wire the BMS correctly?
[/quote]

it depends on the bms, wiring schematic would help here.

one test to ensure charger is working is bypass bms and connect charger directly to battery + and -.

also, a long shot, but your bms' release voltage may be set to below 42v - unlikely.  again, spec sheet and schematic would help.
```

---
## \#12 Posted by: noi Posted at: 2019-06-19T17:10:50.456Z Reads: 28

```
BMS cut off Voltage is 42V and balancing something between 4.18 and 4.2 according to spec sheet.
```

---
## \#13 Posted by: noi Posted at: 2019-06-19T17:11:16.164Z Reads: 31

```
![IMG_5894|500x500](upload://33KTPSI7xsA5fYJdZQPM7pPSCrd.jpeg)
```

---
## \#14 Posted by: Namasaki Posted at: 2019-06-19T17:17:31.778Z Reads: 31

```
[quote="noi, post:12, topic:96814, full:true"]
BMS cut off Voltage is 42V and balancing something between 4.18 and 4.2 according to spec sheet.
[/quote]
Mine is set at 4.28 which is acceptable and allows the pack to fully charge.

![image|364x500](upload://gAkxsTD4Cf5Joha4f4ZlaVAzjTt.jpeg)
```

---
## \#15 Posted by: noi Posted at: 2019-06-19T17:18:38.748Z Reads: 31

```
Charger is charging, if directly connected to the pack and stops charging if connected with the BMS, so the charger is alright, the BMS cuts the voltage.
```

---
## \#16 Posted by: noi Posted at: 2019-06-19T17:27:03.007Z Reads: 31

```
I have seen these ones as well, but I thought it will damage my Lipo with the cut off at 4.28V. If I would have known that it cuts off earlier then it says in the specs, I would have chosen a BMS with 4.28V as well. When does it cut off exactly? Does it charges to 42.8V and then balance it back to 42V or does it just stops way earlier like mine? Maybe I return the BMS and get one with 4.28V cut off. Just strange that mine says 4.20V cut off, but it cuts off way earlier and not a single cell reached the 4.20V (4.14V the highest). Many people in this forum use the Bestech D190, wondering if more people discovered the same with this BMS or if I still have a fault somewhere on my installation. Very disappointing, though I´m getting a quality BMS and just have problems, very annoying. Thanks for trying to figure out the problem.
```

---
## \#17 Posted by: Namasaki Posted at: 2019-06-19T19:10:06.596Z Reads: 26

```
The 4.28 was Bestech’s default setting. 
You have to request if you want it lower. 
The battery’s voltage will not exceed the charger’s output voltage regardless of the bms. 
I have more to say but must return to work. 
I will edit later.
```

---
## \#18 Posted by: legend27 Posted at: 2019-06-19T19:17:22.197Z Reads: 26

```
[quote="noi, post:9, topic:96814"]
0.25 4.14 8.26 12.37 16.45 20.7 24.8 28.9 33.0 37.1 41.3
[/quote]

Might just be me, but why do you have 11 readings? Shouldn't you only be able to have 10 readings. The first reading should be 4,14, right?

Just my few cents... Might be completely wrong...
```

---
## \#19 Posted by: Silverline Posted at: 2019-06-19T19:35:02.072Z Reads: 23

```
My D190 does the same....stops before hitting 4,2v pr cell. My old fullsize bestech BMS (80a load) did charge the very same pack with same Charger to perfect 4.20v pr cell. I dont know if its a D190 thing ? 

When hitting about the 4,12v pr cell, the BMS starts to trigger the charger, so it constantly goes on off on off etc.
```

---
## \#20 Posted by: noi Posted at: 2019-06-20T08:23:53.705Z Reads: 21

```
Makes sense. I should have got a 4.28V Bestech. The D190 is set to 4.20V.
```

---
## \#21 Posted by: noi Posted at: 2019-06-20T08:26:04.215Z Reads: 21

```
I measured it to @thisguyhere instruction. The first value should be 0 or very close to 0, not sure if 0.25V is to high. If I understand it right, it´s just the voltage drop on the cable, I should check it, it seems a bit high.
```

---
## \#22 Posted by: noi Posted at: 2019-06-20T08:27:58.350Z Reads: 21

```
Good to hear this. It looks like that the Bestech BMS needs a 4.28V or 4.25V cut off voltage to get it charged exactly to 4.20V. If the cut off is at 4.20V the BMS will cut off to early.
```

---
## \#23 Posted by: Silverline Posted at: 2019-06-20T09:48:50.943Z Reads: 21

```
I use the same charger as you. I will try play with the voltage output then.
```

---
## \#24 Posted by: noi Posted at: 2019-06-20T10:01:35.802Z Reads: 21

```
The charger is not the problem, if I connect it directly it is charging and will reach the 42V. The problem is the D190 BMS which cuts off to early, sometimes even under 41V and never reaches the 4.20V or close to it. The spec says cut off at 4.20V, but this is not happening. I will try a BMS with 4.28V cut off like the D140 and this should charge the cells to 4.20V.
```

---
## \#25 Posted by: Namasaki Posted at: 2019-06-20T15:12:07.358Z Reads: 18

```
[quote="noi, post:20, topic:96814, full:true"]
Makes sense. I should have got a 4.28V Bestech. The D190 is set to 4.20V.
[/quote]

When you order directly from Bestech, you can specify certain parameters. 
If you buy from a 3rd party, your stuck with the parameters that they choose.

This is true regardless of which model you get
```

---
