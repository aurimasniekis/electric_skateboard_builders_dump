# Samsung 40T - 3900mAh 30A cdr (45A MVA) - avail mid 2018

### Replies: 9 Views: 2620

## \#1 Posted by: Vanarian Posted at: 2017-12-12T20:07:49.720Z Reads: 194

```
Hey, I just saw this in the french forum :japanese_ogre:

 https://www.e-cigarette-forum.com/threads/bench-test-results-samsung-40t-21700%E2%80%A6a-great-30a-3900mah-battery-better-than-ncr20700a.842165/

<img src="/uploads/db1493/original/3X/9/7/97064c55a502a9d8ebff340856dcd934f741afce.png" width="690" height="340">

Available mid 2018 ! Anybody wanna build a 120A 4P 15900mAh pack ?
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-12-12T20:12:56.979Z Reads: 187

```
21700 is such an awkward form factor for our boards. it doesn't quite cut a 30Q 4P in half (meaning a 2P 40T isn't as much capacity as a 4P 30Q) yet takes up more physical space. 

I might be able to fit 36 of these on a board tastefully. If so, thier higher discharge rating would make them good for short distance sprints, such as for racing, where you may not need a lot of watt hours but you want a lot of power at the wheel. 

When are they going to cram these characteristics into an 18650? i demand answers. lol
```

---
## \#3 Posted by: evoheyax Posted at: 2017-12-12T20:14:44.270Z Reads: 181

```
Any news when the 30T will be available?

Still beats the 40T he first half of the charge in sag. Plus they are 40a cells, so 120 amp in 3p. I have hollow core decks being made right now that will fit 12s3p + 4x vesc + bms of these 21700 cells :) Will be ready :)
```

---
## \#4 Posted by: Vanarian Posted at: 2017-12-12T20:51:22.614Z Reads: 167

```
Ha no news yet! I'd predict April 2018 for release :wink:

@longhairedboy I'm sure you can fit them (given the tree wiring you sorted through your decks) one way or other.
```

---
## \#5 Posted by: torqueboards Posted at: 2017-12-12T20:58:02.076Z Reads: 157

```
Looks like a sweet cell. They are most likely much more expensive though.

I have a 12S4P 21700 48G 4800mah. Should get a ton of range 19,200mah. Haven't tested that one yet though. 10A only though.
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-12-12T20:59:10.174Z Reads: 153

```
i would actually prefer a 2.5ah cell that was smaller than the 18650 if we want to get into what i think would be ideal. 

distributing the load over more cells is generally a better idea in my opinion than consolidating lithium into as few cells as possible when trying to mitigate voltage sag and things of that nature. 

that opinion is based solely on what i've seen with my own eyes, not based on theory or conjecture, so it may be biased by my environment and personal experience.
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-12-12T21:02:30.227Z Reads: 146

```
i highly recommend AA’s for packs like that. you can pack tons of them in a small space, I also saved money by using aluminum foil as nickel strip
```

---
## \#8 Posted by: rojitor Posted at: 2017-12-12T21:34:54.773Z Reads: 142

```
[answers](http://www.cell.com/joule/fulltext/S2542-4351%2817%2930180-0)

It's very technical and boring so....translation: they found out how to triple li ion. These kind of things are usually not happening tho. Bad for business ...
```

---
## \#9 Posted by: PXSS Posted at: 2017-12-12T21:51:35.936Z Reads: 137

```
[quote="longhairedboy, post:2, topic:40847"]
it doesn't quite cut a 30Q 4P in half (meaning a 2P 40T isn't as much capacity as a 4P 30Q) yet takes up more physical space.
[/quote]

All the 21700 cells available are less energy dense than the equivalent 18650.

Drawing a continuous or ***average*** of 10A per cell:
GA cells have 605Wh/L
30Q have 566Wh/L
30T have 440Wh/L
40T have 550Wh/L


The issue with the GA cells is that they would be running extremely hot so that kind of makes them useless for anything higher than 5A per cell continuous with 10A bursts of maybe 30s-1min

That is also assuming that you can fill all the nooks and crannies. If we assume they are cuboids...

GA = 476Wh
30Q = 444Wh
30T = 346Wh
40T = 431Wh


---

[quote="longhairedboy, post:2, topic:40847"]
thier higher discharge rating would make them good for short distance sprints, such as for racing, where you may not need a lot of watt hours but you want a lot of power at the wheel
[/quote]

Correct! But then you also have Lipos...
```

---
