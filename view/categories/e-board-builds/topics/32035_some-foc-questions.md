# Some FOC Questions

### Replies: 57 Views: 3260

## \#1 Posted by: Aborn Posted at: 2017-09-01T17:04:45.202Z Reads: 223

```
I'm about to order parts for a build, but i have some questions regarding 'FOC'

I'm planning to get a 'FOC-BOX' vesc from Enertion.

What is FOC, how does it work? What do i need to use it?
```

---
## \#2 Posted by: psychotiller Posted at: 2017-09-01T17:14:28.296Z Reads: 221

```
<img src="/uploads/db1493/original/3X/c/5/c5eca992d2b833f834c13b4410508065085b273f.png" width="350" height="350">

The answers you seek

are the questions you ask..or something like that
```

---
## \#3 Posted by: MontPierre Posted at: 2017-09-01T17:16:54.971Z Reads: 217

```
There are multiple threads here about FOC, pleas try to search forum first. Then once you have some particular questions give us a shout.

Quick search doesn't hurt 

http://www.electric-skateboard.builders/t/vesc-faq-what-is-foc-field-oriented-control/419?u=montpierre
```

---
## \#4 Posted by: Aborn Posted at: 2017-09-01T17:36:35.720Z Reads: 213

```
I did try to search the forum but i couldnt find anything actually. Thanks for the link!

My more specific questions is whether i need any special motor with a special sensor os something for it to function?

*Edit: I acutally did read that post.
```

---
## \#5 Posted by: ikjahaa Posted at: 2017-09-01T17:43:24.608Z Reads: 205

```
Get a sensored motor for foc
```

---
## \#6 Posted by: psychotiller Posted at: 2017-09-01T18:00:02.680Z Reads: 202

```
There you go! yes, you should buy a sensored motor if you want the benefits of foc
```

---
## \#7 Posted by: themegak Posted at: 2017-09-01T18:21:53.140Z Reads: 191

```
I have been rolling around on a pair of sensored 190KV motors FOC style for over a year.  It is buttery smooth on startup and the braking force is how i like it.  Of course that has a lot to do with how i set my VESC's up.  I won't go back to BLDC ever again, FOC is more than worthwhile you will be very satisified, just make sure you tune your VESC's to the kind of batteries, gear ratio, motors, etc you have.
```

---
## \#8 Posted by: ShutterShock Posted at: 2017-09-02T00:24:01.453Z Reads: 175

```
What kind of VESCS are you using? I was looking into FOC a little bit but I was nervous about blowing my DIYelectric VESC's
```

---
## \#9 Posted by: Vanarian Posted at: 2017-09-02T00:36:49.786Z Reads: 169

```
Cool them and you won't blow them ! I was talking about VESCs right there
```

---
## \#10 Posted by: Aborn Posted at: 2017-09-02T00:56:46.326Z Reads: 162

```
Enertions FOCBOX is what i was planning to get. I think the bottom plate is made of aluminum for better cooling?
```

---
## \#11 Posted by: themegak Posted at: 2017-09-02T00:57:05.429Z Reads: 160

```
I am using one ollin vesc and one esk8.de vesc.   I think you can use diys vesc but just run some tests on the bench while clocking realtime data in the bldc tool after you run your detections.  If you see any errors thrown in realtime data while on the bench you know you need to tweak your motor or batt max settings most of the time.  There is plenty of good documentation on this site but the best advice I can give you is to always run tests on the bench and always watch realtime data while you're doing it.  This would save a lot of DRVs in general.
```

---
## \#12 Posted by: ShutterShock Posted at: 2017-09-02T01:51:02.024Z Reads: 153

```
What settings should I watch on the real time tests?  The amp draw and erpm?  Or would you suggest looking around on the forum more?

FOC is appealing to me as I am a college student and use my board mostly on campus.  I don't have a big ability to cool the VESC's through my case, haven't had any issues yet, max temp I've hit on a 100 degree day is 54.
```

---
## \#13 Posted by: onepunchboard Posted at: 2017-09-02T02:47:18.655Z Reads: 148

```
u don't need sensor for foc. Foc designed to use hi torque in any speed given including low speed or dead stop. I use without sensor and never experienced Coggins even on dead stop at hill. 

Of course sensored will give u precision but this add cost and complexity. and generally sensored motors under performs in total power.

I'm not saying do this don't  but you should see the both pro and con before deciding. 

cheers
```

---
## \#14 Posted by: Aborn Posted at: 2017-09-02T03:43:45.267Z Reads: 142

