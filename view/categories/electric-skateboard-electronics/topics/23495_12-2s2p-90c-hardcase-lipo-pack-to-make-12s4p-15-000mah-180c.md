# 12 2S2P 90C Hardcase Lipo Pack to make 12s4p 15,000mah 180C

### Replies: 19 Views: 1851

## \#1 Posted by: Brad Posted at: 2017-05-19T19:58:58.785Z Reads: 242

```
I just need to make sure I got this right before doing anything at all. Almost ready to start a build thread, just need to wait for Torqueboard's 218mm Calibers and the two VESC to arrive.

This is what I think needs to be done to make 12s4p. 
<img src="/uploads/db1493/original/3X/7/a/7a22d6026eb1c1491993b303f943cd48345f9b67.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/7/0/703634c046d83741a3ec9732a6e9d6563649bd2d.jpg" width="565" height="414">

The part that I need checked is for Balancing Board/Equilibrium Module via the banana plugs because each lipo pack contains two series and I will need to connect two of it to form 4 parallel.

Wouldn't just connecting the two blue balance leads from the parallels together to form a single blue balance lead and then just leading it to the correct balancing pin work fine? Obviously need a ground from the first pack. All other grounds not needed.

<img src="/uploads/db1493/original/3X/d/3/d3e93951f5b6c26d47bbae4159ab72a11936958a.jpg" width="690" height="388">

The balance leads is below.
<img src="/uploads/db1493/original/3X/7/f/7f26b94645f916dd572379c53afd6ae894da2739.jpg" width="565" height="414">

I just realized that I could fit 12 2s2p onto my board allowing me to keep the same 15,000mah as 60 30Q cells in 12s5p configuration, but with 180C therefore greatly reducing voltage sag.

Dimensions would be L 41.55cm x W 18.6cm x H 2.5cm
```

---
## \#2 Posted by: Namasaki Posted at: 2017-05-19T20:06:22.136Z Reads: 211

```
This is gonna be soooo good!
Looks like we need to re-think your wiring though
and your gonna need a good bms.
```

---
## \#3 Posted by: Brad Posted at: 2017-05-19T20:11:08.754Z Reads: 209

```
[Balancing/Equilibrium Board for 3S~16S Li-ion/Li-Polymer/LiFePO battery packs](http://bestechpower.com/balanceboard/D172.html)

I will be using [Cycle Satiator 48V 8A](http://www.ebikes.ca/shop/electric-bicycle-parts/chargers/cycle-satiator.html) of which I have already ordered and is also waiting for it.

The reason why I'm not going to use BMS is to save space and will be using Ollinboard's fuse/antispark.

Another reason is I wish to stop charging at 4.1 volt for longer battery life and to allow headroom for voltage surge/overcharge from regenerative brakes if I start atop of a hill one day when the board is hot off the charger.

I will cap Amax at 80amps though and redo the wires with 8AWG [Red](https://hobbyking.com/en_us/turnigy-pure-silicone-wire-8awg-1m-red.html) and [Black](https://hobbyking.com/en_us/turnigy-pure-silicone-wire-8awg-1m-black.html).

What do you mean re-think my wiring, where is it wrong unless you mean too thin wires?
```

---
## \#4 Posted by: Namasaki Posted at: 2017-05-19T20:15:41.522Z Reads: 185

```
I mean the series connections look wrong. I'm still going over it but it appears you have too many cells in series for 12s
```

---
## \#5 Posted by: Brad Posted at: 2017-05-19T20:17:33.438Z Reads: 179

```
2 series and 2 parallel in each box, the other box beside it is connected to make 4 parallel so there is really only 2 series for two boxes.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-19T20:22:54.651Z Reads: 181

```
You could save a lot of money by using the Bestech 12s bms with built in E-switch and you could use a lab power supply to charge to what ever voltage you desire.
I have gone down steep hills with a full 10s battery and the bms keeps regen from over charging the battery and I have had no problem with any thing shutting off.
A stand alone E-switch takes up some room and requires additional high amp connections.

the board your looking at is 122*93*7 mm
The 12s bms isL120mm*W80mm*T25mm so about the same foot print but with built in switch.
The bms will also protect your investment against external shorts and over discharge.
http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#7 Posted by: Brad Posted at: 2017-05-19T20:24:22.140Z Reads: 171

```
I think I see the mistake I made.

You appear to be correct, I have made 24 series instead of 12.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-05-19T20:27:17.098Z Reads: 164

```
It might be easier if you put them in 6 groups of 2 packs in parallel and then put the 6 groups in series.

Are you looking for extreme range?

