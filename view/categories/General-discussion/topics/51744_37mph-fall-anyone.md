# 37mph fall anyone?

### Replies: 160 Views: 4045

## \#1 Posted by: Exiledd_Top Posted at: 2018-04-09T22:23:26.243Z Reads: 553

```
I have one question and one question alone, was going up my daily route going around 37mph up a hill today and felt my board just die on me as if vesc restarted or something long the lines it didn't go into break but all that momentum threw me off because it let go of the throttle fell and rolled like ball pretty bad. Left ankle now mest up right shoulder as well and wrist along with both my hands.
Anyways any thoughts on why this happened thinking its my battery no way in hell I lost 4 vesc at the same time, settings per vesc was 32min 65 amps on motors 12s6p30q BMS bypassed.  Over heated ? Vesc with 4x of them ? Focbox ?
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-04-09T22:25:35.790Z Reads: 540

```
sounds terrible but one of the most graceful things ive ever seen was a gif of a longboarder (fully suited up, unharmed), sliding like superman down a road after he fell off his board
```

---
## \#3 Posted by: Exiledd_Top Posted at: 2018-04-09T22:26:16.617Z Reads: 533

```
I just had a helmet sadly no other gear, this was going up hill
```

---
## \#4 Posted by: GrecoMan Posted at: 2018-04-09T22:26:55.767Z Reads: 526

```
yea that sucks. you good tho?

and I dont just mean physically, the mental game of getting back onto a board after a bad fall is almost worse than the physical effects
```

---
## \#5 Posted by: Exiledd_Top Posted at: 2018-04-09T22:29:27.126Z Reads: 518

```
Am pretty sure am out for a good week or so from riding anything while I heal up and just gana ride my exo for a bit till I  go back on my 4wd . I would post photos but its disgusting
```

---
## \#6 Posted by: Mattmccrary8 Posted at: 2018-04-09T22:29:46.779Z Reads: 500

```
Could it be your battery. Same thing happened to me with a 12s4p. No Bluetooth module data?
```

---
## \#7 Posted by: Exiledd_Top Posted at: 2018-04-09T22:31:07.427Z Reads: 492

```
Am pretty sure it's my battery I went 4wd for a reason so that if one vesc ever messes up or 2 I still have 2 other ones but for all 4 to shut down It looks like its battery
```

---
## \#8 Posted by: Exiledd_Top Posted at: 2018-04-09T22:31:45.481Z Reads: 474

```
I think one if the welds got loose or something inside the battery after I got into a previous accident not so long ago making my board fly 5 feet in the air
```

---
## \#9 Posted by: Mattmccrary8 Posted at: 2018-04-09T22:32:27.880Z Reads: 461

```
I would imagine the battery because maybe you went undervoltage that hit a sudden cut off. The bms discharge could be holding you back as well
```

---
## \#10 Posted by: Exiledd_Top Posted at: 2018-04-09T22:33:01.836Z Reads: 446

```
Battery was at 95% and I have always bombed that hill going  up it around 30-35mph
```

---
## \#11 Posted by: Deckoz Posted at: 2018-04-09T22:33:08.203Z Reads: 430

```
I know mine was from my dumbass setting up -50 battery amps -100 total of braking(not motor amps) when I first built my evo. Lol.. fell like a rock and slid at 35 after tapping the brakes haha..

But I wear all the gear. I couldn't pick up my right arm for two days. Daily stretching. Lifting regularly (slowly working up since has helped. But other then that I was fine...

