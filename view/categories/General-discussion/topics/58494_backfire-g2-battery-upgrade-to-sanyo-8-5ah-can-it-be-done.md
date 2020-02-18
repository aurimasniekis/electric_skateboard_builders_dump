# Backfire G2 battery upgrade to Sanyo 8.5ah can it be done?

### Replies: 20 Views: 2829

## \#1 Posted by: Jlhuxley Posted at: 2018-06-11T07:11:15.353Z Reads: 110

```
Backfire G2 battery upgrade to Sanyo 8.5ah can it be done without changing something?
```

---
## \#2 Posted by: rey8801 Posted at: 2018-06-11T07:24:09.447Z Reads: 110

```
I guess Backfire G2 uses a 10s2p battery and the Sanyo 8.5ah battery that you are talking about is the one that for instance Meepo or other chinese companies are selling? if yes, than they are 10s2p as well. So you can use it without change anything. Anyhow if you have the webpage of the battery you are looking for we can check  :wink:
```

---
## \#3 Posted by: Jlhuxley Posted at: 2018-06-11T07:28:09.280Z Reads: 110

```
:grinning: https://verrealboards.com/products/copy-of-lg-6-4ah-battery
```

---
## \#4 Posted by: rey8801 Posted at: 2018-06-11T07:37:31.226Z Reads: 101

```
ok so those are 20700 battery cells https://www.aliexpress.com/item/1pcs-lot-freight-free-SANYO-20700B-20700-4250mAh-NCR20700B-high-rate-battery-cell-20A-20700/32801056959.html?src=google&albch=search&acnt=479-062-3723&isdl=y&aff_short_key=UneMJZVf&albcp=266121556&albag=7593673036&slnk=&trgt=aud-30186416528:dsa-42862830006&plac=&crea=64152518596&netw=g&device=c&mtctp=b&memo1=1t1&aff_platform=google&gclid=Cj0KCQjwu_jYBRD8ARIsAC3EGCJbIRU0Qd-cxEUXluT5EnnMJnyZYGyoPslwes19L2nVqNDXGjeg5-0aAqfFEALw_wcB to understand.
They are bigger in size than the backfire ones which are 18650 cells, mostly used in esk8. So definitly is a 10s2p, meaning you can use it, but the size of the pack would be a problem. YOu have to check how much space you have left in the backfire enclosure, it might not fit inside.
```

---
## \#5 Posted by: Jlhuxley Posted at: 2018-06-11T07:42:24.961Z Reads: 88

```
Ok will have to consider the size and the fittings are different than the backfire battery has one extra blue and white cables 
http://backfireboards.com/backfire-standard-g2-battery-p-333.html
```

---
## \#6 Posted by: rey8801 Posted at: 2018-06-11T07:51:24.998Z Reads: 85

```
the other wires I guess are for the volt meter (does Backfire have one?) or is there as optional if you use lights, but I can be wrong, anyhow nothing essential for the board do work. The other connectors metter. One for charging and the other one to power the ESC and then the motors. 
YOu can easily check, just open the enclosure and see if is connected, if you do not have lights and no voltmeter is there, then is probably not connected.
```

---
## \#7 Posted by: rey8801 Posted at: 2018-06-11T07:52:29.429Z Reads: 78

```
I know @Lumaci has a backfire G2 so he will know for sure!
```

---
## \#8 Posted by: Jlhuxley Posted at: 2018-06-11T08:01:20.401Z Reads: 71

```
I was looking at ordering the Sanyo battery so should be fine to use but I will open my old battery and check the blue and white wires.
Do you think Rey that the Sanyo would be a good choice or is there something better.
```

---
## \#9 Posted by: rey8801 Posted at: 2018-06-11T08:07:22.995Z Reads: 74

```
I think there are 2 Sanyo 20700 A and B. B has larger capacity so more range but actual tests gave a discarge current optimal at 10A and close to limit 15A which means it will give you 30A costant discharge current which is not a lot but from a 2p battery is hard to find more. I think not a lot of people use it for esk8 yet, So we do not have a lot of feedback, but for sure do not aspect miracles. I would say that a 10s2p Samsung 30Q wuold be comparable or even better. Same size of the one you have it and way better quality of the original back fire. 6Ah camapcity for at least 15-17km and constant discharge current of 20A so 40A in total for a 2p.
```

