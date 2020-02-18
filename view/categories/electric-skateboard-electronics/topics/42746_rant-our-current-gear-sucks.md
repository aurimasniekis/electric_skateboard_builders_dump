# Rant (our current gear sucks)

### Replies: 75 Views: 3590

## \#1 Posted by: pshaw Posted at: 2018-01-04T13:11:25.803Z Reads: 345

```
I'm almost done with my board and there are a few final pieces of the puzzle. Everything is super nice and clean except the final touches. For one... apparently we in the DIY community can't seem to create and anti spark switch that can stay together. The FETs always blow... even on the ones that are deemed "bulletproof". Nothing is worse to be that building a really nice board and then ruining it with a God awful loop key. Yet somehow all the big name boards are doing it with no problem whatsoever. 

Other things that seem like they would be stupid easy to implement. 

Why can't we have vesc based esc with wheel motion to turn on, so you can just turn on the remote throw the board down, give it a kick and take off? This is ridiculously elementary stuff that would take virtually no work whatsoever to make happen!

Drives me nuts.... ok rant over. Since we can't have nice things can anyone point me in the direction of the cleanest possible xt90 port so that I can mount on the side of my enclosure? Also I wonder if there is a loop key out there that has a flat end that would look less terrible than the standard loop key people are using. Any help would be greatly appreciated....

Oh also, if any of you feel the same comment here. Without demand there won't be any innovation, let the vendors hear it! :stuck_out_tongue:
```

---
## \#2 Posted by: Lukas Posted at: 2018-01-04T13:40:48.306Z Reads: 329

```
[quote="pshaw, post:1, topic:42746"]
apparently we in the DIY community can't seem to create and anti spark switch that can stay together
[/quote]

You could create one for the community if you are not happy with the existing solutions. I mean.. it's DIY
```

---
## \#3 Posted by: Cobber Posted at: 2018-01-04T13:44:32.781Z Reads: 318

```


[quote="pshaw, post:1, topic:42746"]
can anyone point me in the direction of the cleanest possible xt90 port
[/quote]

defo recommend you get a black xt90 they are so much cleaner than the baby shit yellow brown ones.

p.s. even after you turn your board off you need to disconnect your batteries so they do not blow up, after you have owned a working board or two for a while you will work this out, or watch your house burn down ;)

edit: Sarcasm (winky face), I'm surprised you got any sincere responses. You just called out every DIY builder and parts manufacturer here and told them all: your gear sucks.
```

---
## \#4 Posted by: Skitzor Posted at: 2018-01-04T13:47:06.387Z Reads: 311

```
You are running 12s? I know LHB is doing this for some years now. What you're stating makes no sence to me. I believe the error is elsewhere then.

Personal opinion about the wheel turn on feature: 
I would not want it on either of my boards. It cannot confidently get a 1 or 0 state like a button. Thinking forward on this, I would not like my board getting turned on while it possible moves in the trunk of my car.
Moving a button to your remote dedicated to turn on remote and board would make it somewhat better. But nothing (reliably) replaces a hardware button on the board itself in my opinion
```

---
## \#5 Posted by: Acido Posted at: 2018-01-04T13:50:26.896Z Reads: 298

```
Get a bms with an eswitch and your first problem is solved
Boom
```

---
## \#6 Posted by: Acido Posted at: 2018-01-04T13:52:13.937Z Reads: 286

```
Someome could think of a solution with a remote with diffrent channels and a reciever on a bestech bms like e switch so you can remotely turn it on or off
```

---
## \#7 Posted by: pshaw Posted at: 2018-01-04T15:00:17.392Z Reads: 276

```
[quote="Cobber, post:3, topic:42746, full:true"]


[quote="pshaw, post:1, topic:42746"]
can anyone point me in the direction of the cleanest possible xt90 port
[/quote]

defo recommend you get a black xt90 they are so much cleaner than the baby shit yellow brown ones.

p.s. even after you turn your board off you need to disconnect your batteries so they do not blow up, after you have owned a working board or two for a while you will work this out, or watch your house burn down ;)
[/quote]

Wuttttttttttttt^ :confused:
```

---
## \#8 Posted by: Deckoz Posted at: 2018-01-04T15:06:26.372Z Reads: 261

```
[quote="Cobber, post:3, topic:42746"]
disconnect your batteries so they do not blow up
[/quote]

Lol... Wut? 

Leaving your ESCs grounded, by having the switch/loopkey on the positive isn't gonna make your batteries explode.. lol
```

---
## \#9 Posted by: GrecoMan Posted at: 2018-01-04T15:08:48.204Z Reads: 249

