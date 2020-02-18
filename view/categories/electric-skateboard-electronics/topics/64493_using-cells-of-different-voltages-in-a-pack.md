# Using cells of different voltages in a pack

### Replies: 4 Views: 142

## \#1 Posted by: mojoo999 Posted at: 2018-08-10T21:31:32.861Z Reads: 57

```
I just bought 50 Samsung 30Q cells from NKON. Most are 3.42V and 3.43V, but some are 3.45V and 3.46V. Are they all safe to use in the same pack? I heard they need to be within 0.01V of each other.

It's been suggested that I use the higher voltage ones in the same parallel. Unfortunately, my configuration doesn't allow to me to use all of the higher voltage cells evenly in parallel. Would be it be catastrophic failure if I go ahead and use them without regard to their voltage difference? I've already waited too long to receive them in the first place, I'd hate to have to wait a few more weeks to get newer ones.
```

---
## \#2 Posted by: pat.speed Posted at: 2018-08-10T22:36:58.682Z Reads: 49

```
They are all good, it is just reccommend when connecting them all together to make sure they are at a similar voltage. This is due to the higher voltage cells trying to charge the lower voltage ones. 

If possible I would balance the cells or at least drain the higher ones a tiny bit so they are the same as the others. IMO I think they would be fine as the difference is minuscule, but I also haven’t build my own 18650 batteries
```

---
## \#3 Posted by: Chase Posted at: 2018-08-11T00:14:37.324Z Reads: 34

```
I’ve spent a lot of time prebalancing cells. I doubt that much difference will matter. Your bms will kick in when one gets fully charged and bleed off the extra voltage until they are all equal.

To be safe you could always buy a 10 dollar usb charger for single cells from amazon and put the low cells on for a couple minutes until they match.
```

---
## \#4 Posted by: Brdchris Posted at: 2018-08-11T01:47:59.461Z Reads: 28

```
If you are using a bms I wouldn’t worry. If anything, I would just mix the high and low voltage in the same parallel groups as they will balance themselves across that particular p group.
```

---
