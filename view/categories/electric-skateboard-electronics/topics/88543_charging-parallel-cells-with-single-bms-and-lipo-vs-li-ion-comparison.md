# Charging parallel cells with single bms and LiPo VS Li-Ion comparison

### Replies: 12 Views: 148

## \#1 Posted by: piepolitb Posted at: 2019-03-28T07:00:51.612Z Reads: 51

```
maybe dumb question... is it possible to charge a 6s2p with a single 6s BMS ?

Trying to explain: what if I buy 12 18650 cells, configure them as 6s2p and treat each parallel couple as single cell? is it possible or do I need another 6s BMS ?
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-03-28T07:20:33.460Z Reads: 48

```
Yes, that's how it works. Each P block behaves as a single cell. If we had to treat each cell as an individual, a board with a 10s5p battery wouldn't have room for anything other than cells and BMSs lol
```

---
## \#3 Posted by: piepolitb Posted at: 2019-03-28T07:23:50.592Z Reads: 46

```
it makes sense :slight_smile:
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-03-28T07:24:31.194Z Reads: 45

```
Keep in mind, a 6s2p 18650 pack will be gutless as frig.
```

---
## \#5 Posted by: piepolitb Posted at: 2019-03-28T07:44:27.851Z Reads: 40

```
you reached my english limit... if you mean something like "not enough", yeah I know: it was an example for simple math and immediate understanding.

Actually I need a 12s (because I already have a charger and a bms) and I-don't-know-how-many-p: I'm just getting close to single cell buying. 
I'm trying to evaluate the total cost and I'm making my mind on the fact that ready-to-use-lipos are cheaper than Li-Ion cells assemblies for same energy and max discharging current. Am I right?


BTW what do "gutless as a frig" mean ??? I got "gutless"... but not frig!
```

---
## \#6 Posted by: MysticalDork Posted at: 2019-03-28T07:48:33.022Z Reads: 41

```
I was just trying not to swear lol

Lipos win in terms of power density (Watts per KG, Watts per Liter) but 18650s win in terms of energy density (watt-hours per KG, watt-hours per Liter).

Price really depends on where you get your batteries from and what quality they are. There are very cheap lipos and very expensive ones too. Same with 18650s.
```

---
## \#7 Posted by: mynamesmatt Posted at: 2019-03-28T08:01:22.604Z Reads: 40

```
look you can use one bms per p group. it's only really necessary if you have paranoia about cells not balancing properly though. it's just unnecessary 😊
```

---
## \#8 Posted by: piepolitb Posted at: 2019-03-28T08:28:39.936Z Reads: 36

```
oook. So let's get practical:

I'm already running with two of [these](https://hobbyking.com/it_it/zippy-compact-5800mah-6s-25c-lipo-pack-xt90.html) : 12s, 5800mAh and 25C for 130€ (BMS not included). 
It's a 12 x 3.7V x 5.8Ah = 257Wh battery package and 0.50€ for each single Wh.


I measured max 80A discharging in my configuration, so I was looking for something similar with at least 100A max discharging current. 

I was quickly searching in Nkon.nl through this nice filtering-website ([check this out](http://kevindark.co.uk/PublicServices/NkonFilter) ) 

I found [these](https://eu.nkon.nl/rechargeable/18650-size/sony-us18650vtc4-flat-top.html) (maybe) as best solution (for now...): I would need 48 of these cells for a 12s4p which would bring me 120A (90A seems to close to my measured limit), so 140€, cells only. 
Let's say 160€ with other manufacturing miscellenea (BMS not included).

In this case it would be 12 x 3.7V x 4 x 2.1Ah = 372Wh battery package and 0.45€ for each single Wh which is quite the same as before, but with some personal to-do on manufacturing.

Am I making any sense? Let's stick with lipo ?
```

---
## \#9 Posted by: MysticalDork Posted at: 2019-03-28T09:20:53.694Z Reads: 31

```
A couple points: Even though Sony VTC4s are rated for 35A, they sag very badly at the top end of their discharge curve, which makes them far less desirable than the numbers would lead you to think. Looking at [these graphs](https://imgur.com/a/r2udz), even at 20A they are sitting around 3.25v after 1Ah. Compared to the old trusty [Samsung 30Q](https://lygte-info.dk/pic/Batteries2012/compare/Samsung%20INR18650-30Q%203000mAh%20(Pink)-Capacity-20.0R.png) (rated 15A by Samsung but out-performs 20A cells at 20A), it retains more voltage across its curve and has about 40% more energy per cell, bringing the price down to 0.35€/Wh. 

Those 18650 prices are for single cells. Buy 50, and the price for VTC4s drops from 2.95 to 2.45 per cell, and the 30Q drops from 3.75 to 3.42.

Sure, a 12s4p 30Q pack will only give 80A but it'll actually sag less than the VTC4 pack would at that current, and it'd give you 518WH for 171€, or 0.33€/WH.
```

---
## \#10 Posted by: piepolitb Posted at: 2019-03-28T10:49:56.435Z Reads: 24

```
yeah, it is a better bargain in terms of €/Wh. But in this way I would be beyond my budget and I would get a 12000mAh battery package, which is twice my needs. 

I guess cells assemblies for eskating applications require more parallelized cells in order to get the typical currents required. It's like that there's some sort of high entry price, coming from low discharge rate with respect to Li-Ion cell capacity.

Correct if I'm wrong, but I think LiPo is still a better solution for me. Maybe for a future mountain board-like building with dual motor and higher required capacity, Li-Ion cells will overcome.

Nice learning, though! Thank you!
```

---
## \#11 Posted by: pat.speed Posted at: 2019-03-28T10:54:20.260Z Reads: 23

```
Something I’ve just noticed is not to be deceived by the manufacturers capacity ratings. These are the ratings when discharged at low currents. When used under loads like we use the capacity is less. A good example to stick with is with lipos you will get 70% of the rates capacity and Li-ions will get 80%, that is assuming the battery is true to the rating in the first place.

This should definitely be taken into account as it can decrease range by quite a bit from the estimated amount
```

---
## \#12 Posted by: Okami Posted at: 2019-03-28T11:29:34.290Z Reads: 21

```
I would aim for capacity not load, unless u plan going up hills all the time.

Choose cell with 2.5-3ah and u should be good.
```

---
