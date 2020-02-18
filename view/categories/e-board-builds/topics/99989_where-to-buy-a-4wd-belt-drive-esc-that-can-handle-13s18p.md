# Where to buy a 4wd belt drive esc that can handle 13s18p?

### Replies: 46 Views: 538

## \#1 Posted by: Dog Posted at: 2019-08-09T09:49:18.228Z Reads: 168

```
Building a awd 13s18p setup, where to buy a VESC for 4 belt motors? 

Suggestions to reconsider for a 2wd are not welcomed ;)
```

---
## \#2 Posted by: Anubis Posted at: 2019-08-09T10:22:10.861Z Reads: 166

```
3p? 4wd would be entirely pointless. No point having a battery capable of at max 3200W (Less for most of the ride) then fitting it out with 10000W+ worth of motors, not to mention the massive cost increase (4 vescs, 4 mounts, 4 motors, 4 pulley sets, 4 belts which all snap...) and massive weight increases. If you're going 4wd, you need at least 8P+ or its just bottlenecked as fuck.

As for a 4WD esc, pretty much any VESC can do 4wd over split PPM or can.
```

---
## \#3 Posted by: glyphiks Posted at: 2019-08-09T10:28:55.197Z Reads: 163

```
13s3p 4wd 🤣🤣🤣🤣🤦‍♂️
```

---
## \#4 Posted by: Dog Posted at: 2019-08-09T10:38:03.487Z Reads: 161

```
It’s actually 13s3p times 6 thank you very much. 

Could you send me a link to the vesc you’re talking about and how to tune it for 4 sets of belt motors?
```

---
## \#5 Posted by: visnu777 Posted at: 2019-08-09T10:43:39.891Z Reads: 161

```
Get two Unitys or 4 Trampa VESC 6 or 2 Flipsky FSESC 6.6 dual (mini). They all can do 4wd
```

---
## \#6 Posted by: Dog Posted at: 2019-08-09T10:45:59.092Z Reads: 156

```
Would it be a plug and play type of esc or I need a manual? 
Also, is there a way to extend the wires that connect the two esc on the ones you mentioned? (I’m assuming the awd setup will be two sets of dual hub esc connected in some way)
```

---
## \#7 Posted by: glyphiks Posted at: 2019-08-09T10:57:55.391Z Reads: 152

```
Wow. 234 cells is a lot of cells dude... like nearly 100 more cells than some of the biggest batteries going around. Search around here for the terms '4wd' 'can vs ppm' 'vesc' 

The questions you are asking have been asked before.
```

---
## \#8 Posted by: Dog Posted at: 2019-08-09T11:03:43.625Z Reads: 153

```
Yea it’s a huge project. 

Tried looking around the forum but couldn’t find an answer to my 13s question, every other build is 12s max. 

Besides, the board I’m installing it on is longer than usual so I would need to extend the connecting wires between the esc’s and I had a load of questions besides the obvious ones. 

There’s lots of general chit chat on the forums and I can’t read all of it to answer a simple question that I would rather ask.

Sorry if a repetitive question annoyed you that you had to direct me to the search bar, you can just ignore it and move on.
```

---
## \#9 Posted by: Komamtb Posted at: 2019-08-09T11:12:10.082Z Reads: 140

```
Will you be making the battery yourself?
```

---
## \#10 Posted by: Dog Posted at: 2019-08-09T11:13:44.995Z Reads: 137

```
No, I have 13s3p battery packs with bms installed.

Gonna be installing them on the 6’6 Hamboards Classic using the liftboard motors mounted on the trucks.
```

---
## \#11 Posted by: JoelMatousek Posted at: 2019-08-09T11:58:52.232Z Reads: 132

```
Are you building a car? This board would be able to run for days!
```

---
## \#12 Posted by: Dog Posted at: 2019-08-09T12:02:50.308Z Reads: 131

