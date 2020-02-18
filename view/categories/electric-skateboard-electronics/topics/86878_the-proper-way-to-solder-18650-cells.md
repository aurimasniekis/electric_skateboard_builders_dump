# The proper way to solder 18650 cells!

### Replies: 46 Views: 1562

## \#1 Posted by: FinnishSnowmobiler Posted at: 2019-03-11T17:41:15.696Z Reads: 345

```
Hi, 

I procrastinated many weeks about whether or not to solder 18650 batteries. I tried many combinations (solder, wire and flux / acid) to find the quickest method to solder these cells together. I'm pretty proud of the outcome (less than one second contact time and to tear the connection apart you need really significant forces and the battery can gives up millimeter or two when applying a huge pull)

Items needed:
- A quality 80w soldering iron
- Lötwasser (soldering acid)
- Stranded copper wire, I took mine apart from an audio cable
- Leaded solder
- The actual cells

What I couldn't demonstrate in the video is how I applied pressure to the joint with a wooden block to really maximize the surface area of the contact. Please enjoy the short video!

https://youtu.be/pptK4TTZr8Q
```

---
## \#2 Posted by: Deckoz Posted at: 2019-03-11T17:42:53.941Z Reads: 327

```
(post withdrawn by author, will be automatically deleted in 24 hours unless flagged)
```

---
## \#3 Posted by: Battosaii Posted at: 2019-03-11T17:49:14.677Z Reads: 320

```
I've soldered wires to nickel that is welded to a cell but never a bare cell.
```

---
## \#4 Posted by: Acido Posted at: 2019-03-11T17:52:17.559Z Reads: 313

```
That is a totally different story, especially when theres 2-3 layers of nickel
But still soldering is not the solution because to get proper connections the cell needs to get to like 250c or something
```

---
## \#5 Posted by: FinnishSnowmobiler Posted at: 2019-03-11T18:01:04.232Z Reads: 300

```
Immediately after the connection was made I could place my finger on top of the joint and believe it or not the contact was only slightly warm. The real reason I'm not using a spot welder: cost...
```

---
## \#7 Posted by: Acido Posted at: 2019-03-11T18:26:47.281Z Reads: 274

```
run away from your board when it sets itself on fire :D
```

---
## \#8 Posted by: Acido Posted at: 2019-03-11T18:27:45.063Z Reads: 267

```
boss level is less than 200$ with the battery to power it, not that expensive if you make more than one pack or sell it after
```

---
## \#9 Posted by: PatRocks Posted at: 2019-03-11T18:57:02.093Z Reads: 255

```
Agreed with decky and acido. While we appreciate your efforts, this is a dangerous method and is not worth the risk
```

---
## \#11 Posted by: FinnishSnowmobiler Posted at: 2019-03-11T20:11:52.210Z Reads: 232

```
@PatRocks Is there a specific reason why would this be a dangerous method as I've cardboard-insulated the positive terminals (and sure as hell the copper won't melt through cardboard no matter what). 

Is there something else that would make this a dangerous method?
```

---
## \#12 Posted by: FinnishSnowmobiler Posted at: 2019-03-11T20:18:01.870Z Reads: 217

```
This is a demonstration on how flexible this kind of installation is. Leaded solder can also withstand the huge forces on a crossbow's bow's tip... Torsional forces are probably something solder can't withstand but I don't see how the contacts would come loose from the 18650's. 

And yes I'm aware of the fact spot welding is a bit safer but I find it interesting to really understand the real differences between spot welding and soldering if done right. Thanks for the inputs guys!


https://youtu.be/QxaPSEX48cs
```

---
## \#13 Posted by: PatRocks Posted at: 2019-03-11T20:24:21.007Z Reads: 206

```
The damage that can be done to the electrolyte by the heat, even for a couple seconds of contact, can mess with the properties of the cell. It can change the internal resistance of each cell, leading to (best case scenario) a pack that drifts more than usual. Additionally, it is risky in terms of electrical connection and may be a critical point of failure. If the contact is compromised, may result in arcing, then heat, and possibly fire. I would never attempt to build a pack without a spot welder.
```

---
## \#14 Posted by: FinnishSnowmobiler Posted at: 2019-03-11T20:56:19.956Z Reads: 198

