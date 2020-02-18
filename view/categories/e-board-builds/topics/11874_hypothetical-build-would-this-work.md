# Hypothetical Build: Would this work?

### Replies: 8 Views: 773

## \#1 Posted by: Jaeger_34 Posted at: 2016-10-25T17:38:20.909Z Reads: 107

```
Hey guys, after about a month of research I have a possible build of what I want my board to be. The part list is as follows: 

TORQUE Single Hub Motor Kit (From DIY) - $229.72 USD

VESC BLDC Speed Controller (From DIY) - $88.00 USD

4 to 5.5mm Wire Extensions (From DIY) - $7.56 USD

ONYX 11.1 3S 5000 mAh x 2 (From local seller in Toronto) - $160 CAD 

Rayne Avenger 37" Cruising Deck- $189.00 CAD
_________________________________________________________

The part that is stumping me now is how to connect the two batteries in series. I would need a connector for those, right?    

At any rate, would this build work? Please let me know, thank you!
```

---
## \#2 Posted by: Luke Posted at: 2016-10-25T18:31:10.022Z Reads: 91

```
Yup there's a series connector you can use for that, but how fast do you plan on going and do you live in a hilly environment?
```

---
## \#3 Posted by: sl33py Posted at: 2016-10-25T18:44:08.974Z Reads: 79

```
[quote="Jaeger_34, post:1, topic:11874"]
ONYX 11.1 3S 5000 mAh x 2 (From local seller in Toronto) - $160 CAD
[/quote]

Not familiar with the Onyx brand, but 80 CAD seems a bit high...

compare with an inexpensive [ZIPPY Flightmax 5000mAh 3S1P 20C](http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=8579) - which are about $20-25 ea.  Shipping and import fees... not sure, but worth looking at?  I would target a minimum of 20c for a 5000mAh pack (more is better: 25c, 30c, etc.)

as for series connector - my favorite is a simple xt90/xt60 adapter.  Here's one i did that's stupid simple:

[img]https://goo.gl/OUuBDF[/img]
[img]https://goo.gl/EH9wIH[/img]

Easy to make, and you can avoid a spaghetti mess of wires w/ your typical adapters from ebay/amazon/etc.

HTH - GL!
```

---
## \#4 Posted by: Jaeger_34 Posted at: 2016-10-25T18:46:39.434Z Reads: 61

```
since I'm using a 6s config, im only planning on going the 20mph the specs suggest. I don't live in a terribly hilly area in Toronto, so It should be fine.
```

---
## \#5 Posted by: Jaeger_34 Posted at: 2016-10-25T18:49:38.102Z Reads: 59

```
I don't think I'd be able to get those across the border since they're all over 100 watt hours. I've tried to see if i can order them to Canada, but it doesn't show up. As for the C rating, what does that mean?
```

---
## \#6 Posted by: sl33py Posted at: 2016-10-25T18:57:16.765Z Reads: 58

```
C rating is used for both charge and discharge rates.  You have a constant C for how many amps they can provide and a C for peak amps they can provide.

Simple math to determine is the Ah x C = xxx Amps.  So a 5000mAh/5Ah x 20c = 100A.  Please understand this is totally suspect and likely marketing.  The higher discharge they can provide - the less voltage sag under load.  Less heat, more pack life, etc.  But usually more $$ too.

I personally set the *minimum* constant amp capacity of 100A.  So i typically avoid 10c packs.

I know the 100 Wh limitations can be a pain, but i've ordered large lipos in the past from HK without any issues.  Slow shipping via ground not air, but not a huge deal if you can wait.

GL!
```

---
## \#7 Posted by: Jaeger_34 Posted at: 2016-10-25T23:26:42.075Z Reads: 42

```
Thanks dude, I really appreciate it! 

 One more question. What charger do you recommend? Also, would I have to unplug each battery to charge it, or is there a way to charge them in parallel?
```

---
## \#8 Posted by: mmaner Posted at: 2016-10-26T00:01:04.998Z Reads: 38

```
Get a 6s to 2 3s balance adapter and you can charge I'm series.  I'd suggest the ax by, been around forever, cheap and do the job.
```

---