```
whatchu smokin over there on kangaroo island?  i’ve left my batteries plugged in (loopkey unplugged) for about 5 months without a problem 😉
```

---
## \#10 Posted by: squishy654 Posted at: 2018-01-04T15:11:26.053Z Reads: 247

```
Hey guys he has a point these batteries can explode at any point in time you really should be careful like when you're riding it carrying it storing it charging it not using it letting it sit if it's plugged-in if it's not plugged-in if it's a Tuesday..stay frosty..
```

---
## \#11 Posted by: Deckoz Posted at: 2018-01-04T15:16:38.939Z Reads: 250

```
Healthy batteries,that have solid connections, and are checked regularly for cell internal resistance and pack total resistance are not likely to explode.

If you check your packs, and know your packs, you'll know when your pack is unhealthy and likely to do such.

It doesn't "just happen"


I've been using lithium for a long time, I know my packs, I take care of my packs, I've never had an 18650 vent, and the only time lipo explode is when the cells are damaged and unsafe to be discharged, and I puncture them with a spike on a stick from a safe distance.

Again batteries don't just explode for no reason, there are causes
-punctures
-over charging
-over discharging
-shorts
-crushed
Etc

There is always a cause.
```

---
## \#12 Posted by: longhairedboy Posted at: 2018-01-04T15:19:36.515Z Reads: 244

```
Here is my experience with these particular eswitches:

<img src="/uploads/db1493/original/3X/0/f/0fe84eb8b11bad822aa9fb640649624f83d5b66a.jpg" width="667" height="500">(That's the IRFS7730 on there)

They're fine at 12S under 60amps and under 40mph loads for people under 200 pounds.  Running them on lipos with crazy vesc settings under crazy high loads will do one of a few things that i have seen:

* through some mystery of science cause the fets to lock into the on position. I suspect the load just welds it into place when it gets to hot. Who knows. I see this 99% of the time when they fail. 
* explode the fet with visible fragmentation. I've seen this twice. 
* heat up the solder to the point of reflow and literally move the fet over untill it shorts and either blows up or cooks something.  I've seen this only once, and the BMS caught the short before anything else was damaged. 

I'm working on one now with 2oz copper and three of these fets instead of two, and also some bolt down fuses. As soon as the parts arrive i'll assemble a few and we'll see how they do. I'll be open to selling a few at cost for testing before i retail them.
```

---
## \#13 Posted by: barajabali Posted at: 2018-01-04T15:20:44.775Z Reads: 236

```
[quote="Deckoz, post:11, topic:42746"]
Again batteries don't just explode for no reason, there are causes
-punctures
-over charging
-over discharging
-shorts
-crushed
Etc
[/quote]

Thank you for saying that :)
```

---
## \#14 Posted by: pshaw Posted at: 2018-01-04T15:22:34.472Z Reads: 223

```
I’d def be down. Any time frame my dude? :)
```

---
## \#15 Posted by: longhairedboy Posted at: 2018-01-04T15:28:24.616Z Reads: 229

```
[quote="squishy654, post:10, topic:42746, full:true"]
Hey guys he has a point these batteries can explode at any point in time **unless you're running a properly built pack with a known good battery management system** you really should be careful like when you're riding **with exposed cells** it carrying it **with exposed cells** storing it **below proper discharge levels because you didn't use a BMS** charging it **after over discharging it because you didn't have a BMS** not using it **with a BMS** letting it sit if it's plugged-in **without a BMS** if it's not plugged-in **with a BMS** if it's a Tuesday **without a BMS** ..stay frosty..
[/quote]

T,FTFY

stay charged.
```

---
## \#16 Posted by: Deckoz Posted at: 2018-01-04T15:31:33.376Z Reads: 230

```
[quote="barajabali, post:13, topic:42746"]
Thank you for saying that :slight_smile:
[/quote]

Yea...

One thing to note about the "over discharging" one

This only applies to two things
-damaged cells
-discharging under heavy load(more then the pack is rated for, or an old cell with high IR that can no longer produce it's rated current and now generates heat at high current draws)

While over discharging at a low wattage load such as a 12v auto/car bulb under 50W on a NOT DAMAGED cell that is dying due to high internal resistance, is a safe way to completely discharge a cell for recycling/disposal

If it's 18650 - discharge and recycle as individual cells

If it's lipo pack - discharge to 0v, cut the positive and negative terminals and twist together to make inert and throw in trash

If it's a lipo cell by itself - discharge to 0v and then puncture the cell through to ensure the layers are shorted and inert then toss in trash

If it's a lipo cell or pack, that cannot be safely discharged,go-to a fire safe area OUTSIDE(concrete/asphalt), put a nail on a fiberglass rake handle and puncture it, let it burn off and cool then toss in trash


If you read anything about saltwater and lithium packs, it's wrong, all it does is corrode the leads off leaving a charged pack, the only way to use salt water is on packs that have preexisting punctures. As manually puncturing a pack will...well you know ;)
```

