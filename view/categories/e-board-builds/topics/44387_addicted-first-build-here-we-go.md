# Addicted! First build, here we go

### Replies: 60 Views: 2612

## \#1 Posted by: ArnhemAnt Posted at: 2018-01-22T23:28:40.825Z Reads: 378

```
Although I am new to the world of electronic skateboards, I have done a lot of reading and watched hours of YT clips. Joining this forum was a massive step in the right direction with so many very knowledgeable people who seem more than happy to give advice. When I first began thinking of building my own board, my initial ideas are far different to where I am now (thanks mainly to this forum) and I am just about to hit the 'BUY NOW' button on a few items to get me started. I figured I would throw up my ideas here and try to open a discussion on whether this is the 'right' choice or whether there are alternatives that I haven't yet considered. 

Firstly, the environment that I will be riding is not your 'standard' urban environment. I live in a very remote part of Australia (Arnhemland) and there are no real 'roads' up here. Most of the surfaces are either just dirt tracks (gravel, dirt, sand (not too deep), etc). This led me to the idea of building a Mountainboard with tyres (tires) that would be suitable to the area I want to ride. I also wanted a board that will be easy to turn as most of the tracks can be pretty tight. I am not aiming to build a board with crazy fast speed, and I would rather compromise speed for torque and longer battery life.
So, with all of this in mind, here is what I have so far as my 'parts list'.
**Trampa Urban Carver board with the Vertigo trucks and 7" wheels (this is put together as a package from Trampa)
**E-Toxx Mini Direct Drive drivetrain. I have chosen this as it is a 'sealed' unit and I think will be better suited to my environment in comparison to a belt drive option.
**2 Dark Matter motors 6374 190Kv
**Dual Focbox
**Enertion Nano-X controller
These parts have all been ordered and I am awaiting their arrival.

Apart from the above, I am still undecided on a few other items like the battery, battery tray and BMS. In my ideal world, I would want the batteries situated under the deck and I have seen some awesome custom builds with low profile, flexible battery trays (like the one on the build that whitepony did), but I can't seem to find anything like this available to purchase. I'm also undecided on battery choice at the moment. I do know that I want 10s4p, but not sure whether I go with LiPo or Li-ion. I'm also on the fence in regards to a BMS and have read that some people don't use them where others do.

Anyway, that's about it for now. Keen to get some feedback on the above and can't wait to get this built and start riding.
```

---
## \#2 Posted by: wafflejock Posted at: 2018-01-23T00:33:59.646Z Reads: 342

```
Regarding the batteries would look at what range you want to get then use some of the calculators to get a rough idea of what size in terms of Wh you need.  10S with 190kv should be good (10\*4.2V\*190kv = 7980 rpm, 60000 erpm /7 pole pairs = 8,571motor rpm so you're under that limit which is good for the DRV safety on the VESC4 based hardware).

In very rough terms 10Wh = 1km so if you want to go 30km between charges you need 30\*10=300Wh.  Most 18650 cells are in the 2500-3000mAh or 2.5-3Ah range and at 10S nominal voltage being 3.7V you have about 3Ah\*3.7V= 11.1Wh per cell, so can take your total Wh you want for range divide by 11.1 and get the number of cells you need in total to be carrying that much energy.  If you go with lipo can just take the Ah on the battery and multiply by 3.7V\*number of cells and get the total Wh.  Example 10S 5Ah (5x2S 5Ah linked in series) then you have 10S\*3.7V\*5Ah = 185Wh

I'm one of the anti-BMS people but I mostly worry about people buying cheap ones with bad instructions and wiring things wrong... also you're effectively strapping your charge circuitry to your board which is basically like a vibration test table.  Basic engineering stuff, less parts = less parts breaking.

That said if you go 18650 and are spot welding your own pack together etc. then I don't see it as a lot more effort to also put a BMS on there for easy charging.
```

---
## \#3 Posted by: ArnhemAnt Posted at: 2018-01-23T01:06:57.694Z Reads: 305

```
Wow - some great info/advice there - thank you very much. 
One reason I am leaning more towards LiPo is that I have experience with this chemistry (flying UAV's) and I have all the charge gear. 
When it comes to  the 18650 batteries, one big hurdle is that I don't have a spot welder and don't really want to fork out for something that I may only use once. I know that I can purchase these battery packs already made up, which is something I am considering.
Decisions, decisions........
```

