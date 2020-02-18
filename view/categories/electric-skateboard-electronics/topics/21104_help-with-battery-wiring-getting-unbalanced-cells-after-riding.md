# Help with Battery Wiring, getting unbalanced cells after riding

### Replies: 16 Views: 1579

## \#1 Posted by: riva_00 Posted at: 2017-04-15T22:17:52.374Z Reads: 168

```
I'm getting worryingly uneven cell voltage after riding.
I've literally only been out 4 times, but I think my wiring must be wrong in some way. Or perhaps may be too n00bish.
Any help here is appreciated, I'd just like to know what others have done to solve this problem, as it must've already been seen.

1st, please take a glance at my build: -

https://www.electric-skateboard.builders/t/the-cat-gullwing-sidewinder-2-trucks-dual-enertion-r-spec-6355-190kv-alien-drive-mounts-8s2p-18650-25r-vesc-psychotiller-wheels/10305/9

I've got 5 5s LiPo packs, and I wire them in series to make a 10s1p. After riding twice, I noticed both times that the cell at the end was about 3.15V, and the rest were about 3.4ish, I didn't think to note them all down at the time, but I know they were quite far apart. on the 2nd ride i noticed that one cell was at 3.01V, and some of the rest were quite higher at about 3.3/3.4
Best I've got is 5.5 KM with those battery's, which isn't very good really, but I wonder if that's the drag from the wheels and relative large belt I'm using. I'm going to be asking psychotiller about this issue separately though (just want this thread about the battery ideally)

Thinking it might be the battery's I'm using, or maybe that I just had one bad pack. I tried with 2x 6s graphene battery's (222WH), which got me 8KM, but when I checked the cells (good job I did), 2 of them in pack one were at about 3.05V, and the rest in the pack 2 were quite higher at about 3.5/3.6ish.

It seems as if certain cells in a pack (the pack which is connected directly to the positive?) are discharging more than the rest, and it's affecting my already disappointing range as i have to stop much earlier than I'd like

I've attached a pic of my wiring and my VESC settings below. However the VESC's share an XT90 that splits the power, which gets wired directly to the battery packs.

<img src="/uploads/db1493/original/3X/6/0/60591f3eda62db10ed33581009354769898ab569.jpg" width="690" height="301">

<img src="/uploads/db1493/original/3X/4/4/4407bde38ebbcd25c64bd8839ad652c83a846f0d.jpg" width="690" height="419">

<img src="/uploads/db1493/original/3X/0/1/01125db81fa90711ee9f866c4b2b3eaab3dc2c61.jpg" width="690" height="415">

I'm going to order a BMS from Bestech tomorrow, hopefully that'll come soon. Is that the solution? Or can i wire it differently so that power is drained more evenly?
Also, just a thought, but I was going up and down some hills in my 8km ride with the 12s graphene battery's, could it be that the VESC is re-charging the battery's wired closest to the negative from the VESC's?

@Namasaki @psychotiller, sorry but I want to tag you in for your help, as I know you have builds using similair setups, and I could use some knowledge from veteran builders :slight_smile: , I hope you can offer some insight into this.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-04-16T00:05:39.443Z Reads: 136

```
On the 5x2s setup where one pack is falling much faster than the rest, it could be that the one pack has much higher internal resistance than the rest.
Example, If 4 packs have total of 4 miliohms each and 1 pack is 10 miliohms, That could be the issue.
There are basically unmatched set
The BMS will not make them discharge evenly but it will stop you if any cell drops down to 3.0v
If you can find a Turnigy IR meter, you can use it to test your packs and see what they are.
http://www.rapidrcmodels.com/turnigy-lipoly-battery-ir-meter-2730-p.asp
```

---
## \#3 Posted by: riva_00 Posted at: 2017-04-16T00:32:04.958Z Reads: 128

```
Just tested the battery resistance.

one 6s graphene pack is 001,001,003,001,002,000
the other is 001,000,000,004,001,002

Is the above within tolerances?
I'll test the 2s ones in the morning as it's 01:31 in the UK right now :slight_smile:
```

---
## \#4 Posted by: Namasaki Posted at: 2017-04-16T00:51:09.278Z Reads: 123

```
What did you use to test them?
You have to use the Turnigy ir meter.
I don't think you can measure it with a multimeter.
```

---
## \#5 Posted by: riva_00 Posted at: 2017-04-16T18:55:03.350Z Reads: 117

```
I used my IMAX B6 charger, it has the functionality built-in.
Should I be possibly using higher gauge wire? Most of it is 10awg, but I used 12awg and 4mm banana plugs to connect to the female XT90 connections coming off of the battery packs, I would have used an XT90, 10awg and bigger connectors,, but I ran out of XT90, so used what I had for the time being.

