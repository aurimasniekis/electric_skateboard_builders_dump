# Dorian Wiskow eMTB Build - Trampa HolyPro 17, E-Toxx Belt Drive, Twin SK3 6374s, Twin MAX6 ESCs &amp; 6S 16,000mAh Lipo

### Replies: 59 Views: 6067

## \#1 Posted by: DWiskow Posted at: 2016-10-09T10:16:41.709Z Reads: 474

```
<img src="/uploads/db1493/original/3X/a/e/aeb5898f1c0c8cabeda36e9c04a29116409c289a.JPG" width="666" height="499">

I have recently completed an Electric Mountain Board build, which is based on the following equipment;

* 1 x Trampa HS11 Brake Deck (Holy Pro 35 with Magura hydraulic brakes)
* 1 x E-Toxx Trampa Motor Mount and 25mm Belt Drive System (6:1 Ratio)
* 1 x E-Toxx ESC/Receiver Mounting Plate with Traxxas Waterproof Receiver Box
* 2 x Hobbyking SK3 6374 192kv motors
* 2 x Hobbywing MAX6 ESCs
* 1 x Winning Remote/Receiver
* 1 x 6s 16,000 mAh HobbyKing MultiStar 10C Battery (I have bought a couple of these at only $80 each)
* 1 x B&W International 500 Waterproof Case

By the way, **_I want to publicly acknowledge Jens Kappel/E-TOXX who have a brilliant product and provide fantastic support/assistance to customers_** to help them get their project off the ground. If you intend to build anything like my eMTB, I recommend E-TOXX motor mounts and drive systems which are bullet proof and come complete with great instructions and every washer, bolt or screw you will need in comprehensively labeled separate plastic ziploc bags.

The entire board is completely waterproof and with the 8in/200mm pneumatic wheels can be ridden in any weather and on any surface (you just need to be careful on wet grass which is like ice). 

I weigh 120kg, so am no lightweight and wanted enough power to comfortably ride off-road and up hills . . . **_the speed and range measurements I have made are with my mountain board carrying 120kg of me !_**

I have both calculated and measured the speed of my eMountainBoard at 25-30 KPH or 16-19MPH (30KPH on a fully charged battery reducing to 25KPH as the battery voltage drops).

* <img src="/uploads/db1493/original/3X/d/7/d7ff5bed1fbc13ab84758a7225014086c29a84ed.png" width="460" height="120">

**_I found the acceleration/braking on the MAX6 ESC (set to punch 5, braking 100%) to be a little too abrupt and sharp, so I have developed a small board (hardware/software) to fit between the receiver and the ESCs that “manages” the rate of change (up or down) of the PWM signal . . . it has four different modes of operation (selected using a button on the board – with LED feedback to indicate mode)._**

* Mode 1 - pass through (no modification of any type to the PWM signal)
* Mode 2 - Slow (limits the maximum throttle to 50% and adds a ramp up/down curve to smooth any sudden acceleration/deceleration)
* Mode 3 - Eco (limits the maximum throttle to 70% and adds a ramp up/down curve to smooth any sudden acceleration/deceleration)
* Mode 4 - Fast (doesn’t limit the maximum throttle (i.e 100%), but adds a ramp up/down curve to smooth any sudden acceleration/deceleration)

The default mode is mode 4, which means I can slam full throttle on and, rather than throw me off, it smoothly accelerates to full speed . . . equally, I can slam full brake on (at maximum speed) and it will smoothly come to a stop . . . modes 2 & 3 are for learners and limit the top speed while providing even smoother acceleration/deceleration (really useful if you let people try the board for the first time). **This also means that in the event of signal loss from the hand held transmitter my board will simply reduce throttle and apply braking in a smooth manner (preventing any sudden stop that will usually throw the rider off the board)**. This reduces the risk of accidents and makes it extremely smooth and easy to ride !

I have recorded the performance over a number of rides and am experiencing a 17-20 kilometer or 10-12 mile range with this set up and my 6S 16,000mAh battery (so with a second/spare battery in my backpack can easily achieve overall 30-40km distance).

* <img src="/uploads/db1493/original/3X/f/5/f536a54fbed70fdadb30ecd20671c061e9caa602.png" width="330" height="130">

The 10C 16,000mAh battery is able to put out 22-25 volts at 160 amps, so has plenty of power to drive the motors (even with my 120kg on board). Obviously, I could increase the performance and overall speed of the board to 40KPH/25MPH by moving to an 8s battery, but frankly the current 30KPH/20MPH delivered by the 6S battery is plenty for me at the moment (and the battery from HobbyKing is a bargain at only $80).

I am currently running with the Yellow (65 shore) Dampas and the springs only very lightly loaded to get maximum turning from the trucks. This means I need to continue to develop my balance and/or reduce speed when I experience high speed wobbles. I have tried both loading the springs and fitting the Green (75 shore) Dampas, but feel I lose some of the control (steering) of the board at lower speeds.

<img src="/uploads/db1493/original/3X/7/5/756b17c597d89a92a9128f800c90f2e0e71619b4.JPG" width="666" height="499">
_Magura hydraulic brakes – mechanical backup in case things go wrong !_

<img src="/uploads/db1493/original/3X/1/7/17dfac2c614af80898c9327701b1a98addd0719a.JPG" width="666" height="499">
_Waterproof MAX6 ESCs, Receiver in Traxxas Waterproof Box, plus my **Magic PWM Manager**_

<img src="/uploads/db1493/original/3X/b/1/b1cb4782631610a2421803bb647c2aa105703a9c.JPG" width="666" height="499">
_E-Toxx Motor Mount & 6:1 25mm Belt Drive_

<img src="/uploads/db1493/original/3X/b/0/b0b6e9a45288c9ebe1332476f1efc1408c2db67d.JPG" width="666" height="499">
_B&W International 500 Waterproof Case holding Battery, Remote, Keys etc_

<img src="/uploads/db1493/original/3X/7/1/71948159cc7ce079c4e0e3544fcc0c7c74925e1d.JPG" width="666" height="500">
_HobbyKing 6S 10C 16,000mAh Battery, Winning Remote, Wallet, Keys, etc_

<img src="/uploads/db1493/original/3X/e/0/e06380a77fb5d1766030ac3e6cc89d752d213440.JPG" width="666" height="500">
_Battery wiring to Speed Controllers & Electronics_

<img src="/uploads/db1493/original/3X/b/8/b82de6ed73a965841c104fe174305f88741539a1.JPG" width="666" height="500">
_Battery wiring & two way splitter using XT90s with MAX6 ESCs Soft Start Power Switches_
```

