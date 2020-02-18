# Dual battery setup ? Two 12s2p to work as 12s4p ? Will it work?

### Replies: 10 Views: 1997

## \#1 Posted by: NAF Posted at: 2016-07-19T06:47:33.076Z Reads: 199

```
Guys, has anyone here tried running two separate battery packs at once ?

The thing is I am going to have two different decks. One smaller 29" Spud style deck and the other one 37" deck.
I would love to use both decks as often as possible on different occasions. 

So I thought about having **two 12s2p LG Hg2 packs**. I could use both packs as swappable ones on the mini 29" deck, but **my question is if I'll be able to use 2 x 12s2p at once as a 12s4p setup in the bigger deck ??** 

Each 12s2p pack will have this BMS : http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#2 Posted by: NAF Posted at: 2016-07-19T07:18:08.381Z Reads: 191

```
I'll be using dual hub motor setup so will I have to connect each 12s2p battery to each single vesc ? Or could I connect both batteries and have them work together as 12s4p ? 

@Namasaki @longhairedboy @barajabali @lowGuido  - any battery experts that could help me explain how this could work ?


Or the whole thing doesn't make any sense at all ??
```

---
## \#3 Posted by: lowGuido Posted at: 2016-07-19T07:36:29.734Z Reads: 183

```
you can connect the batteries together and then wire the VESC's in parallel. ..
or you could run one pack per VESC... it will work both ways
im not sure that there is an advantage to doing it either way.

id be inclined to use them as one big pack. just because its simpler
```

---
## \#4 Posted by: Maxid Posted at: 2016-07-19T09:21:30.804Z Reads: 166

```
2P might be a little risky with "only" 40A discharge rate.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-07-19T10:45:05.866Z Reads: 155

```
One pack 12s4p with bms and parallel Vesc's would be best. 
Be careful with Vesc and 12s. 
If motor KV is too high, you'll fry the Vesc.
```

---
## \#6 Posted by: Namasaki Posted at: 2016-07-19T10:46:58.041Z Reads: 149

```
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#7 Posted by: longhairedboy Posted at: 2016-07-19T16:40:27.418Z Reads: 124

```
yeah from what i understand 190s are as high as you should go really, and they get warm.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-07-19T17:32:04.746Z Reads: 117

```
I'll be running around 190-197kv on 10s
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-07-19T17:33:59.495Z Reads: 117

```
oh that's perfect. I run 190s at 12S and they only get a llittle warm. My personal 10S build on 190s stays cool the whole time, and that's what the raptors are all doing anyway.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-07-19T21:27:48.479Z Reads: 102

```
[quote="NAF, post:2, topic:6318"]
I'll be using dual hub motor setup
[/quote]

Ok, so hub motors are normally low KV so you should be ok with 12s
```

---
