# Is my BMS setup correct?

### Replies: 13 Views: 1551

## \#1 Posted by: JimboRatchet Posted at: 2017-07-29T02:32:14.284Z Reads: 162

```
<img src="/uploads/db1493/original/3X/d/6/d63a35c1766e38cbe05b79a10ae5174862c10e10.jpg" width="690" height="355">

Working on my first build here and decided to go the BMS route.I'm a little iffy on my wiring setup but after looking at several different posts on the internet I think I got it right. Any experts here willing to double check my setup and let me know if there's anything I might've done wrong? Thanks!!!

Setup:

[BMS - 8S ebay](http://www.ebay.com/itm/Protection-Circuit-Module-5A-BMS-PCM-for-8S-28-8V-29-6V-Li-ion-LiPo-battery-440C/222272460111?_trksid=p2481888.c100675.m4236&_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D20160908105057%26meid%3D2eccbaccd3b2422cb2a57c2d74d68075%26pid%3D100675%26rk%3D3%26rkt%3D15%26sd%3D331883428207&_trkparms=pageci%253Adc973688-73bd-11e7-a4a7-74dbd180feca%257Cparentrq%253A8a563f4915d0ac8033325136ffffc755%257Ciid%253A1)

[2x Zippy 5Ah 4s battery](https://hobbyking.com/en_us/zippy-flightmax-5000mah-4s1p-20c.html)

[Torque BLDC VESC](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/)

[Turnigy Sk3 6354 260kv](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html)

[Sector 9 board](https://www.amazon.com/gp/product/B01CKKRU14/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1)

[Caliber II trucks](https://www.amazon.com/gp/product/B00NY3Q5Q8/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1)
```

---
## \#2 Posted by: Smorto Posted at: 2017-07-29T02:56:29.534Z Reads: 143

```
Your diagram looks good but I would not recommend that 5A BMS. I recommend battery supports/supower (same company) or bestech BMS.
```

---
## \#3 Posted by: Namasaki Posted at: 2017-07-29T04:27:08.244Z Reads: 145

```
If you wire this bms like that, it will shut the system down when you hit 20a which will happen with 8s voltage.
you would need to bypass the bms for discharge.
But it would be better to take @Smorto advice. and buy a quality bms.
```

---
## \#4 Posted by: JimboRatchet Posted at: 2017-07-29T06:31:55.215Z Reads: 135

```
Thanks for your input guys. Im gonna change the BMS to [this supower BMS](http://www.batterysupports.com/28v-29v-30v-30a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-262.html).
Updated circuit:
<img src="/uploads/db1493/original/3X/6/3/639a07fce6b49dabd207380ce7d9016b81c09513.jpg" width="690" height="460">

My main concern is the wiring of the balance wires, but I think I've got it correct and good to go. thoughts?
```

---
## \#5 Posted by: Smorto Posted at: 2017-07-29T14:33:28.397Z Reads: 117

```
Looks good to me, maybe go for a 45A BMS but it should be fine. I like to be over prepared when it comes to these things but a 30A BMS should work fine.
```

---
## \#6 Posted by: JimboRatchet Posted at: 2017-07-29T16:31:45.872Z Reads: 110

```
 I might just spring for the 45A BMS just to be safe, but I thought that since I am bypassing the BMS output I wouldn't have to worry about the 30A rating. Is that not the case?
```

---
## \#7 Posted by: Smorto Posted at: 2017-07-29T17:30:28.132Z Reads: 101

```
In that diagram you are not bypassing the BMS.
```

---
## \#8 Posted by: pjotr47 Posted at: 2017-07-29T17:57:39.673Z Reads: 97

```
i have a 80amp BMS from bestech i am happy with the service + shipping + price +-50euro
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-07-29T18:23:42.666Z Reads: 94

```
Or just bypass bms for discharge, and use itbonly for balance charging...
```

---
## \#10 Posted by: JimboRatchet Posted at: 2017-07-29T18:47:32.503Z Reads: 95

```
To bypass the BMS for discharge in my case, i'd just need to wire the VESC a direct path to ground, right? Also, what what would be the advantages of using the BMS for discharge as opposed to bypassing it? From what I've seen most folks use the BMS discharge because of the chance of cells going out of balance from rapid discharge. Is that even a common problem considering most builds ditch a BMS entirely?

<img src="/uploads/db1493/original/3X/e/9/e9e5d40d352dbff8b3cd9b71c88ac26f248351d8.jpg" width="690" height="460">
```

---
## \#11 Posted by: Smorto Posted at: 2017-07-29T19:36:55.086Z Reads: 89

```
Im not sure but I don't think that diagram shows the bMS being bypassed though @Namasaki would know more. Most people who don't use a BMS use a balance charger which balances the cells on every charge.
```

---
## \#12 Posted by: Schirmi Posted at: 2017-07-29T19:39:38.276Z Reads: 89

```
If you bypass the BMS for discharge, then the BMS is no longer able to ensure a safe operation of the battery in this mode.
If for example you draw to much current from the battery because of a wrong setting in the ESC or a short circuit,  the battery temperature could rise to unsafe levels. The BMS would normally shut the output off now, though if you do bypass it, you risk a battery fire.
```

---
## \#13 Posted by: JimboRatchet Posted at: 2017-08-14T05:27:39.581Z Reads: 65

```
Finalizing my build here. Almost everything has been purchased and is on its way minus a couple accessories.
Instead of making a new thread I figured i should just update this one. I'm looking into adding some safety precautions into my build (antispark, fuse). I am trying to wire my setup in such a way that I can "power off" certain parts in whatever situations: purple ovals representing anti spark loop keys. What do u guys think? Is this overkill? Any advice?
<img src="/uploads/db1493/original/3X/d/e/de8acd7c19a39ebb2c8b658814809f8f3d70a536.jpg" width="690" height="460">

1) charging - disconnect vesc from circuit          --- only A would be plugged in
2) storage - everything is off      ---- only B is plugged in
3) on - everything is connected and ready to skate   ---- both A + B plugged in

parts:
[BMS - SuPower 8s 60A](http://www.batterysupports.com/28v-29v-30v-60a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-264.html)
[Motor - Turnigy sk3 260kv 6354](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html)
[Zippy Flightmax 4Ah 4s](https://hobbyking.com/en_us/zippy-flightmax-4000mah-4s1p-20c.html)
[8S 28.8V 29.6V Li-ion Li-Po Battery Intelligent Smart Charger 33.6V 2A US](http://www.ebay.com/itm/221896637604)
```

---
