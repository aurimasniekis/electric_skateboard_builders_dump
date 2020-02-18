# Battery In Parallel

### Replies: 11 Views: 351

## \#1 Posted by: GameOver Posted at: 2019-02-21T23:44:57.948Z Reads: 135

```
I built a 10s2p battery using 30Qs a couple of months ago. Last week I got my hands on 30 samsung 30Q cells. 

OPTIONS:

A) Build a 10s3p pack. Connect in parallel (XT90 parallel adapters or XT90 using 12/14AWG wires) with the 10s2p pack to complete a 10s5p configuration. Is it safe? Should I have a BMS for each pack, or make the balance wires parallel as well?

B) Dismantle the old pack and build a 10s5p pack. Is it easy to dismantle old packs?
```

---
## \#2 Posted by: rusins Posted at: 2019-02-22T00:42:26.044Z Reads: 120

```
How did you build the first pack? I find it a bit strange that someone who has built there own pack wouldn't know how to dismantle it :smiley: You may not need to do that though, you can simply cut the balance wires and add the balance wires of the new pack in parallel correctly, and still use the same old BMS.

P.S.
I'm not sure how to safely calculate the current limits if you were to use 2 packs with different sizes in parallel with each having their own BMS :thinking:
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-02-22T00:57:26.261Z Reads: 109

```
i have a feeling  there about to be a big reveal saying that the 10s2p was actually a 30q pack from ownboard...
```

---
## \#4 Posted by: GameOver Posted at: 2019-02-22T11:03:21.921Z Reads: 88

```
I built it (sorry to disappoint @AlanZhou, no big reveal here) but I haven't tried dismantling a pack yet. I would imagine it would leave marks/burns/welds when I try to remove the nickel strips and such. And I reckon it's gonna take some time to dismantle a pack carefully. And is it advisable to use 2 month old, used cells with new ones to make battery pack?

So instead of wasting my time dismantling, I could just build a 10s3p and connect them in parallel. Hence my original query.
```

---
## \#5 Posted by: TowerCrisis Posted at: 2019-02-22T12:02:44.970Z Reads: 75

```
Yeah, you could just stick it in parallel.

Although, if you're using a charge only BMS then you WILL need two separate BMS's to balance each pack individually.

Alternatively, you could always just rebuild the pack. If you do that, make sure that you have 2 old cells + 3 new cells in each P group. That way you maintain equal capacity between the S groups.
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-02-22T18:12:06.949Z Reads: 57

```
[quote="GameOver, post:4, topic:84975"]
And I reckon it’s gonna take some time to dismantle a pack carefully
[/quote]

it actually doesn't take a lot of time to dismantle a 10s2p (1 hour tops), and

[quote="GameOver, post:4, topic:84975"]
I would imagine it would leave marks/burns/welds when I try to remove the nickel strips and such
[/quote]

^thats not how it works... unless you don't know how to handle a battery dismantling it shouldn't spark...

you could mix the old cells with the new just make sure to mix it in evenly (3 old cells and 2 new cells in parallel)
```

---
## \#7 Posted by: GameOver Posted at: 2019-02-23T00:47:00.680Z Reads: 48

```
Simple and straight to the point answer! This is the confirmation I needed. And coming from you, I know that this is solid advice. Thanks @TowerCrisis
```

---
## \#8 Posted by: TowerCrisis Posted at: 2019-02-23T00:50:08.407Z Reads: 45

```
Keep in mind you need to equalize voltage before you connect them together! Once it's together just avoid ever disconnecting and you'll never have to balance them together again.
```

---
## \#9 Posted by: Wowboard Posted at: 2019-09-02T06:16:37.716Z Reads: 18

```
Just wondering, could I put my 10s5p battery in parallel with my other 10s2p battery? both batteries are from Wowgo
```

---
## \#10 Posted by: Tinp123 Posted at: 2019-09-02T06:25:52.325Z Reads: 17

```
yes you can! if they both have bms, you can just connect them in parallel. if not or you are not sure, charge them to the same level before connecting them.
```

---
## \#11 Posted by: Wowboard Posted at: 2019-09-02T06:54:54.396Z Reads: 16

```
Cheers, much appreciated, love the longer range
```

---
