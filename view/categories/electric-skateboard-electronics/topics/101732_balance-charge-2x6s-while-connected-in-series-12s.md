# Balance charge 2x6S while connected in series (12S)

### Replies: 19 Views: 341

## \#1 Posted by: pmouraguedes Posted at: 2019-09-13T17:01:30.242Z Reads: 63

```
Would it be possible to have 2 x 6S battery packs connected in series and have them being balanced charged individually (assuming each 6S has its own dedicated discharge and balance cables)?
Or would I have to undo the series connection before I balance charge them?

I would like to get rid of the BMS, but also be able to balance charge the pack conveniently, without unplugging anything.

Thanks
```

---
## \#2 Posted by: mutantbass Posted at: 2019-09-13T17:06:41.833Z Reads: 62

```
you mean like this?

https://forum./t/pictures-and-nothing-else/79/1396
```

---
## \#3 Posted by: pmouraguedes Posted at: 2019-09-13T17:16:53.532Z Reads: 60

```
Yes, although in this case it seems they are charged via the balance cable, is that so?
```

---
## \#4 Posted by: mutantbass Posted at: 2019-09-13T17:28:18.831Z Reads: 59

```
yes. the bms is in the enclosure with the batteries so you just charge it like a regular board. no need to open anything.
```

---
## \#5 Posted by: mmaner Posted at: 2019-09-13T18:38:32.211Z Reads: 56

```
I think he saying have the main pack leads in series for 12s but a seperate BMS for each lipo. 

I don't think you could as the pack negative, in this case the negative for each lipo, had to be connected to the BMS, which would create a series connection to each BMS via the series connection at the main leads. 

Cool idea though.
```

---
## \#6 Posted by: mutantbass Posted at: 2019-09-13T19:06:00.167Z Reads: 51

```
yeah. he would need a way to " un serial" the lipos before he charges them.
```

---
## \#7 Posted by: anders Posted at: 2019-09-13T20:44:23.101Z Reads: 48

```
Hi, I used to balance charge as 2 x 6s and discharge in 12s with this method https://www.electric-skateboard.builders/t/discharge-12s-and-charging-6s-parallel-need-help/5126?u=anders 


https://www.electric-skateboard.builders/t/remover-of-obstacles-first-build-rayne-amazon-sk3-6374-149kv-12s-graphene/86399/8?u=anders

Very important you have to break series connection before charging, I do it with xt90 anti-spark.

Now I charge in series 12s at 5A with an external bms connected to the balance wires, also using a portable charger.

https://www.electric-skateboard.builders/t/range-extender-plugged-into-charge-port/64327/140?u=anders
```

---
## \#8 Posted by: pmouraguedes Posted at: 2019-09-15T16:24:36.010Z Reads: 32

```
Hi anders, the scheme included in the post you linked is exactly what I was trying to describe.
So, one has to break the series connection, I see. 
Still don't understand exactly how to make the series connection and how to enable and disable it. Could you shed some light on it?

Thanks!
```

---
## \#9 Posted by: pmouraguedes Posted at: 2019-09-15T17:58:59.495Z Reads: 29

```
Ok so, instead of connecting the + and - as usual for connecting in series, one makes an xt90 connector out of both wires. To connect it in series just insert an xt90 loop connector, to undo just remove the loop.
Alternatively, one can a TB anti-spark switch, is that it?
```

---
## \#10 Posted by: anders Posted at: 2019-09-15T19:50:31.658Z Reads: 28

```
Yes, as you can see on the scheme connect + and minus with  either an xt90 antispark or an as150, when the antispark is connected it will connect both batteries in series to the esc, when you pull out the loopkey it will break the series connection and the power to the esc. From what I read about antispark switches is that they fail or consume power even after being switched off.

  ![image|479x500](upload://8Nka3swYKihfLpxYLN3SzcO4PbO.jpg) 

Which charger, batteries, esc are you going to use for charging?
```

---
## \#11 Posted by: pmouraguedes Posted at: 2019-09-15T22:48:23.339Z Reads: 28

