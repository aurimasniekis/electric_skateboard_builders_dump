# Looking for Good Tutorial on Power Train Math

### Replies: 4 Views: 392

## \#1 Posted by: mfidelman1 Posted at: 2017-05-22T02:40:28.163Z Reads: 65

```
It occurs to me that the FAQ points to lots of information on how to design a drive train (gear ratios, etc.) - but nothing on the power train.

So... I wonder if anybody has a good writeup or video that works through the entire math from:
Basic Operating Characteristics (speed range, load, inclines, operating range, etc.) ->
Specifying/picking a motor (KV, power, etc.) ->
Specing & Configuring an ESC/VESC ->
Specing a battery pack (S, P, C, Capacity)

Bonus points for how this all interacts with drag, gearing, and torque/power curves for motors.  Even more bonus points for electronic braking/recharging.

Specific case in point:  I'm working on an "electric walker" (i.e., adding motors to my dad's walker).  Ideally, I'm looking at using dual hub motors, with tank steering (to stay away from the maintenance headaches of a belt drive system, and maybe look at very small wheels before a gear/belt system).  Looking to achieve avg. speed of 3mph, top speed of 4mph, a range of maybe 4 miles (1 hour).  Assume a 180 pound rider, smooth level ground.  

So I'm trying to work through everything from peak/average power required from the motor(s) to motor ratings to VESC rating/specs to battery specs.  

And, as a separate exercise, holding the load constant, examine the implications of different motor specs & gearing on the power system specs.

So... anybody have a pointer to a good tutorial, video, or book that works through the step-by-step design process from an engineering point of view?  Or maybe somebody who'd be willing to spend some time working with me to put together such a writeup?  (I'm an engineer by training, but more electronics/computers/network stuff - mechanical and motor stuff is new ground, and I'm not familiar with either the math, or the practicalities of available components.)

Thanks!
```

---
## \#2 Posted by: Titoxd10001 Posted at: 2017-05-22T03:22:14.765Z Reads: 52

```
It seems a little complicated to gather all that information to build something that goes under 5mph. I don't think any of us have done. If I were you I would go chain drive or belt drive for gear reduction which means more torque. Hub motors have less torque (per size stator). If you don't want to spend a lot of coin you can even get a 12v-24v brushed motor like ones that come with scooters. They actually have good torque down in the rpms and they're dirt cheap. You could possibly even use the thumb throttle that they come with, not sure how you'd limit speed maybe less voltage. If you're going with vesc maybe a sensored+lowest kv brushless motor you can find. And batteries, the slower you go the less power you use so getting an hour of runtime going 5mph is nothing. 

We're building boards that go 30mph so maybe it's a little difficult for us to explain how to build something that goes 5mph, no offense. Do you have a pic of the type of walker you're talking about
```

---
## \#3 Posted by: mfidelman1 Posted at: 2017-05-22T03:52:44.368Z Reads: 47

```
 https://www.youtube.com/watch?v=1FSWf8vG0kI&t=18s333 at around 1:34
```

---
## \#4 Posted by: Titoxd10001 Posted at: 2017-05-22T04:58:03.306Z Reads: 41

```
Here's what I think will work 
Brushed 12-24v (simple, thumb throttle, good torque from 0)
Brushless preferably sensored
Dual hub motors sensored (you need two esc)

Things I would not worry about are range since in your scenerio your going 5miles. I would not worry about belt maintenance because you you're not braking from 30mph. 

The challenging part would​ probably be mounting a board that pivots that has skateboard trucks attached?

I'm not an expert, just​ trying to help. I would say just go for it, don't think about it to much, modify it later if needed
```

---
