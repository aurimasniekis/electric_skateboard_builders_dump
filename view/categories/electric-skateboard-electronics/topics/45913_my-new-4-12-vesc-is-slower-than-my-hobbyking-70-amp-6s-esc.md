# My new 4.12 vesc is slower than my hobbyking 70 amp 6s esc?

### Replies: 79 Views: 1595

## \#1 Posted by: Gabegds2001 Posted at: 2018-02-08T22:22:13.823Z Reads: 226

```
My new 4.12 vesc is slower than my hobbyking 70 amp 6s esc?? I was pretty sure I set all of the amperages right and set my motor to it's max output (70amp)..  I wonder why it's slower.. plus my old setup was 6s and my new one is 12s. If you have any suggestions please help 😥
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2018-02-08T22:23:34.813Z Reads: 224

```
Can ypu post more Info abouth your board, and maybe some screenshot of your parameter in the bldc tool
```

---
## \#3 Posted by: Gabegds2001 Posted at: 2018-02-08T22:27:12.550Z Reads: 225

```
Here's my setup: two 6s zippy compact 5000mah 60c batteries in parallel
4.12 Benjamin vedder vesc 
Turnigy aerodrive sk3 149kv 
16T motor pulley
36t wheel
orangatang kegel 83mm 
I'm using the vesc tool version .87
For the moment I cannot show you a pic my parameters and settings on my computer because I'm not at home.. will post later.
```

---
## \#4 Posted by: GrecoMan Posted at: 2018-02-08T22:28:07.957Z Reads: 214

```
two 6s 5AH in parallel = 6s 10AH, not 12s.
```

---
## \#5 Posted by: Gabegds2001 Posted at: 2018-02-08T22:29:10.621Z Reads: 209

```
Ob my bad lol I didn't realize that
```

---
## \#6 Posted by: FredrikHems Posted at: 2018-02-08T22:29:27.749Z Reads: 210

```
You said you were running a 12s setup..? That is a 6s setup :upside_down_face:

149kv at 6s wont Get alot of speed
```

---
## \#7 Posted by: GrecoMan Posted at: 2018-02-08T22:29:49.865Z Reads: 205

```
yea...

6s/149kv will be extremely slow no matter what esc you use 🤣
```

---
## \#8 Posted by: Gabegds2001 Posted at: 2018-02-08T22:37:22.485Z Reads: 196

```
Alright guys I'm new lol anyway I just wanted to know why with two batteries rather than one would be slower than before.. especially with a new vesc. Before I could go 18mph and now I go about 14mph, what's the deal!?!j
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2018-02-08T22:40:04.414Z Reads: 192

```
Post your setting and it will be alots more easier to help you 😉
```

---
## \#10 Posted by: pennyboard Posted at: 2018-02-08T22:47:13.628Z Reads: 187

```
[quote="Gabegds2001, post:3, topic:45913"]
two 6s zippy compact 5000mah 60c batteries in parallel
[/quote]


Connect these in Series and you should get a top speed of about 28 MPH


[quote="GrecoMan, post:4, topic:45913, full:true"]
two 6s 5AH in parallel = 6s 10AH, not 12s
[/quote]

What's got me intrigued about this, is that if he connected them in parallel and is running 6s, the board shouldn't even move if he set up the voltage cutoff for 12s in BLDC tool. @Gabegds2001 Probably best if you post your settings cause there's a high chance your current voltage cutoff will destroy your batteries if you connect them in series
```

---
## \#11 Posted by: Gabegds2001 Posted at: 2018-02-08T22:49:42.385Z Reads: 173

```
I'm doing parallel because I want more range but if 14mph is going to be my top speed then that may be my option
```

---
## \#12 Posted by: ZackoryCramer Posted at: 2018-02-08T22:50:24.787Z Reads: 172

```
Here's a quick break down of how speed is estimated:
**premise**: No mechanical parts are changed
higher the voltage (# of series) = higher the potential for top speed
higher the current (# of c) = the more "power" to fufill that speed
Your speed will be capped by voltage regardless.
Rearranging the same packs does not change the range
```

---
## \#13 Posted by: pennyboard Posted at: 2018-02-08T22:50:43.283Z Reads: 168

```
Series and parallel will give you the same range. Range is determined by Watt hours. Watt hours are determined by battery capacity and battery voltage. So connecting in parallel to get 6s doubles the capacity but halves the voltage. So you don't gain any range.
```