But this is why i preach wearing all the gear...if your going above 20
```

---
## \#12 Posted by: SuperBen Posted at: 2018-04-09T22:33:58.718Z Reads: 411

```
Dude that is rough glad you survived, 37 is fast AF
```

---
## \#13 Posted by: Exiledd_Top Posted at: 2018-04-09T22:34:49.271Z Reads: 408

```
No my regen for each vesc was -6 I was going up the hill luckly there was a truck that had a distance when I fell or I would have bin bug splat
```

---
## \#15 Posted by: Exiledd_Top Posted at: 2018-04-09T22:37:45.021Z Reads: 413

```
![20180321_211714|374x500](upload://Ek7g1I81qlkuz0YYwFLiji9Mgu.jpg)

![20180321_211717|374x500](upload://6BAbiRWx90viQmC9V6EyLek8BYV.jpg)
Settings were per vesc four of them
BTW my cut offs were wrong at the time I have fixed them and put them at 38 and 37
```

---
## \#16 Posted by: Exiledd_Top Posted at: 2018-04-09T22:38:59.479Z Reads: 378

```
Yes that's the first thing am doing when I feel good again to ride, it will take some time to get confident again to ride my 4wd evo again but first I got to find out what's wrong with it
```

---
## \#18 Posted by: Blasto Posted at: 2018-04-09T22:44:24.825Z Reads: 387

```
I would lower your batt cutoff end to 28-29V or so. The idea is you want to ease in to the end cutoff. As it is set right now, both start and end are way too close and could just hit the cutoff end without any backing off from the cutoff start.

Ignore my voltages, i was assuming you had a 10S system.

But the idea stays the same, you want a safe voltage distance from start to end. To avoid hitting “end” off the bat
```

---
## \#19 Posted by: Exiledd_Top Posted at: 2018-04-09T22:46:18.429Z Reads: 373

```
Oh my calculations was that i did 12x3.2  38.4 so I set it at 39 and 38 could it have bin since I was pulling so much that it dipped bellow that battery was at 95%
```

---
## \#20 Posted by: Ackmaniac Posted at: 2018-04-09T23:01:36.342Z Reads: 371

```
Possible reasons are: 
- Master VESC had en error and other VESCs are connected by CAN. When master drops out other VESCs also do nothing after timeout.
That would feel like one motor dropped out and after 1 second (default value) the other 3 motor dropped out. In this case you would get unexpected torque steering which already throws you off the board at that speed. 
- Remote lost connection <-- **Most likely**. Did you experience short delays of your throttle or that throttle stays while you released it already? 
Because when all motors dropped out **exactly** at the same time it can only be the throttle. Otherwise the other motors would have dropped out after the timeout.
- loose CAN wire
- loose Battery wire

Other stuff is also possible. So the best is you give us all the details how it felt when the power dropped out.
```

---
## \#21 Posted by: deucesdown Posted at: 2018-04-09T23:11:27.199Z Reads: 336

```
Did you have ackmaniac app? Did it log any errors?

Good job survivng. This is like the Evo of Death.
```

---
## \#22 Posted by: Mikenopolis Posted at: 2018-04-09T23:13:37.694Z Reads: 330

```
You have 4 vescs and two receivers right? so chances of it being the vesc and receivers being the issue is low. Is your controller working fine?

My board died on me completely this weekend at mile 11. Luckily it was on flat ground and we were a block away from our stop so I kicked it back and swapped my pack. During the whole ride I had momentary jots where my board seems to disconnect with the controller then reconnects a second later. 

When I got home, I plugged in the battery for about 30 minutes and attempted to turn it on, I got nothing. So I cut open the pack and saw one of the wires had broken off, I stripped it and soldered it back on and now good as new. I got lucky the wire was probably touching (barely) when I went down some hills
```

---
## \#23 Posted by: evoheyax Posted at: 2018-04-09T23:16:45.218Z Reads: 313

```
Another possibility that I have encountered is the connection between one of your p’s in the battery pack could fail. This lead to me losing power to all four motors and throughing me off lol.

I had another case where a cap, a vedder switch and Bluetooth switch blew at exactly the same time. Still have no idea what cause what to break.

A lot can go wrong really. Best to ride slow and try to recreate the incident. Replace some parts and try again. If it comes back, you know that part is not the problem then.
```

---
## \#24 Posted by: pat.speed Posted at: 2018-04-09T23:17:06.933Z Reads: 304

```
This is probably a good thread to ask in but is there a way to setup the vescs so that if the ppm signal drops out the Vesc will slowly ramp down its speed instead of fully stopping. This would be really great if it’s possible to do as I’ve heard of multiple people falling at high speed because of this
```

---
## \#25 Posted by: Exiledd_Top Posted at: 2018-04-09T23:29:40.182Z Reads: 292

```
Am not using any ppm wire splitter anymore I am using 4 receivers , BRAND new gt2b and put my old gt2b mastercho mod , I felt as it was going really fast and then just felt no response as if I lost connection or vesc restarted or something along the lines . it didn't go into break but having all that force and then just kinda no more force all of the sudden throwing me off
```

---
## \#26 Posted by: barajabali Posted at: 2018-04-09T23:30:22.672Z Reads: 283

```
Hope you’re okay man.
```

---
## \#27 Posted by: Exiledd_Top Posted at: 2018-04-09T23:31:14.996Z Reads: 284

```
What I did realize the night before when I was testing same settings my brakes would not break to 100% even tho my remote was fully calabrated into the vesc tool didn't change nothing but u thought nothing of it, but now I think it's battery or something nor sure haven't opened it up.
```

---
## \#28 Posted by: Cobber Posted at: 2018-04-09T23:31:29.015Z Reads: 281

```
[quote="Ackmaniac, post:20, topic:51744"]
Remote lost connection <-- **Most likely**
[/quote]

I'm with Ack, lost remote connection, but i'd say a brown-out
a drop in voltage to your Rx circuit caused you to lose connection...
```

---
## \#29 Posted by: Ackmaniac Posted at: 2018-04-09T23:31:42.970Z Reads: 284

```
This will sound like i created this thread to advertise my firmware mod but i added exactly that to firmware 3.100.

When it looses connection it will ramp down the power by 50A a second till 0 and then ramp up the brakes 20A per second if braking amps are defined in case of a timeout.
Once the signal comes back alive it slowly ramps the power up again.
This is necessary because mostly when the connection is lost it only happens for like half a second. That means in case of full throttle = full-power, no-power, full-power
With my firmware you will realise the board looses power and gains power but no instant cutoff.

But i don't want to highjack this thread (did already) so you can read more about that here.
http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116?u=ackmaniac
```

---
## \#30 Posted by: Exiledd_Top Posted at: 2018-04-09T23:33:44.347Z Reads: 265

```
Remotes brand new was fully charged as well dam
```

---
## \#31 Posted by: Ackmaniac Posted at: 2018-04-09T23:34:45.726Z Reads: 259

```
Actually the idea that one battery in  one of the P packs lost connection isn't a bad idea. That would result in a instant voltage drop which could cause the cutoff to trigger. But just check the battery if any spot welt connection is loose. If not then that's not the root cause.
```

---
## \#32 Posted by: Cobber Posted at: 2018-04-09T23:35:44.762Z Reads: 257

```
yeah but the receivers are powered from your main battery, by your vesc... this is a common enough phenomen to be given a name by the rc guys, especially the 3d heli guys get it from time to time.
```

---
## \#33 Posted by: Ackmaniac Posted at: 2018-04-09T23:35:54.625Z Reads: 255

```
[quote="Exiledd_Top, post:30, topic:51744, full:true"]
Remotes brand new was fully charged as well dam
[/quote]

Which doesn't mean they can't fail. Which remote did you use.
```

---
## \#34 Posted by: b264 Posted at: 2018-04-09T23:36:33.143Z Reads: 253

```
[quote="Ackmaniac, post:29, topic:51744"]
This will sound like i created this thread to advertise my firmware mod but i added exactly that to firmware 3.100.

When it looses connection it will ramp down the power by 50A a second till 0 and then ramp up the brakes 20A per second if braking amps are defined in case of a timeout.

Once the signal comes back alive it slowly ramps the power up again.

This is necessary because mostly when the connection is lost it only happens for like half a second. That means in case of full throttle = full-power, no-power, full-power

With my firmware you will realise the board looses power and gains power but no instant cutoff.

But i donÄt want to highjack this thread (did already) so you can read more about that here.
[/quote]

This isn't hijacking the thread, it's directly related to trying to fix the problem here :slight_smile:
```

---
## \#35 Posted by: Exiledd_Top Posted at: 2018-04-09T23:38:31.620Z Reads: 245

```
Gt2b with mastercho mod
```

---
## \#36 Posted by: Ackmaniac Posted at: 2018-04-09T23:40:31.461Z Reads: 242

```
Did you cut or shorten the antenna on the remote? Or did the antenna get bended? Because i had 3 GT2B in my hands and 2 of them lost connection because of a modified antenna on the remote or a broken antenna at the receiver (bended too many times).
```

---
## \#37 Posted by: Exiledd_Top Posted at: 2018-04-09T23:50:32.134Z Reads: 242

```
Nope have never bended the antenna
```

---
## \#38 Posted by: Mikenopolis Posted at: 2018-04-09T23:55:51.053Z Reads: 245

```
[quote="Exiledd_Top, post:37, topic:51744"]
bended
[/quote]

bent..Sorry, I had to
```

---
## \#39 Posted by: pennyboard Posted at: 2018-04-10T00:40:31.091Z Reads: 242

```
Pulling enough current through 4 VESCs to go 37 mph uphill would put a strain on wiring/connectors, and/or vedder switch. What AWG is your wiring from your battery to your vescs? Have you checked to make sure you didn’t burn any of your wiring or anything like that?
```

---
## \#40 Posted by: Exiledd_Top Posted at: 2018-04-10T00:44:20.087Z Reads: 239

```
12awg on battery and everything else is 10awg
```

---
## \#41 Posted by: pennyboard Posted at: 2018-04-10T01:06:08.091Z Reads: 225

```
12awg is only rated for 41 Amps. Is it possible that the hill climb was so long that you pulled more current than that for a sustained period of time and melted either the wiring or a connector?
```

---
## \#42 Posted by: Exiledd_Top Posted at: 2018-04-10T01:17:03.036Z Reads: 211

```
I didn't build the battery its a Baja battery so not sure maybe its 12awg or 10awg  @barajabali? I'll look into it tommorow right now am just in bed like a baby in pain
```

---
## \#43 Posted by: barajabali Posted at: 2018-04-10T01:27:34.699Z Reads: 215

```
Lol no it’s 10 awg and supper worm Finley stranded wire can handle so much more then 41 amps
```

---
## \#44 Posted by: b264 Posted at: 2018-04-10T01:29:42.346Z Reads: 210

```
Sure, but not continuously for an extended period
```

---
## \#45 Posted by: barajabali Posted at: 2018-04-10T01:30:47.340Z Reads: 213

```
So I suppose you use 8 gauge wire then?
```

---
## \#46 Posted by: Exiledd_Top Posted at: 2018-04-10T01:36:21.718Z Reads: 215

```
[quote="b264, post:44, topic:51744"]
continuously for an extended period
[/quote]

I mean it was like  than 30 seconds everyday going up that hill to school
```

---
## \#47 Posted by: b264 Posted at: 2018-04-10T01:38:52.591Z Reads: 207

```
Does your wire have silicone insulation?
```

---
## \#48 Posted by: barajabali Posted at: 2018-04-10T01:38:56.344Z Reads: 213

```
@Exiledd_Top. If it is your battery, (100% confident that it isn’t), I offer a 1 year warranty on all my packs. 

I’ll take it back and fix it. I extremely doubt  that your wire or connectors are the issue. I bypassed the bms to your request so the bms can’t be the issue
```

---
## \#49 Posted by: barajabali Posted at: 2018-04-10T01:39:23.445Z Reads: 215

```
It’s silicone wire, super worm. Highest quality you can find this side of the Mississippi
```

---
## \#50 Posted by: Exiledd_Top Posted at: 2018-04-10T01:45:16.915Z Reads: 217

```
My concern is not your battery making skills my concern is that the battery might be damaged from my previous incident when I was using ackm tool and it went full reverse on me when I was going fast and then launched forward hitting a curb and watching it fly 5 feet into the air then making a strip loose or breaking something I will probably send it back for inspection
```

---
## \#51 Posted by: barajabali Posted at: 2018-04-10T01:53:38.126Z Reads: 211

```
Still covered under warranty, Send it in. I'll happily fix it if anything is damaged.
```

---
## \#52 Posted by: CamBo Posted at: 2018-04-10T02:06:22.836Z Reads: 219

```
@Ackmaniac and @barajabali 
Amazing examples of awesome customer service done right.
```

---
## \#53 Posted by: lrdesigns Posted at: 2018-04-10T02:41:29.716Z Reads: 219

```
[quote="Exiledd_Top, post:25, topic:51744"]
I am using 4 receivers
[/quote]

So all the esc's are totally independent? 

Do you use a loop key or antispark switch?

I think @Blasto could have a point of the soft and hard cutoff being too close and you might of sagged below 2.75v Though with your huge battery it is surprising.

Shame you didn't get an error log.
```

---
## \#54 Posted by: Exiledd_Top Posted at: 2018-04-10T02:46:22.928Z Reads: 213

```
It comes with a venders antispark switch like the one that is good for 12s I can still turn the board on , yes each vesc is independently that was my failsafe if one vesc dies or 2 I got 2 other vesc it but all died or restarted or idk yet haven't opened it up I am resting in bed like a baby
```

---
## \#55 Posted by: Bobby Posted at: 2018-04-10T02:59:08.645Z Reads: 214

```
Glad you’re ok! I fell going like 5mph up hill a week ago and my ribs still feel cracked. Couldn’t imagine bailing in the 30’s
```

---
## \#56 Posted by: Exiledd_Top Posted at: 2018-04-10T03:13:13.022Z Reads: 216

```
![20180409_091831|683x500](upload://wF2YaSXnIADua4oLIKUrJVEG1fc.jpg)
Just one of my road rashes  of today
```

---
## \#57 Posted by: E1Allen Posted at: 2018-04-10T03:30:20.824Z Reads: 216

```
I'm leaning towards remote cutout.  

1. Can happen anytime, for no real reason.
2. He lost all power
3. LVC set in the VESC at least on my board doesn't cut power.  I hit LVC under load and the VESC maintains that voltage.  It just sits on LVC till you reduce amp draw and it goes above it.  I use focbox but it should be the same for everyone.  I've even seen transient voltage drops below cutoff but no loss of power.

If it wasn't a remote cutout I would suspect a failure in the battery before the split to each vesc.


Glad you're okay.

Chicks dig scars.
```

---
## \#58 Posted by: Deckoz Posted at: 2018-04-10T03:38:05.684Z Reads: 213

```
![15233314312231553780321|375x500](upload://wKySBTssS9hFlJs4LsVjPHs5SCF.jpg)
I'm just sayin...... scars are better on pads...
```

---
## \#59 Posted by: Cobber Posted at: 2018-04-10T03:38:38.120Z Reads: 213

```
Data log files from the rc guys point towards voltage ripple being one of the causes of a brown out. The ripple is thought to cause a momentary voltage drop in the Rx circuit and the Rx-Tx lose connection...
```

---
## \#60 Posted by: Exiledd_Top Posted at: 2018-04-10T03:39:09.702Z Reads: 215

```
Shoot me a list of your parts I'd buy
```

---
## \#61 Posted by: Deckoz Posted at: 2018-04-10T03:44:52.269Z Reads: 214

```
TSG DHP knees
Triple 8 ep55 hard shell(don't need if leatt5.5)
Hillbilly hip pads
Leatt 5.5 Body Protector(the best) or EVS/alpine stars street vests
Mid top skate shooes to cover your ankles
 
A Kevlar hoodie, Kevlar underpants. Your basically covered except shins...

I get not going full leathers, and ya know.. a helmet, good pads may cost you as much as leathers, but I don't wanna wear a leather suite to the bar lol...
```

---
## \#62 Posted by: lrdesigns Posted at: 2018-04-10T04:25:55.757Z Reads: 209

```
[quote="Deckoz, post:61, topic:51744"]
Kevlar underpants
[/quote]

:face_with_raised_eyebrow: I prefer to free ball.
```

---
## \#64 Posted by: Eboosted Posted at: 2018-04-10T04:57:34.268Z Reads: 207

```
I've had those cutouts going up a hill, scary shit! 

You should give @ackmaniac lost-signal-mod a try, you need to flow the setting letting the vesc know when it looses signal by unplugging the binding jumper, the board will keep on going to the last ppm position known for 1 second, so you don't have that behavior when loosing signal.
```

---
## \#65 Posted by: E1Allen Posted at: 2018-04-10T04:58:10.948Z Reads: 204

```
So I wanted to rule out a fault in the RX because he has four.  Also his wires going from front to back are probably different lengths. I've ran a four foot wire with a wattmeter from batt to ESC pulling 110a, his are less than half. (Varies by board,esc, wires...).  Caps are for combating ripple current.  He has four vesc, all with caps to share the load.  I'm just not sure that adds up to an instantaneous Brown out across all four rx
```

---
## \#66 Posted by: Cobber Posted at: 2018-04-10T05:11:36.396Z Reads: 198

```
I don't think it matters if he has 1, 2, 3 or 4 ESC/Rx, the same condition that could cause a issue with one could just as easy cause a issue with all...
```

---
## \#67 Posted by: Exiledd_Top Posted at: 2018-04-10T05:13:25.473Z Reads: 195

```
Um no if one receivers dies which I have had one die on me while cruising others work perfectly fine, I'll open to dam board tommorow
```

---
## \#68 Posted by: E1Allen Posted at: 2018-04-10T05:15:21.131Z Reads: 192

```
Different type of RX failure
```

---
## \#69 Posted by: Cobber Posted at: 2018-04-10T05:15:38.775Z Reads: 187

```
as I said:

[quote="Cobber, post:66, topic:51744"]
...the same condition that **could** cause a issue with one **could** just as easy cause a issue with all…
[/quote]
```

---
## \#70 Posted by: lazerusrm Posted at: 2018-04-10T05:23:05.122Z Reads: 180

```
Thanks for this. If my board did this if i was near full throttle, or accelerating, i would definitely DIE--6kw dual drive.

I would like to see your work make it into the official firmware, not sure how all the logistics of that kind of thing works though.. Seems like it can get... messy.

Also, E1Allen --- Wear more gear. It's WORTH IT.
```

---
## \#71 Posted by: pixelsilva Posted at: 2018-04-10T06:08:18.834Z Reads: 177

```
(You guys and your miles) The rest of the planet think in kilometers..... Jesus, Mary and Joseph..... 59.5 Kph !!

Mannnnn you are lucky you came out of this one, Miguel.  :astonished: Catapulting at 60 kilometers and up hill ??? Best wishes and full recovery. :+1:
```

---
## \#72 Posted by: b264 Posted at: 2018-04-10T06:10:59.479Z Reads: 181

```
Freedom Units, my friend.  Freedom Units.

Why *don't* you think one big thing should be 5280 medium things (sometimes 6046 or 6080 though) and 1 medium thing should be 12 small things?

`/s`
```

---
## \#73 Posted by: Battosaii Posted at: 2018-04-10T06:16:02.305Z Reads: 182

```
England uses MPH too so it's not just the US
```

---
## \#74 Posted by: pixelsilva Posted at: 2018-04-10T06:17:59.308Z Reads: 191

```
My mind-set is for kilometers...je...je.. Seen the number in miles doesn't give me a real sense of the speed. When I see it in kilometers the perspective changes. 60 kilometers!! I'm speechless. The speed you reach on these things is incredible. :rocket:
```

---
## \#75 Posted by: Battosaii Posted at: 2018-04-10T06:29:08.049Z Reads: 194

```
I've been 72kph on my board but not uphill haha that's crazy
```

---
## \#76 Posted by: pixelsilva Posted at: 2018-04-10T06:38:37.298Z Reads: 193

```
https://i.kinja-img.com/gawker-media/image/upload/voc4eo8ajjbozdfkadnz.gif
```

---
## \#77 Posted by: Battosaii Posted at: 2018-04-10T06:45:08.587Z Reads: 191

```
Either that's a camera trick or he's going 100+kph that looks like my car on the highway lol
```

---
## \#78 Posted by: Ackmaniac Posted at: 2018-04-10T06:46:00.923Z Reads: 191

```
[quote="Exiledd_Top, post:50, topic:51744"]
I was using ackm tool and it went full reverse on me when I was going fast and then launched forward hitting a curb and watching it fly 5 feet into the air
[/quote]
???

You should tell more details about your crash and setup.
Now I read you have 4 receivers. That could be a issue and also the root cause. Sadly we don't know how their protocol work. But if they work with acknowledges then the receiver will get 4 instead of one which can confuse it or lead to software exceptions. And do you have a carbon Fibre enclosure?
```

---
## \#79 Posted by: Exiledd_Top Posted at: 2018-04-10T06:47:30.314Z Reads: 182

```
Pychotiller enclosure (abs I believe) , I was using 2 receivers when I was on your firmware .
```

---
## \#80 Posted by: Ackmaniac Posted at: 2018-04-10T06:48:26.832Z Reads: 185

```
And what happened with my firmware exactly? And are the vesc also connected by CAN?

But when I think about it sounds to me that your remote is the root cause. Maybe loose wire or bent antenna.
```

---
## \#81 Posted by: Exiledd_Top Posted at: 2018-04-10T06:51:54.331Z Reads: 187

```
Was going 30ish on my way to jerry house and I was to close to the sidewalk like the edge I was not on the road so I tried to move a bit so I can you know make it without hitting the curb and then my board when into full reverse causing me to drift land on my ankle saw the board hit the curb and then Launch right after hitting the other side of the curb and fly 5 feet into the air (no idea what that was all about, not blaming anyone giving u the benifit of the doubt and so I ordered a new remote and just had stock firmware )
```

---
## \#82 Posted by: pixelsilva Posted at: 2018-04-10T07:15:10.312Z Reads: 185

```
No camera trick my boy. Actually he (Zak Maytum) was soaring close to 112 Kph (70 Mph) in this famous longboard ride which took place in a downhill attempt in Colorado. Here's the vid....

[https://youtu.be/NgMSnFxvzTc](https://youtu.be/NgMSnFxvzTc)

...take a closer look at 1:39 min, to the right, the road sign reads 30 Mph !
```

---
## \#83 Posted by: Ackmaniac Posted at: 2018-04-10T07:31:56.420Z Reads: 183

```
Did you run firmware 2.54 or 3.100?
```

---
## \#84 Posted by: Exiledd_Top Posted at: 2018-04-10T07:47:04.699Z Reads: 185

```
U didn't have 3.10 at the time I was running 2.54 on focbox
```

---
## \#85 Posted by: TarzanHBK Posted at: 2018-04-10T07:51:12.564Z Reads: 182

```
* signal cutout from remote
* damaged battery from your accident
* loose connection somewhere between battery and vescs - check all xt60/90 connectors

That´s all i can think of - should be one of the above.
```

---
## \#86 Posted by: Ackmaniac Posted at: 2018-04-10T08:21:43.744Z Reads: 183

```
When you had the old firmware did you go that fast the first time? Because i am thinking about the ERPM limit and this checkbox
![image|601x173](upload://6YXvz1RsNqfIjeiWJpH5osDSM3Y.png)
```

---
## \#87 Posted by: Exiledd_Top Posted at: 2018-04-10T08:26:55.848Z Reads: 180

```
I don't even remember if I did am not sure its was checked or not I I posted a pic of my bldc tool and just transfered it , yes just checked it was checked but I was foc so does it matter ?
```

---
## \#88 Posted by: Ackmaniac Posted at: 2018-04-10T08:34:04.946Z Reads: 183

```
Did you do that speed before with firmware 2.54 or was it the first time? And what was the ERPM limit set to and which kv do your motors have?
```

---
## \#89 Posted by: Exiledd_Top Posted at: 2018-04-10T09:05:35.032Z Reads: 186

```
110v carvon speed drive R , first time, dont remeber touching any of that I was just worried about battery min motor max and battery regen
```

---
## \#90 Posted by: Sebike Posted at: 2018-04-10T09:19:58.654Z Reads: 189

```
Is that setting still to be found in the new ack esc-tool?
```

---
## \#91 Posted by: Ackmaniac Posted at: 2018-04-10T10:07:16.905Z Reads: 187

```
In the new version it is removed by vedder which was a smart move.
```

---
## \#93 Posted by: Acidfie Posted at: 2018-04-10T17:52:31.487Z Reads: 175

```
what exactly does the limiting the erpm with negative torque? i know it needs to be unchecked for braking purposes but why?
```

---
## \#94 Posted by: E1Allen Posted at: 2018-04-10T17:54:48.815Z Reads: 178

```
It applies brakes for you. Not so good.

As in you're traveling forward at high speed, you hit erpm limit and it automatically applies brakes so you don't go over the erpm limit.  Unfortunately people are usually leaning forward accelerating when that happens.
```

---
## \#95 Posted by: rok Posted at: 2018-04-10T17:59:32.063Z Reads: 174

```
[quote="Ackmaniac, post:78, topic:51744"]
carbon Fibre enclosure?
[/quote]

Just a question here;
Why would it matter if he had a carbon fibre enclosure? Does it interfere with a remotes signal or...?
```

---
## \#97 Posted by: Battosaii Posted at: 2018-04-10T18:36:25.937Z Reads: 167

```
@Deckoz that guy is insane I get nervous just watching. I know that I'm no we're near skilled enough to hit those speeds even for a second.
```

---
## \#99 Posted by: E1Allen Posted at: 2018-04-10T19:36:16.654Z Reads: 165

```
Typically people who devote their lives to one specific thing will do that.
```

---
## \#100 Posted by: rok Posted at: 2018-04-10T19:37:10.500Z Reads: 170

```
@whitepony made two enclosures with carbon fiber and i never heard that he experienced problems with the signal. If thats true, my plan to make them is fucked lol
```

---
## \#101 Posted by: Mikenopolis Posted at: 2018-04-10T19:38:25.209Z Reads: 178

```
I just took a look at my ride data from my weekend ride where the battery had a wire problem and completely shut off. The voltage was jumping all over the place. If you don't have a BT module, you should. Only problem is, I'm not sure you can run and record all four vescs

 ![image|500x500](upload://eix7qlyt2NRdjEh5zK5dLAoIKaM.jpeg)

![temp|346x500](upload://1SNuKVN1AuY0zZeQzD2tfvYlmMV.png)
```

---
## \#102 Posted by: BoostedBuilder Posted at: 2018-04-10T19:42:23.457Z Reads: 171

```
CF enclosures are not so much a problem because the signal would pass through the wooden deck. However an all in one CF deck with enclosure could cause potential drop outs (if it's thick Carbon Fibre).
```

---
## \#103 Posted by: Acidfie Posted at: 2018-04-10T19:52:10.311Z Reads: 176

```
as long it is no full enclosure, you will have no problems.
```

---
## \#105 Posted by: whitepony Posted at: 2018-04-10T20:34:59.410Z Reads: 178

```
i used carbon reinforced decks with carbon enclosure - the only way to get the signal through was a slot i routed into the board - sank the receiver cable into the board basically. other way is a dangling receiver cable outside the box!
```

---
## \#106 Posted by: rok Posted at: 2018-04-10T20:45:49.745Z Reads: 174

```
I read a bit about it on some RC forums. It's true, if its not an all around CF enclosure there is no problem. Especially with such a small distance. (Reciever to remote)
Nice walk around @whitepony.
```

---
## \#107 Posted by: amazingdave Posted at: 2018-04-11T06:16:31.425Z Reads: 172

```
How would the remote dropping out show up in telemetry? I had the same fault, albeit on a single setup the other day... only 20kmh so no damage apart from pride! Metr telemetry shows no fault just a drop in drive to zero...

Sorry to hijack...
```

---
## \#108 Posted by: E1Allen Posted at: 2018-04-11T06:48:17.187Z Reads: 205

```
If your ESC are setup to go to zero throttle then it would look like you just let go of the throttle while riding
```

---
## \#109 Posted by: Exiledd_Top Posted at: 2018-04-12T04:00:18.213Z Reads: 203

```
Hey guys quick update so I finally had time to open my board up and I strictly remember seeing it at 95℅ the day I rode it and now its at 12%, any leads on that ? My voltage is at 39v that is why all my vesc cut out at all at the same time 39v  was my cut off with 38 but question being is why did my battery go from 95% to 12% in the span of 2 miles ?
```

---
## \#110 Posted by: Exiledd_Top Posted at: 2018-04-12T04:10:12.192Z Reads: 204

```
After further Inspection I suspect,  that this is the culptrid and managed to find small cables loose as well , not sure I'f you guys could see it but the metal is actually exposed 
![20180411_210714|374x500](upload://eyEiQhdX1uTLXtF7sXYUyaLogEp.jpg)
![20180411_210410|375x500](upload://5MVHoDv8fiOnIjNRXa4lZU02TTx.jpg)
@barajabali
I think the board is shorting and draining itself what happens if I ship it to u and it drains itself to low ?
No cables were besides it and were on top also they had some non static foam jerry gave me to cover or pertect the sides , all in all I think it was my fault from my 35mph  full reverse accident sending the board 5 feet into the air
```

---
## \#111 Posted by: Exiledd_Top Posted at: 2018-04-12T04:15:45.248Z Reads: 181

```
After more further inspection ![20180411_211436|374x500](upload://wV9HJGtkH4a4UoLUkvucgU41Gwf.jpg)
![20180411_211437|374x500](upload://13HXA2LVGKwTj1hdXdV3kzcp6so.jpg)
```

---
## \#112 Posted by: Mikenopolis Posted at: 2018-04-12T04:18:15.894Z Reads: 167

```
Holy hell do not ship that. Last thing we need is a flaming UPS truck. Maybe you can have @psychotiller in Lake Forest take a look and isolate the issue before shipping?

Where is @willpark16 these days anyway? Did his injury stop him form persuing the hobby?
```

---
## \#113 Posted by: Exiledd_Top Posted at: 2018-04-12T04:20:49.623Z Reads: 170

```
Lol. Yeah not sure I got some shrink wrap coming in I could probably wrap it and ship it ?
```

---
## \#114 Posted by: Mikenopolis Posted at: 2018-04-12T04:23:07.639Z Reads: 166

```
The wrap is not going to prevent metal to metal contact.
```

---
## \#115 Posted by: Exiledd_Top Posted at: 2018-04-12T04:25:27.953Z Reads: 163

```
I mean I rode it like that unaware for like a week so, am sure it won't catch fire , they exsplains a lot why I felt my board was wonky and weird and brakes were not there there like soft brakes I just thought foc soft break things
```

---
## \#116 Posted by: Mikenopolis Posted at: 2018-04-12T04:28:50.681Z Reads: 160

```
That was basically what my Saturday ride was. Jittery here and there. I thought FOC and FocBox was the issue again 

Idk. Wouldn’t Jerry be able to help with this?
```

---
## \#117 Posted by: barajabali Posted at: 2018-04-12T04:32:21.786Z Reads: 156

```
Well there is your problem, not something I like to see but it looks like that fall from 5 feet really fucked up the pack. 

If you can get in there and rip the nickel strip out carefully, and then ship it to me. that would be ideal
```

---
## \#118 Posted by: Deckoz Posted at: 2018-04-12T04:36:26.819Z Reads: 153

```
So the lesson here is...

If your enosure falls off... Don't put it back on without completely inspecting the battery..
```

---
## \#119 Posted by: Exiledd_Top Posted at: 2018-04-12T04:40:36.278Z Reads: 148

```
Yes sir I didn't bother to check the sides because the foam was still there on the sides but funny enough what took all or most of the impact was the motor can and its scratched but no broken magnet lol the motor can survived a direct impact while it was in the air  and landed on the motor can like a plane taking a dive.
```

---
## \#120 Posted by: Deckoz Posted at: 2018-04-12T04:43:56.844Z Reads: 150

```
True..but if rattles can rip spot welds... No doubt dropped enclosure can. Be careful...that pack could be more volatile then you think...
```

---
## \#121 Posted by: Exiledd_Top Posted at: 2018-04-12T04:51:41.704Z Reads: 152

```
Conclusion time
Battery spot welds broke but still touching a little after my 35mph reverse incident making board fly 5 feet into the air not knowing battery was damaged.
One week after that I rode it and realized board was a bit wonky with loose brakes thought nothing of it.
Rode official like a full on ride to school board was at 95% trying to pull  so much Amp with broken welds caused the board to sag to 12%,(39v) and making all 4 vesc shut off or stop
```

---
## \#122 Posted by: Deckoz Posted at: 2018-04-12T04:54:01.323Z Reads: 143

```
Now that you know, how's the body damage doing.
```

---
## \#123 Posted by: Exiledd_Top Posted at: 2018-04-12T04:56:58.944Z Reads: 141

```
Body wise chicks don't dig it bro, I think they will soon dig it when my gear arrives soon.  Lol...
Anyways my shoulders feel fine now but my left ankle is still pretty bad . Got scuffed up from rolling but there just bruises scratches from rolling. Overal left ankle probably going to have to go to the doctor to check it out
```

---
## \#124 Posted by: Mikenopolis Posted at: 2018-04-12T05:09:40.326Z Reads: 145

```
[quote="Mikenopolis, post:101, topic:51744"]
my weekend ride
[/quote]

I notice my board being a bit weird the second I throttled at the beginning of the ride. It took 11 miles before the wire fully broke off
```

---
## \#125 Posted by: E1Allen Posted at: 2018-04-12T05:35:10.622Z Reads: 143

```
[quote="Exiledd_Top, post:109, topic:51744"]
question being is why did my battery go from 95% to 12% in the span of 2 miles
[/quote]

I don't think it did.

[quote="Exiledd_Top, post:121, topic:51744"]
Rode official like a full on ride to school board was at 95% trying to pull  so much Amp with broken welds caused the board to sag to 12%,(39v) and making all 4 vesc shut off or stop
[/quote]

So, I think your battery was full going up the hill.  However I don't think your board "sagged" to 12% causing your VESC to quit.  I think the broken welds under a huge load of amps shorted making it literally go from full amps to cutoff or 0v but since you were going uphill fast any large decrease wether making your VESC hit LVC or momentarily zero volts caused you to come off the board.  

With your damaged "full" battery in the case there probably was something causing the voltage to drain down to what you see now which is 12%

Just some thoughts because your full battery should have made it up the hill no problem and not go to 12%


Also I'd start separating those batteries sooner than later, maybe some survived.

Also also really glad you're okay.  That's a real fast speed to come off a board.
```

---
## \#126 Posted by: willpark16 Posted at: 2018-04-13T04:05:59.437Z Reads: 137

```
Present and accounted for! Been off the forums for a while now I come back and check every day or so just to look around. Haven’t completely healed from my injury mentally but physically I am all good now. I’ve been spending my time reaclimating myself to everything I used to do Esk8 wise. Haven’t had the courage to hop back on a board yet. If anyone needs me just send me a pm though and I’ll get back to you when I can, won’t be building or selling anything for a little bit longer though😢 thank you though to everyone who offered their support and get well wishes and especially my customers some of whom waited 6 months for me to finally get them their product!!!(can’t thank you enough)
```

---
## \#127 Posted by: willpark16 Posted at: 2018-04-13T04:12:24.352Z Reads: 134

```
One thing I’ve noticed is a couple injury’s becoming more abundant or perhaps they’ve been happening and people are just now reporting them. Outside of warning everyone to wear their helmets I was wondering if anyone has looked at the new Carvon’s on 12s as I’ve seen 3 serious accidents on these in the past 6 months. Not at all blaming Carvon!!!! Just curious to see if it’s been looked at. I can’t say mine was Esk8 related because I lost my entire memory of the accident and only know I had my board with me at the time and don’t know if I was riding or walking during my accident so for the time being it is assumed I was hit by a car. I would say that while Vests have worked fine for some at 12s perhaps 10s really is the safe zone for these boards using vesc or perhaps the remotes are having dropouts? Again though, this is just speculation and guessing but what is certain is to ride safe guys and wear proper gear!!!! -end rant😂
```

---
## \#128 Posted by: Exiledd_Top Posted at: 2018-04-13T04:23:30.444Z Reads: 134

```
Carvons are not the problem I would be the first one to tell u because I have bin using them daily and there no issues i have put some together and the only problem. I could see is if there  could ever be one could be over heat if u ride aggressive(40mph)  for a very long time at 12s or bomb to many hills going up hense they have sensors. There's nothing I can see that would cause them to stop or fry , you could iether destroy a magnet or destroy the inside bearing that's about it.
```

---
## \#129 Posted by: willpark16 Posted at: 2018-04-13T04:25:15.663Z Reads: 133

```
Figures, mine weren’t fried either because they ride fine righ after
```

---
## \#130 Posted by: Exiledd_Top Posted at: 2018-04-13T04:25:32.071Z Reads: 132

```
[quote="willpark16, post:127, topic:51744"]
Carvon’s on 12s
[/quote]

Reason people stay away from 12s is because it could pass or it passes the erpm limit, but carvon to low of a kV to even pass the ermp limit.
```

---
## \#131 Posted by: b264 Posted at: 2018-04-13T05:45:40.709Z Reads: 132

```
[quote="Exiledd_Top, post:130, topic:51744"]
Reason people stay away from 12s is because it could pass or it passes the erpm limit
[/quote]

I stay away from 12S because the components in a VESC are not rated high enough to be using those kinds of voltages.  And I value my safety.
```

---
## \#132 Posted by: webst Posted at: 2018-04-13T08:15:26.295Z Reads: 124

```
Isn’t VESC 6 rated up to 60V?
```

---
## \#133 Posted by: Acidfie Posted at: 2018-04-13T08:37:18.322Z Reads: 122

```
yeah, seems like no problem to me.
```

---
## \#134 Posted by: b264 Posted at: 2018-04-13T17:38:03.501Z Reads: 119

```
[quote="webst, post:132, topic:51744, full:true"]
Isn’t VESC 6 rated up to 60V?
[/quote]

This is the exact problem in fact.  That's not high enough to be running it over 50V before the back EMF.  There is no safety margin at all.
```

---
## \#135 Posted by: professor_shartsis Posted at: 2018-04-13T17:52:45.116Z Reads: 122

```
[quote="b264, post:134, topic:51744"]
That’s not high enough to be running it over 50V before the back EMF.
[/quote]

my understanding is Back EMF voltage **subtracts** from (opposes) the effective voltage of the controller and pack.

((Pack Voltage * Duty Cycle %) - BEMF Voltage) /  Winding Resistance = Motor Current

((50V Pack Voltage * 50% Duty Cycle %) - 24V BEMF Voltage [100kv @ 2400rpm]) /  0.05ohm Winding Resistance = 20a Motor Current

((25V "Effective" Voltage) - 24V BEMF Voltage) /  0.05ohm Winding Resistance = 20a Motor Current

(1V "Drive" Voltage) /  0.05ohm Winding Resistance = 20a Motor Current

25V "Effective" Voltage * 20a Motor Current = 500w Electrical Watts & Battery Watts
```

---
## \#136 Posted by: b264 Posted at: 2018-04-13T17:55:54.162Z Reads: 120

```
[quote="professor_shartsis, post:135, topic:51744"]
my understanding is Back EMF voltage subtracts from (opposes) the effective voltage of the controller and pack.
[/quote]

On the pulse rise it does, but on the pulse fall it adds to it
```

---
## \#138 Posted by: professor_shartsis Posted at: 2018-04-13T18:12:27.461Z Reads: 115

```
Source: http://vedder.se
Posted on January 7, 2015
"...Voltage: 8V – 60V (Safe for 3S to 12S LiPo)..."
```

---
## \#139 Posted by: b264 Posted at: 2018-04-13T18:17:38.676Z Reads: 121

```
I'm all about reliability and everything related to that, which includes staying at 10S, making everything water resistant AND waterproof, and shunning hub motors.

When someone designs a non-esk8 pcb that they want to run at 50V they will design it with components rated at 75V to 100V.  So I don't get it ... people think that just because it's inconvenient that it's okay to bend the rules here when the thing you're doing is actually decreasing your own safety.  And no, I'm still not okay with that.

I mean I understand that science is going out of fashion and that it's going to be turned off soon, but it's not off yet...
```

---
## \#141 Posted by: b264 Posted at: 2018-04-13T18:20:41.784Z Reads: 124

```
[quote="Deckoz, post:140, topic:51744"]
You realize that the only component rated for 63v is the DRV and the rest of the bom connected to the line voltage uses 100v caps?

And that the standard fets used are rated for 75v…
[/quote]

I'm fully aware of that.  You understand that DRV8302 failures are extremely common?  And that they cause a failure of brakes?
```

---
## \#143 Posted by: b264 Posted at: 2018-04-13T18:31:16.045Z Reads: 120

```
[quote="Deckoz, post:142, topic:51744"]
If ya can’t skate ya shouldn’t esk8.
[/quote]


So your response is effectively "it's okay if brakes fail"

Well whether you can skate or not, I disagree with you.
```

---
## \#144 Posted by: PredatorBoards Posted at: 2018-04-13T18:32:03.085Z Reads: 121

```
I definitely support the idea that everyone needs to learn how to do basic skating before they esk8. It's honestly really scary seeing newcomers go 22mph on their second day of riding. Whenever I get on their boards, their bushings are so tight that I can barely turn.
```

---
## \#146 Posted by: b264 Posted at: 2018-04-13T19:18:56.521Z Reads: 118

```
[quote="Deckoz, post:145, topic:51744"]
It’s not ok if brakes fail. But your need to know how to slow down doesn’t change.

If brakes fail on a car… What do you do? Oh wait you don’t drive cars… You might not know.

Same is true for skating. If you can’t skate the speeds you skate on an analog board, you shouldn’t be skating an esk8.
[/quote]

Your entire argument rests on the notion that "making one thing safer means the other thing can be less safe"

You're wrong.

All of it needs to be as safe as possilbe.

And for the record, I drove cars for a long time.  As-if that matters.
```

---
## \#148 Posted by: Exiledd_Top Posted at: 2018-04-13T20:02:15.237Z Reads: 112

```
Derailing my thread :slightly_frowning_face:
```

---
## \#149 Posted by: trancejunkiexxl Posted at: 2018-04-13T21:03:26.795Z Reads: 108

```
Have u gone to doc for your foot yet😞
```

---
## \#150 Posted by: Exiledd_Top Posted at: 2018-04-13T21:52:38.575Z Reads: 111

```
Am going sometime this week
```

---
## \#151 Posted by: willpark16 Posted at: 2018-04-13T22:28:17.001Z Reads: 112

```
I think tight bushings are good if you plan to ride at 22mph otherwise they may get speed wobble. Or is that incorrect? LOL
```

---
## \#152 Posted by: Exiledd_Top Posted at: 2018-04-13T22:40:23.195Z Reads: 112

```
97a riptide  double barrel with bones 96a hardcore bushings and a 97a riptide cone no speed wobles at high speeds weigh 175LB turns okay but I don't mind the turn raduis I actually love it
```

---
## \#153 Posted by: willpark16 Posted at: 2018-04-13T22:46:34.873Z Reads: 115

```
Next build I’ll try it out
```

---
## \#154 Posted by: pat.speed Posted at: 2018-04-13T23:00:05.388Z Reads: 111

```
I think what @PredatorBoards is trying to say is that they have no proper control over speed wobbles, so they tighten the bushings as much as possible.

I think that is one thing everyone needs to learn is to have solid ankles and good balance to mitigate speed wobbles. In my experience I have hit 50km/h multiple times on stock bushings with medium tightness and not a wobble in sight. I think this comes down to riding skateboards for 5-6 before esk8.
```

---
## \#155 Posted by: GrecoMan Posted at: 2018-04-13T23:06:22.003Z Reads: 106

```
those are some hard ass bushings

i ride 92a cone/barrel.
```

---
## \#156 Posted by: deucesdown Posted at: 2018-04-13T23:07:19.753Z Reads: 108

```
I mostly agree but I wired the phase wires wrong on a board and ended up riding backwards, motors up front. Wobs! Even after tightening both trucks. And weight forward, confident and relaxed. Back truck just shimmying back and forth as I picked up speed.

Fixed wiring and readjusted kingpin screws and next day stable as f.
```

---
## \#157 Posted by: Mikenopolis Posted at: 2018-04-13T23:22:07.278Z Reads: 102

```
I use Bones 96a, with my usual backpack of stuff I'm maybe like 220-230lbs
```

---
## \#158 Posted by: GrecoMan Posted at: 2018-04-13T23:22:43.766Z Reads: 102

```
that’s probably about equal to my setup, i’m 145lbs
```

---
## \#159 Posted by: Exiledd_Top Posted at: 2018-04-14T01:50:14.183Z Reads: 102

```
With my entire gear and school stuff I weigh just around 195lb, sometimes 200
```

---
## \#160 Posted by: E1Allen Posted at: 2018-04-14T02:09:28.796Z Reads: 106

```
I'm with you, same duro bushings.  About same weight.  I've have it dialed in so I can carve and hit top speed with no wobbles.
```

---
## \#161 Posted by: pixelsilva Posted at: 2018-04-14T03:08:04.612Z Reads: 107

```
I don't think speculating will be the course to go. Exploding batteries could be by other causes. Otherwise we will start on blaming Carvon about batteries like today public and press blames Tesla on autopilot related accidents. This is the new frontier and we are the new explorers. Exploring new frontiers comes with a lot of risk. Like Ernest Shackleton antarctic expedition hiring ad read:


![image|690x343](upload://7nS31NE4hXNoVJxzRtnLlJL28gT.jpg)http://thebigtimegroup.com/wp-content/uploads/2016/02/about_bg.jpg
```

---
## \#162 Posted by: willpark16 Posted at: 2018-04-14T04:04:19.235Z Reads: 104

```
Exploding batteries? I didnt say anything about that...
```

---
## \#163 Posted by: pixelsilva Posted at: 2018-04-14T04:37:45.713Z Reads: 106

```
> @willpark16
> Carvon’s on 12s as I’ve seen 3 serious accidents on these in the past 6 months. Not at all blaming Carvon!!! Just curious to see if it’s been looked at.

Well, perhaps I misinterpreted what you said. But my point is more about being more flexible about what we are achievieng here with new technology. I think this is a new ground and we all should spect certainly level of risk in all what we do in Esk8. Cheers man. :wink:
```

---
## \#164 Posted by: gstpierre Posted at: 2018-04-19T21:35:49.962Z Reads: 96

```
Another problem I experienced with them would be that they are conductive, and I had phase wires short by touching the carbon fiber and not being properly insulated.
```

---
## \#165 Posted by: Redfire1 Posted at: 2018-04-26T22:05:05.908Z Reads: 89

```
@E1Allen hi I am trying to make a electrical skateboard for so long but keep on hitting walls,hopefully I can finish it this weekend,I am using maytech VES dual and 170kv motor I would like to know how to set the LVC can you are anyone help.
```

---
## \#166 Posted by: E1Allen Posted at: 2018-04-26T22:39:18.188Z Reads: 89

```
![IMG_4866|281x500](upload://pZ5RiQXjXOWhEWZYb6HOjbABh0x.jpg)

I've set my battery cutoff end at 3v per cell.  That's plenty conservative for liion. Lipo need higher cutoff.  So it's up to you.  It won't shut the board down, it will just slowly get slower.
```

---
## \#167 Posted by: Deckoz Posted at: 2018-04-26T22:56:56.341Z Reads: 86

```
Why is your battery max 60v... It really should be 57...
```

---
## \#168 Posted by: E1Allen Posted at: 2018-04-26T23:22:46.568Z Reads: 82

```
Good question.  It's that going to limit the volts while braking to the battery?  I didn't get much input or reading on voltage Max
```

---
## \#169 Posted by: Deckoz Posted at: 2018-04-26T23:26:57.492Z Reads: 84

```
No... I'm on 13s and never hit the 57v cuttoff while braking. Nor does pshaw. The 57v is to turn off the fets if you hit it to not kill components ie the DRV from transients.(60v max, 5sec/63v burn)
```

---
## \#170 Posted by: E1Allen Posted at: 2018-04-26T23:44:24.020Z Reads: 81

```
Makes sense. I shall change cutoff values.
```

---
## \#171 Posted by: Redfire1 Posted at: 2018-04-27T05:08:11.531Z Reads: 78

```
@deckoz I am using 10S and VESC TOOl cause BLCD tool don’t work for my vesc is it the same can I see a pic of your setup please
```

---
## \#172 Posted by: Deckoz Posted at: 2018-04-27T11:43:37.804Z Reads: 69

```
57v is default and should be left as is for max.
```

---
