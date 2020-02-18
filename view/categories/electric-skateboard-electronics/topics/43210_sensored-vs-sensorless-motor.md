# Sensored vs. Sensorless Motor

### Replies: 64 Views: 6362

## \#1 Posted by: madlemgw Posted at: 2018-01-08T19:10:55.893Z Reads: 687

```
I'm trying to put the pieces together I need to build a board.  I have been reading a lot about Sensored and Sensorless motors and not sure which to go with.  The application I plan on using my board is in a unconventional way (golf course).  So I need something that will start softly so I don't tear up the fairways.  From what I have read is that sensored is smoother and can get the motor turning is lower RPM's.  I'm not needing speed 10-12 mph tops.  If sensored is better any recommendations on what to get?   They appear to be quite a bit higher in price.  Sorry if this has been covered already new to the eboard community.
```

---
## \#2 Posted by: SeanHacker Posted at: 2018-01-08T19:15:15.272Z Reads: 670

```
I use two of these  collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-190kv and startup is very smooth. Uncensored motors need to be nudged a bit to make it out of the stutter startup.
```

---
## \#3 Posted by: b264 Posted at: 2018-01-08T19:15:18.088Z Reads: 668

```
Sensored will start from a dead stop very smoothly -- while sensorless you'll likely have to kick-push and once you're moving, even if slowly, the motor can take it from there.  You probably want sensored based on what you said...
```

---
## \#4 Posted by: evoheyax Posted at: 2018-01-08T19:26:59.713Z Reads: 658

```
If the motor gets over a certain size and you have enough together, sensoreless startup can be almost as good as sensorless. For example, I don't need to push my 4x hummie motors (unsensored) to get going. But I think my case is an extreme, haha.

For most, you will want a sensored motor. The only downside is a sensored motor has 3 more parts that can break, and you could get cogging still from the esc while the esc uses the sensors if something does go wrong with one of them, that even kick pushing won't get rid of (you'd have to turn off the sensor mode in the esc to ride unsensored at this point).
```

---
## \#5 Posted by: Battosaii Posted at: 2018-01-08T19:31:17.699Z Reads: 615

```
Had this happen to my dual 6374 build I kept getting errors and cogging and sometimes I'd have a focbox restart and have no power, I figured it had to do with the hall sensors so I ran sensorless and it's been fine ever since.
```

---
## \#6 Posted by: thisguyhere Posted at: 2018-01-08T19:33:53.821Z Reads: 584

```
for sure the hall sensors can introduce another failure point, but having run both sensorless and sensored hybrid, for me there's no going back to sensorless.

smooth startups without having to either push start or hip shake is just a nice luxury to have.  especially if you're doing a lot of start / stops, ie city riding.

besides, i'm not even sure if you can find sensorless motors designated for esk8s, except the sk3.
```

---
## \#7 Posted by: madlemgw Posted at: 2018-01-08T21:00:21.779Z Reads: 547

```
Any suggestions on what motors to use?  Probably looking at a 190kv.  I see Faraday has one but that seems all i can find.  Looking using a 10s Lilo battery.
```

---
## \#8 Posted by: bigben Posted at: 2018-01-08T21:32:05.510Z Reads: 531

```
https://street-wing.com/product/6374-190-kv-motor/

Here’s one Eu option. 
There may be others...
```

---
## \#9 Posted by: thisguyhere Posted at: 2018-01-08T21:39:44.893Z Reads: 511

```
what voltage battery are you using? 190kv is the most common. and where are you located?
```

---
## \#10 Posted by: pixelsilva Posted at: 2018-01-08T21:48:51.961Z Reads: 497

```
Apparently... Bloomington,IL
```

---
## \#11 Posted by: madlemgw Posted at: 2018-01-08T22:13:26.592Z Reads: 472

```
Shooting for 36v.  Hoping to build a battery out of 18650's.
```

---
## \#12 Posted by: laurnts Posted at: 2018-01-08T22:15:33.288Z Reads: 468