---
## \#17 Posted by: longhairedboy Posted at: 2018-01-04T15:35:42.770Z Reads: 219

```
i'll know more when the PCBs arrive and the rest of the components come in from Mouser. Also i'm busy finishing up the first Carvon EVO prototype off my bench so.. i'm not saying it will be a while.. but it might be a minute. That board needs to be finished this week, and its thursday already. 

And i've got a steady stream of business coming in. And i'm probably going to start writing for a magazine soon, and i've got my own youtube show i've been toying with in my head that needs to happen, and i'm writing a book. And i've got to test these BMSs and remotes, and i want to build a board on 76mm kegel cored wheels i found... and i just bought a 12th scale RC buggy to try and rig up a low angle follow cam...
```

---
## \#18 Posted by: pshaw Posted at: 2018-01-04T15:45:19.110Z Reads: 214

```
Cool. Well anyone got a link to a nice looking mountable xt90 port to add to the side of my enclosure?

Also does a super clean looking flat back xt90 loop key exist?
```

---
## \#19 Posted by: Deckoz Posted at: 2018-01-04T15:59:08.991Z Reads: 218

```
@pshaw Get @SORRENTINO to print you one out of ABS, we'll acetone smooth it and paint it matte, use a black male xt90, then rit dye the yellow antispark side black...
```

---
## \#20 Posted by: mmaner Posted at: 2018-01-04T16:32:22.092Z Reads: 229

```
[quote="pshaw, post:18, topic:42746"]
anyone got a link to a nice looking mountable xt90 port
[/quote]

http://www.electric-skateboard.builders/t/3d-printables-for-eskate/23199
```

---
## \#21 Posted by: PXSS Posted at: 2018-01-04T16:32:24.671Z Reads: 221

```
I suggest against using knock off xt-90s. 
I measured the resistance in a real one vs several off brand and the off brands always had 50% to up to 200% higher resistance
```

---
## \#22 Posted by: squishy654 Posted at: 2018-01-04T16:39:23.102Z Reads: 227

```
@pshaw I used a 3d printed xt90 socket holder for making a clean key, here it is on the side of the battery box.....found the model on the interwebs and James Curtis printed it for me. they are handy to have, print a few.....Yes..I know, it needs some Abec11 97mm reflex.. <img src="/uploads/db1493/original/3X/9/3/9351948a8b240be429f816b602ca02e9c39886cb.jpg" width="667" height="500">
```

---
## \#23 Posted by: scepterr Posted at: 2018-01-04T16:53:10.523Z Reads: 220

```
I can send you of one those @mmaner panel mounts if you want
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/3001?u=scepterr
```

---
## \#24 Posted by: pennyboard Posted at: 2018-01-04T18:41:35.970Z Reads: 220

```
Try one of these switches. It costs $5 at Lowe’s, easy to mount, and I’ve been running 100 Amps at 12s on it for over a year with no problems. 

<img src="/uploads/db1493/original/3X/e/3/e32637443bb76e39ec2188ec23dae2833f8496df.jpg" width="281" height="499">
```

---
## \#25 Posted by: Acido Posted at: 2018-01-04T19:39:43.241Z Reads: 207

```
Where did battery disposal thingies went? Hahah
```

---
## \#26 Posted by: 4go10 Posted at: 2018-01-04T20:02:15.167Z Reads: 208

```
As far as the control mode you described when you just kick push and the vesc keeps up the speed its already a thing. Ackmaniac's modded firmware has it. Its called PID controlled mode and you can still use the remote for breaks. :)
```

---
## \#27 Posted by: Deckoz Posted at: 2018-01-04T20:06:56.439Z Reads: 213

```
[quote="Acido, post:25, topic:42746"]
battery disposal thingies went?
[/quote]

? It's still there? I don't understand your question

http://www.electric-skateboard.builders/t/rant-our-current-gear-sucks/42746/16?u=deckoz
```

---
## \#28 Posted by: LAVAMAN Posted at: 2018-01-05T20:17:29.195Z Reads: 193

```
Do you make these (3D print) or do you purchase these? Also, what is good XT90 (name brand) vs off brand? Which brand is the good one? I would like a couple of the panel mounts for my next build. I can purchase if you wish.
```

---
## \#29 Posted by: scepterr Posted at: 2018-01-05T20:34:32.689Z Reads: 193

