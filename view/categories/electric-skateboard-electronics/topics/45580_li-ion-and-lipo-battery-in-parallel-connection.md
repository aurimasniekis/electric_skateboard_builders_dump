# Li-ion and Lipo battery in parallel connection

### Replies: 7 Views: 911

## \#1 Posted by: davewood1982 Posted at: 2018-02-04T23:22:17.343Z Reads: 121

```
Li-ion and Lipo battery in parallel connection , can they work simultaniously? I have a spare lipo battery pack im not really using so the question is, What would happen if i were to hook it up in Parallel with my other battery which is a Li-Ion?
```

---
## \#2 Posted by: b264 Posted at: 2018-02-04T23:24:07.808Z Reads: 121

```
At a minimum, you won't be able to run your Li-Ion down all the way.  I don't know if there would be any other issues
```

---
## \#3 Posted by: PXSS Posted at: 2018-02-05T02:26:39.265Z Reads: 98

```
You're asking for trouble tbh. 

They are different chemically (ever so slightly) therefore they have a different internal resistance. This mismatch of IR means that the cells get loaded unevenly, not only that but the cells with higher IR will run hotter. 

Liion and Lipo also have different voltage profiles as they discharge. So this might harm the load sharing too. 

Then there is also the fact that lipos are empty at 3.0V while Liions are empty at 2.5V so you will not be able to use full capacity. 

Given that Lipos can usually pull loads tenfold that of liions, if you load the battery too much, you could cause the liions to overheat and have a voltage collapse which could lead the lipos to blow. 

There are lots of things that could go wrong. Without lots of testing and data analysis, this is extremely dangerous and I would advise anyone against it
```

---
## \#4 Posted by: Namasaki Posted at: 2018-02-05T03:53:36.751Z Reads: 75

```
If you overheat the Li-ions as @PXSS suggested, they could go into thermal runaway and turn your board into a rolling bonfire.
Better to not take chances.
```

---
## \#5 Posted by: krloz Posted at: 2018-02-05T07:09:49.820Z Reads: 64

```
I'm not quite sure the difference in chemistry would overheat lion. I guess as Lipo cam give more discharge amps they would push more amps when needed.  Balancing back up from the lions when not needed. This could cause some inefficiencies but just as when mixing C ratings. But I'm nor 100 % sure
However as stated. You will be over discharging your Lipos. Or best case under discharging lions. Do you are better off if you make a swappable system and plug the other when the first is empty. 
Be careful with the vesc voltage cut offs.  If you set them for lions add an alarm to the lipo
```

---
## \#6 Posted by: PXSS Posted at: 2018-02-05T12:49:45.648Z Reads: 42

```
[quote="krloz, post:5, topic:45580"]
Lipo cam give more discharge amps they would push more amps when needed.  Balancing back up from the lions when not needed.
[/quote]

The issue is that the internal resistance of lipos is 5ish times lower than that of Liions. So at any point in time your Lipos need to provide 5x the power than Liions, if this is not true then you are overloading the liions and if you do so the voltage will sag, voltage sag equals higher ir which equals larger voltage sag and more heat, this is called voltage collapse, and although it is not terribly dangerous for liions, it is for Lipos. I honestly do not have much experience in said field so take everything with a grain of salt but yeah, this could be quite dangerous
```

---
## \#7 Posted by: davewood1982 Posted at: 2018-02-05T16:25:25.234Z Reads: 35

```
Thanks guys, just wanted to know about the risks, probably not worth the risk
```

---