```
This is brilliant, thanks. I think Trampa beast box use something like this too.
<br><br>
I will probably build two 6S3P flat packs from 21700 45A Molicel cells and balance charge them with two IMAX B6 chargers, no BMS. 
<br><br>
Regarding ESC, some >=120A one, probably VESC or some derivative, still don't know. Suggestions welcome.
<br>
```

---
## \#12 Posted by: anders Posted at: 2019-09-15T23:57:34.051Z Reads: 27

```
Imax B6 comes in 50W 2.4A at 6s or 80W 3.6A at 6s version, your battery will have 12000mAh and nominal 44v 518Wh, to charge at 80W will take 200min at 50W it will take  300min. You will also need two 18V 7A ac/dc adapters to get full power from the chargers.

I use an external 12s bms and an adjustble cc/cv charger with up to 8A charge current at 12s and a watt meter so I can see my charge voltage and current . I charge at 5A 12s, occasionally I hook up my Icharger 308 duo to check the cell balance and internal resistance.

I have  used single focbox and focbox unity with extra heatsink both have been good for me, in my mind it's better to have extra capacity and don't operate close to the limits.
```

---
## \#13 Posted by: pmouraguedes Posted at: 2019-09-16T01:26:30.632Z Reads: 23

```
Interesting charging setup, could you post a link to the external bms and adjustable cc/cv charger you're using?<br>
I'm also thinking about including a 12s charging port, and balance charge only occasionally. Is a BMS needed for simple 12s charging?
```

---
## \#14 Posted by: anders Posted at: 2019-09-17T08:02:24.222Z Reads: 21

```
[BMS](https://www.aliexpress.com/item/32931097519.html?spm=a2g0s.9042311.0.0.1dc14c4dQ6LqSq)

[CC/CV boost converter](https://www.aliexpress.com/item/32919093000.html?spm=a2g0s.9042311.0.0.1dc14c4dQ6LqSq)

[Watt meter](https://www.aliexpress.com/item/32572133851.html?spm=a2g0s.9042311.0.0.1dc14c4dQ6LqSq)

[Power supply](https://www.aliexpress.com/item/32791930537.html?spm=a2g0o.productlist.0.0.446867adzLkMKo&algo_pvid=a45317ce-5e2a-41c7-a306-2659aa221a61&algo_expid=a45317ce-5e2a-41c7-a306-2659aa221a61-0&btsid=98186cf9-64dc-43fa-94e7-ce67d4c4f8e6&ws_ab_test=searchweb0_0,searchweb201602_5,searchweb201603_53)

This is what I use for 12s charging, I can swap between the  48/400 power supply or use a 10s battery and use as a portable charger.
![e334b9c9027c8fe0bf4ef512fcb709447b5e8fcf_2_666x500|666x500](upload://oG12q7Dh38OnE0NMRSrs5GxLqfh.jpeg) 

Portable 12s charger fed by 10s battery boost converted with built in bms and watt meter![64664074_862633927428577_4220953365833580544_n|666x500](upload://4lT0rVvrK97COIlCIkrcBPCR1Q1.jpeg) 


Charging as 2x 6s with  Icharger 308 duo  battery split with xt90 antispark![07d15a574ed9cd01746f5291a7f3131526831315_2_666x500|666x500](upload://b6Uuc6XwsKqLOuk4HoiPkF195y.jpeg) 

BMS is not needed but it's a good safety feature and it's not expensive or hard to plug in, so far my charging methods have worked flawlessly and fast, make sure to have a fuse on the charge plug. I have bought new sp13 connectors that are waterproof and will install them soon.
```

---
## \#15 Posted by: pmouraguedes Posted at: 2019-09-17T14:33:47.310Z Reads: 17

