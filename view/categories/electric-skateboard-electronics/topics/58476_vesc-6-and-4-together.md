# Vesc 6 and 4 together?

### Replies: 14 Views: 535

## \#1 Posted by: DAddYE Posted at: 2018-06-11T01:42:04.585Z Reads: 203

```
Hello fellow builders!

I’m going to test out a flipsky 6. It was on sale for 153$ on rcmoments. 

Do you think I can use it as master and use the torque vesc (4.10) as slave?
```

---
## \#2 Posted by: banjaxxed Posted at: 2018-06-11T20:09:43.735Z Reads: 166

```
That is an interesting question subbing this
```

---
## \#3 Posted by: SuperBen Posted at: 2018-06-11T20:11:57.331Z Reads: 164

```
That is a good question. I would assume you'd have to run dual receivers with both set as masters but I'd be interested to know if they could communicate correctly via can
```

---
## \#4 Posted by: mmaner Posted at: 2018-06-11T20:27:10.284Z Reads: 156

```
I'm just guessing but I think you will get a lot of torque steer with can bus as they handle amperage much differently.  You would likely have to run split PPM and tune them.
```

---
## \#5 Posted by: DAddYE Posted at: 2018-06-11T21:15:17.171Z Reads: 141

```
I guess I’m gonna try myself **when** I get it :rofl:
```

---
## \#6 Posted by: mmaner Posted at: 2018-06-11T21:15:53.796Z Reads: 138

```
Post your results, sems a lot of people are interested.  Good luck.
```

---
## \#7 Posted by: DAddYE Posted at: 2018-06-11T21:16:27.912Z Reads: 133

```
I’ll definitely will! Thanks guys
```

---
## \#8 Posted by: b264 Posted at: 2018-06-11T22:16:20.645Z Reads: 122

```
I would definitely use 2 separate receivers like @SuperBen said.  Which remote are you using?  I know the mini remote and the G2TB can both be run with dual receivers

But if you tried for science I'm sure a lot of us would want to know -- but for safety reasons I don't know if I would trust that.  Those two versions of the firmware may not be intended to work together and I would suspect it's a high probability that if it does work it might be buggy.  Eating street because of software bug would suck.
```

---
## \#9 Posted by: DAddYE Posted at: 2018-06-11T23:37:04.187Z Reads: 111

```
I think I’ll try the can bud for science :)
```

---
## \#10 Posted by: Blitz Posted at: 2018-08-06T16:52:08.171Z Reads: 85

```
Any Updates?
```

---
## \#11 Posted by: fliess Posted at: 2018-08-06T18:14:14.214Z Reads: 80

```
I would definitely agree with @b264 about 2 separate receivers. I am also doing so with mini remote and it's just proven to be super reliable.
```

---
## \#12 Posted by: Deodand Posted at: 2018-08-06T22:15:56.876Z Reads: 71

```
As long as you flash the 4.10 with latest FW from vedder the CAN bus will be fully compatible no problems there. All that is sent across is a current command.

EDIT: suppose its possible but unlikely the transceivers might not play nicely together.
```

---
## \#13 Posted by: Blasto Posted at: 2018-08-07T16:00:54.901Z Reads: 57

```
[quote="Deodand, post:12, topic:58476"]
transceivers might not play nicely together.
[/quote]

Tested, they play nicely
```

---
## \#14 Posted by: Deckoz Posted at: 2018-08-08T14:30:53.226Z Reads: 40

```
I've run 4.12 and focbox together over CAN, and focbox with an DIY Escape on same firmware version (ack 3.100) just fine.
```

---
