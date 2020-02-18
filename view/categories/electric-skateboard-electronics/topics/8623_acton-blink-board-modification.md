# Acton Blink Board Modification

### Replies: 50 Views: 8466

## \#1 Posted by: thatfilmguy Posted at: 2016-08-30T05:01:12.453Z Reads: 417

```
I've got an interesting question. I'm new to electric skateboards, I wanted something small and relatively fast, for a decent price, so I got an Acton Blink Board. After putting over 100 miles on it, I'm fairly impressed by the thing, the speed and size is great (I use it for a short commute). However, I would love to extend the range. I get 3.5 miles per charge in a hilly area.

My thought is to hook an external battery pack to the bottom of the board. I've seen boosted board owners doing this online. The end effect is almost doubling the range. I would like to do something similar to my Blink Board, but I don't know if it is possible, without frying out the electronics.

I have some RC experience, so I am used to working with lipos and electronics. But I don't know the best way of going about this.

I've opened the electronic cover on the board, to try to get a lay of the land. The battery pack reads 41.4 volts at a full charge. And the pack is 72 Wh. I'm thinking the best way to add a second battery pack is to connect the two batteries in parallel before the VESC???

Battery suggestions are appreciated as well!
I was think a 10 cell 18650 battery pack or a large lipo from the hobby store. (I would like double the range or more)

Thoughts???
<img src="/uploads/db1493/original/2X/9/99cd1ae50355a591c8ed739ff5c31d1f95843290.JPG" width="400" height="500"><img src="/uploads/db1493/original/2X/d/df8b9797170f2838f50c3a93da23405eac356693.JPG" width="400" height="500"><img src="/uploads/db1493/original/2X/8/825b6d3d1afa968672dc7c083b1738be5afc30dd.JPG" width="625" height="500">
```

---
## \#2 Posted by: saul Posted at: 2016-08-30T06:31:55.602Z Reads: 379

```
how does it handle hills?

pretty nice that it already has xt60's for the battery. I would mod the case so you can swap packs and extend range that way.

41.5V is about right for a 10s1p 18560, so just get another on of those made...
some 3000mah hg2's should work nice...
you could also do a 2p pack to double capacity but i dont think mixes old/new packs in parrele is a good idea.

oh and thats just an esc(electronic speed controller), VESC is a specific open source esc.
```

---
## \#3 Posted by: thatfilmguy Posted at: 2016-08-30T14:46:02.037Z Reads: 360

```
It handles the hills pretty well, and these are pretty steep hills well well above 15% it is rated for. There is a little speed fall off, but not bad.

Thanks for correcting me about the ESC.

What are your thoughts about using a hobby lipo, keeping a simpler chemistry between the built in battery?<img src="/uploads/db1493/original/2X/5/5669999e19fb5edfadaf9cd063cf8c9f0ea3f8ea.jpeg" width="369" height="500">
```

---
## \#4 Posted by: saul Posted at: 2016-08-30T18:49:20.296Z Reads: 322

```
not bad for a board that size, my next build is going to be similar 29"

I use lipo in my current board, 2 6s 5200mah in series.
with 2 5s packs you can get a slimmer package to attach some how...
like 2 of these  [nano tech 5s](http://www.hobbyking.com/hobbyking/store/__20526__Turnigy_nano_tech_4000mah_5S_25_50C_Lipo_Pack_US_Warehouse_.html)

this would make it alot easier to charge them externally too. 10s chargers are pricey.
```

---
## \#5 Posted by: thatfilmguy Posted at: 2016-08-30T21:27:00.471Z Reads: 318

```
The size of the board makes it pretty nimble, it's a blast to ride, just in case you had any doubts!

How many miles can you cover with two 5200mah batteries?

So, are you recommending something like this?
<img src="/uploads/db1493/original/2X/c/cf8d028d8182f31f75ffe81cc85aed2201bf4f82.jpeg" width="690" height="462">
Or killing off the original battery and just having those two 4000mah in series?

Also, am I correct in thinking that the low power shut off would monitor the additional cells too? Or would it draw all the lipos too low?
```

---
## \#6 Posted by: sl33py Posted at: 2016-08-30T21:37:00.329Z Reads: 284

