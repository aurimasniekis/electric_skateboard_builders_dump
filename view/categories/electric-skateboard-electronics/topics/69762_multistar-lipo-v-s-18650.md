# Multistar lipo v.s. 18650

### Replies: 35 Views: 730

## \#1 Posted by: TheRafter Posted at: 2018-10-01T18:08:47.661Z Reads: 203

```
I'm currently building my first ever beefy electric longboard. One of the things that I'm curious about is the batteries. I'm looking at Multistar HV 14.8v 16ah batteries v.s. your generic 18650 pack. I've heard that the Lipos don't last as long, but they give more of a boost. The 18650s are used by almost all name brand boards, last a lot longer, but don't provide as much of a punch. Is that true. So far, I'm finding that a 18650 is going to run me more money (unless I build my own which I've no idea how to).

Basically, which one is better. I'm not running with a BMS so I'll need a larger capacity (my original design was 950wh, but another was 500wh).
Thanks for the input in advance.

https://hobbyking.com/en_us/multistar-high-capacity-16000mah-4s-12c-multi-rotor-lipo-pack-w-xt90.html

products/electric-skateboard-battery-epower-pack-12s4p
```

---
## \#2 Posted by: Jmding Posted at: 2018-10-01T18:54:59.528Z Reads: 187

```
I suggest you read through the sticky threads.  The nature of this question suggests that your understanding of the physics and the role of the different components is perhaps still not quite at the level where you will be able to produce a satisfactory design.  We can answer your specific questions, but there are going to be lots of questions that you dont know to ask, that we cannot help you with, and that you really ought to be able to answer before starting to buy parts.

For battery packs of this size, the poor power density of 18650s is not a binding constraint, and so you can really take advantage of their extra energy density.
```

---
## \#3 Posted by: telnoi Posted at: 2018-10-01T20:53:42.707Z Reads: 177

```
[quote="TheRafter, post:1, topic:69762"]
Basically, which one is better.
[/quote]

depends on your budget, other components of the build (including motor KV, gearing, total pack voltage, wheel material/pneumatics or PU), weight and a couple of other factors. That said, the multistar 12C is about the worst choice for high amp draw requirements, as it is meant for field charging drone batteries. A low amp application.
```

---
## \#4 Posted by: Namasaki Posted at: 2018-10-01T21:25:19.053Z Reads: 160

```
I agree with @telnoi
Those Multistar Lipos are not good for esk8 applications. 
The only Lipos I know of that are comparable in capacity and can deliver adequate current are the Tattus
They are big, heavy and expensive. 

Frankly if your needing a lot of range then the 30q Li-ions are the way to go.
Although building a dependable and safe Li-ion pack is not a simple task.
And buying a good prebuilt Li-ion battery is not cheap. 

Smaller capacity Lipos like 5ah with high C ratings like 60C-100C, are good for delivering high current and short to medium range in a 10s or 12s configuration and allow you to have a compact, light weight and relatively inexpensive battery solution.
```

---
## \#5 Posted by: Benjamin899 Posted at: 2018-10-01T21:43:12.778Z Reads: 144

```
i once had an RC esc and my turnigy 5Ah with 20c constant and 30c burst could deliver 150amps, i even installed an wattmeter to read it out. So if you ride with an vesc and limit it why would those Multistar be weak?
```

---
## \#6 Posted by: b264 Posted at: 2018-10-01T21:49:15.193Z Reads: 137

```
It may be rated for 100A constant and 150A burst but running things at their rating may drastically reduce their lifespan or safety margins.  The further under that you can get, the better.
```

---
## \#7 Posted by: Benjamin899 Posted at: 2018-10-01T21:54:11.936Z Reads: 132

```
yeah sure thats a given, i always aim to go 50% of constant ratings. but who is even seeing these values, excluding eMTB and people who live in the mountains.
Then again, if you use those lipos with a vescs you will not go near these values, i think. 
Those multistar have a constant rating of 192Amps, lets say they can put up with 70-80 constant, thats still enough breathing room.
Am i missing something? 
FYI i also use 30Q because of safety reasons and longevity.
```

---
## \#8 Posted by: pat.speed Posted at: 2018-10-01T21:56:29.080Z Reads: 129

```
The thing is those ratings are bs. If you tied to pull 190amps through a multi star battery you would get nothing but fireworks. They have been tested to only be around 3-4c in reality
```

---
## \#9 Posted by: b264 Posted at: 2018-10-01T21:57:29.333Z Reads: 125

```
[quote="pat.speed, post:8, topic:69762"]
The thing is those ratings are bs.
[/quote]

And then there's this LoLz

Marketing department hard at work to make sure your money goes to them, regardless of product quality
```

---
## \#10 Posted by: Benjamin899 Posted at: 2018-10-01T21:58:00.696Z Reads: 121

```
oh wow, i knew lipos were 50% off the ratings they get, but that is extreme.
```

