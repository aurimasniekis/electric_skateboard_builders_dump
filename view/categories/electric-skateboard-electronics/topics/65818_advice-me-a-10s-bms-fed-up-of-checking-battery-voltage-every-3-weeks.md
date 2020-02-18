# Advice me a 10s BMS. Fed up of checking battery voltage every 3 weeks

### Replies: 24 Views: 387

## \#1 Posted by: rey8801 Posted at: 2018-08-23T10:08:39.918Z Reads: 105

```
Hi! I change my BMS configuration to charge only and I start having the problem that 2-3 cell packs are not balanced anymore https://www.electric-skateboard.builders/t/battery-doesnt-fully-charge-anymore/59812/49?u=rey8801. I would like to manually balance them every 3 weeks so do you have a good BMS advice? It can be discharge/charging or charging only. For discharge I need at least 60A, but I would like to avoid the problem I had with the BMS turnoff the board durign hard braking, when battery close to fully charge state.
In the other thread @bartroosen12 suggested me this one https://www.aliexpress.com/item/32827750823/32827750823.html?shortkey=fmQRjeYJ&addresstype=600 which I like the fact that I can see real time values and be sure it's working properly.
I haven't look deep in BMS world recently, is there something worth it at the moment?
My limitations are size, max like 100x70x20 mm (already rather big I would say), the balance port, since mine is using the standard one and I would like not to open up all the battery and resolder the balance wires (Current BMS https://www.aliexpress.com/item/10S-60A-bms-Li-ion-large-high-current-BMS-PCM-with-SAME-discharge-port-for-electric/32829800932.html?spm=a2g0s.9042311.0.0.27424c4doLEYok). Thx guys!
```

---
## \#2 Posted by: dg798 Posted at: 2018-08-23T10:10:34.755Z Reads: 101

```
@thisguyhere might have some charge only 10s bms. I use his 12s one and it works fine.
```

---
## \#3 Posted by: rey8801 Posted at: 2018-08-23T10:13:52.715Z Reads: 99

```
Thx, only thing I see that for the 10s the balance port is split it so I would need to resolder everything :sweat_smile: . But thank you for the advice, I know Bestech is a good one.
```

---
## \#4 Posted by: Z4MSupreme Posted at: 2018-08-23T10:19:07.320Z Reads: 93

```
i havent used it yet but i bought a 10s bms from Alien Power Systems. i think it is a bestech and it has a built-in e-switch
```

---
## \#5 Posted by: rey8801 Posted at: 2018-08-23T10:20:41.963Z Reads: 89

```
i will have a look, although I do not need the switch anymore.
```

---
## \#6 Posted by: Z4MSupreme Posted at: 2018-08-23T10:23:00.817Z Reads: 84

```
you dont have to use it. it is just a feature that will save you from having to get an antispark
```

---
## \#7 Posted by: rey8801 Posted at: 2018-08-23T10:24:30.108Z Reads: 81

```
I know it, I was just thinking loud :yum:
```

---
## \#8 Posted by: Z4MSupreme Posted at: 2018-08-23T10:31:50.988Z Reads: 81

```
:grinning:
:+1:
```

---
## \#9 Posted by: mynamesmatt Posted at: 2018-08-23T12:01:53.503Z Reads: 74

```
yeah bestech have the 10 pin plug on them, it works alright. What i did in my enclosure is design a cable that had the bms connected to my 2 5s leads, but have my Voltmeter in parallel with the battery so you can see the individual voltage of each cell. I then wired these up to a small switch so that i could check them only when needed 

![20180622_140311|374x500](upload://s6Uug8Py63sV7NTT5u8FwF7XmHA.jpg)
![20180715_174934|666x500](upload://zXakbxKtmm2jdrmxWcl8q2MsrzY.jpg)![20180715_223711|666x500](upload://A9vMCEmen2i650Q5wdNjrbKBCTT.jpg)![20180715_224021|666x500](upload://ovcTqVRKCH7hIUzrh5j8urlw1x9.jpg)![20180811_230400|374x500](upload://fFjtOKt18xQ1W12xXInFzjgJhVO.jpg)
![Screenshot_20180823-220042_Video%20Player|243x500](upload://eI9DwAxaYbfs6T1i4ICU6OxOZbw.jpg)
```

---
## \#10 Posted by: rey8801 Posted at: 2018-08-23T12:14:57.952Z Reads: 67

```
Brilliant! Really nice
```

---
## \#11 Posted by: mynamesmatt Posted at: 2018-08-23T13:21:15.924Z Reads: 63

```
just a handy idea to save you opening the enclosure to check voltages
```

---
## \#12 Posted by: bartroosen12 Posted at: 2018-08-23T14:47:16.079Z Reads: 57

