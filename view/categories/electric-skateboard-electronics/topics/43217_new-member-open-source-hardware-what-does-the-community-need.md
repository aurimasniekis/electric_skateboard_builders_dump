# \[New member\] Open source hardware - what does the community need?

### Replies: 52 Views: 1688

## \#1 Posted by: AKF Posted at: 2018-01-08T20:26:22.505Z Reads: 207

```
Hi.

New member here, thought I should say hi to the community. My name is Aleksander. I'm an electrical engineer, 25 years old, and my hobby is to design electronics in my spare time. I was a part of a formula student team while I studied so I have some experience with motors and batteries (400V battery and 80KW PMSM motor).

I’m planning to design a ESC (using FOC algorithm or similar) for educational purposes. When I’m done with that I’ll probably begin with a BMS design. 

My questions are: 
1. What do you guys think would benefit the esk8 community? 
2. Anything that is lacking in the open source section? 
3. Any problems with the VESC?
4. Are there any other hardware designers / software developers on the forum?

I’m hoping to get some discussion in this thread regarding the open source hardware available for esk8. It doesn’t have to limited to ESC, but I’m going to work with ESC design first (again for educational reasons) .
```

---
## \#2 Posted by: Achmed20 Posted at: 2018-01-08T21:50:47.653Z Reads: 191

```
an alternative to the VESC probably wont hurt. 
i'm actualy more up for a **small scale** and intelligent BMS.
something combined would probably be the crown jewel in this category ;)
```

---
## \#3 Posted by: FredrikHems Posted at: 2018-01-08T21:55:27.076Z Reads: 184

```
definitely an esc Who have the same futures as a vesc, but can handle alot more amps. :smiling_imp:

Like the Vesc 6, but more affordable :sweat_smile:
```

---
## \#4 Posted by: Achmed20 Posted at: 2018-01-08T22:04:00.837Z Reads: 174

```
more then 240 amps?
OK its peak only but i have yet to see the motor that needs 50a continous. 

how about an ESC that can handle 2 motors? right now you still need 2 ESC's for that.
```

---
## \#5 Posted by: Bor.inc Posted at: 2018-01-08T22:06:10.662Z Reads: 171

```
yess thats very handy if you can make everything in one
```

---
## \#6 Posted by: fedestanco Posted at: 2018-01-08T22:06:31.402Z Reads: 170

```
Welcome to the forum. Usually when people start designing challenging electronics like a foc-esc or a smart bms (see raphaelchang) things get complicated on the software side, leading to uncompleted projects. 
Why don't you start with something simpler like a high amps switch (150amps) with directfets or a non-IC bms?
```

---
## \#7 Posted by: Bor.inc Posted at: 2018-01-08T22:10:30.329Z Reads: 166

```
Btw maybe a lipo charger like the imax b6 just on a pcb and maybe with changeble settings to adapt it to it's battery pack. 
Because, maybe I am wrong, that such a charger charges the batteries a little bit better than a bms but it is pretty anoying to plug the batteries out everytime u charge. With this pcb you can insert it in the enclosure and have a charging plug for the needed voltage

So than you have the best of both worlds, the best charging, and the user friendliness of a bms system
```

---
## \#8 Posted by: LAVAMAN Posted at: 2018-01-08T22:13:27.608Z Reads: 161

```
The largest barrier and creates the most problems is the VESC (for me included). One reason is not plug and play and the other is poor build quality. I understand that some of the folks that are very skilled in electronics like all the adjustability, but the majority of us just want to quickly set up our equipment and go ride. The FOC BOX is the closest product I have seen so far but still not plug and play enough. Should be as simple as setting up an ESC for an RC car with same reliability as say "Castle Creations" or Novak" products. If it had a BMS as part of the package would be that much better. Again, plug and play. Hook it up and pick your battery size (6-12S) and done. Another thing that would be a huge help would be a system where you can combine battery cells to make a larger battery without having to weld the cells together. I have seen some plastic battery cell holders that you just snap the cells into place and combine into a larger battery. If there was a frame that would accept cells to make between 6-12S with no welding required (just soldering connectors) anyone could do it. Maybe it could be 3D printed with some nickel inserts or something?
```

---
## \#9 Posted by: Achmed20 Posted at: 2018-01-08T22:21:05.939Z Reads: 157

