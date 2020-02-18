# \[WIKI\] A beginner guide to DIY an ESK8

### Replies: 196 Views: 64597

## \#1 Posted by: e.board_solutions Posted at: 2018-02-19T15:34:47.140Z Reads: 3970

```
------------------------------------------------------------
This is a work in progress, got some things to add? Let it know!

-----------------------------------------------------------



**_A beginner guide to DIY an ESK8_**

_So you want to build your own electric skateboard but don’t know where or how to start? No worry this guide will cover the basics of DIY’ing your ESK8. If you want more in-depth guides about some particular subjects, use the search function of the forum. You will find what you're looking for!_

Some more blog posts you can find [here](https://electricboardsolutions.com/).

_Very short:_

The 3 big components are the motor, the ESC and the battery
•	The motor gives the mechanical power to your wheels
•	The ESC (electric speed controller) is the brain of your eks8, it controls the motor using the electric power from the batteries
•	The batteries give the electric power needed for your motor

![image|570x202](upload://lD68ctYqry8FYCdeFXntIFqDGvf.jpg)
 
[Picture source](https://vesc-project.com/node/180)

_Overview_

1.	Motor & motor types
a.	kV, Watt & dimensions
b.	Unsensored & sensored motors
c.	Hub motor
2.	Mechanical parts for belt drivetrain
a.	Pulleys & belts
b.	Mounts
c.	Wheels
3.	ESC
a.	ESC
b.	VESC®
4.	Battery
a.	Voltage, amps, Ah, C-rating
b.	Serie & parallel, SP
c.	Charging (balance) & BMS
d.	Switch & fuse
5.	Remote
6.	Enclosure
7. Deck
8. Interesting articles




**1. Motors and motor types**

 ![image|168x167](upload://4GjebJ5mluZEzYm86FHq3bXJoEU.jpg)
_a. Kv, Watt &dimensions_

•	Kv or RPM/V or (Rounds per minute)/applied volt is a unit to tell how fast a motor will spin depending on the applied voltage.
•	Watt [W] is the unit for power, mostly for esk8 motors this will vary between 500W to 3500W per motor. 1HP is 736W, so the strongest motors can go up to almost 5HP (!)
•	The motors dimensions are given by diameter and length. For example a 6355 motor has 63mmØ and 55mm length.

_b. Unsensored & sensored motor_

Most motors have just 3 wires, unsensored motors
![image|141x115](upload://9Ja1B5nKoIeFwAzG6iL0FzXfAfE.jpg)
 
The sensored motors are a bit more expensive and have a fourth cable the “sensor cable”. This sensor cable detects the position of the rotor. That is why sensored motors are better for smooth startup and helps the ESC to be more efficient. 
![image|171x110](upload://qzkjKwqSmoF7PNv3chTTIr6FpyC.jpg)

 

_c. Hub motor_

The latest upcoming trend in ESK8 technology are the hub motors, these motors are built in your esk8 wheel. 
![image|200x165](upload://kyYwyDLsELd6MiTkGk42NjNgLQj.jpg)
 

**2. Mechanical parts for belt drivetrain** _( a great in depth guide about electric skatboard drivetrains you can find [here](https://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53) by @onloop)_

_a. Pulleys and belts_
 ![image|163x185](upload://fYAHeSkPTZvnkYY1pXG0xlyyvn8.jpg)
Most used is the HTD profile with a pitch of 5mm. You will need a pulley for the motor and a pulley for the wheel and a belt to connect them.
There are different ways to connect the pulleys to the wheel/motor.

The motor pulley is mostly fixed to the motor axle with adjustment screws or a key & keyway. Always check the motor axle diameter and the pulley bore diameter! Most common 6/8/10mm.
![image|200x200](upload://ljQQUDugYmr2WV0kekgk8z0Y0iv.jpg)![image|200x200](upload://xT3Ktx5AqgJsfsnIJmT0eoOVoEd.jpg)

The wheel pulley can be fixed to the wheel with screws or kept in place with a bearing and coupler (you will need an adjusted truck).
![image|281x154](upload://jof9lrXi131XNwU0rh215r8eHoi.jpg)![image|131x174](upload://9oDsdBekK4BC1YWzljGQI505oc5.jpg)
 

   


_b. Mounts_

Mounts are used to fix the motor to the truck, most used systems are:

Caliber trucks in combination with this clampmount:
![image|285x144](upload://2oMEqLI9ejO12x7c6vaB99cr96W.jpg)![image|320x240](upload://ApkcRtLqr2bnou1zrm4QIqzRRRB.jpg)
  
Or

Special designed truck for esk8
![image|152x150](upload://sWe3fKI82vvXkcG4k3kX5stCK2E.jpg)![image|200x138](upload://pFbm2Ofln6nPfXutOMGMWH5Frjy.jpg)
    

_c. Wheels_
Mostly used wheels are flywheel clones, because they cheaper and have holes in the core.
![image|119x119](upload://mnu0e7zoUC1zSmI9XyPj9uQLjQp.jpg)
  
Other common used wheels are the abec flywheels or orangatang kegel wheels.
![image|210x100](upload://ywQVQZtYKkHWcHE5qTFono8azKL.jpg)
 
In fact you can use any wheel if you’re whiling to drill holes in it 😉

**3. ESC**

_a.  ESC_

ESC or electric speed controller is the brain from you esk8 and controls the motor. The ESC’s used for esk8’s are mostly RC car ESC’s e.g. Hobbyking X-car 120A, the RC car ESC’s can be used for budget builds.
Two important parameters you should check when looking for an ESC are; the number of cells in serie (s) (look further at point 4. Batteries) and the rated Amperage [A].
For example: https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html, the hobbyking X-car ESC is rated for 120A and 3-6s (serie cels) LiPo.
For your build you will be looking for at least 6s ESC’s & batteries.

_b. VESC®_

A very famous ESC, that is specially designed for electric vehicles like electric skateboards is the VESC®. The VESC® designed by Benjamin Vedder, an engineer from Sweden.
A VESC® allows very smooth startup/braking and silent motors. It also gives the opportunity to change a lot of parameters, like max Amp, voltage cut off, overheat,…

You will find a lot very good in depth guides about the VESC on this formum, just use the search function. A great youtube video you can find[ here](https://www.youtube.com/watch?time_continue=775&v=v1glLDO-EjA).

**Attention:** One known Issue that some people have with their VESC compatible ESCs is that when you roll down hill faster than your boards electric top speed, brakes become unpredictable. It might happen that when trying to apply light brakes, The ESC will do a full brake instead.

**4. Batteries** _(A great in depth guide about batteries you can find [here](https://www.electric-skateboard.builders/t/new-user-looking-for-battery-read-this-complete-walkthrough-of-batteries/26010) by @evoheyax , about C-rating [here](https://www.electric-skateboard.builders/t/what-is-battery-c-rating-is-it-important-for-electric-skateboards/36) by @onloop & about terminology and formulae [here](https://www.electric-skateboard.builders/t/the-terminology-formulae-and-physical-assembly-of-lipo-batteries-or-wtf-does-c-mean/33162) by @Clonkex )_
![image|163x163](upload://p2OQV0trxIFhTVOOKRdyJnYkEsK.jpg) ![image|188x176](upload://boBblRRaWt2tAvexEEHPemEY7wS.jpg)  
Li-ion cell			                  LiPo cell

_a. Voltage, amps, c-rating, Ah_
A battery consists of a certain number of cells placed in series or parallel (look below).

Each cell has a voltage window where it should stay in all the time!
For LiPo commonly used numbers: 3.2V/cell(completely discharged)-4.2V/cell(completely charged)
For Li-Ion commonly used numbers: 2.7V/cell(completely discharged)-4.2V/cell(completely charged)
The capacity (how far you will be skating with your battery) is given in Ah or mAh. The number of amperes a battery can give for an hour. For example, a 5Ah batterie can give 5Amps for the time of 1 hour or 20amps for 15 minutes etc… Another commonly used unit for batteries is Wh or (V*A)h or power it can give for one hour.
A battery that’s being used will give current, the unit is amperes [A], the max current a battery can deliver is based on the C-rating. A higher c-rating means higher price. Li-ion will be around 5-8C, Lipo’s can go up to 20-40C (!). To know the max continuous discharge current multiply the C-rating by the capacity. For example, a 5Ah(5000mAh) LiPo battery with a 20C rating can give 100amperes(!) continuous discharge.

_b. Serie & parallel SP_

Battery cells can be placed in series or parallel
![image|350x175](upload://4i39bryqClXefOKPTMOncFYbkMc.png)

 

The abbreviation for series and parallel is S and P.
For example a batter pack that says 8s4p means 8cells in series and 4 in parallel meaning there are 32 cells in the pack.
Batteries in esk8’s commonly have 6-12s (cells in serie) and depending on using lipo or lion 1-4p (cells in parallel). The capacity varies between 5Ah to 10Ah.

_c. Charging & BMS_

When charging a battery it’s very important that all the cells stay at the same voltage and never go higher than 4.2V/cell. To do that you will need a balance charger or a BMS (battery management system). The balance charger needs to know which voltage each cell has to be able to “balance” each cell equally, that’s why the most battery packs have a balance wire (look bellow). The bigger wires are for charging and discharging, they are thicker because they need to conduct more current.
![image|226x169](upload://38dDU7WyZ6OK6dLzbiO83DWwp6L.jpg)   ![image|213x158](upload://kq56lpEFIOUYz7GSNxboY64dSiV.jpg)
This is a balance charger, mostly used to charge LiPo’s:
![image|229x170](upload://eHgIEyWAuxBEq1sOtljvOYKgHmF.jpg)
 
A battery management system or BMS is a PCB (printed circuit board) that can be placed in your board with your batteries which allows you to charge your batteries with a laptop like charger without taking them out. 
![image|196x163](upload://p82aWVRfEooO2jVIsvg7TvTdt8x.jpg)
 
_d. Switch and fuse_

To protect yourself and your batteries it’s suggested to use a switch or fuse or both.
The cheapest switch is a loop key
![image|156x125](upload://18vuxyNDQB3yZHsewg2Cwgp91b9.jpg)![image|211x118](upload://nnEdvkwdDFQT1HEvFtBQpIfQUMJ.jpg)![image|210x123](upload://3PONmMgFe4SYa5XJ1KC30JsX4Rm.jpg)

     
**5. Remote**

Ofcourse you need to control your esk8, that’s why you will need a remote, there are several options. From RC car remotes to Bluetooth app’s to specially designed esk8 remotes.

Hobbyking GT2B			Maytech esk8 remote
  ![image|228x167](upload://sfbDDchkGbI1nX4wfOUxq8ed4Rl.jpg) ![image|239x153](upload://mVPYeTvn0rJ0SajlUg2gXyCEOlA.jpg)

**6. Enclosure**

To safely store your electronics under your board you’re egoing to need a case. For this there are several options. You can use a bread box, design and 3D print your enclosure, make it from wood, make it from metal or buy a thermoformed enclosure.
![image|148x111](upload://yJJcixmeGhzoLuxkAME1YdEKlyt.jpg)


**7. Deck** _(a great in depth guide about decks you can find [here](https://www.electric-skateboard.builders/t/what-deck-is-best-for-building-your-own-electric-skateboard/30) by @onloop)_ 

_some short general deck info_

**8. Interesting articles**

[Are DIY Electric Skateboards Cheaper? | The False Economy by](https://www.electric-skateboard.builders/t/are-diy-electric-skateboards-cheaper-the-false-economy/165) @onloop
```