```
Giving them away 😋
https://www.electric-skateboard.builders/t/freebies-in-progress/42391/193
```

---
## \#30 Posted by: LAVAMAN Posted at: 2018-01-05T20:49:24.534Z Reads: 192

```
I want a couple. Just let me know when they are available and I will cover the shipping.

Thanks!
```

---
## \#31 Posted by: LAVAMAN Posted at: 2018-01-05T20:51:17.396Z Reads: 186

```
Which is the name brand XT90 (good) vs off brand (bad)? Point me to the good one.
```

---
## \#32 Posted by: PXSS Posted at: 2018-01-05T22:26:25.824Z Reads: 180

```
Amass is the real brand
```

---
## \#33 Posted by: squishy654 Posted at: 2018-01-08T18:25:30.386Z Reads: 168

```
[quote="PXSS, post:32, topic:42746"]
Amass
[/quote]
huh??  The XT60 connector is a high-current, low-resistance battery connector sold and developed by Hong Kong-based Hextronik, Ltd., the parent company of internet retailer HobbyKing.
```

---
## \#34 Posted by: PXSS Posted at: 2018-01-08T20:17:01.377Z Reads: 162

```
Sure it is! Loool. 
Amass actually holds a patent on it. 

Hobbyking states on their "genuine" connectors that they are manufactured by amass.
```

---
## \#36 Posted by: Deckoz Posted at: 2018-01-17T02:52:09.549Z Reads: 147

```
Is there for real an audio advertisement here ^^^^^ lol?
```

---
## \#37 Posted by: squishy654 Posted at: 2018-01-17T02:54:20.531Z Reads: 149

```
It's a podcast and I talked about our gear and it's sucking
```

---
## \#38 Posted by: michichopf Posted at: 2018-01-17T13:41:14.023Z Reads: 136

```
Well, you lost me at the sector 9 comment :sweat_smile:

- :"There is like sector 9 decks, and then there are decks that are racing down maryhill and there is a big difference between the two"

Well:
- In the event at Maryhill, sector 9 is heavily involved and helps out tremendously  [Wupsy daisy.](https://www.google.ch/search?ei=dU9fWr6jJ4SSU9i5m4AD&q=sector+9+maryhill+&oq=sector+9+maryhill+&gs_l=psy-ab.3..33i160k1.110187.110187.0.110422.1.1.0.0.0.0.108.108.0j1.1.0....0...1c.1.64.psy-ab..0.1.107....0.d5G-aezxtqQ)

- They have downhill race boards that are ridden and won with in wold cup races [Wupsy daisy 2](https://www.muirskate.com/longboard/decks/72064/sector-9-downhill-division-louis-pilloni-pro-model-longboard-skateboard-deck-w-grip)

- And they were a huge contributer to the whole rising of downhill long-boarding. To this day, they organise [events (IDF world cups)](https://www.youtube.com/watch?v=L7JLhEmsl6M), cover costs of safety staff, road closures and medics as well as safety nets etc. And are allways happy to give you a lift back up in a truck/car.

So I don't think it is fair to put them in such a small box based upon their products that are catered towards the masses. Even easier to grasp since in almost any online shops they are split in 2 category, Sector 9 and sector 9 downhill division.......

Generally enjoyed the talk during a boring morning in the office, don't want to be the guy who goes around nit picking stuff that isn't quite accurate (same trucks front and back make no sense, "donwhill and parking garage in the same breath instead of free-riding/bombing, etc. )  . Thought since you said you enjoy discourse so much I would reply with a single reaction to it :slight_smile:
 
Admire your drive and ambitions dude. 

Ps: I think that he problem is lack of experience, wrong priorities and missing of so called ultimate experiences. We have amazing performance stuff in the free-ride/downhill world, from trucks, to bushings, to wedges, baseplates, griptape, foot stoopers, decks and so much knowledge and experience. And I think a lot gets lost in translation to esk8. To me The deck, trucks and bushing are the beating heart of any skate, if it is gravity or esk8. Dismissing that simply as other components will diminish any quality ride and experience you might have on your build.
```

---
## \#39 Posted by: stormboard1 Posted at: 2018-01-17T13:55:17.542Z Reads: 123

```
Hes right on the need for innovation part...it’ll come with time but things like the cleaner loop key,the Black xt90s aren’t xt90s tho I thought? An integrated enclosure deck is needed at a decent price too and a VESC that doesn’t blow so easy and not have a 4/500% markup...just my 2cents not a rant  lol
```

---
## \#40 Posted by: Acido Posted at: 2018-01-17T13:58:13.206Z Reads: 125

```
Why to make a short at your battery? When you can just dump it in the can, i didn't read a thing about disposing batteries tho
```

