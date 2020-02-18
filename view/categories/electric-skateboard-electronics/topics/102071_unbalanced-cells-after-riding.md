# Unbalanced Cells after riding

### Replies: 18 Views: 276

## \#1 Posted by: footloops Posted at: 2019-09-22T03:18:03.708Z Reads: 102

```
Hello, everytime I go out for a ride, my LiPO's are always unbalanced severely. I use 2s LiPO's with 5 in total in series to give me 10s. After a ride, 1 cell would be around 3v, while the other would be around 3.30v. I use a cheap china esc, which is what i'm thinking could be causing the issue as they appear to have regen braking.

What do you guys think could be causing this issue? (I plan on buying a flipsky 4.12 50amp later down the road as I save up).
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-09-22T06:08:19.253Z Reads: 90

```
@footloops  That happens when your cells aren't all the same capacity - lipo cells generally aren't as well matched as name-brand 18650 cells. A BMS helps some but not entirely. 

Also, you shouldn't run LiPo cells down anywhere near 3.0v - You should set your cutoff to 3.5 at minimum.
```

---
## \#3 Posted by: torqueboards Posted at: 2019-09-22T06:49:23.997Z Reads: 84

```
Don't use lipo voltage testers also. They'll drain your cells and make them unbalanced. Only use them for checking lipos don't leave them on.
```

---
## \#4 Posted by: telnoi Posted at: 2019-09-22T11:30:44.658Z Reads: 71

```
I'd rather say it is caused by a difference in lipos. Regen braking will automatically distribute evenly.

If you have a balance charger, deplete both lipos to the exact same voltage and charge them individually. See if the same mah goes into each. My guess is one will reach full charge sooner.

Lipo checker is fine during riding, I use 4 in total but also disconnect them after riding and balance charge my lipos. All 4 of mine only differ by 0.3v at most though after riding them down to 3.6v per cell during load.

What brand lipo do you have btw?
```

---
## \#5 Posted by: footloops Posted at: 2019-09-22T14:38:25.045Z Reads: 59

```
LiPO's can be at max, drained down to 3v. But i generally try to stay around 3.1v. And i also can't set cutoff as this is a cheap china esc rip.
```

---
## \#6 Posted by: footloops Posted at: 2019-09-22T14:39:39.386Z Reads: 55

```
I don't use lipo voltage testers unless you're referring to one of these: https://www.google.com/search?q=china+esc+battery+life+indicator&safe=strict&source=lnms&tbm=isch&sa=X&ved=0ahUKEwjKtqii1OTkAhVFLKwKHTQjDyIQ_AUIEigB&biw=2560&bih=969#imgrc=DSkpW6cothU0TM:
```

---
## \#7 Posted by: footloops Posted at: 2019-09-22T14:42:36.207Z Reads: 53

```
Hello, I use zippy 2s 2200 mah lipos. The thing is though is that apparently when my brother rode it and checked the lipos, the cells were all even, around 3.7v. But as he got closer to 3v, the cells all became unbalanced, differing about .3 - .4v. Confusing.
```

---
## \#8 Posted by: telnoi Posted at: 2019-09-22T15:17:25.328Z Reads: 52

```
I don't know where you get 3V from, but that will kill a Lipo quickly. 
3.6 is borderline imo. Lower than that considerable increases the temperature and negatively impacts the life span of the lipo. 

I am not surprised it starts drifting at 3v, since the slightly poorer Lipo (they are not all built equal) will start suffering a whole lot more.
```

---
## \#9 Posted by: footloops Posted at: 2019-09-22T16:36:32.410Z Reads: 50

```
3.7v is the average voltage of a lipo. Going down to 3.6v isn't really much of difference. Every site I go on, always states that going below 3v is harmful, but going to 3v isn't. I always try to stay within 3.1 - 3.3v after use, but the esc I use doesn't allow me to configure the voltage cutoff, so it sometimes cuts off at 3v. Sure it will cause the battery to wear down quicker than normal, but it isn't gonna kill it as fast as you think.
```

---
## \#10 Posted by: telnoi Posted at: 2019-09-22T18:05:09.301Z Reads: 47

```
[quote="footloops, post:9, topic:102071"]
3.7v is the average voltage of a lipo
[/quote]

Up to you. I killed my zippies (4 of them) by going to 3.2v. They will become puffy super quickly that way (in fact, I had to throw away most lipos that I depleted to that level/also with my drone lipos).

The performance also degrades super quickly below 3.6. Not much left in them as the voltage will drop quickly under load/lots of voltage sag.
```

---
## \#11 Posted by: MysticalDork Posted at: 2019-09-22T20:46:09.420Z Reads: 42

```
Hey, that's your decision to make my dude. You reached out asking for advice, we gave you a bunch. It's your choice whether to listen to the people you asked for advice or not. :woman_shrugging: Just don't come crying to us when your shit breaks.
```

---
## \#12 Posted by: footloops Posted at: 2019-09-23T01:44:51.478Z Reads: 35

```
I didn't ask for advice.... I asked for a solution to a problem. I understand that you can damage your lipos after reaching a low voltage point, but that doesn't explain why they're unbalanced after riding it until the cells reach around 3.3v. And if shit does break, then too bad too sad, I can always upgrade.
```

---
## \#13 Posted by: telnoi Posted at: 2019-09-23T02:16:53.894Z Reads: 34

```
![Lipo-battery-guide-Voltage-vs-capacity-used-percentage|630x449](upload://a9hHIclOWSyS6bkzbGn044oDqkK.jpeg)

This explains it pretty well. The per lipo capacity is the deciding factor for the sudden drop in voltage (the lower capacity lipo will reach critical voltage faster), thus at a critical low voltage that difference will show up more prominently. I bet it's always the same lipo. 

You can't fix that, there is no solution other than staying within the previously mentioned voltage range for both lipos (monitored separately).
```

---
## \#14 Posted by: MysticalDork Posted at: 2019-09-23T02:26:08.161Z Reads: 32

```
And I'm telling you, that the "solution to your problem" is to not subject your lipos to that level of ball-punching abuse. You're using small lipos and asking a lot of them, and this is one of the things you can easily change to reduce your problem.
```

---
## \#15 Posted by: torqueboards Posted at: 2019-09-23T03:46:12.984Z Reads: 28

```
I stop at 3.6v-3.7v. Your packs will only last for a few months if you attempt to go any lower before capacity will drop.

Ultimately, this is why 18650 packs are better because typically with LiPo. I've only ever gotten about 50-100 cycles if even and the packs are about 60% capacity after that.

At 3.6v fluctuations can drift pretty far to 3v or less especially if your hard on the throttle.

IMO 18650s are better and cheaper in the long run.
```

---
## \#16 Posted by: telnoi Posted at: 2019-09-23T05:24:18.360Z Reads: 27

```
Except if you need to go raw power and charge at 14A or higher ;)
I still love my lipos. They typically cost 250 a year for my board. After a year, They are ready for recycling.
```

---
## \#17 Posted by: footloops Posted at: 2019-09-23T13:38:30.033Z Reads: 19

```
Where would you recommend to purchase these cells? I am interested in creating my own pack just for the learning experience.
```

---
## \#18 Posted by: telnoi Posted at: 2019-09-23T15:32:03.113Z Reads: 17

```
You're welcome. Tjeez, kids these days.
```

---
