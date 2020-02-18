# Easy Maintenance Batterys - Drill, Li-ION - Graphite UK

### Replies: 18 Views: 1111

## \#1 Posted by: Timotay Posted at: 2019-01-03T18:21:40.685Z Reads: 119

```
Hey,

Im very new so please excuse my poor knowledge.

Im now on my 3rd Electric skateboard build and loving it, However I keep running into the same issues BATTERIES! 

I originally purchased 2 Lipos which have both now puffed up and started leaking, not great..

I want an easy battery system that I dont really need to take care of. Discharging putting them into storage ect. 

Is there any UK sellers that make LI ION battery packs with inbuilt XLR charging port and XT 90 Outputs?
(BMS on board)

I have also looked into drill batteries but I dont think they can deliver enough amps.

My board currently is using:

(I couldn't find my actual components so I have included similar ones)

ESC:
[UK X-car Beast Series ESC Brushless 1 8 Scale 120a](https://www.ebay.co.uk/p/UK-X-car-Beast-Series-ESC-Brushless-1-8-Scale-120a/14012479120?iid=162835176520&chn=ps)

Motor:
Turnigy Aerodrive Sk3

My max Budget for a battery is around £100, I only need the battery to last around 3-4 Miles as thats the distance to work.

Any Help would be amazing, Thankyou so so Much!!!

![49300536_1160085947499331_5676644114616025088_n|499x500](upload://28T29nsWWI3RXBAUsYYCjg3cT7F.jpeg)
```

---
## \#2 Posted by: evoheyax Posted at: 2019-01-03T18:38:26.349Z Reads: 100

```
When you pull currents above what your lipos can really do, they get hot and the electrolyte in the battery starts to break down faster. This results in 2 components, lithium and oxygen, being released inside, and with heat, more oxygen is released than can be absorbed, which results in swelling.

This is why you want to go far less then the rating when it comes to charging and discharging. Just because you calculate the max amp rating to 100a lets say, doesn't mean it can do 100a without puffing up. I would take a quarter of the rating at best, with zippys, and an eighth for multistar packs.

Over discharging and over charging also cause this reaction to occur faster.

Li-ion is safer and easier is this regard, but they also can output far less amps at any given moment for the same price and space and the voltage sags more, resulting in less power compared to a lipo.
```

---
## \#3 Posted by: Timotay Posted at: 2019-01-03T18:47:57.573Z Reads: 90

```
Thanks for explaining this, I'm not too fussed about power,  for the board. So a less powerful, safer battery is good in the situation I'm just looking for the best lithium Ion battery I can get for my budget and will function well with board.

Do you have any reccomendations??
```

---
## \#4 Posted by: evoheyax Posted at: 2019-01-03T18:58:31.317Z Reads: 85

```
You want a battery pack built with Samsung 30Q cells. These are the cells most people in the DIY scene are using, since they really are best combo of capacity (high), discharge rate (high), and sag (lowest of li-ion).

But li-ion is 3-4 times as expensive as lipo. Most of these packs are in the $200 - $300 assembled for a smaller pack, larger ones can run $600+.

Best case, you need at least a 6s4p of 30Q cells. That's 24 cells at ~$5 a piece. So about $100 there. And then a bms, around another $40 - $60. Charger is another $20 -$30. Then plugs and assembly, will probably run you another $40 (very lucky) - $80. All in all, at least $200 for the whole thing. And that's a pretty small battery.

The alternative is something like this: https://hobbyking.com/en_us/zippy-compact-6200mah-6s-40c-lipo-pack-xt90-1.html?wrh_pdp=3

I use zippy lipos myself, and this guy can pack a decent punch.

But the real issue is you need a VESC instead of that controller your using. You can't adjust settings to limit current for example or prevent over discharging. So li-ion or lipo, your going to burn though more batteries.
```

---
## \#5 Posted by: pjotr47 Posted at: 2019-01-03T19:06:47.859Z Reads: 73

```
I have a Samsung 30q 7s3p with high discharge bms laying around. But I think you can only use a 6s battery?
```

---
## \#6 Posted by: evoheyax Posted at: 2019-01-03T19:08:44.761Z Reads: 71

```
That esc can only do 6s. I would recomend the OP jump on the focbox deal that's going on right now though so he can proper manage the battery pack while in operation. Not to mention the quality of ride difference is night and day.
```

---
## \#7 Posted by: pjotr47 Posted at: 2019-01-03T19:12:15.659Z Reads: 66

```
I thought that the Focbox deal was over? 

I have maybe also a second hand vesc with a broken drv that I am going to send for repair. 

I can maybe do the topic starter a good deal :slight_smile:
```

---
## \#8 Posted by: evoheyax Posted at: 2019-01-03T19:15:00.532Z Reads: 65

```
oh, correct, it is. I just saw it on the top of the forum and assumed it's still going on.

I also have ton's of 4.12's lying around I can let go cheap, but I'm not in the uk, so I'll let you handle it!
```

---
## \#9 Posted by: evoheyax Posted at: 2019-01-03T19:45:08.464Z Reads: 58

