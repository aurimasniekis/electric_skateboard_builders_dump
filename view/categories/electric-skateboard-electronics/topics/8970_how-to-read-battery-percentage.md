# How to read battery percentage?

### Replies: 8 Views: 1499

## \#1 Posted by: Brando Posted at: 2016-09-05T13:50:38.944Z Reads: 174

```
I have two e-boards, both with zippy 6S batteies. Both boards have lipo battery indicators that convert the voltage into remaining capacity, but something I noticed is that both indicators don't drain in a linear line. When the battery indicator gets to 50%, the reading starts to drop quicker. By the time it gets to 30%, it is only a matter of a couple minutes before it reaches 0%.
The indicators are different brands completely and they suffer the same issue.
Any thoughts on how to accurately read capacity remaining?
```

---
## \#2 Posted by: mason Posted at: 2016-09-05T15:13:31.741Z Reads: 165

```
Those are accurate. The lower the voltage the faster it drops.
```

---
## \#3 Posted by: Brando Posted at: 2016-09-05T15:35:25.423Z Reads: 158

```
is there any smart battery indicators that counteract this to make a linear drop? Smartphones and other lithium powered devices decrease linearly.
```

---
## \#4 Posted by: mason Posted at: 2016-09-05T15:43:14.111Z Reads: 158

```
Not that I know of.
```

---
## \#5 Posted by: mrjonnyjones Posted at: 2016-09-05T16:11:19.226Z Reads: 146

```
I use [HobbyKing's HK-010 Power Analyzer](http://www.hobbyking.com/hobbyking/store/RC_PRODUCT_SEARCH.asp?strSearch=HK-010) - it measures cell voltage and percentage remaining.  It also balances your cells, so that you can maintain healthy batteries.  I'm not sure if this will help you? :slight_smile:
```

---
## \#6 Posted by: SimosMCmuffin Posted at: 2016-09-05T16:24:45.069Z Reads: 138

```
The phone's battery indicator percentage might decrease linearly, but the battery voltage doesn't, which your battery indicators are showing.

In the below picture is the discharge curve for a LG MJ1 Li-Ion 18650 cell.
http://d112tss1dzpest.cloudfront.net/wp-content/blogs.dir/26/files/2015/02/194412p3dnp2cdldgpzpww.jpg

The voltage is pretty linear in the 100% - 20% after which it will very quickly drop down. A better way to figure out how much battery life you have left based on your indicators is to charge the Li-Pos with a charger that can show how much capacity it has charged back.

[quote="Brando, post:3, topic:8970"]
Smartphones and other lithium powered devices decrease linearly.
[/quote]

[quote="Brando, post:1, topic:8970"]
both with zippy 6S batteies
[/quote]

Zippy batteries are Lithium chemistry.
```

---
## \#7 Posted by: Brando Posted at: 2016-09-05T16:37:41.455Z Reads: 126

```
So its basically a monitor and a bms? That would be awesome.
```

---
## \#8 Posted by: mrjonnyjones Posted at: 2016-09-05T17:05:34.699Z Reads: 120

```
Not simultaneously, you can balance the cells when the battery isn't in use/under load.  It is an epic piece of kit, though :slight_smile:

https://www.youtube.com/watch?v=ARMwAkNf3XE
```

---
