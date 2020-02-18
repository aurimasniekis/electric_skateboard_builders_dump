# Using LifePO4 cells in an esk8

### Replies: 21 Views: 507

## \#1 Posted by: Toughook Posted at: 2018-08-16T20:21:24.354Z Reads: 145

```
I have an old scooter project gathering dust in my warehouse which never really got used enough by my son. It's a Razor300 with a 36v nominal (42v fully charged) lifepo4 battery pack. As you can see from the pictures it's on a rectangular pack, but I'm toying with the idea of breaking it apart, and arranging the cells to fit in a custom esk8 enclosure.

The cells and pack are all in fine condition, and I'm wondering on the pros and cons of doing this. Clearly the major pro is that it's free (in effect) but what are the cons? Would I be wasting my time doing this, and if not, could I use my spare focboxs with it?

Shoot it down as a terrible idea if so, or tell me to have a go if not.... I'm interested in your thoughts 👍👍

![Screenshot_20180816-210826_Gallery|690x335](upload://o4yav55UopRXdwqrb4BpA2upuWt.jpg)![Screenshot_20180816-210852_Gallery|690x335](upload://vBGQjCXDxrX6vyRpkJuLdYdFLUL.jpg)![Screenshot_20180816-210741_Gallery|690x335](upload://8tjYlvWxrCzI3I004n6KKVO0mzA.jpg)![Screenshot_20180816-210806_Gallery|690x335](upload://sTH1oZbJjh6LyUVDmGZmljAApmI.jpg)
```

---
## \#2 Posted by: Blitz Posted at: 2018-08-16T20:25:40.864Z Reads: 132

```
I read a few topics like this a while ago, 
and from the top of my mind,

LEss energy dence less current lower voltage, Q30 much better and lipos Pack better a better punch.

Read the specs If the current and capacity works then it works.
(still better than Lead acid)

I guess there good cells its just there harder to find and can cost more that makes me biased.
```

---
## \#3 Posted by: Toughook Posted at: 2018-08-16T20:30:40.897Z Reads: 129

```
Oh yes, for sure. The only reason I'm even considering it is because it's something I own already and so the cost is zero in hardware..... Just a bit of a project if feasible.
```

---
## \#4 Posted by: b264 Posted at: 2018-08-16T20:31:25.814Z Reads: 128

```
Is it 5Ah?  I have an esk8 with a 5Ah LiFePO4 that looks similar, and it works just fine.

![20180125_150328|690x345](upload://78RemG0tmiDFeWOhlDxVUBNEMTz.jpg)
```

---
## \#5 Posted by: Toughook Posted at: 2018-08-16T20:33:24.217Z Reads: 120

```
I'll have to dig out the specs from the original purchase as don't know off hand. Encouraging that someone's done it already though 👍
```

---
## \#6 Posted by: brenternet Posted at: 2018-08-16T20:34:38.348Z Reads: 117

```
Boosted run lifepo4, they are absurdly safe batteries.
```

---
## \#7 Posted by: b264 Posted at: 2018-08-16T20:35:56.122Z Reads: 117

```
If it's less than 3Ah it may not be enough but if it's 4Ah or more, do it :slight_smile:
```

---
## \#8 Posted by: pat.speed Posted at: 2018-08-16T21:28:38.295Z Reads: 100

```
Honestly there is no reason not to. If it ain’t doing anything and it’s free, why not
```

---
## \#9 Posted by: chuttney1 Posted at: 2018-08-16T22:21:00.588Z Reads: 92

```
The chemistry is just safe.
```

---
## \#10 Posted by: Brdchris Posted at: 2018-08-16T23:15:04.212Z Reads: 89

```
Yup, what these guys said. It will make for a great safe battery. Maybe a little bigger than an 18650 pack but for free, who cares. 

That scooter kinda looks awesome though, I would struggle to cannibalize it for the eboard
```

---
## \#11 Posted by: Lionpuncher Posted at: 2018-08-17T02:43:53.350Z Reads: 79

```
I'm pretty sure they're 50a discharge. Wouldn't that make them excellent for smaller packs?
```

---
## \#12 Posted by: b264 Posted at: 2018-08-17T02:54:56.815Z Reads: 77

```
LiFePO4 are heavy and big for their capacity, but other than that, they are better.  Except heavy and big.  But better in the other ways.
```

---
## \#13 Posted by: Toughook Posted at: 2018-08-17T06:12:39.039Z Reads: 66

