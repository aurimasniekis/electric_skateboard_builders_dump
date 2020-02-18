# Trampa EMTB 8072 Sensored Alien Motors with E-toxx Direct drive

### Replies: 116 Views: 3263

## \#1 Posted by: Risewithin Posted at: 2018-08-17T15:17:52.938Z Reads: 358

```
First I just wanna thank whoever created this awesome site and for all the people who contribute their knowledge and ideas!! I'm starting my very first build and would like to share my experience with everyone here and hopefully help the next guy in line wanting to take on the very challenge of building their first board!!
 I've read and read and read a lot and still have so many questions! lol. Digging into the electronics of this has been the most challenging for me, just with the different options, connections, gauges, etc. Im getting a little older so its getting slightly harder to digest all this information at once so re-reading and watching videos is key for me! So lets go over the game plan and parts list I have or is on the way so far and maybe someone may see some design flaws or challenges I may experience and can help me before I get too ahead of myself lol. 
The idea and goals:
- To have good torque 
- But to also be able to limit it and expand it as my skill level increases 
- Be able to go long distances when needed (30+ miles) 
- Be able to jump so top battery placement is a must 
- Go fast when needed (30+ mph) 

Parts purchased:
- Trampa MTB 
- E-toxx 80mm Direct drive 1:5 gear ratio
- Alien 8072 sensored motors at 250kv 
- 2x Flipsky Fsvesc 6.6 no hw limit firmware 
- 12s8p 30Q battery pack 
- 10awg silicone wire, 5.5 gold bullet connectors, heat shrink, etc 

Jens is working on my hanger as we speak, board and VESC's  are  already in, motors be in Monday, spot welder, batteries and accessories within a week or two! 
First challenge is to see how Im going to mount the Flipsky Vescs to the board! They are already in their own little aluminum case with anitspark switch but I'll have to build a little holder for them probably out of aluminum. Thinking of adding a fan to the enclosure just to ensure things stay cool. Anyone have any good ideas of a good VESC holder for Trampa boards? It's hard to do right now cause I have no clue where the motors and Drives will sit after installation.

That's it so far, I feel like I'm on the right path to meet all my goals. Anyone see anything that stands out that could be a problem?
```

---
## \#2 Posted by: Risewithin Posted at: 2018-08-17T15:18:47.719Z Reads: 325

```
![IMG_4106EEA2C823-1|690x318](upload://eAb9ZM0wLHsLEyFRNKVaDgQE4o7.jpeg)
```

---
## \#3 Posted by: Risewithin Posted at: 2018-08-17T15:22:38.854Z Reads: 326

```
Not sure if accurate 

![51%20AM|690x331](upload://7d81G2gqRSwuzV4MGWWL4KUYJvF.png)
```

---
## \#4 Posted by: Klaerke91 Posted at: 2018-08-17T18:22:42.253Z Reads: 302

```
How do you want to mount your battery. Under or over your board?
```

---
## \#5 Posted by: Risewithin Posted at: 2018-08-17T18:48:07.534Z Reads: 301

```
Up in thread it says I have to do top mount due to jumps brother. I plan on building a nice block like Jens did on his leopard 80mm build.
```

---
## \#6 Posted by: Klaerke91 Posted at: 2018-08-17T19:00:52.621Z Reads: 292

```
Well i need to read slower. Missed the "top" word in that sentence. :upside_down_face:

I personally dont like top mounted batterys as it look really ugly with a big box on top of your board.
Have you seen the enclosure that @Eboosted makes. I have just received mine and its awesome.
```

---
## \#7 Posted by: Risewithin Posted at: 2018-08-17T19:28:33.175Z Reads: 285

```
Yes I love the look of it but for my riding style its not functional. With Jumps your board is going to flex to the ground sometimes and landing on your battery pack is a big no no lol. Thats why the aggressive MTB riders have their battery boxes on top! Also I hate to be limited to a 5p configuration for now
```

---
## \#8 Posted by: Nate Posted at: 2018-08-17T19:56:00.685Z Reads: 279

```
Go lipo if you want that “kick”. I’m using 8085 top mounted with 12S lipo pack with fvt esc, that punch by the motor on every acceleration will scare the shit out of you. You won’t want to go back to any other “smaller” set up if you’re a torque junky.
```

---
## \#9 Posted by: Risewithin Posted at: 2018-08-17T20:07:10.460Z Reads: 280

```
Oh man you have any videos?  I was going lipo at first but decided for a longer lasting battery. Still going to get ~150 amps so its still going to provide a proper punch I believe!
```

---
## \#10 Posted by: Nate Posted at: 2018-08-18T03:50:27.135Z Reads: 282

```
No, i never take any video when i ride, kind of difficult as i'm not used to the wheelies. 

It really depends on which esc you go with. I couldn't replicate the same "kick" on vesc because the FVT esc pulls a lot of amps on initial acceleration that the 150amps bms will kick in and cut power for half a sec, which was enough to stop the momentum of the acceleration. So my solution was to ditch the bms and only use it to charge. I use lipo alarm to check voltage levels instead and supply the esc with as much "juice" as it wants. 

But ya, lipos are not good for longevity but they do provide the punch you're looking for. My thinking is this, if you're gonna build a proper torque machine, might as well go all out and leave no stone unturned.
```

