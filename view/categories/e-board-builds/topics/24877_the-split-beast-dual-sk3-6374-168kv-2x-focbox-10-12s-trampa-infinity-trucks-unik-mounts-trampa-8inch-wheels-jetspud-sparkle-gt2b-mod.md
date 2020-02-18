# The Split Beast &#124; Dual SK3 6374 168KV &#124; 2x FOCBOX &#124; 10/12S &#124; Trampa infinity trucks &#124; Unik mounts&#124; Trampa 8inch wheels &#124;JetSpud &#124; Sparkle gt2b mod

### Replies: 3 Views: 958

## \#1 Posted by: dedinski Posted at: 2017-06-08T09:49:04.941Z Reads: 294

```
So I named it after the city I live in (Split, Cro). The idea is, with so many beautiful islands around and many bicycle routes, to make a mountainboard hybrid, catch a ferry and ride them all. Also, Id like it to be good enough for the hills and unperfect roads in my city on a daily basis. Ever since I saw uniks AT build I knew I had to make one. 
Im just starting this build, so I really need your help. To save money Id rather not make as many mistakes as on my first build. I have a lot of questions so please be kind to answer some of them...

So the parts:

Dual SK3 6374 168KV - Is this the best option? Should I go up or down in Kv? I already have a 245kv motor, I asume its useless here? 
2x FOCBOX - VESC6 sounds nice but way out of budget
9/12S - I bought a 4x3s lipos for my first build, and now Im wondering wether or not to use those to save money with a BMS or go full expense and get 10/12S4P liIon- where to get one?
Trampa infinity trucks - Unfortunately dont offer room for switching to mbs all-terrain wheels, solutions (maybe mini spring trucks)? 
 Unik mounts - seem the most accessible, but not the cheapest and fit only large trampa trucks.. Are there other options (Kaly,CNC files)?
Trampa 8inch wheels - would 7inch be better? 
JetSpud - absolutely love the board, but Ill take any suggestion since its hard to find
Belt/pulley- 15mm I guess from unik (2 belts,2 (15T) pulleys 62 eur - a bit expensive..)
Enclosure, the wheel gear (72T)  and 35 angle risers Id 3d print in petg and nylon (Id appreciate sharing files here)
Sparkle gt2b mod 
Freebord bindings

Thats it from me, please inform me what you think of the idea and possible problems :D Thank youu
```

---
## \#2 Posted by: High-roller Posted at: 2017-06-08T12:40:54.544Z Reads: 265

```
I think you're really on to something- I'm a first timer working the same kind of thing!
In the past few months alone I've read about more and more people wanting hybrids- is that what we're calling them? In short, a board that can handle some offroading but also go around a city without looking completely out of place. I first saw this with the evolve series and then @dinodave's build, then others. I only found out about @unik's undeniably awesome build after that (sorry!)
So let's compare!
Dual Motors- I got the same ones you did, just 192KV. From what I've read it seems to be the best balance of speed\torque. 245KV will get you more speed, as long as you don't try to climb steep hills with it.
The basic rule of thumb is: 
Higher KV= higher top speed, lower torque.
Lower KV= More strength (better hill climbing), lower top speed.
Beyond that it's a matter of personal preference.
2x FOCBoxes- Same here! I figured I'd get something tough with a heat-sink, as it gets pretty hot where I live (32 degrees Celsius at the time of writing!)
Battery- I got a "space cell" type one custom made locally since they're really expensive to import. 36V, 12Ah, 50 cells, includes BMS. I think the battery is one of the easier -if not cheaper- things to change or replace.
What is your voltage and amps? You can always upgrade later.
Trucks- I got Infinity trucks (and Hypa wheels) through Scramboards. The minis are narrower and more carve-y but a little less stable. My solution was to drill a second set of holes through the bottom of the truck, since I already had  two sets of tapped holes in the top. So I can have a "mountain carver" if I want.
I ordered my mounts, belts and pulleys through scramboards, still waiting for those. unik's trampa stuff only came out after.
Wheels- the trampa 7-inchers are good for street riding or LIGHT offroading and will give you lower clearance, which is nice. I went with the 8-inch one since I plan to go on dirt and gravel tracks.
Deck- I forget what mine is, other than being a 9-ply maple drop-down. Got it off an ebay store for skateboards. As long as yours isn't too flexible you should be fine.
35 degree risers- I've been working on some designs for those and printed a few to try out. I may start selling at some point, but I'll be happy to send you a file.
Remote- I ordered a Nano V2 through the recent group-buy. Might try a gt2b at some point.
Freeboard bindings- me too! truly, great minds think alike :wink:
Hope this helps you! Let us know how it goes!
```

---
## \#3 Posted by: dimnsionofsound Posted at: 2017-06-09T01:05:32.202Z Reads: 232

```
You could go middle of the road battery wise and do a LiFePO4 pack with a BMS (bypass the current/charge limiters and only use the balancing function) out of Hobbyking LiFePO4 packs. You'll just need to get some balance leads and a bunch of XT60 connectors and solder a bunch of them for your preferred pack configuration. I did this on my board and it's worked quite well, with some caveats:

Positives:

* LiFePO4 is nearly foolproof - overcharging and short circuits will not cause a fire (as with LiPo and, to a lesser extend, modern lithium ion can cells), just some heat and outgassing. 
* High current capacity similar to LiPos
* Extremely long cycle life - 2000+ cycles means over the lifetime of the pack it's cheaper than LiIon by a long shot and even cheaper than Lead Acid (which we'd never use in boards anyway but is widely considered the cheapest type of battery, which it is, per Wh, though you can only get 500 max cycles out of them and you shouldn't discharge them below 50% often)
* Relatively flat discharge curve (similar power for your entire ride instead of slight reduction as you discharge with Li-Ion)

Negatives:

* They're heavier than Lithium ion (90-120 Wh/kg vs 150-220 Wh/kg for Li Ion)
* Lower cell voltage 3.3v nominal 3.6v peak vs 3.7v nominal 4.2v peak for lithium ion (though you can just add more series cells if this is an issue)
* Relatively flat discharge curve is also a negative since it is somewhat harder to measure current charge level by looking at the voltage. For my board this hasn't been too big of an issue though, at 12s I usually start around 40v almost fully charged, and when I get below 39v figure I should plan to charge soon.
```

---
