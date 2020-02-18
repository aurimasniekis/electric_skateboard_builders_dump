# 12S3P Battery config Vs. 10S4P Battery config performance difference

### Replies: 25 Views: 4751

## \#1 Posted by: davey8 Posted at: 2016-09-17T12:42:44.060Z Reads: 617

```
Can anyone break this down in layman's terms? What's the performance difference between a 12S3P battery configuration, and a 10S4P battery configuration?  How do they compare in range, speed, and torque?
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-09-17T12:56:31.158Z Reads: 615

```
With a 12S3P you'll get more speed and less range.
With a 10S4p you'll get more range and less speed.

In most cases, we're talking about 18650 batteries, so it would be 2500mah more using a 10S4P. I personally would go with the 10S4P, because:

- I like the range
- I don't like running 12S
-I prefer 10S... It seems to take less of a toll on the electronics, but that's just my opinion on the VESC

The disadvantage is you need more cells than a 12S3P... And the speed sacrifice, but the sacrifice can be made up for if you use a different motor/gearing/wheels.
```

---
## \#3 Posted by: davey8 Posted at: 2016-09-17T13:17:08.387Z Reads: 594

```
Does torque suffer with the 12s setup too?
```

---
## \#5 Posted by: Jinra Posted at: 2016-09-17T13:35:08.843Z Reads: 583

```
Torque is dependent in amount of copper on the stator, so running a higher voltage should have little to no effect on torque. Though running a lower voltage can bottleneck the wattage supplied for the motor.
```

---
## \#6 Posted by: Namasaki Posted at: 2016-09-19T04:33:59.851Z Reads: 542

```
I have run 12s and 10s 
12s Lipos with 230kv motors and TB Esc
10s Li-ions with 190kv motors and TB Esc

The 12s produced noticeably faster acceleration 
and throttle response, higher top speed. 
It feels like it has more torque. 

The 10s was much smoother and more controllable 
 
I think if your wanting to build a reasonably reliable board with good but manageable performance, then I would recomend 10s.
```

---
## \#7 Posted by: pigeonic Posted at: 2016-12-10T03:39:51.591Z Reads: 474

```
I'm sorry for being an idiot about this. and jumping on to this thread, because I'm now terribly confused the S and P terms??? I've read some post where they mentioned S=Series while some mentioned S=Cells, and P=Parallel. I know as much as connecting in Series increases voltage and connecting in parallel increases its capacity?? Pls help. On the verge of dying just from finding out what type(kinds?) of batteries fit which type of motor. just for further info, I'm living in singapore, from what I have seen, 30C packs with 1800/1500mah is terribly common here. motors with 300/400kv on 1500w(maybe lesser). I'm 76-81kg, which is about 168-178lbs. kind of a big range, but I'm recovering from a 1-2month long sickness. Appreciated if this can be helped!! Just to put more details. Wheels 83mmm fly, 50deg Caliber II trucks
```

---
## \#8 Posted by: Tuomalar Posted at: 2016-12-10T03:54:52.957Z Reads: 445

```
For example 10s4p = 10 in series 4 in parallel ->  you have 4x samsung r25 2500mah in parallel which means 1s4p (3.6V/10000mah) then you put ten of these 1s4p in series and now you have 10s4p (36V/10000mah).

And read this http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983
```

---
## \#9 Posted by: pigeonic Posted at: 2016-12-10T04:28:47.210Z Reads: 427

```
This is assuming its 1 cell?
```

---
## \#10 Posted by: pigeonic Posted at: 2016-12-10T04:33:32.076Z Reads: 416

```
wait. dont reply to that. I feel like an idiot, I got it
```

---
## \#11 Posted by: pigeonic Posted at: 2016-12-10T09:11:41.592Z Reads: 399

```
Actually, how many batteries does 10s4p require? and, if I use enertion's space battery, would it be compatible with my motor? The current motor I have in hand, is O.S. Motors OMA-5025-375kv
```

---
## \#12 Posted by: Tuomalar Posted at: 2016-12-10T10:26:33.930Z Reads: 378

```
That motor is waaaaay too small and too hi kv. 
And 10s4p = 10x4 cells = 40 cells