---
## \#2 Posted by: e.board_solutions Posted at: 2018-02-19T15:52:39.166Z Reads: 2660

```
@danyCRO @corneel-GBOY
```

---
## \#3 Posted by: laurnts Posted at: 2018-02-19T15:58:40.576Z Reads: 2601

```
We need to pin this post to the top. Very helpful to get newbies started without making and or asking new questions that have been answered multiple times.

I believe that today its thousand times cheaper and easier to make eboard with many high quality parts and suppliers around the world. However the basic knowledge is not well known enough just yet. This is a great starting point. Thunbs up!
```

---
## \#4 Posted by: e.board_solutions Posted at: 2018-02-19T16:29:19.109Z Reads: 2479

```
Thanks :slight_smile:
```

---
## \#5 Posted by: anorak234 Posted at: 2018-02-19T16:52:41.339Z Reads: 2317

```

```

---
## \#6 Posted by: Blitz Posted at: 2018-02-19T17:15:50.511Z Reads: 2264

```
Great Guide dude wish This was here when i started.

You could talk a bit more about the pulley and how it will fix onto your motor
Had a hard time figuring that one out :joy:
```

---
## \#7 Posted by: E1Allen Posted at: 2018-02-19T17:28:32.065Z Reads: 2055

```
The build guide thread has so much good information.  I'd refer people there to get ideas from what others have done.  Shows what worked and what maybe didn't work.  Also could remind about the search function which works great on this forum.
```

---
## \#8 Posted by: squishy654 Posted at: 2018-02-19T18:15:52.965Z Reads: 1906

```
Brilliant thread!

I'd like to see more detail in just how the vesc functions or differs from a traditional brushless esc.

Also needs a skateboarding basics section based on the eskate demographic. Gaps exist in traditional skateboarding setup and safety knowledge. Things like deck purposes, truck types, angles, wheelbase, bushings and wheel types..
```

---
## \#9 Posted by: ZackoryCramer Posted at: 2018-02-19T18:28:10.382Z Reads: 1744

```
I think you need to emphasize that rearranging batteries in series or parallel doesn't give you more range.
```

---
## \#10 Posted by: laurnts Posted at: 2018-02-19T18:32:16.565Z Reads: 1691

```
The whole idea of this forum is actually this post. Niw its being used more often as build perfection, parts sourcing and abit of show off. So this post put this forum and answers all of the questions I wonder when I started my journey as a builder few years back.

Off course there should be do's and dont's with tips and tricks following post, but this should give newbies excellent start.
```

---
## \#11 Posted by: e.board_solutions Posted at: 2018-02-19T18:56:27.958Z Reads: 1558

```
@laurnts @ZackoryCramer @squishy654 @E1Allen @Blitz

I will make some changes soon :)
```

---
## \#12 Posted by: Jammeslu Posted at: 2018-02-19T18:58:50.379Z Reads: 1508

```
Finally someone made this. In addition many noobs asks if this fits to this component and if that is compatible with this etc. 

So try to get a note on compatability and what to look for
```

---
## \#13 Posted by: A-lone-tenno Posted at: 2018-02-19T19:21:38.187Z Reads: 1441

```
another thing is vesc settings and remote connections, that's something that a lot of newbs have trouble with (having trouble now)
```

---
## \#14 Posted by: e.board_solutions Posted at: 2018-02-19T19:23:51.130Z Reads: 1418

```
I think there are some good in depth guides/post about vesc settings on this forum :slight_smile:
```

---
## \#15 Posted by: E1Allen Posted at: 2018-02-19T19:26:30.144Z Reads: 1450

```
Also there is an hour long video on YouTube for vesc settings...  This could probably be updated. And shortened🤔

https://youtu.be/5HLZaMcYRuY
```

---
## \#16 Posted by: Blitz Posted at: 2018-02-19T20:31:25.931Z Reads: 1384

```
20min video that is updated to new User friendly program.

https://www.youtube.com/watch?v=v1glLDO-EjA
```

---
## \#17 Posted by: E1Allen Posted at: 2018-02-19T20:52:37.105Z Reads: 1274

```
🙄 wish I woulda watched that one
```

---
## \#18 Posted by: Blitz Posted at: 2018-02-19T21:00:36.942Z Reads: 1273

```
I spent hours watching and reading how to configure the vesc :joy: 
When I saw this new Program and tutorial and how easy a firmware updates etc are I was Both sad and happy.
```

---
## \#19 Posted by: Yecrtz Posted at: 2018-02-19T21:56:51.794Z Reads: 1245

```
Awesome guide! Very informative and will for sure help decrease the amount of topics with starter questions.
```

---
## \#20 Posted by: Clonkex Posted at: 2018-02-19T22:05:56.315Z Reads: 1237

```
I've been wanting to write a guide like this to supplement my [guide to understanding batteries](http://www.electric-skateboard.builders/t/the-terminology-formulae-and-physical-assembly-of-lipo-batteries-or-wtf-does-c-mean/33162) but I haven't had the time so far. Thanks for doing it for me! :P
```

---
## \#21 Posted by: thisguyhere Posted at: 2018-02-19T23:09:21.536Z Reads: 1108