---
## \#2 Posted by: kyo Posted at: 2016-10-09T10:46:47.340Z Reads: 336

```
wow thats a beast. but the brake thing, i wish somehow you hook it up with a servo and control it wirelessly , thats would be awesome :D :D :D :D
```

---
## \#3 Posted by: DWiskow Posted at: 2016-10-09T11:03:01.517Z Reads: 331

```
I do control it wirelessly . . . using the Winning Remote Controller (which provides brake and accelerator control) . . . the Magura Hydraulic Brakes are deliberately a completely independent mechanical system (because sh*t happens) and I always like to have a 'Plan B'
```

---
## \#4 Posted by: kyo Posted at: 2016-10-09T11:22:26.905Z Reads: 322

```
Soooo you are riding two hands?? Does that feel weird?
```

---
## \#5 Posted by: DWiskow Posted at: 2016-10-09T11:43:00.098Z Reads: 312

```
No not weird . . . I am left handed and ride goofy . . so wireless remote in left hand (at the rear of the board & close to the receiver), and hydraulic brake lever loosely held in right hand (just in case it is needed).

It also makes it really easy to mount and adjust the feet bindings when on a hill . . . I just hold the board with the hydraulic brake while I get my feet in and adjust the bindings.
```

---
## \#6 Posted by: DilatedPupils Posted at: 2016-10-09T13:07:03.502Z Reads: 296

```
Nice!
Interested in your "magic PWM manager". Looks like it could be the solution to having a beginner mode on builds.
You don't have any problems with your multistar with it being just 10c?
```

---
## \#7 Posted by: DWiskow Posted at: 2016-10-09T13:33:34.473Z Reads: 298

