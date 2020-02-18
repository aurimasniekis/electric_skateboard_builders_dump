# DIYES VESC Track Record?

### Replies: 31 Views: 2457

## \#1 Posted by: Goombaacez84 Posted at: 2016-10-16T15:04:15.292Z Reads: 230

```
How's DIY's VESC track record looking thus far? I've been trying to dig through some old threads on the forum and have only been able to find things back from June/July about DIY's VESCs.

I'm looking to purchase a backup VESC for when my Ollin VESC breaks (now... just had to try FOC) when I remembered DIY also sells them. I don't see nearly as many issues with them as I do Enertion's, but that could be just because there's more people buying their VESCs from Enertion. Has anyone purchased one recently from DIY? How has it been running? What's your setup?
```

---
## \#2 Posted by: evoheyax Posted at: 2016-10-16T15:51:02.340Z Reads: 222

```
First off, why do you feel like your Ollin VESC will break? I have 8 of them running FOC, and not a single issue. If you really want a back up, order another Ollin VESC.

From what I could gather about diys vescs, they are the original BOM, no upgrades besides those recommended by vedder have been done. Now that enertion released the VESC-X which supposedly has a bunch of upgrades, and Ollin VESCs have upgrades, I don't really see why risk it with an original BOM VESC. There have been a fair number of complaints about them breaking over the last few months. Less than enertion, but my feeling is enertion is selling way more (The number of orders enertion is getting per day is insane and explains the whole situation).
```

---
## \#3 Posted by: Goombaacez84 Posted at: 2016-10-16T16:03:07.778Z Reads: 217

```
I hear you on the upgraded BOM ones. I wanted to give the VESC-X a shot but I most likely wouldn't get it until after the snow drops where I live. 

About the Ollin VESC - it actually already broke. I went about 3 miles in FOC on a 12s 190kv setup. I configured the VESC with a fresh firmware and following Vedder's tutorial on YouTube as well. Since winter is quickly approaching here, I wanted to have a backup VESC if this happens again and to avoid a two week downtime. I'll probably play it safe with BLDC for now :sweat_smile:
```

---
## \#4 Posted by: evoheyax Posted at: 2016-10-16T16:09:30.239Z Reads: 201

```
A lot of people seem to have issues with FOC, and they all seem to be belt driven systems. I only ride hub motors, of varying (80 -149) kv, all in FOC and never any issues. And I ride a lot.
```

---
## \#5 Posted by: Goombaacez84 Posted at: 2016-10-16T16:20:34.456Z Reads: 200

```
Yeah it seems like everyone has good success with FOC + hub motor combo. I've considered hubs, but I'll be honest, I haven't done much research on them. It seems Carvons are the way to go
```

---
## \#6 Posted by: evoheyax Posted at: 2016-10-16T16:32:09.364Z Reads: 194

```
The biggest down side I've found from hubs is I get less range. I'm running 4wd with hummies hubs again. With a massive 504 Wh 12s4p battery, I'm lucky to get 7 miles on my very hilly route. I would love to race a raptor vs my board, but a 2wd belt drive equivalent can have the same torque and even a higher top speed than me with 2x to 3x the range. I had better range with the 2wd carvons, I could get about 12 miles on my route with the same battery. I still want to try the carvon v2.5s, with more torque, I bet they are good. They are just too low of a top speed for me, which is why I'm building a 4wd carvon v2 board. I should be able to get into the mid 50's (mph) without any issues, maybe even faster.
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-10-16T17:18:55.765Z Reads: 189

```
[quote="evoheyax, post:4, topic:11239"]
I only ride hub motors, of varying (80 -149) kv, all in FOC and never any issues. And I ride a lot.
[/quote]

This why you will get a PM from me soon lol
```

---
## \#8 Posted by: ekitesurfer Posted at: 2016-10-16T17:20:06.259Z Reads: 186

```
Too low of a top speed? Dual 2.5 go faster than I want to go... I just read the bottom of your post.  You want to go 50mph. Never mind.
```

---
## \#9 Posted by: Goombaacez84 Posted at: 2016-10-16T17:28:27.095Z Reads: 180

```
@evoheyax is making me want to try a hub setup for my next build as well lol I really liked FOC when I tried it but don't want to run the risk of blowing more DRVs until it's proven for belt driven systems...
```

---
## \#10 Posted by: ekitesurfer Posted at: 2016-10-16T17:35:58.556Z Reads: 177

```
I think the key to healthy vescs is to run duals
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2016-10-16T17:40:36.351Z Reads: 172

