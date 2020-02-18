# What kind of amperage should I expect to pull?

### Replies: 16 Views: 3251

## \#1 Posted by: NickTheDude Posted at: 2016-10-03T07:48:51.232Z Reads: 314

```
Hey guys, I was just wondering if anyone has an idea of what kind of amps I would be pulling with an 8S setup with 36/16 gearing and 90mm wheels with dual 230kV motors. I'm trying to figure out what discharge rate I should be aiming for when building a li-ion pack. Thanks.
```

---
## \#2 Posted by: susplus Posted at: 2016-10-03T08:24:04.015Z Reads: 312

```
it will depend on: if you plan to connect both motors to the same battery or not....
```

---
## \#3 Posted by: NickTheDude Posted at: 2016-10-03T08:40:09.365Z Reads: 307

```
Wouldn't a 8s4p pack connected to two motors have the same draw from each motor as 2 separate 8s2p packs?
```

---
## \#4 Posted by: susplus Posted at: 2016-10-03T08:59:07.167Z Reads: 296

```
well it would be better for the batteries to separate them. 
I do no know how much 2x230kv motors will pull from the battery :( but if you build separate batteries for each motor then it is highly probable that the LG or Samsung batteries will do just fine
```

---
## \#5 Posted by: Namasaki Posted at: 2016-10-03T11:51:11.348Z Reads: 270

```
Build one battery and connect 2 controllers in parallel to the battery. Then each controller to a motor. 
You should do 10s and use Vesc controllers. 
It's the magic setup. 
Higher voltage=less amps. 
With the Vesc, you control amps from the battery to the motor.
```

---
## \#6 Posted by: NickTheDude Posted at: 2016-10-03T12:43:34.079Z Reads: 255

```
The goal for my build is 40km/h so 10S is not really necessary. What I'm really asking is whether my setup would overheat a VESC. From what I understand the upper limit for the VESC is around 50A. With dual motors do you think I would ever hit that limit? Are amps halved with dual motors or is there some loss somewhere in the system?
```

---
## \#7 Posted by: Randyc1 Posted at: 2016-10-03T13:20:59.859Z Reads: 237

```
Which motors are you using ?
```

---
## \#8 Posted by: NickTheDude Posted at: 2016-10-03T13:34:30.707Z Reads: 223

```
Maytech 230kV motors, part number MTO6355-230-NH.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-10-03T14:25:41.339Z Reads: 218

```
Amps should be half per motor with dual motors because the load is divided between the two motors
```

---
## \#10 Posted by: rpn314 Posted at: 2016-10-03T14:48:34.070Z Reads: 221

```
I've got a similar setup (10s Dual 230kv 16/36 gearing, 83mm wheels), and I set the battery limit on my VESCs to 40 amps total (20 each).

Before I set those (and erpm) limits, I had hit 60 amps total, but I was doing very quick acceleration from 0 to 30 mph (almost 50 km/h). So with my current limits, I think I hit my erpm before I hit my current limit unless I'm climbing hills. 

I built a 10s4p pack with Samsung 25Rs, so I can get 80A total discharge, so the lower limits are by my choice to put less stress on the batteries
```

---
## \#11 Posted by: NickTheDude Posted at: 2016-10-03T16:20:29.979Z Reads: 212

```
Awesome, thanks for the info. So right now I'm trying to decide which cells to pick, I'd like to use Panasonic NCR18650B's since they have a really good cost/Wh. However in a 8s4p configuration the packs discharge rate would only be 27.2A, it seems like this wouldn't be enough. A 8s4p Panasonic NCR18650GA pack would have a 40A discharge rate, I feel like this could be enough for dual motors. That being said, I haven't been able to find too much data on amp draw, so to be on the safe side it might be a good idea to use a 8s4p LG HE2 pack with a discharge of 80A. I'd like to choose the lowest discharge rate I can since it optimizes size/Wh and in the case of these batteries the lower discharge ones have a lower cost/Wh as well. What do you guys think?
```

---
## \#12 Posted by: Pedrodemio Posted at: 2016-10-03T17:02:39.029Z Reads: 196

```
From experience, don't use the NCR B, on paper it looks amazing, but in real life no so much, the internal resistance is too high 110mohms, so a lot of energy is lost in heating up the battery, in theory you have 350 Wh in a 10S3P battery , the maximum I manage to get is around 270Wh, with a cell with lower energy capacity but lower internal resistance I probably could get more energy out

