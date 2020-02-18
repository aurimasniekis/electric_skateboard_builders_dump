# 3S lipo with different volts per cell. Example: (4.11 3.92 3.93)

### Replies: 20 Views: 1148

## \#1 Posted by: xBRAZILx Posted at: 2018-01-22T01:06:38.966Z Reads: 91

```
Hello guys, a short question:

One of my my two 3S 5000mah lipo battery has been a little strange for a while. 

I don´t know why 1 cell is up to 0.10V higher than the others 2 cells. I´ve be running with this battery more than 2 months and suddenly this started to happen .
![IMG_20180121_223149100|375x500](upload://zLA7fQH8jSaulaJ2rvIMy7A5jWL.jpg)

i´m using IMAX b6 original;
i charge it with 3.0A in Lipo Balance mode
my battery cut off is set to 3,7 per cell on the VESC

my two question are:
1)Is this normal to happen?
2)If isn´t normal, this could be a problem?
3)And if is a problem, can be fix?

thanks
```

---
## \#2 Posted by: wmj259 Posted at: 2018-01-22T01:13:14.600Z Reads: 86

```
[quote="xBRAZILx, post:1, topic:44313"]
little
[/quote]

That's not 0.1 above, that's ~0.2. 
You need to balance that asap. The IMAX-B6 should have a balance feature. Once balanced,recheck. If the lipo doesn't stay balanced out, I would discard it.
```

---
## \#3 Posted by: xBRAZILx Posted at: 2018-01-22T01:17:41.608Z Reads: 86

```
i forgot to mention that i always charge in Lipo Balance mode.
i thought it was something with the amps , so i tried  charging with 1.0AMP but i didnt get any sucess, they still UNbalance
```

---
## \#4 Posted by: jmasta Posted at: 2018-01-22T01:20:48.086Z Reads: 81

```
Use your balance charger to check the internal resistance (IR).  They shouldn't be that far off
```

---
## \#5 Posted by: xBRAZILx Posted at: 2018-01-22T01:35:57.796Z Reads: 72

```
i google it about IR and i realized that my imax b6 (is very old) doesn´t have this option...
maybe it is a fake imax?:face_with_raised_eyebrow:

use the discharge function and charge again could be an alternative to bring back the balance between cells?
```

---
## \#6 Posted by: Namasaki Posted at: 2018-01-22T02:22:40.066Z Reads: 67

```
It would help to have more info about your batteries.
Brand?
C rating?
When Lipos get worn, there internal resistance will increase but it's not likely to increase evenly across all cells.
This will cause the cells to charge and discharge unevenly.
If you are using Lipos with a low C rating like 10-25C then the high current demand of esk8 can cause them to age quickly.
Does the pack in question show any signs of swelling?
Is your charger stopping the charge cycle with those voltages 4.11  3.92  3.93 ?
It should continue to charge until all cells reach 4.2v
When cell one reaches 4.2 it will just idle while the other cells catch up. Thats how a balance charger works.
```

---
## \#7 Posted by: xBRAZILx Posted at: 2018-01-22T02:44:12.884Z Reads: 64

```
thanks for your answer

Brand?
**a:HRB ( bought on ali express), this battery has at least 5 years, (not continuos using) and was used just for TRAXXAS RC .**

C rating?
**a:50C discharge/100c burst**

Does the pack in question show any signs of swelling?
**a:Yes, i dont know if you can see in the picture, but the first cell is a little fluffly ( im sorry, i dont know a better word for this) and when it come close to 3.50/3.60 this cell gets totally swelled and very very hot. but i always stop in 3.74/3.75**

Is your charger stopping the charge cycle with those voltages 4.11  3.92  3.93 ?
**a:No, i am able to full charge all cells to 4.20, the only thing is that cell in question stay in 4.19/4.20 till the others gets to 4.20**

It should continue to charge until all cells reach 4.2v.
**a: yes**

the charging situation was perfect until this week. i didnt do anything different that i usually do, didnt change any configuration on the vesc etc etc

![IMG_20180122_002509582|666x500](upload://z1j2Kd4wSVb2pfZJ8lZCMa9Th2A.jpg)
```

