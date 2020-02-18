# LiPo Charger Turningy 12000mAH

### Replies: 29 Views: 453

## \#1 Posted by: xsynatic Posted at: 2019-01-03T17:13:01.752Z Reads: 88

```
Hey ho,

i think i got a bit ahead of myself with ordering all parts but not understanding everything to be honest.
I bought 2x Turnigy High Capacity 12000mAh 6S 12C Lipo Pack w/XT90 batteries. 
But i don't really know how to charge them. I know that i should use a balance charger but my question is if i can charge both at the same time or one by one?  Would this be enough and how would i charge them 
simultaneously?

This would be my balancer : 
[Charger Link](https://www.amazon.de/Genuine-Original-Ladeger%C3%A4t-Multifunkt-Balance/dp/B01AXUZSO4/ref=sr_1_3?ie=UTF8&qid=1546533538&sr=8-3&keywords=lipo+balancer) 

[Battery specs]
Minimum Capacity: 12000mAh
Cell Count:  6 / 22.2V
Constant Discharge:  12C
eak Discharge (10sec):  24C
Pack Weight:  1650g
Pack Size:  183 x 77 x 58mm
Charge Plug: JST-XH
Discharge Plug:  XT90

![197879|566x415](upload://9osFX6US3br9aZMBxC0tti0WEbj.jpeg)
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-01-03T17:26:35.334Z Reads: 72

```
yes you can charge them at the same time using a standard hobby charger and a parallel board from Hobbyking (the imax b6ac is a great one) . just test the voltages first and ensure that they're relatively close before you plug them in. with that monstrous capacity it will take ages to charge as when they're in parallel it essentially creates a 6s 24,000mah pack. so if you charge at 5a itd take just under 5hrs to charge
```

---
## \#3 Posted by: Andy87 Posted at: 2019-01-03T17:27:35.908Z Reads: 71

```
With this Charger you will charge ages.
I need 2.5h for 5Ah.
You could charge them parallel with a parallel board, but than you need to know what you doing and it will take even longer.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-01-03T17:29:04.177Z Reads: 71

```
It’s not a 5a charger 😅 that’s what I thought too.
In 6s max charge current is 2.3a 😱🙈
So pretty close to 10h for both to charge.
```

---
## \#5 Posted by: J0ker3366 Posted at: 2019-01-03T17:41:54.397Z Reads: 63

```
[quote="mynamesmatt, post:2, topic:79771"]
just under 5hrs to charge
[/quote]

That made me laugh
```

---
## \#6 Posted by: xsynatic Posted at: 2019-01-03T17:41:58.539Z Reads: 57

```
So my Wowgo 2s Chagrer has an output of 42Volts  = 2.0A which takes 2.5 - 3 hours for my 6.4Ah Battery pack (18650)

The Powersupply that comes with the Balancer has 12V 5A. The 5A are good, but i need more volts right or is that ok?
```

---
## \#7 Posted by: J0ker3366 Posted at: 2019-01-03T17:44:19.935Z Reads: 54

```
Get this stuff instead
https://www.amazon.de/Crazepony-UK-Ladeger%C3%A4t-Charging-Connectors-Parallel/dp/B06XPHBB3G/ref=mp_s_a_1_8?__mk_de_DE=%C3%85M%C3%85Z%C3%95%C3%91&qid=1546537363&sr=8-8&pi=AC_SX236_SY340_FMwebp_QL65&keywords=lipo+charger&dpPl=1&dpID=51KvfVmrddL&ref=plSrch

https://www.amazon.de/SKYRC-Professional-Balance-Discharger-Batteries/dp/B07CTRDBM1/ref=mp_s_a_1_29?__mk_de_DE=ÅMÅZÕÑ&qid=1546537398&sr=8-29&pi=AC_SX236_SY340_QL65&keywords=lipo+charger
The charger will charge @ 6a so you wint have to wait on Christmas for a full battery.
```

---
## \#8 Posted by: xsynatic Posted at: 2019-01-03T17:48:55.232Z Reads: 47

```
How about this one?

You can choose 24v 5A, 24V 6.25A etc.
[https://www.amazon.de/Netzteil-Ladeger%C3%A4t-LED-Leuchte-Kamera-%C3%9Cberwachungskameras-Festplatten/dp/B01MFFDI1Z/ref=sr_1_10?ie=UTF8&qid=1546536963&sr=8-10&keywords=5A%2Bnetzteil&th=1](https://www.amazon.de/Netzteil-Ladeger%C3%A4t-LED-Leuchte-Kamera-%C3%9Cberwachungskameras-Festplatten/dp/B01MFFDI1Z/ref=sr_1_10?ie=UTF8&qid=1546536963&sr=8-10&keywords=5A%2Bnetzteil&th=1)
```