```
changing this to a wiki will allow community contributions. but you'd be opening it up for everyone to edit.
```

---
## \#22 Posted by: Jc06505n Posted at: 2018-02-19T23:38:26.556Z Reads: 1076

```
Is there not a way to set the wiki restrictions to levels ?
```

---
## \#23 Posted by: E1Allen Posted at: 2018-02-20T00:13:05.035Z Reads: 1074

```
Well I'm not sure how many people take the time to screw up a wiki page on purpose. 
  Honestly it doesn't matter what forum you go on you're going to get the same "dumb" questions over and over even if search was used.  Sure it's a pain sometimes but this sport is changing fast. What was the new hotness a few months ago might be old and busted by the time a new member searches(or doesn't) something.

Don't forget this

http://calc.esk8.today/advanced/

Very accurate if used correctly.  I use about 88% efficiency on dual.  Maybe someone has better numbers for single
```

---
## \#24 Posted by: e.board_solutions Posted at: 2018-02-20T08:38:15.816Z Reads: 968

```
How do I make the post into a wiki?
```

---
## \#26 Posted by: laurnts Posted at: 2018-02-20T09:33:54.380Z Reads: 993

```
This is a forum builder, a wiki would require a separate website framework. I don't think its necessary. This is enough to cover the ground basic concept. More or less people only need to know about which motor to pick, which battery to pick, which esc to pick, the necessary components needed and how everything is assembled. For people who build RC this is a no brainer, since I wasnt at the beginning knowing the overview scope make huge difference.

The details, shops and gimmicks are secondary thing. Its within members in their own time to make their builds better. But knowing how simple esk8 is, is the most important value.
```

---
## \#27 Posted by: b264 Posted at: 2018-02-20T09:44:49.661Z Reads: 929

```
Turning a forum into a wiki is as easy as giving admin access to every account.  :rofl: LoL
```

---
## \#28 Posted by: Jebe Posted at: 2018-02-20T11:59:59.943Z Reads: 907

```
Great work! Maybe add, measure twice, cut once. In that order.
```

---
## \#29 Posted by: e.board_solutions Posted at: 2018-02-20T13:34:09.285Z Reads: 928

```
[quote="Jebe, post:28, topic:46844, full:true"]
Great work! Maybe add, measure twice, cut once. In that order.
[/quote]

Measure twice, cut once?
```

---
## \#30 Posted by: thisguyhere Posted at: 2018-02-20T16:56:01.077Z Reads: 919

```
https://meta.discourse.org/t/what-is-a-wiki-post/30801
```

---
## \#31 Posted by: Bor.inc Posted at: 2018-02-20T17:49:50.025Z Reads: 868

```
Maybe you can add some links from posts that go deeper in a specific topic like motor, esc and battery. So someone can read this post and can learn more about a certain topic in another threat.
Great post btw!
```

---
## \#32 Posted by: e.board_solutions Posted at: 2018-02-20T18:57:44.916Z Reads: 836

```
I'm not an admin or level 3 :confused: Maybe one of the moderators could change it to a wiki?
```

---
## \#33 Posted by: e.board_solutions Posted at: 2018-02-20T18:59:46.014Z Reads: 843

```
Yes that's a very good idea, I already linked the video about the vesc that someone posted above :) Send me some links from good posts you know so I can add them.
```

---
## \#34 Posted by: Bor.inc Posted at: 2018-02-20T19:18:11.802Z Reads: 865

```
Yeah good idea, here are some:

A realy good one about batteries @evoheyax
 https://www.electric-skateboard.builders/t/new-user-looking-for-battery-read-this-complete-walkthrough-of-batteries/26010

Here are some from @onloop:
Deck https://www.electric-skateboard.builders/t/what-deck-is-best-for-building-your-own-electric-skateboard/30
diy drivetrain https://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53
the costs of building your own eskate https://www.electric-skateboard.builders/t/are-diy-electric-skateboards-cheaper-the-false-economy/165
C rating https://www.electric-skateboard.builders/t/what-is-battery-c-rating-is-it-important-for-electric-skateboards/36

This is just a quick search, there are probably more good threads! :slight_smile:
```

---
## \#35 Posted by: e.board_solutions Posted at: 2018-02-20T19:42:03.217Z Reads: 798

```
Added! :slight_smile:
```

---
## \#36 Posted by: Jebe Posted at: 2018-02-21T05:41:41.062Z Reads: 783

```
Cut drill hack whatever you're doing once its done its done. So yeah, measure twice, before drilling cutting hacking etc
```

---
## \#37 Posted by: nmagz3 Posted at: 2018-02-26T20:38:27.348Z Reads: 766

```
Hey brotha, this is great!  I think if a noob reads through this they'll get a great perspective of what's involved in a build.  What' I'm finding lately is people asking of soldering is involved or any manipulation to the parts they purchase.  I think if a perspective builder is shying away from soldering and some tinkering, to make sure their parts work in concert, then maybe DIY isn't for them.  That could be a disclaimer or preface you might want to add.  When a noob sees the sum of these parts some individuals think its plug and play  Either way, this write up is super valuable to the community.  Awesome contribution!
```

---
## \#38 Posted by: Sampreston Posted at: 2018-02-27T05:05:54.626Z Reads: 718

```
Thank you! This was a great place for me to start! Short, concise and informative!
```

---
## \#39 Posted by: teamgee_official Posted at: 2018-03-18T16:15:31.472Z Reads: 707

```
very informative, i will come often and learn!
```

---
## \#40 Posted by: wshepherd Posted at: 2018-03-22T11:06:13.626Z Reads: 781

```
Im doing a college project and decided to make a Normal skateboard electric. I have no idea what I am doing so will someone please help me out? 

So far im looking at buying Turnigy Heavy Duty 4000mAh 6S 60C Lipoly Battery Pack from Hobbycraft, Link Below:
https://hobbyking.com/en_us/turnigy-heavy-duty-4000mah-6s-60c-lipoly-battery-pack.html?countrycode=GB&utm_source=bing&utm_medium=cpc&utm_campaign=UK+All+shopping+products&utm_term=4581252637403622&utm_content=Ad+group+%231&gclid=CID0zonW_9kCFViChQodZ98ABQ&gclsrc=ds&___store=en_us

Im also looking at the 
Turnigy Aerodrive SK3 - 6364-190KV Brushless Outrunner Motor, link below: 
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html?countrycode=GB&gclid=EAIaIQobChMI9qKS19b_2QIVwjobCh2agAv_EAQYAiABEgI2yvD_BwE&gclsrc=aw.ds

Please will anyone advise me if these are good, will they work? What ESC should I be using, pulley system drivetrain? I need all the help I can get. 


Cheers
```

---
## \#41 Posted by: e.board_solutions Posted at: 2018-03-22T11:07:38.377Z Reads: 742

```
Did you read the guide? Where are you from? Motor is good, battery can be cheaper (20c is more than enough)
```

---
## \#42 Posted by: wshepherd Posted at: 2018-03-22T11:08:42.911Z Reads: 700

```
I have been reading http://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53

I am based in the UK
```

---
## \#43 Posted by: e.board_solutions Posted at: 2018-03-22T11:09:20.619Z Reads: 684

```
You can send me a DM, I got some used parts you could use to save money :slight_smile:
```

---
## \#44 Posted by: wshepherd Posted at: 2018-03-22T11:10:56.861Z Reads: 674

```
How do I DM you? Never used that feature before? :)
```

---
## \#45 Posted by: nske Posted at: 2018-03-22T21:34:55.558Z Reads: 668

```
Click on the name, which will take you [here](http://www.electric-skateboard.builders/u/e.board_solutions) and then click **message**
```

---
## \#46 Posted by: MonkeyFist Posted at: 2018-03-23T12:39:56.929Z Reads: 653

```
Could it be that you mean PM?
```

---
## \#47 Posted by: e.board_solutions Posted at: 2018-03-23T12:55:28.105Z Reads: 649

```
PM , DM it's the same right? Personal Message, Direct Message ;)
```

---
## \#48 Posted by: Namasaki Posted at: 2018-03-31T12:57:49.303Z Reads: 612

```

```

---
## \#49 Posted by: onloop Posted at: 2018-04-04T09:58:43.071Z Reads: 628

```
I made this a wiki, it means anyone can edit the OP.... let's see how this idea goes, if people mistreat it ill remove wiki mode.
```