```
I live in Venice beach and it has a very scenic and long bike path and boardwalk that I basically live on, and I love my hamboard so I always wanted to motorize it without having range anxiety and be able to skate for 4-5 hours straight if I wanted to. 

Or just skate 15 miles to downtown and back on a motorized electric concrete surfboard.
```

---
## \#13 Posted by: Anubis Posted at: 2019-08-09T12:16:39.533Z Reads: 126

```
Liftboard motors? Again, kind of pointless then. You're motors are the main bottleneck. I'd suggest you sell 2 of the 13S packs and all 4 motors and get 2 better motors and go 2WD.

6P in street is like 40+ miles of range. You won't get range anxiety unless you're actually doing 80 miles in a day.
```

---
## \#14 Posted by: Dog Posted at: 2019-08-09T12:24:20.022Z Reads: 123

```
as per original post, suggestions to convert to 2wd are really not welcomed because every damn time I ask this question, nobody answers properly and always suggesting something completely different.
Is it hard to just answer the question without including your two cents?

I have battery packs to spare, I have motors mounted on trucks laying around, I have a big fucking skateboard where I can fit 6 of the packs without breaking a sweat.

Is it hard to just point me where I intend to go? I don’t want to be buying anything else besides a VESC that can handle 13s18p and 4 belt motors.
```

---
## \#15 Posted by: Giga Posted at: 2019-08-09T12:33:22.455Z Reads: 120

```
Did you made any calculations or did you just come up with big numbers?
13S18P is (depending on the cells) >2kWh, with 25R a bit less, with 35E bit more, with 30Q and VTC6 pretty much 2.5kWh. 

So assuming your AWD will use around 20Wh/km (which might be in real world conditions more like 10-15Wh/km; my 2WD 9" MTB uses around <20Wh/km on road) you get around 130km (in your units: 65000 bathtubes, around 3.25mio apples or 81miles). Calculating more realistic would end up somewhere around 200-300km (>150miles)
Also at around 50gr. per cell, alone the cells will weight over 11kg (not including BMS + cables + ...)

Maybe you should plan your project a little bit more. Go to the grocery store and get 15kg of water and put it onto your board, then you get a feeling what alone the battery will feel like. Not talking about motors and remaining electronics which will be around the same weight for 4wd.

Still to answer your question: 
13S are proven to work on the VESC6, when avoiding high breaking currents. Still I would not feel safe riding between cars when all ESCs got a safety margin of less than 10%. Which breaks down to your brakes got a safety margin of less than 10%.
So to really be on the safe side try something like the [A200S](http://teamtriforceuk.com/a200s-v2-1/) or the [VESC75/300](https://www.trampaboards.com/single-vesc-75v-300a-in-cnc-t6-silicone-sealed-aluminum-box--the-most-powerful-vedder-electronic-speed-controller-ever-p-26284.html)

Still they are single motor ESCs, so you will need 4 of them...ending up somewhere >1700€

So if I was you, I'd go for 12S battery and some dual vesc6... dual drive :face_with_hand_over_mouth:
```

---
## \#16 Posted by: Dog Posted at: 2019-08-09T12:41:14.459Z Reads: 115

```
This fucking forum, I swear to god. It’s like listening to opinions before getting an answer is a form of payment and everyone is a debt collector.

Yes, I am not a moron, yes I did my calculations right and weighted everything because everything except the vescs are literally in front of me at all times, yes I know how heavy the whole thing will be, I’m used to the weight. Yes, I still want it because I do not ride this boat on the streets with cars, I mentioned that I live in Venice beach which has a long bike bath on the sand.

Thank you for your answer tho, I’ll look into the vesc6.
```

---
## \#17 Posted by: Randy_bobandy Posted at: 2019-08-09T13:16:44.073Z Reads: 109

```
I would get 2 flipsky fsesc 6. Make sure its the newest version since the older one is not only way bigger but doesn't have a canbus so it won't do 4wd. Also they are decent priced for a vesc that can do 60v and 200amp.
```

