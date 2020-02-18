# Building an Ride On Golf Buggy What Battery is Best?

### Replies: 17 Views: 1243

## \#1 Posted by: LikeByte Posted at: 2017-04-11T17:02:16.674Z Reads: 146

```
Hey Everybody,

**TLDR;** 
* **What batteries should I use?**
* I’m building an electric ride on golf cart
* Needs to be able to carry 125kg (Me + Bag)
* Needs to travel at least 10 miles up / down hills
* Speed not massively important, but 15mph sounds reasonable
* Decent amount of space for bigger batteries if necessary
* So far dual NTM Prop Drive 50-60 270KV / 2400W motors are looking like the best option, I’m open to suggestions.
* Using 178mm Mountain Board Wheels with possibly 3:1 gear ratio (This is my assumption what what I’ve read, I might be totally wrong here!)



----------


Hi There,
Great forum you have here, I’ve been searching through it the last few days trying to learn about electronics, motors, ESC’s etc etc… (My brain hurts) but there isn’t a great deal surrounding what I’m trying to achieve. Please excuse my lack of knowledge my background is programming, this hardware and electronics is alien to me.

I’m looking to build an electric ride on golf trolley. I want it to be able to carry between 125kg / 150kg (that includes me / golf clubs / chassis ) for 10 miles up and down hills. I’ve been looking at using dual NTM Prop Drive 50-60 270KV / 2400W motors but the issue I’m facing now is what type of battery to use that will give both the performance and efficiency needed.

I’ve been looking at using 230mm mountain board wheels with a 3:1 gear ratio. As speed isn’t as important as efficiency (I don’t want to get stranded halfway round, hah) But I would like to achieve 15mph. From what I’ve read the 3:1 ratio would give me a decent amount of torque and the ability to get up hills easier?

I've read elsewhere on the forum that the average is 10wh per km on a flat, but golf courses are notoriously hilly. How should I take this into consideration? Would something like a car battery work?

Size isn’t a big factor for me as the battery will be situated between myself and the golf clubs so I could use a big battery if needed. Does anybody have any suggestions for batteries I should use? Also if there is anything else that I’ve got completely wrong please feel free to let me know. I’m completely new to this and I’m still in the planning stages, I’d like to catalog my build once I know which hardware I’ll be using.

Thanks guys!
Ben.

------
Update:

From all the information you amazing people on this forum have given me this is the setup I've decided to go for so far;

2 x Turnigy Aerodrive SK3 - 6374-192kv Motors
2 x ZIPPY Flightmax 8000mAh 5S1P 30C wires in series (Still under debate, I think this should work?)
2 x Maytech VESCs'

------
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-04-12T20:19:23.271Z Reads: 110

```
Get yourself two SK3 6374 motors for better torque instead of the 270KV 5060 motor. SK3 motors can take up to a max of 12S Lithium-ion batteries. Maybe go for a 10S5P or 12S4P pack. I am taking into consideration the weight of the whole kart affect the mileage of the batteries. Don't use lead acid batteries because it's heavier than Li-ion cells. You can use a taller gear ratio but one around 2.5:1 might be optimum between speed and acceleration.You are free to use the 3:1 if there is ample amount of belt teeth "in mesh" (in the grooves) of the pulley.
```

---
## \#3 Posted by: LikeByte Posted at: 2017-04-12T20:26:22.470Z Reads: 109

```
Thanks for the reply man! Yes I found those motors earlier and they are on my buy list now. I've decided Lipo would be best (I would like to use Li-ion but due to lack of experience and price people have told me Lipo is a better choice) Do you think 2 ZIPPY Flightmax 8000mAh 5S1P 30C connected in series would be enough power to get me 10 miles?
```

---
## \#4 Posted by: t0m_r1dd1e Posted at: 2017-04-12T20:43:09.131Z Reads: 99

```
LiPo is cheaper but doesn't have built in safety features like li-ion, and so can be more dangerous to work with. Are you building your own pack? Are you comfortable with electronics?
```

---
## \#5 Posted by: LikeByte Posted at: 2017-04-12T20:46:23.421Z Reads: 88

```
Hey! Yes, I planned on making sure they are kept in a ventilated hard container to avoid damage. My partners dad who is helping me with this is an electrical engineer so I'm hoping he'll know what he's doing :smile: I believe we'll be adding some sort of safety but I'm leaving that to him.