---
## \#4 Posted by: wafflejock Posted at: 2018-01-23T01:11:50.120Z Reads: 295

```
No problem fixed the \* in my post apparently need to escape them now with \

---

Also on the batteries the 3 or 4P is usually used on 18650 based ones because the max discharge/IR on the cells is such that you can't pull 40A+ from a single cell (usually more like 15-20A per cell), and the more you distribute that amp draw across cells the better (putting them in parallel does this).

With LiPo you have to just look around to see what's good, there is a C rating on the batteries for calculating max draw do C rating * Ah capacity = max discharge in amps, example 40C\*5Ah = 200A the higher that max discharge the better you want it to be well above whatever you will ever actually draw when driving the motor(s) (also manufacturer C rating can't always be trusted).  I also had a charger and some experience with them and also no spot welder or experience with that so stuck with LiPo.
```

---
## \#5 Posted by: scepterr Posted at: 2018-01-23T01:34:09.269Z Reads: 270

```
Could also consider using the N.E.S.E for the 18650s if you have the room, no spot welding required. 
https://www.electric-skateboard.builders/t/n-e-s-e-no-solder-module-battery-packs/36847/31
```

---
## \#6 Posted by: ArnhemAnt Posted at: 2018-01-23T01:34:15.228Z Reads: 263

```
Thanks man, If I go with LiPo, I will most probably be using 90c packs.
```

---
## \#7 Posted by: Namasaki Posted at: 2018-01-23T01:49:51.010Z Reads: 256

```
[quote="ArnhemAnt, post:6, topic:44387"]
If I go with LiPo, I will most probably be using 90c packs.
[/quote]

Now your talking!!

SMC makes high discharge Lipos supposedly top quality.

https://www.smc-racing.net/index.php?route=product/category&path=67_152
```

---
## \#8 Posted by: ArnhemAnt Posted at: 2018-01-23T02:07:47.353Z Reads: 241

```
Thanks for the link man.

So, if I get three of [these](https://www.smc-racing.net/index.php?route=product/product&path=67_152&product_id=491) 'bad boys', then that's all I need?
```

---
## \#9 Posted by: scepterr Posted at: 2018-01-23T02:17:30.373Z Reads: 228

```
That's only 4S, would need 3 for 12S
Oh yeah you did say three 😋

That's gonna give you maybe 8-10 miles range
```

---
## \#10 Posted by: Namasaki Posted at: 2018-01-23T02:23:24.033Z Reads: 228

```
[quote="scepterr, post:9, topic:44387"]
That’s gonna give you maybe 8-10 miles range
[/quote]

I got 10 miles plus with 5ah 12s 25C Lipos without regen braking
with 7.4ah 12s 90C I would expect to get 15 miles plus
Matter fact with my 5ah 10s 60C Lipos I have gotten up to 14 miles on flat ground.
```

---
## \#11 Posted by: scepterr Posted at: 2018-01-23T02:45:25.150Z Reads: 221

```
On pnuematics? I was going by that and being quite generous 😉
44.4v*7.4ah= 328.56Wh÷20=16.428km/10.2m
@25wh/km it's 13.124km/8.155m
```

---
## \#12 Posted by: ArnhemAnt Posted at: 2018-01-23T04:16:22.110Z Reads: 206

```
So, just to ensure I am on the right track here, if I go with the above packs for my battery power, then, do I need a BMS? For charging, I am happy to  just remove the packs to charge them. Just need a way of being able to easily split the packs to balance charge them individually.
```

---
## \#13 Posted by: scepterr Posted at: 2018-01-23T04:36:43.834Z Reads: 203

```
Well the choice is either BMS and you don't have to take them out, simple connection for charging/more portable charger or no BMS and using a balance charger
Either works
```

---
## \#14 Posted by: Namasaki Posted at: 2018-01-23T05:44:12.538Z Reads: 202

```
[quote="scepterr, post:11, topic:44387"]
On pnuematics? I was going by that and being quite generous :wink:
[/quote]

Oops, my bad. 
I was thinking street wheels.
```

---
## \#15 Posted by: ArnhemAnt Posted at: 2018-01-23T06:21:10.549Z Reads: 207