```
Well soon I shall find out 😉
```

---
## \#12 Posted by: Jinra Posted at: 2016-10-16T18:38:37.505Z Reads: 166

```
You can check out some data here

http://www.electric-skateboard.builders/t/poll-vesc-problems-or-not-please-vote
```

---
## \#13 Posted by: evoheyax Posted at: 2016-10-16T20:20:25.601Z Reads: 160

```
[quote="ekitesurfer, post:10, topic:11239, full:true"]
I think the key to healthy vescs is to run duals
[/quote]

The more vescs, the better. It's just less stress on your vescs. I can't imagine running a single drive, and I don't personally think it should be a thing. No one wants to publicize the fact that if you want to be able to go from 0-20 mph with a single motor, in under 3 seconds, you will have to counter balance the pull on one side, or it will throw you off. 2wd or 4wd is the way to go if your after more stability. If you have a single drive lower torque motor/gearing, you won't feel much of a pull one way. But I'm all about acceleration and top speed.
```

---
## \#14 Posted by: Goombaacez84 Posted at: 2016-10-16T20:31:31.671Z Reads: 162

```
I haven't had too many issues with my single drive if I'm honest. Everything was fine and dandy until I tried to run FOC on the single drive, which yes, I agree would probably be efficient to have a dual drive in this case to reduce risk of damage to the VESC. Being a pretty light guy and comparing to my dual drive boosted though, I feel little manageable differences, which is acceptable in my mind since it's half the drivetrain cost. I think the general conception is two or more drives is _better_, but people don't consider the fact that a single drive might actually suit their needs and purpose more, while being cost effective. I read a lot about some 150+ lbs guys being moved by a single drive with no problem.

Getting back on topic though, thanks for the link @Jinra. I think I'm just going to fork over the cash for another Ollin VESC eventually, especially since they upped their warranty from a year to two years + further support after those years pass. I'm going to keep an eye on how the first production batch of VESC-X goes as well since I'm curious to see if belt-driven FOC support is increased
```

---
## \#15 Posted by: evoheyax Posted at: 2016-10-16T20:38:51.311Z Reads: 149

```
[quote="Goombaacez84, post:14, topic:11239"]
I'm going to keep an eye on how the first production batch of VESC-X goes as well since I'm curious to see if belt-driven FOC support is increased
[/quote]

The VESC-X or a VESC v6 (when ever those finally come out) sound like the best option for single motor boards. But personally, I like the Ollin warranty. I don't think I will be buying VESC from anyone else in the near future.
```

---
## \#16 Posted by: chinzw Posted at: 2016-10-17T18:32:55.922Z Reads: 134

```
I have a VESC from torqueboards, haven't had any problems so far, i run BLDC tough. I tried FOC but my battery leads were too long and i was getting errors while braking. Ill report back once i re do all my wiring with very short 10aug wires.
```

---
## \#17 Posted by: Goombaacez84 Posted at: 2016-10-17T18:46:41.063Z Reads: 136

```
Good to know about the torqueboard VESC. I'm back and forth on getting one, but am still leaning more towards just settling on another Ollin VESC.

I wasn't aware that battery leads would cause an issue in FOC mode? Would you be able to explain that a little bit more? I'm running a split enclosure design so I do have long battery leads going from battery to VESC so that could be a problem for me.
```

---
## \#18 Posted by: chinzw Posted at: 2016-10-17T18:56:37.791Z Reads: 135

```
I read it over at vedder's forum i believe. It seems that the length of the wires from the battery to the VESC influences the inductance and this affects the DRV chip when using FOC.
At the moment i have 12AUG wires that run about 40+ cm, with about 4 connectors. Not the most efficient wiring. See here, there's a few sections of wire missing lol.

<img src="/uploads/db1493/original/3X/7/7/77649c331764f8b961625a2168be954ff5f4dd0d.jpg" width="375" height="500">
```

---
## \#19 Posted by: whitepony Posted at: 2016-10-17T19:34:44.583Z Reads: 131

```
[quote="evoheyax, post:6, topic:11239"]
With a massive 504 Wh 12s4p battery, I'm lucky to get 7 miles on my very hilly route.
[/quote]

what?! :scream:

what avg speed are you running? do you ride with a braking parachute attached or something? you need the 5fold energy of my single drive per mile :dizzy_face:
```

