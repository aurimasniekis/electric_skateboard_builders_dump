# 6S upgrade to dual drive, decision point time

### Replies: 5 Views: 175

## \#1 Posted by: Makkaman Posted at: 2019-01-04T02:22:40.432Z Reads: 67

```
My current build is a 6S2P DIY pack, VESC, DIY 6355 260kV geared at 14/36T. I recently moved from the flats to the hills and feel like Im pushing my board too hard. Looking to up my torque and alleviate some stress on my single drive build. Also worth noting that I have four 3S 5000mA lipos at my disposal.

Im trying to decide whether to add a second 6355 260kV motor and keep the board at 6s or buy two lower kV motors and wire my lipos in 12S. Id rather keep the build 6s but wonder if i risk any long-term wear running 260kV motors so hot on hills. Cost will be a major deciding factor.

Please advise. Id love to hear feedback from other dual drive 6s riders.
```

---
## \#2 Posted by: monsterbuilder Posted at: 2019-01-04T03:33:48.782Z Reads: 62

```
I'm far from being an expert... so don't take my advice too seriously. I can 100% relate to your dilemna.  I've been running a single motor TB 260kv on a 20c 14,000mah lipo geared at 15/36 on 97mm wheels for the 6 months.  I've been pretty happy with my set up.  It easily gets up to 25mph and 18-20 miles of range on a single charge.

I wanted to rebuild my board over the winter but my fun money budget is extremely tight.  I spent a few months thinking through the most logical and economical upgrade.  I watched for Christmas deals and snagged a brand new TB 190kv motor for $60.  Because of that purchase, I would ideally like to make the leap to a 10s set up sometime in the next few months after I've saved up a bit more.

Here are my thoughts:
* 190kv motor on 10s is going to run cooler than a 260kv motor on 6s.  My motor would get pretty hot to the touch if I rode in temperatures above 90'
* 10s is going to stress your VESC a lot less than 12s
* Dual motor set ups are less efficient due to extra drag in the drive train
* Dual motors are also more expensive and require more maintenance.  Now you are paying for an extra VESC, motor, pulleys and belts.
* i don't think dual motors are required unless you are not satisfied with the acceleration or braking power

Just my thoughts... keep in mind that my opinion is mostly based on the most budget friendly way to approach this.  I hope this helps.
```

---
## \#3 Posted by: linsus Posted at: 2019-01-04T11:33:56.329Z Reads: 38

```
cheap/older VESC= dont go for 12S

6S is incredibly insufficient tho. 10S will decrease the temp in your motors. Current leads to heat. Higher voltage yeilds lower current draw.
```

---
## \#4 Posted by: Makkaman Posted at: 2019-01-06T19:16:21.255Z Reads: 25

```
Thanks for the tips! To keep costs low and future proof my gear list, I begrudgingly made the commitment to another 260kV motor. I'm using VESCs from DIY Electric Skateboard. Albeit not the newest hardware, I believe they're solid builds (im no expert). Now just to solve my lack of range...

Thanks for pointing out the voltage vs current heat trade-off. I had forgotten this in all of my brainstorming. I think Im thinking on harvesting one of these VESCs for a second, 10-12S build in the future and pair up with a larger single-drive motor.

Any feedback regarding hill climbing with a larger single drive vs dual drive? I have no experience with motors larger than 6355 but think that'll be my next endeavor. I'm sure its been discussed before, so feel free to link away if its easier than typing out your own thoughts. Any info is appreciated!
```

---
## \#5 Posted by: mmaner Posted at: 2019-01-07T01:14:48.678Z Reads: 19

```
Hill climbing is all about torque. Torque delivery is optimized by gearing and the amount of amps the ESC can pull. 

Larger wheel pulleys give more torque but less speed, smaller wheel pulleys give more speed but less torque. Larger motor pulleys give more speed, smaller gives more torque. 

I don't know what battery your running but parallel groups till allow you to discharge more amps. 

All that being said, at 6s the best you can expect is mediocre hill climbing performance. At 10s with 4 or more parallel groups you can accelerate up most hills.
```

---