---
## \#9 Posted by: Andy87 Posted at: 2019-01-03T17:51:01.791Z Reads: 48

```
Sorry to say but that’s not correct.
It’s a 60w Charger.
So at 25.2V (6s) thats only 2,38a max charge current.
```

---
## \#10 Posted by: J0ker3366 Posted at: 2019-01-03T17:51:48.639Z Reads: 45

```
You'll then need a bms and more wiring and another hole in your enclosure. If you get what I posted, no more holes, no bms, no more wires.
```

---
## \#11 Posted by: Hummie Posted at: 2019-01-03T17:52:14.051Z Reads: 46

```
https://www.amazon.com/FPVKing-CellMeter-7-Digital-Capacity-Controller/dp/B074W13Y13/ref=mp_s_a_1_13?ie=UTF8&qid=1546537614&sr=8-13&pi=AC_SX236_SY340_QL65&keywords=lipo+balancer

https://www.amazon.com/Intelligent-Discharger-Operating-Discharge-Helicopter/dp/B07K57LKDQ/ref=mp_s_a_1_15?ie=UTF8&qid=1546537614&sr=8-15&pi=AC_SX236_SY340_QL65&keywords=lipo+balancer

https://www.amazon.com/MEAN-WELL-SE-600-48-Supply-Single/dp/B00G8UDEQ8/ref=pd_aw_vtph_328_tr_1?_encoding=UTF8&pd_rd_i=B00G8UDEQ8&pd_rd_r=5e0af44d-0f7f-11e9-a7bd-d918586a92b8&pd_rd_w=as6vP&pd_rd_wg=Jmmn4&pf_rd_p=61cf5fd0-cfc9-447f-a425-f14760645161&pf_rd_r=B0X52J0515T8XDSA7HKR&psc=1&refRID=B0X52J0515T8XDSA7HKR


Never seen a balance discharged this powerful before.
```

---
## \#12 Posted by: Andy87 Posted at: 2019-01-03T17:54:37.095Z Reads: 41

```
The most easy thing is to get a charge only bms 25€ plus a laptop style charger 4-6a for 12s and you can charge both packs with one charger and way faster.
```

---
## \#13 Posted by: Hummie Posted at: 2019-01-03T17:57:28.928Z Reads: 42

```
I feel I always know the easiest because I’m the laziest.  U can skip the bms if ur willing to balance on the side.  This method also allows fastest charging and cheapest.  Best for the laziest, cheapest, and most impatient, but you must be somewhat capable
```

---
## \#14 Posted by: J0ker3366 Posted at: 2019-01-03T18:00:27.497Z Reads: 42

```
Easy peasy
![1223182030_Film1|374x499](upload://aJABYPsw1ga2ADH7iedgWUOCDr9.jpeg)
```

---
## \#15 Posted by: J0ker3366 Posted at: 2019-01-03T18:01:35.133Z Reads: 39

```
Oh and I'm doing that with six lipos now.
```

---
## \#16 Posted by: xsynatic Posted at: 2019-01-03T18:01:47.728Z Reads: 38

```
Technically this doesn't have to be charged the fastest way. I'm building my first DIY Board as my Second Board (Wowgo 2s)
This is supposed to be a Mountainboard. So if it takes 5 hours to charge so be it. I don't want to solder or cut anything on my batteries becuase i don't trust myself with it. Plug and play would be the best
```

---
## \#17 Posted by: Hummie Posted at: 2019-01-03T18:03:40.968Z Reads: 40

```
Hardly easy. Those little plugs drive me nuts and ur doing tons.  One big xt90 plug and putting the balancer intermittently to the two 6s balance plugs 🔌. Easier. Cheaper. Way faster.  But more likely to blow up if u don’t watch out
```

---
## \#18 Posted by: xsynatic Posted at: 2019-01-03T18:04:26.215Z Reads: 38

```
I found this on "Skatemetrics Patriot" Build. What do you think of it? I don't quite understand the last part.

EDIT : They use the same batteries as me! 

Charging the Batteries

You can charge the batteries individually using a 6S balancing charger like ([[this]](https://amzn.to/2BnLcEc)). For bonus points, however, you may also consider building a very simple adapter for a standard three-stage charger like [[this]](https://amzn.to/2R0JLpa) , which will allow you to charge both batteries at once (be sure to balance them from time to time though, or you could start a fire). Creating a converter is as easy as soldering two bullet connectors to a coax charging port, like [[this]](https://amzn.to/2BlOFmA).
```

