# HXT Connector Burning up

### Replies: 11 Views: 1001

## \#1 Posted by: melchiorvester Posted at: 2017-07-20T17:10:43.153Z Reads: 75

```
I have 2, 3s 5000mah batteries in series making it one big 6s 5000mah pack. This also has a series balance connector so I can charge it as 6s on my balance charger.

I used a series connector to put them together but when I connected the 2nd battery the HXT connector just burned up and I had to quickly pull it apart. Could it be the fact that I have the balance connector together before putting the two big leads together or something else?

Before I haven't had an issue with this before but I just recently got the 6s balance lead and I think it could be that the 6s balance lead was connected beforehand that caused this, not sure why. Both batteries were fully charged also.

I have XT90 anti spark connectors coming in today so I will be replacing the connectors anyways since I get a big spark and now the connector is burned and unusable.
```

---
## \#2 Posted by: mmaner Posted at: 2017-07-20T20:39:25.369Z Reads: 56

```
read this, good stuff...

http://www.electric-skateboard.builders/t/lipo-spark-when-plugging-into-balance-board/243/15?u=mmaner
```

---
## \#3 Posted by: melchiorvester Posted at: 2017-07-20T21:00:23.311Z Reads: 52

```
Right I did read that but the issue happened with the HXT connector and not the balance leads. Pictures attached. <img src="/uploads/db1493/original/3X/2/a/2ad2d8099afec1f2a8993f6f8fd1d4e4e4e82e83.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/1/d/1d8eb6511547ae5af2b3e9d2c325741a59c162e3.jpg" width="374" height="500">
```

---
## \#4 Posted by: lowGuido Posted at: 2017-07-20T22:13:42.254Z Reads: 43

```
make sure your polarity is correct.
red with red, black with black.
if you are unsure put a little fuse inline that way it would blow before you set yourself on fire.
```

---
## \#5 Posted by: melchiorvester Posted at: 2017-07-20T22:26:41.226Z Reads: 40

```
I'm putting these in series not parallel
```

---
## \#6 Posted by: TowerCrisis Posted at: 2017-07-20T22:33:00.107Z Reads: 38

```
Here's what I'm guessing.

I'll name them, battery 1, and battery 2. battery one comes first, feeds into battery 2, and battery two hooks up to the positive output overall.

Is it possible that battery one had the balance leads plugged into battery two's port, and battery two was plugged into one? This would be a problem.

If you can, try plugging the batteries back together, but don't plug in the balance leads yet. Double check the wire diagrams for the balance board, and double check.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-07-20T22:36:56.157Z Reads: 36

```
[quote="melchiorvester, post:5, topic:28127, full:true"]
I'm putting these in series not parallel
[/quote]

I can see that.
perhaps what I said was easy to misunderstand. red balance lead with read discharge and so on...
remember that your connection between the 2 batteries is now just a cell connection so your negative becomes the most negative battery and positive becomes the most positive.
cut the red wire off the most negative pack balance lead.
you are melting your connector because you have created a short.
```

---
## \#8 Posted by: TowerCrisis Posted at: 2017-07-20T22:48:39.527Z Reads: 34

```
If he plugged it in as depicted in the second picture, it was right.

Regardless, I would agree with putting a fuse inline.

At first glance, looking at those connectors, it seems like you can't plug it in wrong. The positive (live) lead always has the larger sheath that wraps around the other connector.

@melchiorvester Could we get a full picture of the entire connector you're using to connect the batteries together? Did you attempt to connect it exactly as depicted in your second picture?
```

---
## \#9 Posted by: melchiorvester Posted at: 2017-07-20T22:54:14.628Z Reads: 31

```
Sorry I already started to solder on my XT90 connectors but the end of the connector just does to a anther HXT connector. @TowerCrisis Could be very right about me plugging in the balance connector wrong making a short and making my connector burn up. I will make sure I plug the balance lead of battery 1 in the first red port and so on

Edit: here is the picture actually since I finished besides the anti spark connector
<img src="/uploads/db1493/original/3X/2/4/242dafa611684f2599aba24b2a970690982a3a2a.jpg" width="374" height="500">
```

---
## \#10 Posted by: melchiorvester Posted at: 2017-07-20T23:12:24.025Z Reads: 26

```
Well I connected everything together making sure battery 1 with the positive lead has the first spot on the balance lead and everything is good now. Good lesson learned after that.
```

---
## \#11 Posted by: TowerCrisis Posted at: 2017-07-20T23:31:27.537Z Reads: 25

```
Congrats on getting it solved! Looks like we found the culprit :slight_smile: Good luck on the rest of your build.
```

---