```
I would swap the electronics into a new enclosure to give you more space for additional batteries.  Whatever you decide to modify and add.  An additional battery or replace the one w/ two in parallel to match.
```

---
## \#7 Posted by: saul Posted at: 2016-08-31T01:11:29.331Z Reads: 273

```
yea thats about right, but just one pack at a time. two packs with different capacity would cause issues i'm sure.

but the orginal cutoff should be ok since it should just be monitoring pack voltage.

but yea you'll probably have to mod the case somehow to get more battery in there...
```

---
## \#8 Posted by: thatfilmguy Posted at: 2016-09-10T21:37:22.291Z Reads: 255

```
Thanks Saul for the help. I have a few more quick questions:

Since the original battery was 41.4 V, would it be better to use two (2) six cell batteries (2 x 22.2V) for a total of 44.4V, vs. only 37V (2 x 18.5 V)? I'm worried about the internal low voltage cut off of the board shutting me down way early with a 5 cell batteries.

Lastly, should I be worried about the number of amps coming from any of these battery setups?
```

---
## \#9 Posted by: thatfilmguy Posted at: 2016-09-10T22:09:36.870Z Reads: 259

```
If I did my math correct.

The original battery:
72wh @ 41.4V =1739.13mah
1739.13 / 1000 = 1.7 amps

With the suggested 5 cell battery setup:
4000mah / 1000 = 4 amps 

Two batteries in series, the amps stay the same.

So, 1.7 amps vs 4 amps, should I be worried?
```

---
## \#10 Posted by: saul Posted at: 2016-09-11T04:29:24.591Z Reads: 246

```
so the stock pack is 41.4v full which is 10s, 10 * 4.2 = 42 == 41.4 to be safe.
So i would use the same 2 x 5s packs at 10s. a 12 would probably burn something up.

as for the rest I think you're confusing some of the notation, mah/ah is capacity. discharge rating on lipo is is C for, meaning 10C = 10 x 4000mah = 40 amps max. 
but this is max, the esc should limit amps to hopefully the same power.

keep in mind this is just what I would do to extend range, if your not sure, and carefully you might end up with a regular old skateboard...

honestly if you can I would just build a full diy cruiser, single 6355, and keep the blink as a backup/loaner/super mini.
```

---
## \#11 Posted by: Mikenopolis Posted at: 2016-09-11T04:53:15.267Z Reads: 222

```
Agreed, that what I did just to be on the safe side or not bricking the Blink. Did a full new build and have the Blink as a n00b loaner, love that it can be limited  to 5mph
```

---
## \#12 Posted by: Aivean Posted at: 2016-10-28T02:09:13.562Z Reads: 210

```
I have some crazy idea:  what about connecting some larger battery to the charging port?

It seems like an easier approach as it doesn't require tampering with built-it battery/case, but I'm worried about how it may affect the built-in battery. 

Also I'm not sure about the voltage of  that larger batter. Should it be ~41v (as fully charged built-in one), or it's better to have it slightly lower?

Can someone clarify please?
```

---
## \#13 Posted by: Jinra Posted at: 2016-10-28T05:14:07.172Z Reads: 194

```
Charging ports and wires aren't designed to have large current flow through them. If you connect an extra pack in parallel you'll likely damage them if the BMS doesn't cutoff first.
```

---
## \#14 Posted by: Aivean Posted at: 2016-10-28T21:57:54.021Z Reads: 207

```
Thanks for the response!

Please correct me if I'm wrong, but original battery usually lasts around 45 mins, with capacity 1.7ah.

Than means that discharge current is approximately 1.7 / (45 / 60) = 2.26 A.  Original charger designed to provide 2A, which is pretty close. 

Is that difference ~0.26 A enough to damage charger port or wires?

I was more concerned whether this setup is going to work at all. Lets say I cruise at low speed to make sure discharge rate is less than 2A. In this case what will happen:

* Will the motor take power from both batteries simultaneously? 
* Will the internal battery be constantly charged and discharged, or it will be discharging slowly?
* What voltage should I use for the larger battery?

Are you saying that this setup is essentially the same as both batteries being connected in parallel?
```

---
## \#15 Posted by: saul Posted at: 2016-10-28T22:06:53.658Z Reads: 191