---
## \#50 Posted by: Khadram123 Posted at: 2018-04-05T07:18:30.443Z Reads: 613

```
This is a great guide! Though can anyone direct me to other guides that talk about ADC control or anywhere where I can get information on how to add a potentiometer to my VESC. I know how to plug it in the controller, I don't know how to program it. Any help or guidelines would be great! Thanks!!
```

---
## \#51 Posted by: e.board_solutions Posted at: 2018-04-05T07:24:52.618Z Reads: 588

```
If you can find a more info, you can place the link in the wiki ;)
```

---
## \#52 Posted by: Khadram123 Posted at: 2018-04-05T07:26:48.635Z Reads: 571

```
Will definitely do so! Once I find the information. I have been racking the forums for anything similar to that and I know I might not be the only one! :slight_smile:
```

---
## \#53 Posted by: e.board_solutions Posted at: 2018-04-05T07:32:09.137Z Reads: 544

```
For specific things you might be the first ;)
```

---
## \#54 Posted by: Khadram123 Posted at: 2018-04-05T07:49:45.035Z Reads: 548

```
Seems like it! Would you know where I can learn more about how to program with ADC control or something like that of the sort? Anything would help!
```

---
## \#55 Posted by: e.board_solutions Posted at: 2018-04-05T07:51:50.606Z Reads: 533

```
Start a topic about it ;)
```

---
## \#56 Posted by: Khadram123 Posted at: 2018-04-05T08:03:34.441Z Reads: 512

```
Sorry being insistent...but how do you start a forum topic? Thanks!!
```

---
## \#57 Posted by: L3chef Posted at: 2018-04-05T08:04:31.860Z Reads: 508

```
You need to read for an 0.5  hours before you can create topics
```

---
## \#59 Posted by: Khadram123 Posted at: 2018-04-05T08:18:37.696Z Reads: 508

```
Ohhhh! Alrighty then! Thanks!!!!
```

---
## \#60 Posted by: Jasper1 Posted at: 2018-04-11T05:42:14.833Z Reads: 495

```
So how can I get more range with two10s5p batterys?. other than installing a bigger battery
```

---
## \#61 Posted by: e.board_solutions Posted at: 2018-04-11T06:11:13.284Z Reads: 504

```
batteries with higher capacity. What also can help is put less stress on the batteries, limit the amps to 15amp or something :slight_smile:
```

---
## \#62 Posted by: leo.matis Posted at: 2018-04-11T12:36:56.257Z Reads: 524

```
Hi everyone,

New to this forum trying understand everything better. Not sure if I should write this here but I couldn't find how I open a new topic.

I am a MA student of design innovation and I chose for my major project to build an electric skateboard. I created a quick multiple choice questionnaire that takes only 1-2', to get some feedback of what people like.

I would much appreciate it if you can take a couple of minutes and fill it up, It will help me a lot.

Here's the link https://goo.gl/KVwp5y

Cheers
Leo
```

---
## \#63 Posted by: TarzanHBK Posted at: 2018-04-11T12:46:11.728Z Reads: 475

```
Just filled out the form. Your points sometimes goes hand in hand or don´t affect each other.
More range or topspeed? Bigger battery and you achieve both with more power and more range.
Better question would be topspeed vs. torque to see how people like it geared. Although a good setup has both ;)
```

---
## \#64 Posted by: MyCampGround Posted at: 2018-04-11T12:52:22.199Z Reads: 462

```
i filled it out as well but i left some of the answers blank as @TarzanHBK pointed out the problem with some of the questions.
```

---
## \#65 Posted by: leo.matis Posted at: 2018-04-11T13:01:28.453Z Reads: 478

```
Thank you guys! I will correct these questions!
```

---
## \#66 Posted by: Jebe Posted at: 2018-04-15T10:09:11.118Z Reads: 487

```
Should link to the rise and risk of electric skateboarding clip session error. And talk about safety, helmets at least. Highlight that this is dangerous and can be fatal.
https://youtu.be/bVZz8EN_NKw
```

---
## \#67 Posted by: e.board_solutions Posted at: 2018-04-15T12:28:19.768Z Reads: 461

```
Uhu, it's a wiki so you should be able to make some changes :slight_smile:
```

---
## \#68 Posted by: Belal Posted at: 2018-04-16T08:33:49.770Z Reads: 445

```
Can I use this motor
 Turnigy G25 Brushless Outrunner 710kv?
```

---
## \#69 Posted by: lowGuido Posted at: 2018-04-16T08:34:33.969Z Reads: 442

```
KV is a little too high on that motor.
```

---
## \#70 Posted by: DeathCookies Posted at: 2018-04-18T13:43:20.558Z Reads: 435

```
With the correct reduction, sure...
```

---
## \#71 Posted by: Blitz Posted at: 2018-04-18T14:06:28.315Z Reads: 439

```
Lets not forget that. high RPM and ERPM and make things more complicated.
```

---
## \#72 Posted by: Eric1565 Posted at: 2018-04-19T23:47:58.267Z Reads: 428

```
Are there any programable BMS's around that are not too expensive? :grinning:
```

---
## \#73 Posted by: TdeBeer Posted at: 2018-04-21T02:33:28.518Z Reads: 426

```
Hey there guys.

I've been wanting to build my own electric longboard. But have no idea where to start or how to start.
I would like to have hub wheels instead of a belt driven motor. I also would like it to have a top speed of about 25mph and have power to get up hills with ease. My budget is about 600USD.

Can anyone lead me into the right direction as to what parts I should get, How to build it etc.

Thanks
```

---
## \#74 Posted by: e.board_solutions Posted at: 2018-04-21T07:05:54.677Z Reads: 404

```
Where are you from? If you want to rock uphill, I think it's better you get belt drive :slight_smile:

grtz
```

---
## \#75 Posted by: MysticalUnicorn Posted at: 2018-04-21T09:39:21.976Z Reads: 427

```
Hey there, sorry I couldn't wait 17 hours so made another account.

Also any recommendations as to what companies I could get my parts from and what to stay away from?

I've decided on a 190KV Motor (Don't know which brand yet)
Also decided on 83mm Wheels ( Also don't know which brand)
And a 12S2P Battery pack ( Again, don't know which brand)
Also what ESC would you recommend?
What drive Pulley would you recommend?
What Wheel Pulley would you recommend?
What size belt?

I'd like to have a top speed of 45km/h so what size pulleys and belt will I need?

Really appreciate a quick response.

Thanks.
```

---
## \#76 Posted by: MysticalUnicorn Posted at: 2018-04-21T09:40:01.278Z Reads: 392

```
From South Africa. Where i'm from, we have a lot of potholes and cracks and sometimes the hills can be a bit steep.
```

---
## \#77 Posted by: MysticalUnicorn Posted at: 2018-04-21T09:40:49.400Z Reads: 388

```
Sorry, also what trucks would you recommend?
```

---
## \#78 Posted by: e.board_solutions Posted at: 2018-04-21T09:44:45.326Z Reads: 404

```
Their are a lot of good suppliers in the US and EU, but for Africa I don't know :/
```

---
## \#79 Posted by: MysticalUnicorn Posted at: 2018-04-21T09:45:29.729Z Reads: 426

```
I dont need suppliers in Africa as I fly alot. 

But could you recommend some parts to me and pulley sizes and belt sizes and truck sizes etc?
```

---
## \#80 Posted by: e.board_solutions Posted at: 2018-04-21T09:48:16.235Z Reads: 413

```
yes, DM me, I'm in Belgium EU :slight_smile:
```

---
## \#81 Posted by: MysticalUnicorn Posted at: 2018-04-21T09:51:27.441Z Reads: 412

```
How do I DM you.
```

---
## \#82 Posted by: MysticalUnicorn Posted at: 2018-04-21T09:53:20.118Z Reads: 422

```
I messaged E.board solutions on messenger?
```

---
## \#83 Posted by: Blitz Posted at: 2018-04-21T09:53:50.809Z Reads: 405

```
Step 1, Click on @e.board_solutions
step 2 click message on the top right corner if you go to his page.

Or click on his name and you will see blue message box from the pop up.
```

---
## \#84 Posted by: locomotor Posted at: 2018-04-22T17:07:31.908Z Reads: 421

