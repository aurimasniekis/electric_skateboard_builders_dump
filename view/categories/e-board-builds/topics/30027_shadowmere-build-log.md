# &ldquo;Shadowmere&rdquo; Build Log

### Replies: 29 Views: 1876

## \#1 Posted by: Holyman92 Posted at: 2017-08-08T04:00:43.612Z Reads: 154

```
**The Backstory**

Not really sure where to start...

This build started as a joke among me and a buddy, and well... The more i actually thought about it... The more i decided maybe i could actually make it happen... 

The jest began when he and i decided to check out the new hobby store next door to the tandy's (our original destination.) The store owner had a lot of "hobbyking" merch or at least what looks like re-branded hobbyking stuff, of which we noticed the Turnigy Rotomax 80cc electric engine... the rest is what this post will develop into.


**The Parts**

2x Turnigy Rotomax 80cc:
https://hobbyking.com/en_us/turnigy-rotomax-80cc-size-brushless-outrunner-motor.html

Trampa HolyPro35° Board 16ply:
http://www.trampaboards.com/35-holypro-mountainboard-drilled-sanded-gripped-with-bolt-kit--1417ply--p-11144.html

Custom Independent Suspension trucks (designed and manufactured by me and a buddy)

2x VESC/ESC TBD...

2x 12s/14s (undecided right now hopefully yall can help point me in the right direction)

I will write more in a few hours, emergency has come up but i wanna get this out there to see what y'all recommend

**UPDATE** 

I built a working model (out of card board) of one side of the design I plan to use for the suspension system (not sure if you can even call them trucks at this point) when i get back home i will upload pics of it.
```

---
## \#2 Posted by: lock Posted at: 2017-08-08T04:11:54.639Z Reads: 139

```
I'm still dreaming up a way to mount some [TMotor P80's](http://store-en.tmotor.com/goods.php?id=422) on my Trampa, so I'm keen to see how you get on.

One potential gotcha. There's 20 poles in that motor, compared to the typical 14 or so in most of the motors you see on here. By my calcs 44.4v (12s) x 195kv x 10 pole pairs = 86580 erpm. . .  that's probably going to be pushing the speed controller.
```

---
## \#3 Posted by: Holyman92 Posted at: 2017-08-08T04:15:03.849Z Reads: 138

```
@lock  see, this is the kinda technical stuff i need input on before buying. as for how i mount them, I am designing the mounts myself and if me and my friend cant get our milling machine operable im gonna freehand it all lol

as for the VESC... would you recommend something else?
```

---
## \#4 Posted by: lrdesigns Posted at: 2017-08-08T04:26:06.744Z Reads: 130

```
This will be a cool ride. 

The vesc will not be able to handle a motor this large. It can draw 6600w, while the vesc is only really good for 1000-2000w if it has heatsinks. You need a serious high power esc this motor. 

Beefy ones like these
https://hobbyking.com/en_us/turnigy-fatboy-v2-300a-esc-4-15s-opto.html
https://hobbyking.com/en_us/turnigy-monster-2000-200a-4-12s-brushless-esc.html
```

---
## \#5 Posted by: Holyman92 Posted at: 2017-08-08T04:31:45.119Z Reads: 122

```
[quote="lrdesigns, post:4, topic:30027, full:true"]
This will be a cool ride. 

The vesc will not be able to handle a motor this large. It can draw 6600w, while the vesc is only really good for 1000-2000w if it has heatsinks. You need a serious high power esc this motor. 

Beefy ones like these

  
https://hobbyking.com/en_us/turnigy-fatboy-v2-300a-esc-4-15s-opto.html
"**WARNING
This ESC is suited to R/C model applications only. Do not attempt to use it to power Push Bikes, Mountain boards, go-karts or similar machines. The programming logic is only designed for R/C Plane and Heli use. No warranty will be offered for incorrect use of this item.**"
https://hobbyking.com/en_us/turnigy-monster-2000-200a-4-12s-brushless-esc.html
"**WARNING
This is an R/C plane/heli only ESC. Do not attempt to use it to power car, buggy, skateboard, go-kart or similar machines. The programming logic is only designed for R/C Planes and Heli and will burn if applied to other devices.**"
[/quote]

Did u see these warnings lol
```

---
## \#6 Posted by: lrdesigns Posted at: 2017-08-08T04:34:26.853Z Reads: 101

