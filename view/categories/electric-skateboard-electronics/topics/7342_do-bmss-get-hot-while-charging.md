# Do bms&rsquo;s get hot while charging?

### Replies: 10 Views: 1207

## \#1 Posted by: evoheyax Posted at: 2016-08-09T03:42:47.160Z Reads: 127

```
I was wondering, does a bms usually get hot while charging? I ask because I've decided to 100% scrap my space cell for cells and parts, so I can shape it for my board, and add another p to make it 10s4p.if the bms does not that hot, I can remove its heaksink. The bms is simply being used for charging, and I'm discharging around the bms.
```

---
## \#2 Posted by: paragon Posted at: 2016-08-09T03:59:43.418Z Reads: 125

```
I'm charging at 2a right now, and my bms is getting warm (with the heatsink), but not too hot to touch. I'm using the D205 from Bestech.
```

---
## \#3 Posted by: Namasaki Posted at: 2016-08-09T04:00:45.500Z Reads: 121

```
You can bypass the bms for discharging if it has a separate port for charge - like the Bestech's 
Not sure if you can do it with the Supower bms since it uses the same port for charge/discharge.
The downside is that you will have no individual cell protection while discharging as you do with the bms.
The Vesc or Esc low voltage protection doesn't monitor individual cells while the bms does.
If you have the newer space cell, it has a 50a continuous bms which should be adequate for 10s
```

---
## \#4 Posted by: treenutter Posted at: 2016-08-09T04:10:09.288Z Reads: 120

```
[quote="Namasaki, post:3, topic:7342"]
The downside is that you will have no individual cell protection while discharging as you do with the bms
[/quote]


@Namasaki I've never quite understood this; isn't the protection for each parallel group (as opposed to the individual cell)? I thought it was only in "1P" configurations where each individual cell is balanced on its own.
```

---
## \#5 Posted by: evoheyax Posted at: 2016-08-09T04:17:53.126Z Reads: 112

```
I modified my space cell way back to run 50 amps around the bms. 50 is enough for flat parts, but I do max out at 50 on hills. Adding another p to get to 4p means I can run 80 con from the pack, which Is what I want. 20 per motor x 4 and I should be set :slight_smile:
```

---
## \#6 Posted by: Namasaki Posted at: 2016-08-09T04:39:25.495Z Reads: 97

```
Your right, I was not thinking 100% that time
of course, each parallel group counts as one cell
Still better than just monitoring the total pack as one which is what the Vesc/Esc does.
Good example. when I did my max distance test. I had logged 27 miles and my total pack was between 20-25% but the BMS started shutting it down. Probably one group had dropped lower than the rest. So the BMS saved me from having to pull my pack out, find and replace the damaged cells.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-08-09T04:41:10.365Z Reads: 94

```
Your best option would be to upgrade the bms. Bestech makes a really nice 10s 80a cont bms
it's rather large though.
```

---
## \#8 Posted by: evoheyax Posted at: 2016-08-09T04:54:53.553Z Reads: 86

```
I might but I need to find one smaller than 100mm by 84mm by 24mm. If I don't I'll just leave this bms. If I loose a whole p of cells, Its really easy for me to get more. Amazon sells them in 4's with free one day shipping for $20 USD. So if I lose a p, I'll just replace the 4 cells for $20 and be on my way.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-08-09T04:56:45.110Z Reads: 80

```
Ya, it is kinda big and I'll have to admit that it was not easy fitting it on my system.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-08-09T05:00:54.664Z Reads: 73

```
I've been in the middle of a battery crisis for the last few days. I have a bunch of batteries, but none really fit this board quite right. I decided today to go with my space cell and ripping it apart and adding another p. I like the stability and safety of the 18650s, and after buying 4 motors and 4 vesc, I'm running out of $$$, so it's a win win, in the sense I get my 80 amps, which I was I wanted, and I can reuse the great electronics in the space cell (small charging port and charger, nice battery meter). It's been hard to find small laptop chargers with the port included.
```

---
