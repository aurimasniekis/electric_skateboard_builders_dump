# What amp/watt are most people having success with? Are 10a 18650&rsquo;s strong enough?

### Replies: 54 Views: 2606

## \#1 Posted by: D_Sk8 Posted at: 2017-09-26T17:17:01.409Z Reads: 238

```
I got a hold of 200 2000mah 18650's, which are 10a continuous / 20a max, and not certain that's going to be good enough for my pack. I figure a 12v3p, but not certain if I should go with 4p.

I'm looking at using v4.12 of Vedder's ESC, which has a continuous 50a and either the 6355 190KV or 6374 190KV 3150W. Both are 80amp max.

With 12s/3p i'm looking at 30a continous / 1152-1512 watt (cutoff at 3.2v to 4.2v x 12)  or 60a / 2304 - 3024 max (2664 watt peak at nominal voltage.

https://www.electric-skateboard.builders/t/question-about-max-amps-and-overheating-motors/14795

The above post mentions people topping out the amperage (meaning they have packs that can handle up to 150amp), so my concerns is I am going to be working with a weak power source? Should I ditch these batteries for this project?

In summary, what are people using? The  video walking through how to configure the VESC has a max amp setting of 40 amp (I believe at 12s, but might have been 10s), but 

https://www.youtube.com/watch?v=5HLZaMcYRuY

^^ at 27:21 configures the VESC at 30amp, in a dual setup (so 60amp) (12s)

and 

https://www.youtube.com/watch?v=1TF8XARDa6U

^^

Sets his at 25amp (total) 12s.

Does it all really matter that much? I am not a small person. 220lbs. Will going with the higher watt motor be redundant unless I can increase the amperage, or am I way over thinking this since this really only comes into play going up hill and getting up to speed (although acceleration is one of the main points of performance I am concerned about).

I've read some details that a larger watt motor pulling the same current will provide more torque (I couldn't find much detail or proof behind this, so I am not certain whether that's true), but provide less distance, which isn't a major concern for me (I can always run another parallel if needed), but in my case, a 3p pack will max out at 2664 peak watts at nominal voltage, so would it even make sense to go with the 3150 watt motor?

Long story short, I am building a battery pack and need to know what motor to buy and what type of pack to build and whether I should get some high C rated batteries to do that. It will also decide what BMS I use. If I need to get closer to the max 50amp continuous the VESC can handle, i'll just add more batteries and get a more expensive BMS (vs the 30a BMS I am looking at).

What's everyone else working with? Do we have many lower C rated li-ion packs being used for E-Skates?
```

---
## \#2 Posted by: XIII Posted at: 2017-09-26T17:55:42.442Z Reads: 194

```
On my dual direct drive i pull 40A in Total. SO 20a each vesc!

On my single I have set the vesc to 40 A aswell! Performance is great. I don't need more
```

---
## \#3 Posted by: Okami Posted at: 2017-09-26T17:57:49.446Z Reads: 199

```
Ok this is still fresh.. so will try to clarify a few thins before going into more detail..

Are you planning to ride at 40-50kph (25-30mph) mostly?

Are u planning to up hills?

Do you want to experience / enjoy insane acceleration?

Otherwise I think no more than 1000W are needed..

I think @ackmaniack himself could confirm that for 'general crusing' no more than 400w might be needed (and perhaps about 800w for 'decent' acceleration)..

And yeh.. you can always limit max current since you are planning to go with vesc, which is a big plus, I think..
```

---
## \#4 Posted by: cwazy1 Posted at: 2017-09-26T17:59:57.858Z Reads: 196

```
I use 2900mAh @ 10A cont and 20A burst in a 12s4p configuration. I have my two vescs set at +15a  for battery max and it is plenty. Anymore than that and I'd probably have a harder time with fine adjustments.
```

---
## \#5 Posted by: D_Sk8 Posted at: 2017-09-26T18:17:08.251Z Reads: 188

