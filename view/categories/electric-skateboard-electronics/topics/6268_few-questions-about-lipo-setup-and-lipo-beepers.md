# Few questions about Lipo setup and Lipo beepers

### Replies: 7 Views: 1015

## \#1 Posted by: kampfhahn Posted at: 2016-07-18T11:16:24.521Z Reads: 122

```
I´m building a 10S Setup at the moment with 2x 5S Turnigy Lipos. To avoid deep discharge i ordered [two of these](https://www.amazon.de/fitTek-Spannung-Checker-Schutz-Anzeiger/dp/B009LW48LK/ref=sr_1_1?ie=UTF8&qid=1468840240&sr=8-1&keywords=lipo+warner) lipo warners, one for each battery.

Now i´m asking myself if i also could use just 1 beeper for both (serial wired) batterys using my [parallel balancer adapter](http://www.ebay.com/itm/JST-XH-2x-6S-Buchse-auf-6S-Stecker-Lipo-Balancer-Parallel-Silikonkabel-JST-XH-/161919857024) which i use to charge my batterys parallel? This would make the charging process a bit quicker because i could let the parallel adaptor plugged at the balancer plugs of the batterys all the time. Also the cells of the batterys would balance themselves automatically when they are connected through the balancer ports.

I´m also curious how much the lipo warner(s) will drain the batterys and if one should unplug them while not riding for a few hours.

EDIT: After sketching the circuit like a 5 year old, i realised that plugging the balancers parallel in a serial setup will cause baaad shorts :smiley: So no good idea.

<img src="/uploads/db1493/original/2X/f/fcfe2394dea563d580e253eed295e32e983d8424.jpeg" width="666" height="500">
```

---
## \#2 Posted by: PB1 Posted at: 2016-07-18T11:42:05.138Z Reads: 113

```
Hello @kampfhahn
don't do that! Your cells are not at the same voltage!


Aaah, just saw your edit. Glad you figured it out yourself.
```

---
## \#3 Posted by: DerBrecher Posted at: 2016-07-18T11:43:17.476Z Reads: 114

```
@kampfhahn I am happy you found that out before you tested it. Otherwise your balance leads would have had a bad time :grin:
```

---
## \#4 Posted by: kampfhahn Posted at: 2016-07-18T11:46:25.364Z Reads: 109

```
Thanks guys :smiley:

Any idea about the amount of battery draining of the lipo warners?
```

---
## \#5 Posted by: DerBrecher Posted at: 2016-07-18T11:57:04.801Z Reads: 99

```
I am not sure probably only a few mA but so it should not matter when you are driving. But make sure you disconnect the checker when you are not using the board because their will drain the batteries empty and you get a puffy LiPo this will take very long because we have such high capacities on our boards but after a few weeks it will happen. So stay safe and disconnect the checker if you are not going to use the board on the same day.
```

---
## \#6 Posted by: PB1 Posted at: 2016-07-18T14:15:58.589Z Reads: 83

```
Not sure about this specific model here, but some lipo warners / checkers only use one cell to drive the display. Not a big deal if you ride for an hour. However if you leave them on the specific cell will get drained quicker than the others.
```

---
## \#7 Posted by: gordy Posted at: 2016-07-20T08:00:01.732Z Reads: 65

```
You could always wire a small switch into the negative feed to the lipo warner so that you can switch it off when not in use.
```

---
