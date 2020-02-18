# Power button on ESC or battery enclosure

### Replies: 11 Views: 336

## \#1 Posted by: mikepurvis Posted at: 2019-09-19T16:47:28.588Z Reads: 84

```
Currently planning out my first build (pretty much foosted: dual 6355, VESC6, Ownboard battery) and have a question about the power button story. Flipsky's "Dual FSESC6.6 Plus" controller has the power button logic built in, so you just plug in a $5 switch instead of needing the external $50 circuit for that. The cost is similar, though, since the mini version of that board without the power switch stuff is ~$50 cheaper.

I'm generally a fan of having things integrated, so I was initially thinking of using that plus controller, but the consequence of it is that the power button for the board will be on the ESC enclosure rather than the battery enclosure, and the braid running over the board between the enclosures will be hot even when the board is powered off. This creeps me out, and for this reason I'm now leaning toward using the mini ESC and the standalone switch circuit, so that the switch circuit is tucked into the battery enclosure.

Anyone else given these issues any thought or want to push me one way or the other on this?
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-09-20T16:43:42.087Z Reads: 70

```
Loopkey everyday. 

(Very nearly) Every antispark switch on the market will fail eventually, either while you're on the board, or when you turn it on or off. The only one I don't think I've ever heard of breaking was the Fatboy switch, but it has a high ambient powerdraw... 🤷 Could be worth it to you.

Loopkeys don't suffer any of those issues, but instead are able to be lost or misplaced and then you can't ride until another one is made 🤷

Additionally, a loopkey can take up to whatever electricity rating the connector/wires can, yet a antispark is limited to the ability it's own board(some are better than others)
```

---
## \#3 Posted by: mikepurvis Posted at: 2019-09-20T17:54:27.166Z Reads: 65

```
Can you explain more about the difference or link me to other relevant threads? I googled a bit and it's not obvious to me what I'm looking at. A conventional anti-spark is just one or more resistors with bypasses to slow the inrush as your motor controller capacitors are precharging, right? What is different about a loopkey?
```

---
## \#4 Posted by: mikepurvis Posted at: 2019-09-20T19:59:13.657Z Reads: 60

```
Okay, having browsed a bit further, it appears that a loopkey is really just a high amperage connector with the two pins shorted together— so you don't have any anti-spark or precharge, but the loopkey itself is cheap enough that you basically just have it as a sacrificial component and replace it when it wears out.

Not going to lie, but this seems pretty sketchy to me. If there's concern about the heat and lifespan of the FETs in an anti-spark wearing out, wouldn't it make sense to design one around a socketed relay instead? An 8-bit AVR with a few ADC pins should be more than enough to run it.
```

---
## \#5 Posted by: murdomeek Posted at: 2019-09-25T18:31:58.505Z Reads: 47

```
look up as150 mechanical antispark switch

better implementation than loopkeys.  cant loose it, and can support 150a
```

---
## \#6 Posted by: Tinp123 Posted at: 2019-09-25T18:49:04.027Z Reads: 47

```
Did I understand you right? Wires between vesc and battery are always hot, even when board is turnes off?
```

---
## \#7 Posted by: mikepurvis Posted at: 2019-09-26T00:42:01.053Z Reads: 45

```
Yeah, that's why I'm not in favour of that option— it would make sense if the battery and ESC board were in the same enclosure together, but since they're separate, the button should be with the battery.

Have people in general had good experiences with the dual-VESC boards? I don't have a sense how often an ESC fails, but if it's any more often than "pretty rare", then it might be better to use two single channel ones rather than a dual channel, even if it's pretty convenient having a dual for not needing a separate canbus wire.

As to the power button itself, I think I'll build a proper precharge based on the design that @Pryside published here: https://drive.google.com/file/d/1kMG3GBcZCPoe54R4nuCTkw7K1juGhK98/view This eliminates the spark and inrush altogether instead of just moving it inside a couple FETs that burn out.
```

---
## \#8 Posted by: Flasher Posted at: 2019-09-26T04:52:59.020Z Reads: 40

```
[quote="mikepurvis, post:4, topic:101997"]
anti-spark
[/quote]

Have you looked into xt90 **S** connectors? They include a resistor inside to act as an antispark. They are what we use to make our loopkeys
```

---
## \#9 Posted by: Pryside Posted at: 2019-09-28T20:54:21.518Z Reads: 32

```
I have even made a fully assembled PCB Pre Charge Antispark that you can buy now. :)


https://www.electric-skateboard.builders/t/3d-printed-boosted-board-killer/88803/177?u=pryside
```

---
## \#10 Posted by: mikepurvis Posted at: 2019-09-30T19:50:03.145Z Reads: 22

```
@Pryside Thanks! I will give that some consideration, though I may end up just making my own on perfboard given that I'll be ordering other digikey stuff anyway for this.
```

---
## \#11 Posted by: Pryside Posted at: 2019-10-01T17:29:44.908Z Reads: 15

```
nice, good luck. Use some esd protection, these mosfets can be destroyed very easily
```

---
