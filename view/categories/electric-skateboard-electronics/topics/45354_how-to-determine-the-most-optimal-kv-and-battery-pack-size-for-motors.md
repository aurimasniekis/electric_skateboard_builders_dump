# How To Determine the Most Optimal kv and Battery Pack Size for Motors

### Replies: 26 Views: 1563

## \#1 Posted by: uigiroux Posted at: 2018-02-02T16:41:04.501Z Reads: 185

```
I want to build a direct drive motor, similar to Carvon, or Fliess' build ( https://www.electric-skateboard.builders/t/fliess-3-einmal-directdrive-immer-directdrive/32279 ) and I know how to decide what kv and the type of battery pack to use with a 63xx motor, but I just came across an 8072 with 6000W and is 165kv and can go up to 15s for a battery pack.  Also I was looking at an 80100 which can have a custom kv, or they have it ranging from 50kv-200kv with many kv's inbetween those two values and they are 6000W-7000W, and can have a battery pack up to 18s.

So the most we can run on our VESC's is 12s, but what I would like to know is how to determine the best way to run one of these motors, ranging from the kv choice, to the power of the battery pack.  Or would running these at 12s just be pointless?  I feel like the 8072 is one that could be possible to get good performance out of, but maybe the 80100's are just going to be too underpowered... 

Any advice, comments would be greatly appreciated.  I figure if those are all not worth it, I can at least still use the 6384 that they have at 100kv and 4000W.  That would be a beast in speed and torque I think, and it's only 20mm longer for a dual setup so I know that would be great... I just want to check on the larger 80xx's before I choose.
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-02-02T17:14:36.477Z Reads: 172

```
You will not want to run a high kV motor in hub or direct drive, when its a 1:1 gear ratio you will need lower kV for the torque really high kV you will struggle to even start it, let alone high kV over heats really fast with higher kV as well .kV for direct should be 70kv to 140kv max. Also depends on motor size
```

---
## \#3 Posted by: aigenic Posted at: 2018-02-02T18:19:42.150Z Reads: 155

```
http://calc.esk8.it/

use this calculator, for pulleys use 1:1 ratio

60kv on 12S or 80kv on 12s would work well :slight_smile:

Also you dont want to use so huge motor like 80100, you wont be able to fit it on the truck, not even with wide  calibers :) I would use dual 6354, APS have a nice DIY 60kv 6354 motor kit you could use easily :) there was a user who did so and make really sweet dual drive, I might find the topic later...




EDIT: [Here](https://www.electric-skateboard.builders/t/first-build-diy-sensored-duel-63mm-inline-directdrive-90-mm-wheels-vesc-porn/7893) it is
```

---
## \#4 Posted by: uigiroux Posted at: 2018-02-02T18:26:16.937Z Reads: 141

```
Thanks!  Yeah I figured the 80xxx sized motors were not going to be doable, but, I do know I can get some 6384's on there no problem, just like Carvon's or Fliess did for his build ( https://www.electric-skateboard.builders/t/fliess-3-einmal-directdrive-immer-directdrive/32279 ) though he was using the 6374's, but I think I can fit some of APS's 6384's on there and have a incredibly powerful board...

I just looked at the thread you posted, I have looked that one over many times, but it requires a whole lot of work with tools I don't have.  In the link I have up, the guy doesn't have to do a hole lot to get them working and mounted, plus, now there are hub wheel adapters  already made so I wouldn't even have to have one CNC'd for me now...
```

---
## \#5 Posted by: Exiledd_Top Posted at: 2018-02-02T18:28:48.598Z Reads: 121

```
Your still new to the forum I would tell its going to be a tough job but I'd like to c your progress
```

---
## \#6 Posted by: longhairedboy Posted at: 2018-02-02T18:29:08.189Z Reads: 115

```
the magic formula for hubs is low KV and high voltage. 

You need the lower KV for startup torque, and you need the higher voltage to boost that torque and also get your top end back.
```

---
## \#7 Posted by: uigiroux Posted at: 2018-02-02T18:34:12.678Z Reads: 106

```
I'm thinking that 100kv is a nice sweet spot, between 85kv and 110kv like the V4's, but a more powerful motor so I think it'll have better torque and acceleration.  Probably would have about the same top speed though, or maybe a bit more...  Lol, that's what I'm hoping for!
```

---
## \#8 Posted by: aigenic Posted at: 2018-02-02T18:35:16.373Z Reads: 102

```
Yea you are right, he didnt use a lot of tools, it looks so easy, but if you noticed he later replaced the housing with his own, which certainly took him a lot of time to make...

100kv is too high IMO

[60kv on 12s is the sweet spot IMO](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":60,"system-efficiency":85,"motor-pulley-teeth":1,"wheel-pulley-teeth":1,"wheel-size":90}|) (with 90mm, I would use thicker wheels if i were you)
```

---
## \#9 Posted by: longhairedboy Posted at: 2018-02-02T18:41:38.135Z Reads: 98

```
yeah i'd say 70 to 90 at 12S but i can see why 60 would be good move in a lot of situations. Especially on larger thane.
```

---
## \#10 Posted by: uigiroux Posted at: 2018-02-02T18:42:27.680Z Reads: 92

```
Well the Carvon V4 SD-R are 110kv 2500W and that's a 6364, and it gets a top speed of ~40mph
The V4 SD-XL is 85kv 2750W and it's a 6374, but the top speed is about 5mph less so ~35mph
I'm theorizing that a 6384 with 4000W and 100kv (about halfway between the previously mentioned) will have about the same amount of torque, as the XL and probably have the speed of the R.
```

---
## \#11 Posted by: aigenic Posted at: 2018-02-02T18:45:45.619Z Reads: 86

```
How skilled longboarder are you?
```

---
## \#12 Posted by: Exiledd_Top Posted at: 2018-02-02T18:47:04.074Z Reads: 85

```
Am going to tell u the numbers on speed not always true, one member   had a carvon 4wd speed drive r and easily hit 45mph
My quad carvon xl should easily hit 45 as well
```

---
## \#13 Posted by: uigiroux Posted at: 2018-02-02T18:49:31.974Z Reads: 82

```
Been getting kicked out of parking garages for the past 15 years, lol.  I would say I am not a pro or anything, but I can handle pretty much whatever I put my mind to.
```

---
## \#14 Posted by: aigenic Posted at: 2018-02-02T18:57:07.046Z Reads: 77

```
You plan on going dual or single? You didnt specify...

I like that you have experience :) Hope you are familiar with speeds like 40 MPH...I still dont recommend you to risk your life going that fast...dont risk your life (or at least wear lot of protective gear)...It is your choice and your life do whatever you want to, dont be surprised if you get hurt :/
```

---
## \#15 Posted by: uigiroux Posted at: 2018-02-02T19:04:52.262Z Reads: 74

```
I plan to start with dual, and then go 4WD.  I'm very familiar with those speeds, I am a bit of an adrenaline junkie.  I used to be stupid and didn't wear protective gear, but I always do now... only took a horrible concussion for me to realize that... regardless though, yes I will have all the proper protective gear.  I don't have a car, just a motorcycle, so with my helmet and leathers, with wrist, elbow, shoulder, back, and knee pads/supports I will be very well protected!  I definitely want to build an absolute rocket of a board though with the best of everything.  That's why I am starting with dual, cause the costs of VESC 6 and motors and everything gets rather high, and I am just waiting for samsung to release the 30T and 40T hopefully in a month or so...
```

---
## \#16 Posted by: uigiroux Posted at: 2018-02-02T19:11:42.434Z Reads: 72

```
I am loving this process of getting ready to start building the board, like i'm super ADHD/OCD so I've just obsessed about so many things I want to do with regards to the battery, how to charge the battery, having a bunch of electronics setup and what can be accesed from outside of the enclosure, and have like a wireless charger built into the board, also building my own board, lol....  I will be uploading a ton of pics for my build, I'm like super excited to start this.  I can't work on my motorcycle right now, so this is a good thing to occupy my extra time!
```

---
## \#17 Posted by: aigenic Posted at: 2018-02-02T19:14:42.391Z Reads: 70

```
Your project didnt even really start and I already like it :) Good luck :) 