---
## \#18 Posted by: xsynatic Posted at: 2019-08-09T13:17:30.125Z Reads: 106

```
I mean they just want to help and maybe even prevent some wasted money but ffs just answer the god damn question. If he wants to build 13s80p and he did the math so be it :D
```

---
## \#19 Posted by: Skunk Posted at: 2019-08-09T13:27:46.249Z Reads: 106

```
Lol i love people like this. 

No such thing as a 4wd esc/vesc. You just hook up 4 singles or 2 duals.
Minutes of reading would answer this. 
No they are not plug and play. Especially not at 13s nothing will be.
If you don't want suggestions from the community, then don't ask it for help.
You act as if you're entitled to the answers to your questions...
```

---
## \#20 Posted by: Randy_bobandy Posted at: 2019-08-09T13:29:05.568Z Reads: 108

```
The dual flipsky vesc 6.6 is $280 so $560 total.
Flipsky recently released a high amperage vesc 6. It is a single vesc so you would need 4 total but they are a wopping 60v(13s is 54.6v max so you are good there) 200amps each! That would be 800amps of continuous power total! That's a potential 43,000w of power! Or 57hp!
```

---
## \#21 Posted by: Dog Posted at: 2019-08-09T13:46:09.578Z Reads: 102

```
Thank you for the answers! I’ll order a Flipsky, I’ll email them directly to make sure. 

Will report with pictures and videos soon! 
The motors are 900w each so 3600w but I will go 60% speed max, don’t need to be fast on this monstrosity. 

The board is 6’6 (198cm) and 35lb (16kg) so with the 6 packs at 5.5lb each, ~2lb for vescs and wires, 15lbs for wooden enclosure/riser Liftboard style (google the setup) plus maybe 11lbs for trucks and motors comes to about 85-90 lb board (around 41kg)

Doable. I weigh about 210lb so with the board it’s about 300lbs (142kg) of total weight distributed on the trucks, the board being stiff as possible of course. In realms of possibility.

Will result in a cool looking motorized surfboard on wheels.
```

---
## \#22 Posted by: Skunk Posted at: 2019-08-09T13:49:44.497Z Reads: 96

```
13s isn't common, like at all.  Only people i know running it are running trampa vesc or enertion unitys. 
Flipsky has been stepping it up but idk about them at 13s. 
The new maytech is a beef cake but 4 of them would cost a lot and they aren't small at all.

Do you know the kv of those motors? 
Thought they were 270kv.. if so you might have some issues and just blow your esc
```

---
## \#23 Posted by: Dog Posted at: 2019-08-09T13:52:06.108Z Reads: 93

```
No, no idea about the kv actually, the Liftboard website didn’t provide those specs, just the wattage. 

You’re saying the motors won’t be able to function properly and blow up the esc’s?
```

---
## \#24 Posted by: DerelictRobot Posted at: 2019-08-09T13:53:12.878Z Reads: 89

```
[quote="Dog, post:16, topic:99989"]
This fucking forum, I swear to god.
[/quote]

I mean to be fair, people are being pretty nice given that the board spec you're trying to build is obviously a bit above your skill level and you're using crap motors.  There's a reason experienced builders keep repeating themselves. Frustration that you're not hearing what you want to hear shouldn't be taken out on them. Calm thy digital tits.
```

---
## \#25 Posted by: Skunk Posted at: 2019-08-09T13:54:28.624Z Reads: 90

```
I'm pretty sure they are 270kv and if so at 13s, if you break at a full charge you'll probably blow the esc.
I wouldn't run 270kv at 12s even.  Honestly avoid over 200kv for anything 10s and above. 
270kv is good for like 6s/8s batterys
```

---
## \#26 Posted by: DerelictRobot Posted at: 2019-08-09T13:56:15.426Z Reads: 86

```
Also what's ERPM looking like at 270kv/13S?
```

---
## \#27 Posted by: Dog Posted at: 2019-08-09T13:58:12.438Z Reads: 87

