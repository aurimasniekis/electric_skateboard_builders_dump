# Cheap Lead acid build, help needed

### Replies: 50 Views: 914

## \#1 Posted by: joor Posted at: 2019-05-13T17:00:39.220Z Reads: 158

```
Hi! My first build will be experimental and almost as cheap as possible, just to get a feel for it. 
I need the electrics and my absolutely maximum budget is 100 euros.
I will be using either a motorcycle(10-12ah) battery or for long distances 105Ah car starter battery, secured on top of a basic 8" deck. 

So far i've used 49€ of it by purchasing this kit :
https://www.ebay.com/itm/400KV-Motor-Mount-Electric-Skateboard-Parts-Kit-Pulleys-For-72MM-70MM-Wheels/222613063381?hash=item33d4c5c6d5:g:PZwAAOSwi-9ZkXOb

Which includes N5065 400kv 1285w 12v motor and belt transmission. 

I am having a hard time choosing a speed controller. Firstly i was going for a simple PWM controller but could not find 100A ones. And now i'm looking for 120A ESC's. Since i will be using lead acid battery... i am confused if ESC can be used with lead acid?

Can you find me a somewhat trustworthy 12v speed controller and care to explain why i should use it?
----------------------------------------------------------------
Out of curiosity, what kind of rough range(km) estimate would i be looking at with 1285w motor and 105Ah car battery?
---------------------------------------------------------------------------------------------------------------------------------------
-------------------------------


Out of skateboard context: 

I am also planning on building a super simple and light 12v outboard/trolling motor for my inflatable rubberboat. And i need a proper 1-2kw motor for it which will be ran by 105Ah starter battery.
I really considered a trucks tail-lift motor which was 12v 2kw but turned it down since it's not designed for continuous use.
Do you know where i could find a proper 1-2kw 12v dc motor for this project?  :wink:
```

---
## \#2 Posted by: maxchilton Posted at: 2019-05-13T17:12:32.116Z Reads: 147

```
You're riding something that could injury/kill you, why go for something as cheap as possible?  Do you have budget for safety gear?
```

---
## \#3 Posted by: AgressivStreetLamp Posted at: 2019-05-13T17:22:44.199Z Reads: 143

```
[quote="joor, post:1, topic:93712"]
Do you know where i could find a proper 1-2kw 12v dc motor for this project?
[/quote]

say you have a motor that puts out 1800 Watts. (roughly 2.5 hp) Since Watts = Volts * Amps, and you have 12 volts, that leaves you pumping a blistering(literally) 150 Amps into a single motor.  Thats a ridiculous amount. 
Edit: and also waaaaayyy above what its rated for (and those are chinese amps which are smaller than real amps) 

![image|265x114](upload://xJqldqvoaDsSBUsLjYuqfgcYHqh.png) 

12 volts isn't really a feasible voltage for Eskate. try 2 batteries in series, 24v should get you a bit further.

[quote="joor, post:1, topic:93712"]
12v motor
[/quote]
no it isnt. check again. its brushless, you need an ESC to make the 12v dc into an AC signal to drive the motor.
```

---
## \#4 Posted by: AgressivStreetLamp Posted at: 2019-05-13T17:27:30.349Z Reads: 130

```
OK, so my disclaimer is don't do this, you're very likely just going to melt something and hurt yourself.
I have been given such advice and taken it and now im alive for it so ya know, just don't die cause then i cant tell you "I told you so"

HOWEVER, this ESC will theoretically do what you want it to do. But it will also likely melt very shortly after.
https://hobbyking.com/en_us/hobbykingr-x-car-120a-brushless-car-esc-sensored-sensorless.html
```

---
## \#5 Posted by: Arzamenable Posted at: 2019-05-13T17:40:58.996Z Reads: 118

```
I think you would benefit from perusing a few more build threads. Consider searching “budget build”. 

When you have a better frame of reference with basics, folks will roger up with helpful info. 

Be safe dude. 🤙
```

---
## \#6 Posted by: Halbj613 Posted at: 2019-05-13T17:46:25.784Z Reads: 113

```
I send there any problem with using a car battery as something doesn’t seem right with being able to use that.

If that’s big of a battery was easily usable then everyone would be using them??🤔🤔🤔
```

---
## \#7 Posted by: joor Posted at: 2019-05-13T17:47:13.263Z Reads: 111