---
## \#14 Posted by: Gabegds2001 Posted at: 2018-02-08T22:52:47.865Z Reads: 166

```
Well crap I guess I messed up buying a parallel connector.... @GrecoMan it's probably working with the 6s in parallel because I used a "setup wizard" option and it probably automatically set the right cutoff.
```

---
## \#15 Posted by: pennyboard Posted at: 2018-02-08T22:54:08.042Z Reads: 162

```
Ah that makes sense. Deffinetly post your settings before you ride it again so that we can check them over and make sure you don't blow your board

Also if you have soldering iron, wire, and heat shrink, you can change a parallel connector to a series pretty easily
```

---
## \#16 Posted by: Gabegds2001 Posted at: 2018-02-08T22:55:31.915Z Reads: 160

```
Ok thanks ill wait till I get back home to take pictures. I do have the right equipment to make it a series connector 
too
```

---
## \#17 Posted by: ZackoryCramer Posted at: 2018-02-08T22:55:47.137Z Reads: 153

```
I used to fix my xt90 to xt 60 converter all the time since they were abridged only by solder. Just munny wrap it in electrical tape afterwards. :joy:
```

---
## \#18 Posted by: GrecoMan Posted at: 2018-02-08T23:17:03.240Z Reads: 149

```
[quote="ZackoryCramer, post:12, topic:45913"]
higher the voltage (# of series) = higher the potential for top speed
[/quote]

no dude...
I can get the same speed with a 6s config and a 12s config. speed is mainly based around kV to voltage “ratio”. i don’t mind you embarrassing yourself, but when you start spreading fake facts it’s a different story.
```

---
## \#19 Posted by: ZackoryCramer Posted at: 2018-02-08T23:24:38.397Z Reads: 145

```
[quote="GrecoMan, post:18, topic:45913"]
I can get the same speed with a 6s config and a 12s config
[/quote]

I said the potential for speed. Doesn't mean you have to go at that speed. Speed is theatrically in direct relation to the product of kv and voltage. Yes, you don't have to operate a motor at full 12s voltage even though your battery is capable of supplying it.

[quote="GrecoMan, post:18, topic:45913"]
kV to voltage “ratio”
[/quote]

You lost me there. Are you saying kv/voltage? Isn't kv already rpm/volt? 
Yes, I made assumptions that everything but the battery pack is the same.

[quote="GrecoMan, post:18, topic:45913"]
i don’t mind you embarrassing yourself
[/quote]

I don't either if I and someone else can learn from it.
```

---
## \#20 Posted by: GrecoMan Posted at: 2018-02-08T23:29:27.682Z Reads: 131

```
[quote="ZackoryCramer, post:19, topic:45913"]
You lost me there. Are you saying kv/voltage? Isn’t kv already rpm/volt?
[/quote]

if I meant rpm/volt I would’ve said it.

for example, I can get very close to (if not more) the speed a setup with 12s/159kv with a 6s/270kv. the big thing that voltage changes is torque. 12s/159kv will have noticeably more torque.
```

---
## \#21 Posted by: ZackoryCramer Posted at: 2018-02-08T23:33:50.920Z Reads: 120

```
I realized just a bit before you responded. I think you took into account the change of mechanical setup. I made the assumption of only changing the battery pack and nothing else. Yes, more precisely, changing the gear ratio changes the speed and recalibrates the factor in calculating the speed.
Changed it, it's all good. :hugs:
```

---
## \#22 Posted by: Pedrodemio Posted at: 2018-02-08T23:42:33.536Z Reads: 117

```
[quote="GrecoMan, post:20, topic:45913"]
the big thing that voltage changes is torque
[/quote]

Wrong, torque is directly proportional to current, not voltage, but as your speed increase (same everything) the back EMF of the motor also increase, so you need more voltage to offset that and be capable of pushing the needed current into the motor, with more voltage you can keep the torque for a broader range, which is exactly why you go faster with more voltage, but the torque is the same (perfect world) if   the current into the motor is the same, no matter the voltage
```

---
## \#23 Posted by: GrecoMan Posted at: 2018-02-08T23:45:02.516Z Reads: 114

```
yea sorry, I meant if voltage and kv were kept to the same “ratio”

ex.
6s/270kv will have less torque than 12s/149kv
```

---
## \#24 Posted by: Gabegds2001 Posted at: 2018-02-08T23:46:47.963Z Reads: 108

```
So, should I make a series connector or should I keep the parallel connector if I want more speed?
```

