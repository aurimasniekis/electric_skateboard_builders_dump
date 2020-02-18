# How many 18650 batteries needed?

### Replies: 10 Views: 4122

## \#1 Posted by: Airmacx Posted at: 2016-06-06T14:06:24.903Z Reads: 169

```
I was told that 18650 batteries are slimmer, which is what I want for a slim low profile and minimal cabling shown. But how many do I need? And can I put them in any certain order and size to make things fit or do they have to be put in one big series pack.
```

---
## \#2 Posted by: delta_19 Posted at: 2016-06-06T14:12:50.341Z Reads: 165

```
I would say 30 and they can be wired up how ever you want as long as you get the voltage you need
```

---
## \#3 Posted by: Airmacx Posted at: 2016-06-06T14:17:22.580Z Reads: 167

```
How do I determine the voltage needed?  Sorry if I'm asking some dumb or obvious questions, new to  DIY and electronics in general.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-06-06T14:18:51.823Z Reads: 161

```
Generally you need about 6S (22,2V = 6 cells in series) to 12S (44,4V = 12 cells in series). You will determine the voltage by your electronics, motor and the expected max speed too.
```

---
## \#5 Posted by: Airmacx Posted at: 2016-06-06T14:22:44.362Z Reads: 152

```
I see. I've got a Tacon Bigfoot 160 motor and don't really intend on going above 20mph. Where do u go fron there?
```

---
## \#6 Posted by: DeathCookies Posted at: 2016-06-06T14:29:47.635Z Reads: 141

```
You have many options to decide! First of all i prefer a higher voltage because low voltage means more ampere and more heat... (any) motor is not performing that well with low voltage....

Use this [calculator](http://toddy616.blogspot.de/2013/07/electric-skateboard-calculator.html) to calculate the needed pulley size / voltage.
```

---
## \#7 Posted by: Ulfberht Posted at: 2016-06-06T19:11:26.714Z Reads: 122

```
Start here and read through. Follow the links and stuff and just get deep in it, bro.
http://www.electric-skateboard.builders/t/start-here-faq-for-diy-electric-skateboard-builders/215
```

---
## \#8 Posted by: karma Posted at: 2016-06-06T20:00:31.633Z Reads: 114

```
It all depends on how many amps you safely you want to pull out of the batteries and much range you want. I would suggest looking into @whitepony's post about 18650 Li-Ion packs, there is a a lot of good info in his posts.
```

---
## \#9 Posted by: Ulfberht Posted at: 2016-06-06T20:09:39.721Z Reads: 114

```
Here's a quick breakdown:
Each cell is about 3.7v you will need to connect as many of these "cells" in series as you need to get to the desired voltage. Each "cell" can be wired in parallel to raise the capacity of the pack and also increase the amp output. 
10 cells=36v nominal 
So let's say a 10s3p pack would be 10x "cells" consisting of 3x18650 battys. For a total of 30. 
8s2p would be 8x packs of 2. Does that make sense?
```

---
## \#10 Posted by: whitepony Posted at: 2016-06-06T20:41:04.016Z Reads: 107

```
the order of things is fairly simple:

first you decide **how many** cells you are going to use - which kind of only depends on the room of the board you are running and the enclosure you want to set up. also maybe the target weight of your board (one cell = 46-48gramm). the more cells the better obviously, many cells share the load, less heating of cells, less aging, more range, less voltage sag - there is no downside except the price and the weight.

next you think about your **target speed**, gearing, wheelsize, which motor you want to use -> this will determine the **number of cells in series**, since the motor "KV" numbers means RPM per Volt. youll know that, to reach a certain speed, your motor will have to turn at a certain RPM. with the KV rating of the motor, youll know which voltage you need. you divide that voltage by 3.6 and youll know how many cells you need in series.

now you divide your "total number of cells" by "number of cells in series" and youll know how many cells you have left for "cells in parallel"!

now youll have to think about how much power your setup is supposed to run - dual motor with 2.5kW each? 50kph constant burning or just relaxed cruising at 30kph with a single motor? I would say 60A for a single setup vesc and 2x 30-60A for a dual setup vesc is a reasonable value, so your battery should probably deliver something between 60 and 120A. this max current divided by the number of parallel cells will determine the amount of current per cell. 

lets say you build a 10S4P battery like mine, this means youll have 10 cells in series for a nominal voltage of 36V and 4 cells in parallel. I know that my vesc can take about 60A battery current, but beyond that I might blow it up, so my battery should be able to run 60A continuously. that means 60/4 = 15A per cell. that also means 36V x 60A = 2100Watt continuous power!
most good high capacity cells are rated 10A continuous current, so thats not enough - if you use such cells they will heat up and heat kills cells quickly. Im using LG HG2 for my battery, since they are rated 20A continuous current with 3000mAh capacity - this will provide me 4x20 = 80A continuous current - a nice headroom with nearly 2900Watt continuous power to the 60A I was aiming at!

probably a bit much in one post, but thats basically the order of things ;)

you can finetune with motor KV values, gearing, but I would say the bigger the motor pulley the better (which usually means 15-16T), so whats lets is the motor kv.
```

---
