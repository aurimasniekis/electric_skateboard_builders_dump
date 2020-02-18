# Lipo battery split. Does it make a difference?

### Replies: 22 Views: 692

## \#1 Posted by: Andy87 Posted at: 2018-07-30T04:53:43.445Z Reads: 183

```
If I have 4lipos to create a 12s2p pack,
would it make a difference relating to voltage sag and battery temp. if to power 2 vescs with 12s2p or twice 1 vesc with 12s1p?
```

---
## \#2 Posted by: PatRocks Posted at: 2018-07-30T05:12:27.574Z Reads: 179

```
Assuming you will be running a bms, 12s2p is fine, but it's best if you're using high quality lipos, preferably with matching ESR values, and before you connect the cells in parallel, they need to have identical voltage. 2x 12s1p would need two separate bms's I believe, and two separate chargers. It's a bit complicated either way, but 12s2p may be the simplest way.

Edit: in either configuration, the heat and strain on the batteries will be less
```

---
## \#3 Posted by: Andy87 Posted at: 2018-07-30T06:06:25.561Z Reads: 167

```
Thought about 4 of this one, as they ship international
https://hobbyking.com/de_de/turnigy-battery-heavy-duty-5000mah-6s-60c-lipo-pack-xt-90.html

Balance charge them with a imax b6 and just connect when fully charged.

can you say me what could be the max voltage difference between the cells if to hook them up parallel.

I plan to go quad MTB. So the easiest way will be to run twice 12S1P, right?

You thing a BMS is needed on the board too, if I balance charge them? I know there can be a disbalance because of different load and reg. breaking, but that should be not that high that a balance charge after can fix it again. Or am I wrong?

Just started with the LiPo topic...need to get more information ;)
```

---
## \#4 Posted by: PatRocks Posted at: 2018-07-30T06:40:15.775Z Reads: 131

```
This is a good place to start with Lipos:
https://rogershobbycenter.com/lipoguide/

You want the voltage difference between parallel cells as close to 0.00 as possible, as they will attempt to equalize at an unrestrained amount of current, which can be hazardous depending on the difference of charge. 

For the best sources of information about lipo batteries, I recommend the various rc-hobby forums, as they often have been around for several years more than this one. Additionally, they tend to use lipo batteries exclusively for the power to weigh superiority. Not that this forum lacks in scientific talent by any means, but the rc-hobby groups seem to attract more, as not every geek is thrilled about skateboarding. I really mean no disrespect to our forum, but it's good to look around for an enhanced degree of perspective. 

Just food for thought.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-07-30T07:34:03.421Z Reads: 118

```
do you have a recommendation for legit lipo seller who also ship international?
```

---
## \#6 Posted by: PatRocks Posted at: 2018-07-30T08:03:02.625Z Reads: 112

```
From my personal experience, Gens TATTU are likely the best option available. However, their batteries are very expensive. The packs I've been running for a year and a half are still in remarkable shape even after over discharging them (by being an idiot). Second best option seems to be turnigy graphene. These are from hobby king, and from what I understand, you can demand that they sell you "matched packs only or no deal"!
```

---
## \#7 Posted by: PatRocks Posted at: 2018-07-30T08:07:24.032Z Reads: 111

```
The most important bit of advice I could give you is to do tireless research. Inquire with sellers about matched cells and etc. It NEVER hurts to ask for the best option they will provide. Get a Wayne Giles ESR meter, and you will know exactly what they sold you. Ask @deucesdown about the device, he convinced me to get one and I couldn't thank him enough
```

---
## \#8 Posted by: deucesdown Posted at: 2018-07-30T19:06:50.182Z Reads: 92

```
Hey @PatRocks you're awesome.

The more I read and the more I hang around here, the more I flip flop. :)

Despite the deserved reputation for higher quality and safety of the individual cells, seems like most of the recent battery fires are 18650 builds, and most likely the reason is there are just soooo many connections, so there are soooo many places for things to go wrong. In this respect lipos have a big advantage. Hooking up a pair of 6s1p in series, or  even 3 x 4s1p in series, using the provided connectors, removes a ton of variables.

However, most of the lipos we get a look at are oriented toward hobbyists who want cheap and powerful. And the design is to run for 10-50 cycles.

Regarding, quality, industrial lipos are probably much more carefully built. Like the GensAce Tattu line @PatRocks suggested. I'm thinking, manufacturer's reputation is probably the best thing to bet on. If they can be sued or will go out of business if their lipos catch fire, they'll be a lot more careful with the build. But, even the top tier mfgs seem to have spontaneous fires! I remember reading a story about a fresh Revolectrix pack catching fire on first charge.

For safety, most likely a high end hobby charger (non-parallel charging) will be safer than BMS. Mostly because you can see what's happening. But it's a pain in the balls if you charge every day. @PatRocks sidesteps this by building enough watt-hours to charge once a month...