```
Hello,

Does anyone have experience with the 90mm Maytech hub motors as well as the DIYeboard 90mm hub motors?
Is one appreciably better in terms of performance or durability than the other?

Thanks!
```

---
## \#85 Posted by: meesie Posted at: 2018-04-24T14:07:29.577Z Reads: 401

```
i'm missing a "6.1 mounting your enclosure"!
```

---
## \#86 Posted by: bganglia Posted at: 2018-04-24T14:49:29.335Z Reads: 412

```
I think the diyeboard 90mm hubs perform a bit better, while the maytech hubs are more durable (thicker urethane).
```

---
## \#87 Posted by: Mikenopolis Posted at: 2018-04-25T15:26:09.989Z Reads: 420

```
Just saw a video of your board. Looks very nice and stealth but those hub wheel caps are really ugly.
```

---
## \#88 Posted by: e.board_solutions Posted at: 2018-04-25T15:49:19.330Z Reads: 420

```
It's a wiki you can add info :slight_smile:
```

---
## \#90 Posted by: BrokenGloves Posted at: 2018-05-04T20:29:13.214Z Reads: 401

```
Hi shepherd, I'm in the same boat as you looking at the same motor, how did you get on with this?
Thanks
```

---
## \#91 Posted by: ZEEGREWAR Posted at: 2018-05-06T22:45:51.962Z Reads: 389

```
Hi ther im a first time builder just normally a rider but all this information is great just what i need to get started thanks alout cheers.
```

---
## \#92 Posted by: e.board_solutions Posted at: 2018-05-07T06:52:56.853Z Reads: 398

```
Where are you from? :slight_smile:
```

---
## \#93 Posted by: ZEEGREWAR Posted at: 2018-05-07T18:41:55.256Z Reads: 415

```
Hi ther im from Australia i got my self a R2 a few months back arfter a long 12 month wait i love it ..
```

---
## \#94 Posted by: sylvestertan Posted at: 2018-05-19T19:50:02.595Z Reads: 400

```
Hi!! I'm new to this website. Is there anyone out here from Singapore who have built their own electronic skateboard. Would appreciate if he/she could show me the way on building one here in Singapore. Thanks!
```

---
## \#95 Posted by: Mishsneha Posted at: 2018-05-30T18:35:23.677Z Reads: 391

```
Your post has encouraged me to make an electric skateboard for me. It is the best diy I had ever read. Thanks for this information hope I will make it as fast as I can.
```

---
## \#96 Posted by: plasteroid Posted at: 2018-06-04T18:59:00.922Z Reads: 380

```
Great post, thank you @e.board_solutions for putting this together.    Several things that I hadn't considered.
```

---
## \#97 Posted by: e.board_solutions Posted at: 2018-06-04T19:18:27.496Z Reads: 398

```
you're welcome :slight_smile:
```

---
## \#98 Posted by: Skunk Posted at: 2018-06-07T14:14:20.661Z Reads: 379

```
I'm gonna have to read this a dozen more times.  Thanks for the info. Just got gifted a riptide r1 and now I wanna build something a bit better.
```

---
## \#99 Posted by: WhiteRussian Posted at: 2018-07-02T02:37:35.076Z Reads: 351

```
**Hey Guys need help im 7 feet toll, and 285 lbs and i wanna get Evolve carbon GT is it gonna be good for me or better to build a custom?**
```

---
## \#100 Posted by: e.board_solutions Posted at: 2018-07-02T12:14:55.553Z Reads: 371

```
DIY build FTW :slight_smile:
```

---
## \#101 Posted by: koralle Posted at: 2018-07-02T12:28:32.760Z Reads: 378

```
Heavily depends on your intended riding style.
```

---
## \#102 Posted by: nuttyjeff Posted at: 2018-07-18T05:50:58.817Z Reads: 364

```
Am from SG and have built about 9 boards already (: HMU if you need any help/advice.
```

---
## \#103 Posted by: adrienfeve Posted at: 2018-08-02T21:37:24.936Z Reads: 342

```
Amazing guide thanks
```

---
## \#104 Posted by: exway Posted at: 2018-08-22T05:34:36.283Z Reads: 292

```
Awesome guide. Thanks!
```

---
## \#105 Posted by: dominic Posted at: 2018-08-29T04:38:26.541Z Reads: 292

```
ayyy i havent been on the forum in a quick min but my cad motor mount is in this post next to the enertion one lol. (that cad is bad dont look at it) i have new cad for mounts i might post but with the hobby king mount idk if anyone will even use it
```

---
## \#106 Posted by: kautilyatyagi Posted at: 2018-09-09T23:59:26.726Z Reads: 280

```
Thank you! This is exactly what I was looking for. Is there anyone from Charlotte, NC who has done this ?
```

---
## \#107 Posted by: electric Posted at: 2018-09-19T22:44:52.122Z Reads: 265

```
Thank you for this post!
Very informative and has made me aware of the electric skateboard tech used here.
```

---
## \#109 Posted by: moon Posted at: 2018-10-02T21:28:52.660Z Reads: 256

```
Increase reading time
```

---
## \#110 Posted by: Savace Posted at: 2018-10-02T21:29:46.552Z Reads: 260

```
Thanks just see that in another search i did - thanks for the heads up!
```

---
## \#111 Posted by: moon Posted at: 2018-10-02T21:30:17.771Z Reads: 268

```
If its a simple question post it here

https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559
```

---
## \#115 Posted by: moon Posted at: 2018-10-02T22:07:41.102Z Reads: 249

```
yeah, dont fuck around with batteries
```

---
## \#117 Posted by: Savace Posted at: 2018-10-02T22:24:17.478Z Reads: 278

```
[quote="Savace, post:112, topic:46844"]
Ill try to explain it briefly, basically i have a 12s10p 18650 set up, board keeps cutting at 44volts (should be 50V full charged and can hit around 38V before needing recharge), this is a self build, there are **4** of the packs (pictured below ) in the board, each with **3** rows of **10** batteries ( 4 x 3 = 12s / 10 = series)

when taking the voltage across all the packs this is what it looks like

1st pack | | | X 3.53 3.28 3.53 10.4
2nd pack | | X | 3.8 3.8 3.8 11.68
3rd pack | X | | 3.8 3.8 3.8 11.67
4th pack X | | | 3.8 3.8 3.8 11.67

clearly the 1st pack is the problem which is what is in the pic - the middle row has the lowest voltage across it at 3.28. I have guessed two of the cells and cut them out the series and tested them and they both show 3.28.
so my question is - how can identify the bad cell - do i need to cut them all out and test - i have a feeling they have balance charged since the board cut out so none will be “dead”
[/quote]

CREATING A TOPIC ON THIS NOW _ ADMIN PLEASE DELETE IF YOU WOULD LIKE
```

---
## \#118 Posted by: jippijuk Posted at: 2018-10-07T06:28:24.090Z Reads: 273

```
Hi There , Im starting to get my parts together for my first E Mountain Board.

Due research about my motor speed controller ESC or VESC I would like to add a note to the Beginners guide :slight_smile:
The ESC or VESC need to be set up with the right settings according to your Motor, Batterie and so on. This requires a Computer with software.
NOT all software is supported by Windows and Mac/IOS !
I found only one speed controller that supports software for IOS ( FOCBOX)
Anybody knows a decent speed controller with software for IOS?
thanks
```

---
## \#121 Posted by: skinnykemper Posted at: 2018-10-23T20:45:29.647Z Reads: 239

```
Great post, thanks for taking the time. :ok_hand:
```

---
## \#122 Posted by: Jc06505n Posted at: 2018-10-23T20:52:46.380Z Reads: 258

```
[quote="jippijuk, post:118, topic:46844"]
I found only one speed controller that supports software for IOS
[/quote]


This is wrong, kinda. so long as the vesc has a usable uart port, then a BT module can be used to connect to an ios application (Metr, xmatic, etc) meant for esc's (so long as that app is configured to play nice with whatever firmware you got). But thats not limited to just vesc's 

Hobbywings esc's have their own esc with application interaction.
```

---
## \#123 Posted by: reedbryson Posted at: 2018-10-24T16:42:17.896Z Reads: 258

```
Project wowgo upgrade! |Stock wowgo | Paris v2 | Wowgo hub motors |6.4 Panasonic(I think)| Stock ESC

So I have been looking a lot into upgrading my wowgo2s. It is a great eskate but I want something with a bit more torque and hill climbing ability. I am going to be doing this all in little pieces. I was looking at getting a focbox unity right now and later switch to a belt drive system. Any thoughts? Would the focbox unity work with my stock set up and remote? Is there an esc that is better out there?
```