```
[quote="Aivean, post:14, topic:8623"]
approximately 1.7 / (45 / 60) = 2.26 A
[/quote]

thats an average current, which is not ok for this calculation, current while riding can go from 0 - 20A maybe more.
if you're not sure, you probably shouldn't play with this, but if you do make sure to take video of the :boom:
```

---
## \#16 Posted by: Aivean Posted at: 2016-10-29T06:45:39.677Z Reads: 187

```
saul, 

Thanks for your comment.  

I'm not sure, but I'm really interested, so I'm doing my research, which includes asking people who's knowledge is deeper. 

I see that a lot of people say that usually it's safe to use charger with higher current rating, as device draws only what it needs:
https://www.quora.com/What-would-happen-if-I-charged-my-phone-with-a-5V-1A-or-5V-3A-battery-charger-The-phones-rating-is-3-8-V-1300mA

Isn't that true for the skateboard? Or there is a direct link between motor and charging port?
```

---
## \#17 Posted by: faust Posted at: 2016-11-19T02:52:11.638Z Reads: 178

```
[quote="saul, post:2, topic:8623"]
pretty nice that it already has xt60's for the battery. I would mod the case so you can swap packs and extend range that way.
[/quote]

I really like @saul's idea here. I think I'll do some more research and attempt this myself. 

Has there been any progress on this project?
```

---
## \#18 Posted by: saul Posted at: 2016-11-19T04:10:47.096Z Reads: 176

```
the more i look at this the more I think that it would not be worth the work...

but idk maybe this board is more fun than it looks? haven't seen one in the real world yet....
```

---
## \#19 Posted by: faust Posted at: 2016-11-19T04:13:56.581Z Reads: 177

```
I have the hub motor variety and it's a blast. I'll just be getting the newer model soon, and as battery modification is my primary interest right now, I think a project like this could be ideal.  (Trying to work towards an elegant solution to battery swapping: http://www.electric-skateboard.builders/t/creating-a-swappable-small-battery-system/13006/3)
```

---
## \#20 Posted by: saul Posted at: 2016-11-19T05:28:50.989Z Reads: 178

```
doesn't that only go like 10mph? lol

anyways swappable isn't that hard, it just depends if velcro counts as elegant. i've been using it to hold on the cover with my swappable packs with no problems. 12-15 miles each. swap and i'm back to full speed!

i found a pretty nice solution with aluminum bar to get a nice slide in enclosed battery....might try it as a rebuild but probably not any time soon...
```

---
## \#21 Posted by: faust Posted at: 2016-11-19T07:46:13.568Z Reads: 157

```
Aluminum bar sounds more my speed, though velcro sounds like a good prototyping measure. Snap in and swap was what I was thinking. I expect that once I get something working, I'd build a nice enclosure for it. 

As for the Blink, mine takes me a little past 15MPH. Quite good for my needs.
```

---
## \#22 Posted by: Carlos Posted at: 2016-11-25T20:29:43.075Z Reads: 142

```
I have the Acton hub motor blink board as well, and I am really happy with it... except for the range, If I were to connect another battery pack in parallel would the original charger charge both packs?
```

---
## \#23 Posted by: thatfilmguy Posted at: 2016-12-01T05:50:27.374Z Reads: 143

```
I took Saul's and Mikenopilis advice, and started looking into a ground up type build. I also determined that putting more money into a board that I couldn't tweak all the way to my liking (based on hardware limitations) wasn't worth it.
```

---
## \#24 Posted by: admiralackbar Posted at: 2016-12-13T14:56:46.951Z Reads: 143

```
the solution is simple... gonin the acton blink board user manual and look to see whether the board can be charged and ridden at the same time... ive seen boards that cant even be turned on and charged at the same time let alone ridden...   if its not specified in the manual then just see if its mentioned in a third party video or review...  what i would use is one of those portable outlet boxes on kickstarter for charging laptops... ifylucant charge while riding you could take charging breaks while you arent riding...whenit dies mid trip... these portable outlets are a VERY new product and willlikely transform the way people ridethe subway etc...theye on kickstarter and indiegogo for around 100 bucks and can charge a laptop to 100 percent two times... and charge a phone like 20 times


overal GENIUS idea
```

---
## \#25 Posted by: Okami Posted at: 2016-12-13T18:47:24.355Z Reads: 140