Seems like the only reasonable way to stay safe is to monitor your pack. Total capacity, internal resistance, how balanced does it stay, how well it holds charge, temperatures, mechanical abrasions, etc. And stay close when it's charging.

I know I'm probably on the wrong side of paranoid, but everytime I see a story about battery problems, I try to think, what could i have done to prevent it, detect it, mitigate damage, and also what could I do as it's happening. The most recent story makes me think I need leather gloves and a fireproof blanket near my e-boards, and a gameplan for moving it outdoors while holding my breath. :slight_smile:

All in all, lithium ion and lithium polymers are pretty darn safe! So it's not so much the chance of failure, but the consequence of failure, that drives my paranoia.

Here are some links for your pleasure.

https://www.reddit.com/r/ElectricSkateboarding/comments/933fso/asian_now_video_escooter_battery_explodes/

https://www.rcgroups.com/forums/showpost.php?p=15776103&postcount=4

http://theampeer.org/Learning-LiPo/Learning-LiPo.html

https://www.mpoweruk.com/failure_modes.htm


I guess I should note, usually I charge my board with a bulk charger or CC/CV supply, set to about 90% of full charge voltage, on a a/c outlet timer, running though a volt/amp/watt meter with a time display. I try to be near the stuff when it's charging. I see how much energy goes out via ackmaniac app, and i can see how much goes back in. I'm commuting so this happens twice a day.

