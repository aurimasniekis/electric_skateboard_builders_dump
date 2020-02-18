# Clarification Questions about E-Board Electronics and Mechanics

### Replies: 16 Views: 1267

## \#1 Posted by: HakuG Posted at: 2016-05-28T09:40:47.190Z Reads: 85

```
Hi everyone,

**First Post!** I've been stalking this forum for a long time now and I have to say the community here is amazing. I was kinda curious as to how to make an e-board, but after hearing your discussions, I'm now 100% sure that a DIY e-board is what I want to make for my 21st birthday. I did have a few questions though, which I hope some people can help me out with.

**A Few Assumptions**
So the way I understand it, there are a few ways to increase speed at the expense of torque:
_Lower kv motor_
_Larger Wheel_
_Smaller gear ratio_

These are all capped by certain physical limitations:
_Weight of the user + board_
_Grade of terrain_
_Voltage of Battery_
_ERPM limit of the ESC_

**Are those assumptions correct?**

So let's imagine a scenario where a 75kg user is using it to go to class, where the maximum hill incline he has is 16 feet over .1m (fairly little). There's high peopling traffic on the sidewalks, so the user has to basically use the road, where the speed limit is around 25mph. Using the VESC calculations [here](http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125) and the speed [calculator](http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html?m=1), the user has estimated that he should use a 8S LiPo battery cell with a 245 kv Motor, with a wheel size of 90mm and a gear ratio of 15/36. 

Besides the fact that I like to frame questions about myself in 3rd person, **are there any problems with that conclusion?** Do I need to account for more torque? If I do, where is the best place to add that torque? Should I change to a 10S and get a smaller kv motor? Or should I go with a smaller wheel, like 83mm? Maybe increase the gear ratio? 

**Basic Building Questions**

I've been reading a lot of Instructables to figure out how to add the motor mount. I've decided against using torquebuilds because I'm just getting into engineering and I'm honestly more excited to learn about the process of building an e-board than an e-board itself. I had a few questions:

**1. Why do people like the wheels with holes in them like [here](http://www.amazon.com/dp/B00I1WDZ7Y/ref=twister_B00IAGNVEI?_encoding=UTF8&psc=1)? Doesn't it make sense to have a solid center such that when you drill holes to affix your pulley system, it's more rigid?** 

**2. How important is the center distance between the wheel and the motor and what's the tradeoff? I'm also a little confused as to why it's so important to have a motor mount that has adjustable bolts? Once I've built it, why do I need to adjust it?**

**3. I plan on using a motor mount that is fastened to the trucks like in [this video](https://www.youtube.com/watch?time_continue=317&v=N83c8PjmLcw). Are there better ways of fastening them to the trucks that doesn't involve welding or buying a kit?**

Wow that's a lot of questions. I know you all are super busy building your own epic boards, but I would really appreciate your help. It would help me figure this out and allow me to order parts asap.

Thanks,
Haku
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-05-28T09:49:17.804Z Reads: 79

```
[quote="HakuG, post:1, topic:3932"]
1. Why do people like the wheels with holes in them like here? Doesn't it make sense to have a solid center such that when you drill holes to affix your pulley system, it's more rigid?
[/quote]

The trick here is that if there are holes alreasy, there is no need to drill, it is a slide-fit.
```

---
## \#3 Posted by: lox897 Posted at: 2016-05-28T09:49:58.017Z Reads: 74

```
> Lower kv motor: If you keep the battery at the same voltage and get a lower kv motor, that will give you more torque and less speed.
> Larger Wheel: This will increase speed (Not sure if it decreases torque)
> Smaller gear ratio: If you keep the wheel pulley at 36 teeth (example) and change the motor pulley from 14 to 15 teeth you will get a higher speed.

Pretty sure all of this is correct. If somebody thinks it is wrong then please say.
```

---
## \#4 Posted by: HakuG Posted at: 2016-05-28T09:56:21.481Z Reads: 70

```
[quote="lox897, post:3, topic:3932, full:true"]
> Lower kv motor: If you keep the battery at the same voltage and get a lower kv motor, that will give you more torque and less speed.
> Larger Wheel: This will increase speed (Not sure if it decreases torque)
> Smaller gear ratio: If you keep the wheel pulley at 36 teeth (example) and change the motor pulley from 14 to 15 teeth you will get a higher speed.