```
Okay, I'm in a bit of a bind here, regarding batteries and charging. For batteries, I only want to have a 10s setup. I reckon I'd put myself in hospital with 12s, especially after watching some of the YT videos with 12s boards - that's some crazy shit right there.
So, if I settle on 10s LiPo, then I am best to get 5 X 2s packs. Obviously, the higher the C rating, the better. This leaves me with two possible choices, so far.
This one:https://www.smc-racing.net/index.php?route=product/product&path=67_152&product_id=126

or, this one:http://www.store.revolectrix.com/Products/Blend435-SILVER-Label-70C-GOPACKS/Revolectrix-5800mAh-2S-LiPO-70C-Silver-Label-GP-KO-JST-XH-Balance-Connector

At this stage, I am leaning towards the Revolectrix battery as I know and trust their stuff after using it for many years flying UAV's.

That aside, then I am left with a decision on BMS. This is all new to me, and there is a lot of info on this forum about BMS, but my brain is in overload with all the info I have taken on board so far. Not even beer is helping!!!
So, if you were to recommend a BMS for my current setup, what would it be and why?
```

---
## \#16 Posted by: scepterr Posted at: 2018-01-23T06:31:47.484Z Reads: 192

```
If going BMS there's another decision to be made, use the BMS for charge and discharge or just charge, I recommend charge only BMS and let the vesc handle limiting. Either the Bestech D140 or D190 are good charge only BMS, the 140 does 10A, 190 does 15A
```

---
## \#17 Posted by: ArnhemAnt Posted at: 2018-01-23T06:38:02.862Z Reads: 190

```
So, if I understand you correctly, I can set up the dual Focbox to handle limiting/discharge?

This Focbox thing is another evil demon that I need to learn to understand.
```

---
## \#18 Posted by: louwii Posted at: 2018-01-23T07:24:59.040Z Reads: 195

```
Yep the Focbox, or VESC in general, have settings to limit the discharge of your battery. You can also limit the amps sent to the motor.
And you can even set a voltage limit for the battery, so you don't discharge it too much.
Very intelligent those things, when programmed properly !
```

---
## \#19 Posted by: ArnhemAnt Posted at: 2018-01-23T09:31:19.283Z Reads: 185

```
Not sure if this is already available, but if not, why isn't there a system that incorporates something like the Focbox/VESC6 (or whatever) with the BMS? Surely there is a market for an item like this??
```

---
## \#20 Posted by: scepterr Posted at: 2018-01-23T09:44:57.676Z Reads: 183

```
You want to be able to move those parts around, change them and it would cost much more to replace if one thing breaks on combined ESC/bms

There are things in the works that offer communication between ESC and bms but they're still discrete components
```

---
## \#21 Posted by: ArnhemAnt Posted at: 2018-01-23T10:07:33.684Z Reads: 170

```
I'm thinking back to the 'old days' with flight controllers and multi rotors/UAV's. The flight controller was the brains and it was the link between all other components (ESC's, motors, etc, etc). I don't see why something like this isn't yet available for this application.
Who knows, maybe I am way off track, but it makes sense to me.
The main controller would be where all the necessary settings are made and all other components plug into this and get their programming from this. To save weight and space, this should even be able to be achieved via bluetooth config.
I'm sure this is possible. it just needs the right people to make it happen - and I'm not one of them.
```

---
## \#22 Posted by: scepterr Posted at: 2018-01-23T17:38:32.343Z Reads: 158

```
It's easier on copters because it's much lower wattage application, putting more things together is simpler, and as far as i can recall none have built-in charging which would be the BMS....so still none have integrated BMS with esc
The vesc/focbox has pretty much all the same functionality and more compared to copter esc
```

---
## \#23 Posted by: ArnhemAnt Posted at: 2018-01-25T02:51:48.231Z Reads: 138

```
Update. After a lot of "to and fro' I have learnt that many places that stock and sell batteries and battery enclosures will not ship to Australia (or overseas). I have also decided to move away from LiPo and go with 18650 type batteries instead. I found a setup on DIYboards that includes the batteries, enclosure and BMS and they can ship to Australia. Not the ideal kind of enclosure that I wanted, but I am hoping it will be sufficient.
```

---
## \#24 Posted by: scepterr Posted at: 2018-01-25T02:54:23.198Z Reads: 132

```
Got a link to the enclosure?
Have you considered a box type battery on the back or middle topside?
```

---
## \#25 Posted by: ArnhemAnt Posted at: 2018-01-25T02:58:45.733Z Reads: 135