```
haha well yeah, that shit will be dangerous. Its hard to find an esc with this power level that has all of the nice adjustments that the vesc has to make the ride more controllable. Usually you only get 3 brake settings and maybe 3 power settings if your lucky.
```

---
## \#7 Posted by: Holyman92 Posted at: 2017-08-08T04:38:40.452Z Reads: 101

```
@lrdesigns, since the VESC is open-sourced... anyway it can be modified and sent off to be custom made?
```

---
## \#8 Posted by: lrdesigns Posted at: 2017-08-08T04:51:08.162Z Reads: 98

```
Actually a really good idea if you have the skills, I saw some guys designed a 12 fet version, rather than the 6 fets it normally has, but it never made it to production. Would really cool to see a ultra high power vesc version.
```

---
## \#9 Posted by: Holyman92 Posted at: 2017-08-08T04:55:41.318Z Reads: 94

```
@lrdesigns I dont but some friends might
```

---
## \#10 Posted by: michaelcpg Posted at: 2017-08-08T04:58:24.651Z Reads: 94

```
Why not use VESC 6's?
```

---
## \#11 Posted by: Holyman92 Posted at: 2017-08-08T05:01:56.109Z Reads: 90

```
any links? @michaelcpg
```

---
## \#12 Posted by: michaelcpg Posted at: 2017-08-08T05:17:15.993Z Reads: 85

```
Have a look on trampaboards.com :)
```

---
## \#13 Posted by: Holyman92 Posted at: 2017-08-08T05:22:06.394Z Reads: 86

```
@michaelcpg I found it but i cant see any specs about it outside the 60v max same as the VESC
```

---
## \#14 Posted by: lrdesigns Posted at: 2017-08-08T05:28:16.192Z Reads: 89

```
They say rated up to 80amps continuous, which would be 3500 watts at 44v. It should be able to handle some peaks quite a bit higher than that, but you might need additional cooling. Probably the best option at the moment.
```

---
## \#15 Posted by: Holyman92 Posted at: 2017-08-08T07:45:58.960Z Reads: 78

```
@lrdesigns I'm gonna have a friend look at the VESC design and see what he can come up with
```

---
## \#16 Posted by: Cobber Posted at: 2017-08-08T08:35:26.314Z Reads: 77

```
Looks cool bro!
I'll follow to see what you come up with.
I have pair of [these](http://www.scorpionsystem.com/catalog/clearance/electronic_speed_controllers/59v_esc/14s_160a_esc/) that I'm hooking to a pair of [these](http://www.scorpionsystem.com/catalog/aeroplane/motors_1/sii-55/S-5535-160KV/)
that I'm mounting to a 17ply Trampa.
agreed, your esc will be the limiting factor. I think you should also consider how you will ride it. If you plan on thrashing hills, trying to do wheelies, burnouts... consider that you will spend large amounts of time at "peak" certainly more than you could hot-doging a rc plane. As such I think as others suggested that the ESC is the weak link. The most expensive thing you buy is the thing you buy twice...
```

---
## \#17 Posted by: Holyman92 Posted at: 2017-08-08T08:41:04.560Z Reads: 80

```
@Cobber I agree, i dont want to have to buy something because i burned it up and possibly cause more damage in the process... but where my mother lives its REALLY hilly and no sidewalks (mainly grass and rocks) i want to be able to roll through that w/ ease (also why i am designing an independent suspension system for this rig) i dont plan to spend all my time pushing it to the max (thats why i wanted the vesc since i could adjust the power curve, however i would like to have the option to go balls to the wall... you never know when you will need speed.)
```

---
## \#18 Posted by: Cobber Posted at: 2017-08-08T08:52:22.599Z Reads: 78

```
@Holyman92 those motors look like bad mother... a couple things to consider, at nearly 2kg each they are heavy... you will need to ride it like you drive a porsche, slow in fast out. It's not a deal breaker though, think of it as personality, I'd ask for a go :slight_smile:
The extra rear weight behind the axel will help with traction but when it breaks it will snap away faster. Maybe you can compensate with battery placement to balance out the weight distribution?
Also the 6600W cont. is good but you need figures for the peak watt/ amp consumption to so you can plan your build.
```

---
## \#19 Posted by: Holyman92 Posted at: 2017-08-08T08:54:18.546Z Reads: 73