---
## \#124 Posted by: thatsq Posted at: 2018-11-19T12:32:13.202Z Reads: 235

```
Thanks, very useful!:grinning:
```

---
## \#125 Posted by: Eboosted Posted at: 2018-11-28T05:53:46.215Z Reads: 248

```
[quote="E1Allen, post:15, topic:46844"]
Also there is an hour long video
[/quote]

OMG! 1 hour? If I were a beginner I'd kill myself.

Setting up a vesc should take more than 5 minutes.
```

---
## \#126 Posted by: BruSkater Posted at: 2018-11-28T06:16:52.902Z Reads: 293

```
This one is just perfect:

https://youtu.be/v1glLDO-EjA
```

---
## \#127 Posted by: MannyM0E Posted at: 2018-11-28T06:26:19.693Z Reads: 305

```
☝🏽 What he said 
This video is great in explaining how to use the vesc tool for beginners.
```

---
## \#131 Posted by: Kingdom421 Posted at: 2019-01-21T20:16:45.963Z Reads: 234

```
How do I get these
```

---
## \#132 Posted by: Andy87 Posted at: 2019-01-21T20:40:14.100Z Reads: 240

```
Use the search function here or google 😉
```

---
## \#133 Posted by: Yettyleung Posted at: 2019-01-24T02:03:26.672Z Reads: 244

```
Here there!
I am Yetty from China. 
Here I would like to recommend some new fashion style of wheels if you don't mind.
And if any interested, you can contact me on below link in Alibaba or contact me directly my whatsapp: +86-13528355672 :grinning:
https://www.alibaba.com/product-detail/2019-hot-sale-5-6-7_60834993292.html?spm=a2747.manage.component-marhttps://www.alibaba.com/product-detail/2019-hot-sale-5-6-7_60834993292.html?spm=a2747.manage.component-market-list-item.2.775c71d2MnuICoket-list-item.2.775c71d2MnuICo
```

---
## \#134 Posted by: mmaner Posted at: 2019-01-24T02:08:09.429Z Reads: 216

```
Do you actually have 5in pnumstic wheels?
```

---
## \#136 Posted by: Yettyleung Posted at: 2019-01-24T02:14:18.080Z Reads: 221

```
But we can make 5 inch in production if you want more 300pcs.:blush:
```

---
## \#137 Posted by: Yettyleung Posted at: 2019-01-24T02:14:32.675Z Reads: 225

```
[quote="Yettyleung, post:135, topic:46844"]
Hi. We now only have 8 inch in stock. Size is 200mmX50mm. Is it suitable for you?:blush:
[/quote]

Hi. We now only have 8 inch in stock. Size is 200mmX50mm. Is it suitable for you?:blush:
```

---
## \#138 Posted by: mmaner Posted at: 2019-01-24T02:33:31.138Z Reads: 223

```
No, many of us are looking for 5x2 onumatic wheels. If you can do a smaller MOQ and send ouy some samples to a couple of people to test we could probably do a group buy.
```

---
## \#139 Posted by: badger4life Posted at: 2019-01-26T00:00:21.709Z Reads: 212

```
Hey all, I'm new to the forum and I need to post a question that I have about a VESC that I'm having a problem with.  However, when I try to create a new post it doesn't look like I have the privileges needed to create a post.

Do I need to be a member for a set amount of time before I can post a new topic?
```

---
## \#140 Posted by: jap206 Posted at: 2019-01-28T15:03:43.491Z Reads: 204

```
I have gen 1 boosted board that needs a new battery but Boosted company says it will cost 400.00-500.00 USD to fix. Is it possible to put a gen 2 battery in if I mod the connection? Please email me back at jasonapotts@gmail

Thanks
```

---
## \#141 Posted by: Andy87 Posted at: 2019-01-28T15:33:13.936Z Reads: 214

```
Just get a used gen1 battery and you good to go.
You can get them on eBay for cheap for sure
```

---
## \#142 Posted by: paulbriz Posted at: 2019-02-06T21:58:39.694Z Reads: 214

```
![longboard%20esk|690x477](upload://1ZkwHVZZzLp8EeKlzkXLyWxoF5u.jpeg)  I made this for the lols , but I think it mgkt help diagram
```

---
## \#143 Posted by: buildityourself Posted at: 2019-02-25T17:40:43.384Z Reads: 212

```
Does anyone recognize this input? Where would I be able to buy a wire to connect this to my loop?![image2|375x500](upload://e8teg6ZhHZagnofHrP0Sxun5LDv.jpeg) ![image1|375x500](upload://e8sSRX7u69oSCe0FYY0KS0FB4rm.jpeg)
```

---
## \#144 Posted by: paulbriz Posted at: 2019-02-26T12:39:34.907Z Reads: 193

```
hopefully this video can help anyone, i am also a beginer but think it may help https://youtu.be/DSc-UmukDaI
```

---
## \#146 Posted by: Johnv Posted at: 2019-03-09T17:14:42.086Z Reads: 169

```
I have a question, so my board could reach top speed when I had 83 mm wheels but now that I put 110 mm wheels on it, it runs out of juice so quick but then 20 mins later can do the same thing. Is there anyway I can fix this discharge problem maybe add another battery?
```

---
## \#147 Posted by: Voyager1 Posted at: 2019-03-13T23:51:46.017Z Reads: 168

```
This has made me buy a helmet right now
```

---
## \#148 Posted by: Swaight Posted at: 2019-03-18T20:24:33.527Z Reads: 170

```
Hey do you think you could look over my design and give me some feed back on if it'll work or what i can do to make it better ?

2x 6374 190 kv sensored hobby sky motors 
2x VESC  4.12
4x 5000mAh lipo batteries 11.1v 3s1p

![1|690x318](upload://2biaRQcATSDNjsZv6X2mzcuEFri.jpeg)
```

---
## \#149 Posted by: thisguyhere Posted at: 2019-03-18T21:17:47.642Z Reads: 176

```
preface, i don't use lipos.

you're going after 12s right?  if so, the way you have the batteries diagramed works out to a 6s2p.  if you're going for 12s, should be like this:

![image|690x485](upload://nPQRDtJ9BjLJI4qfUoK7G4j2cF5.png) 

also, the power connection to the two vescs are in serial.  you want that in parallel:

![image|520x500](upload://hSaHNUF2j7E1zzG9NA9j9zPHlXe.jpeg)
```

---
## \#150 Posted by: Swaight Posted at: 2019-03-19T20:59:35.032Z Reads: 174

```
do you think i would  be able to use this for connecting my batteries in series ?


![0bd6e57e76abe77f3eba39b9ec34e8b637be686d|567x425](upload://tkyZVbRkY6cWP0Y78IS7IlOLoau.jpeg)
```

---
## \#151 Posted by: thisguyhere Posted at: 2019-03-19T21:05:44.740Z Reads: 172

```
to be honest, i don't really understand this diagram.  and i don't want to give you bad information.  like i said, i don't use lipos.

maybe someone else can jump in here.
```

---
## \#152 Posted by: Swaight Posted at: 2019-03-19T21:08:57.592Z Reads: 164

```
you know of anyone else i might be able to talk to?
```

---
## \#153 Posted by: bmolnar Posted at: 2019-03-20T05:15:42.612Z Reads: 178

```
To connect in series put the + of one battery with the - of the other battery. This adds the voltage.

To connect in parallel put the + of one battery with the + of the other (and vice versa). This adds the capacities.
```

---
## \#154 Posted by: e.board_solutions Posted at: 2019-03-20T15:14:03.905Z Reads: 180

```
looks good for 4 pacs in serie
```

---
## \#155 Posted by: paulbriz Posted at: 2019-03-30T22:47:02.350Z Reads: 169

```
Here's my battery guide I m guessing this is the best place to post it https://youtu.be/od9hAs69crk please subscribe to help me meet my college target
```

---
## \#156 Posted by: JCV Posted at: 2019-04-05T18:30:56.986Z Reads: 153

```
If I have 3 4s batteries already in series, how do I add another one but in parallel, is there a diagram or any reference to understand how I wire that?
```

---
## \#157 Posted by: Clonkex Posted at: 2019-04-05T22:11:49.562Z Reads: 158

