# Multistar 6s 8000Ah 10C in 2p?

### Replies: 22 Views: 1091

## \#1 Posted by: Acido Posted at: 2018-01-22T08:40:37.312Z Reads: 132

```
Im looking for a battery for a dual emtb for riding around the town, roads are rough here so thats why im building a emtb

My worries are if they will puff and sad with dual motors, I have red lots of negative posts about multistar but all those were in 1p configuration and because of that there was a lot more stress on the batteries.

If it wouldnt puff and sag it would be a huge 12s 16ah 710wh battery for 200$
```

---
## \#2 Posted by: Ishayc Posted at: 2018-01-22T08:45:50.422Z Reads: 129

```
What's the C rating of those?
```

---
## \#3 Posted by: Acido Posted at: 2018-01-22T08:58:24.166Z Reads: 127

```
https://hobbyking.com/en_us/multistar-high-capacity-6s-8000mah-multi-rotor-lipo-pack.html

10c
```

---
## \#4 Posted by: Ishayc Posted at: 2018-01-22T09:06:20.568Z Reads: 125

```
Are you planning on using vesc as esc?
You will be able to pull max of 160 amps from the battery(probably less because the c rating is not
accurate).
How Many amps you are going to pull?
You will probably have some sag but not something series.
```

---
## \#5 Posted by: Acido Posted at: 2018-01-22T09:14:05.587Z Reads: 121

```
Dual motors for mostly flat city max hill is 5% for 40meters

Doubt I will pull much amps like 70tops
For esc i will probably use escape vesc (vesc) or two focboxes
```

---
## \#6 Posted by: Ishayc Posted at: 2018-01-22T09:24:47.286Z Reads: 116

```
You’ll be just fine.
You will have sag but nothing to get worried about.
```

---
## \#7 Posted by: bartroosen12 Posted at: 2018-01-22T09:30:33.092Z Reads: 114

```
Yeah 12S2P 16Ah will be fine with 10C batteries, that will be a very nice pack.
Imagine that they can do like 100A with no problems, for a 12S setup that just perfect and very powerfull.
I run a 10S1P 5Ah 10C multistar pack and they don't get hot or puff.
```

---
## \#8 Posted by: Acido Posted at: 2018-01-22T10:36:10.402Z Reads: 113

```
How will there be sag with 100amp continious it just doesnt make sense to me, ify i never used lipo before and prefeer liion heavily over it but im just too lazy to make a flexible li ion pack
```

---
## \#9 Posted by: Ishayc Posted at: 2018-01-22T11:43:14.016Z Reads: 105

```
In one setup running lipo buttery I see a sag with 240A continues when pulling maximum 40A.
The sag is minor though compared to my second setup running lion with 30A continues when pulling 20A.
```

---
## \#10 Posted by: Acido Posted at: 2018-01-22T11:58:45.253Z Reads: 103

```
I have a second board, never ridden with a 80a continuous (10s4p) 30Q cells, I suppose that it wont sag at all or something that is really small, waiting on other peoples opinion on this, I would like to have batteries as small as possible without any sag, but also for them to be within my budget
```

---
## \#11 Posted by: SimosMCmuffin Posted at: 2018-01-22T12:08:03.048Z Reads: 96

```
Unfortunately there will **always** be voltage sag, regardless of load size. With smaller currents this will of course be smaller, but don't lull yourself into thinking that you can eliminate the sag completely with bigger batteries.

It's _all_ about that internal resistance that the cells have and unfortunately the most reliable way to see and test the sag is to test and monitor the battery in use. Simple Li-Po chargers that support IR-testing may give an idea what the IR is, but still the practical use and test case is very different. In actual use with prolonged discharge times and cell temperatures you might get quite different results.
```

---
## \#12 Posted by: PatRocks Posted at: 2018-01-22T12:54:00.056Z Reads: 91