---
## \#25 Posted by: Pedrodemio Posted at: 2018-02-08T23:47:27.388Z Reads: 105

```
You mean keeping the top speed the approximately same with booth these setups?
```

---
## \#26 Posted by: GrecoMan Posted at: 2018-02-08T23:54:10.521Z Reads: 103

```
yea, speed will be approx. the same, but 12s will have more hill climbing and acceleration capability
```

---
## \#27 Posted by: Gabegds2001 Posted at: 2018-02-09T00:00:28.697Z Reads: 103

```
Ok I'll keep the parallel setup for now let me pull up the parameters on my pc
```

---
## \#28 Posted by: Tuomalar Posted at: 2018-02-09T00:02:31.336Z Reads: 102

```
No. Go with series. Gregoman answered to earlier question. Your high speed will rise if you add some voltage and keep your motors as they are
```

---
## \#29 Posted by: Gabegds2001 Posted at: 2018-02-09T00:03:14.932Z Reads: 101

```
Ok I'm getting a lot of different opinions but I guess I'll try series after I show you guys my vesc tool .87 settings
```

---
## \#30 Posted by: Tuomalar Posted at: 2018-02-09T00:04:22.879Z Reads: 99

```
And please do a lot of research. There are hundreds of similiar conversations like this so you can learn by yourself.
```

---
## \#31 Posted by: Gabegds2001 Posted at: 2018-02-09T00:09:04.880Z Reads: 103

```
![1518134894472500575719|375x500](upload://cPKa4TlT8RCMq5Gnh8YUwtFO57M.jpg)What should I set my battery max to if my batteries are. 5000mh 6s 60c?
```

---
## \#32 Posted by: GrecoMan Posted at: 2018-02-09T00:12:53.973Z Reads: 100

```
did you do ppm detection?
```

---
## \#33 Posted by: Gabegds2001 Posted at: 2018-02-09T00:17:06.840Z Reads: 99

```
I thought so. I can retry it .
```

---
## \#34 Posted by: Gabegds2001 Posted at: 2018-02-09T00:20:21.990Z Reads: 101

```
![15181355973811117127927|375x500](upload://saj3by0Ux9zTwNXFJSdlpOoWOOp.jpg)With two 6s in parallel i set the cell count to 6s right?
```

---
## \#35 Posted by: GrecoMan Posted at: 2018-02-09T00:24:08.721Z Reads: 96

```
yes. was it set to 12 before?
```

---
## \#36 Posted by: Gabegds2001 Posted at: 2018-02-09T00:32:16.682Z Reads: 96

```
Yes it was. I went through the motor and app configuration setup one more time and after doing test on the motor and writing the results to the vesc, the motor sounds different.
```

---
## \#37 Posted by: GrecoMan Posted at: 2018-02-09T00:39:46.560Z Reads: 95

```
yea that was your problem. try it now.
```

---
## \#38 Posted by: Gabegds2001 Posted at: 2018-02-09T00:45:56.352Z Reads: 97

```
It's too dark now lol. I'm gonna try making a series connector with my bad soldering skills
```

---
## \#39 Posted by: ZackoryCramer Posted at: 2018-02-09T00:48:38.562Z Reads: 96

```
Make sure you use lots of solder and cover as much area as possible so heat doesn't build up when you apply a lot current through the connection.
```

---
## \#40 Posted by: Pedrodemio Posted at: 2018-02-09T01:08:06.675Z Reads: 93

```
Them yes, if you used the same motor and same gearing the torque would be the same no matter the voltage, but in this case you give up torque to keep the top speed high. If your 270kv motor could handle double the current of 149kv one them they would be equal

The problem is that until the community dynamometer takes off, all this assume 100% efficiency all the time
```

---
## \#41 Posted by: Gabegds2001 Posted at: 2018-02-09T03:21:14.150Z Reads: 87

```
Alright guys I made a ghetto series connector and GEEZ is it fast... Too fast in fact. No way I'm going to be able to ride it without falling off trying to control the throttle smoothly. Anyone know how to make the throttle not so sensitive?
```

---
## \#42 Posted by: ARetardedPillow Posted at: 2018-02-09T03:34:10.218Z Reads: 88

```
Make sure you don't use too much solder and not cover "as much area as possible"?

Make sure to heat up the wires/connectors and let the solder "flow" into the joint. And use flux, if you don't have flux use rosin core, and leaded solder, lead free solder is a pain in the ass.
```