```
[This](http://www.diyeboard.com/10s5p-360wh-18650-battery-power-kit-with-bmscharger-enclosure-p-572.html) is what I ordered.
Please tell me it is going to work!!!!

As for mounting options, I really want to keep it under the deck. At this stage, I will be trying to mount it towards the rear, just in front of the rear trucks. The main flex in the board will be in the middle so I want to keep the enclosure away from that. I really don't want to mount anything on the top deck (except my feet).
```

---
## \#26 Posted by: scepterr Posted at: 2018-01-25T03:00:31.605Z Reads: 128

```
I think your ok flex wise considering it's pretty short but the height might be an issue for road clearance
Also the bms on those are pretty low amperage discharge, I would consider bypassing if you experience lack of power
```

---
## \#27 Posted by: ArnhemAnt Posted at: 2018-01-25T03:04:17.871Z Reads: 125

```
What do you mean about low amperage discharge for the bms? Does this mean that the motors won't get the full range of power due to restrictions from the bms?
```

---
## \#28 Posted by: scepterr Posted at: 2018-01-25T03:05:12.692Z Reads: 130

```
Yes the BMS limits the full potential of the batteries versus the focbox
That pack is Max 50A discharge and the BMS is likely 30A
I would confirm the specs with @diyeboard though, they got a ton of options and *I think* I have that right but maybe it's changed
```

---
## \#29 Posted by: ArnhemAnt Posted at: 2018-01-25T03:16:20.963Z Reads: 133

```
Even if it was just 30A from the BMS, what effect would this have on the Dark Matter motors? I presume it would restrict their top speed? How much difference are we talking?
I'm happy to take a drop in speed (providing it's not too much) as I am not after a speed machine.
```

---
## \#30 Posted by: scepterr Posted at: 2018-01-25T04:00:07.802Z Reads: 127

```
Top speed would remain the same, torque would be affected, less acceleration, slower uphill
```

---
## \#31 Posted by: ArnhemAnt Posted at: 2018-01-25T04:25:14.070Z Reads: 119

```
Let's hope that isn't the case. I have asked the distributor for clarification on the BMS. I'll let you know the outcome once I hear back.
```

---
## \#32 Posted by: scepterr Posted at: 2018-01-25T04:27:39.225Z Reads: 124

```
Particularly with your drive train, wheel setup, you need torque
```

---
## \#33 Posted by: ArnhemAnt Posted at: 2018-01-25T04:48:03.781Z Reads: 132

```
Just had it confirmed - max 50A discharge from the BMS.
```

---
## \#34 Posted by: Eboosted Posted at: 2018-01-25T06:33:57.537Z Reads: 132

```
For such a bad roads city why didn't you go with a HS11 or Holly pro deck, they are way more stable at mid/high speeds on bad roads, you should also consider the Primo Alpha 8" or the Innova Mud pluggers instead of the 7" narrow tyres which I personally don't like.

https://i.imgur.com/30A5va0.jpg
```

---
## \#35 Posted by: ArnhemAnt Posted at: 2018-01-25T07:10:03.827Z Reads: 136

```
They say hindsight is 20/20 vision. @Eboosted, I wish I would have known this prior to ordering.....
I opted for the Urban Carver primarily because it had the smaller trucks which, if I understand correctly, make it easier to manoeuvre compared to the other Trampa trucks. I don't want a board for speed. Manoeuvrability is my priority.When placing the order, there was no option to choose 8" rims or tyres (tires) with this board. 7" was the only option I had, and therefore, the Innova Inline tyres were the only option I had. 
I considered getting some 'spare' 8" hubs and Mud Plugger tyres but ended dumping them from my cart as I wasn't sure if they would work on this build (if they aren't an option when ordering, then maybe they don't fit??)- Plus, the price was getting scary as it was. I now know that I could have used the 8" with this setup.
```

---
## \#36 Posted by: Eboosted Posted at: 2018-01-25T07:31:43.898Z Reads: 137

```
This is the look you will have on the carver deck

[img]http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/f/f/ff21494d666a4423910fa9e7d4897e0d21ac6f2e_1_666x500.JPG[/img]

Here is the look with the HS11 deck:

[img]https://i.imgur.com/dvhDuq2.jpg[/img]
```

---
## \#37 Posted by: ArnhemAnt Posted at: 2018-01-25T07:47:06.830Z Reads: 132