```
If you get sensored, abit more  expensive but performance wise is nice. It's really huge difference between sensored low rpm and uncensored low rpm. It also depends how low, if you plan 1 / 3 gear ratio on grass, I still prefer sensored. It also have better hill climbing power. At high rpm, both sensored / sensorless doesn't matter. I'd always suggest to get sensored 190 kv rather than 120 kv uncensored. Although the torque of 120 kv is better, but it won't turn on hill start.

I ride eMTB on grass and dirt road with 120kv 1:6 gear ratio and I can't go uncensored.
```

---
## \#13 Posted by: thisguyhere Posted at: 2018-01-08T22:34:20.110Z Reads: 437

```
yea go with a 190kv, you'll be good at 10s (36v).  you have plenty of options, torqueboards, build kit boards, psychotiller, longhairedboy, chiboards, etc.
```

---
## \#14 Posted by: SOICDIP Posted at: 2018-01-08T22:40:50.575Z Reads: 441

```
[quote="laurnts, post:12, topic:43210"]
Although the torque of 120 kv is better, but it won't turn on hill start.
[/quote]

Since it has more torque, isn't it better than 190Kv?
```

---
## \#15 Posted by: b264 Posted at: 2018-01-08T22:48:29.016Z Reads: 424

```
If you'll be riding on pavement I recommend 8S battery with dual sensored 5065

If you'll be riding on grass at all, go 10S battery with dual sensored 6374
```

---
## \#16 Posted by: Dariks Posted at: 2018-01-08T22:53:42.570Z Reads: 415

```
For you golf course application you need a mountain board or really big wheels small wheels will tare up the grass. Can you post a list of the things that you want to get so we can recommend something for each section. For example motor, motor mount, wheels, trucks deck. Also whats your budget?
```

---
## \#17 Posted by: madlemgw Posted at: 2018-01-08T23:26:42.561Z Reads: 409

```
Items needed:

Board - haven't decided yet.  May make my own.  Looking for something with width 10-12" length 38-40"
Trucks - MBS Matrix Pro 
Motor Mounts - If I remember correctly I believe someone on here made and sold them
Motor - 190kv sounds like sensored is the way to go
Wheels and tires - MBS FiveStar with MBS T2 tires (9")
Battery - 36v (not sure on aH, don't need speed really and some torque to get up hills.  Only needs to last for 10 miles or so, that should easily get me through a full round)
Budget - $1000 or less preferably.  They make boards specifically for golf courses (Golf Board & Golf Skate Caddy) but $4-6k is too rich for me!
I know I'm missing other things, I'm very new to this. I don’t have any of this just rough list.
```

---
## \#18 Posted by: b264 Posted at: 2018-01-09T04:59:39.621Z Reads: 384

```
@marcmt88 makes good motor mounts but a number of other folks do too.  @Boardnamics makes ones for Caliber II trucks and @okp makes them too, and probably someone else I've forgotten.  Oh yeah @psychotiller has some too. and @longhairedboy  Motor mounts all over this mug
```

---
## \#19 Posted by: psychotiller Posted at: 2018-01-09T05:09:50.789Z Reads: 372

```
I have mounts for Surfrodz TKP's, RKPS, Randals, Seizmic, Paris, Buck, Liquid, and a few others...But not Caliber. Caliber can suck it.
```

---
## \#20 Posted by: PredatorBoards Posted at: 2018-01-09T05:11:00.741Z Reads: 365

```
Aww, why the discrimination?
```

---
## \#21 Posted by: psychotiller Posted at: 2018-01-09T05:11:38.724Z Reads: 350

```
Self Respect. haha
```

---
## \#22 Posted by: Colson003 Posted at: 2018-01-09T05:19:36.252Z Reads: 348

```
If you only need 10-12mph this would be plenty: 

https://hobbyking.com/en_us/dt6376-14p-sensored-motor-125kv.html
```