```
You can't add just one. You would have to add another three 4s batteries.

Say the batteries are 5000mAh. If you have three of them in series, that's three 5000mAh batteries. If you add another 5000mAh pack in parallel with one of the existing 5000mAh packs, you now have two 5000mAh packs and the equivalent of a 10000mAh pack. That will work (in that it won't immediately blow up), but as soon as you start using it, the 5000mAh pack voltages will drop much faster than the 10000mAh pack voltage and you'll end up with a severe voltage difference. This might simply kill the batteries or it might make them catch fire. Either way it's not something you want to do.
```

---
## \#158 Posted by: JCV Posted at: 2019-04-06T22:19:37.516Z Reads: 145

```
Ok I get it thank you very much
```

---
## \#159 Posted by: JCV Posted at: 2019-04-07T19:51:24.945Z Reads: 147

```
Ok one more question so how can I tell me motor is the one with the problem bc I sent way to much current through it about 82 amps and max is like 70 whoops (6374 190kv) but could it be the vesc that’s the problem?
```

---
## \#160 Posted by: Mainsedora Posted at: 2019-04-09T21:22:57.017Z Reads: 141

```
How long did this current flow?
```

---
## \#161 Posted by: JCV Posted at: 2019-04-12T18:34:09.621Z Reads: 139

```
If anyone knows is the reverse torque motor mount meant for a motor not mount on the inside but on the outside (reverse) so the back? And can you use a regular one that’s meant for the normal way?
```

---
## \#162 Posted by: theblackinfamous Posted at: 2019-04-24T14:58:32.836Z Reads: 125

```
I'm from SG, and was thinking of building an eSk8. Wonder roughly the costing for a beginner? I know this sounds very vague, but if you could provide some information, i'll be thrilled!
```

---
## \#163 Posted by: nuttyjeff Posted at: 2019-04-24T15:14:27.006Z Reads: 124

```
@Linny tagging you in
```

---
## \#164 Posted by: Linny Posted at: 2019-04-24T16:11:14.796Z Reads: 124

```
Good decision of choosing to build one! First is to decide if you want a single or dual drive motor build. If you are 70kg and below, a single drive is good for a first build. It's also cheaper than a dual since you need double motors, mounts, VESCs. If budget is not a problem, i'd recommend a dual drive. A mid range quality single drive build can cost just over $1k SGD, and about 1.5k for a dual.
```

---
## \#165 Posted by: theblackinfamous Posted at: 2019-04-24T17:05:17.737Z Reads: 125

```
Ah, i'm at 60kg, so a single or dual doesn't matter in my case, i guess. For budget, i do have some spare cash that i meant to build one, but sadly, it's around 700. I guess i'll pop back in when i saved up enough. That being said, thanks @nuttyjeff and @Linny!
```

---
## \#166 Posted by: WolffXIII Posted at: 2019-04-27T08:46:08.403Z Reads: 126

```
Thanks so much for this guide. So excited to start my new build :smiley:

Thanks again
```

---
## \#167 Posted by: Joyal Posted at: 2019-04-27T10:09:32.263Z Reads: 122

```
Can please give me the informations about wires
Ie, Ha,Hb,Hc and A,B,C
```

---
## \#168 Posted by: trapsends Posted at: 2019-05-06T09:21:05.526Z Reads: 123

```
Hi Guys,
I am convincing a older relative who is very smart at technology and all stuff to do with voltages and making stuff to help me make and assemble a diy board. he wants some articles and links for reading and i have given him some. i need more please aha! any articles that give insight into esk8 (he wants lots of reading). I need to convince him of why i need more than 20kmh as well aha. If any of you could write a paragraph and link some articles i will love you forever!
Thankyou
```

---
## \#169 Posted by: taz Posted at: 2019-05-06T09:35:54.627Z Reads: 125

```
You have 25m read time on the forum.

Why not try reading some more? Maybe then you will find the articles and information yourself.
```

---
## \#170 Posted by: tylor Posted at: 2019-05-07T03:30:01.886Z Reads: 122

```
use 18650 batteries or other lipo batteries?
```

---
## \#171 Posted by: no-role-modle Posted at: 2019-05-07T21:12:20.064Z Reads: 129

```
Great thread.  I will take my time and go over this!!!
```

---
## \#172 Posted by: pta Posted at: 2019-05-22T01:32:22.713Z Reads: 113

```
Thanks for this. A great start to understand what I've got.
```

---
## \#173 Posted by: Lincon Posted at: 2019-05-29T16:59:19.294Z Reads: 102

```
Hello everyone,,
Well I’m not sure how many people take the time to screw up a wiki page on purpose.
Honestly it doesn’t matter what forum https://youporn.wiki/ you go on you’re going to get the same “dumb” questions over and over https://xhamster.vip/ even if search was used. Sure it’s a pain sometimes but this sport is changing fast. What was the new hotness a few months ago might be old and busted by the time a new member searches(or doesn’t) something.
```

---
## \#174 Posted by: raspberrypi33 Posted at: 2019-06-01T17:34:24.345Z Reads: 96

```
Nice article! I am considering building an esk8 this summer and this forum is a lifesaver! This is my first post, so please be patient with me! Just a quick question, what material should the motor mount and pulleys be made out of? I have seen aluminum, carbon fiber, and even 3D printed versions. Also, does the strength and hardness of the pulleys affect their ability to perform optimally? For example, a 3D printed pulley versus an aluminum one. Thanks guys! :grinning:
```

---
## \#175 Posted by: e.board_solutions Posted at: 2019-06-01T20:03:45.748Z Reads: 96

```
3d printing a mount is a bad idea :) For pulleys it's possible but alu is more durable :slight_smile:
```

---
## \#176 Posted by: raspberrypi33 Posted at: 2019-06-02T02:46:34.982Z Reads: 93

```
Thanks so much! Any specific type of aluminum (like grade or finish)?
```

---
## \#177 Posted by: e.board_solutions Posted at: 2019-06-02T08:43:04.618Z Reads: 94

```
The ones I sell hereare very good ;)

https://electricboardsolutions.com/collections/pulleys-belts-mounts
```

---
## \#179 Posted by: MahmoudMonem Posted at: 2019-06-15T07:58:07.408Z Reads: 90

```
Hello Guys, 
Unfortunately, Inboard technology gave me a board for $1500 that worked for only 2 months and to fix it they need me to pay another $500 + shipping cost. So, I need your help in choosing some parts for my e-skateboard while keep in mind that i'm outside the USA.

I have a battery with the below specifications and I need to understand how to choose a ESC and back truck compatible with that battery;

- Lithium-lon Battery
- Voltage: 43.2V nominal 49.2V peak
- Capacity: 97Wh 2.25Ah


Advanced Thanks.
```

---
## \#180 Posted by: speedystage772 Posted at: 2019-07-01T12:23:58.543Z Reads: 77

```
For the esc it depends on your budget and how you will use your board . A good esc is called a vesc and you can change the settings however there is a diy version but there is no settings options. For the motors you will first have to decide between a hub motor which is less hassle to install with less maintenance or a belt drive which has a better performance.
```

---
## \#181 Posted by: Harrisonwms Posted at: 2019-07-04T01:17:27.019Z Reads: 72

```
What does everyone use to build a li-ion pack? I don’t want to layer 5 strips and I am trying to get a pack that can supply over 60 Amps with losing most of its power by heat!
```

---
## \#182 Posted by: Harrisonwms Posted at: 2019-07-04T01:18:27.567Z Reads: 74

```
I know to spotweld nickel and all but from what I know I would need at least 5 or 6, what can I put on top of just 1 to help carry the amperage?
```

---
## \#183 Posted by: Harrisonwms Posted at: 2019-07-04T01:24:53.492Z Reads: 74

```
@Linny I heard you could give me some insight /\
            |
```

---
## \#184 Posted by: Linny Posted at: 2019-07-04T01:28:02.718Z Reads: 75

```
Ah, i'm no battery builder however. Perhaps you can take a look at this thread and see how people do their packs. 

https://forum./t/the-battery-builders-club/720
```

---
## \#185 Posted by: Harrisonwms Posted at: 2019-07-04T03:28:52.260Z Reads: 71

```
@Linny Thanks you soooooo much just read through it all and now I understand it! Thanks!!
```

