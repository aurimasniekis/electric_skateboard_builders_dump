# Folding Board Concept, Parts List Help

### Replies: 49 Views: 892

## \#1 Posted by: SilverFox Posted at: 2019-02-27T10:33:08.172Z Reads: 190

```
Edit
UPDATE
Current parts list:
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html
https://hobbyking.com/en_us/motor-mount-cover-with-bearing.html
^(don't know if this is necessary)^
https://hobbyking.com/en_us/gear-set-with-belt.html
https://hobbyking.com/en_us/motor-mount-5.html
https://hobbyking.com/en_us/zippy-compact-4500mah-10s-35c-lipo-pack-xt90.html
https:///collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller
https:///collections/longboard-trucks/products/torqueboards-v2-pro-trucks
https:///collections/longboard-wheels/products/83mm-epower-flywheels-clear-blue

Questions
* is there anything I'm missing (e.g. connectors, BMS, fuses, anti spark thingy etc)?
* is it possible to use 5 2s LiPO's to make the battery slimmer, maybe Li-ion?
* what components do I need to buy to make my own controller?
* I'm trying to save space under the board so is there a possibility that I don't need a BMS and I can just use a balance charger
* is 10s1p enough?
```

---
## \#2 Posted by: Vanarian Posted at: 2019-02-27T11:08:44.687Z Reads: 173

```
https://www.electric-skateboard.builders/t/folding-electric-long-board-build/24068/35?u=vanarian

Welcome man!

Actually there are some successful builds around foldable Longboards decks, you might want to check the link above :v: 

Look forward to see what you're building !
```

---
## \#3 Posted by: Grozniy Posted at: 2019-02-27T11:26:17.723Z Reads: 169

```
https://www.electric-skateboard.builders/t/folding-e-board-first-eboard-build/26279?u=grozniy
```

---
## \#4 Posted by: SilverFox Posted at: 2019-02-27T11:32:51.986Z Reads: 163

```
I was picturing something along the lines of the Linky, folded to 400mmx280mmx120mm
![linky-4|690x459](upload://5Bb5d6orvIoKEiHi4SGDOeBKd14.jpeg)
```

---
## \#5 Posted by: Ixf Posted at: 2019-02-27T14:40:48.207Z Reads: 144

```
Board up is a really strong starting point to work with.
I have a deck and been trying to find time to electricfy it with a set of direct drive from metasurf but their concept is stronger then linky IMO.  The deck maintains its flex and def still feels like a longboard.
![image|499x499](upload://aylY8Zr5GxwfFkiKbms2ekrbHes.jpeg)
```

---
## \#6 Posted by: Trans-amers Posted at: 2019-02-27T14:58:31.401Z Reads: 138

```
Been reactivating my project...

Also Im interested in your design as well. My project was built to deal with steep hills, but I moved out before the project was ever finished... so its a bit op right now. 

If you don't mind the "bulge" dual 6374 will be your best choice

https://www.electric-skateboard.builders/t/crazy-build-foldable-deck-jacob-hub-direct-drive-12s1p-mbs-100mm/38717/22?u=trans-amers
```

---
## \#7 Posted by: SilverFox Posted at: 2019-02-28T07:59:29.714Z Reads: 119

```
my main constraints for this build is high torque, small size when folded and great aesthetics. Board Up looks pretty sick but its way too big.
also would you guys recommend hub motors for a fold up board, I know they don't produce nearly as much torque but most fold up boards I've seen have hub motors.
```

---
## \#8 Posted by: gee Posted at: 2019-02-28T08:32:28.598Z Reads: 114

```
hub would definitely save you some room for folding mechanism and electrical components.
```

---
## \#9 Posted by: Winfly Posted at: 2019-02-28T08:33:01.104Z Reads: 110

```
It depends on which hub motors. Direct drive will be too wide for your application since you would want the wheels be under the board I suppose. 
There's only Raptor 2 hubs and hummies V4 left if you want high torque hubs.
```

---
## \#10 Posted by: Vanarian Posted at: 2019-02-28T09:46:02.732Z Reads: 94

