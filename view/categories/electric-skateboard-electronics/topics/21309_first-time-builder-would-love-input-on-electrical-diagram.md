# First time builder! Would love input on Electrical Diagram!

### Replies: 19 Views: 1260

## \#1 Posted by: Challlsss Posted at: 2017-04-18T18:54:41.084Z Reads: 142

```
Hi everyone! I am new to the forum and am exited to become part of the e-skate community :slight_smile:  I just bought "all" (I hope) of the stuff I need to make my first electric longboard! For my first post I am curious if my electrical diagram looks good. :slight_smile: The yellow diamonds will be XT90 connectors. 
<img src="/uploads/db1493/original/3X/9/e/9e1ffac27fef8cfa2d194959a591abb16c17af9d.png" width="441" height="500">
```

---
## \#2 Posted by: SimosMCmuffin Posted at: 2017-04-18T19:03:15.069Z Reads: 131

```
You plan on charging the pack as a single 6S battery, based on your balance connector?

Just a nitpick, but I would put the XT90 loop key on the positive lead rather than cutting the ground. 

Is the loop key XT90 an anti-spark variety? Otherwise if it's a normal one you might get a little zap sound everytime you connect it, because you get a big current rush to the VESC's capacitors and it will slowly eat away the connector.

EDIT:  Overall, good and clean connection diagram.
```

---
## \#3 Posted by: Challlsss Posted at: 2017-04-18T19:06:34.864Z Reads: 125

```
- Yes I intend to charge as 6S so that I can have the charger female end sticking out of the side for easy access.

- What benefit would putting the loop key on the positive end have? Just wondering

- Yes the XT90 is anti-spark (it has the green L on it)

EDIT: I also was thinking it would be necessary for the XT90 to the battery charger to be anti-spark... Is that correct?
```

---
## \#5 Posted by: SimosMCmuffin Posted at: 2017-04-18T19:14:52.255Z Reads: 112

```
In this case I don't see any problems coming from using the loop key on the ground side, but was rather just my personal opinion coming from electronics.

It wouldn't hurt having the charging XT90 be also an anti-spark, as the charger will also have output capacitors, which will charge up upon connection.
```

---
## \#6 Posted by: Challlsss Posted at: 2017-04-18T19:16:46.544Z Reads: 102

```
Sure. Thanks for the reply :slight_smile:

Any chance you have thoughts on the current battery and motor config? I was thinking about adding a third battery but am not sure.
```

---
## \#7 Posted by: SimosMCmuffin Posted at: 2017-04-18T19:17:56.282Z Reads: 95

```
What diameter tires and gear ratios are you planning on using?

Here's my board http://imgur.com/a/Mjodj
```

---
## \#8 Posted by: Challlsss Posted at: 2017-04-18T19:21:56.342Z Reads: 90

```
90mm Wheels - 35 teeth
Motor - 14 teeth
(I believe these are correct, I just got them from enertion)
```

---
## \#9 Posted by: SimosMCmuffin Posted at: 2017-04-18T19:32:56.317Z Reads: 88

```
Mine configuration is:
80 mm wheels - 15:30 gear ratio - SK3 149KV - 6S4P battery (22.2 V, 12 Ah, 266 Wh) - average flat ground travel speed ~24 km/h (~15 mph) - Range at top speed ~24 km

Your configuration:
90 mm wheels - 14:35 gear ratio - SK3 260KV - 6S1P battery (22.2 V, 5 Ah, 111 Wh) - I'll predict a flat speed around 30-35 km/h and not  a lot of range at that speed <5 miles. But as noted these are predictions and you should do some benchmark runs to test your setup's speed and energy consumption / distance depending on your speed.
```

---
## \#10 Posted by: Challlsss Posted at: 2017-04-18T19:42:28.434Z Reads: 82

```
Once I've got it all assembled I definitely update and show statistics.

One thing I am confused about it the Amperage. Since the battery is 20c (30c burst) shouldn't the "Max" current be closer to 100 amps? The motor maxes out at 70 so I'd probably run at closer to 50 amps.

Or am I just way off?
```