```
10C would definitely be a problem if the battery were smaller capacity, but 10C on a 16,000mAh battery means that it can deliver a constant 160amps . . . my motors are SK3 6374s which pull a maximum current of 80amps and can handle a maximum voltage of 44volts . . . so 2 x 80amps = 1 x 160amps which means this battery can supply all the juice the motors can consume (and it is relatively small and inexpensive, so you can easily carry a spare or two and charge via a normal RC balanced charger)

By the way, these two motors can produce up to 2,750 watts of power each . . . That's 5,500 watts or a little over 7 horesepower . . . plenty  to haul me along at more speed than I can handle !

With respect to my Magic PWM Manager, you are absolutely right, mode 1 & 2 are perfect for beginners or children where **_the risk of injury (or loss of confidence) is serious given the power and instant acceleration/braking eBoards are capable of delivering_** . . . I wouldn't discount the stress it takes out of full power either. Knowing that **an inadvertent 'nudge' on the remote when going over rough ground or a sudden loss of signal is enough to throw you off the board and hurt you**, really reduces the enjoyment when out riding. **_My Magic PWM Manager removes all of that anxiety and risk by delivering a buttery smooth experience when either accelerating or braking_**.
```

---
## \#8 Posted by: Monte Posted at: 2016-10-09T13:54:33.587Z Reads: 271

```
What range do you get from that brick?
```

---
## \#9 Posted by: DilatedPupils Posted at: 2016-10-09T14:04:52.785Z Reads: 265

```
Are you gonna be making your magic pwm manager available to the community?
```

---
## \#10 Posted by: DWiskow Posted at: 2016-10-09T14:43:35.522Z Reads: 266

```
Range is detailed in my original build post . . .10-12 miles or 17-20 kilometers.
```

---
## \#11 Posted by: DWiskow Posted at: 2016-10-09T14:44:26.596Z Reads: 255

```
I would need to work out how best to do that, but if there is enough interest then definitely.
```

---
## \#12 Posted by: EssEnn Posted at: 2016-10-09T15:33:38.998Z Reads: 257

```
Love the build! Looks sweet! I'm loving the disc brakes as well. It has even crossed my mind recently to add that to my build. We will see.

I think your Magic PWM manager is a fantastic idea. I have been worried about any of my friends trying my board as it is hard to describe how sensitive these controllers are until you actually try it yourself. That along with the crazy amount of grip and torque as I found out by stacking it hard the first time lol. 

I don't know how it works but would it be possible to have 2 control knobs, one to control max speed and one for ramp up/ramp down aggression between throttle states? Sorry I'm just thinking out loud, its just got my mind thinking...

Really good work btw!
```

---
## \#13 Posted by: DWiskow Posted at: 2016-10-09T23:18:21.258Z Reads: 253

```
@EssEnn I guess you need to think of the one I built as a prototype . . . you are on the right track regarding having a setting for speed an another for the acceleration/braking curves . . . I 'fixed' the speed setting by allowing four modes;

* Pass Through - that changed nothing
* Slow - 50% throttle and ramp up/down curves applied
* Eco - 70% throttle and ramp up/down curves applied
* Fast - 100% throttle and ramp up/down curves applied

Interestingly, I found that different curves were required for each mode . . . and the acceleration and braking curves also needed to be different . . . both the maximum speed/power in each mode and the curves are likely to be personal preference though.

Doing this was easy on my prototype, I just adjusted the software accordingly . . . to make this general purpose and allow individual adjustments to be set requires a bit more thought about the user interface, particularly if the device is to be located inside an enclosure with limited access.

I will have a play and see what is possible.
```

---
## \#14 Posted by: EssEnn Posted at: 2016-10-09T23:44:14.922Z Reads: 249

```
@DWiskow I keep having idea's about this so I'm going to just throw them out there if you don't mind. I just like brain storming but if i'm annoying just say and I'll shut up. 

To have something that was adjustable by the user could you not have a pot like the one below to adjust variables such as max throttle and ramp rate

http://i.stack.imgur.com/d0h2U.jpg

And then just switch between the 4 modes that would have different ramp curves? 
Also would it be possible to have the fast mode always start from neutral? So lets say you go full throttle and then full reverse, can the ramping be instant to neutral and then the curve applied during the braking and visa versa? 

Are you using an Arduino?
```