---
## \#23 Posted by: longhairedboy Posted at: 2018-01-09T12:19:14.686Z Reads: 330

```
[quote="psychotiller, post:19, topic:43210"]
Caliber can suck it.
[/quote]

your mom can suck it. lol
```

---
## \#24 Posted by: pixelsilva Posted at: 2018-01-10T01:10:08.911Z Reads: 318

```
Caliber joker.....:point_down:

![image|500x500](upload://phG74FexzJXHONlh8nK6GZu1lY1.jpg)

....inmerse in Caliber world....:point_down:

![image|666x500](upload://xQTfKIl12uMUVFaNS4TwBgn4KZq.jpg)
```

---
## \#25 Posted by: longhairedboy Posted at: 2018-01-10T02:26:27.179Z Reads: 305

```
what's your point? that i like caliber trucks?
```

---
## \#26 Posted by: pixelsilva Posted at: 2018-01-10T02:27:41.497Z Reads: 309

```
More than caliber trucks, you like caliber mounts.
```

---
## \#27 Posted by: longhairedboy Posted at: 2018-01-10T02:31:43.676Z Reads: 309

```
i do like caliber mounts. Mostly because they work well with caliber trucks, which i like. I tried paris mounts on caliber trucks, but that didn't work.
```

---
## \#28 Posted by: pixelsilva Posted at: 2018-01-10T02:35:57.466Z Reads: 310

```
Your Caliber mounts set the example for me to design my custom mounts....

![image|666x500](upload://nUjDrkQFK9snW2JnipN0W587V8k.jpg)
```

---
## \#29 Posted by: pixelsilva Posted at: 2018-01-10T02:36:59.468Z Reads: 301

```
....the reinforcing beam in particular

![image|666x500](upload://6tHcpcUFrZ0sEyfoseuyVL9H0Ws.jpg)
```

---
## \#30 Posted by: psychotiller Posted at: 2018-01-10T02:41:57.297Z Reads: 302

```
Yeah, without that beam Caliber mounts (on caliber2 trucks or clones) pretty much suck. Sorry LHB

Your Mom likes Surfrodz better..
```

---
## \#31 Posted by: longhairedboy Posted at: 2018-01-10T12:30:37.900Z Reads: 300

```
actually i rode around for about 2 months on these mounts without the bar. They don't creep. I lost a wheel at fun speed and dropped the whole corner of the board down on the mount when the bearing cooked and disintegrated. I rode it out on the mount, scraping the ground and grinding a nice gash in it, and it still wasn't misaligned. I haven't changed my belts in over 4 months because of the better alignment, which hasn't been adjusted or even touched at all since initial install. Enertion mounts suck. DIY mounts suck. Alien mounts suck. Your mom's mounts suck.
```

---
## \#32 Posted by: pat.speed Posted at: 2018-01-10T12:38:04.747Z Reads: 304

```
I have just completed my board. I'm running dual sensorless 6354 motors with the eBay esc. It seems to be running in foc as it states because it's super smooth start up (almost zero cogging) and it's silent except for when accelerating hard
```

---
## \#33 Posted by: psychotiller Posted at: 2018-01-10T16:01:57.658Z Reads: 288

```
That sounds sweet but the fruit at the top of the tree is way tastier.
```

---
## \#34 Posted by: longhairedboy Posted at: 2018-01-10T18:37:43.949Z Reads: 288

