# 5&rdquo; Skike Pneumatic Build \[Germany/EU\]

### Replies: 8 Views: 981

## \#1 Posted by: Maxid Posted at: 2017-03-02T13:10:22.328Z Reads: 174

```
Hi guys,

I recently finished a board with 5" Skike pneumatics in a Dual Diagonal Drive. One SK3 149kv and one 5065 140kv Evolve clone motor hooked up to two 150A X-Car ESCs. I used them with a selfmade 6S4P 25R pack in parallel with two 3S Turnigy 5000mAh Lipos and Mad Munkey Mod GT2B. The board works fine but for me the most fun is actually the building part.
If anybody is interested let me know - I am just trying to get back what I payed in order to build the next board.

Let me know what kind of pictures you want and I'll upload them.
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-03-02T13:12:44.807Z Reads: 171

```
I am not interested in buying the board but i am really interested about the pictures.
```

---
## \#3 Posted by: Norco Posted at: 2017-03-02T13:13:47.130Z Reads: 170

```
Yes - pics and location would help :slight_smile:
```

---
## \#4 Posted by: Maxid Posted at: 2017-03-02T13:26:00.817Z Reads: 165

```
Location: Germany

Pictures: it is only half assembled right now (enclosure not attached)

This is an old one from a couple weeks ago
<img src="/uploads/db1493/original/3X/3/a/3a6703b59cb7d10745126692dd1b8da87856dabe.jpeg" width="375" height="500">
```

---
## \#5 Posted by: hexakopter Posted at: 2017-03-02T14:00:03.754Z Reads: 144

```
I am also not interested in buying, but isn't it a bad idea to combine a 6S4P 25R with a 3s Turnigy 5000mAh? First the different mAh ratings (10000mAh vs 5000mAh), but also when using the same mAh the internal resistance of the different battery packs are far off. And comparing the discharge curves of 18650er compared to Lipos let me come to the conclusion that it is a really bad idea to put them in parallel, right? I have 3 x 4s Multistar packages right now and don't know if it is a good idea to add 4 x 3s Multistars with the same mAh rating, because I think they have slightly different discharge characteristics.

And using two motors with different kv ratings and "normal" ESCs like the 150A X-Car isn't a good idea, too. At least in theory I think.
```

---
## \#6 Posted by: Maxid Posted at: 2017-03-02T14:08:46.405Z Reads: 138

```
[quote="hexakopter, post:5, topic:18450, full:true"]
I am also not interested in buying, but isn't it a bad idea to combine a 6S4P 25R with a 3s Turnigy 5000mAh? First the different mAh ratings (10000mAh vs 5000mAh), but also when using the same mAh the internal resistance of the different battery packs are far off. And comparing the discharge curves of 18650er compared to Lipos let me come to the conclusion that it is a really bad idea to put them in parallel, right? I have 3 x 4s Multistar packages right now and don't know if it is a good idea to add 4 x 3s Multistars with the same mAh rating, because I think they have slightly different discharge characteristics.

And using two motors with different kv ratings and "normal" ESCs like the 150A X-Car isn't a good idea, too. At least in theory I think.
[/quote]

it is not a single 3S Lipo but two in series to make a 6S - in parallel this should be fine: 
https://jacklithium.wordpress.com/2013/12/22/mixing-battery-chemistry-li-ion-and-li-po/
Think of it like that: Lipo gives the the boost and the Liion charges the Lipo when there is little load.
Since the LV cutoff is set to 3.4V anyway we will never get to a region where either of the chemistries is stressed too much. Also this board can be ridden with just the Lipo or just the Liion or a second Liion could be added and so on. I am not saying this is a perfectly finished board and the potential buyer will have to make his own decisions on how to use it.

KV rating does not matter - that is why you have two ESCs - they are completely independent. Also they are geared to make them similar (that is the crucial part). Even though people like @lowguido have already built uneven drives with completely "off" ratings and they perform fine.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-03-02T20:31:13.156Z Reads: 114

```
not only do they perform "fine" they kick ass!
my mates UDR frequently outperforms anything else I have built.
```

---
## \#8 Posted by: Okami Posted at: 2017-03-04T00:15:25.106Z Reads: 87

```
Im starting to wonder what deck fits those small pneumatic wheels.. long / big decks does not seem to go well together with these narrow tires.

Othwerwise.nice.build, clever.thing with.batteries, i also had a setup.with.switchable packs.but.never.ran them at the.same time
```

---
