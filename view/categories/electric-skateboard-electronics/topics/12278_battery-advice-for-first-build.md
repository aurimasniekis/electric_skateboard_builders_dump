# Battery advice for first build

### Replies: 39 Views: 3875

## \#1 Posted by: Freddiecook Posted at: 2016-11-01T20:10:23.573Z Reads: 268

```
Hi, firstly, I am new to all of this so bare with me 
Basically I want to build my first E-board and I have decided on an Alien 6374 Sensored Outrunner brushless motor 130KV 3200W
I would preferably like to make my own lithium-ion battery but to be honest I don't know what kind of voltage I need, how much capacity I need and if it would be too expensive, thank you
```

---
## \#2 Posted by: rpn314 Posted at: 2016-11-01T20:52:15.997Z Reads: 261

```
That seems like a little bit of a low KV for our purposes, but it'll probably work. I'd recommend a 10-12s battery (so that's 36-42V for 10s and 43.2V-50.4V for 12).
Keep reading around on here and you'll find a lot of your answers. Expensive is relative, so you'll have to figure out what kind of range you want, among other things (like which ESC you'll get), to really determine a price. Start with:


http://www.electric-skateboard.builders/t/start-here-faq-for-diy-electric-skateboard-builders/215?u=rpn314
http://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53?u=rpn314
http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983?u=rpn314

And if you're considering the VESC (which I personally would)
http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980?u=rpn314
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125?u=rpn314
```

---
## \#3 Posted by: Freddiecook Posted at: 2016-11-01T21:56:21.490Z Reads: 198

```
Thank you so much, if you're wondering this, is the motor
http://alienpowersystem.com/shop/brushless-motors/alien-6374-sensored-outrunner-brushless-motor-130kv-3200w/
And I will hopefully get a VESC 
thank you again
```

---
## \#4 Posted by: Freddiecook Posted at: 2016-11-02T22:28:39.729Z Reads: 174

```
Is that motor not very good for electric skateboards then? What could you recommend?
```

---
## \#5 Posted by: rpn314 Posted at: 2016-11-02T22:40:47.647Z Reads: 170

```
Correct. I would say in most applications, 130kv is too low. Read through "choosing the right motor kv for the vesc." It's not as simple as recommending a single motor. It's dependent on your battery choices and a little bit how you ride/want to ride.
```

---
## \#6 Posted by: Freddiecook Posted at: 2016-11-03T12:41:39.197Z Reads: 163

```
I've done a bit of reading and I've increased the KV of the motor to 270KV 
http://alienpowersystem.com/shop/brushless-motors/alien-5065-fr-sensored-outrunner-brushless-motor-270kv-2000w/
And initially I was going to base the voltage of the battery to whatever motor I get as I was going to try to build my own Li-ion battery. I've used an online calculator to find that I would need roughly 25V to go the speed I want of 30mph so I was going to put 7x 3.6V batteries in series then have 3 of these in parallel, I just wanted to check that this sounds okay, and if it makes any significance, this is the VESC I want to use as it is relatively cheap
http://alienpowersystem.com/shop/esc/ev-esc/vesc/
```

---
## \#7 Posted by: rpn314 Posted at: 2016-11-03T13:37:17.770Z Reads: 160