---
## \#11 Posted by: bartroosen12 Posted at: 2018-10-01T22:02:57.124Z Reads: 122

```
It just depends on your setup.
I have made a 10S1P with multistar 5Ah 10C cells and a vesc with 25A max battery current and I have never had problems with them, just make sure the cut of voltage isn't to low. I put them on 33V just to be sure and never had a swollen or hot cell.

What will be your setup? How much current, which battery config 12S#P?

I got a 18650 pack and it works perfect, you just need to be carefull with those lipo cells and make sure they can handle the current.

But damn 145$ seems expensive for those multistar packs?
```

---
## \#12 Posted by: pat.speed Posted at: 2018-10-01T22:06:18.367Z Reads: 115

```
Yeah that seems about right, but I bet any higher and it would sag like crazy
```

---
## \#13 Posted by: Benjamin899 Posted at: 2018-10-01T22:06:47.597Z Reads: 115

```
i just looked at the battery from DIY, dude that thing has a BMS ect...why is this even a question.
```

---
## \#14 Posted by: pat.speed Posted at: 2018-10-01T22:12:07.447Z Reads: 113

```
Oh and btw it’s going to cost you the same amount of money to get that 18650 pack from @torqueboards as it would to get 3 of those lipos. I know what I would be buying 😉
```

---
## \#15 Posted by: Jacobee Posted at: 2018-10-02T01:24:51.845Z Reads: 103

```
Feel free to disagree with me but I think multistars are an okay battery if you don't draw at more than 4c. I've been running two 4s 10,000 mAh in series on my board for over a year at this point and they've been good for me. Again I'm not drawing more than 40 amps out of the 10 amp hour multistars and I imagine they wouldn't be ideal if you need more power than that
```

---
## \#16 Posted by: lrdesigns Posted at: 2018-10-02T02:03:09.703Z Reads: 91

```
[quote="pat.speed, post:14, topic:69762"]
Oh and btw it’s going to cost you the same amount of money to get that 18650 pack from @torqueboards as it would to get 3 of those lipos. I know what I would be buying :wink:
[/quote]

That would make the choice easy. But I get a price of $95 from global warehouse. $285. shipping to the US aint gonna be cheap though. What is the price in the US warehouse I can't see it?

I would still suggest be patient and save some more money and get the 30q pack from DIY. It will last much longer and be more resilient to user error.

DIY battery also has, a battery meter, an anti spark switch, a BMS, an enclosure and a friggen charger. Makes it look like good value compared to the Multistar bare bones packs.
```

---
## \#17 Posted by: pat.speed Posted at: 2018-10-02T09:04:37.729Z Reads: 81

```
I'm not sure the US price, but the Australian was about $200 each so thats 600 for 3 of them. The torqueboards pack was about $630 Australian and comes with bms, switch, lcd and charger. 

In conclusion you will save more money just buying from @torqueboards plus you will get good help and support
```

---
## \#18 Posted by: TheRafter Posted at: 2018-10-02T14:44:45.914Z Reads: 77

```
I looked at the 30q pack from DIY, but there are 2 problems that I found. First, it is limited by a 50A output current by the BMS defeating the point of making this way overpowered. Also, it is only ~400Wh which will not be nearly enough. I'll need something closer to 900 as I am putting 2 4100W motors on it. I know those motors are way to overpowered, but their about the same price and allows me to customize it to be offload later (plus who doesn't want ridiculous power, even if you won't use it). This is still all probably gonna change - I'm still not close to the building process yet.
```

---
## \#19 Posted by: Benjamin899 Posted at: 2018-10-02T14:49:01.069Z Reads: 74

```
ok. You should realy start reading up.
```

---
## \#20 Posted by: Jmding Posted at: 2018-10-02T14:59:57.783Z Reads: 75

```
How are you planning on dealing with traction?
```

---
## \#21 Posted by: TheRafter Posted at: 2018-10-02T15:36:35.140Z Reads: 67

```
I got the Orangoutang wheels which do do a good Job. Otherwise, I'm never going to give it full throttle anyways.
```

---
## \#22 Posted by: Andy87 Posted at: 2018-10-02T16:13:26.188Z Reads: 64

```
4100w / 48v = 85,4a per motor, per vesc...
Which vesc you plan to use for it and i hope this vesc has a good heatsink.
If it’s true that the multistar lipos can only output 4c (64a) it would be still too less
```

---
## \#23 Posted by: TheRafter Posted at: 2018-10-02T16:21:23.936Z Reads: 70

```
I decided to go with the DIY electric skateboards 30q 12s4p pack. The VESC I'm using is also from DIY and has a continuous output of 120A. I wanted something around 80A but the next lowest one I could find was only 50. My entire board is overpowered, but it gives me a lot of room for improvement such as offroading.

products/torqueboards-12s-120a-car-esc-opto-hv
products/electric-skateboard-battery-epower-pack-12s4p
```