Another factor is stressing the battery, since it heats up more, I will degrade faster

They would be amazing on a large parallel configuration, 7P or more

The loss of performance is a serious problem too, the voltage sag a lot, so you hit the cut off sooner, and even before this happens, around 36V you can already feel that the board is significantly  weaker

The NCR Ga is a good choice, the ir is 40mohms, I will try them soon, just waiting them to arrive

And interesting comparation:

Scenario 1: NCR18650B - 10S3P 41V (fully charged) 370 mohms IR - 20A draw

<img src="/uploads/db1493/original/3X/9/3/93e88b25f641cd7acb8e80a4816c1df23d286ce5.PNG" width="393" height="500">

Scenario 2: NCR18650GA - 10S3P 33V (almost no charge) 133mohms IR 20A draw

<img src="/uploads/db1493/original/3X/7/5/75782a21b4b1acf57426e613cd41797a6742c658.PNG" width="451" height="500">

As you can see, on scenario 2 we have almost the same power on a fully discharged battery than with a fully charged one

And as a mentioned, the sag is brutal on the NCR B, a little bit of discharge and the voltage will start to hit the battery cutoff and the power will be reduced (using VESC progressive cut off)

The GA does not have the amp draw of the samsung 30Q or LG HG2, but the IR is almost the same
```

---
## \#13 Posted by: NickTheDude Posted at: 2016-10-03T20:14:18.990Z Reads: 153

```
Awesome, thanks for letting me know. Honestly I had no idea about internal resistance. Looks like NCR18650GA's are the cells to go for the Wh I had in mind. Thanks!
```

---
## \#14 Posted by: Okami Posted at: 2016-10-04T08:08:37.745Z Reads: 151

```
Writing from phone so will try to keep it short.

Hi threre, nice to see another li ion enthusiast!

I faced the same problem as you - there's too little data on what amp draw to expect and how much extra 'margin' should be left in terms of max discharge the battery can handle. 

A little bit hard to figure out where the compromise between high capacity and high discharge is so that neither of them lacks, especially when taking into account the cost and size of the battery pack, too.

Anyways, my conclusion was that it is wise to design a battery pack where your board's max cont discharge is 2/3 or even maybe 1/2 of what is said to be the max cont rating of your batteries.

So that would translate to around 60A battery pack if you were going to use 40A. Although, more accurate would be to just take a look at the battery's datasheet and see how much the capacity declines if the battery is drained at specific constant voltage.(matter of parallel battery count, too)

Actually would be great to contact @chaka and / or @barajabali since both of them should (seems to) be more knowing  in this matter.

--

On an end note, I think this is now an offical "eskateboard li-on packbuilders problem" - not knowing the exact power requirements for riding a board / building a powerful enough battery.

Some folks just take the the max his motor can take (~60A ) and build using that. Although I liked the idea to pick the number at what wattage it is most likely the board be ridden at (Also not much data, just speculation). Hard to guess if you have to take into account acceleration and hill climbing (if you have them)
```

---
## \#15 Posted by: Okami Posted at: 2016-10-04T18:32:18.970Z Reads: 127

```
Related to this subject, here is quite lenghty discussion where a lot of good ideas can be found:

http://www.electric-skateboard.builders/t/choosing-18650-cells/6240/25

Other than that.. all I can tell you know is that typical usage would yield around ~300-400w consumtion.

From that you can try to conclude what would be the power requirements.
```

---
## \#16 Posted by: daym10 Posted at: 2018-07-31T19:59:43.252Z Reads: 53

```
Has anyone answered the actual question of the range of amperage you should expect to pull say on a flat surface (best case scenario) or going up a hill (worst case scenario)?
```

---