```
[quote="AgressivStreetLamp, post:3, topic:93712"]
12 volts isn’t really a feasible voltage for Eskate. try 2 batteries in series, 24v should get you a bit further.
[/quote]
Can this N5065 400kv motor be ran by 24 volts? It says Rated voltage:12v , by which meaning i am not clear about.  Or are you suggesting on buying a motor rated for 24 volts?

Anyway i've already ordered that 12v motor. What kind of speed range am i looking at with it? Is 30km/h too much on flat?

[quote="AgressivStreetLamp, post:4, topic:93712"]
HOWEVER, this ESC will theoretically do what you want it to do. But it will also likely melt very shortly after.
[/quote]
Is there better options considering my budget is 51 euros for the ESC?
```

---
## \#8 Posted by: wafflejock Posted at: 2019-05-13T17:57:19.255Z Reads: 100

```
Google for energy density of Lead Acid vs Lithium-Ion/Lithium Polymer to see why pretty much no one here has used a lead acid battery.  All batteries pose some risk but the size/weight of lead acid for the power they can hold isn't worth it in this case.  Lead acid car batteries are designed for very high amp draw for a short period of time to kick the starter motor over and get the engine running but don't have the same watts per liter or watts per kg compared with lithium based batteries.

Extra mass means more inertia, slower acceleration/deceleration, more volume means you need a place to put that thing (away from your feet, typically under the board is where everyone straps the lithium cells)
```

---
## \#9 Posted by: joor Posted at: 2019-05-13T17:57:27.687Z Reads: 95

```
[quote="Halbj613, post:6, topic:93712"]
If that’s big of a battery was easily usable then everyone would be using them??:thinking::thinking::thinking:
[/quote]
Just think of putting a 20kg(30x20x20cm) battery on top of your board, it seems kind of impractical compared to light batteries under the board.
```

---
## \#10 Posted by: Halbj613 Posted at: 2019-05-13T17:58:39.612Z Reads: 97

```
That thing weighs 20kg🤨

Also what is the amp draw and voltage from it

Even though it is impractical it could theoretically work if that sort of idea was redesigned. What sort of batteries does it use
```

---
## \#11 Posted by: AgressivStreetLamp Posted at: 2019-05-13T17:59:57.318Z Reads: 94

```
http://calc.esk8.it/ 
use that to work out your speed. 12 v will be 3s (notice it starts at 6S because that is the lowest at which eskate will work reasonably well)

[quote="joor, post:7, topic:93712"]
Is there better options considering my budget is 51 euros for the ESC?
[/quote]
Hobbyking, or bangood are good sources for cheap parts. I just found this one as a first guess.

The bracket, in that kit, **will** break.
The pulley, will most likely not fit your wheel. (what wheels do you have?)

do more research, put a parts list together and then post it here for review. That will save you money on the long run. This kit was already a misstep
```

---
## \#12 Posted by: wafflejock Posted at: 2019-05-13T18:00:27.498Z Reads: 85

```
Also previously mentioned but to get 1285W at 12V would be 1285/12 = 107A which is a high value for amperage, most components will be rated less than this and would fry with any extended amount of 107A current flowing through them (that said most people won't hit peak values but still, we are typically running 40-50V and at peak will draw 15-25A when accelerating depending on rider, ride style etc., 1/4 the amps is 1/16 the heat being generated/dissipated, I^2*R, so 2A = 4R, 8A = 64R where R is a constant... for the most part)
```

---
## \#13 Posted by: wafflejock Posted at: 2019-05-13T18:17:08.603Z Reads: 79

```
In general to compare apples to apples you want to look at Wh of a battery to know the capacity (Ah x V) that and the discharge rate are the two most important factors (aside from physical dimensions/volume/weight) . The 10Ah motorcycle battery might be more manageable size wise but 10 x 12  = 120Wh whereas my two lipo 5S cells in series to make 10S at 5Ah a piece is 185Wh (and probably around the same size)

https://www.bikebandit.com/blog/tough-questions-answered-are-lithium-iron-batteries-really-better-than-lead-acid
```

---
## \#14 Posted by: joor Posted at: 2019-05-13T18:20:32.961Z Reads: 77

```
[quote="AgressivStreetLamp, post:11, topic:93712"]
The bracket, in that kit, **will** break. The pulley, will most likely not fit your wheel. (what wheels do you have?)
[/quote]
Bracket is not a problem for me, it can be remade. Since i have only 60mm wheels and not going for wheel drive, planning on remaking the trucks out of stainless steel with a spinning axle and pulley attached on the axle.

------------------------
Anyway i have asked for cancellation on the 400kv 12v motor kit order.  24 or 36 volts seems like better option, and those can be ran with few motorcycle batteries. I just like cheap(er) and more practical things and finding multiple purposes for what i already have. Lead acid batteries are easily available and i have them anyway.
```

