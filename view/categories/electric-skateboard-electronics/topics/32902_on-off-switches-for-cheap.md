# On/Off switches for cheap?

### Replies: 11 Views: 1121

## \#1 Posted by: Orin635 Posted at: 2017-09-11T20:50:49.222Z Reads: 150

```
I thought I was all ready to buy my parts for my e-board but then I remembered, "How am I going to turn this thing on and off without having to open it up and unplug/plug in cables?" I found some switches on hobby king for around 3$ but I doubt they could handle 25.2v (I'm using 2 3s lipo batteries) so does anyone have any idea how you'd go about getting an on/off switch?
```

---
## \#2 Posted by: faithfulpuppy Posted at: 2017-09-11T21:05:50.229Z Reads: 145

```
the only three ways to do on/off are:
1) buy a mosfet switch. a tad expensive but really a drop in the bucket as far as eboards go. However they can and do fail for no reason.  When they do fail, they fail in the "on" position so you don't lost control of the board, it's just kinda annoying
2) BMS switch.  Same thing as 1 but it's built in to your BMS. Some have it, some dont.  Remember this only works if you discharge via the BMS
3) XT-90s loop key.  solder some wires and connectors together and you basically get a little plastic doohickey you plug into your board to turn it on.  I originally didn't like this but after my MOSFET switch broke i tried it and honestly it's grown on me.  It's cool and unique and prevents theft. This is also far and away the most reliable option, while also being (kinda) the cheapest.
```

---
## \#3 Posted by: Orin635 Posted at: 2017-09-11T21:07:53.416Z Reads: 135

```
Could you explain more about the xt90s
```

---
## \#4 Posted by: deucesdown Posted at: 2017-09-11T21:18:45.738Z Reads: 129

```
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

if 6s or below, this should also be somewhat safe

http://www.electric-skateboard.builders/t/what-do-you-think-about-using-dc-breaker-switch/1325/22
```

---
## \#5 Posted by: Orin635 Posted at: 2017-09-11T21:35:02.136Z Reads: 112

```
so your saying get a circuit breaker?
```

---
## \#6 Posted by: faithfulpuppy Posted at: 2017-09-11T22:09:15.278Z Reads: 105

```
nah, in my opinion the circuit breakers are big, clumsy, and ugly.  To each his own.  The xt-90s strikes the right balance of elegance and functionality (imo)
```

---
## \#7 Posted by: sk8ace Posted at: 2017-09-11T22:17:48.322Z Reads: 94

```
I've been using some big 60 amp circuit breakers for over a year with mine. They are big and ugly but I've never had a problem with them and they were less than 10 bucks. I care much less about appearance than most though.
```

---
## \#8 Posted by: Orin635 Posted at: 2017-09-11T22:22:07.547Z Reads: 91

```
I see, where would I connect the xt90s?
```

---
## \#9 Posted by: Orin635 Posted at: 2017-09-11T22:23:10.431Z Reads: 87

```
Alright if the xt90s don't work they'll be my backup
```

---
## \#10 Posted by: faithfulpuppy Posted at: 2017-09-11T23:01:16.871Z Reads: 78

```
read @deucesdown's comment.  Basically, take a section of wire (say, the positive and negative running to your esc) and cut one side (eg the positive wire) in half.  Then take each side of the split and attach them to the 2 points of the same xt90 connector.  Then, bridge the two points on the matching connector.  When you plug the bridged one into the one on your board, your board will turn on.
```

---
## \#11 Posted by: Jebe Posted at: 2017-09-12T01:16:33.795Z Reads: 62

```
Link ? .........
```

---
