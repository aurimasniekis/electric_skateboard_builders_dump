# Need help choosing ESC motor

### Replies: 11 Views: 1096

## \#1 Posted by: pcbacon Posted at: 2017-03-07T23:24:08.319Z Reads: 65

```
I have 2 6S 10C 5200 mAh batteries that are connected in parallel. I am not going for the fastest speed but hoping to get about 20 Km out of it. I was maybe looking for a VESC my budget is around $200 USD for esc and motor i can go over a bit more.
```

---
## \#2 Posted by: sl33py Posted at: 2017-03-07T23:40:37.852Z Reads: 65

```
VESC typically are around $100
Motor - 60-120 (DIYes, Enertion have some good 63mm options) - also look for groupbuy and Maytech options for less.

Mount?  That might blow your budget, so look at @korryh and see if he has any left?  Or enertion or DIYes mounts.

GL!
```

---
## \#3 Posted by: pcbacon Posted at: 2017-03-07T23:46:52.982Z Reads: 59

```
i already made my own mount and i have the gears and belt. should i get the VESC BLDC Speed Controller and the Electric Skateboard Motor 6355 190KV? i have the tiny remote that I got from a group buy last year.
```

---
## \#4 Posted by: pcbacon Posted at: 2017-03-07T23:55:36.208Z Reads: 54

```
^ Sorry forget to tag you in the last post
```

---
## \#5 Posted by: caustin Posted at: 2017-03-08T00:13:41.777Z Reads: 53

```
Yes!

10 char
```

---
## \#6 Posted by: pcbacon Posted at: 2017-03-08T00:47:35.723Z Reads: 48

```
does the torque boards vesc have a power button or switch on it?
```

---
## \#7 Posted by: sl33py Posted at: 2017-03-08T00:59:44.767Z Reads: 48

```
As long as you don't expect "rocket" acceleration, and are lightweight - a single motor should work great for you.  Even heavier riders like me can do fine on single - just don't expect to go up steep hills.

Sounds like a good setup.

A note on motor kv...  depending on the voltage (# in series 3s, 6s, etc.) - try to stay below 10s on 190kv or you can have issues with VESC ERPM exceeding 60k (which can/will kill the DRV chip).

If you want to run your two 6s in series for 12s - you'd want the 149 or 170kv motors.

If you have an expectation of speed or hills - it would be good to know your weight and gearing to make sure you are setup correctly.  Have you looked at a speed calculator yet?

Not to knock what you have, but 10c batteries are going to SAG - a lot.  So when in use you will get less range.  Those are giving you a "claimed" output of only 52 Amps (in parallel 104A).  I typically would say 100A is my personal minimum - given it's marketing and likely not able to actually provide the full "C" rating they claim.  The higher the actual output capability - the less they will sag when being used more heavily.

To illustrate in case you aren't familiar with "Sag":
[img]http://marsen.com.au/assets/Uploads/Samsung-25R-discharge-curve2.png[/img]
This shows the affect on increased demand in amps from a battery (these are the venerable 18650 25R's) - the more you ask, the less mAh/Ah you get from them, and the more they sag to a lower voltage from the demand.  Plus more heat - which shortens pack life.

HTH - GL!
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2017-03-08T01:56:47.607Z Reads: 40

```
VESC dont come with power switches like car escs ... would be nice though....but anti-spark xt90 or some type of vedder anti spark switch..... or live with the POP when you connect them
```

---
## \#9 Posted by: caustin Posted at: 2017-03-08T02:05:29.214Z Reads: 38

```
No!

10 char
```

---
## \#10 Posted by: Michaelinvegas Posted at: 2017-03-08T02:10:31.654Z Reads: 37

```
[quote="caustin, post:5, topic:18718, full:true"]
Yes!

10 char
[/quote]


[quote="caustin, post:9, topic:18718, full:true"]
No!

10 char
[/quote]

LOL...Mr.Direct and to the point today
```

---
## \#11 Posted by: caustin Posted at: 2017-03-08T03:24:45.263Z Reads: 34

```
Yes!

10 char
```

---