---
## \#15 Posted by: AgressivStreetLamp Posted at: 2019-05-13T18:24:15.203Z Reads: 76

```
Awesome, sounds like you have access to a machine shop?
```

---
## \#16 Posted by: joor Posted at: 2019-05-13T18:26:08.645Z Reads: 77

```
You're right.  Manual lathe and mill.... and TIG welder.
```

---
## \#17 Posted by: AgressivStreetLamp Posted at: 2019-05-13T18:27:03.906Z Reads: 80

```
for basic components, then Id suggest something like this:

Build:
https://www.youtube.com/watch?v=HuNxDbChhPw&amp;app=desktop

parts list:
https://www.youtube.com/watch?v=DbBctZbym9w


using your machine shop, im sure you can make drivetrain yourself.
```

---
## \#18 Posted by: AgressivStreetLamp Posted at: 2019-05-13T18:35:50.028Z Reads: 80

```
As far as batteries go. DC volts are DC volts, no matter where they come from. Any ESC made for 3 s (3 x 3.7 = 11.1v  ) will run with a 12v car battery. Should it be done? I mean, besides the fact that it weighs a metric f**kton I suppose why not? In general anyway. I'm sure someone here will want to tar and feather me for saying that.
I think i heard @b264 audibly groan from thousands of miles away.

For Eskate, 12v is going to be gutless. 
and you'll need high amps (lots of amps = lots of heat = lots of $$$) .

If you're dead set on lead acid, then get 2 or three in series, and that will be for 6s or 9s. 
This also means you have to figure out your own charging method. 

If you want this to work. Put a list together of what you have already, a budget with which to buy. and then we can help you build a board. Failing to plan, is planning to fail.
```

---
## \#19 Posted by: joor Posted at: 2019-05-13T18:50:51.974Z Reads: 79

```
[quote="AgressivStreetLamp, post:18, topic:93712"]
If you’re dead set on lead acid, then get 2 or three in series, and that will be for 6s or 9s. This also means you have to figure out your own charging method.

If you want this to work. Put a list together of what you have already, a budget with which to buy. and then we can help you build a board. Failing to plan, is planning to fail.
[/quote]
Definately, lead acid is my way to go! 24-36v battery bank made of 2-3 motorcycle batteries just has to be changed from series to parallel and those batteries usually have bolt terminals; can be done but might not be really practical. Or charge them seperately. 

Indeed failing to plan is planning to fail but failing sets things into a clearer perspective. I tend to start from the simplest, it seems to be the only way to know what's really needed.

I still hang onto that 100 euro budget, only with different voltage which is now 24-36.
Would that be enough for a reliable motor and esc?
-----------------------------

I'd like to hear your opinion about a 12v outboard with 1-2kw motor. It's just much practical to use a big car battery than 2-4 smaller ones with less capacity.
```

---
## \#20 Posted by: AgressivStreetLamp Posted at: 2019-05-13T18:53:07.094Z Reads: 70

```
$100 for motor and ESC only?
```

---
## \#21 Posted by: joor Posted at: 2019-05-13T18:54:41.911Z Reads: 66

```
Yes you're right but instead € of $.
```

---
## \#22 Posted by: wafflejock Posted at: 2019-05-13T18:57:22.673Z Reads: 65

```
Most everyone here also uses some variation of the VESC it will work down in the lower voltage range but depending on motor choice etc the amps needed might be higher than what the VESC components are rated for, buy nice or buy twice I personally burned up at least 2 ESCs before throwing down on a VESC.   Really won't get a good feeling about this if you are too focused on budget staying that low similar to racing quads you get in cheap then you'll be throwing it all away if you decide to upgrade and throwing everything away will push you away from it I'd guess.
```

---
## \#23 Posted by: Friskies Posted at: 2019-05-13T18:59:40.851Z Reads: 64

```
So many terrible decisions here. I just came to agree with everyone else here telling you: 

**Do not do this. Please for your safety do not do this.**

Just buy a bicycle and ride that to you can afford something that is less likely to seriously injure you.
```

---
## \#24 Posted by: b264 Posted at: 2019-05-13T19:04:13.206Z Reads: 62

```
Once upon a time prebuilt esk8 were sold with lead-acid batteries.
```

---
## \#25 Posted by: b264 Posted at: 2019-05-13T19:05:09.655Z Reads: 60