```
Oh shit, ok thx for pointing the kv problem out.

I was more frustrated about people pointing out the size of the battery and how unnecesary it is and I was automatically defensive. 

Could you reccomend me hub motors that would go with the 13s18p battery and dual vesc6?
```

---
## \#28 Posted by: Dog Posted at: 2019-08-09T13:59:46.887Z Reads: 89

```
Sorry erry’one, like I said I was defensive because people are not used to see batteries this size and I was just tired and defensive about it so my bad, I calmed my digital tits as long as you don’t try to convince me to size down the battery.
```

---
## \#29 Posted by: DerelictRobot Posted at: 2019-08-09T13:59:54.603Z Reads: 90

```
Check out Hummie Hubs. They're good up to 14S iirc and are much more realistic KV.

People are not shocked at your battery size. They're shocked that you'd put that much weight and cost in cells onto this kind of hub board. You've got a freight train tanker of fuel on a Pinto, and you've already made up your mind that's what you're doing.
```

---
## \#30 Posted by: Skunk Posted at: 2019-08-09T14:00:39.434Z Reads: 91

```
[quote="Dog, post:27, topic:99989"]
Could you reccomend me hub motors
[/quote]

Only hub motors i know of people running at 13s are hummies hub motors.
My hub motor knowledge is limited tho.   Not a fan personally for my esk8 uses.
```

---
## \#31 Posted by: butt_stallion Posted at: 2019-08-09T14:02:55.484Z Reads: 91

```
If you check out the dual 6.6 discussion and findings page you can see a lot of users have had issues with the dual 6.6 having voltage cutouts and incorrect voltage values on 12s, I think it's safe to assume this would only get worse on 13s.  Even more recently they've had issues with the slave side failing completely.  Not sure how much of this has been fixed, but it sounds like you want a super reliable board so I'm not sure if you will find reliability with 13s especially with a flipsky. 
https://www.electric-skateboard.builders/t/flipsky-dual-fsesc-6-6-discussion-findings/67155?u=butt_stallion

Not to say your build will never work on 13s but for reliability you may need to invest in an ESC that can take 13s like a champ.
```

---
## \#32 Posted by: Dog Posted at: 2019-08-09T14:03:47.888Z Reads: 88

```
Oh wow, they’re unavailable online from what I’ve just gathered.

What about 13s belt motors? Would I need a different vesc setup for belts? 

On another topic, the trucks are gonna be ok at moderate speeds and bumps with 140kg on them?
```

---
## \#33 Posted by: Skunk Posted at: 2019-08-09T14:05:31.746Z Reads: 88

```
I get wanting to use what you have. 
13s is an area a lot of experienced builders still haven't tried yet. 
A little over a year ago 12s was still considered unreliable and risking your vesc blowing.
So people see someone shooting for 13s when they don't know the answer to a fairly gone over question, they feel the need to warn you.  It's not outta spite or anything.  Don't take it personally.
```

---
## \#34 Posted by: DerelictRobot Posted at: 2019-08-09T14:07:11.877Z Reads: 85

```
[quote="Dog, post:32, topic:99989"]
On another topic, the trucks are gonna be ok at moderate speeds and bumps with 140kg on them?
[/quote]

Heh. I wouldn't feel safe. 

Also keep in mind how easy it will be to slide out of control on PU wheels with that much weight. I can't imagine a battery like that not on ATs
```

---
## \#35 Posted by: Dog Posted at: 2019-08-09T14:07:51.425Z Reads: 82

```
Got it. I understand now, thank you. I have the option to go 10s12p or potentially 10s24p but aesthetically and functionally the hoard would be a bit different. 

I’ll just abandon the 13s idea for now, it was an optimistic project.
```

---
## \#36 Posted by: Skunk Posted at: 2019-08-09T14:08:00.550Z Reads: 80

```
When it comes to good esc/vesc you don't need belt or hub specific esc/vesc like you do on the cheap plug and play Ebay/diyeboard escs.

Anything 13s I'd shoot for trampa vesc or unity
```