```
If you need 60A I should go for a 80 or 100A bms:
http://s.aliexpress.com/Ar6z2mIF?fromSns=

I'm going to make a 2kW electric mountainbike and gonna use a 20S 100A smart bms, same seller.
I really like the 10S 60A bms I got, it just works perfect. The esc only pulls max 20A so it's very safe with the 60A bms. You can set a lot of setting via bluetooth so very handy.

I have a 10S4P 30Q right now and I haven't ridden for a month because I got exams but It's good to check if the bms uses power when my board it's just laying on my desk.

Inhave charged it to 41.5V, each cell perfect 4.15V and right now every cell is 4.1V so only used 0.5V in total for doing nothing so that's fine.
(I have set balance to always and the voltage diffence is set to 0.005V so the bms is almost always balancing to get every cell the same +-0.005V but I'm gonna set that value back to 0.01V it was just to test)
```

---
## \#13 Posted by: rey8801 Posted at: 2018-08-23T15:03:54.572Z Reads: 51

```
Hi! Yes up to now the one you have is my first choice. I have a 10s3p 30Q so 60A constant it's still ok I think. With the new hubs i am using now I pulled out 52A at most, so should be fine or do you think it is too close? Otherwise I go with the 80A to be sure. I am waiting the sales, they should start in 4 days on Ali. I bought my BMS from the same seller but it is the basic one and only charging doesn't do the job very well unfortunately.
```

---
## \#14 Posted by: Namasaki Posted at: 2018-08-23T15:12:06.543Z Reads: 50

```
@JLabs has Bestech bms’s in stock at bargain prices.
```

---
## \#15 Posted by: rey8801 Posted at: 2018-08-23T15:12:56.282Z Reads: 51

```
Yeh but I am in EU. Probably the shipping will kill the deal. I will check it.
```

---
## \#16 Posted by: JLabs Posted at: 2018-08-23T15:16:53.277Z Reads: 49

```
Shipping should be around $15 for slow but tracked.. if it isisnt let me know and i will have to fiddle with it to get it right
```

---
## \#17 Posted by: TowerCrisis Posted at: 2018-08-23T15:33:45.218Z Reads: 45

```
If a BMS that's charge only isn't working for you, and you still want to bypass for discharge, then a balance board is probably your best option. Something like [This](https://m.aliexpress.com/item/32728243247.html?trace=wwwdetail2mobilesitedetail&productId=32728243247&productSubject=10S-4-2v-li-ion-balancer-board-li-ion-balncing-full-charge-battery-balance-board) would work fine for your use.

It does not have any of the safety measures of a BMS, but you would already be losing all of that by bypassing it for discharge. The only difference between a balance board like this and a bypassed BMS is that the BMS will protect from overcharging from your charger (this excludes brake regen, that is unprotected still)

It's a lot cheaper and a lot smaller than bypassing a BMS. It also will continually balance your cells, whether charging, discharging, or if your board is off.
```

---
## \#18 Posted by: rey8801 Posted at: 2018-08-23T15:39:55.901Z Reads: 42

```
I didnt' know about it. I would only need to connect the balance leads to it. Right? So basically it does balance the cell continuously without the other feature of a BMS, which actually I do not use it anyway. Did I understand correctly?
```

---
## \#19 Posted by: TowerCrisis Posted at: 2018-08-23T15:45:06.109Z Reads: 39

```
Yep, no additional BMS needed. The page says you need one, but electrically there is no difference, the board cannot tell if there is a BMS there or not.
```

---
## \#20 Posted by: rey8801 Posted at: 2018-08-23T15:48:09.125Z Reads: 38

```
Thank you if I won't buy a discharge BMS I will then go for it. ONe question in the diagram it says to connect B+ and B-, since it-s only for balancing two thinner wires is gonan be fine right? the same I use for the balance leads.
```

---
## \#21 Posted by: rey8801 Posted at: 2018-08-23T15:51:44.256Z Reads: 36

```
Do you know the type of JST 10pins used in a BMS. I was thinking of just buy the male version, as on the BMS, and connect to it. So I wont' need to cut the current jst connector in case I wantot come back to normal BMS.
```

---
## \#22 Posted by: bartroosen12 Posted at: 2018-08-23T15:52:33.741Z Reads: 37

```
Yeah the sales Aliexpress are awesome!
![aliexpresshd|281x500](upload://mpxRdRfe3M9A73oJhDMM0dZrbj7.png)
That's the main reason I wanna make an ebike 😅
```

---
## \#23 Posted by: TowerCrisis Posted at: 2018-08-23T15:53:05.793Z Reads: 34

```
Yes, you can use the same wires as the rest of the balance wires.

Some Lipo batteries come preconfigured with 11 pins on a 10S battery, because it includes the additional ground pin.

Most BMS's don't need the ground pin because they are already pulling the ground pin from the inline negative terminal of the battery, which is how they switch the power on and off incase of faults or shorts. But in this case it has no inline negative, so it needs the additional pin.
```

---
## \#24 Posted by: rey8801 Posted at: 2018-08-23T15:55:30.235Z Reads: 33

```
My collegue made an ebike last year and at the time we were looking at that kit. We ended up buying antoher one and it is still going strong. 800 Euro full kit for 60khm bike ahahahah Nice!
```

---