---
## \#42 Posted by: Deckoz Posted at: 2018-01-17T15:27:29.021Z Reads: 125

```
[quote="squishy654, post:41, topic:42746"]
pros in downhill races are the exact same boards
[/quote]

This is partial truth... Example Evo vs carbon Evo... Even if you get a carbon it's not hand made like the original carbon evos. Every skate company has different lines or boards.. cruisers, dh, Freeride, etc. Can't clump the entire lineup into it's a wooden stick with trucks so they're all in the same. :/

Anyway

[quote="Acido, post:40, topic:42746, full:true"]
Why to make a short at your battery? When you can just dump it in the can, i didn’t read a thing about disposing batteries tho
[/quote]

Hey if you want to improperly dispose of lithium by "just dumping in the can" be my guest. But there's proper ways to prepare a battery before tossing in the can, if you don't follow them and your trash or trash collection truck catches fire because you didn't properly discharge and make inert by shorting that's on you man.. lol

[quote="Deckoz, post:16, topic:42746"]
If it’s 18650 - discharge and recycle as individual cells

If it’s lipo pack - discharge to 0v, cut the positive and negative terminals and twist together to make inert and throw in trash

If it’s a lipo cell by itself - discharge to 0v and then puncture the cell through to ensure the layers are shorted and inert then toss in trash

If it’s a lipo cell or pack, that cannot be safely discharged,go-to a fire safe area OUTSIDE(concrete/asphalt), put a nail on a fiberglass rake handle and puncture it, let it burn off and cool then toss in trash

If you read anything about saltwater and lithium packs, it’s wrong, all it does is corrode the leads off leaving a charged pack, the only way to use salt water is on packs that have preexisting punctures. As manually puncturing a pack will…well you know :wink:
[/quote]

The reason for shorting the cells is it makes them inert. In other words after they have been discharged and shorted they will no longer accept a charge. Shorting dimishes the energy density to near zero capacity. The cathode and anode surface are ruined. Meaning you've done your job. And even if someone pulls it out of the trash and tries to use it there is little risk of a fire being caused.

Lithium ion and lithium type cylindrical and non pouch cells should be recycled..not tossed in the trash. Recycling centers provided isolation bags for cells like this. Recycling centers do not recycle pouch cells(lipo)
```

---
## \#43 Posted by: michichopf Posted at: 2018-01-17T15:43:14.692Z Reads: 116

```
Having met them and ridden with them actually it is EXACTLY what they are riding. Having your own pro model is sick as fuq. Two of the sector 9 team-riders rock their models. 

And generally you think to highly of so called prototype high cost boards. Yeah there are riders rocking 1k + decks. But the big majority of IDF riders stay with standard Rayne, Powel peralta, Original, Olson¬Heckmati or anny other given brand. It is the rider that makes the set up work not the other way around. We are mostly not that strong in the money department. Quite a few don't even run with precision trucks cuz of money. All our money goes into traveling to the events, wheels and hostels to stay. Its a small family with not too much ways of living off of it. 

The Idea that the top 50 riders in the world are some sort of super athletes with contracts sponsoring and an endless amount of deck and trucks choices is a pipedream.

So yes, we ride the EXACT same board you buy in a shop and no I am not nuts. I am part of this amazing friendly and open group, where we don't talk how good something is or how amazing I am but we show how much love and appreciation we have for the sport and each other. 

Mayby let a downhiller talk about downhill. Mayby let an innovator talk about innovation. Mayby don't asume that, "research" how ever you define that word in your perspective, is equal to blood sweat and hard earned experience by many.

I mean I tried to inform you on a point super friendly, Instead of accepting or acknowledging any of that information you disregarded it instantly as nuts..... Serious question, not hateful but out of curiosity: Do you really think you know that much ? that you have such an insane grip on any facet of this sport, that it allows you to view any other input than yours inferior ? I have not seen you on any international events nor on any rankings. Yet apparently I know nothing and I am nuts, meanwhile you, you holy entity of all wisdom mister @squishy654 is our compass for all orientation. Our moderator of any discourse, the epitome of human thought ?!

We are a loving [family](https://www.youtube.com/watch?v=hLsIZ9zByVY), we accept everyone of all skill levels, skin color, sexual orientation or nationality. The only thing we don't accept is talking out of ones ass and disregarding other ideal and ideas. Respect of others is a necessity on the course. Otherwise people would get hurt badly.
```

---
## \#44 Posted by: squishy654 Posted at: 2018-01-17T15:45:48.724Z Reads: 98

```
Wow a fine display of that respect to go along with it too.. I think you're reading a lot more into what I'm saying then what I'm actually saying
```