```
@KaramQ do you still have some of those DC motors and controllers?
```

---
## \#26 Posted by: AgressivStreetLamp Posted at: 2019-05-13T19:08:46.877Z Reads: 61

```
again, for the record. I suggest you do not do this, it is a waste of money, and may end up costing you more than just money. But, I was raised to make my own mistakes, so here you go:

https://hobbyking.com/en_us/turnigy-sk8-5045-240kv-sensored-brushless-motor-14p.html

https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html

will work for 6s

the motor you will probably be able to keep,
The ESC is ok for a while.

It comes in slightly above 100 of your monopoly monies but it'll work. Idk about shipping to EU. Used to live in Germany myself and imports from Hobbyking were a pain
```

---
## \#27 Posted by: KaramQ Posted at: 2019-05-13T19:10:52.955Z Reads: 56

```
Nope, all in the trash
```

---
## \#28 Posted by: AgressivStreetLamp Posted at: 2019-05-13T19:14:19.986Z Reads: 53

```
[quote="joor, post:19, topic:93712"]
I’d like to hear your opinion about a 12v outboard with 1-2kw motor. It’s just much practical to use a big car battery than 2-4 smaller ones with less capaci
[/quote]

Don't know anything about motors that go on water. There is an aerofoil builders forum that may help more.
```

---
## \#29 Posted by: joor Posted at: 2019-05-13T19:18:17.584Z Reads: 52

```
My plans are not all carved in stone lol. I'll let this sink in and  focus on the electric outboard which is a lot more useful to me. Thanks for insight everybody!
```

---
## \#30 Posted by: b264 Posted at: 2019-05-13T19:21:25.866Z Reads: 53

```
https://efoil.builders/
```

---
## \#31 Posted by: Dirt_Bag Posted at: 2019-05-13T23:29:09.757Z Reads: 49

```
I have used ntm 5060 270kv motors with mounts and a 6s 120a xcar beast esc. All is barely used and i would sell it super cheap. 


The kit you are looking at is awful. I think most would agree that the mount is the worst ever made


The motors fail in mere miles. The coils short out and the magnets are always loose and rattling
```

---
## \#32 Posted by: nopushing Posted at: 2019-05-13T23:57:40.611Z Reads: 50

```
Car batteries will work for a bit but sealed lead acid is the way to go and 24 v is easy with smaller batteries like 12 v 7 ah.
```

---
## \#33 Posted by: MD84 Posted at: 2019-05-14T02:37:57.369Z Reads: 47

```
If you want to go cheap with the lead acid I would suggest a 24v brushed motor and a pwm controller. Run a tethered hand throttle. You could run 36v on the 24v motor for some more zip. 

Try to keep you cg low by using the mc batteries. Just realize it will be difficult to tilt the board for turning. You won't have so much agility. Stay away from the tall and heavy starter battery. If the batteries are agm or can otherwise lay down that will help keep your weight low. 

 ![_AC_SY400_|406x400](upload://pCDLdRLP6dmHsXvdGJl5bY7AXJ3.jpeg) 

Remember, you can't use a basic pwm controller with a brushless motor. 

Also without Regen or a battery that can accept Regen you won't have brakes. That could be a problem with all those heavy batteries. Of course we never had that problem on regular skateboards....or did we
```

---
## \#34 Posted by: s5300 Posted at: 2019-05-14T02:55:27.757Z Reads: 46

```
![1557796712812|690x382](upload://q2jInX65WNyDgabVYwGFXwHTxqz.jpeg) 

I got u fam
```

---
## \#35 Posted by: AgressivStreetLamp Posted at: 2019-05-14T06:05:00.071Z Reads: 43

```
Godamn abomination :astonished:
```

---
## \#36 Posted by: b264 Posted at: 2019-05-14T06:14:21.885Z Reads: 45

```
I love this for some reason.
```

---
## \#37 Posted by: bazis Posted at: 2019-05-14T06:16:27.739Z Reads: 47

```
I think, you should search local used boards. For example, this board cost €122. It includes li-ion 12Ah battery and 4 acid batteries.
![image|640x479](upload://BqK4JBSduUShpnNLQcDcPfZz6X.jpeg)
```

---
## \#38 Posted by: joor Posted at: 2019-05-14T07:20:31.893Z Reads: 46