```
@PatRocks Is the small difference in internal resistance how relevant as some people have even successfully built well-functioning packs with different cells from different manufacturers. Correct me if I'm wrong - parallel packs (1s6p) difference in cell resistance won't matter so much as the parallel cells are always forming one pack with precisely the same voltage.

And my intention is to never assemble a BMS. I'll always balance charge the pack and monitor it externally and I'll set the low voltage cutoffs etc to the VESC and in addition I'll use low voltage alarm buzzers.
```

---
## \#15 Posted by: FinnishSnowmobiler Posted at: 2019-03-11T20:57:47.344Z Reads: 193

```
@PatRocks Do you mean that the copper would come apart from the cell by "compromised contact"?
```

---
## \#16 Posted by: linsus Posted at: 2019-03-11T21:03:38.327Z Reads: 185

```
wtf, so much hate. Atleast he did it the proper way, been done plenty times before without significant harm to the cell (if you know what you're doing obv.). Looks solid, good work!
```

---
## \#17 Posted by: Battosaii Posted at: 2019-03-11T21:08:35.229Z Reads: 182

```
Raptor 1 deck has 0 flex but it's actually conductive because it's carbon so may be even worse for this application lol
```

---
## \#18 Posted by: Deckoz Posted at: 2019-03-11T21:09:25.121Z Reads: 179

```
it has flex. All decks flex... ALL. You just might not feel the deflection.
```

---
## \#19 Posted by: Battosaii Posted at: 2019-03-11T21:12:44.929Z Reads: 178

```
I dunno man I'm 300lbs and the thing will not budge. If it has any flex then it's not  measurable with out scientific equipment lol. Btw very uncomfortable to ride.
```

---
## \#20 Posted by: psychotiller Posted at: 2019-03-11T23:55:32.408Z Reads: 170

```
Yes, because molecules stretch. If you stare at them long enough.
```

---
## \#21 Posted by: brenternet Posted at: 2019-03-12T00:00:31.873Z Reads: 167

```
You know what else stretches? Belts.

(popcorn)
```

---
## \#22 Posted by: AlanZhou Posted at: 2019-03-12T00:27:44.128Z Reads: 169

```
haha, do you guys wanna see the mess i made soldering? turns out good leaded solder has a hard time sticking to cells

These cells are a goner and I'm pretty sure if I paid @psychotiller or @hyperion1 good money to build a pack out of these they wouldn't

The flux is hard after to clean off almost impossible




![IMG_20190311_203112|375x500](upload://eGPNcqZJLW2suhQE5C3huUE7PjM.jpeg) ![IMG_20190311_203147|375x500](upload://6lxjfig8vJ2fULKMuvWB91AA3dw.jpeg) ![IMG_20190311_202645|375x500](upload://7dOa7l2BekZga4LeHhrpjQvObAX.jpeg)
```

---
## \#25 Posted by: deucesdown Posted at: 2019-03-12T02:25:19.539Z Reads: 150

```
@FinnishSnowmobiler I'm on your team! Most of my packs have felt the heat of a soldering iron. Skinny strips of nickel just ain't enough! :slight_smile:

I look at my A123 26650, and look at the .20 nickel, and I just can't bear to do do it. 3 packs built with solder, no problemo. I really think soldering is the correct way to go with low p count packs built from high power cells.
```

---
## \#26 Posted by: AlanZhou Posted at: 2019-03-12T03:03:24.583Z Reads: 142

```
[quote="deucesdown, post:25, topic:86878"]
Skinny strips of nickel just ain’t enough!
[/quote]

Ay don't insult thin nickle strips, even though I'm biased and I perfer thickk nickle strip 2x 0.30 most people would do , 3x 0.15
```

---
## \#27 Posted by: psychotiller Posted at: 2019-03-12T03:25:49.712Z Reads: 138

```
Your Mom's deflecting!! :rofl:
```

---
## \#28 Posted by: AlanZhou Posted at: 2019-03-12T03:28:24.511Z Reads: 136

```
Hey psychotiller speaking of the same topic. Would you be willing to weld my "lightly used cells?" 🤣🤣😎

Jk
```

