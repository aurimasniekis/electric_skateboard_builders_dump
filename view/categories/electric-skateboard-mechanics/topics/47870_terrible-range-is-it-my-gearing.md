# Terrible range - is it my gearing

### Replies: 25 Views: 1147

## \#1 Posted by: pat.speed Posted at: 2018-03-01T20:50:05.066Z Reads: 216

```
Hi guys

So I've been riding around on my board now for about  a month or two and it's been great fun except for having to go home early. 

My problem is I'm only getting about 5km range on 1 battery (I have two batteries). Each battery is 6s 5000mah 20c. Now I can't figure this out because I should at least be getting something close to 10km for a 111Wh battery.

With the current range I'm getting this puts me at around 20wh per km which is very high for a street board. I also connected my batteries into series and went for a ride this time I only got 4, maybe 6km if I went really low. What is happening here( this could be because I was riding at about 50kmh but still that's like 40wh per km)


So my main question is, is it my gearing? I'm running dual 6355 195kV with a 14:27 gear ratio and 97mm wheels.
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-03-01T20:51:41.601Z Reads: 209

```
have you checked voltage cut?
```

---
## \#3 Posted by: pat.speed Posted at: 2018-03-01T20:51:42.726Z Reads: 206

```
Edit: I meant 14:27 gearing
```

---
## \#4 Posted by: pat.speed Posted at: 2018-03-01T20:52:05.943Z Reads: 202

```
Yep, I'm cutting off around 3.7 -3.8v
```

---
## \#5 Posted by: onepunchboard Posted at: 2018-03-01T20:52:16.523Z Reads: 196

```
wow the gearing is too much
```

---
## \#6 Posted by: onepunchboard Posted at: 2018-03-01T20:52:34.204Z Reads: 194

```
u should cut at 3.2-3.3
```

---
## \#7 Posted by: ZackoryCramer Posted at: 2018-03-01T20:52:50.202Z Reads: 192

```
50kmph is definitely part of the inefficiency. I get over 20wh/mile efficiency at 27mph
```

---
## \#8 Posted by: GrecoMan Posted at: 2018-03-01T20:56:56.384Z Reads: 188

```
yea that’s your problem. lower that to 3.5, 3.4v. the gearing is also REALLY inefficient but isn’t the main reason
```

---
## \#9 Posted by: ZackoryCramer Posted at: 2018-03-01T21:04:09.703Z Reads: 181

```
I cut at 3.6 on my lipos and I get the full ah brotha. 🧦
```

---
## \#10 Posted by: pat.speed Posted at: 2018-03-01T21:04:24.970Z Reads: 182

```
Ok thanks guys @GrecoMan @onepunchboard @ZackoryCramer

I have two new 10t sprockets on the way. That way I'll have a 1:2.7 ratio (hella torque). I will also try lowering my cut off, I just have it so high to max the life cycles of my cells
```

---
## \#11 Posted by: pennyboard Posted at: 2018-03-01T21:09:17.542Z Reads: 174

```
I have my cutoff start at 3.2 and end at 3.0 and my batteries have over a year on them (12s 5000 mah lipos so just like yours), and they’re fine. 
With lower gearing and cutoffs you should see 10-14 miles range depending on weight and riding style
```

---
## \#12 Posted by: GrecoMan Posted at: 2018-03-01T21:09:18.626Z Reads: 166

```
lol that’s not possible 🤣
```

---
## \#13 Posted by: mmaner Posted at: 2018-03-01T21:13:15.372Z Reads: 163

```
The general (and I use the term loosely) accepted cutoff for LIPO's is 3.4.  Geering is a lot of your problem, I would go 15/32 at a minimum.
```

---
## \#14 Posted by: pennyboard Posted at: 2018-03-01T21:16:27.794Z Reads: 160

```
I know for lipos, it’s a little higher cutoff than lions but I still think you can get away with 3.1 volts per cell. Although more to your point, you gain very little range from 3.4 to 3.1 volts because it drop so fast between the 2. So setting to 3.1 volts doesn’t really gain you much
```

---
## \#15 Posted by: louwii Posted at: 2018-03-01T21:23:31.612Z Reads: 151

```
It also can be dangerous for your battery if you don't use a BMS for discharge. If your cells get unbalanced when discharging, you can have a cell got lower than 3.1V which ain't good.
```

---
## \#16 Posted by: pat.speed Posted at: 2018-03-01T21:24:38.981Z Reads: 141

```
Yeah I realise this, but so far all cells have stayed within .03v when discharging
```

---
## \#17 Posted by: pennyboard Posted at: 2018-03-01T21:25:38.265Z Reads: 136

```
Yeah I second this. Don’t be like me 😂. 
Make sure always use a BMS or balance charge
```

---
## \#18 Posted by: Acidfie Posted at: 2018-03-01T21:28:20.441Z Reads: 132

```
Cut-Off for Konion VTC5:

Pulsed: 5s On - 30s Off

Discharge Rate **PULSED**/Sag/Cut-Off (rec.)

30 / 0.6V / 3.2V
40 / 0.65V / 3.25V
50 / 0.75V / 3.35V
60 / 0.8V / 3.4V
70 / 0.85V / 3.45V
```

---
## \#19 Posted by: GrecoMan Posted at: 2018-03-01T21:29:48.774Z Reads: 124

```
he doesn’t even have 18650’s 🤣
```

---
## \#20 Posted by: Acidfie Posted at: 2018-03-01T21:31:47.341Z Reads: 124

```
its just a point of reference for people :rofl::rofl::rofl::rofl::rofl::rofl:
```

---
## \#21 Posted by: pennyboard Posted at: 2018-03-01T21:33:49.717Z Reads: 122

```
Technically 18650s can be drained all the way down to an absolute cutoff of 2.5 volts per cell without damaging them

However I don’t reccommend that for ebords, as if your software or hardware fails to cut off the battery quickly enough if you have voltage sag under load, you will damage the cells if they’re pulled below 2.5 volts
```

---
## \#22 Posted by: Namasaki Posted at: 2018-03-01T23:30:26.345Z Reads: 105

```
Your probably getting a lot of voltage sag with 6s/ 5000 / 20C especially with the gear ratio your running.
Your weight, wind resistance, riding style and riding conditions can have a lot to do with it as well.
```

---
## \#23 Posted by: ShutterShock Posted at: 2018-03-03T21:33:18.131Z Reads: 66

```
I second this, my cutoff start is 3.5, end 3.4
```

---
## \#24 Posted by: Acido Posted at: 2018-03-03T22:40:58.284Z Reads: 61

```
Im at 1:2 and get 20-25 miles and mostly im accelerating hard and breaking and im 100kg 
Single drive 6374
```

---
## \#25 Posted by: Acido Posted at: 2018-03-03T22:41:55.264Z Reads: 61

```
Bmss often cant go that low for some reason bestech can not go under 2.8 i think...
```

---