Would 2 ZIPPY Flightmax 8000mAh 5S1P 30C in series be enough power? From what I've read I think it should be.
```

---
## \#6 Posted by: t0m_r1dd1e Posted at: 2017-04-12T21:00:35.483Z Reads: 83

```
Cool sounds like Lipo will be great for you then. Sorry, I have no idea how to estimate range in this kind of scenario.
```

---
## \#7 Posted by: LikeByte Posted at: 2017-04-12T21:01:57.850Z Reads: 80

```
That's alright, I'm going to give it a go and let the community know whether it works or not! :slight_smile:
```

---
## \#8 Posted by: chuttney1 Posted at: 2017-04-12T21:03:02.421Z Reads: 78

```
Voltage wise, two 5S batteries in series gives you enough power. You just have to select your final drive ratio correctly. Might want to look at other lipo batteries besides Zippy. Some of the lipos tend to slightly puff up from usage, but the better one I have read don't have that problem or it's minimal. I just wish Lipo were not rated by C because I cannot tell what its max amp discharge is. Since you have space.
```

---
## \#9 Posted by: t0m_r1dd1e Posted at: 2017-04-12T21:06:54.367Z Reads: 77

```
Cool project! Keep us posted.
```

---
## \#10 Posted by: LikeByte Posted at: 2017-04-12T21:07:11.987Z Reads: 75

```
I agree, I've chosen the Zippy's because they were the most cost effective to give it a go. Long term I'd like to build a proper 18650 12s4p or something but I need to buy a spot welder and I'd like to get a more more comfortable about learning the in's and outs of how battery's actually work.

Ironically I work for a vape company and have access to HG2's and 25R's for about £3 each so hopefully that will come in handy later!
```

---
## \#11 Posted by: LikeByte Posted at: 2017-04-12T21:10:02.471Z Reads: 74

```
Thanks man! I'll be putting up a build log once all the parts are ordered. I can't wait to get started!
```

---
## \#12 Posted by: chuttney1 Posted at: 2017-04-12T21:48:30.018Z Reads: 67

```
I will be watching how this goes. I knew with the eskate part one could make a go-kart using the same batteries and controller. For the ESC for each motor go get the VESC 6.0 when release. It's better than any speed controller on the market and is currently in testing.
```

---
## \#13 Posted by: smurf Posted at: 2017-04-12T22:01:57.433Z Reads: 66

```
Check out http://www.batteryblocs.com/
You don't even have to weld a battery together to make a pack out of 18650's
```

---
## \#14 Posted by: Mobutusan Posted at: 2017-04-13T05:07:39.568Z Reads: 58

```
Cool project. I'd like to do this also at some point. Will golf courses let you play with something like this though? Too much weight on too skinny of tires might do excessive damage to the turf. I know the Golfboard uses 4" wide x 11" tall tires to spread the load out over a wider surface area. Plus, I'm sure they get much more traction on wet, slippery grass and mud, especially being 4wd. Also, you might want to look into a 4:1 or 5:1 gear ratio if you plan on going up lots of hills, and maybe even <150kv motors. With the setup you are proposing (10s; 192kv; 3:1 gearing; 178mm wheels), you will have an estimated top speed of around 30mph, which is double what you want. Comparatively, 5:1 gearing with 149kv motors will give you close to the top speed you want ~15mph, but you'll have tons more torque and should be easier on the system overall, I would think. 

Check out this calculator: 

http://calc.esk8.it

And, if you haven't checked out the Golfboard much, it would probably be good to study their design for reference. 

http://www.golfboard.com/#product-details

Good luck!
```

---
## \#15 Posted by: NickTheDude Posted at: 2017-04-13T13:27:52.573Z Reads: 50

```
How much horsepower does your average golf cart have? If I'm right dual motors and VESCs can only output around 5kW.
```

---
## \#16 Posted by: TarzanHBK Posted at: 2017-04-13T14:14:41.274Z Reads: 49

```
Even less:
12S at 50A (Vesc max.) = 12 x 3,7= 44,4V x 50A = 2220W
2 Vescs = 4440W
```

---
## \#17 Posted by: smurf Posted at: 2017-04-13T18:17:04.379Z Reads: 44

```
8hp motor 500 amps @ 36 volts  
With a light one seat Vehicle 5hp should be enough.

http://ddmotorsystems.com/GolfCartMotors-Mobile.php
```

---
