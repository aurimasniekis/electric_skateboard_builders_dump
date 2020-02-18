# Fixing Over Discharged 10s4p Battery Pack

### Replies: 19 Views: 325

## \#1 Posted by: Odysseus Posted at: 2019-08-20T16:20:30.523Z Reads: 119

```
Hi Guys,

I've built a custom 10s4p battery pack, made up of Samsung 30q cells, which has been working perfectly for some time.

Unfortunately, the pack has been over discharged to 1.9v, and I am unsure of how to safely recover the pack to a nominal voltage.

What would be the best / safest way to achieve this, to minimise any further damage to the cells?

FYI: I did not integrate a BMS due to enclosure size limitations; I'm working on fixing that.
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-08-20T19:20:40.829Z Reads: 115

```
Is the pack at 1.9v? Or the individual cells...

If the pack total is 1.9v just throw it out, no way you can Rez that :( 

1.9v per cell is really low, and you'll have a severely damaged pack if youre able to Rez it at all
```

---
## \#3 Posted by: Odysseus Posted at: 2019-08-20T19:52:45.929Z Reads: 111

```
Ah damn, ok, that really sucks.

The pack is 1.9v. :frowning:
```

---
## \#4 Posted by: skatardude10 Posted at: 2019-08-20T20:07:58.266Z Reads: 106

```
If the whole pack is 1.9V, most of the P groups are probably 0. If that's the case, I wouldn't even bother. I've revived a few 0v cells, but it's rare and their capacity and ampacity goes to shit. 99% of 0v cells I usually toss in the scrap bin for recycling, it's just pointless most of the time.

Sorry about the pack.
```

---
## \#5 Posted by: linsus Posted at: 2019-08-20T20:23:55.273Z Reads: 103

```
toss it in the bin, or cut them up for sience to see whats inside, should be relativly harmless when they're close to 0V
```

---
## \#6 Posted by: Odysseus Posted at: 2019-08-20T20:29:19.526Z Reads: 103

```
Understood. Thanks man, it's unfortunate, but luckily not fatal. Time for a new pack I suppose.
```

---
## \#7 Posted by: Odysseus Posted at: 2019-08-20T20:30:20.891Z Reads: 101

```
I think you're on to something. :slight_smile:
```

---
## \#8 Posted by: Jonisonvespa Posted at: 2019-08-21T20:19:32.652Z Reads: 85

```
there are ways to revice cells
```

---
## \#9 Posted by: ShutterShock Posted at: 2019-08-21T21:50:56.136Z Reads: 79

```
Not at that low voltage - and even if you do their capacity would be useless
```

---
## \#10 Posted by: skatardude10 Posted at: 2019-08-21T23:35:09.065Z Reads: 75

```
Yeah, sometimes popping them on the charger works. Sometimes just connecting a battery + resistor in parallel works. I try to not salvage any cells below 2.4v, 2.2-2.3 if I'm desperate. 1.9 and below are trash imo.
```

---
## \#11 Posted by: deucesdown Posted at: 2019-08-22T14:39:33.644Z Reads: 70

```
You can try, but it's tedious and somewhat dangerous. You need a lab power supply. Charge the pack at something like 100mA per cell until 3v (30v 1A for your 10s4p) measuring each group's voltage often, and feeling for heat. If cells get warm or voltages yo wonky stop -- will probably need to take the pack apart at that point to salvage what you can.

If you make it to 3v per cell you can increase current (maybe 500ma per cell) and charge to full, still monitoring heavily. All this will take like a whole day or two.

As the pack gains charge, the chances of a big fire increase.

If you make it to full, you can do some careful test rides. Don't pull hard and check the pack often.

It's very unlikely the whole pack is still working, and even if it charges to 4.2v per cell, capacity and power are likely very diminished. And the pack will be hard to keep balanced.
```

---
## \#12 Posted by: Jonisonvespa Posted at: 2019-08-22T15:04:28.442Z Reads: 60

```
id buy a quality 18650 charger, and try to charge them, if they do charge, try and cycle them charge discharge a few times
```

---
## \#13 Posted by: skatardude10 Posted at: 2019-08-22T15:47:20.564Z Reads: 58

```
I'd recommend the litokala lii-500 charger. It's cheap and can automatically do full charge, discharge and recharge cycles testing capacity, internal resistance, with charge rates from 300, 500, 700 and 1000ma settable individually for each of the four slots. This has been the best $25 I've spent on recycling wastes batteries.
```

---
## \#14 Posted by: deucesdown Posted at: 2019-08-22T16:33:19.574Z Reads: 49

```
Makes sense to get a few units if you're dealing with lots of cells. 5 units will let you test 40 cells in 2 rounds instead of 10 lol. Each round takes like a whole day, right?
```

---
## \#15 Posted by: Jonisonvespa Posted at: 2019-08-22T17:22:07.447Z Reads: 47

```
ive got one of those chargers perfect
```

---
## \#16 Posted by: skatardude10 Posted at: 2019-08-22T20:00:42.455Z Reads: 41

```
Yeah I was going through tons of cells for a few weeks, since I only have one charger lol.

If I remember correctly, it takes anywhere from 8-16 hours depending on the cells current state of charge to cycle them and recharge.
```

---
## \#17 Posted by: Goa Posted at: 2019-08-26T04:28:17.684Z Reads: 37

```
I work with batteries, my advice is to toss them into recycle bin. They aren't safe anymore.
```

---
## \#18 Posted by: clistpdx Posted at: 2019-08-26T16:18:26.100Z Reads: 30

```
I recently had an [11s3p battery stored on a shelf](https://forum./t/dead-battery-or-recoverable/6684?u=clistpdx) that I discovered had dropped to 5V total. I trickle charged it for a few days and it has now been restored to the full 46.2V. There may still be hope for your battery depending on the circumstances.
```

---
## \#19 Posted by: aos64 Posted at: 2019-08-29T20:12:05.680Z Reads: 19

```
as others said,you can try to trickle charge to revive cells but even its successfull cells probably gonna lose big chunk of their original capacity and probably max discharge rate.you can also tore apart one parallel group and test on those thus reducing the overall risk of the process.you can use cv/cc power supply,paralleling dead cells with good cells in parallel to bump the dead cells voltage(its best to do it with resistors in parallel to reduce amp flow)and even tp4056 can be used if there is still some voltage in the cells.

there is another possibility tho.are you sure your cells didnt just popped cid fuse?im not quite sure about 30qs but most of the cells has CID fuses in them,it pops when overdischarge/overheating occurs.if thats the case you can fix that easily.however i think it damages the fuse when you pop it back in so it might not work the next time fuse is needed thus making your cells pretty much unprotected cells.

i would try to revive them but im trying to build esk8 battery from salvage low discharge cells just like my mini powerwalls lol so im not a guy you want to listen to.
```

---