---
## \#8 Posted by: Namasaki Posted at: 2018-01-22T02:52:58.023Z Reads: 58

```
Never heard of that brand so I can't comment on their quality.
The pack does look well used and if it got hot enough to melt the shrink wrap, then there could be some deterioration of the cells.
Be really careful about the heat issue. Getting batteries like these hot can cause a dangerous situation.
```

---
## \#9 Posted by: jmasta Posted at: 2018-01-22T02:59:21.162Z Reads: 57

```
[quote="xBRAZILx, post:7, topic:44313"]
Does the pack in question show any signs of swelling?

a:Yes, i dont know if you can see in the picture, but the first cell is a little fluffly ( im sorry, i dont know a better word for this) and when it come close to 3.50/3.60 this cell gets totally swelled and very very hot. but i always stop in 3.74/3.75
[/quote]

Those batteries are beat!  Personally I would replace them
```

---
## \#10 Posted by: xBRAZILx Posted at: 2018-01-22T03:06:29.028Z Reads: 56

```
i´ve never had another battery so i also cant comment about their quality haha
i was buy a turnigy graphene,

so i guess this voltage difference is not a issue ?

and i guess it would be good buy a fire retardant lipo battery bag
```

---
## \#11 Posted by: xBRAZILx Posted at: 2018-01-22T03:09:51.626Z Reads: 53

```
i already have done this... i am still waiting for the new ones... 
i wanted to buy the turnigy graphene, but they dont ship to Brazil, in fact just a few brands ship to here. so the only solution from us is to buy this kinda of chineses brands (nothing against China products)
but you got the point...
```

---
## \#12 Posted by: Namasaki Posted at: 2018-01-22T03:10:17.649Z Reads: 52

```
The voltage difference is not such a big issue but the batteries getting hot is.

You should be able to get batteries from Hobby King's Global warehouse.
```

---
## \#13 Posted by: MannyM0E Posted at: 2018-04-04T19:06:49.883Z Reads: 26

```
Mines are similar to this ? Ones like 4.11 and the others are like 3.98. Should I discharge them to like 3.2 then rebalance charge them ? Running 5s 30c 8000mah
```

---
## \#14 Posted by: xBRAZILx Posted at: 2018-04-04T19:21:13.133Z Reads: 27

```
in this situation i would just balance in a low AMP, something like 0,5 AMP until the cells are all balanced. after this maybe put in storage mode and balance again, something like "reset" the battery. 

below 3.7 you start to "kill" the battery. i never go below 3,75 with mine.
```

---
## \#15 Posted by: Namasaki Posted at: 2018-04-04T20:29:02.501Z Reads: 25

```
Not 3.2v

If your using a hobby charger you can just balance charge them to 4.2v
```

---
## \#16 Posted by: MannyM0E Posted at: 2018-04-04T21:39:57.507Z Reads: 24

```
It won't charge any higher. It stays right there
```

---
## \#17 Posted by: pat.speed Posted at: 2018-04-04T21:45:38.553Z Reads: 23

```
Is it a fake imax B6?
```

---
## \#18 Posted by: MannyM0E Posted at: 2018-04-04T21:46:42.337Z Reads: 23

```
HTRC H120 AC 50W 70W / DC 100W x 2 Dual Ports 10A RC Balance Charger/Discharger for Lilon/LiPo/LiFe/LiHV/NiCd/NiMH Battery https://www.amazon.com/dp/B072JC1P13?ref=yo_pop_ma_swf
```

---
## \#19 Posted by: pat.speed Posted at: 2018-04-04T21:50:56.964Z Reads: 21

```
Hmm I’m not sure, clone imax b6s have this issue. Maybe they are using the same parts
```

---
## \#20 Posted by: MannyM0E Posted at: 2018-04-04T21:53:09.748Z Reads: 21

```
Once I get home planning on discharge all til 3.7 and see if I can balance charge them back. It sucks too because I just got these batteries from HK about a week ago
```

---
