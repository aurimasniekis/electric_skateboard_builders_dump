# Does the cheap eBay esc have regenerative breaking?

### Replies: 17 Views: 1518

## \#1 Posted by: Orin635 Posted at: 2017-10-08T22:50:23.116Z Reads: 142

```
Hi,
Does anyone know if thowse cheap eBay esc have regenerative breaking?
https://m.ebay.com.hk/itm/322688412411?varId=511729893110&_mwBanner=1

I asked the seller and this was his answer <img src="/uploads/db1493/original/3X/1/b/1b294e8b29bf60dfb962f1973df0bdce393a10d9.png" width="281" height="500">
```

---
## \#2 Posted by: darkkevind Posted at: 2017-10-08T23:07:13.978Z Reads: 130

```
Yes it does.
```

---
## \#3 Posted by: Orin635 Posted at: 2017-10-08T23:08:45.260Z Reads: 130

```
Does it work well? Also what if your on 100% battery
```

---
## \#4 Posted by: darkkevind Posted at: 2017-10-09T06:38:43.211Z Reads: 112

```
It's had some very good reviews from fellow builders.

The cut out problem you're referring to relating to being at 100% charged (or there abouts), has nothing to do with your ESC, it's the BMS that would cut out to protect the battery from being overcharged....
```

---
## \#5 Posted by: Orin635 Posted at: 2017-10-09T06:53:50.575Z Reads: 110

```
What if I am not using a bms in my build or am only using it for charging?
```

---
## \#6 Posted by: pat.speed Posted at: 2017-10-09T06:56:30.213Z Reads: 106

```
I've heard that the esc stops charging when the battery is full and the brakes will just become weaker
```

---
## \#7 Posted by: Orin635 Posted at: 2017-10-09T07:09:08.035Z Reads: 103

```
That's what I thought it did
```

---
## \#8 Posted by: Crossfire Posted at: 2017-10-09T07:15:25.044Z Reads: 100

```
Charging li-ions to like 4.10 - 4.15 will compensate for that. I ride without BMS, always balance charge with my hobby charger and it's great.
```

---
## \#9 Posted by: darkkevind Posted at: 2017-10-09T08:31:27.477Z Reads: 96

```
If you're only using your BMS for discharge then the ESC will continue to charge your batteries whether they are full or not, you could end up with them being overcharged but it's very very unlikely unless you're going down a hill for about 1 mile or more and continually braking.
```

---
## \#10 Posted by: pat.speed Posted at: 2017-10-09T08:39:37.161Z Reads: 94

```
The esc will stop charging when the batts reach a certain level
```

---
## \#11 Posted by: darkkevind Posted at: 2017-10-09T08:42:03.089Z Reads: 89

```
Not if there's no software to limit it, or are you speaking from experience?

Thing is, if the motor's producing electricity, that current has to go somewhere.... If it doesn't go to the battery, and there's no where for it to go, it may just fry the ESC.
```

---
## \#12 Posted by: Crossfire Posted at: 2017-10-09T08:52:23.970Z Reads: 84

```
From practical experience I've found out that usually the corelation between VESC charging and discharging Ah or Wh is around +-10% - meaning if I've drawn 1Wh of energy from the battery, 0.1Wh goes back with regen braking. That's on mostly flat terrain, no big hills up or down, just a few slopes here and there.
```

---
## \#13 Posted by: Orin635 Posted at: 2017-10-09T09:09:15.475Z Reads: 83

```
So bassicaly not charge to 100% maybe 90%?
```

---
## \#14 Posted by: pat.speed Posted at: 2017-10-09T10:02:35.178Z Reads: 79

```
The seller has said that the esc will stop the regen when the battery is full and that the brakes will just become weaker
```

---
## \#15 Posted by: darkkevind Posted at: 2017-10-09T10:03:37.322Z Reads: 77

```
Ah, I see. I wasn't aware of that. Thanks :thumbsup:
```

---
## \#16 Posted by: Crossfire Posted at: 2017-10-09T10:14:39.302Z Reads: 77

```
It depens on your terrain...the only scenario which could be a bit of a worry is a steep hill down slope while fullly charged at 4.2V per cell at the start of your ride. If you're like 4.10-4.15V per cell instead of 4.20V I wouldn't bother. Interestingly, my charger won't even let me charge past 4.15V per cell in li-on mode. 

To charge the batteries for 0.1V per cell using regen in 3P or 4P configuration which could overcharge the batteries at the start of the ride is pretty unlikely. Usually we use our boards for everything else than for steep downhills anyway. :)
```

---
## \#17 Posted by: Orin635 Posted at: 2017-10-09T10:15:23.098Z Reads: 73

```
Ok thanks for the help guys
```

---