---
## \#19 Posted by: J0ker3366 Posted at: 2019-01-03T18:05:29.427Z Reads: 38

```
[quote="Hummie, post:17, topic:79771"]
But more likely to blow up if u don’t watch out
[/quote]
We'll ignore that part lol.
```

---
## \#20 Posted by: Andy87 Posted at: 2019-01-03T18:14:35.981Z Reads: 39

```
Honestly i‘m Not holding anything on that guys...
You should always balance lipos, because if not you can easy peasy ruin your full pack because only one cell was over discharged.

If you go with a bms solution you don’t need to solder anything on your battery.
Look, I made this adapter 
![image|375x500](upload://w3llul6KCYMph5R6fnyfmwLma63.jpeg) 

You just connect a usual 12s charger on the charge side. And both your lipos in series( like they are anyhow connected in your board) from the other side. You than connect the balance leads of your packs to the bms and you can balance charge them.

Bms will cost you 25€
The charger 40-60€
And you can charge any 12s packs you want with it
```

---
## \#21 Posted by: evoheyax Posted at: 2019-01-03T18:29:14.387Z Reads: 38

```
That crap will break. These chargers require the a regulator to control current. Batteries will pull 12.5 continuous since there's not regulator in between and it will burn up fast.

You can say you have used a similar one without issues, but how much have you been ridding the past couple years? I went through 3 before I gave up and just bought the proper meanwell for $200 that has adjustable current and can actually do 12 amp con without burning up.
```

---
## \#22 Posted by: xsynatic Posted at: 2019-01-03T18:32:38.188Z Reads: 37

```
So it would basically be like this?
![001|690x264](upload://c1euLpZzkYV5U9NqqBF756JE3V8.jpeg) 

If your bms works like advertised then i only need a suitable PSU
```

---
## \#23 Posted by: Andy87 Posted at: 2019-01-03T18:41:38.676Z Reads: 35

```
 Yes but you need to wire the balances adapter right. If you need help with it just let us know. It’s not that difficult
```

---
## \#24 Posted by: Hummie Posted at: 2019-01-03T18:43:44.101Z Reads: 33

```
Making them w adjustable current is a super easy mod adding a resistor but I never had a problem with them breaking from over current

https://endless-sphere.com/forums/viewtopic.php?f=14&t=75212&hilit=Meanwell
```

---
## \#25 Posted by: evoheyax Posted at: 2019-01-03T18:44:55.647Z Reads: 31

```
[quote="Hummie, post:24, topic:79771"]
I never had a problem with them breaking from over current
[/quote]

Because you've used it like, 20 times in the past 2 years... I was going through them every 1-2 weeks.
```

---
## \#26 Posted by: Hummie Posted at: 2019-01-03T18:47:30.612Z Reads: 30

```
Was using them for 2 years prior no prob.  Actually use it still often to charge lipo to run motors on bench and prior to that used it like crazy charging 3 or 4 times a day maybe a quarter of last year. If ur worried they can’t do their rated current u can simply add the resistor.   Or get the way more expensive meanwell one you got.  Actually I linked a meanwell. Or I read one for leds is better at putting out their continuous max amps.  There are a lot of folks who use them no prob
```

---
## \#27 Posted by: mynamesmatt Posted at: 2019-01-03T19:02:05.440Z Reads: 26

```
[quote="J0ker3366, post:5, topic:79771"]
That made me laugh
[/quote]

yeah i sorta wrote it and then added the imax b6 to it after
```

---
## \#28 Posted by: xsynatic Posted at: 2019-01-03T20:56:58.133Z Reads: 23

```
Sure. How many watts do you think i need if i find a 5/6/7A charger? (5Hours charging would be ok)

Not sure what specific specs i need (volts,watts etc)

[Amazon charger?](https://www.amazon.com/29-4V-Charger-Li-ion-Battery-Auto-Stop/dp/B07538916X)
```

---
## \#29 Posted by: Andy87 Posted at: 2019-01-03T21:02:13.653Z Reads: 23

```
I‘m very happy with this one in 8a
https://s.click.aliexpress.com/e/N52jwN8
But you can find any similar also with lower amps.
I think the cheapest are around 4a.
Just have a quick search on AliExpress.
```

---
