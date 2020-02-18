# Apollo Longboard / 8s Lipo / BMS / SK3 6364 245KV / ENERTION wheels and motor mount / VESC

### Replies: 6 Views: 2429

## \#1 Posted by: gaetjen Posted at: 2016-08-18T12:02:20.748Z Reads: 398

```
So, after a couple of months researching and ordering stuff from all over the world, I finally finished my first electric longboard. It has been finished for a couple of weeks now and I tested it a lot and changed stuff or tried to improve some things. These are the parts I used:
Enertion motor mount
Enertion wheel pulley
Enertion motor pulley
Enertion wheels
Two ZIPPY Flightmax 8000mAh 4S1P 30C connected in series
Apollo longboard of Amazon
VESC from esk8.de
Turnigy Aerodrive SK3 - 6364-245kv Brushless Outrunner
100A BMS and 5A charger from Supower of Ebay
XT90 Anti-Spark
1s-8s Lipo low voltage buzzer
Lipo safety bag
FS-GT2B  transmitter and receiver
Bullet Connectors and cables
wooden strip and steel sheet for the casing

To match the motor mount onto the trucks I had to file them down to give it a angular shape. To make sure that the motor mount doesn’t move I used pieces of a garden water hose. That worked in the beginning. But until now, I still had to improve the motor mount setup because I didn’t file the truck down
symmetrically. I also had to file the motor shaft so the motor pulley would fit with the keyway. To connect the batteries, connect it with the bms and the lipo buzzer, I used a luster terminal. After soldering the BMS, a Anti-Spark-Loopkey, the charging terminal and the Vesc I started the Motor detection on the vesc and it worked. But, I didn’t get the GT2B to work. So, I asked around and finally figured that I made mistake by connecting the ports in the wrong order. It finally worked. 

Other Problems that occurred during the first couple of weeks riding:

- Make sure your belt is tight and that you don’t break too hard.

- At the beginning I had some overheating issues either with the motor or the VESC. After a longer ride my break released when I wanted to fully stop the board and after a couple of seconds the VESC seemed to restart and I was able to break again. I fixed it by making sure that enough air comes to the vesc and
changed some settings in the vesc. Lowered the regen breaking min for example.

- The individual cells of my 8s Lipo kept drifting apart to the point where
cell one was at 3.8 V and cell four was at 4.2V. It was only after some mails
between supower from ebay and myself that I found out that the BMS only works when
I fully charge the battery, which I didn’t do at the beginning. Here is what
supower wrote:

“_the charger will not stop until battery_pack fully charge to 33.6V._If the charger stop charging it, because the BMS protected, some battery are_full at 4.2V (shorter capacity), but some still need to continue charge, the_BMS will keep balancing but if cell capacity with much difference and BMS shut off when fail to balance the battery cell._The BMS start balance on 4.16V with trickle current 45mA until battery full at _4.2V, so as the charger, the charger finally charge with trickle current to make battery full_”

Therefore, I had to buy a charger which is able to balance my batteries now. The problem is that chargers above 6s are really expensive. I bought the junsi icharger 1010B+, which is still expensive but one of the cheaper ones in comparison to some others.  I still charge the pack with my 5A charger, but sometimes the cells drift and I have to balance them again with the icharger, which is kind of annoying. But besides that, the board is a hell lot of fun and everybody looks jealously at you when you pass them. For my next
board I’m going to use Li-ion LG HG2 cells because I don’t want any drifting.
Thanks to the community here for the help and reading material to give answers
to almost all my problems.

<img src="/uploads/db1493/original/2X/e/ee301f3463a478a0c4a788c42600317238c0c5f4.JPG" width="690" height="375">
<img src="/uploads/db1493/original/2X/a/ac5b68e281ed4f104979d5080a73941a75613e97.JPG" width="311" height="500">
<img src="/uploads/db1493/original/2X/d/d9c76dad8c7b1091ca02fc86bdc5cc94811dd0ef.JPG" width="690" height="145">
<img src="/uploads/db1493/original/2X/6/666b467ec1dfb90f928dfac60bed40fb2f4cbfd6.JPG" width="690" height="388">
<img src="/uploads/db1493/original/2X/f/f81d0b429c32fed2cdefb2580b2d3fc6b8c08982.JPG" width="690" height="388">
<img src="/uploads/db1493/original/2X/f/fdf1fa19b34fc852a4d01b6046650e9bf7f87a27.JPG" width="281" height="500">
```

---
## \#2 Posted by: freddyalcazar Posted at: 2016-08-18T12:34:34.749Z Reads: 342

```
Great built man! hope my first goes as well 😅😅😅
```

---
## \#3 Posted by: s00cl0se Posted at: 2017-06-26T16:34:06.718Z Reads: 148

```
HI , I am building a electric skateboard and in the process of ordering the same motor you have. However I saw its picture in the website and don't know how to connect the pulley to the motor firmly. Can you let me know how you did it, thanks
```

---
## \#4 Posted by: gaetjen Posted at: 2017-06-27T18:20:12.705Z Reads: 132

```
Yeah, you have to file down the motor shaft to give it an angular shape and then use the keyway and some loctite to make sure its tight.
```

---
## \#5 Posted by: TunaTee Posted at: 2017-09-24T03:05:52.755Z Reads: 89

```
Hey, 
I am wondering how you connect LED to the board.
Those LEDs are LIT!
```

---
## \#6 Posted by: gaetjen Posted at: 2017-09-24T12:53:58.159Z Reads: 77

```
https://de.aliexpress.com/item/DC-DC-Converter-Adjustable-Power-Supply-DC-DC-Step-Down-3A-LM2596HVS-LM2596HV-DC-Step-Down/32485142548.html?spm=a2g0s.9042311.0.0.rd8Ywa
Use one of these. Connect it to the battery and convert it down 5 v and then hock it up to the led strip
```

---