---
## \#43 Posted by: SOICDIP Posted at: 2018-02-09T03:34:12.288Z Reads: 89

```
[quote="Gabegds2001, post:41, topic:45913, full:true"]
Alright guys I made a ghetto series connector and GEEZ is it fast… Too fast in fact. No way I’m going to be able to ride it without falling off trying to control the throttle smoothly. Anyone know how to make the throttle not so sensitive?
[/quote]

You can map the throttle in VESC tool.
```

---
## \#44 Posted by: ARetardedPillow Posted at: 2018-02-09T03:35:10.840Z Reads: 87

```
Rule number 1, don't make "GHETTO" connectors especially when dealing with BATTERIES
```

---
## \#45 Posted by: Gabegds2001 Posted at: 2018-02-09T03:35:17.404Z Reads: 84

```
I looked at the mapping and I was confused lol I'll look at it tomorrow it's pretty late where I am.
```

---
## \#46 Posted by: ARetardedPillow Posted at: 2018-02-09T03:35:57.924Z Reads: 82

```
Lower your bat max and motor max, 60 amps is way too high for the batteries you're using
```

---
## \#47 Posted by: Gabegds2001 Posted at: 2018-02-09T03:36:07.505Z Reads: 82

```
Yea lol I used alligator wire clamps to hold the last unsoldered connection together bc I really wanted to see what it'd do.
```

---
## \#48 Posted by: ARetardedPillow Posted at: 2018-02-09T03:37:09.987Z Reads: 80

```
Just be glad that it didn't blow up with those clamps.

Also, whats your c rating on the batteries
```

---
## \#49 Posted by: Gabegds2001 Posted at: 2018-02-09T03:37:15.564Z Reads: 79

```
60 amps is too much? I thought 5ahx60=300 amps?
```

---
## \#50 Posted by: Gabegds2001 Posted at: 2018-02-09T03:37:37.522Z Reads: 77

```
They're 60c each
```

---
## \#51 Posted by: ARetardedPillow Posted at: 2018-02-09T03:38:53.254Z Reads: 81

```
Oh then it'll be fine for your batteries, no promises on your vesc though. Most people have their bat max at around 30-45
```

---
## \#52 Posted by: Gabegds2001 Posted at: 2018-02-09T03:39:29.692Z Reads: 77

```
Alright I'll turn it down to like 45-50amps
```

---
## \#53 Posted by: ARetardedPillow Posted at: 2018-02-09T03:40:33.837Z Reads: 78

```
And I'll turn up my amps 😂 @scepterr scolded me for having 35 bat max on dual
```

---
## \#54 Posted by: ARetardedPillow Posted at: 2018-02-09T03:44:19.748Z Reads: 74

```
Oh yea, forgot to mention, that directly affects your top speed and torque
```

---
## \#55 Posted by: Gabegds2001 Posted at: 2018-02-09T03:52:19.838Z Reads: 74

```
So... 45 or keep it at 60?
```

---
## \#56 Posted by: ARetardedPillow Posted at: 2018-02-09T03:52:58.033Z Reads: 77

```
No lower it lol 😂
Actually, I'm not the one to talk, but I suggest setting it at 45 and playing around with it a little bit see what you like yknow, its the DIY life
```

---
## \#57 Posted by: Gabegds2001 Posted at: 2018-02-09T03:53:23.788Z Reads: 78

```
Ok thn lol 
10 characters
```

---
## \#58 Posted by: Clonkex Posted at: 2018-02-09T03:56:47.290Z Reads: 80

```
I run mine at 60A but I have a focbox and they're rated for 60 continuous, 120 peak. I also don't often draw 60A for more than about 5-10 seconds at a time anyway (usually getting up to speed, and then I just cruise on a light throttle).
```

---
## \#59 Posted by: Gabegds2001 Posted at: 2018-02-09T03:57:13.096Z Reads: 83

```
Ok thanks for the help
```

---
## \#60 Posted by: Namasaki Posted at: 2018-02-09T04:23:42.274Z Reads: 82

```
[quote="Gabegds2001, post:24, topic:45913, full:true"]
So, should I make a series connector or should I keep the parallel connector if I want more speed?
[/quote]


If your gonna stick with the 149kv motor, then switch your batteries to series for more speed.
6s..... 149 x 25.2v= 3754 rpm
12s... 149 x 50.4v= 7509 rpm

parallel..... 25.2v x 10ah= 252 watt hours
series....... 50.4v x 5ah=  252 watt hours
The range remains the same, theoretically.
```