After going for a quick ride this morning they seem to be all balanced @ 4.85 (charged fully to 4.20 before setting off), almost all are at that voltage (0.01 difference).
Can't ride any more as it's now decided to rain.....I'll test the 2s battery's once the dog gets his walk :slight_smile:
```

---
## \#6 Posted by: Eboosted Posted at: 2017-04-16T18:59:26.668Z Reads: 112

```
4.85v? That's too much are you sure are using a 42v charger? You shouldn't exceed 4.2v even during charging?
```

---
## \#7 Posted by: SimosMCmuffin Posted at: 2017-04-16T19:22:28.184Z Reads: 106

```
I'm pretty sure he typo'd the voltage and meant 3.85 V, otherwise I think the pack would have atomized itself into the atmosphere.

@riva_00 Have you tried using the other packs and seeing if they exhibit the same problem? At first glance I would suspect just bad quality cells with lower capacity, but I'd like to see you test the other packs as well just to isolate a possible cause.
```

---
## \#8 Posted by: riva_00 Posted at: 2017-04-16T19:49:37.474Z Reads: 105

```
Yeah was a typo, meant to say 3.85.
Resistances of the 5x 2s ones are: -

005 003, 005 003, 004 002, 006 003, 002 004.

Is there a cheap discharge tester out there that you guys use? Perhaps it's the cell capacity and not the resistance?
What's weird is that I'm not getting good range at all, probably about a 3rd of what I thought i should be getting, wonder if that's related......
```

---
## \#9 Posted by: laurnts Posted at: 2017-04-16T20:04:04.809Z Reads: 96

```
I think battery is dead. Discharging lipo under 3.6v is just damaging cells in general. Then every next charge or discharge that went below 3.6v mark again will just continue pressuring the lipo cells till it goes out of balance.
```

---
## \#10 Posted by: Namasaki Posted at: 2017-04-16T21:18:40.882Z Reads: 101

```
.005 ohms is acceptable for Lipo cells. Any higher and your gonna want to keep an eye on it.
That said I would not panic over .006 ohms
But if any cell gets up to 010 ohms, you might want to pull that pack out of service.
Still, looking at your numbers, seems your 2s packs are not very well matched.
 As for wire gauge.
I use 12g for my battery wires. I feel that it's heavy enough and easier to solder than 10g.
However, "bigger is always better"
```

---
## \#11 Posted by: riva_00 Posted at: 2017-04-16T21:30:59.617Z Reads: 97

```
@laurnts You sure? Everything I've read says LiPo nominal voltage is 3.7, and safe drain is about 3.2/3.3 (depending where you read), absolute minimum is 3.0, and anything under that damages them.
Think I'm gonna flash ackmaniacs firmware on the VESC and connect a bluetooth module to it and get some real-time data about what's going on here, @psychotiller seems to think the wheels don't affect the rolling efficiency that much, either way my range is lousy.... 

Ackmaniac's firmware I'm going to use: -
https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286

Hopefully should mean easier speed control as well.
```

---
## \#12 Posted by: Ackmaniac Posted at: 2017-04-16T21:33:24.761Z Reads: 86

```
Please make a video with the app and post a video. I would be interested as well about the Wh consumption of pneumatic wheels on the streets.
```

---
## \#13 Posted by: psychotiller Posted at: 2017-04-17T00:05:34.258Z Reads: 79

```
@riva_00 did you read what I said? I said it depends on which wheels you have. There are definitely effects.
```

---
## \#14 Posted by: riva_00 Posted at: 2017-05-04T23:38:54.347Z Reads: 57

```
@psychotiller, Looks like my expectations were way too high, probably caused by a mixture of excitement and stupidity.
Evolve halves their range when using AT wheels so I'm doing the same, I also need to repair my shoddy work so i'll be getting on that over the weekend hopefully.
Got lots to do over this weekend and beyond, and I've put my plans in my build thread. I hope to make some progress and have something to show for it soon.

I'd still really love to see your average KM per WH for comparison, I'm going for 22~26ish WH per KM since my areas fairly hilly and I also go a little off-road (forest parks).
```

---
## \#15 Posted by: psychotiller Posted at: 2017-05-05T00:59:47.925Z Reads: 56

```
Evolve stroller wheels are a joke. Not even in the same ball park with mine. My v1 and v2 wheels kill that margin. I'm hoping someone who has run visible comparisons will chime in here. @caustin ?
```

---
## \#16 Posted by: riva_00 Posted at: 2017-05-17T19:57:55.259Z Reads: 49

```
Got some 90mm urethane wheels from @atenner, hoping to test and compare the range soon.
@Ackmaniac, I've been running your firmware but I've been too busy recently to repair my boards motor mounts and get riding, hope to change that soon and post some data. I'll have 90mm thane (clones), 150mm psychotiller billet hubs (V1) and 3d printed @Maxid specials out on the road soonish, just need to make sure my new epoxy mixture does it's job this time.

I should also say that I'm not in a particularly flat area, all the roads are quite hilly so I'll have to take care to take the exact same route when riding during testing, and maybe do it 3 times with each setup to get an average.
```

---