```
So the questions comes down to whether the extra precision is worth the extra money and the loss in power?
```

---
## \#15 Posted by: psychotiller Posted at: 2017-09-02T03:52:21.527Z Reads: 139

```
It cost 8 bucks more per motor for sensored. And it's way better!
```

---
## \#16 Posted by: treenutter Posted at: 2017-09-02T03:53:34.670Z Reads: 141

```
It's worth it.
```

---
## \#17 Posted by: Aborn Posted at: 2017-09-02T03:54:12.064Z Reads: 142

```
That is that settled. :slight_smile:
```

---
## \#18 Posted by: hornet90 Posted at: 2017-09-02T05:51:19.178Z Reads: 147

```
for me cutting wiring soldering breaking stuff blowing up stuff comes easy  but looking at the bltc tool and setting that up stresses me out:confused:...i setup foc i had a axle vesc 10s 192kv 100mm mbs
wheels ,it was like floating on air my test track is a park with flats and hills it took the hills like they where flat ground....im 76kg...I forgot my helmet so i took it easy i was hitting 25mph it felt like it would do 30 easy but with no helmet i backed off...went home charged up the batterys went back out and board would turn guess what drv fault...That was 2 weeks ago....
Im waiting on a focbox to get here but i would pay some one to log into my pc and setup my focbox in foc mode theres not a start to finish setup on it...I know i missed up the setting thats why it blew..
will i set up foc again dont know if i will...


https://www.electric-skateboard.builders/t/irish-shamrock-build-no2/23997/29?u=hornet90
```

---
## \#19 Posted by: rich Posted at: 2017-09-02T10:08:58.059Z Reads: 140

```
Hey @Aborn, if you are based in europe (what I guess) don't buy FOCBOX, don't buy maytech (or rebranded like greenmotion amongst others) and don't buy all this cheap crap. BTW FOCBOX is not bad but in case of any fault you have to send it to australia (and pay 2x shipping costs which costs more than 50% of the focbox) plus costs for repair (if it's your fault) and wait for weeks or months.

Be more smart than me. I bought 10 Vescs until now and did waste a lot of money for crap.
I have flier V4.12's (buggy), when I claimed they said no warranty.
I have maytech's (one had cold solder joint), when I claimed I never got reply. BTW maytech don't run in FOC.

In my opinion the best quality and best customer support in europe has @esk8 
You can take a look at www.esk8.de 
You have three options:
1.) Buy PCB and capacitors and solder cables by yourself  (only if you know what you are doing) **130€**
2.) Buy complete V4.12 for **150€**
3.) or get the top model with direct FET'S and many upgraded parts and aluminium housing for **200€** (esk8 controller 1.1)

All controllers are made in germany and the components are top quality. I run them in FOC with 10s without problems.

Beside the fact that they offer warranty on manufacturing faults they offer repair service, this is genius! So if you destroy a V4.12 you can send it to germany and get it repaired for a fair price. If you destroy a focbox, maytech or anything else you can fling it to rubbish (if you don't know where to repair or you are not an electronic engineer).

I hope this helps with your decision.....  and if you'll use FOC get sensored motors :grin:
```

---
## \#20 Posted by: Aborn Posted at: 2017-09-02T13:18:25.799Z Reads: 132

```
Thank you so much, i'll get the top model 1.1! That should be best for FOC right? Also do you know where I can find a sensored 6374 190kv motor?

Edit: Esk8.de has them =D
```

---
## \#21 Posted by: Tuomalar Posted at: 2017-09-02T13:27:00.270Z Reads: 130

```
[quote="rich, post:19, topic:32035"]
Be more smart than me. I bought 10 Vescs until now and did waste a lot of money for crap.
[/quote]

You have made some serious mistakes if you broke so many:DDD 
Focbox is said to be bulletproof with foc. Just like Ollin's vesc. Esk8.de's new 1.1 version should be fine also. But i can't recommend any non-updated 4.12 version like maytech.
```

---
## \#22 Posted by: onepunchboard Posted at: 2017-09-02T13:36:08.823Z Reads: 125

```
agree. FB is really good. not sure why it's on bad list. and it's been around longer and improved overtime.
```

---
## \#23 Posted by: Aborn Posted at: 2017-09-02T13:47:13.721Z Reads: 124

```
They also offer warranty covering mistakes
```

---
## \#24 Posted by: rich Posted at: 2017-09-02T13:59:09.689Z Reads: 128

