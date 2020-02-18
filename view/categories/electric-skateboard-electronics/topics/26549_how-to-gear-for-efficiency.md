# How to gear for efficiency

### Replies: 9 Views: 1123

## \#1 Posted by: flywithgriff Posted at: 2017-07-01T22:43:09.979Z Reads: 136

```
I am curious of hearing options to help reduce vesc temperatures. I am currently running:

10s1p lipo (5x2s 5ah 30c)
Vesc 4.12
15/36
90mm clones

I am a heave rider at 250lbs and am having the problem of a soft shut down due to temperature if the vesc. This only happens on uphill or high speed runs. A brief 30-45 second break from riding and all goes back to normal. My question is what hearing options I should look at to help with this issue. I have been told a 13/36 will help but I am having difficulty finding a 13t drive pulley.
```

---
## \#2 Posted by: sl33py Posted at: 2017-07-01T22:54:55.652Z Reads: 135

```
Hopefully someone with a better recall will chime in, but i thought i remember Vedder suggesting top efficiency was around 8600rpm?  Problem is that usually is over the 60k ERPM limit if i'm not totally off base.

While looking at gears i might suggest the DIYes 13/40 combo, if you don't mind a bit less top speed.

running quick speed calc - your setup should get about 26?  (also being a heavy guy - i don't always reach the calculated top speed).

13/40 = ~20
13/36 = ~22

12mm or 15mm setup?  Single i'm guessing 15mm?  Those can be tough to find...
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-07-01T23:12:37.892Z Reads: 130

```
Thank you for the knowledge. I'm currently running a 15mm setup but I've never had a slip so I may can get away with 12mm. As long as I can hit 20mph I'm good!
```

---
## \#4 Posted by: sl33py Posted at: 2017-07-01T23:51:07.796Z Reads: 114

```
15mm gears can be a PITA to find.  at least with the 3mm keyway.  (edit - 12mm gears are really a PITA, 15mm are just harder to find w/ keyway, but easier for sure.)

Finding HTD5 gears on ebay 15t is easy, here's a 14t:
http://www.ebay.com/itm/8mm-Bore-5mm-Pitch-14-Teeth-15mm-Wide-Belt-Groove-3D-printer-Timing-Pulley-HTD5-/182419894192

(no keyway - just use grub and loctite blue)  Also aluminum so will wear out eventually.

12t (on 15mm still likely to skip unless you run an idler gear) - so not sure i recommend, but def drops speed down:
http://www.ebay.com/itm/HTD-5M-12T-16W-5-6-6-35-8mm-Bore-Pitch-5mm-Timing-Belt-Drive-Pulley-12-Tooth-/252478396028

The best resource i know for these, but expensive, is beltingonline.com in the UK.  Slow to ship and a not-inexpensive flat rate shipping... I think it was 25GBP for shipping last batch i got. But you can get good gears exactly as you want setup.  Oddly not seeing 13t...
12t:
http://www.beltingonline.com/12-tooth-htd5-pulley-12-5m-15f-7708
(adding 8mm bore, dual grub 3mm, 3mm keyway etc = ~$14 before shipping)
(again i'd only run 12t if idler gear to avoid skipping - even on 15mm)

14t (no 13t i could find 15mm wide):
http://www.beltingonline.com/14-tooth-htd5-pulley-14-5m-15f-7771
(about $15 before shipping)

Good, if expensive, options...

HTH - GL!
```

---
## \#5 Posted by: treenutter Posted at: 2017-07-02T00:32:25.247Z Reads: 91

```
@flywithgriff  I know that you asked about gearing efficiency, but if your problem is with overheating, the things that come to mind are increasing to 12S to pull less amps, or adding some thermal dissipation to your vescs. @chaka makes a heat sink kit for VESC 4.12. Not sure if you can buy it separately.
```

---
## \#6 Posted by: flywithgriff Posted at: 2017-07-02T00:34:23.481Z Reads: 87

```
I'm actually talking with him now. I just went 10s and don't have room or the extra cash to do a complete rebuild for 12s. I will adjust gearing and reduce amps untilnit works.
```

---
## \#7 Posted by: Pedrodemio Posted at: 2017-07-02T00:36:52.147Z Reads: 89

```
The thing is, efficiency is only part of the problem, what's you want to lower is current on the motor, since all loses is proportional to I^2, so as Benjamin say in his website, you want to have the motor producing the lowest torque. That is becouse torque is directly proportional to current, so the higher you gearing ratio is, the lower is the current needed to produce the same wheel torque

The simple way, gear for the lowest top speed you are comfortable with or drop motor Kv, Just be cautious about minimum teeth in contact and minimum belt bending radius
```

---
## \#8 Posted by: riverside.rider Posted at: 2017-07-02T01:36:35.859Z Reads: 72

```
http://www.electric-skateboard.builders/t/new-15teeth-pulley-5mm-pitch-for-belt-size-15mm-cheap-for-sale/25900
```

---
## \#9 Posted by: flywithgriff Posted at: 2017-07-02T01:39:18.559Z Reads: 69

```
Thanks man but I'm already running a 15mm drive pulley.
```

---