```
the fruit on the top of your mom is tastier. 


@madlemgw 
I have a set of RSPEC 6355s and a set of Totally Bitchin 6355s. The R-SPECs were rated at something like 2700 watts peak while mine are rated at around 3100 watts peak. Neither of those motors has ever seen anywhere near that, so with that minor discretion ignored, i think either will provide a lovely experience provided you tune it well and keep tweaking it until its how you want it. 

FOC works well on uncensored motors provided you have an ESC that can handle FOC well. IT works really well on sensored motors because of.. well.. sensors. I'm sure the initial startup algorithm would love to see the sensors there, but i think that's the real trick, isn't it? The startup algorithm is the magic because after the damn thing's rolling you can easily guess where the flux angle is. At startup, where the hell is it on an unsensored motor? a good algorithm can figure that out without burping too much, or even at all (perceptively)

so either. 

[quote="evoheyax, post:4, topic:43210"]
If the motor gets over a certain size and you have enough together, sensoreless startup can be almost as good as sensored. For example, I don’t need to push my 4x hummie motors (unsensored) to get going. But I think my case is an extreme, haha.
[/quote]

The Arc Boards penny can start from a standstill on a single un-sensored 4045 using a shit china VESC (flier) and mostly default settings. Minimal burping, but it is BLDC mode and compared to mine in BLDC its like listening to a turbo charged Fiat take off from a late 70's dodge charger. 

All things considered, if somebody was going to name a "best compact slurpee runner of the year" i'd have to hand to those guys in Singapore. The original penny was great but the 121C is a personal favorite and it has a single 5055. 

I realize i'm probably melting some minds right now, considering who i am and what i just said.
```

---
## \#35 Posted by: longhairedboy Posted at: 2018-01-10T20:30:53.328Z Reads: 260

```
[quote="thisguyhere, post:6, topic:43210"]
besides, i’m not even sure if you can find sensorless motors designated for esk8s, except the sk3.
[/quote]

oh yeah, you can get them. I can have a batch of twenty of them next month if the community wants them.  And i can tell you, they're a hell of a lot easier to build my boards with.
```

---
## \#36 Posted by: Deckoz Posted at: 2018-01-10T21:11:31.616Z Reads: 255

```
[quote="longhairedboy, post:31, topic:43210"]
When I mount your mom it sucks
[/quote]

Ftfy

10char
```

---
## \#37 Posted by: mmaner Posted at: 2018-01-10T23:35:49.101Z Reads: 254

```
[quote="longhairedboy, post:27, topic:43210"]
I tried paris mounts on caliber trucks, but that didn’t work.
[/quote]

LOLOLOLOLOL
```

---
## \#38 Posted by: Redfire1 Posted at: 2018-06-07T19:38:24.238Z Reads: 218

```
Hi,I am using racestar motor with sensor,and when I connect the sensor it’s very load and rough like grinder,what could be the reason for than anyone ???![image|360x500](upload://iJmgitsx3iqx8rLYDruilJnvPVj.jpeg)
```

---
## \#39 Posted by: b264 Posted at: 2018-06-07T19:41:43.559Z Reads: 207

```
Did you do a motor detection after you connected the sensors?
```

---
## \#40 Posted by: Redfire1 Posted at: 2018-06-07T19:44:50.853Z Reads: 207

```
I disconnected the motors last week cause I am having some problem with the lining the motors.so I just connected them.
```

---
## \#41 Posted by: b264 Posted at: 2018-06-07T19:46:35.318Z Reads: 204

```
What ESC are you using?
```

---
## \#42 Posted by: Redfire1 Posted at: 2018-06-07T20:04:35.885Z Reads: 201

```
Maytech vesc
```

---
## \#43 Posted by: Redfire1 Posted at: 2018-06-07T20:10:22.742Z Reads: 201

```
![image|497x500](upload://fKFWGprmvKcOrxQdDOmXzhLspJN.jpeg)
```

---
## \#44 Posted by: b264 Posted at: 2018-06-07T20:43:47.210Z Reads: 197

```
Did you do a motor detection after you connected the sensors?
```

---
## \#45 Posted by: briman05 Posted at: 2018-06-07T20:50:06.024Z Reads: 194

```
You need to run the motor detection any time you disconnect or connect phase wires or are connecting or disconnecting the sensor wires.
```

---
## \#46 Posted by: Redfire1 Posted at: 2018-06-07T20:55:17.174Z Reads: 193

```
Ok didn’t know that,I will do it tomorrow thanks
```

---
## \#47 Posted by: Redfire1 Posted at: 2018-06-08T05:02:50.870Z Reads: 183