---
## \#46 Posted by: Acido Posted at: 2018-01-17T16:17:16.715Z Reads: 95

```
I didnt read about it but it just feels weird to short the battery to me especially when disposing  :D
```

---
## \#47 Posted by: squishy654 Posted at: 2018-01-17T16:19:05.808Z Reads: 93

```
I put the old batteries in a bucket of salt water and let them sit for a day or more, once the bubbles stop it's safe to dispose of. It's basically shorting it yup..
```

---
## \#48 Posted by: Deckoz Posted at: 2018-01-17T16:20:41.118Z Reads: 91

```
The first time you get laid feels weird to. But then it seems natural. 

:)
```

---
## \#49 Posted by: Deckoz Posted at: 2018-01-17T16:22:01.198Z Reads: 92

```
[quote="squishy654, post:47, topic:42746"]
put the old batteries in a bucket of salt water and let them sit for a day or more, once the bubbles stop it’s safe to dispose of. It’s basically shorting it yup…
[/quote]

No just no lol electrolysis dude..

[quote="Deckoz, post:16, topic:42746"]
If you read anything about saltwater and lithium packs, it’s wrong, all it does is corrode the leads off leaving a charged pack, the only way to use salt water is on packs that have preexisting punctures. As manually puncturing a pack will…well you know :wink:
[/quote]
```

---
## \#50 Posted by: Acido Posted at: 2018-01-17T16:22:02.854Z Reads: 98

```
I would chop them with an axe, more fun and there's fire which is cool
```

---
## \#51 Posted by: squishy654 Posted at: 2018-01-17T16:24:02.928Z Reads: 98

```
lol..here's a fun way to dispose of a lipo...
https://www.youtube.com/watch?v=yzBFCufUDq0
```

---
## \#52 Posted by: The_Bob Posted at: 2018-01-17T16:24:56.061Z Reads: 99

```
Ya know what would be cool, a push push switch that worked sort of like an xt-90s

It first contacts a resistor, then the real current, then stays in place.
```

---
## \#53 Posted by: Chewie Posted at: 2018-01-17T16:37:16.538Z Reads: 99

```
Yup, this is my favorite way, it 100% ensures that it's inert before going in the garbage.
```

---
## \#54 Posted by: squishy654 Posted at: 2018-01-17T16:47:13.805Z Reads: 93

```
There are "battery switches" and something called Ignition Protection rated devices I wonder if any of them work the way you describe, it would appear many are just sealed, keeping the spark away from fumes...but eliminating the spark is in their best interest as well and I bet someone has made one somewhere..you could modify an existing battery switch as well with the resistor getting contact just before the rotary hits the main contact.
http://shop.pkys.com/Ignition-Protection_ep_43.html
```

---
## \#55 Posted by: Sender Posted at: 2018-01-17T17:01:04.635Z Reads: 92

```
@squishy654 Why does it seem like it is always you that gets into arguments on here?  You always take the opinion it is always some personal attack.  I feel like it is about time to turn the magnifying glass inward to try and understand why you get so much flack.  No hate, just saying, you seem like one of the major themes of "angst" in this forum. Continuously. People don't like "know it all's." Especially when they make definitive claims with no backing. Deuces.
```

---
## \#56 Posted by: Lukas Posted at: 2018-01-17T17:03:43.545Z Reads: 96

```
*cough*

[quote="squishy654, post:45, topic:42746, full:true"]
If your a pro downhill guy into electrics we should get you on that podcast so you can talk and teach instead of just attacking people’s character or opinions in the forums.
[/quote]


https://www.electric-skateboard.builders/t/riding-tipps-introduction-to-high-speed-skating/19006

Edit: to clarify: in my opinion he is @michichopf is a great contributer to this forum and i'm glad he is sharing his knowledge with us. You on the other side are way more demanding than giving back.
```

---
## \#57 Posted by: michichopf Posted at: 2018-01-17T17:13:21.629Z Reads: 94