```
Haha cheers ! The scooter was fun to build, and for a brushed motor (500w 24v effort) overvolted to 36v (42v charged) it flies ! I did a couple of smaller e200 scooters, 36v (24v) 350w SLA batteried as well at the same time. My then 9year old son loved his e200, and would hit 21mph on the straights. The e300 did 24mph with my 95kg frame on it!!

https://youtu.be/gMUen9uNUGA

His mates thought he was awesome. I built the e300 for me, with an eye that he'd promote to it, but he's lost interest now and into other things. So it's sitting around doing nothing. Seems a shame to just let it rot, and now I'm into esk8 and want to learn to build my own Li ion batteries, ultimately, this seems like a fun half-way-house project to familiarise myself with parts of the process.

I'm gonna do it :) 

Then I'm gonna do a 3rd board with my own DIY Li ion.

Nice to have plans :)
```

---
## \#14 Posted by: sk8l8r Posted at: 2018-08-17T06:28:39.097Z Reads: 60

```
Bajaboard gen 3 also used them
```

---
## \#15 Posted by: Toughook Posted at: 2018-08-17T15:01:56.615Z Reads: 52

```
dug out the old emails from this order and found the specs. Might have something to work with here after all ?

Rated Discharging Amperage: 10 Amps
Max Continuous Discharging Amperage: 20 Amps (50 Amps with High Rate BMS)
Maximum Discharging Current: 60 Amps
Discharging Cut-off Protection: 25-30 Amps (65-70 Amps with High Rate BMS)
Lifecycle of the whole pack: >85% capacity after 1000 cycles. Lifecycle of single cell: >85% capacity after 1500 cycles, >70% capacity after 3000 cycles. (<1C discharge rate and <1C charge rate), Averagely 2000 Cycles

edit: I have the High Rate BMS btw

I bought it from here : http://www.pingbattery.com/

What do you think ? The project board is only supposed to be short commuter and not a long range cruiser like my other PaleRider build. I can custom make an enclosure to suit, and go from there....
```

---
## \#16 Posted by: Toughook Posted at: 2018-08-17T15:42:04.298Z Reads: 50

```
I had to open it up....

Wasn't expecting this. Thought they would stubby cells, but evidently not 😂

![20180817_161857|690x335](upload://lBfBeyAokOdjQ0DihwOJ4O3olee.jpg)![20180817_161912|690x335](upload://c5ef85Fjn5H4hfTHHSh4ohuBIS6.jpg)![20180817_161847|690x335](upload://61JOb5dfRhlMd0ScnyrvQwCsOnu.jpg)

Scrap that then ! 😂😂
```

---
## \#17 Posted by: b264 Posted at: 2018-08-17T18:29:28.448Z Reads: 42

```
That still doesn't mention a capacity in mAh or Ah

It may be printed on the blue shrink wrap, like a box checked 2, 5, 10, 20 or something with a check in one box

Judging by size, that's a 5Ah and will work fine if you can physically fit it.  That would be perfect for a short-wheelbase deck with a tail
```

---
## \#18 Posted by: Toughook Posted at: 2018-08-17T19:11:08.500Z Reads: 38

```
Right, sorry... According to the order email thread I found, it's the 10Ah version. As it happens the deck I have earmarked for this project is a 16" wheelbase Powell kick tail.

I'd still struggle to make these cells look sleek though. It's in 6 sections, and I can't lie them 2x3 format as not enough space, and that's not even taking escs and bms into account. Would need to double stack and that would be over 60mm at that point. Not the look I'm after. Might do it on a long board though next time where I've more space to play with. Shame really.
```

---
## \#19 Posted by: b264 Posted at: 2018-08-17T20:41:29.395Z Reads: 33

```
[quote="Toughook, post:18, topic:65108"]
the deck I have earmarked for this project is a 16" wheelbase Powell kick tail
[/quote]

That's the ***absolute perfect deck*** for this ... if it was the 5Ah pack and not the huge 10Ah pack.  If you used axial-direct-drive like Carvon or TB and flattened that pack, it'd work though
```

---
## \#20 Posted by: Hummie Posted at: 2018-08-17T20:51:00.640Z Reads: 30

```
U probably separate the pouches from each other similarly to as done w lipos.  If no one said that yet. Bet u could make it slim.  If u do scrap them as u worded it what would that mean. Surely good for something.
```

---
## \#21 Posted by: Toughook Posted at: 2018-08-17T21:25:13.968Z Reads: 28

```
When I say "Scrap that" it just means bad idea (a northern UK saying) - I'm not actually going to throw the battery away :) 

That said in the 2x3 arrangement it would only be 30mm thick and stealthy, so best for a longboard I think. 

As this board is really supposed to be a cheap project, mainly to introduce my son to esk8 I can't justify the Carvon DD or similar. Maybe dual hubs (hides away in the corner with flame suit on) would work though ! 

The Powell deck is a beauty though !

![20180817_140437|243x500](upload://bPVxbAPUL5fJaYeFqMhUbqx7jaK.jpg)![20180817_140454|243x500](upload://veY1CbEFSsI1e8tGmKmJ3KTRx6U.jpg)![20180817_140516|243x500](upload://n6AsPLSPwK6tlqKw1aJEONHb6sS.jpg)
```

---
