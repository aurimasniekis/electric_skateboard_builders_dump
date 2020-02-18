# Electrics/Electronics review please?

### Replies: 4 Views: 486

## \#1 Posted by: Ragnar Posted at: 2016-09-11T12:54:32.585Z Reads: 68

```
Here's the current (no pun intended) version of my dual motor build wiring design:

<img src="/uploads/db1493/original/3X/5/b/5bf8ee53874c4ceaa48c223337832bc62ec053d2.png" width="414" height="500">

XT60 connectors on the batteries for ease of charging via my XT60 equipped balance board. I plan to wire up a couple of cables that connect two of these batteries in series to one XT90 anti-spark which will form the main connection between the pack and the rest of the board. The idea is that this will allow me to have 2 of these packs (i.e. 2 lots of 2x4S batteries wired up in the 8S configuration) charged up and ready to swap out easily. The board itself also has an anti-spark on/off switch, so I have 2 safe points to be able to shut the thing down if needed.

How does it look to you more experienced builders? Any obvious problems? Anything I've missed?

Does 8S 5Ah sound good for a dual 190KV configuration board? My calculations suggest that this should give me just under 20mph loaded top speed and about 9 miles range (per battery pack), which sounds about right for what I want to achieve for a first build. I could consider upgrading to 2x5S or more capacity later.

20C with 30C burst should allow me to draw 100A continuous and 150A burst I think - enough for the board?

Sorry for all the questions - Learning lots thanks to search but I don't have the confidence to be sure of my designs yet!
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-11T13:24:42.390Z Reads: 57

```
Battery and motors look fine and you have room to upgrade to a higher voltage in the future.

Not sure the anti spark is necessary given you have an anti spark switch. If something does go wrong and you have a spark, it's not the end of the world, you just don't want to spark so much that it builds up carbon on the terminals. If you insist on having two anti spark solutions, you should just the xt90s on a single cable instead of as a plug. I've heard of people running into polarity problems while using it as a plug and burning the resistor in the header.
```

---
## \#3 Posted by: Ragnar Posted at: 2016-09-11T14:08:06.794Z Reads: 43

```
Yeah, I did wonder about the need for the XT90S, or even just a regular XT90. Would an XT60 be good enough? As long as my switch is off then I'm not completing a circuit anywhere and therefore I don't need to worry about a spark? I guess I'm just trying to make it idiot-proof... e.g. if I leave the switch on and plug the batteries in.

I'm building on a Vanguard deck and want separate enclosures for the batteries (up front) and electronics (at the rear) because of the flex. There'll be cables running between them of course - either underneath or maybe embedded into the deck like some builds I've seen - The XT90 was going to be on the battery end of those cables - Maybe I'll just go XT60.

Not sure I understand about the polarity issues when using XT90 as a plug - will do some more searching.
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-11T14:10:52.435Z Reads: 38

```
I use xt60 on 10s4p with xt60 a parallel connector for dual VESCs, no problems with them at all. But yea, even if you spark, no big deal, just try not to do it.
```

---