---
## \#24 Posted by: telnoi Posted at: 2018-10-02T16:28:43.713Z Reads: 65

```
For reference, I am personally using 50A bat & 80a motor x2/6374 motors. Used 4x8000mah 4
30C lipos (zippy flightmax) in the past with a theoretical output of 480A. These ended up swelling after a couple of rides and they are considered an improvement over the multistar based on experience by many. Despite of the swelling, they lasted for about a year before loosing considerable capacity (2000mah). I drain my cells to 3.7v under load.
```

---
## \#25 Posted by: Andy87 Posted at: 2018-10-02T16:31:18.674Z Reads: 61

```
Which lipos you use now?
```

---
## \#26 Posted by: telnoi Posted at: 2018-10-02T16:34:24.227Z Reads: 61

```
Right now trying heavy duty 5000mah 60c. Used them for two months now, they stay cooler and haven't puffed yet. You get around 4000mah out of them when draining to 3.7v.

I need 6 or them though to get a similar range/more range.
```

---
## \#27 Posted by: Andy87 Posted at: 2018-10-02T16:41:39.660Z Reads: 62

```
Nice! I also have the heavy duty 5ah 6s at the moment. No issues so far after two month, but I guess I don’t hit them as hard as you do 😉
Just interested how they would compete with the Graphens. They about 30-40% more expensive.
```

---
## \#28 Posted by: pat.speed Posted at: 2018-10-02T21:18:45.701Z Reads: 52

```
Please don’t get that esc, you will be very disappointed. Just because it says it can handle more current doesn’t mean it’s better. It has a bad acceleration and braking curve, it’s noisy and is not adjustable.

If you read a bit more you will understand that power is not what you think it is. I would get two Vesc’s any day of the week over that esc, they can probs do only about 40a continuous but your battery only does 60a anyway so there’s not point have anymore
```

---
## \#29 Posted by: lrdesigns Posted at: 2018-10-03T00:46:08.854Z Reads: 47

```
That esc is :poop: compared to a vesc. The ridding experience will be much more pleasant with a vesc, and there is more protections built in and adjustability. I hope you can cancel it. 

I also currently use lipo, Turnigy 5000mah 60c in 12s1p config. I would still go for the 30q pack. Lipo's are way easier to kill than the 30q. They really don't like to go below 3.7v without a drastic reduction in cycle life, so you can't really use all the watt hours.
```

---
## \#30 Posted by: TheRafter Posted at: 2018-10-03T18:25:24.190Z Reads: 46

```
do you know of a decent vesc that outputs at least 60A 12s?
```

---
## \#31 Posted by: TheRafter Posted at: 2018-10-03T18:26:00.562Z Reads: 47

```
Do you know of a good <60A 12s vesc?
```

---
## \#32 Posted by: pat.speed Posted at: 2018-10-03T20:54:49.653Z Reads: 46

```
You don’t need a 60a vesc. Your battery can only handle 60a and you need two Vesc’s so you will have 30a per vesc for a combined total of 60a. Do not try to pull more than 60a from your battery, it will result in cutouts from the bms and can cause serious harm
```

---
## \#33 Posted by: TheRafter Posted at: 2018-10-03T21:06:29.874Z Reads: 44

```
Do you know anything about this vesc? Is is any good?

https://flipsky.net/collections/electronic-products/products/torque-esc-vesc-®-bldc-electronic-speed-controller
```

---
## \#34 Posted by: lrdesigns Posted at: 2018-10-04T00:29:34.560Z Reads: 40

```
I have not used this specific one but have used the MAYTECH one. This is pretty much a standard clone of 4.12. It should run fine in BLDC mode. But in FOC mode you risk killing it, especially on 12s. Try to keep the power wires from your battery to the esc as short as possible to help the esc have an easier life on 12s. It helps reduce voltage spikes.

In regards to amps, while 30amps per esc dont seem like much I can assure you it will be enough to scare the crap out of you and put you in life and death situations quite easily. :thinking:  With a vesc you can adjust the battery amps and motor amp indepently. The battery amps is kind of like max system power 30a X 50v = 1500w per motor. But you can set the motor amps to like 60amps which effectively gives you more slow speed torque while still being within the 1500w total system power limit. 

Also motor power ratings are bull crap. There is no standard and its only a peak rating, the constant power they can handle is usually less than half that. Bigger motors get less hot. You can almost rate a motor by weight. If you live somewhere very cold you can push a bit more or if you live somewhere hot you can push less. Gear ratio / load can also have big impact on motor temps.
```

---
## \#35 Posted by: Benjamin899 Posted at: 2018-10-04T09:53:17.143Z Reads: 37

```
i use this one in combination with a focbox, but if you want performance get a focbox or go higher. If you want a beast you need reliable electronics, believe me, you will regret cutting cost. You will pay more in the end to get what you actually want.
```

---
