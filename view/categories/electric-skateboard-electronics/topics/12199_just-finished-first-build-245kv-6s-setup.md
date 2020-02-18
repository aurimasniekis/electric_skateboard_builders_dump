# Just finished first build 245kv - 6s setup

### Replies: 7 Views: 521

## \#1 Posted by: maker7 Posted at: 2016-10-31T14:40:43.490Z Reads: 89

```
I just finished (except for permanent electrical component mounting.)  As soon as I was comfortable with my VESC settings, I temporarily affixed the components to the underside and gave it a try.  My question is this:  Should I have to push off to get started or should I be able to start with both feet on board?  I weigh 165lb and and have a VESC controlled Turnigy 245kv 6s setup.

Thanks!
```

---
## \#2 Posted by: mattdig Posted at: 2016-10-31T14:44:02.402Z Reads: 88

```
What is your gearing and what is your wheel size?
```

---
## \#3 Posted by: maker7 Posted at: 2016-10-31T14:50:02.904Z Reads: 84

```
Oh yeah that would help right? 36t wheel pulley/15t motor pulley, 83mm wheels.  Could it be a belt tension issue?  or a VESC config issue?
```

---
## \#4 Posted by: mattdig Posted at: 2016-10-31T15:00:05.352Z Reads: 79

```
You definitely shouldn't have to push to start, your setup should have a plenty of torque. I'm way up at 17:36, on 90mm wheels, similar weight, and I don't have to push to start (but I always do out of habit). Does it not have any power at all from 0rpm or does it just cog a whole lot?
```

---
## \#5 Posted by: maker7 Posted at: 2016-10-31T15:02:33.026Z Reads: 77

```
Seems to have a lot of power and yeah it is cogging a bit.
```

---
## \#6 Posted by: TarzanHBK Posted at: 2016-10-31T15:03:54.334Z Reads: 77

```
if you are running a sensorless motor (your turnigy) you´re not able to start spinning it without a little bit of movement, because your motor has no orientation to the magnets. If you try it, the motor will stutter. If you have a tiny bit of movement and your motor gets the orientation it will start.

if you are running a motor with sensors, you´re able to start from a standstill, because the hall sensors know where the magnets are and the motor starts in the right direction.

It´s always recommended to start pushing a bit - saves a lot of energy and won´t toss you off the board because of stuttering
```

---
## \#7 Posted by: maker7 Posted at: 2016-10-31T15:07:49.164Z Reads: 72

```
Cool!  I thought I messed something up.  Thanks for the info!
```

---