```
Wow, impressive... I have my share of doubts/questions though :slight_smile:
<br><br>
From the first picture what I see is the following:<br>
<br>
charger positive <-> battery positive<br>
charger negative <-> BMS C-<br>
BMS B- <-> battery negative<br>
two 6S balance leads to BMS 12s balance port: how to adapt between the two?

Did you make xt60 connectors with just one of the cables active, either positive or negative?
<br><br>
The only potencial error prone thing I see here, is that it is easy to make a mistake and swap the lead negative and positive in the wrong xt60 plug, reversing the polarity.

Regarding the portable 12S charger, it's a great idea. I have here some 18650 cells from an ex solar generator, which I could use for that purpose.

[quote="anders, post:14, topic:101732"]
make sure to have a fuse on the charge plug. I have bought new sp13 connectors that are waterproof and will install them soon.
[/quote]

Hum... never used fuses, how would one install and use it? 
<br>
[quote="anders, post:14, topic:101732"]
I have bought new sp13 connectors that are waterproof and will install them soon.
[/quote]

Don't know them, I'll check them out, thanks.
```

---
## \#16 Posted by: pmouraguedes Posted at: 2019-09-17T16:06:20.379Z Reads: 13

```
> Portable 12s charger fed by 10s battery boost converted with built in bms and watt meter

BTW, does the boost converter allow to check the voltage of the 10S battery used as power supply or do you use other way to check it?
```

---
## \#17 Posted by: anders Posted at: 2019-09-17T21:14:55.197Z Reads: 11

```
Here comes some answers (some might lead to more questions) it took  me some time and research to figure this out.

charger positive <-> battery positive: Yes
charger negative <-> BMS C-: Yes
BMS B- <-> battery negative: Yes
Q two 6S balance leads to BMS 12s balance port: how to adapt between the two?
A:  Starting with the negative (negative side to esc from 12s) on the left side 6s balance  port  use all 7, negative to negative. on the second (right) balance port pull out the first negative and connect the 6 in order and finish with positive. Measure all the ports on the  BMS  so that it starts with negative and increase from 3.7V up to 44.4V
![70590576_376859763225825_2504137766619578368_n|375x500](upload://fRUdI9BPL0qb6ymOndxYpEFsWEV.jpeg) 

Did you make xt60 connectors with just one of the cables active, either positive or negative?  Yes negative on left xt60 positive on right xt60.

The only potencial error prone thing I see here, is that it is easy to make a mistake and swap the lead negative and positive in the wrong xt60 plug, reversing the polarity. see picture I connected both  the xt60's with a rubber band to keep them right .![70346106_377915346237909_8583123881970106368_n|375x500](upload://a2cKC5Tx4ZtcmBRUMAHrRXfsxkO.jpeg) ![70392645_500176350544818_9131156683827970048_n|375x500](upload://37hSVRgTXnduzQyJwN4NA4FGydV.jpeg) 

Hum… never used fuses, how would one install and use it? connected it on the negative side on the bms 15A 
![71172845_2674458669285410_5275221756573908992_n|666x500](upload://gSPj8OTFWOqXHKKWjyb9LXxjI3K.jpeg)
```

---
## \#18 Posted by: anders Posted at: 2019-09-17T21:41:08.078Z Reads: 9

```
BTW, does the boost converter allow to check the voltage of the 10S battery used as power supply or do you use other way to check it? : The boost converter have potentiometer that can be set to a minimum input voltage that switches it off  below that value, also input needs to be minimum 2V below output value on the boost converter. The boost converter can have output voltage and current adjusted (cc/cv)and be monitored with the wattmeter. Also use antispark on input.

![70459459_949594062100019_3394753261838794752_n|375x500](upload://6tbNcFv3gcdxBWogIkTpiLv3H1I.jpeg) 

This PSU is not cc/cv and needs to be connected and adjusted to the boost converter.(40V)

![70457104_1226149194224420_4739897101519945728_n|375x500](upload://qr1Epzx8xyk3TzrfcEGsouM6sdS.jpeg)
```

---
## \#19 Posted by: janpom Posted at: 2019-09-17T22:11:43.720Z Reads: 9

```
[quote="pmouraguedes, post:1, topic:101732"]
Would it be possible to have 2 x 6S battery packs connected in series
[/quote]

You can charge it with two 6S balance chargers even without breaking the series **provided the chargers do not have common ground**. Otherwise it will short out. :zap:  :fire: 

This typically means the **two chargers must NOT be powered from the same power supply**. As long as you have two independent power supplies that plug into mains you should be fine.
```

---
