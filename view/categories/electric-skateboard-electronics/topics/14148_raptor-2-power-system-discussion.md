# Raptor 2 - power system discussion

### Replies: 55 Views: 4403

## \#1 Posted by: evoheyax Posted at: 2016-12-03T01:28:02.056Z Reads: 348

```
I've been thinking about your claims @onloop, and I found a flaw in your logic... You say the bottleneck right now is the vesc and while that is a bottleneck, what about the battery? At 10s3p, your getting a manufacturer rated 60a max which will sag heavily and drastically reduce the cels life. It's really more like 40a max to have fair sag, 30a to have little sag. The current vesc v4.12s can do that already (even vedder said in his new video last week that the current vesc 4.12 can do 23 amps continuous, or 46 amps continuous between the 2 without heating up, which is exactly what my real world testing has shown me).

It seems like the real bottle neck is and still will be the fact your using a relatively low discharge battery made of 18650s, and you'll be able to tap into only a fraction of the motors power with such weak batteries...

But you can't even see this necessarily because you don;t even have working prototype yet. You'll find out that there's many surprises in working with hubs in general. I think you would have been better off waiting until you had your "upgraded" motor working, instead of rushing this release without even testing the "upgraded" motor.
```

---
## \#2 Posted by: onloop Posted at: 2016-12-03T13:31:19.302Z Reads: 321

```
We don't use VESC. We developed a new version  that is far superior, it's called VESC-X. we also use 10s4p battery. 

Dont hesitate to ask when you need some engineering help building your 4WD eboard with outrunner adapted hub motors and old style vescs.

Also if you could use sone advice on marketing your start up too im Happy to help.
```

---
## \#3 Posted by: evoheyax Posted at: 2016-12-03T16:31:54.202Z Reads: 304

```
I've learned so much watching what you do already in marketing lol.

Still, even at 10s4p, 80 amps continuous rated by the manufacturer, 50 amps really to bring the sag down to a reasonable level. The current vescs can handle 25 amps each anyways (not forever, but for a few minutes, once your back under 23 amps, they start dropping in temp again).

The real problem is your still running relatively low amps li-ion batteries and hubs.  I estimate around 150 amp continuous battery is what you want, as 100 amps (50 per vesc) is really what you want. Current vescs can't do 50 con but the vesc 6 will, which might be out before your board ships.

You still have a bottle neck in your system.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-12-03T16:41:01.966Z Reads: 292

```
[quote="evoheyax, post:408, topic:12694"]
Current vescs can't do 50
[/quote]

Probably you miss that tread, and some reason why he use the vesc-x 

http://www.electric-skateboard.builders/t/vesc-x-lab-test/12461
```

---
## \#5 Posted by: evoheyax Posted at: 2016-12-03T16:52:25.121Z Reads: 277

```
I know why he uses the vesc x. My point is, I think the raptor 2 gains nothing from the vesc x, because the battery can't do high amps. The current vescs can do the max con amps that battery can do. The whole vesc x is pointless (except in a mono drive) until he uses a battery with a higher continuous amps.
```

---
## \#6 Posted by: Ackmaniac Posted at: 2016-12-03T17:05:33.454Z Reads: 280

```
Can you please be a bit more precise why the battery should be the weak point? Maybe you can post a screenshot of your actual VESC settings and some details about your board to it (battery S and P, dual or single, street or AT) to bring some clarification here.
```

---
## \#7 Posted by: evoheyax Posted at: 2016-12-03T17:24:48.385Z Reads: 283

```
Everything you need to know about my board is here: http://www.electric-skateboard.builders/t/the-rocket-4wd-hummies-hubs-4x-chaka-vesc-10s4p-lg-he2-li-ion-cnc-milled-veneer-pressed-deck/8123

Right now, I limit my four vescs to 74 amps total (16 per vesc). The cells are rated to 80 amps max. The vescs 4.12 can do about 23 amps each without heating up at all, so 25 amps continuous is not an issue. For that reason, a battery that can push 100 amps without sagging would be ideal with the current vescs and 4WD.