---
## \#11 Posted by: Risewithin Posted at: 2018-08-19T00:22:26.249Z Reads: 277

```
![image|375x500](upload://ss3xsYbuxz8xPHDjKXBcxwCdhym.jpeg)![image|375x500](upload://gP1uONH0aX42uix57WBDj9vWvOz.jpeg)
```

---
## \#12 Posted by: Risewithin Posted at: 2018-08-19T00:26:20.497Z Reads: 260

```
Have the mock-up for the Flipsky Fsvesc. Now I need to get some 1/8” aluminum plate to do the real thing. May wait until I get the drive system from @Nowind to make sure nothing gets in the way.
```

---
## \#13 Posted by: Holyman92 Posted at: 2018-08-20T17:55:22.881Z Reads: 258

```
looking good man, I'll keep an eye on this build so i know what i'm lookin at when we ride
```

---
## \#14 Posted by: Risewithin Posted at: 2018-08-20T18:54:30.519Z Reads: 261

```
![image|375x500](upload://6FyPckhkDWr1J9AO3mTTqHqzWvM.jpeg)

New motors are in!! Look at the size difference from my Evolve motor 🤭
```

---
## \#15 Posted by: Nowind Posted at: 2018-08-20T19:38:11.732Z Reads: 253

```
[quote="Risewithin, post:12, topic:65188, full:true"]
Have the mock-up for the Flipsky Fsvesc. Now I need to get some 1/8” aluminum plate to do the real thing. May wait until I get the drive system from @Nowind to make sure nothing gets in the way.
[/quote]


ESC Sandwich is good (-: YAMI
mounted my VESC this way too, but deeper on the Tip ( alot lower )
Why going this high?
```

---
## \#16 Posted by: skatardude10 Posted at: 2018-08-20T19:42:37.685Z Reads: 250

```
Omfg I can't wait to see these beasts mounted up!
```

---
## \#17 Posted by: Holyman92 Posted at: 2018-08-20T21:18:19.237Z Reads: 247

```
hey @Nowind ur adaptor plats for the leapord motors... would those technically work for any mount if they had the 63mm mounting holes?
```

---
## \#18 Posted by: Silverline Posted at: 2018-08-20T21:51:09.419Z Reads: 253

```
Hope you have more luck with that motor, than me and @DK-Odense :-/ We both got lot af stutter at certain rpm`s.....

https://www.youtube.com/watch?v=yxok02O2vSM

https://www.youtube.com/watch?v=8bVVYADISpU
```

---
## \#19 Posted by: Holyman92 Posted at: 2018-08-20T21:56:21.074Z Reads: 244

```
did y'all have the AS5047 Encoder installed? or using hall sensors?
```

---
## \#20 Posted by: Silverline Posted at: 2018-08-20T22:00:01.853Z Reads: 247

```
We tried, bldc with and without hall sensor, and foc with and without hall sensor. The problem did not disappear at any time.
```

---
## \#21 Posted by: Holyman92 Posted at: 2018-08-20T22:01:59.926Z Reads: 234

```
that is strange indeed... I plan to use the encoder instead of hall sensors and im also going to be using leopard 80mm motors, but yea
```

---
## \#22 Posted by: Silverline Posted at: 2018-08-20T22:03:27.895Z Reads: 238

```
Yes.... fortunately Bruno took them back. But it`s sad, because its an awesome motor size for MTB :-)
```

---
## \#23 Posted by: ArnhemAnt Posted at: 2018-08-20T22:04:25.491Z Reads: 235

```
I'm getting close to finishing my Trampa build. That pic with the 'ESC sandwich' has just given me another option for mounting my ESCapes- thanks man.
```

---
## \#24 Posted by: Holyman92 Posted at: 2018-08-20T22:16:43.554Z Reads: 227

```
yea they are lol... im having APS make some custom KV motors with no termination for a project im trying to make with a buddy from school and i've not heard anything negative about APS motors until now... however i wont be changing my mind, they're still gonna make me the motors lol
```

---
## \#25 Posted by: Silverline Posted at: 2018-08-20T22:19:42.342Z Reads: 222

```
APS 63xx motors are rock solid.... Good luck with your motor project , sounds interesting 😀
```

---
## \#26 Posted by: Holyman92 Posted at: 2018-08-20T22:26:20.045Z Reads: 216

```
great cause thats what im getting made haha
```

---
## \#27 Posted by: Risewithin Posted at: 2018-08-21T00:03:54.262Z Reads: 218

```
[quote="Nowind, post:15, topic:65188"]
ESC Sandwich is good (-: YAMI
mounted my VESC this way too, but deeper on the Tip ( alot lower )
Why going this high?
[/quote]

Just a rough mockup for now. I wanna bring them lower but I'll have to wait until your awesome drives come in so I know where I can build them. I have some aluminum plate for the final product! I may put a slight cavity on the front to hold receiver and bluetooth module.
```

---
## \#28 Posted by: Risewithin Posted at: 2018-08-21T00:05:29.356Z Reads: 221

```
[quote="Silverline, post:18, topic:65188, full:true"]
Hope you have more luck with that motor, than me and @DK-Odense :-/ We both got lot af stutter at certain rpm`s…
[/quote]