```
Thanks XIII.
```

---
## \#6 Posted by: NickTheDude Posted at: 2017-09-26T18:24:24.999Z Reads: 186

```
For my single motor build I have my go with a batt max of 40A. For my dual I do 35A on each. However I've been tainted by intoxicating power and I weigh about 190lbs. You likely won't need 70A, especially if you're not climbing any hills. Both boards are using TBs 190kV 6355 motors and they handle the heat fine.

The amount of power you need is really subjective and comes down to your use case. My dual drive can push me up pretty much anything and accelerates hard enough to knock you on your ass while the single struggles with hills and is much tamer.

A few other notes:

Power/amp ratings on motors are usually complete bullshit and shouldn't really be considered. Bigger motor = more copper = less heat = higher efficiency. Bigger is always better unless it's unnecessary for the amount of power your battery/VESC is putting out. With your kind of power you really shouldn't have to run anything bigger than a 6355.

A 12S3P with 10A cells would only be able to safely output 1332W and even then people always recommend that you set you settings to leave some headroom so you don't reduce the lifespan of your pack. What kind of cells are they?

Yes, lower C rating lipos are commonly used, however people usually take the C ratings with a grain of salt and assume the packs are only good for roughly half of what their rated for.

Everybody used to use Samsung 25Rs (20A 2500mAh) cause of their high discharge rates, since then people have moved to Samsung 30Qs (15A 3000mAh) because despite them being rated at 15A they actually preform better than 25Rs at 20A.
```

---
## \#7 Posted by: D_Sk8 Posted at: 2017-09-26T18:28:23.810Z Reads: 161

```
[quote="Okami, post:3, topic:34008"]
Are you planning to ride at 40-50kph (25-30mph) mostly?
[/quote]

 (probably 25 to start, and increase to no more than 30)

[quote="Okami, post:3, topic:34008"]
Are u planning to up hills?
[/quote]


Not a large amount of them, no. I live in Vegas which is pretty flat, but there are some hills (nothing like S.F. though). I'd say the biggest hill is the one headed West, which is about 450 foot incline over the course of 10 miles, so there aren't really any steep hills.

[quote="Okami, post:3, topic:34008"]
Do you want to experience / enjoy insane acceleration?
[/quote]

Yes, I'm a speed freak for sure. I won't really rest until I know I'm getting the best bang for my buck in terms of performance. I won't put a great deal of money to gain 10% performance, but if the return on investment makes sense, I will upgrade. I just don't want to be sitting at, for example, 30%-50% power while having a weak batter.

[quote="Okami, post:3, topic:34008"]
I think @ackmaniack himself could confirm that for 'general crusing' no more than 400w might be needed (and perhaps about 800w for 'decent' acceleration)..
[/quote]

That sounds pretty good then. If I can get some good performance out of 1200 watt, then I think this will work, and even then that's a 3p. I haven't got my board so not 100% certain how big a 4p will look. It's a 42" board so I doubt I'll have an issue going to 4p, but even then that's only 1500 - 1800 watt max, but from what you're saying, that should be more than enough?
```

---
## \#8 Posted by: NickTheDude Posted at: 2017-09-26T18:36:04.804Z Reads: 146

```
There are some videos on youtube with VESC performance readouts overlayed on top of people riding their boards. You could probably watch a few to get an idea of what kind of wattage people are drawing.

These two are pretty crazy boards:
https://www.youtube.com/watch?v=vNNcW0CIh5Y
https://www.youtube.com/watch?v=0PNWIaXaFvw

A less intense boards:
https://www.youtube.com/watch?v=Y-XAAU8Q0YU
```

---
## \#9 Posted by: D_Sk8 Posted at: 2017-09-26T18:36:42.603Z Reads: 134

