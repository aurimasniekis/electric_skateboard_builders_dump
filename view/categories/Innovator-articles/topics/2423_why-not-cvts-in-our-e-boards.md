# Why not CVT&rsquo;s in Our E-Boards?

### Replies: 57 Views: 5359

## \#1 Posted by: claudiofiore88 Posted at: 2016-04-18T03:03:21.542Z Reads: 532

```
Here's a video explaining how CVT's work.

https://www.youtube.com/watch?v=uCEvBGT8twM

My girlfriend recently bought a 2013 Chevy Spark.  This car comes with a CVT (Continuously Variable Transmission). This is not the first time I've heard of this type of transmission.  I find them very interesting and unconventional.  How hard would it be to implement this kind of transmission into an e-board.  The current e-board transmission is pretty limiting in that you only have one gear ratio, so sacrifices have to be made when considering startup torque or top speed.  Some of the advantages I can think of having a CVT would be the ability to use smaller motors, having the motor run at it's optimal rpm, and having better efficiency (longer run time).  What do you guys think?  Is this the future of e-boards?
```

---
## \#2 Posted by: lowGuido Posted at: 2016-04-18T03:16:14.197Z Reads: 505

```
Believe it or not i have thought this over more than a few times. Its just a little too complicated  (read expensive ) to do successfully. 
The good old keep it simple mantra always leads me back to the old toothed belt we all know.
```

---
## \#3 Posted by: Pantologist Posted at: 2016-04-18T03:21:12.438Z Reads: 494

```
I've thought about this too, however, there is no smaller size CVTs that I could find and implementing one would make an eBoard look really bulky. It works with Go Karts and I've seen some scooter versions, but making one for eBoards would be a challenge.
```

---
## \#4 Posted by: thisrealhuman Posted at: 2016-04-18T03:33:07.229Z Reads: 484

```
If you had a three wheel setup with a rear drive wheel over 10" it would be good for long trips but even with the softest wheels and smoothest roads you'd be better off with a scooter. The speeds you would be able to get wouldn't be realistic for a plank of wood, handlebars are a must. If you built something small enough to fit under a board and work with wheels less than 100mm it wouldn't be able to stay clean and the time spent on maintenance would outweigh the benefits.

My big idea is to have two motors with different kv and gearing, one for low end torque and one for high speed, but the gears would need to be freewheels like on a bike and the throttle signal will need to come from a custom flight controller.
```

---
## \#5 Posted by: claudiofiore88 Posted at: 2016-04-18T03:35:42.678Z Reads: 445

```
@lowGuido  Yeah, being complicated and expensive are definitely downsides, but it doesn't necessarily mean it's a bad idea.  I've only heard of CVT's in small vehicles: small fuel efficient cars, scooters, and go karts as @Pantologist also mentioned, so what smaller vehicles do we have than our e-boards? lol

@Pantologist  The only thing I've found on a small cvt is this video from 2008

https://www.youtube.com/watch?v=W0BERPIp364
```

---
## \#6 Posted by: claudiofiore88 Posted at: 2016-04-18T03:38:12.260Z Reads: 413

```
[quote="thisrealhuman, post:4, topic:2423"]
My big idea is to have two motors with different kv and gearing, one for low end torque and one for high speed, but the gears would need to be freewheels like on a bike and the throttle signal will need to come from a custom flight controller.
[/quote]

Something similar has been done by @lowGuido a while back.

http://www.electric-skateboard.builders/t/uneven-dual-rear-drive/113
```

---
## \#7 Posted by: Pantologist Posted at: 2016-04-18T03:39:35.180Z Reads: 369

```
Even with it being that small, the amount of space between the center of the trucks to the start of the wheels is very limited. Putting a cvt system inplace of essentially the belt and pulley system we have now would be very hard.
```

---
## \#8 Posted by: thisrealhuman Posted at: 2016-04-18T03:48:37.108Z Reads: 362

```
@claudiofiore88 NICE! thanks for that. That's a big load of science I can take off my to-do list!
```

