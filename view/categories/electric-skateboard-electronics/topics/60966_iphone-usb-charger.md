# Iphone / usb charger

### Replies: 13 Views: 492

## \#1 Posted by: Hatman30 Posted at: 2018-07-05T13:58:51.275Z Reads: 147

```
I'm not sure if this is the right place to put this but well...here it is.
I've tried a few options before with mixed success. A £3 usb buck converter with built in lcd and usb port that got really hot, melted part of the pcb and then started smoking abd various other cheap dc step downs that only work for android phones or 12v lights. 

This way works, is reliable, and most of all is safe.
I wired in a Fulree DC-DC 15-55v to 12v 3A max converter in parallel to the vesc circuit. I put in a push button lactching switch so I can turn it on and off even when the board isn't on and used an inline fuse which I got off of a 12v motorcyle waterproof usb adapter which is what teh Fulree is outputting to. 
The perks of having this is 
A) It already comes with an inline fuse that is easily swapped should anything go wrong and B) it has an SAE connector which means it's easy to disconnect it if and when I want ot take the case off. 
C) the USB plug has a waterproof cover
Here is a link 
https://www.amazon.co.uk/MICTUNING-Disconnect-Waterproof-Motorcycle-Cellphone-SAE-USB-Adapter-Extension-Cable/dp/B01MSK7ZAV/ref=pd_lpo_sbs_263_img_1?_encoding=UTF8&psc=1&refRID=9VS1KC5GTBE8KWMRA7WR
![IMG_7820|375x500](upload://4nkanPBhGzmUurOqS7IzbBP1DqL.jpg)![IMG_7817|500x500](upload://frKYxJvtsyJheeeDFVzfG5r8NPT.jpg)
![IMG_7822|375x500](upload://ra8unj8GOkYZxDAy6Td2diUSvFF.jpg)

Here is a pic of the push button switch and also for anybody that has epoxied their XT90 into the case this is how I got round not being able to take the case off.
![IMG_7821|375x500](upload://7ziCKjvMtBprgIOEW7GdjpDzus9.jpg)
```

---
## \#2 Posted by: Ebisane9 Posted at: 2018-07-05T14:58:31.679Z Reads: 125

```
@JLabs uses a nice step-down, I think he may have some in stock.
```

---
## \#3 Posted by: Hatman30 Posted at: 2018-07-05T16:16:43.696Z Reads: 120

```
I’ve already got that sorted thx. Read the above thread 👍
```

---
## \#4 Posted by: sunnyD Posted at: 2018-07-05T18:34:18.850Z Reads: 106

```
Haha this is cool! Why not go one step further and include a wireless charging pad XD. But in all seriousness good work dude.
```

---
## \#5 Posted by: mynamesmatt Posted at: 2018-07-06T00:14:27.624Z Reads: 93

```
https://www.ebay.com.au/itm/141871702338?ul_noapp=true
I used one of these and it works great
```

---
## \#6 Posted by: Psmrman90 Posted at: 2018-12-31T05:58:35.037Z Reads: 61

```
Would this work?  Just connect it to the battery?

HOMREE DC DC Converter Buck Module 12V/24V to 5V 3A USB Output Step Down Voltage Regulator Charge for Samsung Galaxy , iPad iPhone 4S 5 6/6 Plus etc (Standard USB) https://www.amazon.com/dp/B01MEF293V/ref=cm_sw_r_cp_apa_i_V-AkCbE4NEZ0K
```

---
## \#7 Posted by: Andy87 Posted at: 2018-12-31T06:00:48.603Z Reads: 57

```
If your battery is max 24V than yes.
```

---
## \#8 Posted by: Psmrman90 Posted at: 2018-12-31T06:04:43.739Z Reads: 57

```
Didn't see that, my BKB 11s3p battery makes out at 48v I think, so this should work, right?  Or is it cutting it too close? 

https://www.amazon.com/dp/B00W52N8XW/ref=cm_sw_r_cp_apa_i_UeBkCbGF79KPV
```

---
## \#9 Posted by: Andy87 Posted at: 2018-12-31T06:07:04.572Z Reads: 55

```
Looks good for me. 46.2v is far from 50v. Shouldn’t make any problems.
```

---
## \#10 Posted by: b264 Posted at: 2018-12-31T08:47:24.203Z Reads: 49

```
[quote="Andy87, post:9, topic:60966"]
46.2v is far from 50v. Shouldn’t make any problems.
[/quote]

46.2V is far from 50V -- when not driving inductive loads with it.  So charging a phone or an apple thing would be fine.

Driving motor windings at 46.2V on 50V rated parts would not be fine.
```

---
## \#11 Posted by: Andy87 Posted at: 2018-12-31T08:53:05.066Z Reads: 47

```
Thank you for making that clear. Totally agree with you in this point 👌
```

---
## \#12 Posted by: Faceplant Posted at: 2019-07-19T06:04:14.813Z Reads: 21

```
So this is probably a bad idea for my 6s Lipo's? I was just gonna solder on an xt-60 and keep it hooked up to the voltage alarm so I don't start a fire.
https://www.ebay.com.au/itm/QC-3-0-Dual-USB-Car-Charger-Cigarette-Lighter-Socket-Power-Adapter-Outlet-12-24V/254181051542?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D1%26asc%3D20161006002618%26meid%3Dfa39ab5cf2e5499686253ab9dd3de027%26pid%3D100694%26rk%3D3%26rkt%3D30%26sd%3D142896995935%26itm%3D254181051542%26pg%3D2385738&_trksid=p2385738.c100694.m4598
```

---
## \#13 Posted by: Faceplant Posted at: 2019-07-19T06:07:24.747Z Reads: 21

```
Otherwise I'll probably just add a small container and pad it with foam for my power bank, bit bulky for pockets and I don't always want my backpack weighing me down but I suck at keeping my phone ready to leave the house lol.
```

---
