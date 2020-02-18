# A solution: Discharging using e-switch with always-on charging

### Replies: 11 Views: 1030

## \#1 Posted by: eitan Posted at: 2017-05-16T15:16:28.501Z Reads: 118

```
There has been [discussion](https://www.electric-skateboard.builders/t/bms-with-e-switch-pros-and-cons-and-how-to-charge-discharge-elegantly/19652/4) on the ideal setup where a BMS with an e-switch is used for discharging (turning on the board), BUT also where that same BMS supports charging the battery without turning on the board/switch. 

It seems obvious, yet according to SuPower, such a configuration is not possible:

<img src="/uploads/db1493/original/3X/8/e/8e9f3f75ef36fadee053b8f9b7e39deec98ae085.png" width="345" height="82">

That sucks, because who wants to have to turn on their ESC just to charge?!

#### Well, I believe I have figured out a solution using TWO BMS's:
 - Use one [high-amperage BMS](https://www.aliexpress.com/item/SuPower-10S-36V-37V-42V-45A-Li-ion-Lithium-LiPo-Battery-BMS-Management-System-Balance-PCB/32800545892.html?ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10068_436_10136_10137_10157_10060_10138_10155_10062_10156_10154_10056_10055_10054_10059_100032_100033_100031_10099_10103_10102_10096_10147_10052_10053_10050_10107_10142_10051_10172_10084_10083_10080_10082_10081_10110_10111_10112_10113_10114_10181_10183_10182_10185_10078_10079_10073_10123,searchweb201603_1,ppcSwitch_5&btsid=e0fd9333-b020-48d3-855c-040a0350e49e&algo_expid=3ee55d2e-be1f-4c7a-83b6-0a578d26c065-0&algo_pvid=3ee55d2e-be1f-4c7a-83b6-0a578d26c065) with an e-switch for discharging
 - Use another [low-amperage BMS](https://www.aliexpress.com/item/10S-15A-BMS-for-36V-li-ion-battery/1195130789.html?ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10068_436_10136_10137_10157_10060_10138_10155_10062_10156_10154_10056_10055_10054_10059_100032_100033_100031_10099_10103_10102_10096_10147_10052_10053_10050_10107_10142_10051_10172_10084_10083_10080_10082_10081_10110_10111_10112_10113_10114_10181_10183_10182_10185_10078_10079_10073_10123-10050,searchweb201603_1,ppcSwitch_5&btsid=58d84c76-92db-4605-a316-7c0c2e15c152&algo_expid=544db308-e118-4901-adda-86c6432232c1-2&algo_pvid=544db308-e118-4901-adda-86c6432232c1) for balance charging (+$15)

Please observe the diagram below. Would this work?

<img src="/uploads/db1493/original/3X/d/4/d4aef805a701b09b52168fe729820f1c5019245a.png" width="690" height="497">
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-16T15:33:20.904Z Reads: 108

```
Enertion's space cell bms does exactly this somehow, not really sure how it works.  

I personally bypass bms discharging to avoid this issue.
```

---
## \#3 Posted by: eitan Posted at: 2017-05-16T16:22:23.788Z Reads: 103

```
In this case, the discharging BMS essentially functions as a big anti-spark switch (edit: with OC protection h/t @SilentException).  So @Jinra, if you're bypassing the BMS discharging, I'm guessing you're using a vedder or anti-spark switch?
```

---
## \#4 Posted by: Maxid Posted at: 2017-05-16T16:26:43.775Z Reads: 96

```
why use a BMS for discharge at all then? Use a Vedder Switch to turn on your board if you want an "e-switch".
```

---
## \#5 Posted by: Jinra Posted at: 2017-05-16T16:27:24.512Z Reads: 96

```
Yep I use an anti spark switch
```

---
## \#6 Posted by: eitan Posted at: 2017-05-16T16:51:39.668Z Reads: 93

```
> why use a BMS for discharge at all then? Use a Vedder Switch to turn on your board if you want an "e-switch".

