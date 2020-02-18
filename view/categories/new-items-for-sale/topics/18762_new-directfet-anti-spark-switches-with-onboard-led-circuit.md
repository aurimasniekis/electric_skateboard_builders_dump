# New DirectFet Anti-spark Switches with onboard LED circuit

### Replies: 24 Views: 4274

## \#1 Posted by: goldenHusky Posted at: 2017-03-08T17:40:06.570Z Reads: 488

```
## This product still requires real-world testing, you will get a full refund/ free repair if problems occur, I appreciate any feedback! Thank you!

Hi,

I designed a new anti-spark switch, based on the circuit of the Vedder switch.


Features:
• completely presoldered 
• 3 DirectFets (the ones that will also be used on VESC 6.0)
• onboard LED driver circuit with adjustable LED current, lights up depending on switch state
• only 28x28mm, equals 40% reduced pcb size compared to the original Vedder switch
• JST connector for your external switch
• 2oz copper
• parts purchased at mouser
• pure copper heatsink
• shrink tube


<img src="/uploads/db1493/original/3X/f/f/ff8e676c034c3da770abdcb012ca65c2fe2477a9.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/7/0/7020b81b8c22d64babaa85f31f668680e3088d37.JPG" width="666" height="500">

I'm selling the second version of this switch, below you see pictures of the first prototype compared to a Vedder Switch.

<img src="/uploads/db1493/original/3X/7/3/73556ad2e6955a083e822a43bb806fbf0eae23e6.jpg" width="666" height="500">

45€ + shipping (worldwide)
Located in EU (Salzburg, Austria)
```

---
## \#2 Posted by: barajabali Posted at: 2017-03-08T17:44:13.200Z Reads: 441

```
Should it handle the same amount of amps as the vedder?
```

---
## \#3 Posted by: goldenHusky Posted at: 2017-03-08T17:48:35.532Z Reads: 435

```
[quote="barajabali, post:2, topic:18762, full:true"]
Should it handle the same amount of amps as the vedder?
[/quote]

Even more :wink:
I built a test circuit with a 70A supply. 
Anyway, if the switch fails somehow you get a full refund. 
I would like to receive feedback from real world conditions.
```

---
## \#4 Posted by: barajabali Posted at: 2017-03-08T17:56:07.742Z Reads: 411

```
Oh okay I have yet to blow out a vedder switch on my mountain boards but im pretty sure that the switch is a bottle neck considering the system can output 140 amps constant safely.
```

---
## \#5 Posted by: Maxid Posted at: 2017-03-08T17:58:35.591Z Reads: 385

```
but no fuse? :cry:
```

---
## \#6 Posted by: barajabali Posted at: 2017-03-08T18:00:58.964Z Reads: 377

```
Just use an inline fuse :)
```

---
## \#7 Posted by: Namasaki Posted at: 2017-03-08T18:35:28.963Z Reads: 367

```
Looks really good!
```

---
## \#8 Posted by: goldenHusky Posted at: 2017-03-10T12:33:28.789Z Reads: 349

```
[quote="Maxid, post:5, topic:18762"]
but no fuse? :cry:
[/quote]

Sorry, sadly I found no compact fuse holder rated for more than 40A and I also wanted to make it as compact as possible. Anyway, Inline fuse holders will do the job,

[quote="Namasaki, post:7, topic:18762, full:true"]
Looks really good!
[/quote]

Thank you!

First unit is on its way to @barajabali, the switch won't be the bottleneck anymore for sure haha :wink:
```

---
## \#9 Posted by: barajabali Posted at: 2017-03-10T16:58:28.260Z Reads: 318

```
My dude! Thank you
```

---
## \#10 Posted by: ipv6app Posted at: 2017-06-20T14:38:09.229Z Reads: 281

```
@goldenHusky -- I'm interested in testing out 3 units.  I have a dual hub board 800W, dual motor belt 1200W board. that I can try this out on. Using 10s batteries.  Recently built these boards.  Think you can private msg me and we can complete the transaction for the new direct FET version?   Thanks!
```

---
## \#11 Posted by: goldenHusky Posted at: 2017-06-20T21:59:29.370Z Reads: 267

```
Hi @ipv6app 

awesome that you found this topic, I almost forgot it myself haha :joy:
Pm sent, thanks!
```

---
## \#12 Posted by: dimnsionofsound Posted at: 2017-07-29T05:13:28.566Z Reads: 241

```
This looks pretty slick! Do you have measurements of the temperature profile over time given certain loads?

I'm considering DIYing something like this but if what you've got fits my requirements (considering an all out build with 2x VESC 6) I'd be down to get one of yours. 

Specifically, assuming the other components can handle it, I want to see how long I can consume 2800 watts of power @ 40 volts, which coincidentally works out to 70 Amps, matching your test setup. This 2800 number is what I calculated for going up a 20% grade hill at 25MPH given an efficiency of 70%. 

In reality I wouldn't be pulling this much power for very long but there is something nice about overbuilding to never have to worry if anything is operating at its limits.
```