---
## \#11 Posted by: SimosMCmuffin Posted at: 2017-04-18T19:49:37.648Z Reads: 75

```
We'll if you're pulling 50 amps from the battery, you are using 50 A * 22.2 V = 1100 Watts of power and really you won't be pulling that high amount of current from the battery unless you're accelerating pretty hard or going up a steep hill. I'd estimate you to run at max flat speed at about ~600 Watts continuous, which then it comes to 600 W / 22.2 V = 27 Amps continuous.

The simple way to test if you're pulling too much current from the battery is to see if it heats up. So ride around some and put some load on it and then stop, open your enclosure and touch the battery and feel if it has warmed up.
```

---
## \#12 Posted by: SimosMCmuffin Posted at: 2017-04-18T19:51:43.454Z Reads: 72

```
Also, I'd like to just point out I base these calculations on my own test results shown here:
https://www.electric-skateboard.builders/t/speed-vs-range-practical-test-results/21015
```

---
## \#13 Posted by: Challlsss Posted at: 2017-04-18T20:43:57.540Z Reads: 67

```
Makes sense. I will try that
```

---
## \#14 Posted by: whatthejess Posted at: 2017-04-18T21:44:04.797Z Reads: 66

```
I have the exact power setup. but you should use one plug for charge and balancing like the computer monitor type I have used. Also put a voltage meter after the loop key. <img src="/uploads/db1493/original/3X/d/6/d675d4e02332d5521d7b843775da8d3a60b4a741.jpg" width="666" height="499">
```

---
## \#15 Posted by: Fabian287 Posted at: 2017-04-18T22:22:23.787Z Reads: 61

```
electrons are flowing from negative to positive ^^
```

---
## \#16 Posted by: rpn314 Posted at: 2017-04-19T01:50:44.389Z Reads: 56

```
[quote="whatthejess, post:14, topic:21309, full:true"]
I have the exact power setup. but you should use one plug for charge and balancing like the computer monitor type I have used. Also put a voltage meter after the loop key. 
20170322_202929.jpg826x620 85.6 KB
[/quote]

That would be a good option for an all in one plug when using an external balance charger. You're other option is to get a BMS and just have a single 6s charger input. If you don't already have one or the other.
```

---
## \#17 Posted by: Challlsss Posted at: 2017-04-19T19:21:35.259Z Reads: 50

```
Thanks for all the replies!

I just got out of my reply limit (since this was my first day posting and they cut me off haha)

So here's a few questions:

- Do you know where I could find a build that explains how to set up the one part plug for charging? I don't fully understand how it works.

- Curious what a BMS is @rpn314 

- What voltmeter did you use?
```

---
## \#18 Posted by: rpn314 Posted at: 2017-04-19T19:50:55.484Z Reads: 51

```
[quote="Challlsss, post:17, topic:21309"]
Curious what a BMS is @rpn314
[/quote]

Battery Management System. At the very least it does the job of the balance charger, so the balance leads are plugged into that and then you just provide it with the power supply (like a standard barrel plug at the right voltage). Most will also provide over current protection so you don't draw too much from your battery pack and even a soft switch circuit built in so you don't need any anti-spark loop or something.
```

---
## \#19 Posted by: whatthejess Posted at: 2017-04-22T18:13:54.844Z Reads: 39

```
<img src="/uploads/db1493/original/3X/9/f/9f2cd2188c6419eebc1ab91ed48f76e661fc0970.jpg" width="374" height="500">

I'll look for a diagram Also. But here is the basic idea
```

---
## \#20 Posted by: Challlsss Posted at: 2017-05-03T13:21:37.661Z Reads: 31

```
Update* I tried charging the way my diagram was.... and my charger started smoking, it said that it only detected 5 cells instead of 6. Sooooo I added the fourth black wire to the balance connector, soldering the orange/red wire and the new black wire together and it worked as expected.
```

---