No bms (but I'm warming up to the bluetooth bms for charge only -- very attractive little units, $60ish and you get a phone app where you can see individual cell voltage, can be configured for like 10s-15s)

I tear down the board and use hobby chargers to cycle test the pack once a month or so.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-07-30T19:32:43.534Z Reads: 72

```
Prevention is always good and never enough...
I don’t think it’s a paranoia. Just some people worry more some less. Both can be lucky all there life but if something goes wrong only the prepaired ones can minimize the damage...
If you think about to get your burning board out of the room...don’t forget to buy safety glasses.
You don’t want to get hot rubber flying into your face...
I know what i‘m speaking about, I had experience with a burning board just some days ago😬
```

---
## \#10 Posted by: deucesdown Posted at: 2018-07-30T19:37:55.628Z Reads: 73

```
Right you're one of my inspirations. :) I'm thinking, based on that reddit video I linked, there's no time for glasses, probably not even for gloves.

Open door, hold breath, throw blanket over, give it a hug and run, take a few burns and bruises. Then fire extinguisher for inside if needed, water/sand for board if inside is under control. Maybe?

EDIT and pliers for the loop key ;)

EDIT EDIT one of the things I've learned from everyone posting their experience, and my own experience. It's when we want to just try it after completing a big stage of the build, that terrible things happen. :) Must be patient, and stay safe.
```

---
## \#11 Posted by: Andy87 Posted at: 2018-07-30T20:14:20.773Z Reads: 68

```
My advice, find a workplace where you just can let it burn...and which is easy to clean😜
Took me f... 4 days to get 90% of the dirt out of the flat (including professional cleaning help).
Still happy that I was prepared.

I already ordered a new pack of 18650 before that sh.t happened. I already had plans to make the new pack more safe. Cell level fusing, fuses, powers switch and bms...and wanted to redo the old pack...I think sooner or later i‘ll built it, but definitely not in my home.

I‘m now on the point where I think about LiPos...
Started to research...and think how much they more or less dangerous.
My next built will be a mountain board with the batteries on the top, so the size doesn’t matter.

Maybe you can say what you think about my first thoughts. 
I plan to run 4wd 170kw 12s
Powerd by twice 2x6s lipo (the heavy duty 5000mah 60c I linked in the post up)
So the max battery output shouldn’t be more than 60-80a for one 12s pack.
I thought about a12s2p pack to power all 4motors with one, but I guess the parallel lipos need a bit more attention.
I plan to buy two imax charger (no fakes) to balance charge the packs.
No bms on the board 

Any thoughts on it? Something else I should look for?

I looked the tattu lipos also but i couldn’t come on there website as it’s under construction at the moment.
```

---
## \#12 Posted by: deucesdown Posted at: 2018-07-30T20:37:18.805Z Reads: 59

```
SOS @Cobber :slight_smile:

At those loads the 10awg wires start to look too wimpy, XT90 looks wimpy, etc etc. And if you think about 80a -> 5ah pack, you'll get what, 3-4 minutes out of it? I think you'll need to scale everything way way up.
```

---
## \#13 Posted by: Andy87 Posted at: 2018-07-30T20:49:40.068Z Reads: 55

```
I don’t think I can get more than 30a constant for each pack... would be crazy... don’t wanna fly to the moon
80a burst for 3-4sec. guess even not that
With 4 motors more isn’t even rideable
Xt90 can handle 80a, 10awg 55a
think the set up is not so bad 
With the 4blocks 5000mah as 2x12s1p I should come around 15-18km. Not only 5min.
Most time it’s flat surface where I drive. 
Some hills, a bit off-road but no Mount Everest.
And I don’t weight 200kg
```

---
## \#14 Posted by: PatRocks Posted at: 2018-07-30T21:28:32.542Z Reads: 49

```
My thoughts are that if you are planning to lay down the cash for a 4wd build, then why not spend extra on higher performance batteries? The hk graphene 6Ah 65c packs are really REALLY killer batteries. The ones that I'm testing are showing a safe,  sustained 180A discharge capability. The rcgroups guys are getting more than a thousand cycles on their packs (smaller capacity, but shouldn't be any different for larger packs) , but that's my two cents. Don't bottleneck your build at the batteries!!
```

---
## \#15 Posted by: PatRocks Posted at: 2018-07-30T21:39:33.062Z Reads: 50

```
[quote="Andy87, post:13, topic:63277"]
I don’t think I can get more than 30a constant for each pack
[/quote]

Also, the "C rating " stamped on the label is not a true story. However, batteries sold as high-c rated are likely to have fairly low ESR  levels, which is directly related to the voltage sag you will experience under high amp loads. The ESR (equivalent series resistance) is ultimately the determining factor of battery performance.

The point I'm trying to make is that voltage sag is what you (edit: _want to_ )minimize! But I'm a shameless hardware geek. It just seems that if 4wd is the plan, then obviously money ain't a thing!! Right?
```

---
## \#16 Posted by: deucesdown Posted at: 2018-07-30T22:05:02.090Z Reads: 47

```
[quote="PatRocks, post:14, topic:63277"]
REALLY killer batteries
[/quote]

https://www.youtube.com/watch?v=NOcpv12BZM8

testimonials are from the regulars at rcgroup.com. hmmmmm! Maybe it'll make the 65c black&red ones cheaper...
```

---
## \#17 Posted by: PatRocks Posted at: 2018-07-30T22:08:17.962Z Reads: 45

```
I saw these two weeks after buying 4x of the 65c's 😭😭😭

At least I was able to get them cheap (father's day sale and 10% new customer discount) paid $380 for the set 😎😎😎
```

---
## \#18 Posted by: deucesdown Posted at: 2018-07-30T22:11:21.799Z Reads: 43

```
Damn, and that's your baby pack lol
```

---
## \#19 Posted by: PatRocks Posted at: 2018-07-30T22:25:57.017Z Reads: 41

```
Lol, yes it is. My plan is to deconstruct the packs to slim the whole thing down and connect as 12s2p with the DieBie bms (80a fuse bypassed) monitoring the powerplant. Should be a good time. 

@Andy87 which ever path you take, I think you will be pleased with the results. Like @Cobber said, the helifreak forum guys drain those turnigy HD packs in ~5min. with no drama.
```

---
## \#20 Posted by: pixelsilva Posted at: 2018-07-31T04:32:44.203Z Reads: 36

```
> @PatRocks 
> 
> For the best sources of information about lipo batteries, I recommend the various rc-hobby forums, as they often have been around for several years more than this one. Additionally, they tend to use lipo batteries exclusively for the power to weigh superiority. Not that this forum lacks in scientific talent by any means, but the rc-hobby groups seem to attract more, as not every geek is thrilled about skateboarding. I really mean no disrespect to our forum, but it’s good to look around for an enhanced degree of perspective.

Very eloquent @PatRocks. Well said. :+1:
```

---
## \#21 Posted by: Andy87 Posted at: 2018-07-31T05:15:00.383Z Reads: 34

```
So that’s all pretty clear so far. 
Just my thoughts, without to say that the c-rating is correct or not.
If to look on the point that I want to reduce the voltage sag, yes it depends on the internal resistance, BUT it also very much depends on the load (current) drawn from the battery.
To go single pack 12s1p hk Graphen lipos 6000mah and 65c or dual 12s1p hk heavy duty 5000mah 60c, i think the Heavy Duty version get less stress on the single cell.
Less output current, less sag double ah, double range for even less money.
Can’t say anything about cycle life but in „theory“ and on the paper it looks like this for me.
Need to find some reviews why the heavy duty lipos worse than the others

And a 4wd don’t need to be so much more expensive. Just to look I can buy 2vesc 6 from trampa or 4 escapes from stewii...same price....
But I agree, in every built you shouldn’t safe in important quality parts like the batteries
```

---
## \#22 Posted by: PatRocks Posted at: 2018-07-31T06:14:28.235Z Reads: 30

```
Excellent! Glad to see such a well informed thought process. Andy, despite the major setback you had with the fire ( 😭😭😭 ) you're really kicking ass in this "hobby" (lol @b264 ). Can't wait to see your next board, document the process!!

Edit: thanks @pixelsilva !!
```

---
