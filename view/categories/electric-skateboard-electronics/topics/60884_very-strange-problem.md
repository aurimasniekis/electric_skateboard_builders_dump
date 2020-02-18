# Very strange problem

### Replies: 9 Views: 531

## \#1 Posted by: KevinMinato Posted at: 2018-07-04T15:01:36.377Z Reads: 141

```
I have run into a pretty big issue with my electronics on my DIY board. I am running 4x 3s lipo batteries in series. I just finished the first battery discharge using the board or so I thought. But now I am not able to get it to charge again. I then got out the volt meter and check all the cell voltages and it goes like this…

Lipo 1:
- 3.5
- 3.5
- 3.5
Lipo 2:
- 3.5
- 3.5
- 3.5
Lipo 3:
- 0.4
- 2.0
- 0.7
Lipo 4:
- 3.5
- 3.5
- 3.5

now obviously that 3rd battery in series is completely off. And I am not sure what is wrong with my wiring if anything? When I plug in my laptop style charger the light never turns red to indicate its charging. it just stays green. I am stumped 
![Wiring%20Diagram%20ESK8|690x424](upload://lV5toj3oHkOUv0mF3BQQ7djk3L0.jpg)
![20180704_072419|690x388](upload://amueS3cYFhPCCfxOrvhnqA7sCI8.jpg)
```

---
## \#2 Posted by: Martinsp Posted at: 2018-07-04T15:12:44.080Z Reads: 123

```
Are you measuring on the BMS input? or at the batteries? It may be just a bad connection somewhere along the way If your battery is really at near 0V the BMS may not start charging since it could be dangerous.
```

---
## \#3 Posted by: KevinMinato Posted at: 2018-07-04T15:15:37.637Z Reads: 119

```
I am checking at the batteries balance leads directly. from what I have read these voltages seem impossibly low.
```

---
## \#4 Posted by: Martinsp Posted at: 2018-07-04T15:16:58.174Z Reads: 116

```
Yeah they are very low. I would not suggest using them any more. I have heard of people that revived their batteries from a very low voltage but unless you know what you are doing, and even then, I would not recommend it.
```

---
## \#5 Posted by: BoostedBuilder Posted at: 2018-07-04T15:23:30.812Z Reads: 109

```
Battery 1, 2 and 4 are perfectly fine. It's the 3rd one that's the problem. If you bought them at hobbyking, contact them and they'll send you a new one.
```

---
## \#6 Posted by: KevinMinato Posted at: 2018-07-04T19:24:36.012Z Reads: 79

```
Would this faulty battery cause the charger to not do anything?

![20180704_092627|281x500](upload://4ewlzKlJCX9pHCOQfBEdHwDOgnE.jpg)![20180704_092538|281x500](upload://cPdYWGoFYVQ62RWTbxHGZZB2KKv.jpg)![20180704_092603|281x500](upload://uZfgSmWW8IrIBMYxrmjdbvPELmf.jpg)
```

---
## \#7 Posted by: banjaxxed Posted at: 2018-07-05T21:04:18.796Z Reads: 54

```
Did you charge each lipo with a lipo balance charger before making the pack?

Which bms is it, does it supports float charging - cell balancing? If so did you leave it charging long enough to get a float charge?

Did you ever see the pack at full voltage measured?
```

---
## \#8 Posted by: KevinMinato Posted at: 2018-07-05T21:34:11.973Z Reads: 51

```
I got a facebook friend to balance charge them all before i made the pack

I am using this BMS: https://www.ebay.com/itm/44V-48V-50-4V-12S-30A-Li2MnO4-ion-Li-ion-LiPo-Li-Polymer-Battery-BMS-PCB-System/221274094989?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649

I am not sure what float charge is. 

I just charged it now with my charger. this one: https://www.aliexpress.com/item/Yangtze-50-4V-4A-3A-Lithium-Li-ion-Battery-Charger-For-44-4V-Lipo-Bike-Power/32836644573.html?spm=a2g0s.9042311.0.0.91fd4c4di78vMo 
seems like it is charging it far past 11.1v per battery pack

everything got to the same level after charging but it seems like battery 3 is discharging faster
```

---
## \#9 Posted by: banjaxxed Posted at: 2018-07-05T21:38:09.406Z Reads: 44

```
Cell balancing is where one of the parallel groups does not report the correct voltage, good bus's can account for this and bring it back in line. I'm a little out of my depth on this topic but I would definitely have concerns about continuing to use that problem battery in the pack regardless of how it's charging. From my read of the bms specs it does not appear that it could help with a serious imbalance 

Bms specs 

The BMS only use for new and consistent high drain batteries. 
Do not use for battery packs that mix with new & half-used, or mix with different brand battery cells.
Do not use for used and imbalance battery cells.

Balanced current: 60mA (VCELL = 4.20V when)
Balanced for: 4.20 ± 0.05 V

Technical Parameters:
Balanced current: 60mA (VCELL = 4.20V when)
Balanced for: 4.20 ± 0.05 V


Over-discharged threshold: 2.90 ± 0.05 V
Over-discharged delay: 5mS
```

---