---
## \#15 Posted by: DWiskow Posted at: 2016-10-10T04:09:56.346Z Reads: 230

```
@EssEnn Your instinct is right about 'starting from neutral' and that is the way my code already works . . . not sure regarding the use of pots, if the board is installed in a location that is not readily accessible (e.g. inside an enclosure).
```

---
## \#16 Posted by: barajabali Posted at: 2016-10-10T05:07:47.133Z Reads: 231

```
Very nice build. Clean simple effective. Post a video!

How are the brakes? I'm thinking about installing some on my mountain board since I'm strapped in and can't bail if I need to. I almost got hit by a car. Held onto a stop sign for dear life.
```

---
## \#17 Posted by: EssEnn Posted at: 2016-10-10T10:51:35.040Z Reads: 227

```
I don't see any issue mounting pots in an enclosure to adjust parameters. Thing is, can it be done?

I'm totally in helping out where ever I can with this as I think it is a great idea. Do I need to learn to program an Arduino? How can I help? I got loads of ideas at least
```

---
## \#18 Posted by: EssEnn Posted at: 2016-10-10T11:12:39.070Z Reads: 226

```
Lucky in the UK I can't ride on the roads or pavements. Well I can but police would not be happy about it and take the board. Not worth the risk. 

Still I have been thinking about the brake kit as it looks sick as well as giving an option to stop if things go wrong.
```

---
## \#19 Posted by: benjammin Posted at: 2016-10-10T19:00:09.934Z Reads: 215

```
Dude... you guys are freaking me out :grinning: Do these things really just take off, and/or lockup unexpectedly? :fearful: 

@barajabali Why did you have to hang onto a stop sign?
```

---
## \#20 Posted by: smudgeUK Posted at: 2016-10-10T19:16:10.209Z Reads: 216

```
Really nice work @DWiskow !! I like it!
Im not sure i saw a response to the question of whether you are using arduino to control the acceleration?
This is something that could really allow friends/family to safely experience an emtb ... would you mind sharing your code?
Keep up the good work !!
```

---
## \#21 Posted by: barajabali Posted at: 2016-10-10T19:59:39.326Z Reads: 202

```
No they're super reliable it's just that they need breaks other than motor breaks. The motors will just slow them down to a slow jog but they don't stop. And you can't put your foot down to stop
```

---
## \#22 Posted by: DWiskow Posted at: 2016-10-10T20:39:54.747Z Reads: 202

```
@smudgeUK I am not using an Arduino, but that should be possible. I am using a 32bit uprocessor and programming in python
```

---
## \#23 Posted by: smudgeUK Posted at: 2016-10-10T20:43:12.727Z Reads: 193

```
@DWiskow ok thanks for the info. Im not familiar at all with python though at the end of the day, code is code :-) maybe i'll look into the arduino project once my current project is complete.
Keep us updated with your progress, this sort of thing is really interesting!
I can see wheelie control and launch control coming in the not too distant future ;-)
```

---
## \#24 Posted by: EssEnn Posted at: 2016-10-10T23:01:16.660Z Reads: 196

```
I thought it would be an Arduino as it has a RC servo library already (I did a little research after reading this thread) and there are a few easy ways to read the inputs it seems.

@benjammin there is a lot of torque, a 6:1 reduction and a lot of grip. Its not hard to have the front of the board lift up or just shoot out from under you.  Mine does not accelerate, it just changes speed almost instantly. Its quite easy to squeeze the trigger a little too hard or hit a bump and before you know it you are looking at the sky. 

@smudgeUK there are a lot of possibilities with something like this. You could even put sensors on the front wheels and have some kind of traction control. 

 @DWiskow I'm loving your idea. Please keep on developing your little box!
```

---
## \#25 Posted by: smudgeUK Posted at: 2016-10-10T23:05:11.266Z Reads: 185

```
What signal is sent from the receiver to the esc? is it 0-5v?

*Edit - i dont want to hijack your build thread @DWiskow - if you'd prefer us to discuss this elsewhere id be happy to make a new thread
```

---
## \#26 Posted by: rodriguejoe1 Posted at: 2016-10-11T00:26:01.745Z Reads: 189