---
## \#13 Posted by: goldenHusky Posted at: 2017-07-29T06:27:13.390Z Reads: 227

```
[quote="dimnsionofsound, post:12, topic:18762"]
This looks pretty slick! Do you have measurements of the temperature profile over time given certain loads?
[/quote]

Thanks! Unfortunately I haven't, maybe on a rainy day but I can't promise it.
Maybe @ipv6app can tell something  regarding the temperature and current on his boards.
Like written in the headline, I will refund you if you aren't satisfied or any problems occur.
```

---
## \#14 Posted by: dimnsionofsound Posted at: 2017-07-29T07:04:54.109Z Reads: 219

```
I did some research on the DirectFETs, so for anyone else out there that may have been wondering, this should be fine at 70A continuous.

Using values from the [datasheet](http://www.mouser.com/ds/2/196/irf7749l1pbf-936035.pdf):

* Worst case Rds_on of ~2mOhm for each at 125ºC
* Thermal resistance to ambient of 20ºC/W in a mounting configuration with heatsink similar to yours

 The power dissipation at 70A would be about 3.3 watts total ( = 70A * ( 70A * 0.002 / 3)), 1.1 W each, giving a temperature rise of only ~22ºC above ambient. Solid!
```

---
## \#15 Posted by: Vanarian Posted at: 2017-07-29T07:45:01.748Z Reads: 217

```
Nice job, you should make a 6 FETs option too! Many folks here don't understand that without the DirectFET package, top cooling is useless. 

With the metal all around that's perfect.
```

---
## \#16 Posted by: WawiKirsinger Posted at: 2017-08-28T21:05:00.347Z Reads: 212

```
Hi! i´m new and i´m considering your E-switch..... how much is in US dollars? and the sipping to Chile? thanks!
```

---
## \#17 Posted by: goldenHusky Posted at: 2017-08-28T22:30:28.725Z Reads: 211

```
Hi @WawiKirsinger thanks!

I will be launching some new versions of the direct fet switches together with some other switches this week, plus an onlineshop for antisparks. Pcbs arrive on Wednesday. They have now a better layout/routing and up to 6 direct fets @Vanarian , but are still not bigger than a vedder switch. Furthermore I had a chat with Fechter to make them literally bulletproof, and they are now :smirk:

Hopefully I get permission from the government in the upcoming days. 
I will send you the link to my shop so you could choose what model you'd like if you don't mind.
Thanks!

Best
Fabio
```

---
## \#18 Posted by: WawiKirsinger Posted at: 2017-08-28T23:25:03.447Z Reads: 204

```
dude awesome! thanks very much... and sorry for the question but :sweat_smile: what is "6direct fets".... i dont understand to much yet sorry for ask :smiley:
```

---
## \#19 Posted by: willpark16 Posted at: 2017-08-29T00:06:57.349Z Reads: 200

```
Direct fets are better at heat dissipation they replace mosfets
```

---
## \#20 Posted by: Vanarian Posted at: 2017-08-29T18:40:03.494Z Reads: 189

```
It is another type of FETS with metal body instead of plastic ; it does directly conducts the heat in every direction thus being better at dissipation.

Good job @goldenHusky for the new anti spark!
```

---
## \#21 Posted by: Rollbrett Posted at: 2018-03-30T08:12:42.790Z Reads: 111

```
@goldenHusky Sorry for digging up this old conversation, but I'm looking for a small Anti-Spark Switch and was wondering if you still have any of these available?
```

---
## \#22 Posted by: pat.speed Posted at: 2018-03-30T08:36:43.461Z Reads: 113

```
He has a website now



http://www.antisparkheaven.com
```

---
## \#23 Posted by: Rollbrett Posted at: 2018-03-30T08:40:13.068Z Reads: 114

```
I'm aware of that. It only lists Dinosaur-series Antispark switches though and I'm looking for something small
```

---
## \#24 Posted by: goldenHusky Posted at: 2018-03-30T08:43:34.221Z Reads: 113

```
Hi @Rollbrett,

the switch, this topic is about, is an old prototype, I don't have it anymore but I can send you some of the switches below, the dimension of the single fet switch is 36mm x 21mm and the dual is 40mm x 32mm 

![7730_1|519x500](upload://kSPsshcFmOXPlPUkzFCvaFmf6Kw.jpg)

![7530_2|605x500](upload://d4y2jcK8sfZ5F4JJRrFFoL55qYT.png)
```

---