```
Are you trying to make me envious?? LOL. 
Looks like I'm jumping back on the Tramp site and ordering a full set of the 8" hubs and Mud Plugger tyres.
I'm fine with my selection of the deck and trucks. Overall, the difference is about 115mm in overall length, yet the wheelbase looks the same. I guess a small deck and mini trucks will allow me to turn a lot tighter, which I am good with.

Anyone want to buy a full set of brand new 7" hubs?
```

---
## \#38 Posted by: scepterr Posted at: 2018-01-25T07:48:00.772Z Reads: 133

```
Did the order ship already? Maybe you can change it
```

---
## \#39 Posted by: ArnhemAnt Posted at: 2018-01-25T07:55:13.002Z Reads: 136

```
Shipped. Trampa are pretty quick with their shipping, but not as fast as you dude.:grin:
```

---
## \#40 Posted by: Eboosted Posted at: 2018-01-25T07:55:22.415Z Reads: 139

```
I made a modification on my ultimate hangers and my turning radio is ridiculous small, I mean it's crazy compared to even a regular longboard truck and fun to ride. The stability is also pretty nice up to 55km/hr you feel extremely safe and in control. 

Checj the modification  on my thread:

https://www.electric-skateboard.builders/t/the-phoenix-trampa-hs11-urban-board/43448

I'm sorry to raise doubts on your build, but I thought you might be open to suggestions/improvements, I'm so happy with the ride quality that I want everyone to get the same benefits and enjoy this board as much as I do.
```

---
## \#41 Posted by: ArnhemAnt Posted at: 2018-01-25T07:58:23.374Z Reads: 138

```
You're not raising doubts man. In fact, I'm glad you have pointed all this out as it may help others in the future.

I guess a skateboard is just like a boat (I come from a fishing background). No matter what boat you have, it's always a compromise - you'll never get everything you want in the one package. Although, it looks like you are a lot closer to this than I am.
```

---
## \#42 Posted by: rich Posted at: 2018-01-25T10:41:55.453Z Reads: 139

```
[quote="ArnhemAnt, post:37, topic:44387"]
Anyone want to buy a full set of brand new 7" hubs?
[/quote]


There are no 7" hubs, the hub is the same for 6.5" to 8" and 125mm Gummies :grinning:
If you like wider tyres you can use the evolve GT 7", perfect fit.
```

---
## \#43 Posted by: ArnhemAnt Posted at: 2018-01-25T13:02:01.841Z Reads: 136

```
[quote="rich, post:42, topic:44387"]
There are no 7" hubs, the hub is the same for 6.5" to 8" and 125mm Gummies
[/quote]


Oh Man! I'm a dick! Shows how much I know about all this stuff.......
So, all I need to do is order some 8" tyres (and tubes) to go onto my current hubs? That's cool.
Thanks also for the tip on the evolve tyres. I'll keep these in mind as well.
```

---
## \#44 Posted by: rich Posted at: 2018-01-25T14:13:32.780Z Reads: 131

```
Don't be too hard to yourself :joy: 
One year ago I had to research all this trampa stuff, can be confusing in the beginning.
```

---
## \#45 Posted by: ArnhemAnt Posted at: 2018-04-16T04:28:28.528Z Reads: 114