---
## \#9 Posted by: claudiofiore88 Posted at: 2016-04-18T03:56:52.459Z Reads: 371

```
[quote="thisrealhuman, post:8, topic:2423, full:true"]
@claudiofiore88 NICE! thanks for that. That's a big load of science I can take off my to-do list!
[/quote]

...Not saying you shouldn't do it, you just reminded me of @lowGuido's build.  As far as I know, he's the only one to try an uneven kv dual drive.
```

---
## \#10 Posted by: lowGuido Posted at: 2016-04-18T04:03:06.171Z Reads: 359

```
[quote="thisrealhuman, post:4, topic:2423"]
My big idea is to have two motors with different kv and gearing, one for low end torque and one for high speed, but the gears would need to be freewheels like on a bike and the throttle signal will need to come from a custom flight controller.
[/quote]

haha yeah been there done that.

you want a list of what I have tried and my thoughts on them??

**single wheel drive** 
pros: light weight, economical, long range, simple.
cons: low on torque, not so great on loose surfaces, hard carving on the offside can lose traction.

**Dual rear drive**
pros: awesome torque, good hill climber, good for heavier riders. no traction problems.
cons: heavy, uses more battery, need wider trucks, more expensive.

**Dual diagonal drive**
if you set it up heelside rear and toeside front this makes the ultimate carving machine!
pros: same as dual rear except you can use narrow trucks.
cons: same as dual rear.

**uneven dual drive**
this involves the combination of a big motor and a small motor (in power not size)
this is like a twin turbo high speed boost super fast!
pros: low end torque combined with high end speed, super fast!!
cons: expensive, heavy, still only roughly equivalent to single drive torque.

**direct hub drive**
as far as I can tell so far these are king!!
pros: loads of torque, no belts to skip or snap, and looks a bit more normal
cons: High voltage required, large diameter is starting to get a bit too big for my liking.
```

---
## \#11 Posted by: thisrealhuman Posted at: 2016-04-18T04:16:00.289Z Reads: 303

```
I don't trust hub motors because my riding style involves riding off curbs, staircases, and eventually boardslides. I don't believe a hub motor is strong enough to outlast my satellite motor, and belts are still cheap.

I am wondering about using something like [THIS](http://www.hobbyking.com/hobbyking/store/__67035__Quanum_MT_Series_5206_320KV_Brushless_Multirotor_Motor_Built_by_DYS.html ) as a 90 degree friction drive system. It could be mounted flat on top of the truck with a simple clamp and quad drive would cut the amps way down. My list of science TODOs goes on and on. Too bad money is still a thing. @lowGuido your stack is inspiring!
```

---
## \#12 Posted by: lowGuido Posted at: 2016-04-18T04:21:21.881Z Reads: 283

```
I dunno... im currently testing Jacobs hub motors and I have a set of hummies on the way, the things are solid!
```

---
## \#13 Posted by: Pantologist Posted at: 2016-04-18T04:22:19.744Z Reads: 293

```
But direct drive motors don't really have a gear ratio right? I've only seen one direct drive with a planetary gear system, but just looking at that thing screams hard to maintain because
```

---
## \#14 Posted by: lowGuido Posted at: 2016-04-18T04:24:54.976Z Reads: 287

```
the ones im testing have a 1:1 ratio being direct drive. but they are like 70kv or something..
actually that the only downs side.. you need to run like 10S or 12S to get any decent speed out of them.. I like my small 6S systems.
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2016-04-18T07:54:43.366Z Reads: 274

```
Ok....uneven dual drive....

So like offset KVs?
```

---
## \#16 Posted by: lowGuido Posted at: 2016-04-18T08:05:16.373Z Reads: 275

```
yeah man. cmon pay attention. Crickey! Strewth!
```

---
## \#17 Posted by: Michaelinvegas Posted at: 2016-04-18T08:09:21.638Z Reads: 279

```
Ok saw he other thread from Aug 15' .... I guess some bathroom reading is in order👍🏻
```

---
## \#18 Posted by: lowGuido Posted at: 2016-04-18T08:18:17.767Z Reads: 282

```
hey PS. @claudiofiore88 I don't want to poo poo the idea.. its a great Idea, and I hope someone builds it!
mini CVT would be awesome.
```

---
## \#19 Posted by: Okami Posted at: 2016-10-03T16:21:19.420Z Reads: 250

```
hah, I think @nowind could be one of the first ones to try this out (by making it).. 

