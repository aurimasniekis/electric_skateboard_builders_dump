# Will this BMS work for 10s2p A123 26650 battery pack?

### Replies: 8 Views: 1076

## \#1 Posted by: DanTheBarista Posted at: 2017-02-04T23:36:28.871Z Reads: 93

```
So I know a pack in a 10s2p configuration should be only 33v and have 140a max continuous discharge. Can I hook it up to this bms rated for 36v and 150a max continuous?

Also, I'm going to be running two 190kv motors using this pack as well as two Vescs from Chaka. Am I at risk of blowing the vescs if they are rated for 50a continuous? 

http://www.batterysupports.com/36v-37v-42v-10s-150a-10x-36v-lithium-ion-lipolymer-battery-bms-p-391.html
```

---
## \#2 Posted by: rpn314 Posted at: 2017-02-05T00:00:57.557Z Reads: 89

```
Nothing wrong with having a BMS that is higher than your max current, just don't rely on it to protect your batteries from over discharge (so make sure the battery currents are set properly in the VESC). And your VESCs will be fine, but again, make sure the current setting isn't too high on the VESC itself.

On a side note, I'm hoping that 10s2p pack is Li-Pos or carefully selected Li-Ions, cause I only know of a few Li-Ions that can handle 70A continuous.
```

---
## \#3 Posted by: Pantologist Posted at: 2017-02-05T01:52:44.715Z Reads: 75

```
No because this BMS will overcharge your batteries to 4.2v compared to the correct 3.6v.
```

---
## \#4 Posted by: rpn314 Posted at: 2017-02-05T02:19:14.076Z Reads: 70

```
Really? Isn't the charge voltage for (almost) all lithium batteries 4.2 volts?....Their nominal is 3.7 or 3.6 (if it's Li-Ion or Li-Po), but I thought they generally charge at and up to 4.2

The only ones I'm aware of that are lower are LifePo4 cells
```

---
## \#5 Posted by: Pantologist Posted at: 2017-02-05T02:29:48.057Z Reads: 65

```
Well his title says A123 cells which are LiFePO4 chemistry.
```

---
## \#6 Posted by: rpn314 Posted at: 2017-02-05T02:33:31.297Z Reads: 64

```
Wow. No idea how I missed that. I was wrong. Thank you.

My comments on current ratings stand, but you need a BMS that's made for your battery chemistry, LiFePO4.
```

---
## \#7 Posted by: DanTheBarista Posted at: 2017-02-05T04:03:41.698Z Reads: 55

```
So I decided to only use a bms for balance charging and found this bms but I'm curious as to why it's only rated for 32v?

http://www.bestechpower.com/32v10spcmbmspcbforlifepo4batterypack/BMS-D316.html
```

---
## \#8 Posted by: Aeroquiv Posted at: 2017-02-05T12:53:11.688Z Reads: 50

```
It's probably stating its total nominal voltage, which for a LIFEPO4 battery, is 3.2 V. The 2nd line in the data spec says that it charges at 36V which is what you want as LIFEPO4's max voltage is 3.6 V. 

So it should be fine.
```

---