```
Great! Let's start with batteries. If i'm understanding what you wrote, you're looking at a 7s3p* pack paired with a 270kV. That combination should work fine. I wouldn't expect to climb any insane hills, but it'll get you around at a decent speed. Actually hitting 30 will be dependent on your gearing ratio, and that ratio will also effect your torque. If you haven't used it yet, I'd look at [this calculator](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":7,"motor-kv":270,"system-efficiency":75,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":83}|). With what you're telling me, I'd expect closer to 20 mph, not 30.

If you're going to do a single motor setup at 7s just be very wary of what Li-Ion cells you choose. A 7s setup will most likely draw a decent number of amps and Li-Ions don't put out as many amps per cell as Li-pos do. And be aware that they do usually cost more, but I think it's generally accept that they last longer (no guarantees, and definitely dependent on how well you take care of them). Also, how were you planning on building a battery pack?

Now about the VESC. I'm not familiar with alien power system's VESC, but looking at that link it just looks like they're just reselling two manufacturers that you can chose between. The "Flier Model" (which I've never heard of) and the Maytech. We've discussed Maytech here before, and I don't think we can give them a solid recommendation right now. To be honest, I would not go for a vesc because it's lower priced. I'd go for the most solid one you can, cause while it's extremely powerful and a fantastic piece of engineering, it's also very prone to breaking when less than top of the line components are used. @chaka has made the tried and true solid VESC for the longest, and you'll pay much more for it, but it'll last you. There's plenty others as well, but with the VESC, you definitely get what you pay for. I assembled my own (not for the faint of heart) and have had very few issues, but I was purchasing parts from US suppliers which generally have very good components. I don't know what kind of availability there is where you are (which looks like England?)

I hope I don't come across as just slashing down your ideas, it just takes a lot to get one of these things all built and functioning long term. I definitely over-engineered mine and I'm quite happy I did. Hope I'm actually being helpful.

*7 cells in series, 3 cells in parallel, for a total of 21 cells if you're not familiar with the s/p battery terminology. You'll see it a lot around here
```

---
## \#8 Posted by: Freddiecook Posted at: 2016-11-03T15:22:26.804Z Reads: 137

```
Of course you're not slashing down my ideas, any constructive criticism is very helpful and you're really helping.
Where I live there aren't any majorly big hills so I don't need to go over kill on the motor but I do want it to last me as long as possible really, I have read up on the chain and sprocket vs belt and pulley and have found a chain system which would suit me quite well (I think) with the motor sprocket having 15 teeth and the motor's sprocket having 32 teeth. Also I completely forgot about my weight when working the speed out, my bad (I weigh roughly 72 KG if that's significant in any way)

The reason which I don't really want to go down the Li-pos is because I don't want to constantly be monitoring them and after watching a few DIY Li-Ions videos (where people use the batteries from computer batteries) they been relatively cheap. With regards to building it I would just follow a guide online like this one 
https://www.youtube.com/watch?v=DJaToOJcZ_o

And with the VESCs I don't really know what is good and what is bad and living in England I have struggled to find ones which are highly recommended as shipping is usually £30+. I am up for spending the extra money for a more reliable VESC but I just don't know what to buy if I'm honest.
```

---
## \#9 Posted by: axelleboss Posted at: 2016-11-03T20:25:40.786Z Reads: 124

```
Why don t you use the 120a esc from APS?
```

---
## \#10 Posted by: Freddiecook Posted at: 2016-11-03T23:26:39.597Z Reads: 123

```
Have you had any experience with it? I only ask as on forums people really seem to think normal ESCs are nothing compared to the VESC
```

---
## \#11 Posted by: axelleboss Posted at: 2016-11-04T18:32:13.008Z Reads: 123

```
Well no but I ordered one because the Vesc seems to blow up as it is still work in progress. @Janis told me it worked great for him and he put 300km on it. Also check out this video: https://youtu.be/_NoZkS_mWY0
```

---
## \#12 Posted by: rpn314 Posted at: 2016-11-04T21:42:40.623Z Reads: 120

```
Anything with lithium has to be monitored. The laptop battery route is a ton of work, just a warning. It can be a little cheaper, but after taking apart the battery packs, and separated the individual cells, you have to test each one and then properly pair them so the pack is balanced (in this video he breezes past this part). And though this guy soldered them, it's a little tougher cause you have to be super careful to not overheat the batteries. Just fair warning.
```

---
## \#13 Posted by: Esrapp21 Posted at: 2016-11-06T13:26:49.939Z Reads: 118

```
I am about to build by first electric skateboard, and I am using 2x 6s 5000mah lipo batteries and a 130kv motor. Should I hook the batteries up in series so I get a 12s Battery with 44.4 volts but still 5000mah, or in parallel to get 10000mah but still 6s batteries with only 22.2 volts?
```