```
[quote="Tuomalar, post:21, topic:32035"]
You have made some serious mistakes if you broke so many:DDD
[/quote]


No, I didn't broke them :joy: 
My flier V4.12's have broken temp sensor and hall sensor ports (manufacturing fault)
My maytech V4.12's had cold solder joint (but fixed it). But they don't like FOC so they are useless for me (already 1 sold).
My esk8.de V4.12's perform excellent in FOC mode (I also have 2x controller 1.1. but not tested yet).

All my vescs are working but since I switched to sensored motors (on 2 builds) FOC was my only solution against cogging and I love it! I won't use BLDC mode anymore with sensored motors.

BTW I managed to short a vesc this week and both were dead. After reupload of FW everything seems fine, motors working again :grin:

[quote="Aborn, post:20, topic:32035"]
do you know where I can find a sensored 6374 190kv motor?
[/quote]

esk8.de has 170kv and 200kv 6374 sensored motors with 8mm shaft-
alienpowersystems.com has different kv (if in stock :wink:) but with 10mm shaft.

For FOC it's better not to use high kv motors, but 170kv or 190kv should be alright.
```

---
## \#25 Posted by: Aborn Posted at: 2017-09-02T14:05:49.921Z Reads: 119

```
Great stuff! I think I'm gonna get a antispark switch, 1.1 Vesc and a 170 Kv motor from there
```

---
## \#26 Posted by: rich Posted at: 2017-09-02T14:23:22.659Z Reads: 110

```
Sounds good :grinning:!
Which battery you'll use, how many cells in series?
```

---
## \#27 Posted by: Aborn Posted at: 2017-09-02T14:24:09.345Z Reads: 111

```
I'm gonna build a 10S4P out of Samsung 30Q with BMS :slight_smile:
```

---
## \#28 Posted by: rich Posted at: 2017-09-02T14:25:21.817Z Reads: 109

```
That's perfect, you gonna have a very nice build!
```

---
## \#29 Posted by: Aborn Posted at: 2017-09-02T14:29:34.776Z Reads: 110

```
I might need to find a new wheel pulley tho, the one I had in mind was from https://www.unikboards.com/en/
But the wheel pulley is 32T which is bit too few teeth for 170Kv, either that or I could go for some bigger wheels.
```

---
## \#30 Posted by: psychotiller Posted at: 2017-09-02T14:34:08.123Z Reads: 107

```
Scratches head...Sensored BLDC doesn't cog at all brotha! And you have more control over every aspect of throttle and brakes. I love FOC, but it's only benefit (the one I love) is the silence. That's it.
```

---
## \#31 Posted by: psychotiller Posted at: 2017-09-02T14:35:28.276Z Reads: 106

```
[quote="rich, post:24, topic:32035"]
do you know where I can find a sensored 6374 190kv motor?
[/quote]

Maytech has sensored 6374 190kv motors. I have some that are being installed on a couple of builds right now.

https://psychotiller.com/product/sensored-6374-190kv
```

---
## \#32 Posted by: Aborn Posted at: 2017-09-02T14:45:14.755Z Reads: 101

```
Yeah but that's California, so shipping and toll will be excessively expensive

I'm in Europe
```

---
## \#33 Posted by: psychotiller Posted at: 2017-09-02T14:46:42.436Z Reads: 105

```
Order straight from maytech.. I just put my link so you could see the specs. They'll have motors to you in 3 days from China.

And for the record, I ship to Europe often and rarely get complaints on fees
```

---
## \#34 Posted by: Aborn Posted at: 2017-09-02T14:48:37.580Z Reads: 104

```
Oh, that's great
```

---
## \#35 Posted by: Aborn Posted at: 2017-09-02T14:58:23.256Z Reads: 108

```
How much performance is lost when you run FOC?
```

---
## \#36 Posted by: psychotiller Posted at: 2017-09-02T15:28:04.006Z Reads: 106

```
A fraction of your top speed is lost. Where as in bldc you can run Hybrid so sensors aren't operating at higher speeds (when you don't need them)
```

---
## \#37 Posted by: Aborn Posted at: 2017-09-02T15:37:22.178Z Reads: 105

```
Okay thank you!

I'm probably getting this:
http://www.maytech.cn/en/mto6374-190-ha/10340.html
```

---
## \#38 Posted by: rich Posted at: 2017-09-02T15:59:48.962Z Reads: 109