---
## \#10 Posted by: Jlhuxley Posted at: 2018-06-11T08:14:29.665Z Reads: 68

```
Ok cheers m8 do you know where I can buy a Samsung 30Q 6ah ready to go online?
```

---
## \#11 Posted by: rey8801 Posted at: 2018-06-11T08:15:43.494Z Reads: 65

```
Where are you located?
```

---
## \#12 Posted by: Jlhuxley Posted at: 2018-06-11T08:16:13.181Z Reads: 63

```
Perth Australia
```

---
## \#13 Posted by: rey8801 Posted at: 2018-06-11T08:26:36.498Z Reads: 65

```
Damn...I know US and EU seller for that and ship battery is a mess. Although you could check on Check out the “Electric Riders Melbourne” group on Facebook. Or I know winboard sell custom made battery pack with the cell and BMS you want. I asked at the time the price and it was competitive. At the end I made it by myself.
Here the link https://winboard.en.alibaba.com/productlist.html?spm=a2700.icbuShop.0.0.4e244d3b8w8KpF you send them an email with what you want the they make it for you. I would ask a battery pack, double stack 10s2p with 30Q Samsung cell. You can check the battery size of backfire and get the same. Then ask a small 10s BMS only for charging, whihc is the same you have on the backfire now. Let we know...
```

---
## \#14 Posted by: Jlhuxley Posted at: 2018-06-11T08:32:39.202Z Reads: 58

```
Thanks for the help will look into it cheers :grinning:
```

---
## \#15 Posted by: Jlhuxley Posted at: 2018-06-11T08:34:28.891Z Reads: 61

```
Hey do I need a different bms then the backfire with the Samsung battery
```

---
## \#16 Posted by: rey8801 Posted at: 2018-06-11T08:38:41.143Z Reads: 64

```
No absolutely. It has to be a normal 10s BMS charghing only. MEnaing it will only help balancing the cell during charging. In this way it can be small and do not affect the whole battery size. I think all the pre-built boards use the same strategy. BSM is wired to the battery so Either you do it by yourself or you will need to let them do it with a new one.  cheap BMS is 10$, just to understand the range of price.
```

---
## \#17 Posted by: Jlhuxley Posted at: 2018-06-11T08:38:59.915Z Reads: 62

```
https://www.electricskateboardparts.com/product/10s2p-samsung-30q-electric-skateboard-battery-36v-6ah/
Will this one work
```

---
## \#18 Posted by: rey8801 Posted at: 2018-06-11T08:42:51.793Z Reads: 61

```
absolutely. The onyl thing I see different from backfire is the chaerger connector. You may want to ask them to change it or you do it later. It will take 2 minutes. Check the size and which connector you have on backfire for the battery (Xt60 or xt90) becuase you can choose it. Just open and post a close picture and I will tell you. Usually they use xt60. Then you only need to know if the male or the female part is attached and you ask the complementary one.
```

---
## \#19 Posted by: goldrabe Posted at: 2018-06-11T13:43:05.432Z Reads: 55

```
Hi,
you can swap to the Sanyo battery quite easily! The Backfire battery and the meepo/wowgo/ownboard Sanyo battery seems to have a similar size. The only thing you need to do is to change the charge port or build an adapter. Here is a link to a thread found on reddit. Since this is the builders forum you might have more luck finding stuff there cause the backfire is a prebuild.
https://www.reddit.com/r/ElectricSkateboarding/comments/86a8x0/swapping_batteries_on_backfire_v2/
```

---
## \#20 Posted by: luketommy98 Posted at: 2019-12-07T15:23:02.708Z Reads: 7

```
hi guys new user here looking for help 

i currently own a backfire g2 black 2019 with 36volt 5ah 10s2p 18650 battery but cannot take it on a international flight. im looking to take my board on the plane without the battery and buy a cheapish lipo battery to use whilst on holiday. My question is , would this work and not damage my esc? thats if i can find lipo batterys to connect in parallel to make 36volts. cant seem to find anything online about backfires hobbywing ESC specs either... if anyone ran lipos on their backfire before? or meepo board as they have similar hobbywing esc on models
```

---