@Maxid Cost. 
Vedder switches cost upwards of $40-60 plus shipping, **and** you need buy a BMS.
With the two-BMS setup, the cost for  **both together** is under <$55.

Example: [60A Discharging BMS ($39 shipped)](https://www.aliexpress.com/item/SuPower-10S-36V-37V-42V-60A-Li-ion-Lithium-LiPo-Battery-BMS-Management-System-Balance-PCB/32801166001.html?spm=2114.01010208.3.16.O7uhf2&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10065_10151_10068_5160014_436_10136_10137_10157_10060_10138_10155_10062_10156_10154_10056_10055_10054_10059_100032_100033_100031_10099_10103_10102_10096_10147_10052_10053_10050_10107_10142_10051_10172_5150014_10084_10083_10119_10080_10082_10081_10110_10111_10112_10113_10114_10181_10183_10182_10185_10078_10079_10073_10123_10120,searchweb201603_9,ppcSwitch_5&btsid=6041132b-e4bb-419f-828e-c9f430bdf56c&algo_expid=52810880-c68c-458e-8bbc-d1f89d06e89a-2&algo_pvid=52810880-c68c-458e-8bbc-d1f89d06e89a) and [charging BMS ($15 shipped)](https://www.aliexpress.com/item/10S-15A-BMS-for-36V-li-ion-battery/1195130789.html?spm=2114.01010208.3.2.EGdi3a&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10065_10151_10068_436_10136_10137_10157_10060_10138_10155_10062_10156_10154_10056_10055_10054_10059_100032_100033_100031_10099_10103_10102_10096_10147_10052_10053_10050_10107_10142_10051_10172_10084_10083_10119_10080_10082_10081_10110_10111_10112_10113_10114_10181_10183_10182_10185_10078_10079_10073_10123_10120-10050_10120,searchweb201603_16,ppcSwitch_5&btsid=6f074a7e-4c1d-4436-bd4b-5bdea4468eda&algo_expid=5b30fac5-0fd6-4a81-9e99-7c0e797740d5-0&algo_pvid=5b30fac5-0fd6-4a81-9e99-7c0e797740d5)
```

---
## \#7 Posted by: SilentException Posted at: 2017-05-16T16:58:09.049Z Reads: 88

```
Output BMS also serves as LV and OC cut-off, not just glorified anti-spark switch ;) 

I'm talking about configuration from OP, and that should work just fine for the purpose. Would be a bit careful using cheap BMS even if just for charging. Balancing cells is an art :)
```

---
## \#8 Posted by: Maxid Posted at: 2017-05-16T17:09:12.187Z Reads: 88

```
Where are you buying your Vedder switches? Esk8 sells them for like 25€. Also the Vedder needs less space than two huge BMS

https://www.electric-skateboard.builders/t/new-vedder-sparcprotectionswitch-1-3-for-sale-lowest-price-from-28-free-shipping-worldwide/17402
```

---
## \#9 Posted by: Namasaki Posted at: 2017-05-16T18:12:08.935Z Reads: 78

```
I'm been charging with dual Vescs on for months on 2 builds and it has caused no issues at all. 
I feel its well worth it to have all the protection a BMS affords in discharge mode along with a dependable and convenient anti-spark solution. 
I tried stand alone e-switches and they failed. 
The e-switches in my Bestech bms's have been rock solid.
```

---
## \#10 Posted by: eitan Posted at: 2017-05-16T19:33:02.785Z Reads: 70

```
@Namasaki  Ah, can you clarify your setup?
Dual Bestech BMSs like the setup described in the original post?
Or are you using Bestech BMS + vedder/anti-spark switch?

Thanks
```

---
## \#11 Posted by: Namasaki Posted at: 2017-05-16T20:14:06.530Z Reads: 64

```
Just Bestech Bms with dual Vescs on 2 separate builds.
That is, I have 2 builds that have same setup.
```

---