---
## \#14 Posted by: Freddiecook Posted at: 2016-11-06T14:20:02.448Z Reads: 110

```
I have a friend with a home made spot welder so I could use that instead of soldering and I'm willing to put the extra work in as I like to learn about this stuff and tinker around with the electronics, what kind of battery set up do you think would be good for an average user? And are the li-ion batteries safer? P.s sorry for the late responses
```

---
## \#15 Posted by: Freddiecook Posted at: 2016-11-06T14:22:48.605Z Reads: 108

```
I'll check it out when I get home :) when it arrives can you tell me how it performs?
```

---
## \#16 Posted by: axelleboss Posted at: 2016-11-07T18:58:02.945Z Reads: 103

```
Sure will! They just shipped it should arrive
 tomorrow.
```

---
## \#17 Posted by: Freddiecook Posted at: 2016-11-11T11:09:35.366Z Reads: 96

```
Any news about the new ESC?
```

---
## \#18 Posted by: axelleboss Posted at: 2016-11-11T12:28:08.211Z Reads: 99

```
Yes I just received it and am currently connecting/soldering everytging together...will tell you how it goes..
```

---
## \#19 Posted by: Freddiecook Posted at: 2016-11-12T19:17:04.382Z Reads: 93

```
I've been doing some more research and I was wondering, do you split the cells up into groups then balance the group or do you still balance each cell separately? I managed to buy 20 genuine samsung 18650s and was going to put them in 10s2p so I need to know how to hook these up to the bms. I know that I could balance each cell if I have 2 bms' and then switch between the two packs when I'm riding but I'd prefer to avoid this
```

---
## \#20 Posted by: rpn314 Posted at: 2016-11-12T19:41:29.387Z Reads: 91

```
Valid question. I definitely balance all of the parallel cells together. I use 1 bms on my 10s4p pack, so I have have 10 sets of 4 cells in parallel, all stacked on top of each other (that's what the diagram would look like, I actually have them physically laid out a little differently), so I just connected the BMS balance wires in between each set of 4 cells.
```

---
## \#21 Posted by: Freddiecook Posted at: 2016-11-12T20:06:17.710Z Reads: 86

```
So if I did 10 sets of 2 batteries do I put the balance wire in between the batteries? and could I stack them like they do in TV remotes?
```

---
## \#22 Posted by: rpn314 Posted at: 2016-11-12T20:18:06.023Z Reads: 85

```
Correct. This article will probably be very helpful for you. It's be referenced many times around here before.

http://www.ebikeschool.com/how-to-build-a-diy-electric-bicycle-lithium-battery-from-18650-cells/
```

---
## \#23 Posted by: Freddiecook Posted at: 2016-11-20T19:45:47.792Z Reads: 76

```
Anything yet on the esc? I'm really interested
```

---
## \#24 Posted by: axelleboss Posted at: 2016-11-21T19:41:53.245Z Reads: 67

```
I am waiting for the chain to be able to test under load but so far it has performed flawlessly(speed control, connecting it to the computer to change settings...)
Here is a link to the testing setup: https://goo.gl/photos/crLjisEReYtcvCp29
I ll let you know once I finish receiving parts and installing everything under the board.
```

---
## \#25 Posted by: kbazzy98 Posted at: 2016-12-06T22:46:27.632Z Reads: 58

```
I'm currently working on my on diy battery, you're absolutely right, it's a lot of work doing the laptop method(what im doing). I have all the battery sorted but I have not decided which way to put my batteries in because I don't know which way is the best. Also, if I I have a good laptop battery, could I just disassemble it and directly hook up the balance charge leads instead of disassembly and re- soldering?
```

---
## \#26 Posted by: Okami Posted at: 2016-12-07T10:57:09.632Z Reads: 59

```
Can you give a number about how much batteries you've already harvested?

Wel,, if all the cells are 100% good, I assume you could just desolder the pcb and keep the balance wires, as I think, they should be in the right order.. unless the bms requires opposite wiring.
```