```
[quote="psychotiller, post:30, topic:32035"]
Scratches head...Sensored BLDC doesn't cog at all brotha!
[/quote]

I wish that would be true in my case, but with trampa 6364 136kv and maytech 6364 200kv motors (with sensors) and no matter which V4.12's there is always evil cogging at startup (I made a own thread and was fiddling around for weeks with all possibilities to fix that). The hall sensor implementation is better in FOC and since I use FOC, the startup is butter smooth. I don't use FOC because of silence (but it's still nice) , it's because of startup. In BLDC mode (hybrid or sensor) mode I get angry :joy: 

Yeah 1000 words can't tell.... look at this video I did where you see the difference between BLDC and FOC. Especially the difference in startup which is in the beginning of the video (now i have to laugh when I see this but BLDC was annoying). I'm sure there are people which are using BLDC hybrid or sensored without problems, I just tell about my personal experience.

https://www.youtube.com/watch?v=ptlHqK7kqCA
```

---
## \#39 Posted by: Aborn Posted at: 2017-09-02T16:12:37.993Z Reads: 107

```
That is a huge difference wow!
 Why is it that so many people fry their vescs with FOC?
```

---
## \#40 Posted by: onepunchboard Posted at: 2017-09-02T16:15:25.245Z Reads: 107

```
foc switches fet faster than bldc thus more calculation req and possibly more electrical noise introduced. if vesc use cheap components well🤑
```

---
## \#41 Posted by: Aborn Posted at: 2017-09-02T16:21:13.945Z Reads: 105

```
I see, thanks!
```

---
## \#42 Posted by: Hummie Posted at: 2017-09-02T16:30:17.968Z Reads: 107

```
you increase performance with foc in many ways in that it's more efficient and is smoother.  maybe 2mph top speed decrease.
```

---
## \#43 Posted by: esk8 Posted at: 2017-09-02T16:38:31.289Z Reads: 110

```
Sorry but,
we have only Motors with 10mm shaft,
i don't need Motor with 8mm shaft.
```

---
## \#44 Posted by: esk8 Posted at: 2017-09-02T16:46:41.731Z Reads: 111

```
And our Motors have sensors too,
but i think we was the only shop, where you became 
the motors with sensor cable in optimal length and
with solders 6Pin sensor cable for the Vesc.
<img src="/uploads/db1493/original/3X/9/a/9a6eaa6de5976fbaac4f74528bbd037c7349e511.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/0/9/09501dc1d1b2b38da05bf93a290b78211c6434cb.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/e/2/e276814de14c01dc2ab6382f9dae0fafab2adb0c.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/2/8/286caa634f9200ddf6e984e7a59ff3dad4ea755f.JPG" width="500" height="500">
```

---
## \#45 Posted by: rich Posted at: 2017-09-02T16:49:26.208Z Reads: 106

```
[quote="esk8, post:43, topic:32035"]
we have only Motors with 10mm shaft,
[/quote]

You are right, my bad!
```

---
## \#46 Posted by: Aborn Posted at: 2017-09-02T16:56:36.247Z Reads: 106

```
I need 8mm shaft and 190 Kv :confused:
```

---
## \#47 Posted by: esk8 Posted at: 2017-09-02T17:10:35.537Z Reads: 113

```
Ok thats ok,
but what du you think?
Witch bearings holding and working longer?

8mm ore 10mm ?

<img src="/uploads/db1493/original/3X/5/4/5442b3b549b65103b2ccf1a070dad71aeb391842.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/3/234b75a692dd900cb5f2c9a9891f28d062803145.jpeg" width="666" height="500">
```

---
## \#48 Posted by: Aborn Posted at: 2017-09-02T17:37:57.868Z Reads: 106

```
That's a valid point, how much is a full single drive transmission kit with trucks from you?

That would be:
6374 200 Kv sensored motor
2 x caliber trucks
Motor mount
Timing belt
Wheel pulley
Motor pulley
Kegel wheels

It's a bit confusing that many of your item descriptions are in german

Also are your pulleys 9mm or 15mm
```

---
## \#49 Posted by: psychotiller Posted at: 2017-09-02T17:52:09.775Z Reads: 105

```
What motor did that 8mm bearing and shaft come out of? I realize you wan't to sell your 10mm axled motors, but don't mislead people into thinking your bearings are outlasting everyone else's. Because they're not. Not all 8mm motors use that bearing.

<img src="/uploads/db1493/original/3X/f/c/fc7c6c282cdb240df3a489dd8cb89be5f07ce645.png" width="500" height="352">
```

---
## \#50 Posted by: onepunchboard Posted at: 2017-09-02T21:26:18.915Z Reads: 102