---
## \#37 Posted by: Skunk Posted at: 2019-08-09T14:11:20.221Z Reads: 83

```
You can still make a beast at 10s awd. Probably a much more reliable one at that. 
You could even make two boards.

A heavy weight with crazy range. 
And a light weight board easy to carry in a store for quick trips. Use the liftboard motors on that.
```

---
## \#38 Posted by: DerelictRobot Posted at: 2019-08-09T14:11:39.107Z Reads: 83

```
If you intend on using PU wheels, I would suggest no more than 10S12P just for weight considerations. 

Big heavy boards handle considerably different than lighter ones. I say this as someone who has built and/or rode boards from 8kg to 20kg (heyo Nazere Lonestar). Weight matters even more when you're on PU wheels, and a 25-30kg board on PUs is going to be dangerous if you're riding it in public places.
```

---
## \#39 Posted by: Dog Posted at: 2019-08-09T14:17:11.006Z Reads: 83

```
I understand the pu weight considerations. I ride the hamboard pretty often so I am familiar with constant sliding or “drifting” of at least some wheels coz the board is about 18kg itself, besides that I am constantly powersliding on it, 4 wheels slide as a form of workout, and I recently learned how to powerslide on my boosted v2, wide 4 wheel drifts up to 180 degrees or a tighter 360 but very rare for now (I fell a few times and got neck whiplash) so I’m very much looking forward for the physics that you’re trying to warn me about. 

It’s gonna be an epic drifting awd surf/skateboard.
```

---
## \#40 Posted by: Skunk Posted at: 2019-08-09T14:23:56.520Z Reads: 83

```
If you're wanting a 4wd drift machine shoot for low kv motors. Even something like racestars 5065 150kv motors would do the trick at a good price. 
I doubt you need high speed for the boardwalk.
You'll probably get more use out of crazy acceleration and braking.
```

---
## \#41 Posted by: Dog Posted at: 2019-08-09T14:28:30.392Z Reads: 83

```
Definitely!

And 10s would be fine with them yes? 

Should I still get the expensive vescs or look for cheaper since it’s not 13s anymore?
```

---
## \#42 Posted by: Skunk Posted at: 2019-08-09T14:35:38.059Z Reads: 81

```
You could get away with the flipsky at 10s for sure.
Maybe the liftboard motors.... but it's still 70kv over what most builders would recommend as a max.
The racestars have some of the best feedback for a budget motor. They are basically what Evolve uses
```

---
## \#43 Posted by: evoheyax Posted at: 2019-08-09T15:45:02.306Z Reads: 75

```
I think your way over killing your battery still. 1500wh should be able to get you 50 miles if your not doing 30 mph to 0 back up to 30, back down to zero every block. 2600wh should be able to do like 75 miles or so. It's hard to stand on a board for that long without your legs giving out.

I think you should reconsider your battery. I run 1300wh lipo with 4wd hummie hubs. 0-30mph in 1.9 seconds. It's stupid fast and still can ride 20+ miles of thrashing on hills with stop signs everywhere and I weigh around 200lb.

My question for you is why 13s? Your just more likely to run into problems with esc's blowing up or motors blowing up. It's not necessary to get insane power outputs. So what's the point of 13s?
```

---
## \#44 Posted by: Randy_bobandy Posted at: 2019-08-09T20:04:41.175Z Reads: 62

```
Thats the old flipsky 6.6 esc. The new one is smaller and is redesigned.  Also the one you are talking about can't do 4wd like the new one can.
```

---
## \#45 Posted by: butt_stallion Posted at: 2019-08-09T20:57:08.798Z Reads: 61

```
Is the new one the 6.6 plus model?
```

---
## \#46 Posted by: Randy_bobandy Posted at: 2019-08-12T02:23:06.032Z Reads: 48

```
Ya its the smaller looking one.
```

---