```
Nah there's also MAD hubs and Diyeboard (replaceable PU) hubs ! 

Hummie and Raptor 2 hubs sure are torquier but for his goal a dual Diyeboard is plenty enough (only 30-35km/h top).
```

---
## \#11 Posted by: pat.speed Posted at: 2019-02-28T10:20:24.971Z Reads: 85

```
Yeah I agree, I’d buy them from meepo or wowgo/ownboard diyeboard is a little shady
```

---
## \#12 Posted by: SilverFox Posted at: 2019-02-28T19:35:14.386Z Reads: 79

```
If I were to use a regular belt driven motor. What would be a good choice to maximize torque without sacrificing high top speed. Maybe dual motors?
```

---
## \#13 Posted by: pat.speed Posted at: 2019-02-28T20:11:59.735Z Reads: 75

```
Any 63mm around 190kv for 10s. The larger the length the more powerful though
```

---
## \#14 Posted by: Sn4pz Posted at: 2019-02-28T20:14:32.009Z Reads: 76

```
While pat.speed is right, you might want more torque, in which case you can change the motor kv to around 170 or 180 to gain more torque than before without too much loss of top speed

going lower than that is going to slow you down more than you'd like
```

---
## \#15 Posted by: SilverFox Posted at: 2019-03-01T14:11:23.890Z Reads: 70

```
So think I'm gonna go belt driven, still haven't decided if should do dual motors for extra torque. If so what are the best dual motor configurations you guys can recommend

I've been trying to upload photos of my 3d model but it keeps saying "No space left on device @ io_write"
```

---
## \#16 Posted by: Sn4pz Posted at: 2019-03-01T14:30:14.121Z Reads: 75

```
Other than cost aversion, I don't see why anyone would not want to build a dual. There have been many times people have proven the the power consumption of a properly tensioned and setup dual belt is only slightly higher than the power consumption of a single. 

Singles struggle on hills, and have you ever turned and lost traction of your drive wheel at full speed?? Not fun.

A dual would be perfect in my mind. But if you want to in go single now, maybe you should upgrade your enclosure and get it read for the second vesc... as well as make sure your trucks will be ready to just slap the second motor and mount to it when you're ready
```

---
## \#17 Posted by: SilverFox Posted at: 2019-03-01T16:05:55.462Z Reads: 75

```
what do you guys think, the "crank" part has a 5mm overlap. I'll probably use machined aluminium 
https://imgur.com/WyxOIMG
https://imgur.com/w9HKq8I
https://imgur.com/Hn0YTbj
```

---
## \#18 Posted by: Sn4pz Posted at: 2019-03-01T17:22:21.206Z Reads: 76

```
I am nowhere near qualified enough to give you an answer, sorry :)
```

---
## \#19 Posted by: Mikenopolis Posted at: 2019-03-01T17:56:37.935Z Reads: 76

```
Ronnie just posted a video showing off his Mellow on the BoardUp folding deck. Start at 2:30
https://youtu.be/8SKZnRa7_lQ?t=150
```

---
## \#20 Posted by: pat.speed Posted at: 2019-03-01T19:58:56.580Z Reads: 74

```
I really want to get a mellow just for the convenience when travelling, I’d just take the drive and then buy a deck in the new area to save room. Then I’d have a cool ass board collection from all over the world
```

---
## \#21 Posted by: SilverFox Posted at: 2019-03-01T20:28:47.794Z Reads: 71

```
I added bumpers to the deck and just neatened up. I think I'm gonna go with this design with dual belt driven motors. its time to start compiling my parts list: l
* For the pulleys, belts, wheels, trucks and mounts I'm thinking Enertion, if theres a cheaper option let me know
* I assume the specs of the motors will be different because I'm going dual, so I'm not sure about that 
* Any advice for esc, don't know much about those

what do you guys think

https://imgur.com/UL3n7MY
```

---
## \#22 Posted by: pat.speed Posted at: 2019-03-01T20:30:09.519Z Reads: 64

```
Enertion don’t sell parts like that anymore. They only sell remotes, escs and hub motors. Oh and whistles
```

---
## \#23 Posted by: SilverFox Posted at: 2019-03-01T20:32:10.357Z Reads: 66