---
## \#186 Posted by: Harrisonwms Posted at: 2019-07-04T03:30:08.173Z Reads: 69

```
Also @Linny my esc that I used overheated super quick after about 2 miles, would installing some micro fans help stop it from over heating?
```

---
## \#187 Posted by: Linny Posted at: 2019-07-04T03:38:54.261Z Reads: 67

```
How hot did it get? An aluminum heatsink or fans will definitely help. I'd go for the heatsink.
```

---
## \#188 Posted by: Harrisonwms Posted at: 2019-07-04T03:49:58.477Z Reads: 63

```
The heat sink came already on it, it’s pretty thick to
```

---
## \#189 Posted by: Harrisonwms Posted at: 2019-07-04T03:51:33.799Z Reads: 62

```
@Linny it got so hot that I couldn’t hold it, over 120 °F, then it just shut off, it turns back on after it cools, did I mention that it melted through the duct tape I used to protect my batteries 😂
```

---
## \#190 Posted by: Harrisonwms Posted at: 2019-07-04T03:53:07.318Z Reads: 67

```
This is the exact esc I have https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F322688416729
```

---
## \#191 Posted by: Linny Posted at: 2019-07-04T04:05:37.505Z Reads: 76

```
Ah, these are notorious for having issues.

I'd get a flipsky 4.12 VESC minimum. I run these on a single drive and it gets up to 50 deg c which is normal, but will not cutout.
```

---
## \#192 Posted by: Harrisonwms Posted at: 2019-07-04T04:16:34.994Z Reads: 78

```
Could you provide I link for a cheap one? I am kinda on a budget
```

---
## \#193 Posted by: Linny Posted at: 2019-07-04T04:51:53.020Z Reads: 80

```
The Flipsky one **is** a budget haha. 

Currently on sale now for 60 US. Anything lower than that will be the ESC that you are using now. 

https://flipsky.net/collections/electronic-products/products/mini-fsesc4-20-50a-base-on-vesc-widely-used-in-eskateboard-escooter-ebike
```

---
## \#194 Posted by: Harrisonwms Posted at: 2019-07-04T05:06:55.498Z Reads: 81

```
Awesome thanks!
```

---
## \#195 Posted by: jason-skateboarder Posted at: 2019-07-05T03:19:54.136Z Reads: 76

```
I want to build a skateboard. But it seems a little difficult.
```

---
## \#196 Posted by: samr Posted at: 2019-07-14T04:44:39.651Z Reads: 68

```
I want to buy the dual FSESC4.20 but I don't know which controller is compatible with it. Do I need to buy a receiver that plugs into this esc and then buy the controller with that?
```

---
## \#197 Posted by: mohitkorganji Posted at: 2019-07-14T18:56:48.210Z Reads: 69

```
Hi everyone, I've been trying to download the vesc project tool, but the website is either down or has been moved. Does anyone know where I can get it?  Thanks.
```

---
## \#198 Posted by: wandagoner Posted at: 2019-07-15T07:16:03.554Z Reads: 73

```
I believe the vesc project site is down @rpasichnyk mentioned it in the [All new 2019 VESC-Tool release thread](https://www.electric-skateboard.builders/t/all-new-2019-vesc-tool-release/83619/654?u=wandagoner).  you can probably grab it from [GIT](https://github.com/vedderb/vesc_tool) if you cannot wait
```

---
## \#199 Posted by: rpasichnyk Posted at: 2019-07-15T07:28:35.590Z Reads: 76

```
You can get VESC Tool here https://github.com/rpasichnyk/vesc_tool/releases if you don't want to compile it yourself
```

---
## \#200 Posted by: pundahh Posted at: 2019-07-15T09:09:48.782Z Reads: 80

```
All ppm controllers are compatible with the esc. Your remote should come with a receiver. Just note not to buy an ESC controller is all :smiley:
```

---
## \#201 Posted by: bshin100 Posted at: 2019-07-16T00:25:53.685Z Reads: 85

```
Hi everyone! I didn't want to spam you guys with a new topic so I decided to reply here! I'm new here (just created an account), and I've been lurking the wikis and posts (without an account), and doing research (mostly YouTube and Reddit) for the past several weeks. I'm looking to build an electric longboard for fun, and I'm an entering freshman in college so this could be a cool way to get around campus. 

So like I said, I've been reading and researching, and I compiled this spreadsheet with the potential parts for my new E-Board from sellers that seem to be liked among the esk8 communities: 
https://docs.google.com/spreadsheets/d/1rAdDfoDBLXXPcLyFwsk4NGGoB_o_kkf0g2Eyqb2e5I0/edit?usp=sharing
I've included alternate parts/packages (not checkboxed) that I am considering if the selected ones don't work. I've left out the minor stuff like grip tape or connectors, because I want to focus on the main components. I also plan to make my own enclosure.

I'd greatly appreciate any kind of feedback that you all have on these parts. Are there any compatibility errors I'm missing? Is there a better & cheaper source for the parts I have selected? 

Thanks in advance!
```

---
## \#203 Posted by: trainingforutopia Posted at: 2019-08-17T21:14:12.879Z Reads: 65

```
@e.board_solutions
I know the LFP vs LiPo vs LI discussion has no clear answer, but I think it is time to include LFP cells as a serious alternative for LiPo and LI. They have reached a point where they have the same price, but are just way easier and safer to assemble and use than LiPo and LI. Yet, they are not seriously included in the guide. Maybe time to update?
Example: https://www.electric-skateboard.builders/t/cylindrical-lifepo4-as-serious-alternative-to-lipo-18650s/100462
```

---
## \#204 Posted by: e.board_solutions Posted at: 2019-08-18T09:55:27.895Z Reads: 65

```
It's a wiki you can make changes yourself :slight_smile:
```

---
## \#205 Posted by: jasonfoy123 Posted at: 2019-08-22T11:01:10.417Z Reads: 64

```
I reading all the comments almost But I realised here's people are so professional, I am also working as fresh elctrical engineer in [Ripple Electrical](https://rippleelectrical.co.nz/) company located at Auckland, New Zealand.
```

---
## \#206 Posted by: Grabacr Posted at: 2019-09-04T04:09:35.089Z Reads: 60

```
Hey everyone! I'm new to the DIY eskate scene and I finally recieved my unity not too long ago. I've Been trying to set up the motor via the guided setup, but every time I do I get the error "L is 0. Please measure it first." I've looking for an answer for the last two weeks and haven't found one. Has anyone had a similar issue or know what the problem is or how to fix it?

Thanks in advance!
```

---
## \#207 Posted by: Bona Posted at: 2019-09-04T22:39:03.552Z Reads: 65

```
cool, thanks!
```

---
## \#208 Posted by: SkateYS Posted at: 2019-09-09T00:46:54.186Z Reads: 62

```
Edit: Diagram is good! Not sure why you don't just rewire the packs as a single pack!
```

---
## \#209 Posted by: MaxGoldenson Posted at: 2019-11-05T05:46:48.982Z Reads: 37

```
Hello everyone,
I am planning on starting my first Electric skateboard build. Unfortunately I have little knowledge of how to do this (but I know the basics), and even less funding (i'm a broke teen) so I was wondering if anyone had any advice for me and would like to donate to my cause. Thanks a lot!
-Max Goldenson

LINK:
https://www.piggybackr.com/users/maxwellgoldenson/fundraisers/help-me-make-my-diy-electric-skateboard-a-reality/public
```

---
## \#210 Posted by: paulbriz Posted at: 2019-11-07T12:40:05.671Z Reads: 33

```
Helo i thought you will like this build vid its of the making of an electric skateboard which is in the style of the back to the future board 
 https://www.youtube.com/watch?v=HZ8u3TFPAYQ
```

---
## \#211 Posted by: Kayotiic504 Posted at: 2019-11-13T22:48:11.596Z Reads: 29

```
That’s so sick looking!
```

---
## \#212 Posted by: Analogue_Sk8r Posted at: 2019-11-29T14:52:52.488Z Reads: 27

```
I'm kinda new on this E-sk8 stuff. Is there any way to build an e-sk8 with direct wire controls. Is there a way to replace remote control with a potentiometer that's directly wired to the ESC, or rather just potentio-battery-motor.

Thanks
```

---
## \#213 Posted by: esk8me Posted at: 2019-11-29T15:39:48.473Z Reads: 27

```
Great guide,Thanks for sharing!
```

---
