# Easy exchangable Battery packs for travelling

### Replies: 25 Views: 1070

## \#1 Posted by: ron Posted at: 2018-03-29T10:14:05.989Z Reads: 198

```
Hey there!

I am going to build two e-boards and one of them on a 22" Deck with 10S3P Samsung 30Q Battery Cells. This one is going to be my travel Board. Because of the restrictions on batteries in planes I wanted to make the Battery into 3 packs of 10s configuration which can be slided into the overall encasing. So it is basically a swappable battery.

So for the electric connection I thought about using XT90 for Power and a DB15 Pin connector for the Balancing leads. It will be a tight fit under the board but I think it is doable.

I did a "mockup" in Fusion360 so you can imagine what I am intending. Sure it needs worked on further for the enclosure.

I just need Ideas how to acomplish this in the best possible way with your help. :)

So for now it looks like this (I know I still ned to model the mechanics of the Batery Packs and the "main" Enclosure where the Battery packs will be slid in. I'm not as good in 3D CAD as I would want to but I'm learning.

![pack_side|690x324](upload://i4PLKGplVlaGcjgpZhtUeepf699.jpg)![board1|690x457](upload://qtUjxPQspo0nCf5jOf6FDKTbv2e.jpg)![board3|690x254](upload://2YUlyHY4XIwxKBZRdFcmMfLYqdA.jpg)![board2|690x325](upload://ceZ64DwNwsUph8xeRU3G4ut8gTY.jpg)
```

---
## \#3 Posted by: Vanarian Posted at: 2018-03-29T10:30:26.530Z Reads: 182

```
Just create a rail with spring clamps and voilà!

You've already done a good part of the job. Better make a nice looking printed case too.
```

---
## \#4 Posted by: Namasaki Posted at: 2018-03-29T21:45:52.643Z Reads: 158

```
Very cool idea, please keep us updated.
```

---
## \#5 Posted by: BoostedBuilder Posted at: 2018-03-29T21:55:08.747Z Reads: 160

```
If you want it to be a travel board, shouldn't it hence be a portable one too? 30 cells will weight quite a bit and really, on a 22" deck you don't need all the power!
I designed the enclosure below and it's being CNC'd out of ABS as we speak so I can test it. You could have something similar done and use only 2 for a 10s2p. You'll still have a good enough range, they won't weight like crazy and you'll have 12mm more clearance under the board! Just wanted to throw this out there.

![44 PM|345x225](upload://dVXyR9mDLtWIbbIrnUoWhZ0AJiu.jpg)
```

---
## \#6 Posted by: pat.speed Posted at: 2018-03-29T21:57:34.910Z Reads: 148

```
He could technically run however many p packs as he wants as he has swapppable series packs. For example he could just unplug one pack then he’ll have 10s2p and then adjust the amp settings by a phone app
```

---
## \#7 Posted by: BoostedBuilder Posted at: 2018-03-29T22:00:37.422Z Reads: 141

```
Of course he could, the modularity in his design is perfect. It's just that he had 3 batteries on his board so I assumed that's what he wanted to use, and the batteries are double stacked on what seems to be 83mm wheels, so I'd be sort of worried about clearance.
```

---
## \#8 Posted by: LukePL Posted at: 2018-03-29T22:01:21.904Z Reads: 140

```
Wow you really found someone that is able to do it? :) Please send me a pic when it's ready! Congrats ;)
```

---
## \#9 Posted by: BoostedBuilder Posted at: 2018-03-29T22:02:15.549Z Reads: 134

```
Yeah haha, Chinese seem to grab onto anything I ask them to do!
```

---
## \#10 Posted by: mikenyc Posted at: 2018-03-29T23:25:36.559Z Reads: 120

```
interesting. are the cells going to be spot welded or is there going to be a bar inside the pack to make the series connections?
```

---
## \#11 Posted by: BoostedBuilder Posted at: 2018-03-29T23:33:25.839Z Reads: 119

```
So plan is for a 10s1p, 8 of the cells will be placed in parallel and spot welded with a nickel strip and then I'll have a wire running for the other 2 cells to continue the series connection.
```

---
## \#12 Posted by: mikenyc Posted at: 2018-03-29T23:35:51.970Z Reads: 120

