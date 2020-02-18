# Help on this esk8 build

### Replies: 31 Views: 1213

## \#1 Posted by: Joakim1 Posted at: 2017-06-18T00:42:24.363Z Reads: 117

```
Hi all.
I've read a lot in here, and about many different builds.
So, i thought about you could help me with my build, and about if there misses something or something don't have to be there, and if it's good enough. I would like it to drive about 45-48 km/h. So pls tell if it does, and/or if i should change something so it get better:)

10s3p Battery.

HTD 5M 53 teeth Belt

HTD 5M 15 Teeth Steel Motor Pulley

HTD 5M 36 Teeth Nylon Carbon ABEC 11 FLYWHEELS Wheel Pulley

motor 6374 190Kv

12mm caliber trucks

Speed Controller (Maytech)

Bearings

Anti-Spark Switch

Nano Remote – V2

Wheels 90mm 75a

So again, pls let me know about all the things u want to say about this build.
```

---
## \#2 Posted by: Smorto Posted at: 2017-06-18T01:16:11.323Z Reads: 103

```
Looks good so far, however, that setup is only going to do around 41 km/h according to [this](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":90}|). The easiest way to get your 46km would be to go to a 12s pack, that is shown [here](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":12,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":90}|). You could also bump up speed a little bit by changing you gearing, well size, or motor kv. 

[quote="Joakim1, post:1, topic:25604"]
12mm caliber trucks
[/quote]

Do you mean 180mm trucks? Or 210mm trucks?
```

---
## \#3 Posted by: Joakim1 Posted at: 2017-06-18T01:30:01.843Z Reads: 87

```
What changes of the gearing do you mean exactly then, and what wheel size do u recommend then? :)
What's the best trucks? 180mm or 210mm?
```

---
## \#4 Posted by: jaymu86 Posted at: 2017-06-18T02:31:26.252Z Reads: 86

```
Could go with a 230kv motor
```

---
## \#5 Posted by: Smorto Posted at: 2017-06-18T02:33:37.106Z Reads: 87

```
Honestly I would recommend exactly what you have but if you want more a little more speed you could go with a 16/36 gearing and crazy huge 107mm wheels if you want though they are expensive. 180mm trucks should be fine. Again, I think you will be more then happy with your current setup, but it is up to you.
```

---
## \#6 Posted by: Smorto Posted at: 2017-06-18T02:33:58.814Z Reads: 83

```
This with a VESC will blow it due to the ERPM limit.
```

---
## \#7 Posted by: Joakim1 Posted at: 2017-06-18T07:51:20.500Z Reads: 76

```
Okay. So when you say 16/36 gearing do you mean 16 teeth motor pulley and 36 teeth wheel pulley? and if so, is the 53 teeth belt fine then?
```

---
## \#8 Posted by: Joakim1 Posted at: 2017-06-18T07:52:01.967Z Reads: 78

```
So, my battery and motor and vesc would work great together with this setup?
```

---
## \#9 Posted by: i2oadsweepei2 Posted at: 2017-06-18T11:36:47.362Z Reads: 66

```
I think that 10s and 190 kv is ok and below the erpm limit. However I am not very well versed with the vesc yet. The motor mount you are going to use will determine the belt length. I have enertion mounts with 16/36 that use 265mm belts and torqueboards V4 mounts that use 255mm belts same ratio. At the moment those are the only two I have used.
```

---
## \#10 Posted by: BoostedBuilder Posted at: 2017-06-18T14:25:34.796Z Reads: 56

```
You could make a 18/36 gearing. That could give you speeds of up to 48km/h with your setup
```

---
## \#11 Posted by: Joakim1 Posted at: 2017-06-18T16:15:23.243Z Reads: 51

```
Okay, but what exactly does 18/36 mean? Sounds good if i can reach 48 km/h :slight_smile:
```

---
## \#12 Posted by: Joakim1 Posted at: 2017-06-18T16:16:52.022Z Reads: 49

```
Is the vesc bad or?
```

---
## \#13 Posted by: BoostedBuilder Posted at: 2017-06-18T16:17:42.771Z Reads: 46

```
18 teeth on the motor pulley and 36 teeth on the wheel pulley and you choose whatever width you prefer
```

---
## \#14 Posted by: BoostedBuilder Posted at: 2017-06-18T16:18:59.736Z Reads: 47

```
I believe a higher number on the motor pulley results in more speed while a lower number (such as 12T) will give you more torque.
```

---
## \#15 Posted by: Joakim1 Posted at: 2017-06-18T16:20:49.786Z Reads: 48