Oh man you know the first thing I saw when I got these were loose windings and it bothered me a bit but I told myself @AlienPowerSystem is an awesome company and they know what they're doing! Crossing my fingers, I really want these to work good!!
```

---
## \#29 Posted by: Risewithin Posted at: 2018-08-21T00:06:16.798Z Reads: 226

```
[quote="skatardude10, post:16, topic:65188, full:true"]
Omfg I can’t wait to see these beasts mounted up!
[/quote]


Me too!!! I wish I had all the parts in so I could work my butt off and get it going!!!
```

---
## \#30 Posted by: Risewithin Posted at: 2018-08-21T01:17:26.645Z Reads: 235

```
![image|375x500](upload://pIyjMEgPnkKeAFeW9xsAOzBC20F.jpeg)

Got the batteries in. Checked every single one of them and they are all 3.86 +/- .1v. ✔️
25’ pure nickel strip. ✔️
1/2” pure braided copper ✔️
Heat shrink ✔️ 
XT90 connectors ✔️ 
Braided wire cover ✔️ 
10awg silicon wire ✔️ 
Motors ✔️ 
Direct drives 🔜 
Flipsky’s Vesc ✔️ 
Board ✔️ 
Spot welder 🔜 
Aluminum for vesc enclosure ✔️ 
Battery charger 🔜 
Battery box 🔜 got wrong size kind of 
Remote ✔️ 
Xt60 charging port 🔜 
Vesc tool downloaded and ready ✔️ 

Am I missing something?
```

---
## \#31 Posted by: ZmasteR Posted at: 2018-08-21T02:25:18.686Z Reads: 213

```
Fuse and BMS ?
```

---
## \#32 Posted by: Risewithin Posted at: 2018-08-21T03:00:56.540Z Reads: 210

```
Oh yeah I do have BMS coming and forgot to put that in there.  I haven't checked on fuse yet, probably a god idea!!
```

---
## \#33 Posted by: Risewithin Posted at: 2018-08-21T03:09:59.550Z Reads: 213

```
[quote="ZmasteR, post:31, topic:65188, full:true"]
Fuse and BMS ?
[/quote]


Question about fuse.  If my battery has the max capacity of 160 amps, those Amps will be split into two Flipsky Vescs that can handle 150A Burst each, according to them. BMS is rated 150 amps as well. So what size fuze should I get and where should I put it?  Thanks
```

---
## \#34 Posted by: ZmasteR Posted at: 2018-08-21T03:22:47.474Z Reads: 205

```
I would advise to take advice from more skilled people around here.
For me a 120A on the main PSU line did the trick so far.
But you can put one on each ESCsince they're supposed to handle this amount of current. To be checked that said.
```

---
## \#35 Posted by: Andy87 Posted at: 2018-08-21T05:01:03.901Z Reads: 222

```
If you use a bms and a fuse you go double safety. If you choose the fuse to 150a I guess your bms will cut off before the fuse burn.
Usually the fuse can handle the marked amps for constant current. Make sure that you get the right fuse to your voltage. Most car fuses 32V but there also 58V which would fit better for a 12s setup.
```

---
## \#36 Posted by: DK-Odense Posted at: 2018-08-21T05:36:24.788Z Reads: 230

```
@Silverline and I bought 6x 8072S - All failed :-(

https://www.youtube.com/watch?v=f-diUOkPGPE

https://www.youtube.com/watch?v=he0yy7EHB40

https://www.youtube.com/watch?v=LFQSmIPuAU8
```

---
## \#37 Posted by: xilw3r Posted at: 2018-08-21T05:39:54.209Z Reads: 226

```
When going for a fuse be sure to check the graphs at the manufacturers site, they show for how long what ammount of amps the fuses can take. For example, some can take the rated amps for 60s before melting, others can take rated amps for 0.1s before melting :slight_smile:

@Silverline  @DK-Odense in the videos that sounds just like a resonance to me. With a bigger diameter bell resonance effects will be more pronounced. And I bet that the bell was not dynamically balanced. Then if you add the magnets at a slightest offset it will make matters worse. But it did not sound too bad at all, I think it should be usable if it is not shaking too much.
Or is there something more I dont see?

Edit: I saw the vibration on the last video from DK-Odense...... that sucks. Looks like the whole bell is violently vibrating.

@Risewithin Those motors look insane, jeebus. I am very interested to see how FlipSkys work out for you. And that battery... lawd almighty.. This build probably costs like 2x more than  my car :D
```

---
## \#38 Posted by: DK-Odense Posted at: 2018-08-21T05:47:10.736Z Reads: 218

```
Yep - When the stutter/vibration kicked in at a certain level of RPM there was a loss in power, and you felt this very much riding your board. If the board was running smooth i could live with the sound, but there was a massive loss in power.
```

---
## \#39 Posted by: Nate Posted at: 2018-08-21T05:55:36.139Z Reads: 212

```
Sorry to go off topics @Risewithin.

 What kind of gear drive are you using @DK-Odense? I see those Korean wheels gears alllllll the way back there :eyes::eyes::eyes:
```

---
## \#40 Posted by: Nowind Posted at: 2018-08-21T07:28:11.184Z Reads: 231

```
[quote="Holyman92, post:17, topic:65188, full:true"]
hey @Nowind ur adaptor plats for the leapord motors… would those technically work for any mount if they had the 63mm mounting holes?
[/quote]

Yeah technically for sure !

[quote="Holyman92, post:21, topic:65188, full:true"]
that is strange indeed… I plan to use the encoder instead of hall sensors and im also going to be using leopard 80mm motors, but yea
[/quote]

The Leopard copper fillment is really high, also the design is very sexy IMO.
Have used them with AS5047 too, okay one Motor failed at some point, but i used the Leopard already since around 2 years... 
https://www.youtube.com/watch?v=7dfILUz61CQ

[quote="xilw3r, post:37, topic:65188"]
Those motors look insane, jeebus. I am very interested to see how FlipSkys work out for you. And that battery… lawd almighty… This build probably costs like 2x more than my car :smiley:
[/quote]

Also interrested how the Flipsky work with the Alien !
```

---
## \#41 Posted by: Holyman92 Posted at: 2018-08-21T07:46:59.267Z Reads: 216

```
[quote="Nowind, post:40, topic:65188"]
Yeah technically for sure !
[/quote]

Awesome, I may need to get them for my current build I'll find out soon
```

---
## \#42 Posted by: Risewithin Posted at: 2018-08-21T10:54:25.706Z Reads: 212

```
Thanks @Andy87 and @xilw3r for the fuse info!! 

@DK-Odense oh man that’s terrible and has me severely worried. How long ago was that? Did you ever find the cause? Looks like the bell bowed at at its resonant frequency which makes sense with the loss of power due to the magnets being pulled away not making great contact. 

@AlienPowerSystem do you guys know what caused this or a solution? 

@Nowind hey brother will that drive system work with the leopards? Looks like I may have to switch if these Alien motors don’t work right.
```

---
## \#43 Posted by: DK-Odense Posted at: 2018-08-21T11:09:33.558Z Reads: 201

```
About 3 months ago.

We tried with different vescs and different setup/motor detection parameters. We ended up concluding that this motor just did'nt fitted for this type of task. Bruno from aps was super cool about it, and just said that we could send it back and we figure something out.

I have two 80100 running without probs, so it is not a "80 mm" problem.
```

---
## \#44 Posted by: Nowind Posted at: 2018-08-21T12:03:44.761Z Reads: 199

```
[quote="Risewithin, post:42, topic:65188"]
@Nowind hey brother will that drive system work with the leopards? Looks like I may have to switch if these Alien motors don’t work right.
[/quote]


Nope,
Alien APS 80mm has different Bolting Circle then LEOPARD

I used 8085 and 80100 APS Motors without any problems.
Good Motors , Fair Prices, nothing to complain
```

---
## \#45 Posted by: Risewithin Posted at: 2018-08-21T12:09:36.012Z Reads: 192

```
Ok cool I’ll switch over to one of them if these don’t work out! Thanks brother!
```

---
## \#46 Posted by: Risewithin Posted at: 2018-08-21T12:11:09.142Z Reads: 197

```
[quote="DK-Odense, post:43, topic:65188"]
I have two 80100 running without probs, so it is not a “80 mm” problem.
[/quote]

I will try this one out next if this is a problem for me. Thank you!
```

---
## \#47 Posted by: Risewithin Posted at: 2018-08-21T23:18:40.158Z Reads: 205

```
![image|374x500](upload://fte3NZ15Z6mAGVB8P6BnpJSpidt.jpeg)

Started working on the vesc holder. Will trim off the tail when I figure out exactly where I want it to sit.
```

---
## \#48 Posted by: Riako Posted at: 2018-08-22T11:21:25.745Z Reads: 205

```
Hey mate ! Massive beast coming here :yum:
Just to report (what I could, and if it could help a bit), the noize doesn't sound that bad on some video here ... I mean its a "standard" from APS motor no ?
The RSPEC got a special noize too at some rpm ?
I admit that here it's worse ... your problem 3 vid is a bit scary.

Did you think guys this could come from the under-sizing bearing and all inside stator-rotor configuration make like 63xx motor?
Opposite to the 8085/100 who got huge bearing inside and weight a lot more (I have dissected mine for a project not used yet, that what scared me a bit since this. And got an 8085 not set yet), it looks getting [bigger/better](https://www.youtube.com/watch?v=yZoEGcTtR-Q) quality and strongest conception ... (IMO at 1st looking in hand). As bearing and also 10mm shaft against 12... for example.
Did the high kV could be an issue on a big motor like this ?..
refound some old vid of my APS 63xx, sound a little bit like you : 
https://youtu.be/TPcN76FxFjg
https://youtu.be/_ffUzkjkFus

Cool setup anyway ! :smiley: I will follow this crazy big toy setup !!
```

---
## \#49 Posted by: Silverline Posted at: 2018-08-22T13:30:02.929Z Reads: 196

```
Maybe. My bearings on 8072 was not smooth at all
```

---
## \#50 Posted by: Riako Posted at: 2018-08-22T14:47:49.961Z Reads: 202

```
I was more thinking about the size, and maybe the design and implementation of them : 
https://alienpowersystem.com/wp-content/uploads/2017/10/20171031_140100.jpg
https://alienpowersystem.com/wp-content/uploads/2016/04/20160414_143708-FILEminimizer.jpg
... just look stronger on the 8085/80100 one !

for the stator copper/wires, should we resin it ?
https://discourse-cdn-sjc1.com/business6/uploads/openrov/_optimized/5bc/d06/d93c2e0a29_543x480.jpg
https://discourse-cdn-sjc1.com/business6/uploads/openrov/3254/92be0712c6b36826.jpg
I would like to upgrade them before to be disappointed :smile: ?!?
```

---
## \#51 Posted by: Risewithin Posted at: 2018-08-22T20:08:19.290Z Reads: 193

```
![image|374x500](upload://ek4X50Q1xB5W2bB7EeWLUbqK05n.jpeg)

I think I am done with the vesc holder for now. Got the spot welder in today so about to start putting the battery pack together! Pray for me lol
```

---
## \#52 Posted by: Risewithin Posted at: 2018-08-22T23:04:06.049Z Reads: 196

```
![image|666x500](upload://wrqgHiBhN3Vsddo0b2WLHJP7lAy.jpeg)

Busy busy 😁
```

---
## \#53 Posted by: Risewithin Posted at: 2018-08-23T00:19:02.505Z Reads: 192

```
![image|666x500](upload://wGKKvkYIZxpepg39TxJGJF3UG4q.jpeg)

Have dual layer nickel strip 8mm .15 pure. Then adding these copper wires in series. Then it’ll be silicone tapes and heat shrinked
```

---
## \#54 Posted by: Risewithin Posted at: 2018-08-23T02:38:14.279Z Reads: 190

```


![image|230x500](upload://yPWrHTF1Rb0kVzO3riKqkf6LAf6.jpeg)

Waiting for bms to come in. Going to hook up vesc’s tomorrow temporarily to set them up with the motors so I’ll be ready for @Nowind direct drives when they get here!!
```

---
## \#55 Posted by: 2Old2Sk8 Posted at: 2018-08-23T14:53:40.470Z Reads: 184

```
12s8p?  Nice!  I am no expert on building batteries having only built one myself so far but it seems to me that by using only 2 layers of 8mm x .15 nickel you are limited to only about 40 amps max capacity in your series connections which is not nearly enough for what those motors will draw or what that pack could produce.  But maybe you know something I don't?...
```

---
## \#56 Posted by: Risewithin Posted at: 2018-08-23T15:33:31.570Z Reads: 175

```
I don’t know a lot about batteries myself. From what I understand from reading replies from some battery guys in here is that the parallel connections don’t have to be so robust. The series connections is where it’s needed most. We’ll see though. If things get hotter than I’d like or the motors don’t het the acceleration desired I’ll try adding some copper wire to the parallel connections to see if it makes a difference
```

---
## \#57 Posted by: Silverline Posted at: 2018-08-23T15:42:31.893Z Reads: 175

```
For i build like that, with those big motors. I would go with lipo instead.
```

---
## \#58 Posted by: 2Old2Sk8 Posted at: 2018-08-23T15:55:42.836Z Reads: 178

```
I guess you don't understand what I am saying.  Your parallel connections would be more than adequate if it was only handling parallel current but because you don't have direct cell to cell series connections it must also handle series current and is therefore insufficient.
```

---
## \#59 Posted by: Risewithin Posted at: 2018-08-23T17:00:12.315Z Reads: 184

```
Oh I see you think the distance bereeen the series connections are too far apart and probably not enough causing the voltage to travel down to each connection before crossing.
```

---
## \#60 Posted by: Klaerke91 Posted at: 2018-08-23T17:11:57.453Z Reads: 187

```
Take a look at this video. Good explanation on this issue

https://www.youtube.com/watch?v=wdZ_Ca_sAZE
```

---
## \#61 Posted by: Risewithin Posted at: 2018-08-23T23:42:54.391Z Reads: 177

```
Since all he's talking about is nickel strips how do you figure out how much copper wire do you need? These are 1/2' strips about 1mm thick

added two more strips of copper. Thats gotta be plenty lol
```

---
## \#62 Posted by: michaelcpg Posted at: 2018-08-24T01:12:16.979Z Reads: 173

```
Two strips of that size should be enough to handle the total current between each series group but the issue is, like you mentioned, because you have the copper soldered near each end of each series group, the current produced from the cells in the middle of each series group first have to run through a lot of thin nickel strip to reach the copper  at the end which isn't ideal. 

I would recommend soldering another two evenly spaced copper strips to each series group in between the two copper strips you've currently got soldered. This would mean that the current from each series group cell only has to travel across a couple cm of nickel strip at most to reach a copper strip.
```

---
## \#63 Posted by: michaelcpg Posted at: 2018-08-24T01:19:43.094Z Reads: 172

```
Another thing, be VERY careful with the sharp edges of the nickel strips on the positive sides of the cells. 

If one of the sharp edges of one of those strips pierces or scratches through the insulation around the positive cell terminals, you're going to get a short and a battery of that size that's closely packed together like that could very quickly start a runaway effect which will result in the whole pack going up in flames...

Ideally you should be rounding the corners of the strips so they can't come in contact with the negative part on the cells positive side. Would also really recommend using insulation paper rings as well. Unfortunately a little bit difficult to do at this point.
```

---
## \#64 Posted by: Risewithin Posted at: 2018-08-24T01:31:24.514Z Reads: 160

```
Cool I’ve added two more strips. I’ll go and try and round off the edge of the nickel. What do you think about adding liquid electric tape around the edges as well?
```

---
## \#65 Posted by: michaelcpg Posted at: 2018-08-24T01:49:23.487Z Reads: 168

```
No worries, again, just be careful you don't get any bits of metal that you're rounding off end up falling in between the positive and negative points and shorting something :stuck_out_tongue:

Liquid electrical tape sounds like a good idea, you'll want to leave a small gap somewhere though so that if the worst case does happen, you're not completely blocking the cells from venting
```

---
## \#66 Posted by: Risewithin Posted at: 2018-08-24T01:58:49.110Z Reads: 169

```
Cool thanks for the advice brother!
```

---
## \#67 Posted by: lrdesigns Posted at: 2018-08-24T02:06:57.434Z Reads: 177

```
Looks like you could dissipate one MILLION watts of heat with this setup! :snowflake::snowflake::snowflake::snowflake::snowflake: 
![image|641x384](upload://5zBKEyoyfdb2VBeCXVY2zYUP0aY.jpg)
```

---
## \#68 Posted by: Risewithin Posted at: 2018-08-24T02:25:11.598Z Reads: 173

```
😂😂😂😂😂 Hahahaha hopefully!!
```

---
## \#69 Posted by: Risewithin Posted at: 2018-08-25T12:02:36.293Z Reads: 172

```
Does anyone know how to get ahold of @Nowind? Tried emailing him from e-toxx.com website and on here with no response.
```

---
## \#70 Posted by: Klaerke91 Posted at: 2018-08-25T12:38:15.362Z Reads: 165

```
I talked to him yesterday by PM. Maybe he is taking some time off this weekend?
```

---
## \#71 Posted by: Risewithin Posted at: 2018-08-25T12:43:36.557Z Reads: 166

```
[quote="Klaerke91, post:70, topic:65188, full:true"]
I talked to him yesterday by PM. Maybe he is taking some time off this weekend?
[/quote]

Yeah that’s weird cause I sent him email super early at 5:32am yesterday so if  he’s talking to other people then I don’t understand why he’s not responding to me.
```

---
## \#72 Posted by: Risewithin Posted at: 2018-08-26T01:51:12.926Z Reads: 168

```
https://youtu.be/WqtQVvaw_z4

 Same issues with mine. Its very aggravating when the owner knows about these issues and still sells and ships these faulty motors around the world. After days of trying to get ahold of Bruno @AlienPowerSystem I cannot seem to get any answers. He has replied a couple times and he's tried to send me more 8072's  ( a new design) but I cannot waste anymore time on a faulty motor so I suggested the 8085 which people have had good luck with. Now theres no communication at all and Im tired of sitting here having my time wasted. Does anyone out there know how to get Bruno to respond and try to resolve this issue as fast as possible?  @Silverline @DK-Odense 
[quote="DK-Odense, post:36, topic:65188"]
@Silverline and I bought 6x 8072S - All failed :frowning:
[/quote]
```

---
## \#73 Posted by: Klaerke91 Posted at: 2018-08-26T06:33:50.723Z Reads: 162

```
seems i gonna check my new motors too :weary: :face_with_symbols_over_mouth:
```

---
## \#74 Posted by: Nowind Posted at: 2018-08-26T07:48:12.450Z Reads: 165

```
[quote="Risewithin, post:69, topic:65188"]
Does anyone know how to get ahold of @Nowind? Tried emailing him from [e-toxx.com ](http://e-toxx.com) website and on here with no response.
[/quote]


LOL
anserewed your question about 12mm Spurs on Friday.
parts are packed and going out next buisness day
now its weekend!
```

---
## \#75 Posted by: Klaerke91 Posted at: 2018-08-26T08:08:58.360Z Reads: 159

```
Are you sure that was not me you where talking too? We talked about the same thing???
```

---
## \#76 Posted by: Nowind Posted at: 2018-08-26T08:12:54.754Z Reads: 157

```
Nope

yeah you both wants the same on the same day (-;

Answered him and yours
```

---
## \#77 Posted by: Risewithin Posted at: 2018-08-26T12:34:11.693Z Reads: 155

```


[quote="Klaerke91, post:73, topic:65188"]
seems i gonna check my new motors too :weary: :face_with_symbols_over_mouth:
[/quote]
Yeah this is really aggrevating. Knowing about the issues from other members here and still selling more to other people. I mean that just shows they don’t even test these motors before they send them out. There should be some sort of QC set in place you would think.
```

---
## \#78 Posted by: Risewithin Posted at: 2018-08-27T11:48:29.546Z Reads: 157

```
Hey brother so Bruno has 8085 unsensored motors he can ship me. Will those mount to your drives? I can add encoder later?
```

---
## \#79 Posted by: Nowind Posted at: 2018-08-27T14:33:03.231Z Reads: 159

```
Yeah 8085 fits to the Mounts, no matter if sensored or unsensored.
Encoder can be used with the new 3D printed Encoder Housings.
You have the CNC machined non Encoder Mounts.
```

---
## \#80 Posted by: Risewithin Posted at: 2018-08-27T14:46:01.386Z Reads: 166

```
Ok cool so I have a buddy with a 3D printer. I just gotta download the housing files and have them printed? And aren’t you asking me if I have the mounts or that I need the mounts?
```

---
## \#81 Posted by: Nowind Posted at: 2018-08-27T14:52:06.760Z Reads: 165

```
[quote="Risewithin, post:80, topic:65188"]
I just gotta download the housing files and have them printed?
[/quote]

We not puplished any data!

[quote="Risewithin, post:80, topic:65188"]
And aren’t you asking me if I have the mounts or that I need the mounts?
[/quote]


Dont understand
```

---
## \#82 Posted by: Risewithin Posted at: 2018-08-27T15:25:07.368Z Reads: 155

```
Oh so you sell the housing and mounts for the encoders. I thought they were an open source thing. I’m very unfamiliar with how encoders work or what I need to install them.  I have not done any research just yet. Just from what I know I hear encoders are better than hall sensors and if I do not have sensors encoders are the way to go.
```

---
## \#83 Posted by: Nowind Posted at: 2018-08-27T15:29:38.625Z Reads: 155

```
Here we showed the Encoder Housing, also some questions about Encoders : 
https://www.electric-skateboard.builders/t/e-toxx-webshop-online/45039/281
```

---
## \#84 Posted by: Risewithin Posted at: 2018-08-27T16:19:12.822Z Reads: 150

```
Cool thanks brother. So do you’ll sell these kits? I don’t see them for sell anywhere?
```

---
## \#85 Posted by: Nowind Posted at: 2018-08-27T18:10:47.765Z Reads: 155

```
We actually sell them with the new Matrix2 Gearboxes.
But also we will sell for every other Drive from us.
Thats why we made them, to use the future shit AKA magnetic Encoder :laughing:
```

---
## \#86 Posted by: Risewithin Posted at: 2018-08-28T18:10:53.875Z Reads: 149

```
So how much are they if I had to buy a kit?
```

---
## \#87 Posted by: Riako Posted at: 2018-08-28T18:13:33.041Z Reads: 156

```
Just here ;) 
https://www.e-toxx-shop.com/mbs/
```

---
## \#88 Posted by: Risewithin Posted at: 2018-08-28T18:26:48.055Z Reads: 148

```
Thanks! I have direct drive already for Trampa board. Just curious about the encoders! I don’t see them listed in the site at all.
```

---
## \#89 Posted by: Riako Posted at: 2018-08-28T18:32:31.680Z Reads: 153

```
[quote="Nowind, post:85, topic:65188"]
We actually sell them with the new Matrix2 Gearboxes.
[/quote]
On the 10 x 40T now
https://www.e-toxx-shop.com/mbs/mini-gear-box-drive-mbs/1-4-helical-gear-box/#cc-m-product-10006723570
And soon on the 8 x 40T he says in the topic he link you :slight_smile: 
[quote="Nowind, post:85, topic:65188"]
But also we **will** sell for every other Drive from us.
[/quote]
If it's just the carter to move (and some wires managements) it should be easy I guess. Maybe you could start whitout and the time to finish the build they were available !?.. But I don't know ...
```

---
## \#90 Posted by: Risewithin Posted at: 2018-08-28T19:03:59.550Z Reads: 145

```
Ah I see them now. Yeah poop eventually I'll have to see about adding encoders. I just bought the etoxx 80mm direct drives. Maybe Jens can make just the cover? Idk
```

---
## \#91 Posted by: Nowind Posted at: 2018-08-28T19:21:18.980Z Reads: 147

```
No Problem you can buy them seperate.
75€ for a pair.
```

---
## \#92 Posted by: Risewithin Posted at: 2018-08-30T00:26:35.348Z Reads: 151

```
https://youtu.be/pIybFybks2Q

New light installed. Still waiting for parts. Bruno is sending new motors 8085 and will be here Friday! Should have the beast ready to roll soon. Customs taking forever to releases the drives 😤
```

---
## \#93 Posted by: Risewithin Posted at: 2018-08-31T20:35:27.482Z Reads: 143

```
![image|690x318](upload://fJ9qKtXnu7Ky1J5W5BAxCsi5t1A.jpeg)

New motors in. Already programmed and ready to go. Just needs some gears and mounts which are stuck at customs for a week now 😭😭😭
```

---
## \#94 Posted by: Silverline Posted at: 2018-08-31T21:41:37.050Z Reads: 145

```
Nice.... And the do not have stutter problems ?
```

---
## \#95 Posted by: rich Posted at: 2018-08-31T21:52:45.631Z Reads: 148

```
That are some serious motors :laughing:
```

---
## \#96 Posted by: Risewithin Posted at: 2018-08-31T22:27:55.868Z Reads: 146

```
Nope these so far seem to be really smooth!! I’ll let’s you know for sure if I can ever get the drives in and test them with weight on!
```

---
## \#97 Posted by: Silverline Posted at: 2018-08-31T22:34:08.767Z Reads: 145

```
Thanks

Are you planning to DIY hall sensor PCB on this motor ?
```

---
## \#98 Posted by: Risewithin Posted at: 2018-08-31T23:53:43.071Z Reads: 142

```
Plans are to get the encoder from @Nowind after I save up some money 💰
```

---
## \#99 Posted by: Silverline Posted at: 2018-09-01T00:01:15.533Z Reads: 145

```
Great plan 😀
```

---
## \#100 Posted by: Duffman Posted at: 2018-09-01T10:56:55.025Z Reads: 145

```
The main problem is that those AS5047P encoders are out of stock in every shop I know. 

Last info on delivery date was Jan 2019...

There seem to be some issues with the manufacturer...
```

---
## \#101 Posted by: Risewithin Posted at: 2018-09-01T12:51:07.386Z Reads: 140

```
Oh wow i guess I’ll be running sensorless for awhile lol.
```

---
## \#102 Posted by: Risewithin Posted at: 2018-09-02T16:08:20.482Z Reads: 143

```
https://youtu.be/DP_04p80cT4

Quick demo of the system working with the 8085’s.
```

---
## \#103 Posted by: Risewithin Posted at: 2018-09-07T21:17:26.645Z Reads: 136

```
![image|375x500](upload://yOTLNiDCXYCwXuXkHZrbzZoLFZB.jpeg)![image|375x500](upload://lTQCVRp0WyCbOemSazOCHUEqpnU.jpeg)

Looks like imma be busy tonight after I get off work!
```

---
## \#105 Posted by: Silverline Posted at: 2018-09-10T18:48:45.580Z Reads: 131

```
Standard chinese motor sound :-/ sounds like the APS 8072...... It could be a loose magnet.
```

---
## \#107 Posted by: Risewithin Posted at: 2018-09-16T18:16:15.874Z Reads: 131

```
https://youtu.be/fKrdkkv67X4

Ok just about all done. Still waiting for BMS  and I ordered it on August 13th. Bruno from @AlienPowerSystem instructed me through the motor noise issue and there was a loose screw on the casing. All motor noise is gone and running very well now. So even though we had some issues with the 8072 early on I can say their customer service was excellent and I'll probably order some 250kv motors in the future due to these maxing out at 30mph, yes I want to faster. The torque on these are absolutely insane and I love it! The Drives from @Nowind are top notch and working well. I highly recommend his drives as not only the quality of them were great but he's also a great guy who will take his time to answer your questions and get you on the right path. Also so far the Flipsky Fsesc's are doing great handling the 80mm motors and big battery. According to the Bluetooth app Xmatic from @twan they are running ~30 degree Celsius cruising and ~35 degree running somewhat hard.
```

---
## \#108 Posted by: Nate Posted at: 2018-09-16T18:21:39.239Z Reads: 126

```
dude, upload that raw footage! we gotta hear them motors especially if they're 80xxmm
```

---
## \#109 Posted by: Silverline Posted at: 2018-09-16T18:24:12.590Z Reads: 127

```
A loose screw ?? Where ??

Yes, we wanna hear those bastard in action :-)
```

---
## \#110 Posted by: Risewithin Posted at: 2018-09-16T18:27:14.172Z Reads: 128

```
Those little bitty screws that go around the casing of the motor. A couple were loose so it allowed the casing the vibrant at certain rpm. Slight lack of quality control but at least it was an easy fix!!
```

---
## \#111 Posted by: Risewithin Posted at: 2018-09-16T20:55:57.222Z Reads: 128

```
https://youtu.be/d8pzBjarwwM

Sound of the motors.
```

---
## \#112 Posted by: Kug3lis Posted at: 2018-09-16T21:26:52.712Z Reads: 125

```
I don't know if its worth to switch to 250kv... My experience from switching 170kv to 200kv massive torque loss I don't have anymore instant launch like I had with 170kv I get good acceleration at around 2kRPM or etc, until then its trying hard compared to 170kv. When I will by trying FatBoy SS I will be using probably 1:4 with 80100 180kv for higher speed but still have that monster torque :)
```

---
## \#113 Posted by: michaelcpg Posted at: 2018-09-17T02:12:23.659Z Reads: 121

```
What motor max/battery max have you guys got set for each ESC currently?

@Kug3lis I noticed the same thing when going from 170kv 6374 to 200kv 6384 motors as well, have also noticed my FocBoxes start thermal throttling much quicker. 

Currently I have each FocBox set to 40A battery/ 80A motor. Wondering how much much of a difference pushing the max current settings up a bit is likely to make.
```

---
## \#114 Posted by: Risewithin Posted at: 2018-09-17T04:51:28.941Z Reads: 121

```
Right now Im pushing 100A Battery, 120A Motor. Capable of 120A battery max and each motor can handle 150amp max.  Im guessing I can sacrifice some torque for speed cause theres plenty to spare here lol. I tried 200kv 6374's and they still had some good torque. Only one way to really find out. If not, I still have the 170Kv to reinstall.
```

---
## \#115 Posted by: michaelcpg Posted at: 2018-09-17T06:03:55.171Z Reads: 116

```
100A Battery/120A motor per VESC?
```

---
## \#116 Posted by: Risewithin Posted at: 2018-09-17T10:48:54.020Z Reads: 113

```
100A battery total and 120A per motor.
```

---
## \#117 Posted by: Risewithin Posted at: 2018-09-26T21:31:10.865Z Reads: 103

```
![image|375x500](upload://wF4thTMaIXcJxZOmHFoqTUoX0pt.jpeg) 

finally got the bms today!
```

---
## \#118 Posted by: banjaxxed Posted at: 2019-02-26T17:23:12.089Z Reads: 57

```
How is this running for you? Do you notice any problem with motor noise?
```

---