```
I agree. even contract grade tool uses normal skate bearing or sometimes plain bushings and brushed motor. but they last 10 yrs or more. shaft size only matters for loading capacity. unless u plan to move 250lb gorilla with that motor full throttle all the time, 8mm will do the job.
it depends on the design but thicker shafts reduces stator size as well.
```

---
## \#51 Posted by: Vanarian Posted at: 2017-09-02T23:29:50.865Z Reads: 103

```
You got a nice build on the track ! For the motor you are in EU, you can also order from eskating.eu they're based in Italy, the guy has shipped many parts to France already  without sweat. He has sensored and non sensored sizes I think ? Or you have Banggood too for no name 63mm sensored motors.

esk8.de is reputable and already answering your questions though, what will you choose? lol

For antispark, you can look for a member from here he built reinforced antisparks, multiple models. I wait for his 3 direct-FETs compact version, bridge between the classic Vedder anti spark and his custom 6-direct FETs antispark. The website has antispark in the name but can't remember right now.
```

---
## \#52 Posted by: rich Posted at: 2017-09-02T23:52:59.644Z Reads: 102

```
[quote="Vanarian, post:51, topic:32035"]
The website has antispark in the name but can't remember right now.
[/quote]
http://www.antisparkheaven.com

The direct FET version looks interesting..... For now I have standard antispark switches with fuse running on 10s without problems. Do you know the continious rating for the 3 FET version? (standard is 60A, the 6 FET's version 160A). The only thing I don't like is that they come without switch and you can't buy switches in the shop.
```

---
## \#53 Posted by: Vanarian Posted at: 2017-09-03T00:08:45.591Z Reads: 92

```
Yup but if you want to get any custom switch it is better. Typical standard switch with Torqueboards anti spark for example is too big for my use (no offense here, his switches are very nice and will fit most boards).
```

---
## \#54 Posted by: rich Posted at: 2017-09-03T00:44:09.619Z Reads: 93

```
I know what you mean, custom switch is always better, but it takes time to find, order and receive the switch. Maybe he will offer different switches to choose and rename the page in antisparkswitchheaven :laughing:
I think this is slightly offtopic :joy:
```

---
## \#55 Posted by: Aborn Posted at: 2017-09-03T04:30:05.466Z Reads: 95

```
[quote="Vanarian, post:51, topic:32035"]
what will you choose? lol
[/quote]

I don't know man, so many options :stuck_out_tongue:

I think I'm either gonna get esk8.de's 20kv 6374 and then the whole drive system/pulleys and trucks there

Or

I'm gonna get a maytech 190 Kv 6374 with 8mm shaft and the drive system from Unikboards.com

Or

I'm gonna get a 8mm 200 Kv 6374 from @rich and pulleys trucks / drive system from unikboards.com

Ultimately I just want the best possible build plan before I start purchasing and lock out my possibilities.

Ultimately I want:

* 6374 motor with a (Kv + gearing) that will go around 45 km/h topspeed

* 15 mm timingbelt / pulley width

* Good looking solid aluminum pulleys and motor-mount

* In Europe

I think the closest thing to my ultimate is @rich 's 200 Kv 8mm bore 6374 motor with unikboards "smart series" drive system. It's aluminum and 15 mm. Looks very nice :) @okp 

[quote="Vanarian, post:51, topic:32035"]
For antispark, you can look for a member from here he built reinforced antisparks, multiple models
[/quote]

Honestly I'm not too concerned about antispark switches, they don't perform a very advanced task 

I'm not interested in a super fancy double upgraded heatsinked directfet 60€ switch

When a 25€ switch will do the exact same job just fine

Its a switch, it turns my board on. 

I'm confident that esk8.de's antispark switch will serve my build just fine. I'm gonna be pulling 160 amps. 60 max given the restriction on my bms. And the motors are rated at 60-65 max so I'm good. And not concerned.

My opinion, I could be wrong. But until I've encountered burning out a antispark switch, this is my opinion.
```

---
## \#56 Posted by: thisguyhere Posted at: 2017-09-03T04:31:11.589Z Reads: 84

```
Im Cackling like a lunatic over here...
```

---
## \#57 Posted by: Vanarian Posted at: 2017-09-03T17:22:35.428Z Reads: 77

```
For the upgraded anti-spark you should not overlook it because the standard Vedder one is good for 40A when no defects, based on 7530 heat dissipation. Past this level you either put separate cooling on the PCB or play Russian roulette. Once seen too many boards get problems because of fried antispark.

As I don't wanna have this problem I prefer to overbuild a bit. That's why 3 direct FETS sounds good to me!
```

---
