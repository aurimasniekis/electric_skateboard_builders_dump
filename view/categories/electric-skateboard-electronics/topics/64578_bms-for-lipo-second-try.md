# BMS for LiPo - second try

### Replies: 4 Views: 242

## \#1 Posted by: TiMMaTTie Posted at: 2018-08-11T19:42:41.486Z Reads: 76

```
Sooo I just destroyed my BMS (I think). At some point, I connected the balance leads before the ground to B- was connected. Now, the BMS gets hot when the balance leads get connected, without charger or esc. 

Before I make the same or some other mistake, I would appreciate additional pairs of eyes before I re order and try it again with the B- being the first connection.

I used the following bms for charging only and wired it as follows (2x 4s lipo): 
https://www.aliexpress.com/item/Protection-Circuit-Module-5A-BMS-PCM-for-8S-28-8V-29-6V-Li-ion-LiPo-battery/32747679482.html?spm=2114.search0104.3.23.6f8424b8GP70Ph&ws_ab_test=searchweb0_0,searchweb201602_2_10152_10151_10065_10344_10068_10342_10343_10340_10341_10696_10084_10083_10618_10304_10307_10820_10821_10301_10843_10059_100031_10103_10624_10623_10622_10621_10620,searchweb201603_16,ppcSwitch_4&algo_expid=617cb7ee-532d-4955-b141-5da147837a8a-3&algo_pvid=617cb7ee-532d-4955-b141-5da147837a8a&priceBeautifyAB=0
![s-l1600|615x500](upload://20frSKX5kYRlJxlNwWeLvg0o3eM.jpg)
```

---
## \#2 Posted by: Jake2k17 Posted at: 2018-08-12T04:23:12.501Z Reads: 57

```
A couple mistakes here, 
1: Your ground balance cables from both batteries should be disregarded. They are not needed with a bms. However. Your negative lead should be connected to b-. Your positive lead is good where it is.
2: I can’t see the numbers on your 8 pin balance port, but the 2nd pack should be your first pack, because the pack that supplies the negative lead to esc is always first. The 1st pack connects to the bms balance ports 1-4. The order should be the positive balance cable farthest away from the red balance cable, because the red balance cable is the last positive balance cable in the pack. So if you hold up your white balance connector with the ground cable on the right, the balance cable just to the left of that is your 1st cable, the wire to the left of that the 2nd, and so on until your red wire is 4th. Same thing on the next pack, the wire to the left of the ground wire is 5th, and so on until the red wire is 8th.


Sorry if that was confusing, I Don’t know what colors your wires are except for the red wire.
```

---
## \#3 Posted by: TiMMaTTie Posted at: 2018-08-12T19:04:12.882Z Reads: 39

```
Thanks for your reply, feeling more confident now :slight_smile:
1)  The balance cable I connected to b- should be the same as the main negative lead but thinner wire which doesn't matter for charge only. But I intended to swap to main negative just in case.
2) b8 is on the far left so this should be fine (far left in the diagram, far right in the picture), I noticed I numbered the lipos in a less logical way![IMG-20180811-WA0005|250x500](upload://pxrNmhiIoX2Cg5ec4Fp2nsjav3X.jpeg)
```

---
## \#4 Posted by: Jake2k17 Posted at: 2018-08-12T19:11:46.431Z Reads: 36

```
No problem! I had the same problem a while ago, now your wiring seems to be fine, good luck with the rest of your build:grinning:
```

---