```
Yea, okay. That makes sense.
```

---
## \#16 Posted by: Joakim1 Posted at: 2017-06-18T16:21:56.175Z Reads: 47

```
Okay, then i think that if it is like that, imma go with 16 teeth. Then it goes around 42 km/h, and at the same time i get some torque which is great. :)
```

---
## \#17 Posted by: i2oadsweepei2 Posted at: 2017-06-18T16:47:54.639Z Reads: 48

```
No not at all. I come from a heavy rc background and chose Torqueboards 12s esc's for my first two builds because they are basically rc esc's with a modified firmware. Very simple and no issues. I own four of them. Just never owned a vesc before. However I just ordered a couple vesc x last week.
```

---
## \#18 Posted by: Joakim1 Posted at: 2017-06-18T17:33:21.685Z Reads: 43

```
ah, okay. I've heard that vesc is better than esc and thats propably why i'd like a vesc. But, i really don't know if it's true.
```

---
## \#19 Posted by: jaymu86 Posted at: 2017-06-18T18:37:43.598Z Reads: 43

```
 I thought as long it is under 60k it was ok 230kv with 10s is like 57k erpm
```

---
## \#20 Posted by: Smorto Posted at: 2017-06-18T18:59:55.444Z Reads: 42

```
Yes those gears an belt are correct. The belt does depend a bit on the motor mount you are using though as @i2oadsweepei2  mentioned. 

In theory they should work though Im not sure what motor you are using because you have just said 6374 190kv motor. Also Im not sure what the may tech speed controller is, I'm assuming it is the vesc which will be good.
```

---
## \#21 Posted by: Smorto Posted at: 2017-06-18T19:00:18.160Z Reads: 39

```
Yes, vesc is much better then car ESCs.
```

---
## \#22 Posted by: Smorto Posted at: 2017-06-18T19:02:02.480Z Reads: 39

```
230kv with 10s is over 60k, it is shown at 59,570 [here,](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":230,"system-efficiency":80,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":90}|) but this calculator using nominal voltage I believe which means at full voltage it will be above 60k.

190kv with 10s or 12s though is a great setup and balance of speed and tourqe.
```

---
## \#23 Posted by: Joakim1 Posted at: 2017-06-18T19:03:40.818Z Reads: 40

```
Okay good, thanks.

I'm using [this](http://eskating.eu/product/electric-skateboard-motor-6374-190kv/) motor and [this](http://eskating.eu/product/electric-skateboard-speed-controller-maytech/) vesc.
Soo :)
```

---
## \#24 Posted by: Smorto Posted at: 2017-06-18T19:05:44.678Z Reads: 37

```
Yes those should work. Out of curiosity, have you ever ridden skateboard/longboard before?
```

---
## \#25 Posted by: Joakim1 Posted at: 2017-06-18T19:07:15.264Z Reads: 35

```
Yea. I have a Yuneec E-GO skateboard right now. But it's just started to be too slow for me.. It was very fun at start, but it started to feel more boring to ride it.
```

---
## \#26 Posted by: Smorto Posted at: 2017-06-18T19:12:48.296Z Reads: 36

```
Makes sense, just so you know though, the max of speed of around 12mph of that and the 30mph that you are looking to get out of this board are completely different. I think you are fine to start out with 10s, 190kv, 16/36, 53 tooth belt. These should get you about 25+mph and can also be upgraded later if you need more speed.
```

---
## \#27 Posted by: Joakim1 Posted at: 2017-06-18T19:15:59.483Z Reads: 37

```
Yea i know. I've tried one of my friends board (koowheel) which go around 25 mph, and thats wayyy more fun :)
But thanks for the help. Do you have any places to buy from which is good and not too expensive? My build i have found right now cost about $1000. And thats a lot over my budget..
```

---
## \#28 Posted by: Smorto Posted at: 2017-06-18T19:25:31.496Z Reads: 33

```
At hobby king you can get an sk3 192kv 6374 motor for around 70 or 80 usd I believe. Where are you getting everything else? There might be a few places to make things a bit cheaper.
```

---
## \#29 Posted by: Joakim1 Posted at: 2017-06-19T18:13:39.321Z Reads: 25

```
I'm getting everything from [this website](http://eskating.eu/).
```

---
## \#30 Posted by: Smorto Posted at: 2017-06-19T20:28:31.812Z Reads: 23

```
Hmm, I would search hobby king and http:// to see if you can cut costs a little.
```

---
## \#31 Posted by: Joakim1 Posted at: 2017-06-21T15:06:09.615Z Reads: 20

```
Okay, i''ll try it. TY
```

---