```
oh, that sucks. What other vendors can I look to?
```

---
## \#24 Posted by: pat.speed Posted at: 2019-03-01T20:37:45.547Z Reads: 64

```
@torqueboards @JLabs @marcmt88 are a few 

There are lots more tho
```

---
## \#25 Posted by: danile Posted at: 2019-03-01T20:54:21.638Z Reads: 62

```
Do a basic stress analysis before you commit to dimensions/material
```

---
## \#26 Posted by: SilverFox Posted at: 2019-03-01T20:59:42.433Z Reads: 59

```
definitely will do that. Right now I'm just going to focus on getting a parts list so I start ordering things. 
btw thanks pat
```

---
## \#27 Posted by: SilverFox Posted at: 2019-03-02T04:14:48.568Z Reads: 52

```
Is it necessary to have two VESC's, also is there an upper limit to the kv rating for a dual configuration?
```

---
## \#28 Posted by: Lunasi Posted at: 2019-03-02T05:07:33.014Z Reads: 53

```
I think what you need is to take the new Samsung fold and use that as your hinge and build it into the deck just so you can laugh at Apple users who don't have a tablet phone built into their deck :stuck_out_tongue::sweat_smile:
```

---
## \#29 Posted by: SilverFox Posted at: 2019-03-02T05:11:03.580Z Reads: 54

```
taking android flex to the next level
```

---
## \#30 Posted by: SilverFox Posted at: 2019-03-02T05:22:44.340Z Reads: 56

```
I'm thinking dual KEDA 56-63 195KV. How will a 6s configuration affect my torque and top speed compared to a 10s setup?
https://hobbyking.com/en_us/kd-53-20-brushless-outrunner-195kv.html
```

---
## \#31 Posted by: pat.speed Posted at: 2019-03-02T08:22:02.342Z Reads: 53

```
I haven’t run at 6s for a while since by first iteration of my board but these motors work well and have enough torque for my liking. 

However I now run at 12s and a 2.7:1 gear ratio on 100mm wheels and these things are super fast, in speed and acceleration. I don’t think I could stay on under full acceleration but I am only light (60kg)
```

---
## \#32 Posted by: SilverFox Posted at: 2019-03-02T10:07:20.544Z Reads: 47

```
I really want to go dual but i'm having a hard time convincing myself to drop $200+ on VESC's. is there a budget option that wont sacrifice too much function. Perhaps DIYeboards dual ESC's
http://www.diyeboard.com/v11-dual-belt-motor-sine-wave-foc-esc-speed-controller-p-522.html
http://www.diyeboard.com/upgraded-v21-dual-belt-motor-sine-wave-foc-esc-speed-controller-p-599.html
```

---
## \#33 Posted by: Sn4pz Posted at: 2019-03-02T10:40:57.538Z Reads: 44

```
Diyeboard esc is about as anti-vesc as it gets unfortunately. With those controllers you're going to have 0 customisability, just plug and play

If that's what suits you and your budget then go for it, or if you want to save and make sure you get it done right (the first time ;) ) you could save a little more and get a bangin dual vesc

If you're looking for cheap vescs I would recommend maytech and flipsky, they both make different speed controllers. Please do your research as some of the flipsky models are kind of broken across the board. We have plenty of threads about which ones have problems, and what settings work on what setup
```

---
## \#34 Posted by: SilverFox Posted at: 2019-03-02T10:56:46.475Z Reads: 47

```
would I be able to buy this truck and mount only one motor for the time being so if I ever want to convert to dual I don't have to replace the trucks
also its not very clear if they're selling the front and rear trucks
https://maytech.cn/collections/trucks/products/dual-belt-driven-skateboard-truck
```

---
## \#35 Posted by: pat.speed Posted at: 2019-03-02T11:22:49.506Z Reads: 45

```
Yes that is possible but I would be careful with round trucks, I’ve used similar in the past and it was very hard to secure to mount to the truck without vibrations making it move after a while. I would look at some caliber clone trucks and maybe getting some scratched/ imperfect mounts from @Boardnamics if he’s got any left. 

As for vescs I would look at he flipsky 4.12 or hobbyking vesc as it has a 1 year warranty
```