---
## \#20 Posted by: evoheyax Posted at: 2016-10-17T19:39:13.453Z Reads: 129

```
My average speed is 25 mph with inclines of 7% grade or higher for at least 40% of my route. I'm a 200 lb guy also, which from testing with hummie who's about 140 lb, makes a big difference.
```

---
## \#21 Posted by: Mrmoonlight Posted at: 2016-10-17T20:14:40.124Z Reads: 124

```
I have an Enertion, diyelectric and Ollin VESC. I have a Carvon V2 and V2.5 singles and have tried both FOC and BLDC. I have overheating issues with the V2 on all 3, but at different levels. Ollin is by far the best performer followed by Diy then Enertion. The Diy VESC is just fine all day for flats and short inclines. The Enertion cuts out on any inclines and does okay on flats. The Ollin only has heat issues when I push it hard. With the V2.5, all 3 VESCs work fine in BLDC, but on FOC, the Enertion and Diy VESCs don't run as smooth as the Ollins VESC. 

If I had a choice, I'd stick with the Ollin VESC. Better performance and high quality workmanship.
```

---
## \#22 Posted by: saul Posted at: 2016-10-17T23:29:53.762Z Reads: 118

```
25 up hill is pretty impressive. still seem oddly inefficient! I wonder if your front wheels are fighting the rear....


back to topic, I got a vesc from diy, first or second run I think, after the usual months of delays for vesc production I got it. but its just been sitting on my desk as a backup does.....
```

---
## \#23 Posted by: Bataleon Posted at: 2016-10-23T18:54:01.880Z Reads: 107

```
[quote="Mrmoonlight, post:21, topic:11239"]
The Enertion cuts out on any inclines and does okay on flats.
[/quote]

Was the Enertion from an older Chinese-made batch or more recent USA-made?
```

---
## \#24 Posted by: Luke Posted at: 2016-10-23T19:39:45.719Z Reads: 100

```
This maybe getting a little sidetracked from the op of diy vescs, but I've run 2 enertion vescs with heatsinks on FOC, a 10s battery, dual 190kv motors up 10%-25+% hill daily with no issues from the vescs for about a month now
```

---
## \#25 Posted by: Mrmoonlight Posted at: 2016-10-23T21:38:33.070Z Reads: 94

```
Not sure. I got it in July if that helps.

@Luke duals will put less stress on your VESC than a single. Hubs or belts?
```

---
## \#26 Posted by: Luke Posted at: 2016-10-23T22:01:35.759Z Reads: 96

```
@Mrmoonlight  belts, and pretty pathetic performance from a single from when my second motor was broken
```

---
## \#27 Posted by: Mrmoonlight Posted at: 2016-10-24T13:32:30.963Z Reads: 93

```
Belts are more forgiving on high KV motors than hubs. My Carvon V2 single has a 149kv motor and it maxes out my VESC's capabilities. A single belt would put a lot more stress on your VESC than a dual, but less than a single hub. If your going up a lot of hills, dual is the way to go. I prefer singles, because I like the weight savings and minimizing motor drag, but it's a trade off when it comes to performance.
```

---
## \#28 Posted by: Ulfberht Posted at: 2016-10-26T03:59:22.318Z Reads: 82

```
So far it's pretty obvious from the lack of complaint threads/posts that Dexter@  has received speaks a lot without saying a word. :v:
```

---
## \#29 Posted by: Goombaacez84 Posted at: 2016-10-26T04:13:31.463Z Reads: 79

```
True, that's what I thought at first. But it's difficult to make that assumption due to the idea that the lack of complaint threads/posts might be due to DIY not selling nearly as many VESCs as Enertion does.
```

---
## \#30 Posted by: Spek Posted at: 2016-10-26T22:54:08.669Z Reads: 65

```
More likely prompt and reliable customer service so people don't have to result to complaining on the forum.
```

---
## \#31 Posted by: Goombaacez84 Posted at: 2016-10-26T23:43:50.039Z Reads: 61

```
Also plausible, but DIY's customer service regarding the VESC is just like Enertion's - if you don't buy the extended warranty and you have any issues, even on first start up on the bench for motor detection, you're on your own unless you can prove it was a manufacturing defect and not your fault. For this reason, I opted not to buy one.
```

---