Pretty sure all of this is correct. If somebody thinks it is wrong then please say.
[/quote]

What are the drawbacks of a higher Voltage battery source then? Is it just bigger and heavier and more capable of handling higher torque?

[quote="flatsp0t, post:3, topic:3932, full:false"]

The trick here is that if there are holes alreasy, there is no need to drill, it is a slide-fit
[/quote]

Hmm. Does that mean that when I'm figuring out the dimensions of the screws that go into those 6 holes, I have to choose ones big enough to completely fill up the holes given? 

Thank you guys for your responses!!!
```

---
## \#5 Posted by: lox897 Posted at: 2016-05-28T09:58:56.115Z Reads: 62

```
[quote="HakuG, post:4, topic:3932"]
What are the drawbacks of a higher Voltage battery source then? Is it just bigger and heavier and more capable of handling higher torque?
[/quote]

Good things about higher voltage:
Less current having to go to the motors.

Bad things:
Depending on battery, it could be taller and longer. Most people fit it easily on their boards.
```

---
## \#6 Posted by: lox897 Posted at: 2016-05-28T09:59:56.515Z Reads: 57

```
[quote="HakuG, post:1, topic:3932"]
3. I plan on using a motor mount that is fastened to the trucks like in this video. Are there better ways of fastening them to the trucks that doesn't involve welding or buying a kit?
[/quote]

Clamps that use bolts.
```

---
## \#7 Posted by: flatsp0t Posted at: 2016-05-28T10:34:54.751Z Reads: 54

```
[quote="HakuG, post:4, topic:3932"]
Hmm. Does that mean that when I'm figuring out the dimensions of the screws that go into those 6 holes, I have to choose ones big enough to completely fill up the holes given?
[/quote]

Yes, or buy pulleys for the type of wheels you like:

Otang kegels:
product/36t-kegel-drive-wheel-pulley/

Flywheels and flywheel clones (the picture you pasted):
http://www.enertionboards.com/buy-build-your-own-electric-skateboard-parts/enertion-drive-36t-HTD-eboard-wheel-hub/
(beware you need to modify your trucks for these)

or
product/36t-abec11-drive-wheel-pulley/
without modding truck
```

---
## \#8 Posted by: delta_19 Posted at: 2016-05-28T21:51:03.716Z Reads: 32

```
[quote="HakuG, post:1, topic:3932"]
A Few AssumptionsSo the way I understand it, there are a few ways to increase speed at the expense of torque:Lower kv motorLarger WheelSmaller gear ratio
[/quote]

i think you mean higher kv motor
```

---
## \#9 Posted by: Hummie Posted at: 2016-05-28T22:36:42.342Z Reads: 32

```
Change motor pulley to bigger gets you more torque less speed

Bigger wheel more speed less torque
```

---
## \#10 Posted by: delta_19 Posted at: 2016-05-28T23:07:41.761Z Reads: 30

```
the wheel is right but if you go to a 15T motor pulley you get less torque then if you had a 12T
http://www.engr.ncsu.edu/mes/media/pdf/gears
```

---
## \#11 Posted by: Hummie Posted at: 2016-05-28T23:16:11.035Z Reads: 28

```
Yea sorry Dudududud
```

---
## \#12 Posted by: delta_19 Posted at: 2016-05-28T23:22:21.563Z Reads: 29

```
for a minute there i was like holy fuck brah.
```

---
## \#13 Posted by: Hummie Posted at: 2016-05-28T23:29:43.461Z Reads: 29

```
I try to distance myself from pulleys.  Complicated enough. Brah?  Thought u were English or euro
```

---
## \#14 Posted by: delta_19 Posted at: 2016-05-28T23:34:52.310Z Reads: 29

```
https://www.google.ca/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=brah
```

---
## \#15 Posted by: Hummie Posted at: 2016-05-28T23:38:34.779Z Reads: 27

```
Didn't think they said that in England.  Maybe you aren't in England.  Don't know why I assume ur euro.


Aha. You're in Canada.  Don't you have your own similar expression.
```

---
## \#16 Posted by: delta_19 Posted at: 2016-05-29T00:27:43.176Z Reads: 27

```
most us slag is used in canada.
```

---
