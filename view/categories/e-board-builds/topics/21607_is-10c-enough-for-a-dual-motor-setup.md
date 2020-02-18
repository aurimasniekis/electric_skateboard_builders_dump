# Is 10C enough for a dual motor setup?

### Replies: 14 Views: 1130

## \#1 Posted by: poviking Posted at: 2017-04-23T12:33:42.238Z Reads: 170

```
Hi there!

I'm planning to build my first electric longboard and I've done all the research that is needed.
The only thing is what batteries to choose. I was planning on 10s4p.  Would these batteries be enough for a dual motor/dual vesc setup with a 60A BMS? is 10C discharge rate enough or should I get a higher discharge rate battery? I'm trying to build the highest capacity battery pack with these cells [http://www.illumn.com/batteries-chargers-and-powerpax-carriers/batteries/18650-sanyo-ncr18650ga-3500mah-high-discharge-flat-top.html](http://www.illumn.com/batteries-chargers-and-powerpax-carriers/batteries/18650-sanyo-ncr18650ga-3500mah-high-discharge-flat-top.html)
```

---
## \#2 Posted by: lowGuido Posted at: 2017-04-23T12:39:02.230Z Reads: 169

```
10C is more than adequate at 4P. thats 140A continuous draw.
and considering that you are going to use a 60A BMS you should never see that kind of current anyway.
```

---
## \#3 Posted by: lowGuido Posted at: 2017-04-23T12:47:59.119Z Reads: 163

```
hold on.. I just looked at the battery in that link... its specs are 10A not 10C..
so that's only 40A not 140A as I previously stated..
```

---
## \#4 Posted by: poviking Posted at: 2017-04-23T13:18:01.001Z Reads: 151

```
So i should check on batteries with 10C dischsrge or higher?
```

---
## \#5 Posted by: lowGuido Posted at: 2017-04-23T13:21:59.970Z Reads: 147

```
10C would be fine. but those batteries are not 10C
```

---
## \#6 Posted by: saul Posted at: 2017-04-24T04:43:34.692Z Reads: 115

```
those are 10A, not 10C. only lipo are rated in C.
so no, 40a is not enough.
```

---
## \#7 Posted by: Okami Posted at: 2017-04-24T13:51:55.967Z Reads: 105

```
Im actually using these sort of cells for my mountainboard build but I have 6s6P pack

If you dont expect to draw more than 400w regularly, you might be okay but you are basically very close to the recommended limit.

Also depends on do you plan to go uphills.
For me power draw going up hill usually is about 30-40A (~860 W max)
And I've got single drive.

It has been said that ''safe'' / good power draw is about 3A (~1C) per cell, so in your case that would be 12A total, 6A per motor.

at 36v (10s), that would give you 216W per motor, and 412W total.
So if you go only on flats and not more than 30-35kph, it might be enough..

---

I dont have data on hot hot they become, but Ive heard they start to become hot if you draw 7A per cell from them and.. reasonably, capacity then is also lower.

For 4P pack, Samsung 30Q might be your best bet, you would get the desired 60A, would still be very close in capacity Sanyo's GA anyway, as I think they deliver more like 3.250 mah not 3.5ah as advertised.

So yeh, with samsung 30Q pack, at maybe 2.8ah usable capacity, you would still get 36v x 11.2ah = 403.2 Wh

For longboard this might be a huge range.. something like 40km probably or 25miles.
```

---
## \#8 Posted by: poviking Posted at: 2017-04-25T10:30:37.721Z Reads: 85

```
Okay, i don't wanna be in the safe zone😂. But ill try finding batteries that are atleast 10C and with the highest capacity available.
```

---
## \#9 Posted by: Okami Posted at: 2017-04-25T10:32:55.885Z Reads: 82

```
@poviking

U got to understand that for 18650 li-ions discharge is usually marked as '''max continous amperes''

while for lipo it is this ''C rate''

For lipo you would need 5-6ah pack with 20c rating to be safe, since it is recommended to ''downgrade'' the rating.
```

---
## \#10 Posted by: poviking Posted at: 2017-04-25T14:39:31.673Z Reads: 72

```
Yeah sorry, i know now. I should go with 20A discharge rate batteries. I dont wanna be in that "safezone".
```

---
## \#11 Posted by: Okami Posted at: 2017-04-25T15:48:27.184Z Reads: 62

```
yeh, if you plan to conquer hills or speed everywhere like a daredevil, get some higher output cells..

Sanyo's also might sag a bit more than others for this reason, hence lower power output / speed a bit.
```

---
## \#12 Posted by: poviking Posted at: 2017-04-25T15:59:38.898Z Reads: 61

```
You think these to be good, or should i get other brand?
What is your exprience with LG brand cells?

http://www.illumn.com/batteries-chargers-and-powerpax-carriers/18650-lg-18650g2-3000mah-high-discharge-flat-top.html
```

---
## \#13 Posted by: Okami Posted at: 2017-04-25T22:12:42.047Z Reads: 50

```
Seems okay to me! I know vapers use these a lot and also @whitepony used them.. so far.. Haven't seen anything bad being said about these cells..Not sure are they the newest.. but should perform decently..

If you do wish to study batteries thoroughly, I recommend for you to visit this site:

http://lygte-info.dk/review/batteries2012/Common18650comparator.php

You can quickly take a look at different specs of different make batteries.

The site is a very good reference point to see whenever the choosen cell will perform as you ''planned''.

--

In short - cell is quite good, the price would be the one which bites! Ask @PXSS whenever it is still possible to get 30Q cells for a low price. He managed to order some from Nkon internatioal site for quite a bargain.. ask him whenever it is possible to get 30Q.. but if you are very forward with getting ''officially'' stated 20A cell.. then go with HG2 cells or similar, even though it looks like 30Q performs good enough for not high enough / maximum loads.

--

Looking at this, it looks like 30Q performs a bit better than HG2 actually but im not informed about the temprature these cells face at these discharge levels!

<img src="/uploads/db1493/original/3X/4/e/4e63dc15990d3df61d756b1da0731f2df09fe0b5.png" width="690" height="430">

Im not sure do you regularly need more than 10A per motor (total 20A for 4P pack @5A per cell.. So that is why I chose 5A, but for 7A it is similar, the capacity might be a bit less
```

---
## \#14 Posted by: poviking Posted at: 2017-04-26T13:18:14.978Z Reads: 32

```
Thanks mate, i will try asking him.
```

---