And for the speed you want 100kv on12s will be the sweet spot, maybe bit less if you want to use 97 wheels :)
```

---
## \#18 Posted by: uigiroux Posted at: 2018-02-02T19:17:46.375Z Reads: 70

```
I'll either use 97's or 107's... Probably the 107's...
```

---
## \#19 Posted by: fliess Posted at: 2018-02-02T20:46:21.650Z Reads: 70

```
@uigiroux, adrenaline guy :grinning: I hope you will eventually build your proper direct drive beast, because a pair of 6374 easily pushes you to 60-65kmh...with 0 noise and correct wheels...man you wanna experience this believe me (if you are not yet spoiled downhiller, who cannot have fun on less than 80kmh haha).
```

---
## \#20 Posted by: uigiroux Posted at: 2018-02-02T20:58:25.209Z Reads: 69

```
@fliess that's what I'm hoping to achieve lol!  I am waiting to hear back from some manufacturers about some custom motors, but I expect I'll be starting my build within a month.  I think I'm going to make a proper skateboard press first since I wanna design this board from scratch.
```

---
## \#21 Posted by: Exiledd_Top Posted at: 2018-02-02T21:12:07.809Z Reads: 59

```
1 month to do a project like that is going to take you probably a good 2-3 months getting batteries rn 18650 cells shipped or custom made would take a month alone.
```

---
## \#22 Posted by: uigiroux Posted at: 2018-02-02T21:17:41.331Z Reads: 57

```
I meant i'll be able to start in about a month, not finish in a month.  They haven't even released the batteries I want to use yet.  I'm waiting for the Samsung 40T 21700 cells to come out.
```

---
## \#23 Posted by: NickTheDude Posted at: 2018-02-02T21:41:47.791Z Reads: 56

```
I figure your bottleneck is gonna be the ESC. If you want huge power you're probably going to have to go 4wd or dual with VESC6s.

People use larger motors for hubs since you need to mass in order to combat the heat but it seems to me that not many people using dual belt driven 6374s with normal VESCs are really able to get enough power out of the VESC to use the motors to their full potential.
```

---
## \#24 Posted by: uigiroux Posted at: 2018-02-02T21:45:43.068Z Reads: 56

```
I'm already on the waitlist for the ESCape 6, so I've got the VESC6 covered.  Also, I will have to start out dual drive, but I completely plan to go 4WD as soon as finances allow it.  I think just waiting for the cells I want to use in my battery pack is going to be a bottleneck just waiting for them to be released...
```

---
## \#25 Posted by: NickTheDude Posted at: 2018-02-02T21:46:33.975Z Reads: 58

```
Awesome, sounds like it's gonna be a beast!
```

---
## \#26 Posted by: uigiroux Posted at: 2018-02-02T21:50:37.267Z Reads: 57

```
I'm really hoping it is!  I think one of the things I'll have the most fun with is all the things I plan on adding to the sides of the enclosure that display things or turn something on/off, allow for me to balance charge the battery but as 2 6s batteries, but it'll be a 12s setup...  Oh I can't wait haha!
```

---