```
Just to clarify, if you did use a battery pack with a bms inline (not bypassed for discharge), it would protect your battery from over discharge. But those are hard shutdowns that can throw your off your board (this is a mistake enertion made on the original raptor 1). A VESC based esc will gradually throttle back the power and allow you to get all of the power from your battery, instead of, oh you hit this voltage, no more power all of a sudden.
```

---
## \#10 Posted by: Timotay Posted at: 2019-01-03T19:46:05.470Z Reads: 56

```
I've looked at some Lipos with hardcases, if I match this up with a voltage alarm this hopefully should be slightly safer regarding over discharging while riding.

If I'm going to get lipo, it will properly need to be a hard case. Can you recommend any that are under £50 On hobbyking?
```

---
## \#11 Posted by: evoheyax Posted at: 2019-01-03T19:57:45.396Z Reads: 57

```
My recommendation for lipos is stick with zippy. They have a good reputation. You can just search for 6s zippys that are over 5000 mah.

You want at a min 100 wh to be safe. wh = ah * nominal voltage. With 6s, that's 22.2 volts. So anything less than 5ah at 6s will run you risky of not getting the range you need.

Also, weight and especially hills play a big roll. Efficient drive trains get around 10 wh per mile with light riders and on flats at 15 mph top speed and 5 mph min speed. Even a minor hill will eat 4 times as much energy as on flat. So now if your whole trip is on a minor hill, with 100 wh, you'd maybe get 3 miles at best. Now steeper hills, can be as much as 16 times as much. So you have to look at your route, and take a guess as to how much is up hill vs flat.

The one I listed you is my best recommendation that I believe would get you the range you need, assuming your a lighter guy with mostly flats and not steep hills.

Just be careful, the false economy is real. It's easy to buy cheap, break it, and have to replace it. We've all done this. If this is a serious transportation use as it seems to be for you, reliability, as well as durability, should be high factors on your list (late to work cause your board broke down? Easy to get in trouble here). A proper investment of ~$400 for a good li-ion pack and good vesc (do not buy the sub $100 vesc's if you want durability), will go a long way.

I use a DIY electric bike for work, and I burnt through 3 $100 vesc's in under a month. Then, spent the $300 for an official vesc 6 and now 4 months later and no problems. I should of just bought the official one from the beginning, would be $300 richer. I also push it hard, which is probably why they kept breaking. But not all are created equal. Even the same looking one, could have 2 different qualities of assembly, and fake components are a serious problem in escs.

Why do you want a hardcase lipo? They are just as likely to puff and are usually more expensive also.
```

---
## \#12 Posted by: Timotay Posted at: 2019-01-03T20:16:23.795Z Reads: 46

```
God dam, I would love to meet you in person. You know so much. I think I will but go for a basic battery this time, if everything goes well I will look at a fill rebuild with a new vesc, li-Ions and dual motors. 

Thanks for your help!
```

---
## \#13 Posted by: evoheyax Posted at: 2019-01-03T20:22:53.408Z Reads: 47

```
[quote="Timotay, post:12, topic:79782"]
You know so much.
[/quote]

Experience and passion my friend. I learned a lot through trail and error. Back when I started 4 years ago, there were no experts to turn to for advice. So idk how many thousands of dollars later, I learned a lot.

Cheers!
```

---
## \#14 Posted by: Timotay Posted at: 2019-01-03T21:46:43.741Z Reads: 46

```
For now im just going to go with:

Battery
https://hobbyking.com/en_us/zippy-compact-4500mah-6s-40c-lipo-pack-xt90.html

Voltage Alrarm:
https://hobbyking.com/en_us/hobbykingtm-lipo-voltage-checker-2s-8s.html

Is that okay as a cheap solution?
```

---
## \#15 Posted by: Bor.inc Posted at: 2019-01-03T22:53:20.533Z Reads: 40

```
Yes the zippy lipo is decent

I myself use the standard (I cant find it on hk anymore tho) 2x zippy 3s 5000mAh 20c lipos in series and they serve me well. You even have higher C-rating so thats a bit better. I've never done a range test but I can go (with the 5000mAh) around 8km which is enough for only in the city but after some riding I personaly would have liked some more range. You have a slightly lower range (because of the 4500mAh) so you can try it but maybe you want some extra range :slight_smile:
```

---
## \#16 Posted by: brenternet Posted at: 2019-01-03T23:16:19.781Z Reads: 37

```
[quote="evoheyax, post:13, topic:79782"]
I started 4 years ago, there were no experts to turn to for advice
[/quote]

TIL no one used batteries in 2015.
```

---
## \#17 Posted by: evoheyax Posted at: 2019-01-04T00:55:17.088Z Reads: 29

```
I’m not talking about batteries in general, I mean in electric skateboards and the factors that affect range most and what not. A lot more has become agreed upon by the eskate community.

4 years ago, you had almost no options in eskate. Now we have specific eskate stuff.
```

---
## \#18 Posted by: ryansinatra Posted at: 2019-01-04T00:58:01.307Z Reads: 28

```
Hey, hit me up about those 4.12 s 😁
```

---
