# Question about a 10s5p LG HG2 pack

### Replies: 15 Views: 435

## \#1 Posted by: never4getf150forums Posted at: 2018-05-30T06:03:36.733Z Reads: 123

```
so.. i recently bought a used LG HG2 10s5p pack, they're all at about 2,880-2,900 mah capacity.

I would like to convert this pack into a 10s6p pack, and I bought a few more hg2 cells, these are brand new at 3000 mah capacity.

Would it be ok to add the slightly newer batteries in a separate P, would this be a fire hazard or should it be fine?
```

---
## \#2 Posted by: Ishayc Posted at: 2018-05-30T06:07:50.703Z Reads: 121

```
I wouldn't do that if i were you.
If the capacity has changed it means the drain might be different which means the voltages of the old cells will differ from the new ones when you discharge them.
```

---
## \#3 Posted by: never4getf150forums Posted at: 2018-05-30T06:10:43.163Z Reads: 115

```
i'm ok with that, my question is will it be an issue like a fire hazard, if it just drains the battery unevenly with no other problem it should be fine
```

---
## \#4 Posted by: Eboosted Posted at: 2018-05-30T06:20:32.030Z Reads: 108

```
You can't not combine different cell capacities, one cell will charge at 3000mAh and the other will keep flowing current even though has already been full, fire hazard that no bms could ever detect as they are part of the same pack.
```

---
## \#5 Posted by: never4getf150forums Posted at: 2018-05-30T06:22:48.208Z Reads: 102

```
is it possible to then make them charge at just 2900 instead of the full 3,000?
```

---
## \#6 Posted by: Eboosted Posted at: 2018-05-30T06:35:58.212Z Reads: 99

```
No, the batteries charge at 4.2v SOC that means 100% of their capacity, no matter if they are 1000mAh or 3000mAh, but one will deplete faster than the other no matter what. So when your highest capacity cell reaches 3v the lower capacity cell will be all the way down to 1.5v and you will need to change it after the first ride.
```

---
## \#7 Posted by: never4getf150forums Posted at: 2018-05-30T07:01:06.108Z Reads: 91

```
gotcha, so there is absolutely no way at all to use the newer cells and make it a bigger pack correct?
```

---
## \#8 Posted by: pat.speed Posted at: 2018-05-30T07:14:10.055Z Reads: 84

```
What if he were to open the pack and add one new cell to each parallel pack. That way each lot of cells will increase by the same amount of mah. It would be a lot of effort though and I’m not sure it would be worth it.

If this has already been mentioned, sorry I skipped through
```

---
## \#9 Posted by: Eboosted Posted at: 2018-05-30T07:20:51.601Z Reads: 80

```
This is what the original question was and the answer is the same, because of my previos post.

Don't do thatguus not worth it, buy/build a new battery, safer for everyone
```

---
## \#10 Posted by: pat.speed Posted at: 2018-05-30T07:38:30.360Z Reads: 82

```
But when connected in parallel it is essentially just 1 big cell, which means the cell would only charge to 4.2v no matter the capacity each cell has. Well at least that’s how I recall paralleling cells works


Edit: Also as stated here, although does not take into account aging and differing ir 

 ![image|281x500](upload://cIaYkqrfLznBEu6gtQsedzO2FtI.jpeg)
```

---
## \#11 Posted by: linsus Posted at: 2018-05-30T07:40:47.410Z Reads: 72

```
Technically its not impossible. You just need a charger that is accurate on meassuring internal impendance and you can match your cells somewhat. Just cause the cells are branded 3000 mah doesnt mean they'll have it coming out of the box. They're probably mora around 2900 as avrage so I'm not too concered about the actual capacity of the cells. If the older pack has significant aging the drain and charge will differ between the cells however so you would need to rip the pack apart to make safe assumptions. A job that will consume alot of time. I'm with @Eboosted on rather rebuilding a new pack to get best result possible.
```

---
## \#12 Posted by: Eboosted Posted at: 2018-05-30T07:59:19.715Z Reads: 68

```
On the other hand, you need to consider the maximum safe discharge rate of each cell, if you parallel cells with different discharge rates and set you maximum to the highest cell, the lower discharge capacity may raise the temperature causing eventual thermal runway.
```

---
## \#13 Posted by: linsus Posted at: 2018-05-30T08:03:16.444Z Reads: 64

```
6P tho,unless he has hell of a beast of a board he wont be touching the Specified max. cont. dis. of 120A. 

setting max 80A should give enough headroom
```

---
## \#14 Posted by: onepunchboard Posted at: 2018-05-30T13:29:22.868Z Reads: 43

```
I doubt it will be fire hazard, people make battery wall with random laptop batt.
if you mix old and new they tends to drift voltage a lot when charging. 
I've noticed 1 or 2 cells always have 0.1~0.3 volt lower and other cells gose 4.21 for 0.5 sec and come back sometimes, during charging.

It took me 30min ~1hr longer to charge and cells get touch warmer but there is no fire.

However, bms gets hot because longer balance charging time and that can be problem if the board is already hot after ride. 

Also, battery cycle may be affected because of such irregular charging and discharging.

if you can keep the battery like 4.15 at full charge, I think it will be safe and the cycle improves. that is maybe way to go for you.

and interms of discharging with set of proper cut off, all the cells end at same voltage, with 0.02 voltage differences. again I don't worry about it I've drained completely and charged right away after.

with 10s6p u will have to 120 ( with old pack may be110?)  batt amp but i doubt that would happen often unless if it's hard core mtb.

and 100mah is only 3% difference from original capacity which is already present in brand new batteries anyways I bet you wouldn't even notice voltage differences occurs to me.
```

---
## \#15 Posted by: never4getf150forums Posted at: 2018-05-30T16:38:20.676Z Reads: 28

```
cool thanks!

@ARetardedPillow

please read this, what do you think!? :smiley:
```

---