```
[quote="NickTheDude, post:6, topic:34008, full:true"]
For my single motor build I have my go with a batt max of 40A. For my dual I do 35A on each. However I've been tainted by intoxicating power and I weigh about 190lbs. You likely won't need 70A, especially if you're not climbing any hills. Both boards are using TBs 190kV 6355 motors and they handle the heat fine.

The amount of power you need is really subjective and comes down to your use case. My dual drive can push me up pretty much anything and accelerates hard enough to knock you on your ass while the single struggles with hills and is much tamer.

A few other notes:

Power/amp ratings on motors are usually complete bullshit and shouldn't really be considered. Bigger motor = more copper = less heat = higher efficiency. Bigger is always better unless it's unnecessary for the amount of power your battery/VESC is putting out. With your kind of power you really shouldn't have to run anything bigger than a 6355.

A 12S3P with 10A cells would only be able to safely output 1332W and even then people always recommend that you set you settings to leave some headroom so you don't reduce the lifespan of your pack. What kind of cells are they?

Yes, lower C rating lipos are commonly used, however people usually take the C ratings with a grain of salt and assume the packs are only good for roughly half of what their rated for.

Everybody used to use Samsung 25Rs (20A 2500mAh) cause of their high discharge rates, since then people have moved to Samsung 30Qs (15A 3000mAh) because despite them being rated at 15A they actually preform better than 25Rs at 20A.
[/quote]

Those are actually what I was just researching too, in terms of what I would upgrade to if the 10a weren't going to push enough.

The batteries are LGDAMF11865, bought below.

http://www.ebay.com/itm/10-LG-36V-4-4AH-BATTERY-PACK-18650-EBIKE-VAPE-POWERWALL-BATTERIES-200-CELLS-BMS-/201916138726?hash=item2f0323c4e6:g:nKUAAOSwuspY9YNZ

By way of:

https://www.youtube.com/watch?v=6YTToSxAdV8&t=7s

^^ Jehu's got some decent video's about battery tech that got me interested.
```

---
## \#10 Posted by: D_Sk8 Posted at: 2017-09-26T18:38:05.249Z Reads: 127

```
[quote="D_Sk8, post:9, topic:34008"]
By way of:

eBay's  $1 per LGDAMF11865 Cell Deal is BETTER  than expected

^^ Jehu's got some decent video's about battery tech that got me interested.
[/quote]

It's interesting though, that and 

http://www.staringpower.com/product/lgdamf11865-18650-2200mah/

Both state a max continuous discharge of 20a which doesn't seem to line up with the 10a the seller is advertising.
```

---
## \#11 Posted by: D_Sk8 Posted at: 2017-09-26T18:38:38.084Z Reads: 121

```
Sick, let me check those out. Thank you
```

---
## \#12 Posted by: Okami Posted at: 2017-09-26T18:46:20.819Z Reads: 121

```
yeh, these sort of videos are good source of info.. you should check to find your 'sweet spot' for power..

Honestly.. I dont have real data about 'where the real fun starts''.. I just know that 1000W of power should work quite good (for single drive).. for dual you probably would need 1500w minimum I think, to have decent 'kick'·

Though.. I have limited experience but I know that you dont need that many watts to reach these speeds and acceleration should be pretty scary anyways with these smaller (non-pneumatic) wheels anyways.

--

If possible, I would recommend to meet up with someone and test their board.. ideally they have the same app to monitor power levels, so that you can see how much power is 'enough'.

Some might claim 2000w is still not enough for them.. and that they 'feel good' only with 3000w of power.. though I think this would really go for power hungry boards and would probably be a dual system already.
```

---
## \#13 Posted by: D_Sk8 Posted at: 2017-09-26T18:56:59.757Z Reads: 119

```
[quote="NickTheDude, post:8, topic:34008"]
These two are pretty crazy boards:
[/quote]

That's pretty sick and helps a lot in terms of comparing things I wasn't able to find answers for. Thank you.

The less intense board still seems to do what i'm hoping it would. It peaks out over what amp I can obtain, but also notice he's running lower volts. In the end I think I can do a little better peak/continuous watts while running about the same peak amps for a shorter period of time.
```