```
@Cobber batteries are gonna be as far to the front as i can get them lol... 2 12s/14s packs should add a good counter balance
```

---
## \#20 Posted by: Cobber Posted at: 2017-08-08T09:00:38.634Z Reads: 75

```
and then your feet get in the way... and your battery wires get longer... causes more spikes to your esc... do a search on something like [this](http://www.yge.de/en/accessories/) and why people like Jenso who abuse there kit in the name of fun use them in their builds.
I am adding 2 x (9) capacitor banks to mine.
and then you need to sort out a antispark because of the caps...
it goes on and on...

as I said I look forward to see what you come up with :smiley:
```

---
## \#21 Posted by: Holyman92 Posted at: 2017-08-08T09:04:57.781Z Reads: 59

```
@Cobber true, could always throw it dead center of the board... the custom truck system i am building will add some weight too.... its gonna have small coil overs and swing arms similar to a car's suspension
```

---
## \#22 Posted by: Cobber Posted at: 2017-08-08T09:12:44.371Z Reads: 66

```
[quote="Holyman92, post:21, topic:30027"]
its gonna have small coil overs and swing arms
[/quote]

Awesome!
It has surprised me the tech that is in mountain bike front shocks has not made it to mountain boards. Be it coil over oil, or even air shocks?
For the moment speed can be found with horse power, but in the future it will be with chassis development.
```

---
## \#24 Posted by: Cobber Posted at: 2017-08-08T09:21:49.065Z Reads: 64

```
@Holyman92 have you seen [this](http://www.electric-skateboard.builders/t/my-new-built-and-new-creations-using-aluminum-deck-just-photos-for-judging/29461/15) thread? 
Some cool looking CNC coil over... but I fear it hasn't had the development it needs.
pnumies and active suspension will eat horse power, there will be a cost for a smooth ride. It will take some of the massive motor out of your build.
They still be massive though hehe
```

---
## \#25 Posted by: Cobber Posted at: 2017-08-08T09:40:03.070Z Reads: 59

```
I'm not sure I get you diagram... sorry
```

---
## \#26 Posted by: Holyman92 Posted at: 2017-08-08T09:46:10.294Z Reads: 60

```
@Cobber the board is just kinda there... I'm not good at drawing whats in my head lol... but the shock is between the swing arms, the top will mount to the mounts im making that attach on the top of the board (not shown)... the bottom mounts to the bottom swing arm, and one side mounts to the wheel mount (the square on the left of the pic) and the right will mount to the main part of the trucks (also not shown)
```

---
## \#27 Posted by: Cobber Posted at: 2017-08-08T09:49:12.145Z Reads: 61

```
all cool bro, build hard, get cray cray!
I look forward to see what you come up with
```

---
## \#28 Posted by: Holyman92 Posted at: 2017-08-08T09:55:12.110Z Reads: 67

```
@Cobber I think i might end up going with  [these](http://www.campusskooters.com/shock-absorber-124mm?utm_source=google_shopping&gclid=Cj0KCQjwn6DMBRC0ARIsAHZtCeN-i12Ry-7kREos09zM0aCex6lEXJuncTKM_Hb80hFOGe51F2visBwaAqkmEALw_wcB) or they have some shorter ones that are 100mm from eye to eye.. but only time will tell
```

---
## \#29 Posted by: Cobber Posted at: 2017-08-08T10:26:54.161Z Reads: 70

```
I am messed up, I practically first learnt suspension adjustment from a ktm moto I had. The spring you have will provide rebound, does it have any dampening? That's why the trampas have the rubbers as well as the springs.
Maybe I'm all wrong bro?
Go for it I want to learn from you pushing the boundaries.
Time will tell but I'm going for green or blue rubbers in the back and yellow or none in the front of my trampa... it is a tuning thing. I am looking for evo type handling. I ride goofy and can push the back end with confidence to slide steer.
it is late, gl bro, go hard
```

---
## \#30 Posted by: Holyman92 Posted at: 2017-08-08T10:50:32.450Z Reads: 68

```
@Cobber maybe something like this then? its an air shock

https://www.ebay.com/p/X-Fusion-O2-RCX-Rear-Shock-165mm-X-38mm-MTB-Suspension/1424005747?iid=162580229457
```

---