```
[quote="LAVAMAN, post:8, topic:43217"]
Another thing that would be a huge help would be a system where you can combine battery cells to make a larger battery without having to weld the cells together.
[/quote]
they only reasons you dont see these things beeing used in sekates, is because those methods waste alot of space and also dont handle vibrations very well. the last thing you want on your board is failing breakes because the battery decided to have a small outage. if you need an easy method, go with lipos ;)

PS: the Focbox actualy is a VESC, it just has different components and a different formfactor. both have the same "experience"!
```

---
## \#10 Posted by: laurnts Posted at: 2018-01-08T22:22:48.483Z Reads: 157

```
Low cost FOCBOX / VESC with same performance.

I mean look, everyone here most of the chances are running FOC mode (when they can) as it's silent and doesn't catch police attention. It provides more torque anyway, so not supporting BLDC mode that doesn't matter so much. If it runs on both BLDC and FOC is the best. Yet also need to support sensored and uncensored. It's even more marvelous if the BLDC tool is much simpler. People want more voltage, more current, higher max erpm. But again if you can make simpler version of VESC with 80 euro price range, thats a hard contender for VESC. More or less soooo many people have their VESC / FOCBOX broken in away. If the fragile components is plug and play replaceable using something like this https://cdn-shop.adafruit.com/1200x900/1281-00.jpg That would make replacing broken things soo much easier.
```

---
## \#11 Posted by: Hummie Posted at: 2018-01-08T22:27:21.298Z Reads: 151

```
just make something that does foc and doesn't break!  the rest is unimportant.  vescs and focboxes break nonstop its ridiculous and at this point it seems there's almost nowhere to get one of these vesc versions other than the crazy expensive 6, the lackluster focbox, or some Chinese crap that might not even do foc.  no more ollin and it seems no more axle these days or at least theyre so backlogged they might as well be gone.  please make a simple cheap foc machine that doesn't break!  you will be rich and we will all have it
```

---
## \#12 Posted by: b264 Posted at: 2018-01-08T22:37:09.587Z Reads: 151

```
[quote="AKF, post:1, topic:43217"]
What do you guys think would benefit the esk8 community?
[/quote]

VESC 6.4 pcb designs open-sourced.  A pcb that's skinny (35mm) and long (120mm) versus square. (65mm * 65mm)  We have options for square already.  Easier to fit in tight spaces.  Also preferably a way to have two paired on the same PCB, possible able to break them apart into 2 pcbs (the canbus lines etc would just sever at the board break) if needed for single motor ESCs.  And with protected DRV and CAN chips so they aren't blowing all the time.

It'd be great to have "trapezoidal FOC" mode and "sinusoidal FOC" mode --- instead of BLDC and FOC modes
```

---
## \#13 Posted by: Deckoz Posted at: 2018-01-08T23:14:51.945Z Reads: 145

```
If I was to say anything...

Antispark that won't fail lol.
```

---
## \#14 Posted by: baxter Posted at: 2018-01-09T01:51:56.847Z Reads: 140

```
Someone should offer kits to make your own battery packs, assuming you have minimum set of tools.

Maybe offer pre spotwelded 3p or 4p packs with balance wires that can be connected modularly into a 6s or 10s configuration with a simple charge only BMS?

I would love to try and build my own pack but I don’t have the confidence (or a spot welder) to do it.  Similarly, while the process may be theoretically straightforward, I tend to be reluctant to try this sort of thing for fear of destroying or shorting cells, or it all catching on fire.

If I could buy all the compatible parts and assemble them following a set of instructions that were easy to follow (read: idiot proof) and procedurally correct (EE certified), I would be very interested. It would hopefully reduce the perceived complexity of assembly, especially where a BMS is desired for ease of charging.

One could get into the argument about the ease/ difficulty of shipping the 3 or 4p modules internationally, but depending on cost, you could potentially have a ready and waiting international market, especially when your local battery builder wants to charge you arm and a leg for a pack.
```

---
## \#15 Posted by: Cobber Posted at: 2018-01-09T02:25:33.679Z Reads: 129

```
* more powerful esc that doesn't make magic smoke

The current vesc has components rated to just over 13s voltage as I understand it. Many use it at 12s (some 13s). 10s has shown to be more reliable though so what we really need it would seem is a esc with components rated to at least 15s or 16s voltage so it is reliable at 12s. Essentially we are using our gear at its limit with little to no headroom so it brakes down often....
```

---
## \#16 Posted by: ThierryGTLTS Posted at: 2018-01-09T10:03:50.401Z Reads: 112