---
## \#36 Posted by: SilverFox Posted at: 2019-03-02T12:17:42.124Z Reads: 41

```
if youre talking about the turnigy one its out of stock
```

---
## \#38 Posted by: Sn4pz Posted at: 2019-03-02T14:26:15.766Z Reads: 41

```
If you haven't bought torqueboards ESC yet, I would rather spend the 30 extra dollars and buy a focbox. with that purchase I know that my ESC will last longer, and more aftermarket support is available
```

---
## \#39 Posted by: SilverFox Posted at: 2019-03-02T14:29:20.204Z Reads: 43

```
where can I get a focbox for $115, aren't they more expensive?
```

---
## \#40 Posted by: Sn4pz Posted at: 2019-03-02T14:35:02.643Z Reads: 44

```
99 dollar esc, 129 focbox

I've seen people sell them for 135. I sold two for 115 each. just gotta find the deals and have your nose to the floor

E: it actually is 85, I was reading the product description 🤷

You've got half a point but if you want something reliable...
```

---
## \#41 Posted by: Sn4pz Posted at: 2019-03-02T14:38:14.752Z Reads: 44

```
If you don't go for the focbox, at least invest in a way to dissapate heat. The mosfets come wrapped in thick plastic heatshrink, it's not great for them to breathe
```

---
## \#42 Posted by: SilverFox Posted at: 2019-03-02T14:42:34.478Z Reads: 41

```
any suggestions on how I could do that?
```

---
## \#43 Posted by: pat.speed Posted at: 2019-03-02T21:10:09.125Z Reads: 42

```
Add heat sinks to the mosfets
```

---
## \#44 Posted by: SilverFox Posted at: 2019-03-03T14:50:54.191Z Reads: 45

```
How does it look, missing anything?
```

---
## \#45 Posted by: SilverFox Posted at: 2019-03-08T14:20:55.831Z Reads: 45

```
UPDATE: I haven't ordered anything so feel free to comment on anything that I should change

Current parts list:

Single belt drive
https://hobbyking.com/en_us/turnigy-sk8-6364-190kv-sensored-brushless-motor-14p.html
https://hobbyking.com/en_us/motor-mount-cover-with-bearing.html
https://hobbyking.com/en_us/gear-set-with-belt.html
https://hobbyking.com/en_us/motor-mount-5.html
2x 5ah 5s in series for 10s1p
https://hobbyking.com/en_us/turnigy-5000mah-5s-30c-lipo-pack-xt-90.html
From Street Wing

[Caliber II 50 degree trucks](https://street-wing.com/product/caliber-ii-fifty-degree-truck/?attribute_colour=Black)

[Enertion FOCbox](https://street-wing.com/product/enertion-focbox-vesc-x/)

[Anti spark switch 180A](https://street-wing.com/product/anti-spark-switch-180a/)

Questions

* Turnigy sk8 190kv or Turnigy Aerodrive sk3 190kv, the sk8 is sensored and the same price as the sk3? Not much info on it on the forum

* Where can I get a 10s bms that won't destroy my budget, is it okay if I just use a balance charger?

* What connectors do I need to connect the motor, batteries and FOCbox (e.g. 3.5mm/5.5mm bullet connectors, XT-60 and XT90)?
```

---
## \#46 Posted by: pat.speed Posted at: 2019-03-08T22:08:03.148Z Reads: 29

```
Unless you are using hobbyking trucks don’t use there motor mount. Get a cheap one from @Boardnamics
```

---
## \#47 Posted by: Mich21050 Posted at: 2019-03-08T22:09:29.386Z Reads: 31

```
Or from @dickyho  :slightly_smiling_face: 

@pat.speed
```

---
## \#48 Posted by: pat.speed Posted at: 2019-03-08T22:11:44.447Z Reads: 33

```
Just wondering has he addressed the bending issue?
```

---
## \#49 Posted by: dickyho Posted at: 2019-03-08T22:15:54.123Z Reads: 31

```
problem fixed long time ago.  :smile:
```

---
## \#50 Posted by: pat.speed Posted at: 2019-03-08T23:45:13.149Z Reads: 27

```
Awesome great to hear
```

---