---
## \#14 Posted by: D_Sk8 Posted at: 2017-09-26T18:59:09.121Z Reads: 114

```
[quote="Okami, post:12, topic:34008"]
Some might claim 2000w is still not enough for them.. and that they 'feel good' only with 3000w of power.. though I think this would really go for power hungry boards and would probably be a dual system already.
[/quote]

Yeah, that seems crazy now that I am watching the videos. I think I will go with 4p though, to get to that 1500 watt mark. I'm going to start with 1 motor, then add another when I get the cash. I think at this point, though, I will stick with the smaller motor and only consider the bigger motor if I get some higher discharge batteries.
```

---
## \#15 Posted by: D_Sk8 Posted at: 2017-09-26T18:59:40.039Z Reads: 113

```
Thanks a lot all, this helps a lot.
```

---
## \#16 Posted by: Vanarian Posted at: 2017-09-26T19:06:48.218Z Reads: 112

```
Thanks for the videos, it was very useful. Actually making me hope to get a good performance at 3200W (2x1600W) despite 50mm size. The calculator already gave out pretty nice numebrs but it is difficult to "comprehend" without seeing it.
```

---
## \#17 Posted by: NickTheDude Posted at: 2017-09-26T19:23:00.564Z Reads: 109

```
No problem, another good resource for comparing cells is this dude called Mooch from the vaping community that has been testing different cells on the market.

You can see his results here: https://www.e-cigarette-forum.com/forum/blog-entry/18650-battery-ratings-picking-a-safe-battery-to-vape-with.7447/
```

---
## \#18 Posted by: D_Sk8 Posted at: 2017-09-27T16:20:52.664Z Reads: 108

```
[quote="NickTheDude, post:17, topic:34008, full:true"]
No problem, another good resource for comparing cells is this dude called Mooch from the vaping community that has been testing different cells on the market.

You can see his results here: https://www.e-cigarette-forum.com/forum/blog-entry/18650-battery-ratings-picking-a-safe-battery-to-vape-with.7447/
[/quote]

Thank you, I would have replied earlier but I am a noob and can only post so many times a day.

I decided, screw it. The packs I bought have 20 batteries each so I might as well just use all 60 of them and do a 12s5p.  I don't have the board yet, so it's hard for me to determine whether 2 rows of 30 will fit. It's 24" by length, and I think only 60% of the 42" board is available for the pack (which amounts to 25.5" or so, which leaves no room for the controller unless I put it on the side). With the black battery brackets, going 3 rows across is 8", which only gives me 1.5" of lip and room for screwing the enclosure down, assuming the whole board is 9.5" across.

I'll create another post and link it here once I start building the pack. I am hoping the 2 rows fit, otherwise I'll have to figure out how to pack and wire 60 batteries sideways which seems more difficult.
```

---
## \#19 Posted by: D_Sk8 Posted at: 2017-09-27T17:28:23.742Z Reads: 94

```
Actually, if 12s5p and controller/bms doesn't fit on the board in a 24" length formation, I either have to take the brackets off and glue them or stack them, which I don't really want to do (but not certain of the clearance yet), or reduce to 12s4p.
```

---
## \#20 Posted by: Okami Posted at: 2017-09-27T20:13:34.348Z Reads: 99

```
Ok tested my 'mountainboard' setup today.. pulled about 650W of power going almost max speed, when battery was at about 55%.. though it sags a lot,.. so with sag included it showed about 15%.. which translated to about 1.5-2v sag from total capacity of the pack (if i remember correctly and meter does not lie).. I think it might translate to about 0.3v or so sag per cell group.. 

Dunno if this matters to you.. but yeah.. this is with 6s and 4.33 gearing, 9inch tires.. dunno how much you might need..
```

---
## \#21 Posted by: D_Sk8 Posted at: 2017-09-27T20:45:22.568Z Reads: 86