---
## \#61 Posted by: Tuomalar Posted at: 2018-02-09T11:47:50.982Z Reads: 73

```
I use 40A with my 10s dual and its more than enough for my 95kg of pure beaty. What remote are u using?
```

---
## \#62 Posted by: Gabegds2001 Posted at: 2018-02-09T13:36:02.369Z Reads: 69

```
Alright last night I made a series connector and it was way faster
```

---
## \#63 Posted by: Namasaki Posted at: 2018-02-09T16:06:33.877Z Reads: 64

```
Don’t forget to adjust your low voltage settings in the Vesc tool
```

---
## \#64 Posted by: Gabegds2001 Posted at: 2018-02-09T16:18:28.895Z Reads: 64

```
![15181930673031355903701|375x500](upload://g4KXA7HjsOjQf46SN55q2CPL1Vj.jpg) rate my enclosure?😂
```

---
## \#65 Posted by: GrecoMan Posted at: 2018-02-09T16:28:32.338Z Reads: 64

```
i’d give it a solid 2/10 🤣
```

---
## \#66 Posted by: ZackoryCramer Posted at: 2018-02-09T17:36:06.588Z Reads: 62

```
4/10 hey, at least it’s fireproof like mine 🤣 Is it stainless steel?
```

---
## \#67 Posted by: longhairedboy Posted at: 2018-02-09T17:47:26.776Z Reads: 63

```
i give that enclosure a solid 6 for clearly being made of whatever you happen to have laying around and yet it does exactly what its supposed to and could look hella worse.
```

---
## \#68 Posted by: Gabegds2001 Posted at: 2018-02-09T18:38:18.584Z Reads: 63

```
It's made out of aluminum lying around our high schools robotics shop lol yea it's really thin and weak.
```

---
## \#69 Posted by: TarzanHBK Posted at: 2018-02-09T22:20:41.251Z Reads: 59

```
it´s shiny and gives lots of magic smoke if your batteries comes off their insulation :monkey:

For real though.. isolate that beauty inside ;)
```

---
## \#70 Posted by: Gabegds2001 Posted at: 2018-02-10T00:50:26.349Z Reads: 56

```
Can I just line it with duct tape?
```

---
## \#71 Posted by: GrecoMan Posted at: 2018-02-10T00:56:12.396Z Reads: 55

```
don’t do that 🤣
```

---
## \#72 Posted by: celica39 Posted at: 2018-02-10T01:48:00.380Z Reads: 57

```
still very slow for 6s ! i can go 25mph but i have 192kv motor
```

---
## \#73 Posted by: Gabegds2001 Posted at: 2018-02-10T02:19:11.470Z Reads: 55

```
Too late lol i don't have any exposed wires anyway
```

---
## \#74 Posted by: Gabegds2001 Posted at: 2018-02-10T21:16:40.170Z Reads: 42

```
![1518297330130727550880|374x500](upload://p0mZELE3FNryr3xNSfXJ9bCYwwj.jpg)If I wanted to try using this 12v fan which plug would I use?
```

---
## \#75 Posted by: ZackoryCramer Posted at: 2018-02-10T21:18:53.969Z Reads: 39

```
There isn't a 12v supply output(that i know of). Vesc 4.12 should be fine without any heat solution assuming you don't blaze 30mph to work. If you really want that fan, get a 12v voltage regulator. The wiring is relatively simple.
```

---
## \#76 Posted by: Gabegds2001 Posted at: 2018-02-10T21:26:59.735Z Reads: 37

```
Ok thanks for the help
```

---
## \#77 Posted by: Tuomalar Posted at: 2018-02-11T11:29:35.884Z Reads: 34

```
Yeah no need to add fan if u don't go uphill with full throttle all the time. Or be heavy AF.
```

---
## \#78 Posted by: SOICDIP Posted at: 2018-02-11T11:41:02.741Z Reads: 32

```
[quote="Gabegds2001, post:74, topic:45913"]
If I wanted to try using this 12v fan which plug would I use?
[/quote]


If you really wanted a fan, the proper way is to get a 5V fan that draws little current <0.5A and power it from the VESC's 5V output.
```

---
## \#79 Posted by: Gabegds2001 Posted at: 2018-02-11T17:56:17.517Z Reads: 28

```
Well from what you guys say I'm in no need of one as theres no way I'm going up a hill 30 mph plus I'm 150lbs
```

---
