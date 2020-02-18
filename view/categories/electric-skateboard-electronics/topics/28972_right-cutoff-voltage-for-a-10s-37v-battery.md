# Right cutoff voltage for a 10s 37v battery

### Replies: 31 Views: 2232

## \#1 Posted by: dg798 Posted at: 2017-07-28T20:53:49.730Z Reads: 268

```
what should i make the cutoff for a 37v battery
```

---
## \#2 Posted by: FredSaberhagen Posted at: 2017-07-28T20:55:04.021Z Reads: 268

```
3V/cell or 30V
```

---
## \#3 Posted by: dg798 Posted at: 2017-07-28T20:56:08.162Z Reads: 268

```
ok thank you
```

---
## \#4 Posted by: Achmed20 Posted at: 2017-07-28T20:57:02.034Z Reads: 268

```
3V seems allready very low.

most people here go with 3.3 - 3.2V tops
```

---
## \#5 Posted by: dg798 Posted at: 2017-07-28T20:57:17.004Z Reads: 266

```
i want to be safe but also i want to get the most out of my battery.
would it still be the same.
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-07-28T20:58:49.750Z Reads: 256

```
liion or lipo?
```

---
## \#7 Posted by: Achmed20 Posted at: 2017-07-28T20:58:58.014Z Reads: 249

```
are we talking about LiPo's or Li-Ion's?
```

---
## \#8 Posted by: dg798 Posted at: 2017-07-28T20:59:04.347Z Reads: 247

```
lipo battery
```

---
## \#9 Posted by: Achmed20 Posted at: 2017-07-28T21:00:54.058Z Reads: 246

```
then 3.4V to get the most out of them. 3.2 is allready borderline for them in terms of max charge cycles
```

---
## \#10 Posted by: thisguyhere Posted at: 2017-07-28T21:00:56.828Z Reads: 245

```
lower limit for lipos seem to be 3.2v to be safe and preserve longevity.

but, this is from my 10s balance charger manual:

<img src="http://www.electric-skateboard.builders/uploads/db1493/original/3X/5/d/5d8ef7ee2d4c242bb3df4a2006a3d872b6b124f3.png" />
```

---
## \#11 Posted by: thisguyhere Posted at: 2017-07-28T21:01:32.802Z Reads: 238

```
or what @Achmed20 said
```

---
## \#12 Posted by: dg798 Posted at: 2017-07-28T21:02:53.736Z Reads: 229

```
so 32v in total is good for maximum preformance and to also conserve the energy?
```

---
## \#13 Posted by: Achmed20 Posted at: 2017-07-28T21:04:11.783Z Reads: 217

```
i run mine down to 3.2V btw.
replacing them costs me like 60€ but i usualy have 40% left after a ride.
```

---
## \#14 Posted by: dg798 Posted at: 2017-07-28T21:04:54.770Z Reads: 211

```
ok thank you
```

---
## \#15 Posted by: thisguyhere Posted at: 2017-07-28T21:06:30.818Z Reads: 207

```
i don't feel comfortable advising on lipos, i've personally never used them.

i would go with a more conservative bottom cutoff at 3.4v, so 34v for your 10s pack, like @Achmed20 said. 

not sure about "maximum performance and to also conserve the energy."  it's more to extend the life of your batteries because draining them to their extremes is a great way to kill them prematurely.  and lipos are volatile in general so good to be conservative.

there's peopel here using lipos very successfully, may want to ask them (@Namasaki comes to kind).
```

---
## \#16 Posted by: dg798 Posted at: 2017-07-28T21:09:07.322Z Reads: 193

```
so what kind of battery would you recommend
```

---
## \#17 Posted by: Namasaki Posted at: 2017-07-29T01:11:12.409Z Reads: 178

```
If your gonna use Lipos, then I highly recommend getting Lipos with a high C rating.
I've been using 60/120C Lipos for long time and they are doing very well.
```

---
## \#18 Posted by: marcus Posted at: 2017-07-29T01:24:50.837Z Reads: 174

```
Mine as well
```

---
## \#19 Posted by: Sirshaunsta Posted at: 2017-12-28T23:18:48.191Z Reads: 134

```
Hey guys just wanna run something by the more knowledgeable members, if a lipo fully charged is 4.2v and fully discharged is 3v, running a 10s8p 20c 40 000mah battery would I be better off setting my cut off to 3.2 or 3.3? I will already have a huge range I just want to preserve cycle and charge life of my batteries
```

---
## \#20 Posted by: GrecoMan Posted at: 2017-12-28T23:22:05.034Z Reads: 129

```
set cutoff start to 34 and end to 32
```

---
## \#21 Posted by: Sirshaunsta Posted at: 2017-12-28T23:40:33.666Z Reads: 120

```
I love this guy @GrecoMan always well informed
```

---
## \#22 Posted by: Sirshaunsta Posted at: 2017-12-28T23:42:14.282Z Reads: 118

```
So 32 is safe for my batteries to maximize range and power with a healthy battery charge life?
```

---
## \#23 Posted by: GrecoMan Posted at: 2017-12-28T23:43:30.620Z Reads: 116

```
the chances that you'll run them that low is very slim.  the best way to increase the amount of charge cycles is to charge to 41v instead of 42v, that will double them and make up for discharging them "low" every now and then
```

---
## \#24 Posted by: Sirshaunsta Posted at: 2017-12-28T23:47:04.386Z Reads: 105

```
Perfect, by those numbers my board will hit 65 km at full charge 41 and 50km at 32 @GrecoMan with only 16/32 gearing. Faster if I go to 20/32
```

---
## \#25 Posted by: GrecoMan Posted at: 2017-12-28T23:48:57.189Z Reads: 101

```
cool :smile:

the 1v that you don't charge is only equal to about 5% of your actual "juice" since at that voltage, it will deplete way quicker than at 3.7ish when it evens out
```

---
## \#26 Posted by: Sirshaunsta Posted at: 2017-12-28T23:49:49.371Z Reads: 95

```
Awesome info man, thank you @GrecoMan
```

---
## \#27 Posted by: GrecoMan Posted at: 2017-12-28T23:50:37.831Z Reads: 93

```
damn I'm outta likes for today

pretend I liked that post :wink:
```

---
## \#28 Posted by: Sirshaunsta Posted at: 2017-12-28T23:56:10.648Z Reads: 86

```
Will do buddy, cheers @GrecoMan
```

---
## \#29 Posted by: Sirshaunsta Posted at: 2017-12-29T02:20:28.859Z Reads: 79

```
I think 16/32 will be a good place to start I will give an update when I have more parts
```

---
## \#30 Posted by: GrecoMan Posted at: 2017-12-29T02:23:44.910Z Reads: 77

```
16/32 is much better than 20/32.

I personally use 16/36 on 97mm wheels
```

---
## \#31 Posted by: Sirshaunsta Posted at: 2017-12-29T02:33:04.179Z Reads: 74

```
Yes my only concern is the belts fitting @GrecoMan
```

---