```
As said, battery power switch with integrated antispark would be great.

Most of the problems come from the fact that DRV and MOSFETs are voltage limited, 13S is too much if you use regenerative braking.

Yes there are other hardware designers / software developers on the forum and on the VESC forum.
```

---
## \#17 Posted by: Kug3lis Posted at: 2018-01-09T10:13:22.533Z Reads: 106

```
Thanks for reminding my project :joy:
```

---
## \#18 Posted by: Kug3lis Posted at: 2018-01-09T10:14:43.970Z Reads: 106

```
I am curiuos how good are your programming skills, because  esc most of the part is only software, electronics are easy part to design ;)
```

---
## \#19 Posted by: SimosMCmuffin Posted at: 2018-01-09T10:55:13.487Z Reads: 104

```
But good electronics design is not so easy and since your software is relying on your hardware to control your motor, if your hardware is not well done then your software's performance will also be limited by proxy.

[quote="Kug3lis, post:18, topic:43217"]
electronics are easy part to design
[/quote]

Hardware costs money, software is free. This was the saying in good days of Nokia.

I don't want to sound rude, but that comment just seems so layman to me.
```

---
## \#20 Posted by: Kug3lis Posted at: 2018-01-09T11:00:37.023Z Reads: 100

```
I am electric/software engineer I can design ESC board in a day software will take 1-3weeks. So here is an example for you why electronics are easier.

Plus the motor control is I think the easiest stuff to do because it only depends on 3 x half bridges, current sensors, voltage sensors and that's all... For e.g. I am working at the moment with a main control unit which would do like data logging, aggregation of data from multiple vesc and etc. So that board is way more complicated than ESC
```

---
## \#21 Posted by: Deckoz Posted at: 2018-01-09T12:59:05.728Z Reads: 93

```
[quote="Kug3lis, post:17, topic:43217"]
eminding my project
[/quote]

Hey

You were working in escs...and battery pack boards... Lol not antispark lol
```

---
## \#22 Posted by: Kug3lis Posted at: 2018-01-09T13:47:13.524Z Reads: 89

```
http://www.electric-skateboard.builders/t/fatboy-anti-spark-switch/38869/18
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2018-01-09T13:54:38.761Z Reads: 88

```
[quote="Kug3lis, post:18, topic:43217"]
electronics are easy part to design :wink:
[/quote]

Yeah.... It only 4 years and over dozen of people to refine the electronic on a simple VESC and even there they are only a hand full of people that could done it :wink:... as @SimosMCmuffin said  [quote="SimosMCmuffin, post:19, topic:43217"]
Hardware costs money, software is free. This was the saying in good days of Nokia.
[/quote]
```

---
## \#24 Posted by: Kug3lis Posted at: 2018-01-09T13:57:42.817Z Reads: 84

```
It was never production style project there vedder put his 100% of time into it. The whole design is from several reference designs.
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2018-01-09T14:01:04.396Z Reads: 85

```
[quote="Kug3lis, post:24, topic:43217, full:true"]
It was never production style project there vedder put his 100% of time into it. The whole design is from several reference designs.
[/quote]

So... It still took 4 year to refine the product!!! and it wasn't vedder who done it by the end... You can make easy electronic, but will they be reliable??
```

---
## \#26 Posted by: Kug3lis Posted at: 2018-01-09T14:48:34.664Z Reads: 81

```
First, look at the schematic difference between 4.12 and 6 for e.g. What was changed? Not much DRV was changed because it went obsolete so its whole sheet was changed because of new requirements for that DRV, added current sensors and etc.

I created my own VESC design without DRV in a week working for several hours in a day.

I have been doing production level electronics for over 10 years and I can say there are no easy electronics like you mentioned. It's just electronics...
```

---
## \#27 Posted by: JohnnyMeduse Posted at: 2018-01-09T15:20:32.153Z Reads: 81

```
[quote="Kug3lis, post:26, topic:43217"]
I created my own VESC design without DRV in a week working for several hours in a day.
[/quote]

So was probably the Vesc 1.0, but still it went over 4 Major hadware design revision (probably most of them had never seen the light of the day) and 12 minor change, which are simple as adding a capacitor to improve FOC ability. I have some doubts that it took one week to go all over those change. If this in one week... I’m impressed.

But truth is, making electronic circuit reliable and efficient take time and testing.

You can make a good Rye Whiskey in the backwoods with corn in a week, and It will get you drunk, but you ended up blind... And it won’t taste like a recipe that people have developed over centuries, and fermented for over dozens of year. 

[quote="Kug3lis, post:26, topic:43217"]
I have been doing production level electronics for over 10 years and I can say there are no easy electronics like you mentioned. It's just electronics...
[/quote]

And It is nice for you.

Edit: I think we are going off topic now... let get @AKF is topic back 😉
```