The reality is, 4WD is more expensive, and won't be practical for everyone. 2WD will save $200 of a boards price, which cosumers want. The problem with 2WD, is the vescs can't do 50 amps con without major heat up and eventual shutdown. The vesc-x fixes this bottle neck (the vesc 6 will also, and there's another guy working on an FOC esc (non vesc based) which can handle much higher amps), but, even if these new vesc-x's can take 50 amps continuous without heat issues (which I know, testing says, we'll see when my beta vesc-x arrives), the battery can't supply the current needed. The current battery will likely be limited to 40-50 amps. Each VESC-X needs 40-50 amps to tap fully into the power of the motors (and for there to be a reson to have the VESC-X instead of the current VESCs). So you would need at least 2 space cells to supply enough current. The problem is, this battery was great for satellite drive, but it doesn't convert over to hubs as nicely. You need a battery that can give higher amps, or the VESC-X is useless.

Bare in mind, the numbers I give are from testing at 12s. Since your at 10s, you need even more amps. Hubs love 12s, this has been stated by many in the community. This is the problem though with everyone preordering a board that hasn't been build yet or tested. There is no working board right now, and I'm sure when he gets these motors, Jason will realize this, and try to come up with a solution. But right now, the only solution is lipos, which aren't the best of solutions. Or a massive li-ion battery, like chakas free ride boards have. But a 10s4p is not a very large battery for 18650s and hubs.
```

---
## \#8 Posted by: Ackmaniac Posted at: 2016-12-03T17:51:38.477Z Reads: 253

```
The batteries are rated to 20 amps each which is 80 amps on a 4P setup. I don't know why it should be less? I quickly read the thread you were writing about your board and i couldn't see that you mentioned that the battery is too weak. 
You switched to 12S which is cool but i guess mostly because of the higher speed. I even have a 12S8P btw, but thats another story.

Then you are a heavy rider with a extreme ride style, you mentioned 38 mph. (<- respect). That means a 33 % higher gear ratio which results in 33% more amps to draw and you mention that you have a lot of hills in your area. 
I still don't see something that shows that the batteries are not capable and also not in your boards thread where you say that they are the bottle neck. 
And there are a lot of test available that show that the batteries are capable of 20 amps continuous which we all don't need when we ride. Nobody of us draws that continuous, maybe 10% of our ride if we drive hard, you maybe 25 % of the time if you drive really hard.
But anyway i would be interested in your VESC settings for the motor.
```

---
## \#9 Posted by: evoheyax Posted at: 2016-12-03T18:36:00.659Z Reads: 248

```
From my testing, these cells (at least the LG HE2, which the graphs I've seen between these and 25r are very similar) can not do 20 amps continuous without major sagging. When I pull 72 amps (they are rated to 80 amps con), I will sag from 80% down to 20%. If I limit my amps to 40 across the entire board, the sag at 40 amps is less than 5%... So in reality, 40-50 amps continuous is what a 4p of these cells can do. (this is why my understanding is, the space cell 4p version has a 40a fuse)

If high amps aren't what most people need, than the VESC-X is a useless improvement for dual drive boards (and only useful for single drive boards). If you only need 25 amps per esc, than the VESC v4.12 will do that just fine. If you want to do the extra amps the VESC-X can support, you need a battery with really double the continuous rating. Putting the VESC-X in the raptor 2 wouldn't be much different than putting the VESC v4.12 with this battery. You can't utalize the extra amps the VESC-X can do, because the battery can't do the extra amps also.
```

---
## \#10 Posted by: Ackmaniac Posted at: 2016-12-03T19:14:00.967Z Reads: 245

```
So you are measuring that via a battery meter which gives you a reading at no load. But you use it for load situations. That doesn't mean anything. Most of them even have a linear calculation for the battery which is also wrong. When the battery is under load it is normal that the voltage goes down a bit. That is why they are rated to 3.6 V under load even when they are charged up till 4.2V. My 200 max amps continuous Lipo's do that as well. So you would be very surprised that you have the same behavior with Lipo's on your battery meter.

So please don't try to make the battery's bad when they work like they should work.

I can't tell much if the VESC-X is necessary for a dual setup but it can't hurt anyway. All i know is that most hub users say that hubs need more amps. But i have no experience with them yet that so i should be quiet for now.
```

---
## \#11 Posted by: evoheyax Posted at: 2016-12-03T19:31:07.910Z Reads: 245

```
No offense, becuase I'm excited about your work with the vesc firmware and watt control mode. But you clearly haven't followed any of my work, so let me fill you in...

I have built a bluetooth + iphone app system from the bluetooth communication code on up so I can see the data straight from the VESC while riding. I save data into sessions, so I can go back and look at both the graphs and my avg and max values for all important data the vesc keeps track of. I created a video overlay recorder in my app so I can see how my load changes while riding without the need of exporting data and using a second application to overlay it.

I collect data straight from the vesc while riding. I also have a panel of LCDs on my board to see what the voltage of every cell plus the overall voltage of my board is. These, I have found compared to the VESC's data, to be somewhat inaccurate.

I tried watt meters, and compared to the vesc's data, they are highly inaccurate. I trust the data the vesc sees and processes, as we are trusting it when we set all these limits (voltage cutoffs, max temp, max motor amps, max battery amps, ect.).

Here's a diagram of what the 2 power systems could look like with the raptor 2, to highlight how pointless the vesc-x is with the current battery system:

<img src="/uploads/db1493/original/3X/d/c/dc8ab663462f0418f2d0ce84959336cb3cce260b.jpg" width="690" height="414">

As you see, you don't utilize any of the extra amp capabilities of the VESC-X vs a VESC v4.12.

I am in no way saying the VESC-X is not an improvement, just that Jason said the main reason for the VESC-X is so the raptor 2 can do the higher amps the motors need. But the current VESC's can already do the max amps the space cell 4p version can do, so it's pointless besides the new BLDC tool for the raptor 2.

The reason cells sag is because your too close to the max discharge the cells can do. When you pull lower amps, like I said, 40 amps for the 4p config, you sag very little. This (and the fact your cells last longer the further you are from your batteries rated max amps) is why there has been a 40 amp fuse on the space cell 4p version.

If your lipos are sagging heavily, then the numbers the manufacurer gave you are bs. A great example of this is multistar lipos. They give normal lipo ratings (20c), but many in the online RC and even endless sphere have tested them and found they are a fraction of what they advertise (maybe only 4c instead of the 20c they advertise).

So even though these cells are rated to 80a, they will sag a lot and won't last very long.

I will be testing with more lipos in the near future to highlight this, so watch out for some tests in the near future from me about this.
```

---
## \#12 Posted by: Ackmaniac Posted at: 2016-12-03T19:43:56.084Z Reads: 225

```
Also no offence from me. I am also only interested in the facts. i want to avoid that another myth is created because of misunderstandings. because there are already enough of them.
I have also build a Android app to watch the live recordings to understand the VESC much better.

Your mentioned that the battery is going from 80% to 20 % at 80 amps. Please tell us the voltage for that because percentage values don#t make sense. Because i am quite sure that the voltage sag you are talking about is absolutely normal.
```

---
## \#13 Posted by: evoheyax Posted at: 2016-12-03T20:12:47.346Z Reads: 223

```
I will be recording more video soon to highlight this, but my battery sags from 48.6 volts down to 42.2,which is not a good amount of sag. As a result, When I get down to 46 volts with no load, I have to stop riding, as I will sag it down to 38 volts or less at that point on a steep hill. Min I should go is 38.8, max is 50.4 volts. Evolve's new Carbon GT has this issue. The reason, this is their first board with li-ion. They always used lipos before, and never had this issue. Before, when I used to use lipos, I never sagged like this. Chaka has talked a lot about sag in the 18650 thread, and recommended going up to a 12s6p (which is what he uses) to resolve the sagging issues I have. Jason is aware of them too, this is one reason why he doesn't run cells close to their max discharge ratings. Some sag will always exist, but it's ideal to get the sag as low as possible (preferably < %5)
```

---
## \#14 Posted by: Dedbny Posted at: 2016-12-03T20:16:35.870Z Reads: 218

```
Im loving this and its going to go on for 6 months.
```

---
## \#15 Posted by: evoheyax Posted at: 2016-12-03T20:21:38.587Z Reads: 229

```
Also,if you want data about sagging, check out this poll I did: http://www.electric-skateboard.builders/t/lets-talk-about-voltage-sag-poll/12085

Bear in mind, the numbers I give in there are based off of readings from my built in volt meters and was before the app. Now that I have the app, I can see better and determine these things when I'm not going 25 mph and trying not to fall, lol. So I know now my sagging is actually much worse.

This poll confirmed to me that the sagging I'm seeing is not normal.

I don't know why your against percentages... I get that batteries don't discharge linearly, like percentages are calculated, but they are pretty close.

Also, regardless of whether this kind of sag is normal or not, the point is that you can't run these cells that close to their max con rating without a lot of sagging, so again, the VESC-X solves nothing here, since the battery is the limiting factor.
```

---
## \#16 Posted by: Ackmaniac Posted at: 2016-12-03T20:42:03.238Z Reads: 224

```
Why is a sag from 48,6V to 42,2V (3,52 V each cell) not a good amount of sag? It#s just normal and what the battery is made for.
When the battery is at 46V (aorund 30 - 40 % battery left) with no load then a sag to 38V (3,17 V each cell). Which is still or because the battery is rated to 2.5V minimum under load. So you still can go full throttle and have fun.

BTW: insead of not doing full throttle you could also set the VESC settings for battery cutoff start and end right because then the VESC is doing that for you. I let mine start to reduce the power at 3.2V and stop powering at 3.0 V. But that is because i run laptop batteries which are only rated for a max power output of 5 A and continuous at 2.5 A. So i overpower them drastically. And instead of my batteries the samsung 25R are build to do that. 
But even mine still do absolutely fine and don't get hot. Because the battery temperature would predict the limit of the cells and even if i drive hard i use max amps for maybe 10 % of the time. On average i hardly ever use max amps. For example if you go full throttle all the time on the flat you don't even get close to the max amps. Up a hill with your gearing, weight and speed you might do that.

And we don't draw constantly the max amps so we are absolutely fine. I would even say it would be fine to draw max 100 amps from a 4P setup of those cells because they can stand the burst.
```

---
## \#17 Posted by: evoheyax Posted at: 2016-12-03T21:06:50.061Z Reads: 211

```
I'm not saying it's not normal, but it's just not desirable nor good. And there's solutions to solve this issue, which are good lipos or higher p li-ions. @Jinra and @chaka are better people than me to talk about the details of voltage sag.

What lipos are you using btw?

The best lipos I used were the zippy flightmax 8000 mAh cells, and they sagged very little.

[quote="Jinra, post:2, topic:12085"]
To mitigate sag, you have to leave as much buffer room as you can between maximum actual current under load and maximum rated discharge current. Best way to do this is to use prismatic cell lipos. Otherwise building a huge parallel pack would work as well.
[/quote]
```

---
## \#18 Posted by: Ackmaniac Posted at: 2016-12-03T21:23:37.022Z Reads: 203

```
Don't know the brand of my lipos? On my laptop cells I have a huge voltage sag.  From 50 Vdown down to 32 V (not recommended)  under heavy load (80 A) but they still do fine and the board is doing well and powers out 2500 watts which is enough for my weight of 80 kilos with clothes on. And I can bomb up my hills with 42 km/h.  But I don't know about the hills in San Francisco but I can imagine that they are a completely different level. 
But you could drive longer on your cells because you could go lower with the volt level under load. I am simply saying the cells are doing absolutely normal and they are not a bottle neck.
```

---
## \#19 Posted by: evoheyax Posted at: 2016-12-03T21:31:22.684Z Reads: 206

```
Regardless of whether they are doing what they should or not (since we seem to differ largely in opinion here), how can they not be a bottle neck? Your not going to be able to pull higher amps from those cells than the current VESC v4.12 can already do continuously, so the VESC-X does nothing to increase performance here...
```

---
## \#20 Posted by: Ackmaniac Posted at: 2016-12-03T21:34:20.082Z Reads: 203

```
Why shouldn't you pull 80 continously from them when they are build for that. You said you only can do 40A or 50A from that pack and I simply say that this is not the case. Anyway,  we should stop here.
```

---
## \#21 Posted by: laurnts Posted at: 2016-12-03T21:39:04.350Z Reads: 194

```
Sometimes there is a reason why you want to have higher amps. One - two thing I can point out are better heat management, better quality material (last longer), doesn't get damaged easily. Just same reason why boeing 737 is a huge success although they fitted in way bigger engine that they don't need, because only using 20% of the load increases it's life expectancy.
```

---
## \#22 Posted by: evoheyax Posted at: 2016-12-03T21:41:40.322Z Reads: 201

```
Because you get more sag... Ask @onloop why he puts a 40 amp fuse on his space cell, when the batteries cells are rated to 80 amps?

The closer you get to your rated max amp (assuming the rated max amp is valid and confirmed by people like Mooch), the more sag you get... This is a fact, which any person whose researched batteries extensively on this forum can back up. Ask chaka, ask jinra, ask onloop, and many others. They will tell you the same thing.

I'm sorry, and I mean no offense, but I'm done wasting my time arguing about it. You can either accept it as a reality or not.

But most likely, Jason will keep the 40a fuse on the battery pack for the the Raptor 2, which as I have already shown with diagrams even, will make the vesc-x a useless improvement in a dual drive raptor 2 in terms of it's increased continuous amp rating.
```

---
## \#23 Posted by: Hummie Posted at: 2016-12-03T23:52:34.947Z Reads: 183

```
Assuming the 40amp fuse as the amp limit  we can figure what will be the max power of this board while integrating voltage sag.  At full charge ten amp draw from a typical Li-ion with a 20 amp rating will be at 3.8 volts at full let's say X the 40 amps = ...

The most powerful direct drive board can do 1520 watts max before dropping precipitously within seconds from voltage sag. No?
```

---
## \#24 Posted by: Ackmaniac Posted at: 2016-12-04T00:03:05.209Z Reads: 187

```
By the way. I drive my 80 A max board with a 40 A fuse. Not recommended but on more than 1000 km i never had a problem. I guess my car fuse needs way more than 40A to blow. But Enertion might use other fuses.
So @Hummie now i am curious. Just tell me what we will see in the future of you. More P batteries, A123 or Lipo's.
```

---
## \#25 Posted by: 2-alex-2 Posted at: 2016-12-04T00:13:46.000Z Reads: 186

```
From looking at all these claims and reading the true figures it does look that it's not going to be much better than raptor 1 and not worth the extra money. Feel sorry for anyone who has paid more than $1000 as personally don't think it's worth much more.
```

---
## \#26 Posted by: Hummie Posted at: 2016-12-04T00:19:39.621Z Reads: 178

```
i have no plans but am surprised we all let the important fact slip through that the motor and esc typically isn't near their peak abilities with these Li-ion battery packs.  The real power limit is the batteries and power is so important
```

---
## \#27 Posted by: Ackmaniac Posted at: 2016-12-04T00:40:28.194Z Reads: 175

```
Didn't evoheyax switch from the batteries to the fuse as bottle neck? But now really let us stop here. Otherwise we kill this thread with bitching around. @evoheyax impressive board btw. (seriousely)
```

---
## \#28 Posted by: Hummie Posted at: 2016-12-04T00:58:18.816Z Reads: 172

```
I don't think we are bitching but just figuring out what's going on.  Talking about the facts should always be welcome
```

---
## \#29 Posted by: Dedbny Posted at: 2016-12-04T01:32:11.452Z Reads: 162

```
Love the debate, but maybe it should be on its own thread. Modetators please move. Raptor 2 debate/discussion. Maybe the others may want to call it.
```

---
## \#30 Posted by: Dedbny Posted at: 2016-12-04T05:29:34.277Z Reads: 130

```
Ok now that we have a thread that is just for RV2 my interest with the new board is going to be how reliable it will be. The vids that are coming out against the V1 Id like to see powering on numerous laps up and down hills for say 20mins. Rather than just a power lap on veladrome or once up a hill. Ok it will need to be sped up.
```

---
## \#31 Posted by: E-Boarding Posted at: 2016-12-04T07:38:01.522Z Reads: 121

```
I like this debate too
the VESC-X should be an improvement for FOC which is a big deal for some people
```

---
## \#32 Posted by: 2-alex-2 Posted at: 2016-12-04T07:47:30.547Z Reads: 127

```
But a video by Jason for comparison just now could also be rigged to make the raptor 2 loot better. Really he needs to get some beta boards out to 3rd party people to give some honest feedback agains diy board.
```

---
## \#33 Posted by: Dedbny Posted at: 2016-12-04T08:32:06.572Z Reads: 131

```
For sure there should be and we hope will be independant videos. Early days. He hasnt even got beta boards yet. But the comparison videos he was doing with Raptor 1 seemed ok. Albet you can edit what you like and set test parameters as you like. 

Hes had parts tested, just not the whole early model yet.

Be good if he could do one against Evolve GT, the Raptor V1 dual rather than mono and new RV2. Big expectations.

He was meant to do a CGT vs Rpator V1 . That never happened. Might be logistics as owner of GT wasnt in his state.

Also to be fair. Do you see any other eboard conpany puting their product against opposition. Non. Thats because Enertion put themselves out there. They back their product. And they will have to to claim the powerfull direct drive mantle.
```

---
## \#34 Posted by: evoheyax Posted at: 2016-12-05T18:41:00.130Z Reads: 126

```
The real issue with the raptor 2 in my mind, is the battery. I'm sure there will be other hub motor issues too (I'm not going to do Jason's homework for him).

The fact that Jason won't say "this won't be an issue because of x, y and z", is because he knows I'm right.

@Ackmaniac if you look at the discharge graph for the LG HE2 (which is the cell I'm using), you'll notice it's normal at 20 amps (it's max continuous rated amps) that it'll sag to 3.8 immediately. That's a .4 volt sag at full charge. If you discharge only 10 amps, it sag's immediately down to 4. So half the current, and you half the sag. This is why I say, even if they are rated to 20 amps continuous, that amount of sag is not desirable on an electric skateboard. If you have a 10s4p pulling 80 amps, and a 10s8p pulling 160 amps, we can expect the same amount of sag. The higher the max continuous rated cell, the less sag we can expect. 18650s in this 20 con class all sag pretty similarly, but lipos all sag pretty differently. This could explain why your lipo sags more. You said it was also a laptop battery? This could explain the sag also, as those cells are likely cheap and not really 200 amp con cells.

The Raptor 2 with the current 10s4p will either have a lot of sag or will run way below it's max amp rating. My guess is he'll put a 60 amp fuse. This would make the vesc-x a needed upgrade, but will still sag quite a bit.

The fuse bottle neck is easy to get around, but it's there because more than 40 amps will cause a lot of sag. I mention it to illustrate my point.

And @onloop, still waiting to hear your side of this. So far, nothing but silence...
```

---
## \#35 Posted by: NickTheDude Posted at: 2016-12-05T19:11:32.709Z Reads: 120

```
So... I don't know anything about voltage sag, but it'd be interesting to see where amperage is capped on other productions boards.

If hes pulling 30 amps for each motor, then like you said, the VESC-X was a nessecary upgrade. And if his hub motors can handle 30 amps continuous than I'd be pretty impressed, and it would therefor be the most powerful direct drive system.
```

---
## \#36 Posted by: Ackmaniac Posted at: 2016-12-05T19:16:36.434Z Reads: 122

```
Shortly wnat to make clear that i have a single board with 2 lipos 10S 4Ah 25C in parallel. So 10S2P 8Ah 25C = 200 amps. And they don't sag as much. 
And i have the 12S8P battery made from laptop cells which sag much more because they are absolutely not build for that, but still do it. 
But the 25R are build for it and the 0.4 V sag is normal and not an issue.

Otherwise it would mean that they rate it to 20A but tell the costumer that they should not do that.

So what would those 3.8V * 10S = 38V be good for? At 40A on each motor (80A total) it would be 38 * 80 = 3040 watts.
That is a bit more than 4 hp and maybe even too much for the most of us. But that depends on everybody's personal taste and experience.
```

---
## \#37 Posted by: evoheyax Posted at: 2016-12-05T19:53:59.870Z Reads: 119

```
The 0.4 V sag is normal, but that doesn't mean it isn't an overall issue with the board. With sags like that, you have to stop at 3.6 volts per cell without load, as any more, and you'll sag down under load past the 3.2 the community agrees we should stop at for the sake of the cells life span. In this case, the 10s battery is 32 min volts, 42 max volts. That's a 10 volt range, with a sag of 4 volts, so 6 volts of usable energy. That's almost half of the battery range in sag, which means you'll get half of the range you would get with no sag. With a sag of 2 volts instead, you would still have a range of 8 volts, 1/3 larger than with the 4 volt sag. This means running at half the suggested rating would yield 1/3 better range.

Getting 25 miles on a battery this size is a stretch for any hub motor in my mind. If you are loosing 1/3 of the battery to sagging, than this is an issue. I never said the batteries are malfunctioning and not doing what they are designed to do, just that these cells in this configuration will either sag heavily, and under deliver on power. Or a medium of the two with still quite a large sag. There won't be 80 amps of power without a large sag, which no one wants due to the range issues it will exacerbate.
```

---
## \#38 Posted by: evoheyax Posted at: 2016-12-05T20:03:56.731Z Reads: 118

```
[quote="NickTheDude, post:35, topic:14148"]
And if his hub motors can handle 30 amps continuous than I'd be pretty impressed, and it would therefor be the most powerful direct drive system.
[/quote]

I think your getting confused by motor amps vs battery amps. The two go hand in hand, but motor amps are always higher than battery amps. 30 motor amps is not that high. I hit 50 motor amps peak with 30 continuous per hub with hummies small hubs in 4WD. This is usually around 18 battery amps. I'm sure I could pull more, but like the Raptor 2, I'm limited by my batteries max amps. I am sure I can pull much higher amps once I solve my battery issue.
```

---
## \#39 Posted by: Ackmaniac Posted at: 2016-12-05T20:09:27.161Z Reads: 114

```
That is so much mixed up miscommunication here. 
Simple example, at 3.6V with no load a lipo is already empty. 

Started to explain it but then you will come with the next stuff where numbers get mixed and taken out of context.

I know you don't like the raptor 2 and you don't have to, which is absolutely fine. Hopefully we will see in the future if it is a great board or not. Time will tell.

I will concentrate on source code again.
```

---
## \#40 Posted by: evoheyax Posted at: 2016-12-05T20:19:57.692Z Reads: 115

```
I'm trying to get to the bottom of the facts, not create bs to attack a board. I want the board to do what it claims, so the sake of everyone whose blown their money on it. Otherwise, I would keep my mouth shut and wait until it comes out and the problems are there. I've talked to many respected people in this community about this issue in private and they all agree with me and what I'm saying about this batteries problems. You seem to be a programmer, I am also. But I've spent the last 18 months studying electric skateboards, and the electronics in them. My ideas aren't crazy, but we clearly disagree that using this battery, you will either have bad voltage sag or low amp limit, or a mix of the 2.
```

---
## \#41 Posted by: NickTheDude Posted at: 2016-12-05T20:24:30.213Z Reads: 105

```
Yeah I probably am... Could you explain their relationship cause I seem to keep getting hung up on this. 

This is how I understand it right now, let say you had a 10S pack. On the battery side of the VESC voltage is a constant 37V and amps fluctuate depending on how much power is needed. On the motor side, voltage is determined by rpm of the motor (rpm/kV) and amps are equal to the power being drawn from the battery divided by the voltage in the motor. The motors amps would always be higher since the motor can never actually reach top no-load rpm. Is this correct?
```

---
## \#42 Posted by: evoheyax Posted at: 2016-12-05T20:27:53.572Z Reads: 109

```
The process of how the battery amps are converted by the esc to motor amps is debatable, and most of us don't fully understand it. I am one of those who doesn't fully understand this process. But I let the esc do that work for me. The part I can control is the battery amps, so my main focus as a builder is on the battery amps, as the motor can't get more amps without the battery also giving more amps.

I can tell you the battery amp are always lower than motor amps from experience of looking at the graphs of the two together with app.
```

---
## \#43 Posted by: Ackmaniac Posted at: 2016-12-05T20:33:26.882Z Reads: 109

```
By the duty cycle you know at how much volts the motor is currently working and that also predicts the ratio of motor ams to battery amps.

So 10% duty cycle means 10% of the batterys volts are at the motor. (36V battery is 3,6V motor)
So also 40A at the motor result in 4A (10%) at the battery.

So 25% duty cycle means 25% of the batterys volts are at the motor. (36V battery is 9V motor)
So also 40A at the motor result in 10A (25%) at the battery.

So 90% duty cycle means 90% of the batterys volts are at the motor. (36V battery is 32,4V motor)
So also 40A at the motor result in 36A (90%) at the battery.
```

---
## \#44 Posted by: NickTheDude Posted at: 2016-12-05T20:39:39.983Z Reads: 102

```
Ahhhhh, and throttle is directly tied to duty cycle?
```

---
## \#45 Posted by: Ackmaniac Posted at: 2016-12-05T20:50:51.627Z Reads: 112

```
Of course it is not that easy.
There are different control modes. Most are using current control.
That calculates how much volts need to be powered to the motor to reach the exact amount of amps that you control with your throttle.
So when your motor max is set to 80 amps then at 25% throttle you tell the vesc to reach 20 amps. Doesn't mater at which speed. You always want 20 amps when you don't change the throttle.
So the VESC constantly adjusts the voltage to the motor to match 20 amps.

This is the power output then

<img src="/uploads/db1493/original/3X/7/b/7b986b429302b0767b2ec3d406ad82279abbed05.png" width="338" height="499">
```

---
## \#46 Posted by: Ackmaniac Posted at: 2016-12-05T20:55:12.254Z Reads: 113

```
But now we do the same thing for 100% throttle.

<img src="/uploads/db1493/original/3X/b/6/b62247c4ef5ec4572e9717ab4573082300e461bb.png" width="339" height="500">

Here we can see that the battery max amp setting of 40 A reduces the maximum power output already at half the speed. Which is the reason why i invented my firmware mod.

On the other side we also start to draw all the allowed battery amp at half the speed. Before we don't even reach that value. And the closer max motor and max battery amps are together the faster you have to go before you start to draw the maximum.
```

---
## \#47 Posted by: Hummie Posted at: 2016-12-05T21:01:03.483Z Reads: 108

```
Any reason not to try 200 amps motor max with standard 60 battery amps in current control?  Greater acceleration from start? Possibly less cogging at lowest speed?
```

---
## \#48 Posted by: Ackmaniac Posted at: 2016-12-05T21:03:07.263Z Reads: 117

```
Please try and make a video of that. I tried to keep it simply instead of complicating thinks.
```

---
## \#49 Posted by: JohnnyMeduse Posted at: 2016-12-05T21:19:51.953Z Reads: 117

```
I'm just wandering why noboby use the Duty cycle in there equations????
```

---
## \#50 Posted by: Michaelinvegas Posted at: 2016-12-05T21:27:02.526Z Reads: 120

```
This is a good thread @evoheyax I see your points
```

---
## \#51 Posted by: Ackmaniac Posted at: 2016-12-05T21:34:56.880Z Reads: 120

```
Because it is hard to explain.
Lets say the motor runs at half the speed on the bench and there is no wind, rolling or bearing resistance. The it would be 18V on the motor because it is at 50 % duty cycle. when you want to go faster then you have to give it more volts. Lets say 27V (75% duty cycle). Then it accelerates hard until it reaches 75% of the speed. If you would reduce the voltage then it brakes and charges the battery by that because it has too much volts and wants to go back unil it reaches the speed at 20V.
When add some resistance now like wind and rolling resistance then it can't stay at it's speed. So it slows down a bit but you still power it with 20V. So it will go down a bit until the voltage difference is enough to produce enough power to keep the speed with resistance. So it stays at 50% duty cycle but can't keep half the speed (maybe only 40% of the speed).
 
The maximum speed is then predicted by the maximum duty cycle which is 95% for the VESC. So we only can reach a speed that produces enough power at close to 95% of the battery's volts.

I hope that this simplified it enough. Maybe i am even wrong because you can complicate that drastically and that is the way i explain it to me. All of that can be calculated with the resistance of the motor and so on but don't even ask me. I am not a electric engineer, so i will be the wrong person to explain that.
```

---
## \#52 Posted by: JohnnyMeduse Posted at: 2016-12-05T22:17:18.733Z Reads: 116

```
I know about duty cycle...😉 I just that people need to realize that the battery only need to provide a true rms current of what the motor need base mostly on the duty cycle... for a exemple if look at the last video from vedder, he run is motor at 70 amp (yes the ermp is low), but only need the supply to provide 7A since the duty cycle is at 10%, so before arguing that the battery need to be bigger, you need to take a closer look upon the esc and the motor you are using.
```

---
## \#53 Posted by: Hummie Posted at: 2016-12-06T00:05:03.946Z Reads: 120

```
As you say at lower speeds the amps to the motor will be much higher than from the battery (for fractions of a second) but it's not worth confusing the issue.  a wattmeter or amp meter is telling the actual amperage running from the battery and when you quickly get to the peak of the duty cycle the amps to the motor are the same as from the battery and pulling 40 amps or 45 or more straight from the battery is common in my experience as well as others. The 2 motors and esc may even be able to do that continuously with no decrease in performance but the battery voltage will drop like a rock and with it speed, power, amp hours, and the packs life on a 10s4p Li-ion pack with 20p rated cells.  It's typical and normal and not the end of the world but it is the limitation of the power that can be put out and a big limit. By my simple math assuming even a 40amp max (the limit of the fuse and suggested for batteries) the peak power the board will have, which will last seconds before sinking with voltage sag= 1520 watts.
```

---
## \#54 Posted by: Ackmaniac Posted at: 2016-12-06T00:19:48.752Z Reads: 120

```
OK i have enough. Have fun guys.
```

---
## \#55 Posted by: Hummie Posted at: 2016-12-06T04:38:11.008Z Reads: 112

```
My mistake, somehow I wa under the impression that the board came with a 40 amp fuse.  That would of course limit power a lot. I haven't heard there isn't a fuse but judging from the most recent post by onloop it seems the board will be able to put out 80 amps. 
He doesn't factor in sag with his Mac power number, which goes back to the earlier Li-ion issue but whatever a world of difference from a 40p fuse
```

---