```
I would advise to check what wiring - connections this board has.. 

Right now without pictures it is hard for me to guess how the wiring looks. The best way would probably be to cut into the battery wires which go to esc and then make a switch or connectors there (or just make a parallel wire harness with xt60 connector). 

If you want to ''upgrade'' the existing battery, it would be good if the specs of your new battery would be similar, so that there is not a big difference in capacity or discharge load.
```

---
## \#26 Posted by: Sapphirinia Posted at: 2017-01-25T05:57:23.543Z Reads: 129

```
So for other folks wanting a smaller build like me? Where should I begin? I want to do hub motors on my penny (nickel) board using as much of the original components as possible. Someone referred me to the blink board but now I see it makes more sense to do my own
```

---
## \#29 Posted by: Badrish Posted at: 2017-04-02T21:59:12.235Z Reads: 109

```
How has it worked out for you? I ordered a power bank and I am just asking people if it works. Not sure if it will screw up the battery or the charging port but I will take my chances.
```

---
## \#30 Posted by: admiralackbar Posted at: 2017-05-21T18:40:41.159Z Reads: 102

```
i have the same board... 

what i have been trying to do is find a hub motor that has the same "specs" as the blink board motor... to swap out and plug the 3 motor wires into... this is because i am also swapping out the "deck" for an 6 foot long deck that i am selling... but my customers dont like the idea of the front trucks being very wide and low... and the back trucks being the standard acton blink board trucks... i need a way to use the acton blink motor on VERY wide and low trucks that fit my board... or to swap in a hub motor that fits on ANY truck..

i have been told that hub motors also require special truck brackets? are there hub motors that can just slide onto any truck... 

furthermore... will this hub motor fit the specs of the acton blink board battery compartment... the reason i want to use the acton blink battery is solely because... i have imax chargers and prefer the simple AC plug in system that off the shelf boards have...
```

---
## \#31 Posted by: free888368 Posted at: 2017-11-15T05:32:26.947Z Reads: 85

```
i had a Blink S , the battery almost dead:joy:. can i change the battery by myself?
```

---
## \#32 Posted by: Mikenopolis Posted at: 2017-11-15T05:43:17.243Z Reads: 88

```
Dead? As is not taking a charge any more? How long have you had the board. Use it often. I would think they have enough recharge cycles to last longer. 

You will have to open it up and see what’s inside. They advertised it as Samsung Li-ion but that’s all I know. Shouldn’t be hard to put a new pack together if you know how. Or someone like @barajabali or @willpark16 will assist with battery pack builds
```

---
## \#33 Posted by: willpark16 Posted at: 2017-11-15T06:01:32.631Z Reads: 90

```
Does the blink have bms attached to battery?
```

---
## \#34 Posted by: free888368 Posted at: 2017-11-15T06:18:39.179Z Reads: 88

```
.<img src="/uploads/db1493/original/3X/1/2/129ecd51053334ee392e993c891f19f794613c4f.jpg" width="666" height="500"> 
i use it about eight months:blush:
```

---
## \#35 Posted by: free888368 Posted at: 2017-11-15T06:21:53.651Z Reads: 84

```
i think i will buy a new pack battery:wink:.
```

---
## \#36 Posted by: Mikenopolis Posted at: 2017-11-15T06:27:21.228Z Reads: 84

```
Was is a good/fun 8 months? Personally, I had a horrible experience with Acton so I’ll never buy anything from them again. 

Their battery shouldn’t be too large, this not too much to replace if you want to keep that board.
```

---
## \#37 Posted by: Mikenopolis Posted at: 2017-11-15T06:28:58.816Z Reads: 86

```
Hard to tell by this picture, but their old blink board did. I don’t see why it won’t now
```

---
## \#38 Posted by: free888368 Posted at: 2017-11-15T06:59:18.770Z Reads: 87

```
[quote="Mikenopolis, post:36, topic:8623"]
horrible experience
[/quote]

Can U share with us ? thanks buddy:scream:
```

---
## \#39 Posted by: willpark16 Posted at: 2017-11-15T07:01:56.434Z Reads: 87

```
10s1p? That's pretty small I'd say u need 26650s
```

