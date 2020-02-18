# Is this how I can use my batteries in series and charge them individually?

### Replies: 5 Views: 859

## \#1 Posted by: itsmikeholland Posted at: 2016-07-19T15:34:33.934Z Reads: 106

```
So for the time being, I'm going to just use 1 80W charger to individually charge my 4s 99wh batteries till the 4x 6s monster is back in stock, so I need a solution to run all 3 in series while being able to charge them individually. I'm an absolute newbie, and have screwed up every step prior to this, so could somebody look over this diagram and let me know if this is how it should look? Also, what material should I be soldering with? I have a soldering gun, but no lead or anything. Thanks guys! I'm stoked to get this board running! is anything missing from this diagram?

<img src="/uploads/db1493/original/2X/5/59e1954bf28b8c3d3ee5fe311705ebc69a418eea.png" width="690" height="431">
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-19T15:47:59.148Z Reads: 101

```
If you're going to be charging 12s, how are you going to be plugging in the balance leads. Does your charger support 12s balancing?

Your diagram is correct for the main terminals, you'll just need a 12s charger or BMS to balance. 

I use 60/40 rosin core solder myself.

EDIT: nevermind misread. Your setup looks good as long as you unplug each one for charging. make sure you have an anti spark loop!
```

---
## \#3 Posted by: itsmikeholland Posted at: 2016-07-19T17:15:02.071Z Reads: 88

```
Awesome! Do I just need one between the vesc and the last battery connector, or do I also need to add antisparks in between the batteries?
```

---
## \#4 Posted by: Jinra Posted at: 2016-07-19T17:23:53.756Z Reads: 80

```
Just 1 is fine. It only sparks when the circuit is completed. I would put it on your series connector on either the positive or negative wire.
```

---
## \#5 Posted by: itsmikeholland Posted at: 2016-07-19T17:33:05.116Z Reads: 73

```
Sweet, I ordered the Chaka vesc with an antispark on the battery side, so I think that'll take care of it. I seriously couldn't be more excited about this build now that I have an arrival date for the last key part! Thanks for all of your input!
```

---
