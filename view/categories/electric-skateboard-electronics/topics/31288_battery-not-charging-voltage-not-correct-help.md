# Battery not charging, voltage not correct. Help!

### Replies: 18 Views: 1136

## \#1 Posted by: Yecrtz Posted at: 2017-08-22T22:03:24.307Z Reads: 116

```
Gents, I am having a problem with my board. When I plug in my charger, it doesn't even starts to charge and tells me the board if full (green led + no fan going on). When checking the voltage, the VESC is receiving a nice 41.7 volts.

But! When I remove the charger, the voltage the VESC receives drops to 39 again. Something is going wrong here. The cells are all charged to 3.9 volts (checked them one by one).

The setup is 10s with a SuPower BMS, worked perfectly fine for two weeks... until now. Do you know what could be the problem?

@Namasaki, any idea? You have a lot of battery knowledge and expertise..
```

---
## \#2 Posted by: Namasaki Posted at: 2017-08-22T22:09:18.192Z Reads: 111

```
I would try another charger.
```

---
## \#3 Posted by: Jinra Posted at: 2017-08-22T22:09:49.019Z Reads: 112

```
Sounds more like a BMS issue to me. Could you take a photo on how everything's hooked up.
```

---
## \#4 Posted by: Yecrtz Posted at: 2017-08-22T22:15:34.873Z Reads: 113

```
Here is a picture. I did around 25± charges with it without problems. Just removed the BMS from the board for a closer inspection. But no visual damages there as far as I can see.

2x 5s in series, connected through the bms to the antispark switch and charge port.

<img src="/uploads/db1493/original/3X/a/6/a656a542f448cc178b970fe7b3f70df410976081.jpg" width="666" height="500">

I only have one charge brick and one IMAX b6 charger, can I in some way hack that thing to get it to output 42 volts?
```

---
## \#5 Posted by: Jinra Posted at: 2017-08-22T22:21:12.310Z Reads: 107

```
can you probe the charger to see what output voltage you're getting from it? Also, to clarify, you probed each of the orange balance leads to confirm each cell is 3.9v?
```

---
## \#6 Posted by: Yecrtz Posted at: 2017-08-22T22:28:04.649Z Reads: 104

```
Thanks for the quick replies! Correct, I checked the 10s balance connector that goes in to the bms and the voltage nicely counts up. The output of the charge brick is 42 volts without anything connected. But it has CC, CU & Float built in so I'm not completely sure how it regulates its volts/amps when connected.
```

---
## \#7 Posted by: sl33py Posted at: 2017-08-22T22:55:19.286Z Reads: 98

```
I would remove the BMS - charge each 5s pack individually on your iMax and look for a cell w/ issue.  Run resistance test again to look for problems.  If everything checks out OK - then i'd dig into the BMS or replace.

Process of elimination and i'd simplify first.  Double check everything - especially any wires you soldered - check resistance if in doubt, etc.  i'd first confirm the batteries are good before digging too deep into individual wires and BMS.

(Especially given your change is ~3v - about one cell.  Very suspicious of your cells or one bad would be my guess)

GL!
```

---
## \#8 Posted by: Namasaki Posted at: 2017-08-23T02:35:17.888Z Reads: 92

```
I like @sl33py idea of disconnecting the bms and charging the packs with your hobby charger.
If they charge properly with the hobby charger, then reconnect the bms and go ride.
Then if you experience the same under charge issue on the next charge with the bms and brick charger, I would try another brick charger.  From your description, it sounds like the output of your brick charger is low during charging.
Cells being too far out of balance can cause undercharge issues but you said your cell are balanced at 3.9v
2a brick chargers are only about $12 on eBay.
```

---
## \#9 Posted by: Yecrtz Posted at: 2017-09-04T21:47:16.976Z Reads: 69

```
I charged the batteries normally a couple times with the B6 but no problems occured. Just got another charge brick in the mail and I'm experiencing the exact same problems. 38V right now, plug the charger in > voltage goes to 41.7 and charger does nothing. Disconnect charger > voltage drops back to 38V...

Contacting SuPower...
```

---
## \#10 Posted by: Yecrtz Posted at: 2017-09-06T11:24:25.572Z Reads: 61

```
Measuring from the first pins all the way to the end of the balance plug that goes into the BMS:

3,90 V
7,78 V (+ 3,88)
11,67 V (+ 3,89)
15,61 V (+ 3,94)
19,52 V (+ 3,91)
23,45 V (+ 3,93)
27,36 V (+ 3,91)
31,28 V (+ 3,92)
35,20 V (+ 3,92)

Does anybody know what could be wrong?
```

---
## \#11 Posted by: pat.speed Posted at: 2017-09-06T11:39:29.404Z Reads: 59

```
Maybe cells are stuffed? I know that my lipos (2x 3s) will only charge up to about 4 to 4.1v with my hobby charger. This could be the same issue
```

---
## \#12 Posted by: Yecrtz Posted at: 2017-09-06T11:41:59.801Z Reads: 56

```
Lipo's are perfectly fine. Can charge them to 42 with my hobby balance charger without problems. But when I try to charge them through my BMS the voltage is always 42 when I have the charger connected, and it won't charge. The moment I disconnect the charger the voltage drops immediately down to the original amount.
```

---
## \#13 Posted by: TarzanHBK Posted at: 2017-09-06T11:42:40.976Z Reads: 54

```
so your BMS seems broken
```

---
## \#14 Posted by: pat.speed Posted at: 2017-09-06T11:43:17.403Z Reads: 55

```
Oh yes forgot you said they work with the hobby charger. Must be the bms then
```

---
## \#15 Posted by: Yecrtz Posted at: 2017-09-06T11:47:33.224Z Reads: 55

```
Thanks, SuPower is giving me a hard time asking me four times in a row to check the voltages.. :sweat:
```

---
## \#16 Posted by: Yecrtz Posted at: 2017-09-08T23:14:42.005Z Reads: 51

```
They suggested it may had something to do with the 'big' difference in cell voltages. So I balanced all 10 to 4.00 volts but the problem is still here. Am I missing something? The bms must be broken right? I'm out of ideas.
```

---
## \#17 Posted by: capfirepants Posted at: 2017-09-22T08:52:10.932Z Reads: 49

```
@Yecrtz  Did you get this resolved?
```

---
## \#18 Posted by: Martinsp Posted at: 2017-09-22T10:26:52.514Z Reads: 43

```
Well if I understand you correctly you have voltage on the output of the charger and when you plug it in the bms the voltage is at 42 and when you unplug it it drops back down to voltage of the batteries. That sounds correct to me. Charging is nothing else than voltage from the batteries is "trying" to be the same as the voltage of the charger and it draws current to get there. Measure the current that flows to your battery when you have your charger connected. Maybe it is just very slow. 

Hope I understand you and the description of your problem.
```

---