```
[quote="barajabali, post:16, topic:10859"]
Held onto a stop sign for dear life
[/quote]

So what brakes are out there for a trampa besides magura? Since holding on to a stop sign seems a little painful.. plus that means we would need to wear a jock strap too just in case..
```

---
## \#27 Posted by: Mobutusan Posted at: 2016-10-11T00:37:12.531Z Reads: 189

```
Are there any options for a channel 2 operated disc brake or something? I could see having the wheel on the GT2B or mini remote working the brake for full stops or emergencies, and trigger for throttle control.
```

---
## \#28 Posted by: barajabali Posted at: 2016-10-11T00:43:36.255Z Reads: 186

```
Hahah yea true.

From my knowledge Magura brakes are the only ones made for trampa.
```

---
## \#29 Posted by: rodriguejoe1 Posted at: 2016-10-11T01:01:53.217Z Reads: 185

```
ok. thanks...
```

---
## \#30 Posted by: EssEnn Posted at: 2016-10-11T09:03:43.432Z Reads: 182

```
@DWiskow yeah, sorry to hijack your thread like this. Maybe a good idea would be to start a thread in the electronics sub? This is the problem with great ideas....
```

---
## \#31 Posted by: Okami Posted at: 2016-11-27T20:30:53.131Z Reads: 167

```
@DWiskow Are you still visiting  this forum .. ? 

Could you share some more details on how you made that throttle ramp module?

I think there are a couple of people who would like to find more about it!
```

---
## \#32 Posted by: 2Old2Sk8 Posted at: 2017-06-03T00:18:42.270Z Reads: 144

```
[quote="barajabali, post:21, topic:10859, full:true"]
No they're super reliable it's just that they need breaks other than motor breaks. The motors will just slow them down to a slow jog but they don't stop. And you can't put your foot down to stop
[/quote]

Sorry to revive an old thread but I am new to electric mountain boards and I am confused by this statement.  This is the first board I have seen with mechanical 'backup' brakes.  If the ESC break doesn't really work how is everyone else able to stop?  I have heard that the ESC brake can work too well and send people over the front of the board if they are not ready for it...
```

---
## \#33 Posted by: davewood1982 Posted at: 2018-03-25T22:14:03.003Z Reads: 107

```
Did you need some kind of adapter to connect the SK3 6374 motors to them MAX6 ESCs?
```

---
## \#34 Posted by: tricky-fpv Posted at: 2018-07-14T10:08:28.391Z Reads: 92

```
Hi there. I am extremely impressed with your build. Is there any way u can send me a parts list with all the parts that you bought and the total price. And where to order them if possible. I am really intressed in building a board like yours. Cheera
```

---
## \#35 Posted by: telnoi Posted at: 2018-07-14T13:36:07.345Z Reads: 92

```
All the parts are listed already/post #1.
Prices will depend on location, immediate availability (or not...how are we supposed to know in how much of a hurry you are) and if the parts are even available after two years time. This is an old build.

I'd start here though. Good luck. 

https://shop.elektro-skateboard.de/eigenbau-tuning/e-toxx/219/e-toxx-carbon-rc-platte?c=22
```

---
## \#36 Posted by: tricky-fpv Posted at: 2018-07-14T13:49:34.738Z Reads: 83

```
Thanks mate.
Why is the carbon plate so expensive?
I fly freestyler fpv drones higest qaulity carbon and whole frame is 100bucks. 
And thats with a lifetime warranty
```

---
## \#37 Posted by: telnoi Posted at: 2018-07-14T13:59:18.018Z Reads: 80

```
Because e-toxx doesn't mass produce somewhere in Asia ;) you'll find esk8 stuff more expensive that drone parts, simply because for some items mass production doesn't make sense/the market is much smaller. 

It's a simple design though. With a bit of cad knowledge and good measurements you can have something similar cut by someone else.
```

---
## \#38 Posted by: tricky-fpv Posted at: 2018-07-14T14:02:50.805Z Reads: 80