There just needs to be enough influential figure to impact this decision.. I hope something does come along one day what would make @nowind to make this crazy mini-scale transmission for eboards.

 From what I've seen, @nowind from machining perspective should be up for this job with no problems :)

---

Once it would be built some calculations could be made, such as: does it outweight the cost / use of sensored system vs transmission system (cost, max speed, energy usage etc)
```

---
## \#20 Posted by: Hummie Posted at: 2016-10-03T17:13:31.263Z Reads: 227

```
Cvts seem ideal for combustion engines where the torque is limited to a smaller range of the possible rpms than electric motors are.  With an electric motor you can get decent torque from almost a standstill and at much higher speeds, not so with a combustion engine without a variable gearbox or a cvt.  They're pretty efficient but seem an unnecessary complication with electric.  Except if u have an electric motor that's really small then I can imagine it would be a benefit.  Seems simpler to get a bigger motor, but cvts are cool and love to see one on a board
```

---
## \#21 Posted by: DanButcher Posted at: 2016-10-31T23:50:07.951Z Reads: 188

```
If anyone would know the basics of CVT -_- CVT transimssion have very poor efficiency at low RPM's, so for esk8 it's useless. You should achive higher top speed but when it comes to launch and hills it would be quiet poor
```

---
## \#22 Posted by: Okami Posted at: 2016-10-31T23:51:40.840Z Reads: 187

```
How much higher RPM would that be?

isnt 4000-8000 rpm high enough? Most petrol engines mostly work in 2-4 range anyway, I think
```

---
## \#23 Posted by: DanButcher Posted at: 2016-11-01T00:19:11.841Z Reads: 189

```
Probably you don't know but cars CVT are more advanced they've got additional electrohydraulic system which allows them to set proper gear even if they don't have such high rpms. This also would be hard to fit (for sure new design of trucks). You need to design CVT specially for the engine(torque) which is another problem. Another thing is that you will have to use high rpms more often and this will probably lower lifecycle of your motor but i'm not sure.

Sorry for me English.
```

---
## \#24 Posted by: Okami Posted at: 2016-11-01T00:20:56.808Z Reads: 186

```
Your english is quite okay! I can understand everything!

 Thanks for educating us, as it turns out you are more advanced in this fields than the rest of us (at least for the ones joining this discussion..)

Too bad that they are not effective in low rpm range..  I assume a 2 different motor or 2 different gearing system would work better then!
```

---
## \#25 Posted by: DanButcher Posted at: 2016-11-01T00:27:48.060Z Reads: 176

```
Yep, and 2 gear ratio system should be quiet easy to apply in esk8 as there are similar rc transmissions.

With chain drive it should be easy ass hell ( similar to bike) and anybody can do it diy.
```

---
## \#26 Posted by: Hummie Posted at: 2016-11-01T06:16:39.041Z Reads: 159

```
why do you say they're inefficient at low speed?  if a simple cvt is set up right it could have an  appropriate gear for low speed.  You could decide the gear ratio.
```

---
## \#27 Posted by: DanButcher Posted at: 2016-11-01T15:33:38.357Z Reads: 157

```
First of all there are no gears in CVT, the ratio is simply changed depends on rpm's. If you would look at specs of cars you can easly see that always same model with CVT have lower torque than manual one. You say about appropriate setup, indeed this can be achived but than you have to build CVT considering engine and wheels. I don't think that we can find manfacturer which will supply us proper belts and the ones that we are able to get will fail quiet often. Imagine belt at 3000 rpm hitting parts of your CVT, in most of cases it will result in buying new gearbox. Another thing are trucks we need to redesign them to get a place for CVT pulley. There are a lot of pros when it comes to CVT, smoothnes of ride, battery saving ( they will use less power than your normal setup). But there are also cons as far as i understand the way how CVT works we've got huge problem when it comes to brakes, probably you need to use external brakes, no regenerative breaking and maintanance cost.