```
Figured I'd better provide a few updates and I've finally got some time up my sleeve. Since my last post, a fair bit of the gear has arrived and I now have something resembling an E-MTB. The only things I am still waiting on are the enclosure (from @Eboosted) and then a battery pack. 
I have to say that this forum has been a HUGE inspiration to me and I have learnt so much in such a short time - just from reading posts/threads and watching what other members have been doing. This 'hobby' is changing so fast that I'm sure what we are doing right now will be outdated in far less than a year from now.
Massive thanks to the following (Shit, I hope I remember everyone......)
@scepterr for the Dark Matter motors and other bits and pieces.
@Nowind for the 'sexy as fuck' mini direct drive. If you only knew how many nights I sat just staring at these, while enjoying a few cold ales.......
@trampa for a pretty cool deck and trucks. One of the better options, particularly for off-road, which is my ONLY intention with this build.
@stewii for providing me (and the rest of us) with a fantastic alternative to the current market options with the ESCape. Stewii has also provided me with a lot of assistance along the way, with my myriad of 'stupid' questions, as has @Nowind.

I'd also like to send a big thanks to @DanSkates and @Cobber for the PM's - you guys have helped me a lot and I'd love to be at the level you two are at in both your riding and your understanding, and the fact that you are both pioneering some pretty cool shit right now.
Oh, and to @gbutcher for getting me into this mess right from the start. Gaz, because of you, I now have yet another addiction. 

Anyway, as they say, "pictures, or it didn't happen"

![P4161083|333x500](upload://iTa4zznjwyisY6eaVYdJMFUM502.JPG)
The "Arnhemlander" E-MTB as it currently stands. Note that the front trucks are the Mini's, whilst the rear trucks are the 'standard'. This is because I needed wider hangers for the dual E-Toxx drive system. I'm going to stick with this current configuration and just see how it rides.

![P4161084|333x500](upload://ryoIBfdpmavfleQyuxTKO3hgICE.JPG)
What's a MTB in Arnhemland without the iconic Buffalo head? Had to do it.....

![P4161087|624x416](upload://5MhNdEZ0BG2bwmsLmG4vG1yg9TY.JPG)
Rear of board showing the direct drives and Dark Matter motors. I just love how this whole drive system is so compact.

![P4161086|624x416](upload://wAIg0WVNYBq5MxY0Sldh5T6f1X8.JPG)
Stereotypical board shot.

![P4161085|333x500](upload://GI9SU4jLaMHcHg0xU4roBOJO2N.JPG)
Underside of board - @Eboosted enclosure on it's way to cover up that sticker. Got me buggered why this pic is so outta whack.

![P4161092|624x416](upload://j82ddUZ2G8fUsrCXdHAyKPCYtR1.JPG)
My 'riding boots'. I don't wear shoes!

![P4161093|624x416](upload://y4vdpNATg2mFHEI9k4U7d0DzWE7.JPG)
ESCapes awaiting connection.

![P4161088|624x416](upload://zk3e6RCaX6Kfd8eccYBHhgUuyYl.JPG)
Check this out! I took this shot to highlight just how compact the drive system is. viewed from the side, with the 8" tyres, you can't even see the drive system. I like that a LOT.

![P4161094|624x416](upload://kBX393GiPdxE6YA8fkKaZEaPPFh.JPG)
Thank you @stewii 

![P4161090|624x416](upload://gjS1QeUFVP0mMe66BM6mps4ATJ4.JPG)
Ground clearance looks pretty good. Hmmmm, better go mop the floor when I finish posting this!!

![P4161089|624x416](upload://jmnuLxotnmrWOGjjtRee6XUE7WX.JPG)
Another angle showing how compact the drive system is. Did I mention just how much I LOVE this??

Apart from the enclosure and battery/BMS the only other thing I'll probably change is to ditch the Superstars (don't like the bearing 'fit' and the balancing) and go with the hubs that @Kug3lis is making. Just waiting to hear back from him on pricing and availability.
```

---
## \#46 Posted by: Cobber Posted at: 2018-04-16T04:53:30.341Z Reads: 98

```
I have some of kugies hubs coming, they are not perfectly balanced though, so you will still need to counter the valve stem weight somehow (I use ABC ceramic balance beads).

I have some gravity decks that I run different width axles on, 10mm wider front. It is crazy how different the bushings feel, and changes in stuff like wheel lift...  

crazy sugestion but, don't be afraid to try fwd with your set up ;)
```

---
## \#47 Posted by: ArnhemAnt Posted at: 2018-04-16T05:26:51.170Z Reads: 100

```
[quote="Cobber, post:46, topic:44387"]
don’t be afraid to try fwd with your set up
[/quote]


What is 'fwd'??
```

---
## \#48 Posted by: Aleks Posted at: 2018-04-16T06:12:13.148Z Reads: 96

```
i assume he means front wheel drive
```

---
## \#49 Posted by: ArnhemAnt Posted at: 2018-04-16T06:38:36.240Z Reads: 90

```
Interesting. I had never considered that. I'll keep the drive on the rear for now, but it may be worth playing with swapping it over to the front too... This would put the wider trucks on the front and the narrow (mini's) on the rear.
```

---
## \#50 Posted by: Eboosted Posted at: 2018-04-16T06:44:08.426Z Reads: 91

```
Hope you get the enclosure soon, it's gonna be a blast to ride it!
```

---
## \#51 Posted by: ArnhemAnt Posted at: 2018-04-16T08:18:54.691Z Reads: 89

```
Yep. I can't wait to see the enclosure. One of the very last pieces of this E-MTB puzzle.
```

---
## \#52 Posted by: DanSkates Posted at: 2018-04-16T11:37:12.220Z Reads: 82

