# BMS experiences

### Replies: 5 Views: 518

## \#1 Posted by: chrismccabe Posted at: 2018-01-20T20:44:41.801Z Reads: 86

```
Hi guys,

Have done a few battery packs before for other uses, but lipo. Am looking into doing a 18650 liion pack for a board 10S3P (VTC-6 cells).
Just have a few more questions left before starting, and browsing through the forums I didn't find a definitive answer to this.

What are your experiences on charging these larger (series) packs?
- Splitting into two 5S packs and leaving the balancing to a normal li-ion charger? 
- Using a 10S BMS for balancing and powering with a dumb power supply?
- When not using a BMS, you use your VESC for average over- and under voltage protection?


What are your experiences with different BMS's and which are the good ones?

[This one any good?](https://www.aliexpress.com/item/SuPower-10S-36V-37V-42V-60A-Li-ion-Lithium-LiPo-Battery-BMS-Management-System-Balance-PCB/32801166001.html?spm=2114.search0104.3.158.54ae82cdBHPCus&ws_ab_test=searchweb0_0,searchweb201602_1_10152_10151_10065_10344_10068_10342_10343_10313_10059_10340_10341_10534_100031_10084_10604_10083_10103_10304_10307_10615_10301_10142,searchweb201603_25,ppcSwitch_2&algo_expid=6f49ff0e-5598-40c3-9070-68ec2dd1f648-23&algo_pvid=6f49ff0e-5598-40c3-9070-68ec2dd1f648&priceBeautifyAB=2)

Sorry if this has been posted loads before, couldn't quite find a topic covering the pro's and con's of charging in comparison to the setup of the board.
```

---
## \#2 Posted by: Martinsp Posted at: 2018-01-20T20:53:38.225Z Reads: 78

```
I use the linked 60A BMS on my daily board. I have it set to both charge an discharge through it and it works very well for me. I ordered it here http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html For charging I use a "dumb charger" which is just two notebook power supplies that I -connected in series a couple of years ago and it charges to 41V. It sounds dangerous and "janky" but it works flawlessly.
```

---
## \#3 Posted by: SeanHacker Posted at: 2018-01-20T21:03:39.613Z Reads: 66

```
I use the linked BMS also, with this  dumb charger. No problems at all. Works great!

![IMG_20180120_130211|690x388](upload://gYt2Bic21UlT92afACWCLnX8TPv.jpg)
```

---
## \#4 Posted by: chrismccabe Posted at: 2018-01-20T21:06:58.470Z Reads: 59

```
Wow you guys are great! Cheers for the speedy reply! :slight_smile:
Looks like the same one I was looking at, cool. Do they actually manage the CC-CV part of the charging in a correct way or have you never really monitored that? And do you manage to put the full power through it? Have you also been using the BMS for a while?

And nah, that power supply sounds good to me. Haha! I've bodged some stuff together in the past also. Xbox or server PSU's work perfectly.
```

---
## \#5 Posted by: Martinsp Posted at: 2018-01-20T21:10:59.555Z Reads: 50

```
At the time I put the board together I did not know a whole lot about charging just the voltage and basics so I never really checked if it works as it should. Maybe someone else has done some testing with this.
Well the BMS is in use on that board for a little over a year now. I am using 30Q 10S3P so I have the limit set to 45A in VESC so I have never pulled 60A through it, during hard acceleration it does 45A based on ackmaniacs app.
```

---