And  yes they are less efficient in power delivery just by design when you compare them to manual.
```

---
## \#28 Posted by: Hummie Posted at: 2016-11-01T15:42:36.149Z Reads: 160

```
when you say "manual" I guess you mean stick.  tell me if i'm wrong but on a car to achieve the most torque you want to be a gear that allows you to be in a really high rpm.   Maybe the cvt for the car you talk of is designed in such a way as to have less torque but its not inherent in a manual vs cvt as you could make the cvt spindle thinner or larger or whatever to achieve a better "gear ratio".  

no brakes is the real deal killer for me.

i read its less efficient but havent gotten to why.  dont understand why it would be
https://www.physicsforums.com/threads/cvt-efficiency.304935/

http://ecomodder.com/forum/showthread.php/transmission-efficiencies-mt-auto-cvt-27432.html

getting to the bottom of it

in all the efficiency comparisons I come across between manual and cvt the manual is using cogs which are more efficient so it's not a fair comparison as we'd be using a belt in both situations.
```

---
## \#29 Posted by: DanButcher Posted at: 2016-11-01T15:54:00.612Z Reads: 151

```
Yep i mean stick (i'm from Poland and in Europe you call it Manual). It work same in CVT, Stick and Automatic  to get highest torque you use the gear which has the highest ratio ( drive wheel is biggest). The effectivness difference comes from design  stick and automatic transmissions use wheels with teeths so each teeth transfer the torque but when we look at design of CVT it uses friction to transfer torque so you need to loose some of torque.

And if somone think that we can apply teeths on CVT pulley, the belt will wearout quiet faster as you will push it only on sides of belts. There are soultions for cars which use chain instead of belt but our problem is to get such small chain designed and manufactured for us.
```

---
## \#30 Posted by: Hummie Posted at: 2016-11-01T16:08:58.217Z Reads: 149

```
since we'd be using a belt in either set-up a cvt would allow the motor to run in it's most efficient rpm.    at slow speeds it seems to run better on efficiency than a car from what I read as a manual doesnt drop down gearing automatically so you end up stuck in a way in an inefficient ratio. (what they say but i dont understand why as it's manual and you could plan ahead and drop down a gear).   the big loss with the cvt seems to be the belt...but we're doing that anyway, well some of us are.
```

---
## \#31 Posted by: DanButcher Posted at: 2016-11-01T16:29:42.725Z Reads: 155

```
You are right but we use belt with teeths which work with teeth pulley since that it's almost same as using gears, cvt pulley doesn't have teeths it's all about friction. I'm using stick daily, you can plan to shift a gear just by hearing how your engine is working. Basicly when you hear that rpms are going lower even if you push throttle than you shift to lower gear ( higher gear ratio) and get additional torque.  It doesn't run better on efficiency it just feel smoother beacause you don't have 1,2,3,4,5,6 gear just one which is automatically adjustable till you reach lowest ratio ( like 6th gear in stick).
```

---
## \#32 Posted by: Okami Posted at: 2016-11-07T23:10:21.188Z Reads: 140

```
https://www.youtube.com/watch?v=cd2-vsTzd9E

This thing looks rather small.. can someone comment on the video?>
```

---
## \#33 Posted by: Hummie Posted at: 2016-11-07T23:34:05.671Z Reads: 140

```
I watched it. Goes from 0:1 to 1:1. That seems good for a board but it's not automatic and u need to physically adjust the lever.  And there's also an over torque safety so if u are in too high a gear, trying to go fast up a steep hill, it won't do it to protect itself from breaking , and u have to adjust the lever.  
So no brakes if u use it, and u need to use another controller other than a simple transmitter for the esc as it's not automatic like a cvt, and the over-torque safety would likely kick in unwanted.  
a cvt would be better on a board I think
```

---
## \#34 Posted by: Okami Posted at: 2016-11-08T10:02:30.140Z Reads: 133

```
Ok thanks, for the review ;) could not make all the details from the video myself.

Though, really liked the small form factor, too bad the ratio is so little and that there are some other ''problems'' / ''stepping stones'' in this one.
```

---
## \#35 Posted by: Maxid Posted at: 2016-11-08T10:13:46.563Z Reads: 132

```
small form factor? this is not the motor but just the "gearbox". Where would this thing fit on a board in addition to the motor?
```

---
## \#36 Posted by: Okami Posted at: 2016-11-08T10:17:58.596Z Reads: 137

```
ah, well im looking more into mountainboards section,.. so longboards are not my primary concern :D

 sorry for that.

---

There are a few areas, where pehaps, by not stepping the voltage way much higher, a somewhat ''low-cost'' gearbox would justify the cost/extra weight.. For example, a high ratio gearing for pure off roading - snow riding etc.. then, a lower gear ratio for just reaching maximum speed..

--

Of course, you can always just switch the pulley on the field.. :D but that's an extra effort
```

---
## \#37 Posted by: Hummie Posted at: 2016-11-08T14:42:56.046Z Reads: 130

```
The gear ratio I think is the good part about it. Confusing with 0:1 to 1:1 but it seems to be effectively an infinitely large wheel pulley , slow, all the way down to a 1:1 which would be effectively the same rpm as the motor and fast
```

---
## \#38 Posted by: DanButcher Posted at: 2016-11-08T14:58:15.492Z Reads: 141

```
What about something like this:
http://www.bigtoysusa.com/evo2speedgearbox.aspx
http://www.instructables.com/id/transparent-gearbox-on-a-homemade-bicycle/?ALLSTEPS
```

---
## \#39 Posted by: Hummie Posted at: 2016-11-08T15:15:08.029Z Reads: 150

```
Why make complications though and lose ur nice smooth brakes.  
Especially with an electric motor whatever you're  after; more torque or greater speed, can be had with a simple single gear ratio.  The losses of ading extra gearing would very likely be greater than if u just ran a large gear ratio, 3:1 or 4:1 maybe, for the torque u want and a used a really high voltage to get the speed.  To get a tiny bit better efficiency u could reduce the voltage but not worth it.

Cool clear gearbox though.  if u want to just do it for the fun of it that's another story
```

---
## \#40 Posted by: DanButcher Posted at: 2016-11-08T15:22:18.119Z Reads: 150

```
With CVT you will loose your smooth brakes but with geared gearbox you won't.
```

---
## \#41 Posted by: skatardude10 Posted at: 2019-02-27T01:27:54.054Z Reads: 94

```
https://www.ebay.com/i/283036536271?chn=ps&ul_ref=https%253A%252F%252Frover.ebay.com%252Frover%252F1%252F711-117182-37290-0%252F2%253Fmpre%253Dhttps%25253A%25252F%25252Fwww.ebay.com%25252Fi%25252F283036536271%25253Fchn%25253Dps%2526itemid%253D283036536271%2526targetid%253D475515274021%2526device%253Dm%2526adtype%253Dpla%2526googleloc%253D9028718%2526poi%253D%2526campaignid%253D1669934840%2526adgroupid%253D65058350539%2526rlsatarget%253Dpla-475515274021%2526abcId%253D1139296%2526merchantid%253D101980505%2526gclid%253DCj0KCQiA5NPjBRDDARIsAM9X1GI0G5tRqoq02hgrlcxBNWK7J1LZaTB_4XzzV9IsxHXjn3C15anzjCgaAt9IEALw_wcB%2526srcrot%253D711-117182-37290-0%2526rvr_id%253D1874243247401%2526rvr_ts%253D2c8395791690ad786876344bffe18c87

Bolt this thing on where the motor normally mounts and moving the motor to the other side?
```

---
## \#42 Posted by: b264 Posted at: 2019-02-27T01:31:44.510Z Reads: 86

```
This is solving a problem that doesn't exist when you use electric motors.  That thing makes a combustion engine act more like an electric motor.  If you already have the better electric motor, then you don't need that thing.
```

---
## \#43 Posted by: skatardude10 Posted at: 2019-02-27T02:35:17.637Z Reads: 84

```
I was just thinking, other than getting an extremely powerful motor/battery combination, how can we get the best of both worlds- extreme low end torque and extreme speeds at the high end simultaneously? It's always a trade-off between speed and torque minus crazy components to offset the lack of torque or lack of speed one way or another. A variable gear ratio sounds perfect.
```

---
## \#44 Posted by: Boardnamics Posted at: 2019-02-27T02:39:08.629Z Reads: 84

```
A 2 speed gearbox could do something like that
```

---
## \#45 Posted by: maxchilton Posted at: 2019-02-27T03:02:58.112Z Reads: 87

```
[quote="skatardude10, post:43, topic:2423, full:true"]
I was just thinking, other than getting an extremely powerful motor/battery combination, how can we get the best of both worlds- extreme low end torque and extreme speeds at the high end simultaneously? It’s always a trade-off between speed and torque minus crazy components to offset the lack of torque or lack of speed one way or another. A variable gear ratio sounds perfect.
[/quote]

It's obvious you've ever ridden a fast board before.  lol.   You're proposing a solution to a problem that doesn't exist. And when you factor in the cost, complexity, unreliability, reduced efficiency, space constraints under the board, control mechanisms etc etc.  It doesn't sound feasible at all.
```

---
## \#46 Posted by: skatardude10 Posted at: 2019-02-27T03:11:53.576Z Reads: 85

```
I am going to assume you meant it's obvious I haven't ridden a fast board? If so.. I gear my board anywhere between 35mph for torque or 50mph for speed. I'm fairly comfortable at 45, easy. 

Secondly, the problem does exist for me. When I have my board geared to max out at 55mph, the low end torque is just alright, but not what I'd want. When geared for 35, torque and braking is much better but maxing out at 35 kinda sucks. 

Besides going 12S8-10P to double+ my available battery min/max, I figured I'd think a bit outside the box if there is another way. My old car had an electric engine + CVT and it worked... sure that doesn't apply directly to Esk8 but at least there are purpose built small form factor CVT transmissions available for stand up scooter sized vehicles for exactly this purpose.

And I am definitely not thinking under the board. Of course this all wouldn't fit under the board. I've got enough stuff on top of my board, I can make more room up top in the rear: take a solid crossbar motor mount, mount the output end of the CVT to that and motors to the other end, with reinforcements where it's needed. It'd be a hunk of junk out the top of the rear end, but I've already got a hunk of junk out the top of my rear end and I don't mind.  Esk8 unlike some is *not* my main form of transportation and if my board takes a rideability hit or downtime for some experimentation, I love the experimentation.

If a CVT means I could spin my motors closer to their max efficiency RPMs at most speed, and have the ratio adjusting on the fly based on load... That's my dream

I'll update later on if I at least draw up some concepts at some point. Seems nobody has even tried it, might as well try it to see for sure. People said steering dampers were pointless, just get better at riding or tune your bushings- imo they were way wrong. I trust your guys opinions for the most part, but I think there may be something to all this. And if it's $300 down the drain, so be it.
```

---
## \#47 Posted by: b264 Posted at: 2019-02-27T05:18:05.085Z Reads: 78

```
[quote="skatardude10, post:43, topic:2423"]
I was just thinking, other than getting an extremely powerful motor/battery combination, how can we get the best of both worlds- extreme low end torque and extreme speeds at the high end simultaneously?
[/quote]

The best way is with 2, 3, or 4 different motors.  Different kv and different gear ratios.  Maybe one motor on the back for extra low-end torque and two higher-speed motors in the front.  You might have to write a modified version of firmware to control that correctly.

Or just two motors in the back with different settings.
```

---
## \#48 Posted by: skatardude10 Posted at: 2019-02-27T05:32:20.280Z Reads: 84

```
That's not a bad idea... Maybe for the low speed high torque motors in the rear have those one way bearings between the shaft and a custom pulley so that at their max speed the front end high speed motors can continue to pull beyond the max speed of the rear motors... 

Or vice versa... All the braking force would come from one side in that situation.... 

The problem that arises, ime, is that when I reach a limit in speed on one or a set of vescs, (may be due to ERPM limits in firmware?) That when you are applying throttle the motors resist going any faster. So, the torquier motors would resist the faster motors, necessitating the need for a one way bearing to allow them to roll faster than the max speed of that KV motor. 

Still, with one way bearings on the lower speed motors, the brake force will have to go through the higher speed motors- less brake force. 

Regardless of one way bearings, do people commonly do a 4wd setup with 2 motors at higher KV and two at a lower KV? I haven't seen much at all... It sounds like a great solution if at higher speeds we could disable and free-roll the low-KV motors, and re-engage when we need braking force. 

I'd much prefer this approach than retrofitting clunky CVTs to my drives.
```

---
## \#49 Posted by: b264 Posted at: 2019-02-27T05:44:14.283Z Reads: 80

```
[quote="skatardude10, post:48, topic:2423"]
The problem that arises, ime, is that when I reach a limit in speed on one or a set of vescs, (may be due to ERPM limits in firmware?) That when you are applying throttle the motors resist going any faster. So, the torquier motors would resist the faster motors, necessitating the need for a one way bearing to allow them to roll faster than the max speed of that KV motor.
[/quote]

Yes -- custom firmware that disables throttle and braking for the *sensored* torquier motor above max erpm might be something you'd need, leaving power on the unsensored higher-speed motors.  It'd all depend upon exactly how you implemented it.  Maybe cutting power from the unsensored motors at the lowest of low speeds.

I think if you chose wisely though you could probably design this in a way where you could use standard firmware.
```

---
## \#50 Posted by: Acido Posted at: 2019-02-27T06:05:46.491Z Reads: 76

```
If "simple" gear drives are like 500eur, I would imagine the prices of cvts double
So a 1000eur just to get maybe a 3-4miles out of your board?
No thanks
```

---
## \#51 Posted by: Goonman Posted at: 2019-03-02T11:47:24.882Z Reads: 61

```
If you can pull this off it would be pretty special. Give it a try. There is only way to know for sure.
```

---
## \#52 Posted by: Schulerbible Posted at: 2019-03-02T12:00:24.854Z Reads: 59

```
Google Voltige Board, they made a miniature CVT for an Esk8. Sadly, the kickstarter failed
```

---
## \#53 Posted by: Pedrodemio Posted at: 2019-03-02T14:57:25.297Z Reads: 60

```
But if will go over the ERPM by a considerable amount you will start braking with that motor due to the MOSFETs conducting when the voltage gets above the battery plus diode drop *2

A solution would be o have a one bearing inside the pulley, and a custom controller that completely cuts power to that motor once up to a given speed, something like that CarvOn hybrid with a single motor in the back
```

---
## \#54 Posted by: Bobby Posted at: 2019-03-02T15:04:50.427Z Reads: 60

```
Id prefer my board not smell like a petting zoo.... cvt oil stinks
```

---
## \#55 Posted by: Battosaii Posted at: 2019-03-02T19:23:52.015Z Reads: 52

```
I hate CVT in cars they are no fun. I'd rather have a set gear ratio on my board, plus how will the CVT handle braking?
```

---
## \#56 Posted by: Friskies Posted at: 2019-03-03T05:11:48.611Z Reads: 37

```
You want more torque and the same high speed on your board? Ever thought of just adding another two motors to the front? It will literally fix all of your problems.
```

---
## \#57 Posted by: uigiroux Posted at: 2019-03-03T07:07:05.966Z Reads: 34

```
I created a topic for the Voltiage board with CVT a longggg time ago.  I'm to lazy to look it up, lol, but, I was quite convinced as to why not to persue it.  The main reason I even thought about it was at the time I was also thinking of building a custom moped with CVT which is pretty sweet... However, I don't think it'll translate well for a Esk8.  If you can pull it off though that would be pretty cool!
```

---