```
I don't think I am reading anything into it. You made a statement on the podcast that is wrong and I didn't agree with. Came here and voiced my opinion and gave facts  and arguments to support it. You then proceeded to dismiss all that altogether and stating that holding an understanding about the subject like mine was "nuts" and misinformed. 

- I shall be summary: Without participation in the sport or the competition, you dismissed my input I thought was solid information, re-used and reworded the same argument that was proven false prior and accused the thinking of using standard decks in competitions as nuts/crazy. 

- I then simply followed up with a further explanation tho why I said what I said and to why your reaction should not have left your thoughts. Since you based your strong opinion about my post not in facts but rather a gut feeling or  pseudo-knowledge. 

- I thought since you often say that you enjoy discourse I could hold one with you, but usually a discussion is an open talk, based upon arguments and facts. Usually there are different fields of expertise withing the discussion group to give more information about a certain subject. Mostly people respect ones own limitations and welcome critic about their statement since correction is the fastest way to improvement.

- And most importantly, in a discussion you attack arguments or opinions masked as arguments, not people. That is basically how discussions work and since you apparently enjoy them so much I am flustered that you misunderstood. In my field a discussion is an intellectual battle, warfare based upon knowledge with a clear result and not just differing opinions. 

[quote="squishy654, post:45, topic:42746"]
instead of just attacking people’s character or opinions
[/quote]

- Ideas are there to be ridiculed, that how human growth works. I corrected a statement rather detailed. Instead of bearing an open mind and learning something you presumed to know it based on ?? feelings ?? and are then surprised when you get called out again ? That is how adult interaction works.

Wrote this so many times to you already, I guess I shall try again and again:
I admire your energy and drive. I like how involved you have become. Don't confuse opinions with facts and never presume you are the smartes guy in the room, since that will negate every learning possible. Talk about what you know, what you experienced what you are a part off. Don't force ideas on others and most importantly be humble in your approach. Don't presume anything, go out there and learn from others.

Over and out

(still not a single hard feeling over here, but this is how we normally conduct proper discourse)
```

---
## \#60 Posted by: squishy654 Posted at: 2018-01-17T17:27:50.925Z Reads: 78

```
Sorry I said anything actually..I'll just delete my comments..
```

---
## \#61 Posted by: michichopf Posted at: 2018-01-17T17:28:24.647Z Reads: 85

```
[quote="squishy654, post:58, topic:42746"]
I’m not up in here blowing smoke, trashing companies
[/quote]

Well you kinda did. Imagine working at sector 9, or being a pro rider. Thinking about joining esk8 and stumbling upon your podcast. How nice would that make them feel to hear:"There is like sector 9 decks, and then there are decks that are racing down maryhill and there is a big difference between the two”

Having produced multiple world champions, having people rock their stock boards and wheel in the upper echelon of downhill, being a big contributor in the sport always helping out smaller events ?

This is what rubs people on here the wrong way. Such a statement cannot be made publicly just because you felt like it or you presume  to know it all. This is basically slandering one of the OG donwhill brands.

Then you were given the easy out by saying:" Dang man that is wicked, didn't know the were so involved and thanks for the input on racing gear within the circus" But you chose like every other time confrontation, belittling others and not even trying to change your way of thinking about it even when faced with the music.....
```

---
## \#62 Posted by: michichopf Posted at: 2018-01-17T17:30:01.647Z Reads: 82

```
https://www.urbandictionary.com/tags.php?tag=u%20lost%20me%20there

https://dictionary.cambridge.org/de/worterbuch/englisch/dismiss


No sir, I didn't. That is not the same and will never be. You cannot change definitions of words to suit your argument. Not happening.
```

---
## \#63 Posted by: squishy654 Posted at: 2018-01-17T17:32:54.634Z Reads: 80

```
The funny part is you think I'm arguing with you...lol

Sorry I ever muttered the phrase sector9, it will never happen again..it popped up because they are the largest factory of longboards, something people may know or understand, it was not meant for you, I could have use any major longboard brand as an example...if you don't understand what I was saying how can you argue with it? I have told you now, this is the third time, that is not what I was saying, the point was about gear and how pros racing use much better gear than even is sold to the public..by ANY BRAND, take it or leave it..
```

---
## \#64 Posted by: squishy654 Posted at: 2018-01-17T17:35:14.432Z Reads: 81

```
Stop putting words in my mouth or characterizing what I said to suit your need to attack my character in front of the audience...I think they understood what I said better than you because they lack this insider "I know it all" bias that makes you hear things the laymen wouldn't...and like I said, I'll be sure to never mention sector9 again..if that's your problem with my point..
```

---
## \#65 Posted by: Deckoz Posted at: 2018-01-17T17:44:20.202Z Reads: 82

```
Lol the greatest part about this is **I had nothing to do with it.** Look @JohnnyMeduse it's not my fault this time  

And it's not on Facebook and you can only delete your own replies..not the entire thread 🤣🤣🤣🤣🤣🤣🤣
```

---
## \#66 Posted by: stormboard1 Posted at: 2018-01-17T17:47:12.231Z Reads: 83

```
If ya say something either stand by it or say sorry and stfu
```

---
## \#67 Posted by: JohnnyMeduse Posted at: 2018-01-17T17:47:25.672Z Reads: 84