Because those batteries would rock the house even with only 6 packs in series.
```

---
## \#9 Posted by: Brad Posted at: 2017-05-19T20:49:16.961Z Reads: 168

```
I think I got it now.

First do two 6s4p separately and config it as below.
<img src="/uploads/db1493/original/3X/9/c/9c46a2280164a601f558b6f119b69dd0dbc0bcb9.jpg" width="690" height="388">

After that is done, then join them both up as below
<img src="/uploads/db1493/original/3X/5/c/5c2e28b3e04c4e7cb45748d8c4b96148281ee933.jpg" width="690" height="388">

I do not think the range is extreme, only 52kms. Here is my calculation. (I set watts per km at 11 as that would be average normal use, screw ECO mode)
<img src="/uploads/db1493/original/3X/e/c/ec09862bd130be5fe5cc6ef99506fd5ebc219d4b.png" width="690" height="440">

I see that the watts for each motor may be a bit high which is why I might have to lower Amax to 60amps.

I know Evolve GT has two motors combined for 3,000 watts but I do not believe that the garbage battery pack they use is capable of feeding that much, probably peaks at 1,800 watts combined.
```

---
## \#10 Posted by: Namasaki Posted at: 2017-05-19T21:03:12.155Z Reads: 144

```
52 km / 32 miles, not extreme?
32 miles is very extreme for an eboard.
```

---
## \#11 Posted by: Brad Posted at: 2017-05-19T21:05:43.584Z Reads: 148

```
Perhaps.

I get very annoyed with Evolve that I own, cos 15 Kms is just way too short.

Another thing is I do not have a car and use the board very heavily. Do not want to wait around to recharge that pissant 15km Evolve half of the day.....

Just think of the board as a charge and forget for the day sort of thing.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-05-19T21:08:18.538Z Reads: 144

```
The balance wires are incorrect now. you've taken the pack that are in series and put their balance wires in parallel.
Plus it will be easier to do this system with a bms that will monitor each cell group individually if you make 6 groups of 2 packs in parallel and them put the 6 groups in series.
```

---
## \#13 Posted by: Brad Posted at: 2017-05-19T21:38:07.937Z Reads: 149

```
Well, maybe I got it this time. It is amazing how much easier it is to get config right with 18650 cells and no cables.
<img src="/uploads/db1493/original/3X/f/7/f794dfb8a11b5512ceafdb7bd30f1872060b1d53.png" width="690" height="388">
```

---
## \#14 Posted by: Namasaki Posted at: 2017-05-19T22:09:10.825Z Reads: 138

```
think you got the main cables now.
Ready to figure out the balance wires.
```

---
## \#15 Posted by: Brad Posted at: 2017-05-20T06:21:21.980Z Reads: 135

```
Thank you very much for your input, I appreciate it.

Now that I have had my beauty sleep and can think it through more thoroughly, here is the new updated diagram.
<img src="/uploads/db1493/original/3X/d/4/d413d96713d43596878e0fb0f6aa0ba6973997e8.png" width="690" height="388">

This is looking so much neater.

Not going to buy the batteries as of yet, still need to wait for the two VESC so I can lay it on my board and eyeball the remaining space instead of just trying to imagine it all.

I'm a bit apprenshive about this [BMS.](http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html) A bit odd that I would need to leave the board on to charge it up? Also, I read this [thread](https://www.electric-skateboard.builders/t/e-switch-on-bms/13484/56).

With the e-bike charger, at least I will not have to buy another charger for different configs in the future as I can adjust it from 24v to 52v and charge from 1amps to 8amps, so still ok with the somewhat expensive purchase.

I forgot to mention another advantage of longer mileage which is fewer cycles in the same amount of time, meaning the pack will last longer before hitting 80% capacity.

Edit: Improved wire plan
```

---
## \#16 Posted by: Thatdudedominic Posted at: 2018-03-08T15:07:08.513Z Reads: 78

```
What does the green wire represent
```

---
## \#17 Posted by: Brad Posted at: 2018-03-31T21:35:07.052Z Reads: 71

```
Sorry, been away for a while.

Green is balance leads. It is no longer my plan.
```

---
## \#18 Posted by: Orin635 Posted at: 2018-03-31T21:42:32.387Z Reads: 69

```
how big is the enclouers to fit all them LiPos?
```

---
## \#19 Posted by: Brad Posted at: 2018-04-01T06:10:23.761Z Reads: 50

```
Battery enclosure length would not be much of a problem, but the width is impossible. 

I have gone Li-Ion 12s5p. Two 5p in parallel side by side is 18.5cm which can fit and have both terminals on the same side instead of one near the BMS and the other at the other end of the pack.
```

---