```
This thing is gonna be AWESOME!!!! Love the bare foot shot :sweat_smile:  

[quote="ArnhemAnt, post:45, topic:44387"]
@Nowind for the ‘sexy as fuck’ mini direct drive. If you only knew how many nights I sat just staring at these, while enjoying a few cold ales…
[/quote]

It's funny how you can fall in love with these machines.  I frequently crack a beer, turn on the lights in my workshop, look at my board and spin the wheels!  My wife thinks I'm crazy - I'll make sure she knows there's plenty more crazy people out there too :rofl:

I've had full on rain here the last 2 days and it's killed me not to ride my board.  I'm actually setting my alarm for sunrise so I can ride first thing in the morning!
```

---
## \#53 Posted by: rich Posted at: 2018-04-16T12:23:11.744Z Reads: 78

```
This is a very interesting and unique build. I like the combination of trucks, stability plus easy steering. Man your riding boots really made my day :rofl: but I don't think it's a good idea.

[quote="DanSkates, post:52, topic:44387"]
It’s funny how you can fall in love with these machines.  I frequently crack a beer, turn on the lights in my workshop, look at my board and spin the wheels!  My wife thinks I’m crazy - I’ll make sure she knows there’s plenty more crazy people out there too :rofl:
[/quote]

:joy:
This ain't crazy, that's normal.....
Hope you turn on the vescs before you spin the rear wheels. My build took some time because I had to play with the parts before assembling it :grin:
```

---
## \#54 Posted by: gbutcher Posted at: 2018-04-16T12:27:16.138Z Reads: 70

```
Mate this is looking sweet.  Can't wait to hear how she rides.  Jelly as.  Must resist buying one myself....
```

---
## \#55 Posted by: ArnhemAnt Posted at: 2018-04-16T13:10:07.919Z Reads: 72

```
[quote="DanSkates, post:52, topic:44387"]
It’s funny how you can fall in love with these machines.  I frequently crack a beer, turn on the lights in my workshop, look at my board and spin the wheels!  My wife thinks I’m crazy - I’ll make sure she knows there’s plenty more crazy people out there too
[/quote]


Glad to know that I am not alone.......

[quote="rich, post:53, topic:44387"]
Man your riding boots really made my day :rofl: but I don’t think it’s a good idea.
[/quote]

My riding boots have served me well for the past 47 years just as they are. I'm sure they'll continue to do the same, regardless of what I do.
```

---
## \#56 Posted by: ArnhemAnt Posted at: 2018-04-19T06:55:05.223Z Reads: 66

```
@Eboosted enclosure arrived in the post today - yeehaa. 

Not sure yet whether I'll have the ESCapes in the enclosure or not. My main aim is to get a 12s4p with BMS in there. 

![P4191097|624x416](upload://gHUrSEzR45cpKClKlDAds04Su0O.JPG)

![P4191098|624x416](upload://Auu9wvOWkrlJYLhCKrGvWSeV43E.JPG)
```

---
## \#57 Posted by: koralle Posted at: 2018-04-19T09:14:18.510Z Reads: 64

```
[quote="ArnhemAnt, post:45, topic:44387"]
I don’t wear shoes
[/quote]

I really hope you won't fall at high speed. Then you'll reconsider. 

Had a crash _with_ vans on Sunday and my foot is smashed. Kinda wish I had worn boots...
```

---
## \#58 Posted by: ArnhemAnt Posted at: 2018-04-19T09:18:16.002Z Reads: 64

```
[quote="koralle, post:57, topic:44387"]
I really hope you won’t fall at high speed.
[/quote]


Thanks man. I don't plan on high speed. My goal is to ride on bush tracks, which will be slow going.
```

---
## \#59 Posted by: Jebe Posted at: 2018-04-19T10:04:25.558Z Reads: 61

```
Bush tracks, high torque for the ride in and to drag all those barra back out? Want to see some footage man. CU in the NT 😂 are you based in Darwin?
```

---
## \#60 Posted by: ArnhemAnt Posted at: 2018-04-19T10:32:19.317Z Reads: 61

```
You're almost spot on mate. Might also try to drag a few buff out of the scrub while I am at it. All the more reason to upgrade to those Helical gears that @Nowind now has - this will give me 'stealth mode'. 

Not based in Darwin - I don't like cities. I'm based out in the real country - Arnhemland. Nothin' but bush out here mate.
```

---