```
Thank you.

I think I've ditched the idea of trying to make a compact battery enclosure and am going to do a full 12s5p. At least then I can run 2 motors and not worry too much about things.

Thanks for the heads up.
```

---
## \#22 Posted by: thisguyhere Posted at: 2017-09-27T21:00:10.217Z Reads: 87

```
[quote="Okami, post:20, topic:34008"]
pulled about 650W of power going almost max speed
[/quote]

max speed won't get u Max current draw. you'll draw max amp during hard acceleration, I've pulled 100a for dual 6374s on 107mm thane wheels.
```

---
## \#23 Posted by: D_Sk8 Posted at: 2017-09-27T21:02:47.936Z Reads: 83

```
I'm not as worried about speed, than acceleration and getting my fat arse up to speed. There's some conflicting info on the batteries. 20 amp max continuous seems to be double that of what the seller is suggesting. Even if it's peak, at least with 12s5p I can peak at 100amp, and continuous at 50a.
```

---
## \#24 Posted by: Okami Posted at: 2017-09-27T21:40:58.812Z Reads: 84

```
Well, i dont have the nice vesc or vesc app but meter shows about 1000w for acceleration. Usually it does.not peak over 50-60amps and as today witnessed about 35amps when battery is.lower to go at constant speed.

Forgot.to mention ive got turnigy sk3 192kv motor.

I will check these vesc app videos myself once again, that @BigBoyToys board looks rather interesting entrant to energy consumtion game


---
So yes 50amp for dual might be just right for peak but as people have been talking before what counts more is.the continous current.. i think these short bursts of power.dont heat up the batteries as much compared.to constant load.. though would like to confirm this with video and temp sensor (someone with vesc app and temp monitor in batteries?)
```

---
## \#25 Posted by: scepterr Posted at: 2017-09-27T21:50:03.441Z Reads: 82

```
@D_Sk8
Don't use those cells at 10A each, assume and plan for 5A each, they will sag significantly at 10A each and get hot,. I've got almost $2k of these cells, about 300 of them in boards being ridden currently.
Building a board with 4 packs currently, 20A batt max is what will be set in vesc
<img src="/uploads/db1493/original/3X/6/4/64739466e78af15b95566081449c398a139cbbb4.jpg" width="690" height="274">
```

---
## \#26 Posted by: Okami Posted at: 2017-09-27T21:56:05.792Z Reads: 79

```
Thanks for extra.info. i didnt personally go into too much detail about his cells but building 12s 5p pack  sounds wise.. should give plenty of power even at 25amps at about 43.2v = ~1100w
```

---
## \#27 Posted by: scepterr Posted at: 2017-09-27T22:10:41.955Z Reads: 80

```
If using the eBay packs 10S is the only option unless rebuilding the packs, you can do 10S2P,4P,6P,8P,10P
Also the BMS are rated for 10A discharge max on all of those packs
```

---
## \#28 Posted by: Okami Posted at: 2017-09-27T22:11:45.980Z Reads: 78

```
Yeh he might need to consider this, 12s is also no good for most vescs
```

---
## \#29 Posted by: D_Sk8 Posted at: 2017-09-28T02:59:56.455Z Reads: 74

```
When you set a 20A batt max, does that mean max peak, or is that max continous? Does the VESC take into consideration peak at all, or is it 1 single setting, and it'll stick to that amperage regardless of the peak battery capabilities?

5a is much less than what the seller is suggesting it supports. It's also much less than the technical details of the battery. That's pretty disappointing.
```

---
## \#30 Posted by: D_Sk8 Posted at: 2017-09-28T03:07:36.128Z Reads: 74

```
Do you think this would be a better bet?

http://www.ebay.com/itm/201916140363?rmvSB=true

I think it's the same seller, but different batteries, double the claimed C rating.
```

---
## \#31 Posted by: scepterr Posted at: 2017-09-28T03:15:28.014Z Reads: 69

