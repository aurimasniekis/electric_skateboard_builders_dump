# LiPo Built In/BMS Charging?

### Replies: 14 Views: 1901

## \#1 Posted by: cryzies Posted at: 2016-09-25T10:14:11.112Z Reads: 156

```
I might have to go the budget route and do 3x4s (or 6x4s) LiPos. I'm trying to achieve built in charger like the Boosted Board v2. Where you just have the power supply to plug into the BMS. Is that possible with LiPos? Have it wired in series for 12s1p or 12s2p for output but wired in 4s3p or 4s6p for charging? How would this work? Couldn't find much info, if anyone have any links that'd be great. At the end of the day I don't want to remove my batteries to charge.
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-25T10:31:25.462Z Reads: 151

```
Why do you want to charge in 4s? Just charge in 12s if you want to use a bms. @namasaki did this recently in his build
```

---
## \#3 Posted by: cryzies Posted at: 2016-09-25T10:32:51.941Z Reads: 150

```
It'd be much cheaper and safer to charge in 4s though right?
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-25T10:46:09.794Z Reads: 147

```
it's no safer or more dangerous if you get a quality bms such as Batterysupports.com. And BMS's are fairly affordable at ~$40

I bought a $20 bms for 10s myself, but I'm not planning to use it for discharging.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-09-25T16:56:49.465Z Reads: 127

```
[quote="cryzies, post:3, topic:10117, full:true"]
It'd be much cheaper and safer to charge in 4s though right?
[/quote]

I agree with @Jinra 
A quality BMS will balance charge your pack just as good as any balance charger.
I'm using a Bestech BMS. 
I believe that They keep the pack balanced during charge and discharge as well. 
I will be testing that theory shortly.
I'm guessing that battery supports BMS will do the same. 
Both of these brands are proven to be a quality product.
```

---
## \#6 Posted by: Jinra Posted at: 2016-09-25T21:55:09.131Z Reads: 111

```
balancing only happens during the last few decimal points of charging. However, discharging through a BMS will prevent invidividual cells from dropping below a certain voltage as well.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-09-25T22:47:24.064Z Reads: 99

```
It is now thought that certain bms's keep the batteries balanced continually. I am going to test the theory by discharging my pack and then checking individual cell voltages to see if there the same.
```

---
## \#8 Posted by: Jinra Posted at: 2016-09-25T22:48:24.682Z Reads: 94

```
Make sure you test without a BMS as well. AFAIK, cells don't stray much of a couple discharges. They stray over time.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-09-25T23:27:29.232Z Reads: 93

```
I did think about that. even without balance discharge they only vary slightly.
When balanced, they will be exactly the same. I figure if balancing is in fact being done continually, then once discharged, every cell should show exactly the same voltage.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-10-01T00:19:21.564Z Reads: 75

```
Just checked individual cells to see if BMS is balancing during discharge.
After full balance charge to 42v. I ran it down to 37.8v and here are cell voltages:
01:  3.78
02:  3.79
03:  3.78
04:  3.80
05:  3.78
06:  3.79
07:  3.79
08:  3.79
09:  3.79
10:  3.79
Does this look like balance discharge or just normal discharge?
Or normal discharge with good quality cells?
```

---
## \#11 Posted by: Jinra Posted at: 2016-10-01T00:31:46.381Z Reads: 70

```
Looks normal discharge to me. But i think it's hard to be sure unless you repeat it over a bunch of cycles without using a bms. Easiest way is to probably ask the manufacturer though.
```

---
## \#12 Posted by: Namasaki Posted at: 2016-10-01T00:37:12.629Z Reads: 69

```
Either way, the cells are discharging very close to each other. Probably because they are quality packs.
I think it would be safe to take the total pack voltage down to 34v maybe even 32v Especially since the voltage sag is like 1volt or less going up hill.
What do you think?
```

---
## \#13 Posted by: Jinra Posted at: 2016-10-01T01:41:06.036Z Reads: 66

```
voltage sag aside i think lipos shouldn't go below 3.6v. You'll have to check the datasheet for your lipos
```

---
## \#14 Posted by: Namasaki Posted at: 2016-10-01T01:46:13.009Z Reads: 65

```
I had 2 Venom 6s Lipo packs. It said right on the pack that min voltage was 18v so 3v per cell.
I used to run my Zippy Lipos down to 3.4
Funny thing is the Venom Lipos had much higher internal resistance than the Zippys.
```

---
