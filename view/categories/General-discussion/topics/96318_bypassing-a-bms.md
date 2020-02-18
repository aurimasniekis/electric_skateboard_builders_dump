# Bypassing a BMS

### Replies: 16 Views: 342

## \#1 Posted by: xatonic Posted at: 2019-06-10T22:46:16.575Z Reads: 118

```
Hey guys I've been building my board and I almost have the battery fully welded so I'll start wiring everything up soon and I wanted to clear up my situation with my bms. I am using a 12s3p 25r pack which can put out a constant current of 60a and my bms is rated up to 60a, it feels like I'm pushing to it's limit so I want to bypass the bms for discharge. What are the cons to this? Because I can't find much about it, and does this wiring diagram look right for doing it? Is there a simpler way?![15602067267073373237402133049229|236x500](upload://eY3by1HA10rS5zq7f7cfnL06Ebi.jpeg)
```

---
## \#2 Posted by: Flasher Posted at: 2019-06-11T00:03:28.909Z Reads: 107

```
Still second guessing yourself?
```

---
## \#3 Posted by: xatonic Posted at: 2019-06-11T00:31:49.894Z Reads: 104

```
I'm worried, I don't want anything to go wrong🤣
```

---
## \#4 Posted by: Jinra Posted at: 2019-06-11T00:54:47.402Z Reads: 101

```
Looks okay, even if you discharged through your BMS, you'd likely never trip it. Your charge fuse seems too high too, what do you plan on charging at?
```

---
## \#5 Posted by: Flasher Posted at: 2019-06-11T01:10:41.040Z Reads: 97

```
Im about to push 130 amps through mine (12s5p p26a) and my wiring is the same as yours. Only differences are the hardwares. Also, as @Jinra asks, what charger are you using to need that big of a fuse?? 15a will never trigger and if it does, chances are you fried an egg on top XD
```

---
## \#6 Posted by: Jinra Posted at: 2019-06-11T01:18:02.854Z Reads: 91

```
at 15a I bet the charging wires will fuse out before the actual fuse depending on wire thickness
```

---
## \#7 Posted by: Flasher Posted at: 2019-06-11T01:22:24.752Z Reads: 80

```
Yeah theres a chance that'll happen too :slight_smile: I use a simple charger with a replaceable fuse on the side so I have no use for one in my wiring. And as an added measure my wires are 8awg on batteries and 10awg in motors XD just in case I decide to be stupid or cops try to catch up to me
```

---
## \#8 Posted by: xatonic Posted at: 2019-06-11T01:58:38.348Z Reads: 65

```
I'm running 10awg everywhere except for the balance wires, motor wires, and possibly the stock input wires on the focbox (might swap it out if I have some wire on hand). I got the 15a fuse because that's what the bms is rated for (https://bmsbattery.com/bmspcm/833-16889-smart-bms-10s13s-60a-with-blue-tooth-android-or-ios-app.html#/16-battery_type-lifepo4/107-cells_in_series-10) but since I'll only be charging at 8a I may uer a 10a fuse instead
```

---
## \#9 Posted by: xatonic Posted at: 2019-06-11T02:00:45.532Z Reads: 66

```
Do you guys think bms bypassing is necessary?
```

---
## \#10 Posted by: Jinra Posted at: 2019-06-11T02:29:57.735Z Reads: 62

```
Id try a 5a fuse first. Fuses actually take a long time to blow at their rated current and you won't be charging for excessively long anyway. But 10 is fine too.

You don't have to bypass discharge, but i personally would get a smaller bms and bypass.
```

---
## \#11 Posted by: adammunich Posted at: 2019-06-11T08:33:18.622Z Reads: 53

```
Find the big resistor that is used to measure the current from the BMS (often a thick metal bar) and reduce its resistance. It is a linear function, so half the resistance, will give you twice the current. 

If the MOSFETs get too hot after that, replace them with MOSFETs that have a lower RDs(on) value --you can find this in their data sheet. Or throw a hunk of aluminum and a fan on there, either solution works.

Please don't "bypass" this feature, it would be a great way to kill your batteries if you discharge them too low.
```

---
## \#12 Posted by: janpom Posted at: 2019-06-11T11:38:02.686Z Reads: 50

```
Looks good. :+1:

Regarding bypassing the BMS, it depends on how you ride and what board is that. With 12S and a single drive, I think you would have to ride extremely aggressively to get above 60A. I personally get close to 60A battery amps but not above with 10S and dual drive. This is on a street board.  

Do you have anything you can use for measuring your max battery amps while riding, such as the Metr module? If you do, then maybe best start with the bypassed BMS and you could later change it to discharge through BMS if you find out you don't get over the 60A.
```

---
## \#13 Posted by: xatonic Posted at: 2019-06-11T13:45:24.077Z Reads: 37

```
doesn't the focbox have a voltage cutoff feature?
```

---
## \#14 Posted by: xatonic Posted at: 2019-06-11T13:45:50.608Z Reads: 34

```
ok thanks for the reassurance!
```

---
## \#15 Posted by: adammunich Posted at: 2019-06-11T17:31:11.192Z Reads: 30

```
The voltage cut off feature of the FOCbox is only possible when the mircocontroller is ON --it has to wake up and measure the voltage then shut off. I don't believe it even shuts off properly, so you'll still have 20mA burning your batteries when empty. 

In principle it COULD work this way, but I have not seen evidence of them using STM32 low-power modes.
```

---
## \#16 Posted by: Jinra Posted at: 2019-06-11T17:35:33.920Z Reads: 30

```
the LVC doesn't even shut off the VESC it simply reduces power output when it hits it. Even if you hit end LVC you can still turn the motors when on the bench, it just won't really move if you stand on it.
```

---