```
How about 3d print. 
Anybody do it that way?
Is there a cad design flying around here perhaps.
I am planning on running 12s for sure
And i saw the turnigy motor for 86bucks at hobbyking. Are these any good.
And as for the board. We have a second hand site over here in holland with bits and bobs and i saw fair amount of mountain boards from 75euros to 299.
What should i keep am eye on?
Can u use any kind of offroad board?
Btw thanks for the tips and info dude
```

---
## \#39 Posted by: tricky-fpv Posted at: 2018-07-14T14:10:15.888Z Reads: 79

```
What was the totaal cost of the build if i may ask
```

---
## \#40 Posted by: FredrikHems Posted at: 2018-07-14T15:46:06.680Z Reads: 81

```
I cant say for sure, but I would have guessed around $2000
```

---
## \#41 Posted by: tricky-fpv Posted at: 2018-07-14T15:54:15.237Z Reads: 79

```
Darn was hoping around 1200euroish
```

---
## \#42 Posted by: Nemesis Posted at: 2018-07-14T16:16:47.772Z Reads: 85

```
This is a visual representation of previously made Eskate "budget" plans... :joy:
 ![budget%20plans|605x403](upload://xJqz5byoWpR84dYskEQNCKPrqwg.jpg)
```

---
## \#43 Posted by: telnoi Posted at: 2018-07-14T17:06:26.792Z Reads: 85

```
What you should be looking out for depends on your budget really. Since you're Dutch, things are a bit easier (no significant hills to climb) 

* your target speed. It will determine the motor kv, gearing and voltage. 
* your weight. Pretty much the only board that comes with custom PLY (amount of layers) is trampa. Hard to find second hand. If the board is for light weights and your target speed is beyond 30 km/h there is an increased risk in speed wobbles.
* 3D prints. Yes, of course possible. I mount my dual focbox with a 3d printed slab. Check thingiverse. Only issue is mounting holes for your specific board. Pays off to learn fusion 360.
* Turnigy Sk8. There's a thread here discussing these. They apparently have no circlip, motor can could separate (you know how it is with drone motors) 
* an excellent board will indeed cost more than 1500 euro

If you get second hand, make sure you get trucks for which motor mounts are actually available. Forum member idea sells mounts for a fair number of boards. Search his thread.
```

---
## \#44 Posted by: tricky-fpv Posted at: 2018-07-14T17:36:25.351Z Reads: 84

```
Hahahahhaha ok ok i have to admit i love the humor allready here lol.
I live in holland yep correct but i am british. Cup of tea. Fish and chips ect ect hahahah.
But yes a budget between 1100 to 1500 euros give or take.. i do want a twin motor setup. Hugh insane speed i dont want. If it goes 40kph i will be happy
```

---
## \#45 Posted by: tricky-fpv Posted at: 2018-07-14T18:27:56.966Z Reads: 87

```
![Screenshot_20180714-202524_Marktplaats|281x500](upload://n0eQQPugqc1ZC8BkyX9XaBRHJdz.jpg)

How about this board?
```

---
## \#46 Posted by: telnoi Posted at: 2018-07-14T19:06:25.837Z Reads: 84

```
Yah, seems popular to move east or something. I am Dutch but live in Germany. 

As for the board, depends on the PLY of the deck and your weight. If you want to keep eating fish and chips, maybe go for 16 Ply. 
Also, figure out what hubs and trucks those are and search for a complete belt drive that fits. That's where the fun starts or ends. 

Typically, it's easy to find a drive train for MBS matrix 2 + rockstar hubs, trampa infinity/vertigo + superstar hubs. Everything else is a bit more exotic.

Think of the following. All hubs have their own bolt pattern and the trucks have their own profiles. There aren't that many universal drive trains out there.
```

---
## \#47 Posted by: tricky-fpv Posted at: 2018-07-14T19:20:32.983Z Reads: 84

```
Well my wieght is max 65-70kilos
So think this board would be fine for my light ass.
As for trucks i will ask what ones thay are dude thanks
But the board is the correct one?
```

---
## \#48 Posted by: tricky-fpv Posted at: 2018-07-14T19:24:34.654Z Reads: 88

```
![Screenshot_20180714-212222_Marktplaats|281x500](upload://aCcQ9K42KYAUuqUxznJuAXMmLGs.jpg)those are the wheels
```

---
## \#50 Posted by: tricky-fpv Posted at: 2018-07-14T20:38:03.284Z Reads: 87

