# 11s Dischargable BMS, Does Thou Exist?

### Replies: 20 Views: 750

## \#1 Posted by: Jc06505n Posted at: 2018-05-22T17:17:31.425Z Reads: 95

```
I've search and cant find any BMS for 11s, every supplier skips from 10s to 12s. Anyone know of any 11s BMS that are out there?
```

---
## \#2 Posted by: BoostedBuilder Posted at: 2018-05-22T17:39:45.388Z Reads: 88

```
You can use a 12s BMS as an 11s BMS : )

Or: http://bestechpower.com/407v11spcmbmspcbforli-ionli-polymerbatterypack/
```

---
## \#3 Posted by: Jc06505n Posted at: 2018-05-22T17:54:23.278Z Reads: 80

```
You beautiful Bastard, 

So [this](http://bestechpower.com/407v11spcmbmspcbforli-ionli-polymerbatterypack/BMS-D298V1.html) 

would be the 11s version of 

[these](https://buildkitboards.com/collections/batteries/products/bestech-bms?variant=7201537687582) ?
```

---
## \#4 Posted by: BoostedBuilder Posted at: 2018-05-22T18:12:35.397Z Reads: 71

```
[quote="Jc06505n, post:3, topic:56363"]
You beautiful Bastard
[/quote]
😘

Not really, no. [This one](http://bestechpower.com/407v11spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html) is the 11s version of [this one.](https://buildkitboards.com/collections/batteries/products/bestech-bms?variant=7201537687582) But I think Bestech no longer sells them, and released [this new version.](http://bestechpower.com/407v11spcmbmspcbforli-ionli-polymerbatterypack/PCM-D596.html)
```

---
## \#5 Posted by: Deckoz Posted at: 2018-05-22T18:15:15.126Z Reads: 66

```
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F222373438927


https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F263603764507
```

---
## \#6 Posted by: Jc06505n Posted at: 2018-05-22T18:18:06.033Z Reads: 57

```
I see interesting , guess I have to hit them up to buy it?
```

---
## \#7 Posted by: BoostedBuilder Posted at: 2018-05-22T18:18:39.349Z Reads: 56

```
Yes, write them an e-mail, but I think their MOQ is 2 pcs.

sales@BesTechPower.com
```

---
## \#8 Posted by: Deckoz Posted at: 2018-05-22T18:18:53.727Z Reads: 59

```
They restock ever couple weeks. Just add it to watch list and wait :) err..nvm not me..
```

---
## \#9 Posted by: Jc06505n Posted at: 2018-05-22T18:20:46.399Z Reads: 56

```
Bear with me Deckoz , we’re going to dwell deep into my stupid questions here...


Since this is for an 11s3p 30Q pack, is 20 A enough or should I shoot for 80A like on Jlabs Site? 


And that charger should work for the one @BoostedBuilder just linked right?
```

---
## \#10 Posted by: Deckoz Posted at: 2018-05-22T18:21:32.855Z Reads: 51

```
I missed the discharge part. This would be charge only bypassed discharge.
```

---
## \#11 Posted by: Jc06505n Posted at: 2018-05-22T18:21:52.909Z Reads: 49

```
[quote="Deckoz, post:8, topic:56363"]
wait :slight_smile: err…nvm not me…
[/quote]


![image|375x500](upload://ehQLwSnG8zrwej86HUneyiwAsyE.jpeg)

Tell me what you know
```

---
## \#12 Posted by: Deckoz Posted at: 2018-05-22T18:24:57.769Z Reads: 46

```
Honestly I try to stay away from discharge BMS.. there's plenty of topics why..so I can't help much with sourcing them as I don't look for discharge BMS/keep bookmarks etc.

Anyway that charger would work. 4.2v*11s=46.2v, id probably change the xlr to a different plug though...
```

---
## \#13 Posted by: Jc06505n Posted at: 2018-05-22T18:26:26.588Z Reads: 48

```
Interesting, I thought the sentiment was that getting Discharge BMS was safer than getting a charge only BMS (as well as less work). 

Thank you both btw
```

---
## \#14 Posted by: Deckoz Posted at: 2018-05-22T18:36:02.702Z Reads: 49

```
Discharge will help protect the battery if there is a short on the load side so it shuts down outbound current. If you build and isolate your wiring properly you shouldn't have a short capable on the power wires from battery to ESCs. 

The bigger part - related to personal safety. Discharge BMS can cut current if your pulling to much. This could cause your body to fly forward off the board when acceleration cuts out and you aren't expecting it.

The other part of that is braking, if your battery is full, or the Regen current is to high, can cut off regeneration. While the ESCs will still brake for a second,it will quickly go into over voltage protection leaving you with no brakes.

The ESC can properly prevent over discharge like a BMS, provided you setup your voltage cutoffs right.

So there are many sides to the coin. My opinion personal safety is the highest. Being as high amperage BMS cost more money, and take up alot more space, and add heat to the enclosure. I tend to stay away. Basically if I did use a discharge BMS. It would have to be 20-30a higher then the max battery ampers combined set on the ESCs. (Ie dual with 30batt max for a total of 60, I wouldn't use less then an 80A discharge BMS)


Anyway don't wanna clutter your thread.. there are plenty of topics regarding this.. but food for thought..
```

---
## \#15 Posted by: Jc06505n Posted at: 2018-05-22T19:12:33.184Z Reads: 47

```
Interesting, it seems every path has its hiccups. 

Charge Only BMS require the use of Antisparks Switches (or fugly lookpeys) with very very few reliable retail ones making them the weakest link, 

Dischargable BMS have inherit risk that sacrifices space for thoughts of reliability. 

ESK8 parts really has a long way to go.
```

---
## \#16 Posted by: Acido Posted at: 2018-05-22T19:14:04.116Z Reads: 44

```
bestech has 11s bmss
```

---
## \#17 Posted by: Deckoz Posted at: 2018-05-22T19:23:47.116Z Reads: 43

```
[quote="Jc06505n, post:15, topic:56363"]
Antisparks Switches (or fugly lookpeys) with very very few reliable retail ones making them the weakest link,
[/quote]

I thought this for the longest time too... Then I did this and moved on. I can't loose it. It won't fail. And it fits. All I gotta do is push it in or pull it out..

![15270169924901449405450|666x500](upload://BKye1P4xZqD5qlANfazNc1TH0O.jpg)
![1527016900824597593010|375x500](upload://oJcgFEEY2CpgfQDOiiXUK9MRoLn.jpg)
```

---
## \#18 Posted by: Jc06505n Posted at: 2018-05-22T19:37:41.301Z Reads: 40

```
Ohh Interesting, Does that act similar to a loop key?
```

---
## \#19 Posted by: Deckoz Posted at: 2018-05-22T19:41:53.613Z Reads: 41

```
That is my loop key..

It's an AS150. Basically a bullet connector with a resistor in it to charge the system. Just like a XT90S has a resistor to charge the system and prevent a spark.
```

---
## \#20 Posted by: b264 Posted at: 2018-05-22T19:49:40.754Z Reads: 40

```
@scepterr has connected a 12S BMS to an 11S battery successfully
```

---