```
Someone summon the Wizard...

Because

https://m.youtube.com/watch?sts=17544&utcoffset=-300&v=Fi6Ddd6eRqM&has_verified=1&client=mv-google&layout=mobile
```

---
## \#68 Posted by: Deckoz Posted at: 2018-01-17T17:48:29.729Z Reads: 83

```
Hahaha man he's funny. His best is the happy birthday song from the league

https://youtu.be/zuVsLR_2GX0
```

---
## \#69 Posted by: stormboard1 Posted at: 2018-01-17T17:59:25.207Z Reads: 80

```
😂😂😂😂 most awquard few minutes but couldn’t stop laughing
```

---
## \#70 Posted by: benjammin Posted at: 2018-01-17T18:00:02.330Z Reads: 78

```
Dude, what happened to the podcast?
```

---
## \#71 Posted by: squishy654 Posted at: 2018-01-17T18:08:50.342Z Reads: 78

```
I deleted it.. simple as that, I don't have time to fend off attacks or straighten out misunderstanding when people are looking to cause it, over and over again..sector9 was just added to my shitlist too, lol, they are like the walmart of longboards, lol
```

---
## \#72 Posted by: benjammin Posted at: 2018-01-17T18:14:50.025Z Reads: 80

```
Was just gonna listen to the rest of it.

? My favorite board I have is a Sector9 :neutral_face:
```

---
## \#73 Posted by: michichopf Posted at: 2018-01-17T18:32:38.828Z Reads: 82

```
Thats how I understood a dialogue.

- You can delete a post if you can no longer stand by what you said or you changed your opinion (should concern you and make you look inwards)

- You can delete a post that was made in the heat of the moment and you went overboard (again should you make look inwards)

- You can delete a post if the content is obsolete or wrong (also should make you rethink and look inwards)

- Or you HAVE to delete the post since you cannot stand by it or you cannot handle the following discussion sparked by your brainfart.

Oh well, I guess I should chill a bit and not actually go into a discussion mindset. Doing memes and banter seems easier apparently.....

Since all I wanted was an adult conversation, no Idea how people get offended or think it is an attack. None should give a shit about feelings in a discussion only care about facts. Ah well, going to relax with an actual [Debate](https://www.youtube.com/watch?v=Qb1-F_UEtS4)
```

---
## \#74 Posted by: squishy654 Posted at: 2018-01-17T18:41:08.426Z Reads: 80

```
My 1st longboard was a sector9...I think most people have one if they have multiple longboards..that's why they popped in my head as an example, they are the most prolific longboard on the market and everyone knows them when I mention them, a brand or name the most number of my audience could relate too, but a fanboi took offense to the premise that pro riders do not ride store bought cruisers..thinking I was ignorant because some sector9 pros ride the factory decks...an exception to a generalization can always be found, I am not ignorant of this fact, but the continued pattern of intent of this person is my main concern, they are on a mission to discredit and put me down publicly, here and in other threads so misunderstanding what I said and repackaging it for this audience is in his best interest.. I posted it on redit and facebook, find it there..

I delete my posts to reduce the number of targets for these particular people, to spare the community, not to hide what I said, I stand by everything I said and I would say it again. I just feel it's not needed here..I understand my deleting of comments can also be misconstrued by those same people and it will..that's par for the course for a troll..
```

---
## \#75 Posted by: squishy654 Posted at: 2018-01-17T18:42:11.223Z Reads: 74

```
Your version of an  adult conversation is sort of slimy and I have no desire to debate or speak to you...you are extremely transparent to me..
```

---
## \#76 Posted by: Deckoz Posted at: 2018-01-17T18:47:54.298Z Reads: 73

```
But humans are opaque 🤣😂 especially adult humans.
```

---
## \#77 Posted by: squishy654 Posted at: 2018-01-17T18:48:02.725Z Reads: 73

```
I have an idea, I'll post the podcast in it's very own thread just for comments and criticisms so you can pile it all on...like? that way we can at least contain it, lol..
```

---
## \#78 Posted by: squishy654 Posted at: 2018-01-17T18:50:07.707Z Reads: 78

```
http://www.electric-skateboard.builders/t/omg-i-did-a-podcast/43967
```

---
## \#79 Posted by: ATLesk8 Posted at: 2018-01-17T19:20:37.606Z Reads: 75

```
[quote="squishy654, post:75, topic:42746, full:true"]
Your version of an  adult conversation is sort of slimy and I have no desire to debate or speak to you…you are extremely transparent to me…
[/quote]
 Then why keep on about it?
```

---
## \#80 Posted by: Sapphirinia Posted at: 2018-01-18T04:27:41.474Z Reads: 64

```
Maybe that would work with my co2 powered Bb gun 😀
```

---