```
Do you have any link video how to do it
```

---
## \#48 Posted by: CHAINMAILLEKID Posted at: 2018-06-08T05:21:53.486Z Reads: 183

```

[quote="b264, post:3, topic:43210, full:true"]
Sensored will start from a dead stop very smoothly – while sensorless you’ll likely have to kick-push and once you’re moving, even if slowly, the motor can take it from there. You probably want sensored based on what you said…
[/quote]

Just out of curiosity, could you make it work using only one sensored motor, and sensorless everywhere else?

Instead of you having to do the manual push off, the sensored motor would do it for you.
```

---
## \#49 Posted by: Colson003 Posted at: 2018-06-08T06:32:22.475Z Reads: 180

```
@CHAINMAILLEKID yeah I ran a board like that for awhile, on steeper hills the one sensorless motor would cog at start up. 

My advice is if you have them, then use them.
```

---
## \#50 Posted by: Redfire1 Posted at: 2018-06-08T19:50:40.240Z Reads: 175

```
Thanks for the info I did and they are much better
```

---
## \#51 Posted by: Phillisuper Posted at: 2019-01-05T03:30:25.528Z Reads: 114

```
I am doing my first build and plan on ordering the focbox unity.  Does choosing a specific esc determin what kind of motor you should use? I was looking at Flipsky R-6374 190Kv brushless.  Is running two of these a good set up or should I go with sensorless?
```

---
## \#52 Posted by: Andy87 Posted at: 2019-01-05T08:11:55.273Z Reads: 107

```
Don’t buy Flipsky motors.
```

---
## \#53 Posted by: Phillisuper Posted at: 2019-01-05T14:10:45.718Z Reads: 100

```
Is there something particularly wrong with them?
```

---
## \#54 Posted by: Andy87 Posted at: 2019-01-05T14:27:18.100Z Reads: 98

```
They break very fast. Lose magnets etc.
```

---
## \#55 Posted by: Phillisuper Posted at: 2019-01-05T22:46:10.942Z Reads: 92

```
Thanks, what brand do you swear by?
```

---
## \#56 Posted by: mmaner Posted at: 2019-01-05T22:54:34.053Z Reads: 94

```
@psychotiller 6374 190kv motors, best motors around.
```

---
## \#57 Posted by: Skunk Posted at: 2019-01-05T22:55:28.409Z Reads: 96

```
Maytech or bust
```

---
## \#58 Posted by: mmaner Posted at: 2019-01-05T22:55:31.838Z Reads: 98

```
https://psychotiller.com/product/sensored-6374-190kv
```

---
## \#59 Posted by: Andy87 Posted at: 2019-01-05T23:59:16.835Z Reads: 94

```
What they said ☝️
```

---
## \#60 Posted by: mutantbass Posted at: 2019-01-06T00:15:05.352Z Reads: 92

```
those maytech 6374s are absolute monsters. have 2 running on my trampa. start off is smooth as fuck yo :slight_smile:
```

---
## \#61 Posted by: yelnats8j Posted at: 2019-01-06T00:38:01.873Z Reads: 88

```
What about Torque Boards??

Never had any problema with the motors them self on broke 1 because im retarded.
```

---
## \#62 Posted by: Phillisuper Posted at: 2019-01-06T03:18:13.278Z Reads: 81

```
I'm retarded too so I should probably avoid them lol
```

---
## \#63 Posted by: yelnats8j Posted at: 2019-01-06T03:20:59.996Z Reads: 81

```
No it was me taking my board for a spin on the shitty side walks of hershey
I dented the casing by hitting a big rock
(Al the tree roots they planted along side the side walk are lifting it up.)

**There really good In my opinion and even picked up 2 6374 of them for my new build.**

Can someone second me on this?
```

---
## \#64 Posted by: Phillisuper Posted at: 2019-01-06T03:47:00.582Z Reads: 77

```
I was joking lol
```

---