---
## \#29 Posted by: psychotiller Posted at: 2019-03-12T03:30:56.134Z Reads: 141

```
https://www.youtube.com/watch?v=rqtr_RvR3sY
```

---
## \#30 Posted by: Dmaxx Posted at: 2019-03-12T04:17:32.941Z Reads: 134

```
Umm I have 4 working packs all made by soldering buswire to cells and then to brass busbars and havent had any issues after 1.5 years. Used 3d printed cases to keep cells separate and used plenty of flux but the solder joints are quite strong. Not sure why you say never solder..
```

---
## \#31 Posted by: Pedrodemio Posted at: 2019-03-12T05:13:26.697Z Reads: 134

```
@barajabali take on it 

![image|281x500](upload://i6f4Vuwb0r0vEmysQNlP1QFxkXW.jpeg)
```

---
## \#32 Posted by: MysticalDork Posted at: 2019-03-12T06:18:14.893Z Reads: 130

```
I've never had good results just using the flux built into the solder, no matter how good the solder. Just not aggressive enough to quickly tin nickel plated steel. A non-rosin-based flux (I use Ruby Fluid liquid flux for copper plumbing) is much more aggressive and faster.

Also, I've never met a rosin based flux that either isopropyl alcohol or acetone didn't take right off.
```

---
## \#33 Posted by: TowerCrisis Posted at: 2019-03-12T08:18:35.527Z Reads: 130

```
I'm just going to leave this here. Everything is quoted directly from samsung in their datasheets.

"Don't heat partial area of the battery with heated objects such as soldering iron."

"Don't solder on the battery directly."

"The cell should not be soldered directly with other cells. Namely, the cell should be
welded with leads on its terminal and then be soldered with wire or leads to solder."

And consequently:

"Otherwise, it may cause damage of component, such as separator and insulator, by
heat generation."

Keep in mind that there is plastic directly in contact with these components you solder and giving excessive heat WILL cause damage. That is undeniable. There is potential to melt the separator and cause an internal short no matter how brief you solder cells.

These are NOT like soldering lipos, as those have heatsinks temporarily placed between the tabs and the cell during soldering to prevent damage.
```

---
## \#34 Posted by: barajabali Posted at: 2019-03-12T15:12:11.648Z Reads: 120

```
Normally I would advise against soldering cells but its not as bad as people think it is. i recall watching a video about someone measuring capacity lost after soldering for an extended time. It only really affects the negative terminal and the loss is negligible if you do it correctly. 

You need a high power iron and tin all parts first.
```

---
## \#35 Posted by: Deckoz Posted at: 2019-03-12T22:06:09.899Z Reads: 110

```
probably an incredibly boring deflection... lol
```

---
## \#36 Posted by: Deckoz Posted at: 2019-03-12T22:10:03.887Z Reads: 112

```
[quote="Dmaxx, post:30, topic:86878"]
Not sure why you say never solder…
[/quote]

Well.. lets see, solder pops and fizzles. He didn't even cover the holes over the positive buttons. What if theres solder/flux that got under the button as a bead and pops off and jingles around and shorts.

I mean, I did say if it worked for him cool. But there's better, safer ways, with less potential fallout risk later down the line. That's all I was saying. Solder away if you wish. But yes, _'I'_ will never solder to cells directly, happy?
```

---
## \#37 Posted by: thisguyhere Posted at: 2019-03-12T22:55:56.749Z Reads: 104

```
[quote="Deckoz, post:36, topic:86878"]
What if theres solder/flux that got under the button as a bead and pops off and jingles around and shorts.
[/quote]

this has happened to me before, a little solder bead got caught inside the positive terminal cap.  jiggled it around in there, and POP!  mini solder explosion when it shorted.

my biggest issue with soldering onto cells is NEVER being able to salvage them.  like, weld tabs can be ground off.  solder bead isn't coming off.
```

---
## \#38 Posted by: Deckoz Posted at: 2019-03-13T02:16:57.476Z Reads: 98

```
that too, recovering and rebuilding is alot easier and possible.
```

---
## \#39 Posted by: J0ker3366 Posted at: 2019-03-13T02:19:53.300Z Reads: 98