```
Acido,
Exactly what @SimosMCmuffin said. Aaaand,
All I've read suggests that although not directly related, nor associated with, or measurably linked to each other, "C-rating" of a battery indicates (but does not reflect) what you might be able to expect in terms of internal resistance. I.E: A small pack with a REALLY high C-rating, like a 5000mAh 90C  pack, probably tests low on IR values, whereas a 8Ah 10C pack will drift in per-cell-voltage and sag, more than the smaller, more 'capable' battery. 

My pack, which is a 22Ah 25c 12S lipo 😈💪 can supposedly do (22*25)= 550A continuous (wtf, right??). Doesn't mean I can actually pull 550A without causing an inferno of some-magnitude. It does however, imply that this pack is going to perform predictably well under normal to extreme  (lol) demand 😎

But again, low C-rating per mAh of capacity doesn't equate to anything, it just proposes a class. Real world performance will _likely_ be better in the longrun with higher levels of quality, however suggestive and biased their metrics may be! 

Build a board after the battery, and regret not
```

---
## \#13 Posted by: Alanhunt123 Posted at: 2018-01-22T14:50:48.868Z Reads: 77

```
Your setup will probably be able to draw plenty of current when the pack is fresh and new, but I found that after around 100 cycles the multistar batteries really show how low quality they are. I used multistar 10c batteries on my first build, and within 75 cycles, some of the cells were already starting to lose a lot capacity, to the point where I was getting less than 50% range than when the board was new. It kept getting worse and worse until I finally decided to go with a 10S4P 18650 setup that has shown little signs of degradation after around 200 cycles.

The setup on my build was 8S2P with the multistar 5200mAh batteries, so it was an 8S 10.4Ah pack running a single 6364 SK3 motor, with the battery current set no higher than 50A, which the pack should have been able to handle 104A, based on its 10C rating.

Best of luck with your build!
```

---
## \#14 Posted by: Der6FingerJo Posted at: 2018-01-22T14:59:18.444Z Reads: 76

```
According to some posts on endless sphere, multistar batteries are more like 2-3C real world than the 10C  advertised by Hobbyking. I'm using 12Ah 15C Graphene Packs and they work well, but that's no comparison price wise to multistar batteries.
```

---
## \#15 Posted by: Acido Posted at: 2018-01-22T17:40:41.839Z Reads: 64

```
So 10s4p 30q it is

Just need to make it fit in a box
```

---
## \#16 Posted by: TheRafter Posted at: 2018-10-01T08:49:38.862Z Reads: 40

```
I, too, am trying to build a electric longboard. Do you know where I can get a 18650 customly built for me? I need ~900wh because I'm not using a BMT to restrict the current to the motors (Although I am using one to charge).
```

---
## \#17 Posted by: Andy87 Posted at: 2018-10-01T09:15:15.741Z Reads: 38

```
where are you located?
@Acido meanhile make custom battery packs.

900wh is a number ;)
with such a big pack you probably will not even need a bms for charging, as the balancing process would take for ever...
```

---
## \#18 Posted by: TheRafter Posted at: 2018-10-01T17:06:44.692Z Reads: 28

```
are there any reliable websites to make a custom pack? It would be much more convenient to get one online (or even just a bunch of small ones).

It should be able to easily charge fully in a whole day (24 hrs). Because its so large, it should ideally last a long time. I would need the BMS to still regulate it, and now I'm thinking twice about regulating it going to the battery. Lastly, the BMS makes sure it doesn't go below min voltage.
```

---
## \#19 Posted by: Acido Posted at: 2018-10-01T17:07:29.981Z Reads: 28

```
not if you get a bms that is always balancing
```

---
## \#20 Posted by: Andy87 Posted at: 2018-10-01T17:27:30.010Z Reads: 28

```
Ok, that might be different. Do you know of any?
As far as I know the bestech all just start balancing when reached 4.2v
```

---
## \#21 Posted by: Andy87 Posted at: 2018-10-01T17:51:39.167Z Reads: 26

```
I don’t know about a website who makes custom battery packs, but here in the forum some guys can make you a pack to your needs, just say make a thread with what you want and from where you are and i‘m sure you will get a pack done.
A bms never bad. Just in case you didn’t know, in your vesc you can set a battery cut off limit too, so that you will not discharge your pack too much. Not only the bms can do so.
```

---
## \#22 Posted by: monsterbuilder Posted at: 2018-10-01T19:01:01.531Z Reads: 21

```
My commuter board uses (2) Multistar 6S battery packs in parallel.  I've put about 60 cycles through them so far and have not seen any degradation or puffing.  All commutes are tracked for mileage and battery consumption.  

One thing to note is that I do balance the battery cells after every charge.  Also placing the lipos at storage voltage when not using the board.
```

---