```
[quote="Dirt_Bag, post:31, topic:93712"]
I have used ntm 5060 270kv motors with mounts and a 6s 120a xcar beast esc. All is barely used and i would sell it super cheap.
[/quote]
That sounds intriguing but since i live in Finland, the postage is high. Even so i'd like to know the price for these goods of yours including postage to Finland if possible. 

[quote="s5300, post:34, topic:93712"]
I got u fam
[/quote]
That's wonderful!

[quote="bazis, post:37, topic:93712, full:true"]
I think, you should search local used boards. For example, this board cost €122. It includes li-ion 12Ah battery and 4 acid batteries.
[/quote]
Not in Finland, those are non-existent in here.
```

---
## \#39 Posted by: Dirt_Bag Posted at: 2019-05-14T15:38:47.751Z Reads: 38

```
I would sell the motors for 29 each, the dual mount for 10, and the esc for 40.

If you are seriously interested i can get an exact shipling quote, but i estimate its around 30 to 40. 


All prices in usd
```

---
## \#40 Posted by: mutantbass Posted at: 2019-05-14T15:46:22.102Z Reads: 40

```
Its so ugly its beautiful
```

---
## \#41 Posted by: joor Posted at: 2019-05-14T16:09:40.765Z Reads: 39

```
[quote="Dirt_Bag, post:39, topic:93712"]
If you are seriously interested
[/quote]
No thanks, atleast for now.
```

---
## \#43 Posted by: AgressivStreetLamp Posted at: 2019-05-14T16:30:05.613Z Reads: 39

```
How difficult is it to get something from a chinese vendor to your location? Their shipping rates are usually rather reasonable for global delivery, even if it can take a fortnight
```

---
## \#44 Posted by: joor Posted at: 2019-05-14T16:45:22.442Z Reads: 35

```
Not at all difficult, usually very low or free....downside being long delivery time.
```

---
## \#45 Posted by: joor Posted at: 2019-05-17T15:56:26.826Z Reads: 27

```
Quick question, not about skateboards but about outboard. 48v bldc 1500w motor, what is a good size for a controller? 1500w controller is cheap and 2000w is double the price, but i am assuming 1500w controller for 1500w motor may be too small?
```

---
## \#46 Posted by: AgressivStreetLamp Posted at: 2019-05-17T16:06:14.951Z Reads: 25

```
best post links. Its a little more complicated than just wattage
```

---
## \#47 Posted by: joor Posted at: 2019-05-17T16:37:54.525Z Reads: 20

```
https://www.ebay.com/itm/1500W-Watt-48V-Volt-BLDC-electric-motor-w-Base-BOMA-BM1024-T8F-sprocket-GoKart/163360872237?hash=item260911172d:g:LpsAAOSwyQVb45jE

https://www.ebay.com/itm/48-72V-1500W-Electric-Bicycle-E-bike-Brushless-BLDC-Motor-Speed-Controller/183681573570?hash=item2ac44662c2:g:4YoAAOSwJ8hcYjTw
```

---
## \#48 Posted by: AgressivStreetLamp Posted at: 2019-05-17T16:42:14.334Z Reads: 15

```
looks like the controller is rated up to 40A@72V and the motor is only 40A@48V 

You should be fine. There is plenty of headroom.
```

---
## \#49 Posted by: joor Posted at: 2019-05-17T17:11:56.521Z Reads: 13

```
Do you think it would be possible(smart) to run those items with big 12v battery and a DC to DC 12-48v converter? Any real downsides to it?
```

---
## \#50 Posted by: AgressivStreetLamp Posted at: 2019-05-17T17:19:05.335Z Reads: 15

```
If you somehow find a 40A ,12 to 48V DC/DC converter. Go for it...
```

---
## \#51 Posted by: joor Posted at: 2019-05-17T19:08:38.703Z Reads: 13

```
i am comparing these motors at the moment: 
https://www.ebay.com/itm/Kids-ATV-Electric-48V-1800W-26A-Brushless-DC-Motor-T8F-9T-Moped-Buggy-Go-kart/183566969818?hash=item2abd71abda:g:bbgAAOSwVHpcBdlc
https://www.ebay.com/itm/1500W-Watt-48V-Volt-BLDC-electric-motor-w-Base-BOMA-BM1024-T8F-sprocket-GoKart/163360872237?hash=item260911172d:g:LpsAAOSwyQVb45jE#shpCntId

And what caught my attention was the amps. How can 1500w(5300rpm) have 40A and 1800w 26A(3300rpm), do you think they're rated differently or is rpm the cause of different amps?

I am leaning towards the cheaper one, due its price and more suitable rpm..
```

---