```
can't a nickel strip be built into the container? or will that not be a reliable enough connection. I guess the goal would be to not have to spot weld anything at all.
```

---
## \#13 Posted by: BoostedBuilder Posted at: 2018-03-29T23:38:27.981Z Reads: 113

```
hmm, didn't think about that. Just having a strip built into the enclosure will most likely not be very reliable, in fact it won't be reliable at all, but definitely an interesting idea! Need to think of something!
```

---
## \#14 Posted by: mikenyc Posted at: 2018-03-29T23:39:33.858Z Reads: 109

```
there could be something behind the nickel strip that can press the nickel strip into the battery. there must be a way
```

---
## \#15 Posted by: BoostedBuilder Posted at: 2018-03-29T23:40:09.072Z Reads: 112

```
There is always a way!
```

---
## \#16 Posted by: mikenyc Posted at: 2018-03-29T23:41:09.652Z Reads: 110

```
maybe a copper bus bar that runs along the bottom, and something like a copper standoff, or nickel standoff that gets pressed onto the top and bottom of each cell

check this thread out

https://endless-sphere.com/forums/viewtopic.php?t=60517
```

---
## \#17 Posted by: BoostedBuilder Posted at: 2018-03-29T23:44:22.168Z Reads: 109

```
I could send you the file so you play around with it too : )
```

---
## \#18 Posted by: mikenyc Posted at: 2018-03-29T23:45:51.708Z Reads: 109

```
sure, I'll PM you my email now. I'll be able to play around with this next week.
```

---
## \#19 Posted by: uigiroux Posted at: 2018-03-30T16:21:26.818Z Reads: 96

```
From what I've heard, you can't have a battery that is over 99Wh right?  But can you have multiple packs like that and then just connect them once your at your destination?  Or is that limit like in total, regardless of how it's set up?
```

---
## \#20 Posted by: BoostedBuilder Posted at: 2018-03-30T16:41:28.684Z Reads: 90

```
You can, that's the whole point!

I just travelled across Europe with 100 individual VTC6 cells - no questions asked!
```

---
## \#21 Posted by: uigiroux Posted at: 2018-03-30T16:43:43.827Z Reads: 88

```
If they were assembled then no way though, lol. I would bring like 4 or 5 separate 12s1p packs to connect at my destination.
```

---
## \#22 Posted by: ron Posted at: 2018-03-30T16:44:42.558Z Reads: 88

```
You can have as many <=100Wh packs as you want. From 100 to 160Wh you can carry 2 packs with you.. 10 of the 30Q will have slightly more than 100Wh but you can label them accordingly on the pack with 99Wh .

That is the whole point in making the battery in smaller packs. Will work on the 3D Cad over the weekend. The DB 15 connectors are ordered. I just don't know how to make the packs fixed to the whole Enclosure on the Board so it doesn't rattle or fall out of the main enclosure. 

Maybe Something like these clamps:
![_AA320_|320x320](upload://pORugpe78VuTiy8SzOT7cboJMh.jpg)

Or something easier to handle with. 

But I am lacking ideas.
```

---
## \#23 Posted by: BoostedBuilder Posted at: 2018-03-30T18:18:20.147Z Reads: 84

```
What @ron said is on point : )
```

---
## \#24 Posted by: 3dman Posted at: 2018-04-02T08:51:03.587Z Reads: 73

```
Nice looking board. What size are the hangers and the width of board?
```

---
## \#25 Posted by: ron Posted at: 2018-04-02T20:03:12.401Z Reads: 60

```
Its a Cruiser Board from Jucker Hawaii:

https://www.juckerhawaii.com/JUCKER-HAWAII-mini-cruiser-WOODY-BOARD-KAPUA
https://www.juckerhawaii.com/media/image/product/346/md/jucker-hawaii-mini-cruiser-woody-board-kapua~4.jpg

Width is 15cm and the Hangers idk. Need to measure it...
```

---
## \#26 Posted by: mmaner Posted at: 2018-04-03T17:30:02.757Z Reads: 50

```
I've got a Jucker Hawaii Woody Kick board that I am crazy about, they make good decks.
```

---
