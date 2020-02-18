# Single 4800w motor

### Replies: 22 Views: 513

## \#1 Posted by: ron.k Posted at: 2019-06-03T11:58:44.136Z Reads: 223

```
Hi,
I'm looking for a 4800W 160-190kv motor with 8/10 mm shaft .
I'll be happy if someone can send me a link if such a thing exists. 
Thank you :-)
```

---
## \#2 Posted by: nuttyjeff Posted at: 2019-06-03T12:03:59.901Z Reads: 221

```
I think you're just looking for a 6374/6380/63100 motor.. if that's the case, check out the motors from @torqueboards
```

---
## \#3 Posted by: ron.k Posted at: 2019-06-03T12:23:59.538Z Reads: 211

```
hi,
Not exactly ,I'm looking to upgrade my dual 6380 4100w bored to more powerful motors. 
Do you have anything in mind ? ( the strongest ones I could find  were 4600w).

Thanks 8-)
```

---
## \#4 Posted by: Andy87 Posted at: 2019-06-03T12:30:34.338Z Reads: 202

```
you could get 63100 from APS or step up to 80xx motors.

I´m sure you know that bigger motors will not always bring you more torque and power. your whole system need to be able t work together.

what´s your esc right now and if it´s a vesc based one, which motor and battery max/min values did you set them to?
```

---
## \#5 Posted by: torqueboards Posted at: 2019-06-03T12:31:29.236Z Reads: 189

```
You need a big battery or you’ll have a bottleneck.
```

---
## \#6 Posted by: nuttyjeff Posted at: 2019-06-03T12:49:19.700Z Reads: 182

```
Your max output will still be limited to your batts though.. Dual 4600watt motors = 9200watts of power..

Assuming no sag, a 12s lipo/liion batt would need to output 216A of current to reach your motor's rated peak power... Is your battery capable of that? Are your wires sized for those amps?

In any case, assuming you've sized everything appropriately, how about going for a 4wd with another 2x 6380s?
```

---
## \#7 Posted by: Kug3lis Posted at: 2019-06-03T13:18:23.920Z Reads: 164

```
How much current do you allow ur motor to consume in the first place? I doubt you even using 4100W...
```

---
## \#8 Posted by: Andy87 Posted at: 2019-06-03T13:20:49.904Z Reads: 161

```
i vote for max 1500W per motor on short intervals. probably even less.:sweat_smile:
```

---
## \#9 Posted by: Kug3lis Posted at: 2019-06-03T13:23:02.629Z Reads: 160

```
BTW Motor consumes as much current/power as it needs for that load... You can't just push more current into it :D I am running 6kW motors rarely see them to consume more than 2kW on avg
```

---
## \#10 Posted by: Hummie Posted at: 2019-06-03T14:07:25.649Z Reads: 148

```
Why don’t ur max setting get reached on full throttle.  Why doesn’t the esc increase the load by accelerating faster.
```

---
## \#11 Posted by: Kug3lis Posted at: 2019-06-03T14:23:21.222Z Reads: 140

```
I mean I get top peaks but on **avg** normal riding its near 2kW I can't sustain full throttle all the time, I mean you can't handle wheelies and crazy torque all the time
```

---
## \#12 Posted by: ron.k Posted at: 2019-06-03T14:40:19.281Z Reads: 134

```
Thank you everyone, super helpful.

The thing is that I also use my board to toe other people on skateboards so I need a bunch of torque. But yeah I usually only use something like 3000W combined.
```

---
## \#13 Posted by: Kug3lis Posted at: 2019-06-03T14:56:06.349Z Reads: 128

```
Change ur current settings
```

---
## \#14 Posted by: ron.k Posted at: 2019-06-03T15:09:35.061Z Reads: 127

```
6000w for a single or combined?
```

---
## \#15 Posted by: Kug3lis Posted at: 2019-06-03T15:15:07.201Z Reads: 126

```
Single, I am running 2 x 80100
```

---
## \#16 Posted by: banjaxxed Posted at: 2019-06-03T18:55:07.639Z Reads: 110

```
I’m interested in the 63100 with its giant stator and no room for a sensor board, with encoders for start up and smoothness, thinking the power vs weight could be way cool

Battle hardened of course
```

---
## \#17 Posted by: Andy87 Posted at: 2019-06-04T05:49:08.623Z Reads: 93

```
I can imagine battle harden is a pain in the a** 
They so long that you will have problems to reach the last corner.
```

---
## \#18 Posted by: banjaxxed Posted at: 2019-06-04T09:02:01.889Z Reads: 85

```
Remove the grubs holding the shaft and take it out, there is more room to manoeuvre? = easier?
```

---
## \#19 Posted by: Andy87 Posted at: 2019-06-04T09:10:41.218Z Reads: 84

```
that´s always a good idea, buuuut you know the grub screws like to strip ;)
```

---
## \#20 Posted by: banjaxxed Posted at: 2019-06-04T12:04:04.320Z Reads: 70

```
Only get one chance to harden the motor correctly, worth it? think so

Removal should be with a Hex plus key of course. It really does help so much. That and the hardened 12.9 grubs. Probably sensible to replace them if they show any sign of deformation.

If all else fail heat and a torx key

But you're the master of hard  :bowing_man:
```

---
## \#21 Posted by: Dirt_Bag Posted at: 2019-06-05T05:12:17.793Z Reads: 42

```
Are your old motors for sale?
```

---
## \#22 Posted by: evoheyax Posted at: 2019-06-05T05:37:21.978Z Reads: 37

```
Depends on how you use it. Every full throttle acceleration for me pulls a bit over 8000 watts for a few seconds. I have posted graphs from metr pro showing this. Now you can say that's not continuous, and it's not really, but it's the entire acceleration of 0-30mph which takes 2.8 seconds.

The battery, like said before, is he biggest bottle neck... My lipo pack is a 12s25ah monster I built to output 200a bat 480a motor between 4wd. You just have to be willing to build heavy. I'm at about 35lb with everything. Look for larger diameter motors.

Another cool idea is you can always build your own motors. Just have to order a few stators from china, wind them, and the right glue with the right parts you have machined.
```

---
