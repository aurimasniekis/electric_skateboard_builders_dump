# Battery Dilemma &#124; Dual Motor cheap ESC build

### Replies: 9 Views: 263

## \#1 Posted by: TheArus Posted at: 2018-12-16T22:47:50.964Z Reads: 106

```
Hello there! I was looking for a similar post on forum but nothing found so far. I have two Racerstar 6368 Motors 
https://banggood.app.link/bh3ArbPOHS which are rated for 6-12S and two Racerstar 120A ESCs
https://banggood.app.link/lZa2qv0OHS (don't judge me, i am going to buy VESC someday).  The esc is rated for 6S. I would like to create dual motor build. I have two 6S 8A batteries 
https://banggood.app.link/OQy6vi7OHS and i have no idea of how to connect them. Should I connect each esc to each battery? Or connect them in parallel? Or use some BMS? (i would like to get rid of my microprocessor charger and use casual power supply).
```

---
## \#2 Posted by: Grozniy Posted at: 2018-12-16T22:54:04.252Z Reads: 101

```
Connect in parallel the batteries, then connect to ESC's
You can use a BMS. Search for 6s lipo bestech or supower BMS. Because of high amperage, search charge only bms
```

---
## \#3 Posted by: totalgeek9224 Posted at: 2018-12-16T23:34:03.908Z Reads: 80

```
dont you mean charge only? :p
```

---
## \#4 Posted by: totalgeek9224 Posted at: 2018-12-16T23:39:48.225Z Reads: 73

```
Any whom, to keep the setup that you've linked with minimal changes, id say hook a battery to each ESC, link the ESC's with CANbus or PPM. The only issue with this is that it means two BMS's if you chose to go that route, which is.....meh. I'd suggest looking at some alternative ESC's. Even if getting a VESC now means single drive- Thats okay for the sake of reliability and safety.
```

---
## \#5 Posted by: TheArus Posted at: 2018-12-17T06:50:36.583Z Reads: 49

```
Well, two people and two different responses. What are the pros and cons of both options? Will my setup be powerful enough to carry my 95kg? Or it's better to create single motor build using such a weak ESC?

edit: my motor is rated 60A for 6s, which BMS should I use for two Motors and parallel battery connection? 60/80/100/150A?
```

---
## \#6 Posted by: totalgeek9224 Posted at: 2018-12-17T07:55:24.300Z Reads: 39

```
Give me a minute I'll respond to this, but note- focbox is back on sale for $99, not that much above your linked esc's yet tried and tested
```

---
## \#7 Posted by: totalgeek9224 Posted at: 2018-12-17T08:22:46.820Z Reads: 35

```
HM maybe I've misunderstood. It's your motor limiting you to 6s? That's a different story then.

As for the bms, if you go for a VESC, then you'll be onak going fused and charge only. This would be cost effective and has no real drawbacks for the setup. If you chose to go this route, the VESC would be reliable for discharge protection, and would eccentuate the importance of a good VESC.

If you truly want to get a charge/discharge bms, search with bestech or some other brand with a minimum of 100a discharge (assuming then that you run each motor at 45 or so amps) leaving you with some safety headroom. That being said, if you want to push everything to that max, then 150A would be your best bet for a bms.

As for the power of your setup, I think that it should be powerful enough if everything acts like it's supposed to. That being said, if the motors aren't really putting out what they say they are rated for, of the ESC is weaker than advertised, or even the batteries, then it's really a toss up. What terrain do you live in? Hilly, flat? And what kind of board are you hoping to build? An MTB kind of thing or more of a street cruiser?
```

---
## \#8 Posted by: TheArus Posted at: 2018-12-19T22:52:58.248Z Reads: 19

```
No, my motor is 12s max. Thanks for your help, i've ordered two focbox VESC on sale. Now i would like to connect them in series (to have 12s). Should i use 12s BMS or 6S?
```

---
## \#9 Posted by: totalgeek9224 Posted at: 2018-12-19T22:54:12.158Z Reads: 18

```
12s bms for the packs connected in series!
```

---