---
## \#28 Posted by: Blasto Posted at: 2018-01-09T16:35:15.774Z Reads: 71

```
Sadly i don't think i will ever find the time to do this so i mind as well share the idea

[quote="Achmed20, post:2, topic:43217"]
i'm actualy more up for a small scale and intelligent BMS.
[/quote]

1S4P pack PCB (other flavors can accommodate more P's) with a high power bleed circuit directly on each 1S pack (2-3W bleed). 

[PCB 4P pack example](http://www.electric-skateboard.builders/t/arch-s-build-log-kaly-nyc-build-dual-6374-focbox-12s4p/25995?u=blasto)

on each pack (slave) has a CAN bus voltage monitor/gas gauge that communicates with a master that controls the main fets.

This would make the BMS fully expandable, up to the max number of slaves on the CAN bus. Eliminates all the sense wires, only a CAN bus will run to each pack. Saves a lot of real estate on the bleed circuit. The master would also be very small, the fets & the high current path will be the biggest component on the master pcb.
```

---
## \#29 Posted by: Kug3lis Posted at: 2018-01-09T16:38:09.964Z Reads: 67

```
But it will require isolated power supply on each board :D
```

---
## \#30 Posted by: Blasto Posted at: 2018-01-09T16:41:49.008Z Reads: 68

```
i just flirted with the idea a bit, but i think it would be acceptable to run 4 wires across each pack (if you would want an external power). But most 1S gas gauges i looked at can take it's power from the 1S pack.

I'm just giving ideas... i don't have an entire solution designed
```

---
## \#31 Posted by: Kug3lis Posted at: 2018-01-09T16:42:54.531Z Reads: 69

```
I looked too, and almost went with one design which would let me to big BOOM, because that cell ground for other stuff can be not ground...
```

---
## \#32 Posted by: Kug3lis Posted at: 2018-01-09T16:43:28.704Z Reads: 68

```
P.S. Interesting idea, but I think it would be expensive and not much for this community...
```

---
## \#33 Posted by: Blasto Posted at: 2018-01-09T16:44:19.380Z Reads: 67

```
I also think it is a safe solution, no battery voltage dangling on a small gauge wire
```

---
## \#34 Posted by: AKF Posted at: 2018-01-09T17:20:09.160Z Reads: 63

```
I'm aware of that, but as i said i'm doing it for educational purposes. I want to learn more about the programming part, which is why i'm interested in the complexity. Obviously it's going to take some time to finish. I might start with something simpler.
```

---
## \#35 Posted by: LAVAMAN Posted at: 2018-01-09T17:22:17.314Z Reads: 61

```
I agree, space is an issue but design could be compact and vibration issues could be solved. My point with the FOCBOX is that the packaging and quality have been improved greatly. As far as the FOCBOX being a VESC, VESC's and ESC's are the same thing, the VESC being open source and ESC's not but both do the same thing. The new VESC tool is coming closer to plug and play and one day in the future it will be.
```

---
## \#36 Posted by: Kug3lis Posted at: 2018-01-09T17:24:45.769Z Reads: 58

```
ESC is a just short term for Electric Speed control, It has nothing to do with being a not open source. And VESC means Vedder Electric Speed Control
```

---
## \#37 Posted by: JohnnyMeduse Posted at: 2018-01-09T17:26:56.480Z Reads: 55

```
Sorry but not really (and that why there was such a fuss abouth the trademark)

VESC = Vedder Endless Sphere Controller !!!
```

---
## \#38 Posted by: Kug3lis Posted at: 2018-01-09T17:27:19.769Z Reads: 56

```
[quote="b264, post:12, topic:43217"]
VESC 6.4 pcb designs open-sourced.  A pcb that's skinny (35mm) and long (120mm) versus square. (65mm * 65mm)  We have options for square already.
[/quote]

Where are PCB design available?
```

---
## \#39 Posted by: Kug3lis Posted at: 2018-01-09T17:27:52.235Z Reads: 57

```
Oh ok, you got me with this :D I thought it s Vedder ESC
```

---
## \#40 Posted by: b264 Posted at: 2018-01-09T17:28:31.325Z Reads: 60

```
[quote="Kug3lis, post:38, topic:43217"]
Where are PCB design available?
[/quote]

They aren't
```

