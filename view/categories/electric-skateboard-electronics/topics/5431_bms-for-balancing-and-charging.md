# BMS for Balancing and Charging

### Replies: 11 Views: 1409

## \#1 Posted by: mason Posted at: 2016-07-01T18:17:44.526Z Reads: 143

```
Please help me understand why everyone decides to use the BMS output rather than the batteries. The way I see it, you use the BMS for balancing, laptop style charging, and low voltage cutoff. I don't see the reason to output from the BMS. Additionally, you can get a much cheaper BMS because you are not needing to output 60amps from it. Am I wrong here?
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-01T18:21:15.428Z Reads: 142

```
BMS's do a couple different things.

1. Over Current protection. Used as another line of defense along with fuses, and VESC max amperage settings.
2. Over Charge protection. One of the most useful features which helps balance cells.
3. Over Discharge protection. Used with or without VESC low voltage cut off settings.

If you have a BMS, you would probably want to discharge from it to get the benefits of #1 and to save space so you don't need a bunch of different wires for charge/discharge.

I think the real question is why would you NOT want to discharge from the BMS if you have one?
```

---
## \#3 Posted by: lowGuido Posted at: 2016-07-01T18:45:07.115Z Reads: 135

```
LOL @link5505  I just said the exact same thing in another thread.
I agree.
```

---
## \#4 Posted by: mason Posted at: 2016-07-01T19:30:09.380Z Reads: 124

```
haha great minds think alike
```

---
## \#5 Posted by: mason Posted at: 2016-07-01T19:30:50.686Z Reads: 122

```
The only reason I would buy a BMS is for balancing and ez charging. I believe in the vesc to handle the rest :)
```

---
## \#6 Posted by: akira Posted at: 2016-07-01T20:10:54.496Z Reads: 120

```
If you only use the bms for charging, you need a much smaller one ... and at least half as expensive !!
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-01T20:22:21.357Z Reads: 117

```
true, i guess it depends how trustworthy a cheap bms is
```

---
## \#8 Posted by: akira Posted at: 2016-07-01T20:24:22.166Z Reads: 113

```
A 30A is not necessarily cheaper per Amp than a 60A. It is just smaller ...
```

---
## \#9 Posted by: mason Posted at: 2016-07-01T20:25:17.845Z Reads: 113

```
decided I'm just gonna discharge through BMS for extra safety. probably getting [this](http://www.ebay.com/itm/44V-48V-50-4V-12S-60A-Lithium-ion-Li-ion-LiPo-Li-Polymer-Battery-BMS-PCB-System/221644780045?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D1%26asc%3D20131003132420%26meid%3Deeecc468f2c1406d9accf58f07e4e203%26pid%3D100005%26rk%3D2%26rkt%3D6%26sd%3D221274094989). What chargers do you guys recommend?
```

---
## \#10 Posted by: Jinra Posted at: 2016-07-01T20:25:18.475Z Reads: 114

```
I'm referring to the cheap $10 ones you find on alibaba
```

---
## \#11 Posted by: akira Posted at: 2016-07-01T21:19:24.960Z Reads: 110

```
Ok I understand.
```

---