```
Ok found out what trucks thay are

15 ply, and vector trucks from MBS,  twistar hubs from mbs
```

---
## \#51 Posted by: telnoi Posted at: 2018-07-14T21:10:11.930Z Reads: 82

```
You'll have to do the searching yourself, but apparently there have been (maybe still are) few members who converted those trucks and offered motor mounts for them.

15 Ply should be ok.
```

---
## \#52 Posted by: tricky-fpv Posted at: 2018-07-15T10:45:43.952Z Reads: 79

```
Thanks telnoi i do appreciate the feedback. As a beginner its hard to figure out whats right and not so really big thumbs up man
The board is good then
If need be i can allways get other trucks to fit the board.
Thanks dude.
```

---
## \#53 Posted by: tricky-fpv Posted at: 2018-07-16T14:10:18.191Z Reads: 73

```
Small update and question 
Found these at trampboards.
Can i use these for the e toxx sytems?
Mini diŕect drive?
And compatable with the trampa board i posted above

![20180716_160749|666x500](upload://s53wpHciEfhxnY018Ms4vBxNr6r.jpg)
```

---
## \#54 Posted by: telnoi Posted at: 2018-07-16T15:20:46.671Z Reads: 70

```
[quote="tricky-fpv, post:52, topic:10859"]
If need be i can allways get other trucks to fit the board.
[/quote]

Doesn't look like it's 35 degree like trampas' holypro and 35 long/short. That will have an impact on stearing and stability if you get infinity or ultimate trucks.

The minidrive has a ratio geared for speed rather than torque, so you will be somewhat limiting the off-road capabilities. The mini drive is usually paired with trampa gummies.

PS. The axle width/diameter will also be different, thus if you want to keep those wheels and hubs you'll probably need a sleeve to make the bearings fit. Probably some spacers too.

My advice. If you don't like those trucks, don't get the board.
```

---
## \#55 Posted by: tricky-fpv Posted at: 2018-07-16T16:00:59.118Z Reads: 63

```
Mmh getting more complicated as i read more and more:-(
Isnt there a list anywhere here of compatible parts for a general setup and where to order them?
I have seen the trampboard site but i prefer the e toxx rear drive direct drive to be honest
```

---
## \#56 Posted by: FredrikHems Posted at: 2018-07-16T16:04:22.982Z Reads: 67

```
Buy a trampa board from them and pair it with etoxx drives, no? :grinning:

Edit: You should start your own thread where you could ask questions and such, instead of asking in this one. Many of the questions is pretty irrelevant to this topic. :wink:
```

---
## \#57 Posted by: tricky-fpv Posted at: 2018-07-16T16:10:16.349Z Reads: 66

```
Cant start my own thread yet as i am fresh meat:-(
```

---
## \#58 Posted by: FredrikHems Posted at: 2018-07-16T16:31:38.110Z Reads: 66

```
I guess you should read more then :grinning: It will help answering alot of your questions too.
```

---
## \#59 Posted by: telnoi Posted at: 2018-07-16T17:03:22.032Z Reads: 66

```
The direct drive is only compatible with a certain deck shape. Since they are no longer selling the Hs11 deck, that means the holypro 35. You can also get a 35 long or short, but you would have to cut the tail with a pendulum saw or something/metal blade.

The toxx drive is compatible with infinity or vertigo trucks and superstar hubs only.

All in all expensive.
Cheapest complete board around 520 Euro, direct drive around 500, motors around 280, speed Controllers around 320, speed controller enclosure around 50, lipos around 350. Random crap around 100 Xtra (connectors, loctite, lipo checkers, cables, velcro).
```

---
## \#60 Posted by: Ghost1068 Posted at: 2019-03-20T15:05:13.901Z Reads: 31

```
Beautiful build! I am looking to do a very similar build; Trampa Board, E-toxx mini direct drive, 6374 dual motors, Flipsky 6.6 dual Vesc, however I am really unsure of how I want to do the batteries and case. Most likely a top mount for the durability. With LiPo's what kind of range are you getting? What kind of speed are you getting on this board build/ what kind of acceleration? And do you get any voltage sag??

Thank you!
```

---