---
## \#41 Posted by: JohnnyMeduse Posted at: 2018-01-09T17:29:31.892Z Reads: 61

```
But I give it to you, this one was pretty hard to know, specially if you haven’t seen the original thread on Endless-Spere 😜
```

---
## \#42 Posted by: LAVAMAN Posted at: 2018-01-09T17:33:54.519Z Reads: 62

```
I thought I just said that.
```

---
## \#43 Posted by: Kug3lis Posted at: 2018-01-09T17:37:19.755Z Reads: 61

```
Oh sorry I understood incorrectly I was like what? Where? When? :D I highly doubt they will release it like 99.99% doubt.

@JohnnyMeduse I have skimmed but did not read much of it... Guess what is this

<img src="/uploads/db1493/original/3X/8/5/85608c28e4572912defdf4447c716f0cd589d850.jpg" width="666" height="500">
```

---
## \#44 Posted by: LAVAMAN Posted at: 2018-01-09T17:41:34.668Z Reads: 61

```
That is what I am talking about. Sometimes I think the big companies don't get involved because of liability issues. If they make a plug and play ESC (specifically for skateboards) and someone falls and cracks their head open, they get sued. If you crash your RC car into a wall with their ESC, no one gets hurt. If they design a kit for building a battery pack and you blow yourself up, they end up in court. I was surprised when I saw Hobbyking jumping into the eskate market.
```

---
## \#45 Posted by: SimosMCmuffin Posted at: 2018-01-09T18:12:59.331Z Reads: 58

```
There are some WIP documents available from the VESC 6 beta stage at:
http://vesc-project.com/node/247
```

---
## \#46 Posted by: MrHappy Posted at: 2018-01-09T18:17:36.508Z Reads: 56

```
What school's Formula team were you on? Im at IIT Currently
```

---
## \#47 Posted by: Kug3lis Posted at: 2018-01-09T18:18:54.734Z Reads: 54

```
It's nothing new, and like I said I doubt he will ever release ;)
```

---
## \#48 Posted by: florensvb Posted at: 2018-01-09T18:21:59.060Z Reads: 53

```
Hey! 
I would love it if there was a BMS just like the ones from Bestech, but also  
- be able to adjust the input voltage from 6s to 12s
- has a built in e-switch
and most importantly
- is smaller than the bestech ones.
Limiting the size will make it harder to handle the current- but thats the challenge i guess, right? :smiley:

what do you guys think?
```

---
## \#49 Posted by: AKF Posted at: 2018-01-09T18:28:17.487Z Reads: 51

```
I have experience with automation theory and programming microcontrollers, but i'm far from a excellent programmer. I Intend to improve on that, which is one of the reasons that i want to design a ESC.
```

---
## \#50 Posted by: Achmed20 Posted at: 2018-01-09T18:28:18.497Z Reads: 54

```
[quote="LAVAMAN, post:35, topic:43217"]
As far as the FOCBOX being a VESC, VESC's and ESC's are the same thing
[/quote]
i think you got something wrong there. the Focbox IS a VESC 4.12 and those RC car ESC's are playing in an completly different (lower) league. 
same goes for the chinese  ESCs which (i think) are plug and play. but those are usualy nothing a DIYer wants to play with because ther is nothing to tweak.
```

---
## \#51 Posted by: AKF Posted at: 2018-01-09T18:54:19.529Z Reads: 49

```
Can't say i completely agree with that. The time it will take to design something is obviously dependent on previous experience with similar systems and whether or not you have access to previous work that you can "borrow" from, but that is a discussion for another thread :P . On the other hand, I do agree with you that the software part of an ESC is the most demanding. 

Do you have any ESC designs (or other electronics projects for that matter) that are publicly available? I would be very interested to look at the schematics/layout :)
```

---
## \#52 Posted by: LAVAMAN Posted at: 2018-01-09T23:12:03.025Z Reads: 44

```
I understand that. I was just saying that I felt the VOCBOX is an improvement over standard VESC in overall quality and design (packaging). VESC and ESC are the same except VESC is able to handle larger loads and batteries. ESC manufactures (Castle Creations, Novak) design their products for small light R.C. vehicles and VESC is designed to carry human on skateboard. Both provide the same function. I said previously that some DIY'ers will want all of the adjustability but many (like myself) want more plug and play. I think the proper design and interface can provide both, basic setup for me and advanced user adjustability for you, all in the same package.
```

---