```
[quote="brenternet, post:21, topic:86878"]
You know what else stretches?
[/quote]

Did someone say channel trucks?
```

---
## \#40 Posted by: FinnishSnowmobiler Posted at: 2019-03-13T05:36:53.503Z Reads: 92

```
Lol why would you want to salvage these kind of cells? :smile:
```

---
## \#41 Posted by: FinnishSnowmobiler Posted at: 2019-03-13T05:41:13.511Z Reads: 89

```
As you can see in the video the only time the solder pops is when it's applied to the iron in the first place... When the chemicals burn from the solder and the smoking stops the substance is stable.
```

---
## \#42 Posted by: mynamesmatt Posted at: 2019-03-13T06:10:11.290Z Reads: 83

```
[quote="brenternet, post:21, topic:86878, full:true"]
You know what else stretches? Belts.

(popcorn)
[/quote]

you had to say something didn't you
```

---
## \#43 Posted by: L3chef Posted at: 2019-03-13T06:43:56.791Z Reads: 79

```
[quote="mynamesmatt, post:42, topic:86878"]
you had to say something didn’t you
[/quote]

He just wants to see the world on fire
```

---
## \#45 Posted by: thisguyhere Posted at: 2019-03-13T15:57:22.810Z Reads: 68

```
[quote="FinnishSnowmobiler, post:40, topic:86878, full:true"]
Lol why would you want to salvage these kind of cells?
[/quote]

P groups die frequently....so one P group dies, may need to rebuild the pack.  or...pack comes to end of life but still has some viable cells inside.  you going to throw those out too?

i've salvaged a number of 25r cells from before 30q's came into favor...using the 25r cells for all manner of non-esk8 related stuff around the house.
```

---
## \#46 Posted by: Deckoz Posted at: 2019-03-13T23:49:53.746Z Reads: 57

```
same... like leaf blower & weedwhacker/trimmer. Battery backup system for network and servers. rebuild drill and impact batteries. portable boom box. battery backups for our night stands to charge phones/power alarms. portable pi as a vpn router for public wifis. the possibilities of reuse are endless.
```

---
## \#47 Posted by: Sn4pz Posted at: 2019-03-13T23:53:01.387Z Reads: 57

```
[quote="thisguyhere, post:45, topic:86878"]
P groups die frequently
[/quote]

How frequently are we talking? 

Obviously it's not quantifiable in the # of days it will take, but what's your estimate?

I'm having my battery built by a professional but I'm still terrified of failiure rate

12s7p btw
```

---
## \#49 Posted by: Battosaii Posted at: 2019-03-14T00:05:47.904Z Reads: 52

```
I salvaged a very poorly built 10s3p (raptor space cell) with HG2 cells and use the cells on my main esk8 light. I carry a few cells in my backpack so I never have to worry about having to charge my light I always have extra cells.
```

---
## \#50 Posted by: Sn4pz Posted at: 2019-03-14T00:06:35.039Z Reads: 51

```
With that rational I shouldn't have a failiure ever! 😂

What's a good indicator or a failing pack? I've been assured that it's going to be relatively difficult to pull a 12s7p out of balance, especially when I'll be using lower amounts of amps per motor (40, 45 maybe? I'm not looking for a rocket)


That being said, would you think that I should balance once a week? Once every two weeks? 🤔

I'll be using a metr module as well as a DieBieMS to look at the technical numbers of my pack, so I think I'll have a good suite of software
```

---
## \#52 Posted by: Sn4pz Posted at: 2019-03-14T00:19:04.130Z Reads: 48

```
Thank you so so so much for your response. It's exactly what I needed to hear/wanted to know :) 

I've got one more question... But I'll come back tomorrow if I can't find the answer out on my own. :) 

Thank you!

E: I guess I could set my cutoff to 40/39v and never worry about it 🤔🤔 not saying I would disregard taking care of it... I just figure that would significantly lower my chances of failiure by undervolting
```

---
## \#54 Posted by: Sn4pz Posted at: 2019-03-14T01:18:25.924Z Reads: 44

```
I going to pm you an additional question, sorry to keep adding onto the pile of questions 😂

It's a quick one, I would think 🤔
```

---