```
That does not look legit and seems to be removed already lol
That's cont current, burst current gets filtered by vesc, if you burst over 130 for too long it'll trigger over current fault. That's the abs current max setting below battery motor max/min, limit is 150A burst
```

---
## \#32 Posted by: D_Sk8 Posted at: 2017-09-28T03:25:26.770Z Reads: 70

```
Thanks.

The link is still there. It's via Jehu's youtube. Looks like they sold out of the batteries in the video, and he linked an alternative. Lower MAH rating but higher C rating. 

https://www.youtube.com/watch?v=tTetQ37ZKIU&t=468s

If those LG's can't handle 10a continous, i'll probably use them for a prototype single drive and see how they do. Sell it, then get some better batteries and build a dual drive, or stronger single drive.
```

---
## \#33 Posted by: scepterr Posted at: 2017-09-28T03:30:12.424Z Reads: 68

```
The 22p is identical to mf1
Regardless of whether they can, the BMS is 10A limited....so you cant draw more than that without replacing bms
```

---
## \#34 Posted by: D_Sk8 Posted at: 2017-09-28T03:31:56.996Z Reads: 71

```
I pulled the batteries out of the pack and am going to build a 12s5p pack with 12s BMS.
```

---
## \#35 Posted by: scepterr Posted at: 2017-09-28T03:32:49.673Z Reads: 72

```
Don't forget to rewrap them and insulate them
```

---
## \#36 Posted by: D_Sk8 Posted at: 2017-09-28T04:00:39.183Z Reads: 73

```
That is odd. I clicked the link again and I got that the listed was deleted, but clicked it again and it was there again. Odd.

I think the 22p was what they were originally trying to sell. The new link refers to Sona batteries but there's no mention of a model number. Only that the "actual" capacity is now about 2000mah. The date is from 2015.

Yup. It's a project, still learning but want to make certain it's done right.

I'll probably get a bulk of the Samsung 25R and be done with it if the seller can't prove those Sona's can handle 10a.

I guess I could buy a pack and test them. See if the voltage sags at 10A-15A.
```

---
## \#37 Posted by: scepterr Posted at: 2017-09-28T04:05:08.305Z Reads: 70

```
I've never seen or heard of Sona cells, that's a red flag to me, considering...😋
<img src="/uploads/db1493/original/3X/3/3/33015b97a753e8dff6e4030aa01d9cb95f31844e.jpg" width="666" height="500">
```

---
## \#38 Posted by: D_Sk8 Posted at: 2017-09-28T04:13:23.185Z Reads: 70

```
Yeah, the only reference I see online is his ad.
```

---
## \#39 Posted by: D_Sk8 Posted at: 2017-09-28T04:13:56.186Z Reads: 69

```
Any suggestions on the most economical battery to use?
```

---
## \#40 Posted by: scepterr Posted at: 2017-09-28T04:18:50.270Z Reads: 71

```
As far as 18650 the mf1 or 22p packs are the cheapest
One other thing I should mention it's very likely that new fresh mf1 or 22p would perform better at 10A, these cells are a couple years old and stored in unknown conditions. They test with good resistance and capacity and perform reasonably well if you have the right expectations...you did pay $1-$1.25/cell 😉
```

---
## \#41 Posted by: thisguyhere Posted at: 2017-09-28T04:34:22.071Z Reads: 67

```
focbox, ollin, vesc6 all for fine on 12s. pretty sure TB too as long as it's not pushed too hard. 

running dual focbox 12s, no issues yet and way over powered.
```

---
## \#42 Posted by: D_Sk8 Posted at: 2017-09-28T04:34:52.353Z Reads: 68

