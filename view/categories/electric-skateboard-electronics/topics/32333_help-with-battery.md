# Help with battery

### Replies: 16 Views: 1072

## \#1 Posted by: TeslaAlex Posted at: 2017-09-05T14:56:10.633Z Reads: 111

```
Hi, I recently made a topic about my board stopping when I accelerate too fast. With some of you guys answers and some reading on the forum I think has to do with voltage sag. Yeterday I installed a voltage meter, and noticed that the voltage went from 100 % to 70% when I went up a kind of flat hill... It seems like alot! 

At the moment I have 2x 5000 mAh 20C lipo´s = 100A output. I was wondering if I should buy another pair of those batteries to get a 10 000 mAh battery = 200A output. Would this solve my problem?
```

---
## \#2 Posted by: willpark16 Posted at: 2017-09-05T15:01:08.531Z Reads: 109

```
It could just be ur liposhow old are they?
```

---
## \#3 Posted by: mmaner Posted at: 2017-09-05T15:01:41.074Z Reads: 107

```
20c is pretty light for an electric skateboard.  If you have the room do as you asked, just create a n identical pack and put it in parallel to the first pack.  If you dont have the room, look at the 60c lipo packs...

https://hobbyking.com/en_us/turnigy-heavy-duty-5000mah-3s-60c-lipo-pack-w-xt-90.html?countrycode=US&gclid=CjwKCAjwlrnNBRBMEiwApKU4PKIgCZDCQMxPwh9osz0xJqpE6JA62LU5d8OGCsUjV7O6jvL_F4NF4hoCnjUQAvD_BwE&gclsrc=aw.ds
```

---
## \#4 Posted by: TeslaAlex Posted at: 2017-09-05T15:25:34.360Z Reads: 91

```
They are like new, only been used for about 25km or so.
```

---
## \#5 Posted by: TeslaAlex Posted at: 2017-09-05T15:28:28.287Z Reads: 86

```
Ok nice! I will have to build a new enclosure but thats fine with me! And you are sure that it will solve my issue (or at least make it better)?
```

---
## \#6 Posted by: mmaner Posted at: 2017-09-05T15:29:42.337Z Reads: 84

```
I'm not sure, havent seen the board or the build.  Just KNOW that 20c is light and its logical that the board would sag with that amount of AMP delivery.
```

---
## \#7 Posted by: TeslaAlex Posted at: 2017-09-05T15:41:20.430Z Reads: 86

```
Ok, thanks. 
I have this motor and esc:
Ntm Propdrive v2 270
X Car Beast Esc 120A
```

---
## \#8 Posted by: Namasaki Posted at: 2017-09-06T06:17:19.453Z Reads: 71

```
[quote="TeslaAlex, post:7, topic:32333"]
I have this motor and esc:
Ntm Propdrive v2 270
X Car Beast Esc 120A
[/quote]

There are a couple things here.
(First) 20C is too low of a C rating as @mmaner said and don't believe that those batteries can really handle 100a continuous. Lipo C ratings are more of a relative than a real rating.
(Second) running only 6s your gonna pull a lot more amps than you would running 10s or 12s
(Third)  car esc's unlike the vesc operate in duty cycle mode which means that the voltage is controlled by the throttle and the current is determined by the amount of load in relation to the amount of voltage.
This makes car esc's much less efficient than a vesc which operates in current control mode and delivers full voltage at all speeds the current draw being controlled by the throttle.
Current control is more efficient because the more voltage you supply the less amps you need and the less amps you draw the less your battery sags and the longer it will take to discharge it.

I'm not an expert on motors but I believe the combination of low voltage and 270kv motor will be lacking in torque and could also contribute to higher current draw during hard acceleration or when climbing hills.
```

---
## \#9 Posted by: TeslaAlex Posted at: 2017-09-06T08:08:40.497Z Reads: 57

```
Thanks alot! This is exactly the info I was after, after all Im still a rookie regarding electric longboards. So what you suggest is that I should by a Vesc and a 10s battery? Would this work good with my 270kv motor? 

Im not super interested in spending alot of money at this build right now, maybe a bit more in the future. I really only want to fix the issue with the board stopping immediatly. Could I just by a couple of better rated batteries? Since other people has been using the same ESC without any problem, I dont feel like investing in a Vesc just yet. 

I was thinking to use 3x Turnigy 2s/5000mah/60c hard packs, and then buy another 2 to get to 10s and add a BMS when upgrading the whole board.  ([https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014](https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014)). =)
```

---
## \#10 Posted by: pat.speed Posted at: 2017-09-06T11:53:26.318Z Reads: 42

```
It could just be that your motor is pulling a lot of amps as it is a high kv and a little small. I have the same setup just with a 190kv motor and hardly see any voltage sag
```

---
## \#11 Posted by: TarzanHBK Posted at: 2017-09-06T12:00:14.998Z Reads: 39

```
If the board stops while under load you hit the max amps of the xcar beast.
On paper thats 120A, so at 6s about 2664W, which is a bit lower in reality.
Unfortunately the xcar doesn´t slow down, but brakes hard when he reaches it´s limit.
That´s the only bigger downside on that thing.
I´m running the 150A version of the Xcar and reached these levels too while going up a huge hill.
```

---
## \#12 Posted by: TeslaAlex Posted at: 2017-09-06T12:18:05.537Z Reads: 36

```
Thank you, nice to finally know whats causing my problem! Should I buy another motor that doesnt draw as much amps? Whats do you think?
```

---
## \#13 Posted by: TarzanHBK Posted at: 2017-09-06T13:10:43.407Z Reads: 36

```
I would leave it as it is.
Important are good batteries able to deliver the juice you want.
If it bothers you, buy another xcar and and motor and go for a dual drive.

But like i said, i would leave it like it is. If you wanna upgrade, take the 10s vesc route with a nice 6374 190 kv motor.
All other minor upgrades are not worth it in my opinion.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-09-06T13:39:53.106Z Reads: 33

```
270kv is too high with Vesc and 10s. 
190kv with Vesc and 10s is a good dependable combo. 
You could just upgrade your batteries for now and see if that will suffice
```

---
## \#15 Posted by: TeslaAlex Posted at: 2017-09-06T13:52:29.494Z Reads: 30

```
Ok, I think I will wait with any upgrades then. Maybe I could buy a ampere-meter so that I could monitor my amps? That way, I would be able to see how much I can pull the trigger without the ESC braking.
```

---
## \#16 Posted by: Benjamin899 Posted at: 2017-09-06T14:56:57.294Z Reads: 27

```
Hey i have a similar question. You recommend a higher C rating since most batteries can't deliver exactly what is written on them, meaning LiPo. So what C rating with 6s as max and a 120A Car ESC would you recommend.
```

---