---
## \#40 Posted by: Mikenopolis Posted at: 2017-11-15T07:16:31.670Z Reads: 89

```
Trying to keep is short. 

I had the original Blink belt board for a while, they offered a $160 ($100 and roughly $60 shipping to and from) upgrade to a hub motor a few months later and I jumped on it. That drive looked like it was repaired because of the hot glue mess on the hubs. They denied it. The drive died after a mile of slow ride. They refused to replace the drive. After two months of trying to get a response from their online support page they finally started to respond. Eventual resolution was they sent me a Blink Lite as a replacement. I told them I was 210lbs and that it was a useless boards but they did not care that they were sending me something I cannot use. I got it, rode it up and down the block and wanted to set it on fires. Eventually I sold it to someone here for $100. Didn’t want it to go to waste.
```

---
## \#41 Posted by: Selzier Posted at: 2017-11-23T02:34:19.369Z Reads: 81

```
I have a Blink S board that will only charge to 70% and will only travel for about 3 miles. Can I buy or build a new battery pack?

Here's what's inside the Acton Blink S:

Battey Pack:
https://s18.postimg.org/xuixp6yrt/Blink_S1.jpg
```

---
## \#42 Posted by: Selzier Posted at: 2017-11-23T02:34:51.221Z Reads: 80

```
PCB:
https://s18.postimg.org/gu01gie0p/Blink_S2.jpg
```

---
## \#43 Posted by: aigenic Posted at: 2017-11-23T17:03:07.386Z Reads: 71

```
Yes you can :slight_smile:
```

---
## \#44 Posted by: Inkowalski Posted at: 2018-03-29T21:35:17.198Z Reads: 58

```
I recently bought an Acton Blink S California Bear (1st Gen) and I have the same problem described here, although the charge meter indicates 80% low voltage and the skate is turned off and on several times and left to be supplied energy to the engine.
I have no idea what battery should buy for this or if I should mount the BMS of the old battery in the new or how to do it.
Can someone help me?
```

---
## \#45 Posted by: Mikenopolis Posted at: 2018-03-29T21:53:16.582Z Reads: 63

```
[quote="Inkowalski, post:44, topic:8623"]
Acton Blink S California Bear
[/quote]

If you are saying "California Bear" then you have a BLINK not a BLINK S. Single motor belt drive, not hub right?
```

---
## \#46 Posted by: Inkowalski Posted at: 2018-03-29T21:59:07.244Z Reads: 62

```

I must have been wrong, in a reference on another page they called it "california bear". It has a single motor hub.

![image|666x500](upload://flR9mXg58BOKTJltSY7rGFW0ILz.jpg)
```

---
## \#47 Posted by: Mikenopolis Posted at: 2018-03-29T22:07:26.362Z Reads: 59

```
Ahhh, that's kinda the 2nd generation Blink board, basically they took the first generation single belt and swapped in a single hub.

I think @Tomer might be able to give you some pointers as he's modified one before
```

---
## \#48 Posted by: Erod Posted at: 2018-03-29T23:40:51.159Z Reads: 61

```
Post if you find a solution! My Blink S is dying and it's the same battery.. Battery will read %100 but torque/acceleration is affected.
```

---
## \#49 Posted by: Mikenopolis Posted at: 2018-04-01T03:46:43.432Z Reads: 59

```
@Inkowalski  @Erod 

Just saw this on Facebook.

![image|363x500](upload://fZjd8jXWEd4p1P7OSHY7pxSwj9U.jpeg)
```

---
## \#50 Posted by: 99Questions Posted at: 2018-05-18T13:00:14.130Z Reads: 47

```
How does it all end? Opened my board and now weighing out the options.
```

---
## \#51 Posted by: admiralackbar Posted at: 2018-07-04T14:30:46.534Z Reads: 32

```
so that battery in the acton blink is 10s1p ????

doe that mean i can use this battery on a 36v hub motor and a maytech 50A esc?

the motor is 100Kv
```

---
## \#52 Posted by: Grozniy Posted at: 2018-07-04T14:38:41.801Z Reads: 29

```
You can but the battery output will be very weak. This will shorten the life of it. Unless you go very conservative on vesc config. The escs they use pull less current than vescs. More amps you pull, hotter the battery will be, shorter life cycle and probably more dangerous.
```

---