---
## \#27 Posted by: Ackmaniac Posted at: 2016-12-07T11:14:30.070Z Reads: 61

```
How many cells you want to put in series and how many in parallel. I made a laptop battery which is working quite well. But you really need a lot of battery's. 
The best would be to put 12 in series and as many as you can fit in parallel when you stick to your laptop battery plan.
In minimum you have to go for 48 batteries 12S4P. But the power output would only be enough for a cruiser. Better would be 12S8P, then you have some decent power.
```

---
## \#28 Posted by: kbazzy98 Posted at: 2016-12-07T11:26:55.470Z Reads: 59

```
I probably have about 30 battery's harvested. I could acquire more, just ask local PC shops. They throw them away anyways so they might just give you them
```

---
## \#29 Posted by: kbazzy98 Posted at: 2016-12-07T11:29:40.959Z Reads: 60

```
I tried that with 2 battery packs but it didn't work, I must be doing something wrong.<img src="/uploads/db1493/original/3X/6/f/6f33100c7dcaa8e815621566c0bb52a822f41c1c.jpg" width="690" height="393">
```

---
## \#30 Posted by: kbazzy98 Posted at: 2016-12-07T11:31:20.818Z Reads: 55

```
It just gives me an error message on my iMax b6
```

---
## \#31 Posted by: Ackmaniac Posted at: 2016-12-07T11:31:54.592Z Reads: 53

```
Remove the Laptop BMS
```

---
## \#32 Posted by: kbazzy98 Posted at: 2016-12-07T11:32:43.915Z Reads: 55

```
By removing it, it's should work?
```

---
## \#33 Posted by: Ackmaniac Posted at: 2016-12-07T11:35:23.948Z Reads: 55

```
Wire the balance leads directly to the batterys. But then you need 5 wires. I recommend to watch some videos about building DIY battery packs and balancing battery's.
```

---
## \#34 Posted by: kbazzy98 Posted at: 2016-12-07T11:38:01.241Z Reads: 52

```
I've watched every video out there. How much batteries did it take your board to run how you'd like it.
```

---
## \#35 Posted by: Ackmaniac Posted at: 2016-12-07T11:41:23.796Z Reads: 53

```
I made it 12S8P = 96 cells.
```

---
## \#36 Posted by: Okami Posted at: 2016-12-07T12:29:53.886Z Reads: 54

```
You probably need a 5 wires for this battery. There seems to be 4 groups of 2cells in each group..

I dont remember anymore.. but you need to find a balance cable wiring diagram..

Basically, you connect the first wire to the negative terminal of the first battery, then you connect the rest of the cables to the positive side of each parallel group.. 

---
And yes, get rid of that bms circuit board.. It is probably not gonna let you access the battery directly. ( i think you can re-solder the red wire, as the rest of the wires seem to be soldered directly to the battery)

From the picture it looks like you still need to access the brown cable.. other than that, you should be able to use it after that.. you can find a 5pin connector and once everything is done check if balance charger recognizes the battery.
```

---
## \#37 Posted by: Ackmaniac Posted at: 2016-12-07T12:33:20.296Z Reads: 53

```
That is how you need to wire the power cables and the balance cables.

<img src="/uploads/db1493/original/3X/5/a/5a22420e0925da01553ef8c6562485fbe68787ee.jpg" width="640" height="480">
```

---
## \#38 Posted by: kbazzy98 Posted at: 2016-12-07T12:48:55.053Z Reads: 53

```
Yeah I've looked at this diagram before, it's pretty helpful. For my battery, I need one more wire, I'm just gonna order jst 4s from Amazon. In the picture is the jst 3s.
```

---
## \#39 Posted by: Ackmaniac Posted at: 2016-12-07T12:55:34.085Z Reads: 52

```
You got it. But i think you have to separate the cells anyway. Maybe you can leave the P packs together because they worked together during their entire lifespan so they also should act identical. And then you could charge all the cells in parallel (the 4 packs in parallel).
```

---
