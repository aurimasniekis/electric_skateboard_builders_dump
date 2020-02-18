# 2 Side Enclosures - Do I really need to upgrade my VESC capacitors?

### Replies: 9 Views: 741

## \#1 Posted by: ACIN Posted at: 2017-03-17T00:11:23.263Z Reads: 176

```
Hello community,
with my upcoming build I'm going for the two-sided, boosted board like look: Batteries on one side VESC's on the other.
It is a fairly long board and the distance between both enclosures will be about 70 cm.
I have heard that I need to upgrade my capacitors if the cable gets too long, but I also have seen that my two Maytech VESC's are equipped with some pretty solid capacitors already: 3 times 680µF for each VESC.

Do I really need to buy more capacitors, if yes does anyone have a good source?
Does it make any difference that I use an AntiSpark or BMS? Or where I place them, on battery or VESC/Motor side?

My Setup:

- Dual Carvon V2.5
- Dual Maytech VESC
- 3 x 4S Zippy Compact 25C LiPo 5800 mAh
- Steeze Remote
- Alienpowersystem Antispark
- Some BMS not sure yet
- 12S Laptop Brick
- LED Strips, SBEC 12S to 12V (for LED) & 5V (For USB Port), Remote on/off
```

---
## \#2 Posted by: benwong Posted at: 2017-03-17T00:28:52.476Z Reads: 162

```
That is fine for me as i have two side of enclosure. 
I dinnt add any or modify my capasitor. I try to avoid power lack issue, so i shorten the middle connection wire around 35 to 40cm. Boosted board connection wire is almost end to end of the board.
```

---
## \#3 Posted by: ACIN Posted at: 2017-03-17T00:39:49.368Z Reads: 151

```
Ok, yeah I have heard it is fine for that sort of distance. But I really have a long board and my board is nicely flexible (and I want to keep it that way) in the middle which is why my distance will really be more like the one of the boosted board.

If I'm not mistaken the Voltage of the Capacitors I might buy has to be the same as the one already on the VESC but the capacity doesn't have to, right?
Anyway I found [these](http://www.ebay.com/itm/10x-Elko-Kondensator-radial-680-F-63V-105-C-UPR1J681MHH-680uF-/310969407189?hash=item48673896d5:g:LNAAAOSw8RJXCNY6) ebay, they look good to me. Does anyone have some advice?
```

---
## \#4 Posted by: benwong Posted at: 2017-03-17T01:54:23.188Z Reads: 135

```
seem like you have a loooonnnngboard. :grin:
Also depend what kind of wire you use as the connection between. 
need some expert to advise. i poor on electric thing.
```

---
## \#5 Posted by: willpark16 Posted at: 2017-03-17T02:57:45.842Z Reads: 119

```
The better insulation there is the less resistance and energy lost amongst wire
```

---
## \#6 Posted by: Nordle Posted at: 2017-03-17T15:17:16.128Z Reads: 98

```
Better insulation only means wires can be closer together (this means less inductance, and thats what we want). Twisting wires also can help. 
If you buy capacitors look for genuine ones with low ESR(electric series resistance) rating, lower is better here. And finally, dont buy cheap caps or transistors on aliexpress or alibaba, they might work for some applications but for me those parts failed most time.
```

---
## \#7 Posted by: ACIN Posted at: 2017-03-17T15:25:18.866Z Reads: 93

```
Thanks, I am probably going to end up using normal 10 AWG cable. Since I am planning to embed it in the board (directly under the griptape), do you think it would be a better idea to keep the cables further (like 8 cm) apart or twist them and embed them in one big notch?
Also does it matter where I put the antisparkswitch, bms or voltmeter?
```

---
## \#8 Posted by: bullrider12 Posted at: 2017-03-17T15:42:23.687Z Reads: 83

```
You can use flat tinned copper braid for your setup. Im going to use this for my board too. Somewhere in this forum I read that 6mm wide braids are enough.

Something like this: http://www.ebay.com/itm/10-FEET-1-2-BRAIDED-GROUND-STRAP-GROUNDING-Tinned-Copper-Flat-Braid-MADE-IN-USA-/291855955896
```

---
## \#9 Posted by: Nordle Posted at: 2017-03-17T15:43:21.583Z Reads: 80

```
Wires closer together is better. Lol just read im out here now;)
```

---
