# Connect Lipo with Laptop battery

### Replies: 11 Views: 922

## \#1 Posted by: IsTalo Posted at: 2017-03-11T14:51:47.581Z Reads: 65

```
Hello Guys, I have a 6s 6300mah Lipo Battery from Alien, but in the future I want to start using Hub Motors, so I'll have to use 10s batteries, I find in my country a laptop battery that is 2s 6300mah and it have a nice price, but it is Li-Ion and I want to know if I could connect them in series? And about the different C-Rating, there will be any problem?
```

---
## \#2 Posted by: Montiey Posted at: 2017-03-11T16:20:19.661Z Reads: 58

```
Li-Ion Packs are not the same as Li-Po, but I don't know anything about them so I can't tell you which is better. By laptop battery, I assume you mean single round cells? To make a 10S pack you would need 10 of the cells, and maybe another whole set of them in parallel for more capacity.

I wouldn't recommend using any different batteries together, especially not with different C ratings… Some people stay so far away from mixing batteries that they buy 3x as many as needed and only use those that are exactly the same, much less different cells all together.

Before you buy any, figure out if they have the C rating you need: 3600 * number of parallel packs * C rating.
But depending on the ACTUAL C rating, those laptop batteries may be too weak! You may end up needing 4 sets in parallel to feed your motors, which would be ridiculous. How much current do the hubs draw at maximum power / stall current?
```

---
## \#3 Posted by: locktight Posted at: 2017-03-11T16:24:33.181Z Reads: 50

```
I wouldn't recommend this however it is possible. You will have to make sure the mAh rating is the same for both batteries so that one doesn't drain faster than the other. Constantly check the voltage and balance of the batteries. Dont exceed the draw rating for the labtop battery as it is the weakest link of the two.
```

---
## \#4 Posted by: VikasG Posted at: 2017-03-11T20:48:21.643Z Reads: 39

```
NEVER MIX  BATTERIES WITH DIFFERENT CHEMISTRY. Also, when you connect in series, its recommended to use 2 of the same series to scale up (2x5s in series for 10s). But seriously, don't mix chemistry - it could be very dangerous and you often lose capacity even if it works because of the different operating voltages.
```

---
## \#5 Posted by: IsTalo Posted at: 2017-03-11T21:01:31.286Z Reads: 34

```
A lot because it don't have gearing, I imagine something like 60A max, really don't know exactly
```

---
## \#6 Posted by: Maxid Posted at: 2017-03-11T21:03:00.780Z Reads: 32

```
Don't generalize - I am runnung 6S4P Liion parallel to a 6S Lipo just fine. Important thing is the parallel connection.
```

---
## \#7 Posted by: IsTalo Posted at: 2017-03-11T21:04:26.086Z Reads: 33

```
Yeah, but I want to put it in Series, I think I'm going to buy 5 of these and make a 10s 6300mah
```

---
## \#8 Posted by: mmaner Posted at: 2017-03-11T21:06:53.475Z Reads: 30

```
The reason, at least one of thrm, I'd that the charge & discharge rated for lion and lipo are very different. Also the max charge and discharge rates are very different. 

If you are going to balance charge the packs separately and check each cell while charging, you would probably be ok.  But it's a pain j the ass to do that.
```

---
## \#9 Posted by: VikasG Posted at: 2017-03-11T21:15:19.048Z Reads: 32

```
I'm not saying it won't work but it is generally not recommended. Also, don't you lose capacity because of the different operating voltages?
```

---
## \#10 Posted by: Maxid Posted at: 2017-03-11T22:26:21.099Z Reads: 28

```
Yeah some energy can not be used - but still better than not having both batteries in the first place. If you had to buy them it is obviously not recommended but if you have them lying around why not use them?

In my case I am not able to fully utilize the Liion anyway because the ESC has cut-offs tailored to Lipos. Damn Car ESCs :)

Saying "never do ..." In all caps does not look like just a recommendation though does it?
```

---
## \#11 Posted by: Namasaki Posted at: 2017-03-11T22:38:58.825Z Reads: 23

```
Don't mix battery chemistries, especially in series.
You would do much better to buy another 6s pack like the one you have and put them in series.
Batteries and electronics is not where you want to cut corners and pinch pennies.
```

---
