# Making a Battery

### Replies: 15 Views: 1006

## \#1 Posted by: butt_stallion Posted at: 2018-01-24T21:09:55.385Z Reads: 219

```
Alright, here is what i'm thinking.  I just wanted to get some other opinions on it.  I don't have access to a spot welder so I wanted to figure out a way I could build it without having to solder directly to the battery.  I 3-D printed 10 battery sleds so I could make a 10s3p battery.  This is just 3 of the 10 sleds but you get the general idea of what i'm going for.  I am going to cut a piece of wire like in the picture below for the parallel connections and then bridge the positive and negative terminals for my series connections.  What do y'all think of this?

![0124181604|281x500](upload://nSpcZmImn0aCi3Jf6QVBXVtSjJr.jpg)
```

---
## \#2 Posted by: Acido Posted at: 2018-01-24T21:38:52.200Z Reads: 194

```
Im suggesting to fully remove the wire isolation for the positive and do the same for the negative, but my question is why didnt you just connect them with nickel?
```

---
## \#3 Posted by: Skifree Posted at: 2018-01-24T21:40:24.465Z Reads: 190

```
Looks good to me, I just built one of these for my quadcopter, except 4P3S. You could check out this thread for a spot welder, I bought one and it has made battery building so much easier! The guy builds it from an Arduino and you can use LiPo batteries to run it.

http://www.electric-skateboard.builders/t/boss-level-custom-spot-welder


If you don't want to read through the thread, basically send and email to the maker, he doesn't speak much english. Basically "Please sell me a spot welder" he will email the price, and wait for you to paypal the money, and he ships it extremely fast from South Korea.
```

---
## \#4 Posted by: butt_stallion Posted at: 2018-01-25T01:45:36.865Z Reads: 157

```
Well I would but I don't have a spot welder and I don't feel comfortable soldering them because I don't want to damage the batteries.
```

---
## \#5 Posted by: butt_stallion Posted at: 2018-01-25T01:46:47.930Z Reads: 150

```
I read that thread!  I love how small that thing is!  I am planning on getting one but as of right now it's not in the budget.
```

---
## \#6 Posted by: Acido Posted at: 2018-01-25T06:16:57.292Z Reads: 133

```
Ohh i misunderstood,I red that you did haveacces to a spotwelder
```

---
## \#7 Posted by: Skifree Posted at: 2018-01-25T18:38:08.416Z Reads: 109

```
That's fair, I keep reading that people hate to see others solder their batteries, but at the same time, it can't be too terrible if they claim their batteries work well in the end. I think if you move really quickly and keep the solder blobs small, you should be fine. I've seen some videos where the builder holds the iron on for nearly 10 seconds, that can't be too good for it.....
```

---
## \#8 Posted by: deucesdown Posted at: 2018-01-25T18:48:14.854Z Reads: 103

```
It's do-able but there's a few issues.

- the spring contacts on the negative can't carry much current. gets hot, 3d printed part deforms, springs lose their springy property, contact gets looose, intermittent connection

- batteries can get hot when doing big loads, can deform the sled, loosen, intermittent.

- vibrations can break connection momentarily and often, arcing, carbon buildup, increased resistance, heat, see above.

Good luck if you go for it!
```

---
## \#9 Posted by: Acido Posted at: 2018-01-25T19:00:55.122Z Reads: 99

```
im suggesting you get a spot welder its 70e, worth it
```

---
## \#10 Posted by: butt_stallion Posted at: 2018-01-25T19:04:44.354Z Reads: 95

```
I'm going to go for it but this is just a temporary solution.  As soon as I can get a spot welder I will rebuild the battery.  For now I think this will work.
```

---
## \#11 Posted by: sash Posted at: 2018-01-25T19:11:37.281Z Reads: 91

```
I second that Arduino spot welder is a great investment. Small, easy to set up, runs on a car battery, works like a charm. Much easier than soldering.
```

---
## \#12 Posted by: sash Posted at: 2018-01-25T19:18:33.905Z Reads: 87

```
You can damage the cells by soldering, unless you are very good at it and have a 100+ Watt soldering iron.  When I was thinking about building a battery I also looked at these soldering irons and found that they cost more than an Arduino welder.
```

---
## \#13 Posted by: Acido Posted at: 2018-01-25T20:23:21.514Z Reads: 77

```
Also 18650 are treated with some anti solder shit so you will have to sand them a bit
```

---
## \#14 Posted by: GrecoMan Posted at: 2018-01-26T02:22:29.810Z Reads: 70

```
[quote="Acido, post:13, topic:44561"]
sand them a bit
[/quote]

that's quite the understatement lol. was gonna solder about 40 cells together for a shits-n-gigs powerbank. long story short, after sanding the pos and neg of 6 cells I threw my sandpaper across the room, put the cells in a box and gave up. don't solder your cells.
```

---
## \#15 Posted by: butt_stallion Posted at: 2018-01-29T14:24:59.324Z Reads: 52

```
I am definitely going to get a spot welder.  I do not trust this and won't be using it in my board.  I feel like the connections are very sketchy and the plastic has already become weak because of soldering.  Definitely would not try this again.
```

---