```
That's true. The eSk8 is actually my 4th project to do the batteries with. I originally bought them for a clone SoundBoks and to build a remote 12v water mister (It gets 117 here), to run on a boat during the summer. All that stuff is low amp. I didn't start thinking about the Sk8 until watching Casey Neistat's videos (Started with Jehu's channel and he mentioned Casey a couple times, I had never heard of the guy.)

I'll give it a shot and see what happens. If I have to tone it down and find someone half my size to sell it to, i'll build another one and get better batteries.
```

---
## \#43 Posted by: scepterr Posted at: 2017-09-28T04:40:34.890Z Reads: 65

```
They are great for low current use or where size/weight isn't an issue, 10S20P can chug along at 100A with 44Ah capacity at $250 and all you have to do is make a bus bar to plug all of them into
```

---
## \#44 Posted by: Okami Posted at: 2017-09-28T04:45:41.407Z Reads: 64

```
Well 10s20p is just crazy. I could imagine ebike with 200 battteries but not eboard.. 60cells alone will be closw to 3kg in weight /6 lbs probably
```

---
## \#45 Posted by: D_Sk8 Posted at: 2017-09-28T04:46:31.685Z Reads: 64

```
I think he's talking about other uses, like a cheap PowerWall or something.
```

---
## \#46 Posted by: Okami Posted at: 2017-09-28T04:55:35.979Z Reads: 62

```
It could be.. i suppose that 200cell, 100amp number was.just for reference, afterall jehus videos were about powerwalls probably too
```

---
## \#47 Posted by: scepterr Posted at: 2017-09-28T05:01:38.991Z Reads: 67

```
I specifically said "where size/weight isnt an issue"
I have 1 client with 2 boards each 10S10P :wink:
Transitioned from 6 lead acid batteries on each board which weighed even more and had less capacity
I think it was  only 8.8Ah with the sla batteries..crazy
```

---
## \#48 Posted by: Okami Posted at: 2017-09-28T05:04:00.194Z Reads: 69

```
Hah thanks for info, didnt know such huge battery setups werea thing for some. I think largest ive seen is about 80cells or so (on forum)

So what range does he get? Do u know? Sounds like he could do 50km / 30miles easily.
```

---
## \#49 Posted by: scepterr Posted at: 2017-09-28T05:05:25.599Z Reads: 66

```
Mid-rebuild
<img src="/uploads/db1493/original/3X/3/e/3e50290243246c8a97f84153eb4d121e052f52de.jpg" width="666" height="500">
Originally fit 10S8P, but was able squeeze another pack in moving some stuff out of the enclosure
```

---
## \#50 Posted by: Okami Posted at: 2017-09-28T05:06:44.317Z Reads: 65

```
Yeh i had suspicion it might be one of these boards and not typical longboard :) they are heavy as hell with the stock batteries, thats for sure.. so fitting huge range, less weight li ion pack is a big saving

Could comment on the board but that would be offtopic.. otherwise.nice.choice. 

Interesting trucks (in front) and the deck also looks like made from aluminium, so.i suppose this isnt typical e-glide?
```

---
## \#51 Posted by: D_Sk8 Posted at: 2017-09-28T17:13:12.659Z Reads: 62

```
I'm taking a chance and bought 10 packs of them. Worst case I'll use as an off grid power source. I've got a 3k solar array on the house so I'm sure I can make use of them. I'll let you know what I find. jehu has a pretty good reputation. If they suck, I'll make certain he's aware of it.
```

---
## \#52 Posted by: E1Allen Posted at: 2017-11-18T00:59:36.544Z Reads: 47

```
So the Sona cells. Did anyone buy and try these yet?
```

---
## \#53 Posted by: D_Sk8 Posted at: 2017-11-18T16:58:50.627Z Reads: 40

```
I did but have so many projects going I haven't built a battery load/heat tester yet. My LG battery pack just got welded and am waiting on the BMS from China before I can finish it. I could test without it but just don't have time, kinda stalling.
```

---
## \#54 Posted by: aponty Posted at: 2017-11-18T19:43:14.896Z Reads: 38

```
I'm curious about this as well, looking forward to hearing the results!
```

---
