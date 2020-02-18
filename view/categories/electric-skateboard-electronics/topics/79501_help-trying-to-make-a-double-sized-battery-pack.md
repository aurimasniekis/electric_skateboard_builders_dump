# *HELP* Trying to make a double sized battery pack!

### Replies: 8 Views: 315

## \#1 Posted by: ethanfields Posted at: 2018-12-31T23:21:04.686Z Reads: 108

```
Hey all! I'm really new to esk8 community and I have obtained two Koowheel 5500mah batteries for the board. I understand that the batteries are swappable, however my question is... Could I take two of the koowheel batteries and put them on top of eachother and then, make both power sources run into my board?? If so how would I go about doing so?![1pcs-free-shipping-36v-5-5ah-Koowheel-battery-for-electric-skateboard-D3M-self-balance-scooter-longboard|500x500](upload://4G9gQaX08DLWgR6p62w593CLTfU.jpeg) ![battery-koowheel-kooboard-d3m|690x345](upload://eLXDZHqdAbNqgEXSl1gVImo5nGt.jpeg)
```

---
## \#2 Posted by: b264 Posted at: 2018-12-31T23:22:02.314Z Reads: 101

```
You can connect them in parallel but they need to be the exact same voltage when you connect them together, and DO NOT disconnect them from one another when you charge them.  If you accidentally connect them backwards, you will have created a fire starting device, so don't do that.
```

---
## \#3 Posted by: ethanfields Posted at: 2018-12-31T23:24:53.833Z Reads: 93

```
So would I Connect them together and run both of them into the board?? And then charge them by using the charging port on the board?
```

---
## \#4 Posted by: TowerCrisis Posted at: 2018-12-31T23:31:20.602Z Reads: 88

```
Connect them together once and then never disconnect them from each other.

Ensure that they are the same voltage as each other when you initially connect them together.
```

---
## \#5 Posted by: ethanfields Posted at: 2019-01-01T00:02:29.022Z Reads: 81

```
Okay sweet
```

---
## \#6 Posted by: skatardude10 Posted at: 2019-01-01T01:41:34.109Z Reads: 69

```
If I can sidebar the thread a bit but still related to paralleling multiple packs...

Why never disconnect? Are you assuming they are both new, to keep them in sync?

Even random, oddly sized, varying health, different internal resistance cells in parallel will tend to keep each other balanced at the same voltage... Right? Otherwise people wouldn't be able to build massive powerwalls of recycled batteries or salvage old cells for other uses.

I only ask because I want to connect a few 6S packs in parallel with each other. One has a charge only BMS and it's about 400Wh, while the other has presumably just a balance module of some sort and it's 50-80Wh or so. I was under the assumption that as long as they start at the same voltage, they can be plugged in in parallel and as they both get used they will tend to stay around the same voltage as they will keep each other balanced... And I'd be disconnecting and reconnecting them to charge them both separately and individually as modules... Just making sure they are both fully charged when putting them together.
```

---
## \#7 Posted by: TowerCrisis Posted at: 2019-01-01T03:42:49.719Z Reads: 52

```
It doesn't matter if they're new or not, but it does matter to keep them in sync. You want to just "set and forget". Aka, deal with it once and never have to worry again.

Yes, differently sized cells will keep each other balanced. But they MUST start at the same voltage, otherwise it's essentially a dead short from one to the other dumping capacity.

[quote="skatardude10, post:6, topic:79501"]
And I’d be disconnecting and reconnecting them to charge them both separately and individually as modules… Just making sure they are both fully charged when putting them together
[/quote]

This is a surefire way to ignite your pack.

The different capacities are okay, so long as both have the same series count and both have a BMS or both have no BMS for discharge.

But charging them separately is just a mistake waiting to happen, especially since one has a BMS and the other doesn't.

For all you know it could be "done" charging, but the BMS needs to continue balancing, or some other issue. If the voltage drops a little it'll suck up power from the other. That's probably okay because the voltage difference would be minimal.

But if you forget to fully charge one? Oh boy, it will literally explode or you will melt the plug as you connect it.

In the case of incompletely charging it and forgetting, or let's say you charged it a few days ago (or at least THINK you did, even if you're SURE) and you accidentally mess up... It's bad.

That's why you shouldn't leave it up to you, human error will eventually cause a problem.

Just charge them together in parallel if you can. If they've both got balance circuitry then you can charge them together.
```

---
## \#8 Posted by: skatardude10 Posted at: 2019-01-01T04:40:59.563Z Reads: 39

```
Got it! So it boils down to if I'm not a dumbass and charge 100% and allow for balancing of each packs six serial groups prior... 

Basically your argument is why I haven't plugged them in parallel yet, despite having it wired in to just slot it in... I'm still afraid I'll dumb out at some point like I did having the same size charge port for different voltages once.

I think I'll just let it be and run one pack at a time. I'd reconsider if I were doing two exactly the same brand new packs that I could get together, set in parallel and forget, *as one* if it were. Thanks for the insight.
```

---