But at first you should read this forum thru and then you know everything you need to know.
```

---
## \#13 Posted by: pigeonic Posted at: 2016-12-10T10:34:56.219Z Reads: 376

```
Honestly, I've been reading through it countless of times. Still don't get lots of things. If you say the motor is small, what would you recommend? (Affordable, not into enertion yet)
```

---
## \#14 Posted by: Tuomalar Posted at: 2016-12-10T10:44:23.861Z Reads: 370

```
6355, 6374, 5065 these are most common sizes. And KV variates depending you esc/vesc and battery. For you sk3 would be good. 6374 190kv, vesc and 10s3-4p
```

---
## \#15 Posted by: pigeonic Posted at: 2016-12-10T10:48:41.933Z Reads: 362

```
ah okay. clears up loads of things. Thanks!
```

---
## \#16 Posted by: Spencermiller Posted at: 2017-01-03T03:57:04.490Z Reads: 330

```
How did you come to the conclusion that the 10S causes less wear & tear on the VESC?  Is it from something you read or personally experienced?
```

---
## \#17 Posted by: Kabby450 Posted at: 2019-10-20T16:01:44.512Z Reads: 54

```
What is the TB esc
```

---
## \#18 Posted by: pjotr47 Posted at: 2019-10-20T20:21:11.446Z Reads: 54

```
Lol this topic is 3years old...
```

---
## \#19 Posted by: Namasaki Posted at: 2019-10-20T20:56:48.863Z Reads: 53

```
The TB esc was an old school 12s 120a car esc that we used before the Vesc was available.
It worked ok but it's performance was not even close to even the earliest version of Vesc and in reality it could not really handle 12s or 120a.
I ran two of them on my first build.
![59%20PM|583x291](upload://63xAuRgy39Xca6PFsYdEXpLIhKV.png)
```

---
## \#20 Posted by: Kabby450 Posted at: 2019-10-20T22:30:58.624Z Reads: 47

```
Thanks for getting back to me.  I’m building an AT using the backfire X2 rear wheel hub motor set.  I want to use 2 esc’s instead of a dual.  Would you have a recommendation.  I plan on using 10S4P.
```

---
## \#21 Posted by: Kabby450 Posted at: 2019-10-20T23:53:13.479Z Reads: 45

```
Your point.....
```

---
## \#22 Posted by: Namasaki Posted at: 2019-10-21T04:59:17.502Z Reads: 42

```
Would definitely NOT recommend any CAR ESC.
I would only recommend something based on Vesc design.
I have been running Ollin 4.12 Vescs for years without any problems.
I paid about $180 ea. for mine a couple years ago and now they are selling a new and improved version for only $169.95 ea.
https://www.ollinboardcompany.com/product/direct-fet-vesc-v4-12
```

---
## \#23 Posted by: Sn4pz Posted at: 2019-10-21T06:48:33.877Z Reads: 42

```
When are they going to sell a vesc 6 version 🤔🤔
```

---
## \#24 Posted by: Kabby450 Posted at: 2019-10-21T12:05:44.449Z Reads: 42

```
Just checked them out.  They look “bulletproof”!  Sn4pz mentioned a VESC 6.  I’m new too this can you tell me the difference between the 4.12 and 6.
```

---
## \#25 Posted by: murdomeek Posted at: 2019-10-21T19:12:10.358Z Reads: 36

```
4.12 is old tech but cheap and reliable (you can get them for $50usd on aliexpress)

6.x is newer design, nearly bulletproof, more expensive
```

---
## \#26 Posted by: Namasaki Posted at: 2019-10-22T04:45:06.691Z Reads: 34

```
I have never bought any from Aliexpress and I wonder how dependable they are.
In the past few years, there have been many reports about cheap 4.12 Vescs being very undependable because they don't have much needed upgrade components and heat sinks.
With Ollin Vescs, you get quality components and heavy duty heatsinks.

If my memory serves me, Ollin was the first company to produce quality Vescs.
Later the Focbox came out and in my opinion, it was also a good quality Vesc.
Then the Vesc 6 came out and brought it to a whole new level.
```

---
