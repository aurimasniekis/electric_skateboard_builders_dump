# Me this weekend - and discussions about other things

### Replies: 69 Views: 2011

## \#1 Posted by: thisguyhere Posted at: 2018-03-12T17:18:43.662Z Reads: 305

```
hearing about burned up drvs on foc has always kept me using bldc but felt like living on the edge, this is me now

![image](upload://h8fXvf21D6PxQv6HowopiNdf5QC.png)
```

---
## \#2 Posted by: faithfulpuppy Posted at: 2018-03-12T17:20:25.001Z Reads: 288

```
does more torque and quieter operation sound awesome? yes. do i want to risk my hardware? eeeeeehhh
```

---
## \#3 Posted by: pennyboard Posted at: 2018-03-12T17:21:48.547Z Reads: 281

```
Now that ollin is done making vescs, is there any VESC that can reliably do 12s FOC?
```

---
## \#4 Posted by: thisguyhere Posted at: 2018-03-12T17:23:45.724Z Reads: 279

```
not sure about more torque but the quiet operation is pretty awesome.

snuck on my girlfriend inside the apartment, she had no idea what hit her.

did it mainly because there's a long corridor leading to the elevators in my building, and i felt bad about the whining noise.

[quote="pennyboard, post:3, topic:48874"]
VESC that can reliably do 12s FOC?
[/quote]

i mean, enertion runs their R2 on foc using focbox so take that for what it's worth
```

---
## \#5 Posted by: faithfulpuppy Posted at: 2018-03-12T17:25:37.755Z Reads: 262

```
yeah but ERPM on those hubs is lower than on my 15:40 "190kv" (remind me to test this for LHB this weekend) belt drive
```

---
## \#6 Posted by: barajabali Posted at: 2018-03-12T17:28:17.029Z Reads: 257

```
haha Love it 


@pennyboard All my boards run 12s FOC with Focboxes
```

---
## \#7 Posted by: Mikenopolis Posted at: 2018-03-12T17:30:54.540Z Reads: 256

```
[quote="barajabali, post:6, topic:48874"]
All my boards run 12s FOC with Focboxes
[/quote]

good to know. I'm sweating since I was planning on 12s FOC the dual 6374 build
```

---
## \#8 Posted by: Deckoz Posted at: 2018-03-12T17:34:02.603Z Reads: 240

```
2 boards FOC sensored on 13s here... 10+ on FOC sensored 12s. And 10+ on FOC sensored 10s..


FOC yourself across the stars... It's worth it
```

---
## \#9 Posted by: thisguyhere Posted at: 2018-03-12T17:34:11.144Z Reads: 236

```
limiting erpm at 60k tho, and turned switching freq to 18khz.  i have no idea if that'll preserve anything any better but voodoo doll whispered it into my ears.
```

---
## \#10 Posted by: thisguyhere Posted at: 2018-03-12T17:34:27.971Z Reads: 223

```
dope, any tuning hints?
```

---
## \#11 Posted by: Deckoz Posted at: 2018-03-12T17:34:30.573Z Reads: 217

```
There's no such thing as erpm limit in FOC
```

---
## \#12 Posted by: thisguyhere Posted at: 2018-03-12T17:34:46.006Z Reads: 213

```
oh...well then there you go.
```

---
## \#13 Posted by: Deckoz Posted at: 2018-03-12T17:36:13.669Z Reads: 208

```
But yea I setup as 25khz on all 190kv motors and 30khz on 170kv motors.

Lower switching frequentcy can induce some cogging.
```

---
## \#14 Posted by: Blitz Posted at: 2018-03-12T17:37:21.636Z Reads: 205

```
I got my focbox From group buy and I Don't know how returns work if Foc Focs it up.

But tell me is running foc Uncensored 2kw keda 190kv motor 9s lipos safe?
```

---
## \#15 Posted by: Deckoz Posted at: 2018-03-12T17:38:32.755Z Reads: 199

```
Don't see why it wouldn't. The boards I've buiilt and help setup are mixed between 2.54 and 3.100 ack firmware. Both are solid in FOC
```

---
## \#16 Posted by: Blitz Posted at: 2018-03-12T17:39:16.330Z Reads: 198

```
I will use new vesc tool and use the handy firmware update that comes with the tool.
```

---
## \#17 Posted by: thisguyhere Posted at: 2018-03-12T17:39:40.490Z Reads: 204

```
i see, vedder in his video said at 40khz mosfets and drv switching would require more current which means more heat so i though the opposite would be better.

i need to tune it some more tho because getting wheel lock at low speed braking.  would you still use the "Max ERPM at Full Brake" to tune this?
```

---
## \#18 Posted by: Deckoz Posted at: 2018-03-12T17:44:23.146Z Reads: 208

```
So that is accurate.  More current will be used but it's negilgible from what I have seen. I use the switching frequency to tune the smoothness of the torque.

Anyway FOC has a weird behavior that it likes to not hold position when fully braked and standing still and under 3mph it quickly ramps to full brake.

For FOC you've gotta use the current values to tune braking.
Motor min for high speed braking force, batt min for lowspeed braking force. But I've never been able to "fix it" completely. So I've just gotten used to progressively releasing brake around 3mph and putting my foot down.


Once you figure out where the full brake point is your thumb will get used to do a progressive release so you can stop without it wheel locking..
```

---
## \#19 Posted by: thisguyhere Posted at: 2018-03-12T17:46:02.615Z Reads: 200

```
that's great advice, thank you.

gonna F with it tonight, tighten it up.
```

---
## \#20 Posted by: ShutterShock Posted at: 2018-03-12T17:54:13.465Z Reads: 196

```
My board is on FOCBOX's and running 12S, 190kv sensored.  Observing the graphs in the VESC Tool, the erpms max out at around 54k.  So I feel plenty safe, especially considering that is like 34 mph which I will probably never hit.  

These are TB motors, so they probably are around 180 or 170kv in the end.
```

---
## \#21 Posted by: barajabali Posted at: 2018-03-12T17:54:55.868Z Reads: 183

```
Yes i always limit erpm to 60k just to be safe.
```

---
## \#22 Posted by: ShutterShock Posted at: 2018-03-12T17:55:25.427Z Reads: 183

```
Yeah I second this, it has almost thrown me when I'm going 1 mph next to someone walking and then accidentally lock the wheels by braking.

It is quite annoying... but bearable.

I don't really have a choice either since for whatever reason the VESC tool refuses to do BLDC detection on my focboxes.
```

---
## \#23 Posted by: PatRocks Posted at: 2018-03-12T18:05:16.868Z Reads: 178

```
@Deckoz Thanks for the info! It's sweet to have these settings summarized. 

@thisguyhere I also run 12s foc sensored. Both FOCBOX's, one is new, and one is from when they werr still called Vesc-X. Probably put 200-300 miles on the old one, but that was mostly at 8s. All in all, each has around 70 or 80 miles on 12s foc
```

---
## \#24 Posted by: squishy654 Posted at: 2018-03-12T20:53:14.892Z Reads: 173

```
I run the Hobbyking cheapo VESC that everyone says is crap, and I run it on 12 cell in FOC mode, sensored, ON ALL MY SETUPS! and I have never blown a HK VESC...(except when shorting phase wires mechanically and disastrously..lol)

I plugged in my 1st FOCBOX this weekend to program it for a forum member here, it smoked on the 1st test...so I installed a Hobbyking cheapo crappy older version and I literally went through the wizard, enabled FOC, sensors, did the tests, saved and rode it..

I am beginning to think there's some silly marketing going on or things out of spec..and this cheap crap everyone hates from Hobbyking is the most robust stuff I have used yet, and I spent thousands acquiring examples of everything to test..so I'm not just saying this because it's what I use or bought 1st, but I'm speaking from experience..I have never used BDLC mode on any vesc, because I have never had too and nothing ever smoked, till I plugged in a FOCBOX...I thought the FOCBOX was suppose to handle more power and be more robust? I'm not trying to be negative or trash anything, but the people who all run around saying this or that, I find to be wrong, from experience earned with my own hands and thousands of miles of testing...take it or leave it..
```

---
## \#25 Posted by: b264 Posted at: 2018-03-12T20:56:36.068Z Reads: 167

```
[quote="thisguyhere, post:4, topic:48874"]
did it mainly because there’s a long corridor leading to the elevators in my building, and i felt bad about the whining noise
[/quote]

And I thought I was the only one that wanted FOC solely because feeling-bad about the noise in the hallway leading to the elevators.  Outside, I don't give a hoot.
```

---
## \#26 Posted by: MannyM0E Posted at: 2018-03-12T21:23:39.425Z Reads: 159

```
What about FOC mode on 10s with the focbox ?
```

---
## \#27 Posted by: thisguyhere Posted at: 2018-03-12T21:50:28.125Z Reads: 151

```
i think 10s is the sweet spot, meaning it's been shown to be more unstable at higher voltages.

but considering the responses above, there doesn't seem to be any solid consensus on idea FOC setups.
```

---
## \#28 Posted by: cosmicc89 Posted at: 2018-03-13T02:42:53.752Z Reads: 148

```
This is really interesting. I'm curious how many others have encountered something similar?
```

---
## \#29 Posted by: ATLesk8 Posted at: 2018-03-13T11:34:30.123Z Reads: 139

```
I've also run FOC unsensored at 10S on a TB vesc and no problems, in fact the TB complete boards came 12S FOC stock and my brother's has been fine and is a rocket. 

I tried it 12S FOC with focboxes, but I missed the electric motor sound. Honestly I love that high pitched whine and it lets pedestrians know I'm coming (that is if they're paying attention at all). So i guess I prefer BLDC
```

---
## \#30 Posted by: Namasaki Posted at: 2018-03-13T11:48:10.206Z Reads: 136

```
How woul you describe performance differences between FOC and BLDC?
```

---
## \#31 Posted by: ducktaperules Posted at: 2018-03-13T13:26:37.523Z Reads: 129

```
I run 12s FOC no problems with FOCBOX and i weigh 1/8th of a metric fuck-tonne.
```

---
## \#32 Posted by: Deckoz Posted at: 2018-03-13T13:34:24.838Z Reads: 128

```
FOC and BLDC both pull hard... Almost the same. But top speed of FOC is a few mph slower then BLDC.

FOC is significantly smoother transitions of throttle. And quieter.
```

---
## \#33 Posted by: Blitz Posted at: 2018-03-13T13:56:45.407Z Reads: 124

```
So for making a top speed test etc you'd go bldc but for normal cruising Going foc right?
could changing them around increase Odds for error significantly?

Edit: Oh no I'm asking noob questions again :joy:
```

---
## \#34 Posted by: Deckoz Posted at: 2018-03-13T14:02:37.434Z Reads: 120

```
I wouldn't be bothered to change modes because it changes the feel of the board.
```

---
## \#35 Posted by: Blitz Posted at: 2018-03-13T14:04:28.779Z Reads: 118

```
I wan't that Vrum Vrum! but I need to fly under the radar :joy:
I need something load and then quite on the press of a button any ideas?
```

---
## \#36 Posted by: DeathCookies Posted at: 2018-03-13T14:22:34.183Z Reads: 115

```
Changing from one to another mode Needs a restart. So if you push your button you will have to wait 3 seconds before you can go on with your ride...

[quote="Blitz, post:35, topic:48874"]
I wan’t that Vrum Vrum! but I need to fly under the radar :joy:
[/quote]
Maybe just build two boards? One to pose and one stealthy?
```

---
## \#37 Posted by: SeanHacker Posted at: 2018-03-13T14:23:05.231Z Reads: 111

```
You can use @Ackmaniac's firmware/app to switch between FOC/BLDC on your phone. You just need a bluetooth module. ;)
```

---
## \#38 Posted by: DeathCookies Posted at: 2018-03-13T14:26:36.186Z Reads: 110

```
[quote="SeanHacker, post:37, topic:48874"]
You can use @Ackmaniac’s firmware/app to switch between FOC/BLDC on your phone. You just need a bluetooth module. :wink:
[/quote]

Please tell me how you can do that on the android app?

I know that i can Change modes which means different throttle curves and different max values (amp, Volt, ...) but i did not find anything about changing from bldc<->foc on the fly
```

---
## \#39 Posted by: Blitz Posted at: 2018-03-13T14:29:12.087Z Reads: 112

```
Wow guys Never thought that would be possible Thanks for the Input @SeanHacker and @DeathCookies  Because once I'd get out of my neighborhood and be near a straight stretch of clear road I'd like bldc.
```

---
## \#40 Posted by: DeathCookies Posted at: 2018-03-13T14:34:18.051Z Reads: 111

```
IMHO that just sounds silly... maybe because i am not a poser and want to drive the board instead of Hearing it.
The drawback of loud Motors is that you overhear Problems with your board. You can easily overhear some rattling which indicates Trouble never the less..... 

Just to put it in a nutshell: I will not go back to BLDC anytime soon, because:
- you hear a lot more without loud Motors
- you have a much smoother startup
```

---
## \#41 Posted by: SeanHacker Posted at: 2018-03-13T14:37:42.999Z Reads: 108

```
I can't connect to my board right now to check. But long press the box in the upper left hand corner. ;)
```

---
## \#42 Posted by: Blitz Posted at: 2018-03-13T14:39:24.251Z Reads: 105

```
oh look that Ferrari makes loud noises what a poser! does that sound silly?
and i'm no poser I said Once i'm out of the neighborhood.

[quote="Blitz, post:39, topic:48874"]
straight stretch of clear road I’d like bldc.
[/quote]
 I would like a few more km/h at times Kinda like sport mode that you can enable in a BMW.
```

---
## \#43 Posted by: b264 Posted at: 2018-03-13T14:42:42.381Z Reads: 102

```
Changing your VESC settings everytime you ride sounds like one of two things:

A) you ride once a month/year
or
B) the fastest way to kill a VESC
```

---
## \#44 Posted by: DeathCookies Posted at: 2018-03-13T14:42:54.279Z Reads: 107

```
[quote="SeanHacker, post:41, topic:48874"]
I can’t connect to my board right now to check. But long press the box in the upper left hand corner. :wink:
[/quote]

You can only Change the app mode but not the Motor mode! 


app mode 
- min battery
- max battery
- min Motor
- max Motor
-  throttle curve

motor mode
- bldc 
- foc
```

---
## \#45 Posted by: Blitz Posted at: 2018-03-13T14:44:00.101Z Reads: 104

```
Its just what I think is a cool Idea, maybe it could be a possibility in the future if so don't you think that would be a bit cool eh?
```

---
## \#46 Posted by: b264 Posted at: 2018-03-13T14:45:16.222Z Reads: 103

```
Getting into the VESC settings is the last thing I want to do.  Personally, I don't ever want the motors to make noise.  I want two buttons, one that goes ding, ding, ding and the other is a locomotive horn.  That's it, as far as the board making noise.
```

---
## \#47 Posted by: DeathCookies Posted at: 2018-03-13T14:45:42.345Z Reads: 105

```
[quote="Blitz, post:42, topic:48874"]
and i’m no poser I said Once i’m out of the neighborhood.
[/quote]

I never said you are a poser ;) Sorry when it sounded wrong..

[quote="Blitz, post:42, topic:48874"]
I would like a few more km/h at times Kinda like sport mode that you can enable in a BMW.
[/quote]

You mean it will make a big difference if you drive 42kmp instead of 40 kmh?
There is really no big difference in topspeed at all. I always ignore this fact. Not because it is not true. It is absolutely true but there difference is negligible.
```

---
## \#48 Posted by: Blitz Posted at: 2018-03-13T14:46:41.062Z Reads: 100

```
maybe 3km/h more and I could feel the difference but Hey!
https://media.giphy.com/media/xUA7bhz139D3kTIowg/giphy.gif
```

---
## \#49 Posted by: DeathCookies Posted at: 2018-03-13T14:51:14.216Z Reads: 101

```
[quote="Blitz, post:45, topic:48874, full:true"]
Its just what I think is a cool Idea, maybe it could be a possibility in the future if so don’t you think that would be a bit cool eh?
[/quote]

To **ME** it does not sound like a cool idea. If it sounds to you like the best idea ever: thats okay. Everyone has different Needs!

[quote="Blitz, post:48, topic:48874, full:true"]
maybe 3km/h more and I could feel the difference but Hey!
[/quote]

We could argue that everybody could even feel the difference between 40 and 40,2kmh but i do not want to fight. I also do not want to judge you. I just give you **my insights** ;)

PS: @b264 hat some good aspects too (Y)
```

---
## \#50 Posted by: SeanHacker Posted at: 2018-03-13T14:51:33.962Z Reads: 97

```
I must've missed the point. I thought @Blitz was asking if he could switch from FOC to BLDC on the go. Wouldn't the FOC/BLDC switch in the app be what he's looking for? Maybe not. I'm confused now. Lol.
```

---
## \#51 Posted by: DeathCookies Posted at: 2018-03-13T14:53:37.798Z Reads: 106

```
[quote="SeanHacker, post:50, topic:48874"]
Wouldn’t the FOC/BLDC switch in the app be what he’s looking for? Maybe not. I’m confused now. Lol.
[/quote]

In the VESC TOOL there is a Switch to Change the mode. But you can barely Access the VESC TOOL on the fly... (attaching usb cable to a pc with the software installed)

In the VESC MONITOR (the Smartphone app) you can Change the mode like explained earlier over Bluetooth with your smartphone
```

---
## \#52 Posted by: Deckoz Posted at: 2018-03-13T15:25:35.645Z Reads: 110

```
Y'all realize with a metr module you have Perimetr which can change all vesc settings. Or wirelessly tcp bridge over Bluetooth to vesc tool. 

For example I left my board outside in the garage plugged in walked up stairs to the computer changed settings  and walked back outside... Vs carrying 30lb board upstairs, unbolting enclosure to plug in USB etc

Metr TCP bridge to VESC Tool
![Screenshot_20180313-112734|281x500](upload://iWG7w1npKjQGBLC9KnoO70g3LUZ.png)

Or second example just turn on board and open Perimetr instead of metr and change your settings.

PeriMetr settings
![Screenshot_20180313-112719|281x500](upload://rJj8DxzC2JKHfwXo84hzjjzpHY9.png)

Can even do wireless motor detection in PeriMetr or over tcp bridge...
```

---
## \#53 Posted by: DeathCookies Posted at: 2018-03-13T15:30:11.020Z Reads: 100

```
[quote="Deckoz, post:52, topic:48874, full:true"]
Y’all realize with a metr module you have Perimetr which can change all vesc settings. Or wirelessly tcp bridge over Bluetooth to vesc tool.

For example I left my board outside in the garage plugged in walked up stairs to the computer changed settings  and walked back outside… Vs carrying 30lb board upstairs, unbolting enclosure to plug in USB etc

Or second example just turn on board and open Perimetr instead of metr and change your settings.
[/quote]

Well, many of us could alter the VESC MONITOR app to Change all values possible.
Why did not ackmania or someone else did this earlier?

Because you do not Need These Settings to Change daily. It will only lead to Problems...
How often does a user make a Motor calibration. Normally only the first time he sets the board up. After Setup he will leave it like that. But to Change if the board has more or less power is good Option!
```

---
## \#54 Posted by: Deckoz Posted at: 2018-03-13T15:31:38.864Z Reads: 93

```
The point is more so you can wirelessly setup the board with the enclosures buttoned up vs having the board half sprawled out doing detections and having to use usb

So really it's upto the use case of the user..it covers blitz's want to change on the fly. Use it how you see fit.
```

---
## \#55 Posted by: DeathCookies Posted at: 2018-03-13T15:35:43.068Z Reads: 94

```
[quote="Deckoz, post:54, topic:48874, full:true"]
The point is more so you can wirelessly setup the board with the enclosures buttoned up vs having the board half sprawled out doing detections and having to use usb
[/quote]

If you have to fix your board this is a nice Feature. Else it does not have much use.

[quote="Deckoz, post:54, topic:48874"]
So really it’s upto the use case of the user…it covers blitz’s want to change on the fly. Use it how you see fit.
[/quote]


You are absolutely right. I did not know the possibilities of metr.

@Blitz The perfect solution for you would be the Metra app. When you drive away in FOC you can stop and Change to BLDC on the fly. Just make sure that the vesc has restarted
```

---
## \#56 Posted by: Deckoz Posted at: 2018-03-13T15:40:40.539Z Reads: 92

```
Doesn't have much use?

I dunno about you but being able to assemble a board without mucking with configurations first is super useful. Being able to tune the boards settings, or update firmware wirelessly, super useful. 

Who wants to use a USB ever? Not me.. lol who wants to unbolt thier enclosure to change a simple setting..  it's alot more useful then you think...
```

---
## \#57 Posted by: Jc06505n Posted at: 2018-03-13T15:43:51.147Z Reads: 93

```
I plan on changing my VESC settings on my Anubis a few times since the Anubis is meant to be able to switch drives. I plan on doing so via the Perimetr app. 

[quote="DeathCookies, post:51, topic:48874"]
In the VESC TOOL there is a Switch to Change the mode. But you can barely Access the VESC TOOL on the fly… (attaching usb cable to a pc with the software installed)
[/quote]


Like @Deckoz, You can assess the VESC Tool wirelessly on the fly via TCP bridge. 

[quote="DeathCookies, post:53, topic:48874"]
Well, many of us could alter the VESC MONITOR app to Change all values possible.

Why did not ackmania or someone else did this earlier?

Because you do not Need These Settings to Change daily. It will only lead to Problems…

How often does a user make a Motor calibration. Normally only the first time he sets the board up. After Setup he will leave it like that. But to Change if the board has more or less power is good Option!
[/quote]


That's because most boards don't have a reason to. On my build im planning on testing out how practical and ease changing drives would be. 

[quote="DeathCookies, post:55, topic:48874"]
If you have to fix your board this is a nice Feature. Else it does not have much use.
[/quote]


Swappable Drive Trains man. Swappable Drive Trains. 

[quote="Deckoz, post:56, topic:48874"]
Who wants to use a USB ever? Not me… lol who wants to unbolt thier enclosure to change a simple setting…  it’s alot more useful then you think…
[/quote]


Agreed!
```

---
## \#58 Posted by: b264 Posted at: 2018-03-13T16:24:15.068Z Reads: 81

```
I will count-down the days until you accidentally make a mistake and cook an ESC.

For doing something like swapping drives, you should probably be changing the user interface to support that as well, because it's too easy to make a critical mistake getting in the VESC settings that often.
```

---
## \#59 Posted by: b264 Posted at: 2018-03-13T16:24:52.320Z Reads: 81

```
What about attaching the ESC(s) to the drive and they get swapped as well?
```

---
## \#60 Posted by: Jc06505n Posted at: 2018-03-13T16:56:28.793Z Reads: 85

```
After one detection it should be as simple as selecting a mode and loading it: 

![image|281x500](upload://qK93MGs3j3Vwjg9yRyTLmKVW0Rm.jpg)

But carefulness should be taken agreed. 

I rather not swap out the VESC everyone since that kills part of the point. I think using Perimetr should be fine
```

---
## \#61 Posted by: Blitz Posted at: 2018-03-13T16:56:36.157Z Reads: 86

```
I hate when people change the title and don't say that they did it So I'll say it I removed the "Heated" part,

This is a pretty good discussion @Deckoz made us aware of a good program and the power of Bluetooth module and @b264 said well you could ruin something. But if there would be an app where you can preset idiot proof modes I see something useful.  The risk factor is there but ill research this idea
```

---
## \#62 Posted by: Deckoz Posted at: 2018-03-13T16:58:38.644Z Reads: 87

```
You can do this.

Use VESC tool, program the vesc. Read the settings with perimeter and save it as a config profile. Change the vesc tool settings, read again from perimeter save as a different config profile.

Switch between profiles you setup with vesc tool via perimeter
```

---
## \#63 Posted by: Blitz Posted at: 2018-03-13T17:00:35.766Z Reads: 89

```
Yeah, that sounds good, If I bought enertions warranty I would totally do that Near my neighbourhood be quiet not to disturb near roads get load and powerful in the city back to Foc,

For me its nothing about being practical Its just having cool features that makes my board different from others,
and that was just one of the Ideas I probably won't do that because I can't afford a blown vesc or any error.
```

---
## \#64 Posted by: ducktaperules Posted at: 2018-03-15T16:52:06.718Z Reads: 87

```
looks like i spoke to soon,  after 6 months one of my focbox quit on me this morning. DRV error :frowning:
```

---
## \#66 Posted by: Mikenopolis Posted at: 2018-03-15T20:48:07.676Z Reads: 86

```
do you happened to known WHEN it died? like hill? braking? acceleration?
```

---
## \#67 Posted by: ducktaperules Posted at: 2018-03-16T13:39:09.848Z Reads: 86

```
Yeah i was on my normal work commute, it was a little wet on the ground but nothing unusual. just finished a big flat section, came up to the big hill. There are traffic lights at the bottom so i usually go past them them wait for the lights to go red, this way i can go up the hill without worrying about any cars being behind me cause they are all stuck at the lights.

So the lights go red and the last car goes past. I pull away as normal, get about 2m forward when everything cuts out. look down and red light is flashing on one of my vesc's. Seems like in fault condition it also stops sending throttle commands over CAN bus.

It was not under much load and nowhere neer erpm limit. maybe it happened at the point of switching from hall to sensorless??

Walk to work. at lunch open up and everything looks good, plug in usb and its showing drv error on my master, slave is fine. inside focbox everything looks ok, no obvious signs of electrical damage, no smell of magic smoke.

i built a new temporary enclosure ~2 weeks ago so i know everything was secure inside and nothing would be touching that shouldn't be. 

Only thing i can think is that maybe it got wet? maybe one of the caps died? 

it seems like the DRV error can be caused by a whole host of things. if anyone knows a good way to diagnose i would like to know :frowning:
```

---
## \#68 Posted by: scepterr Posted at: 2018-03-24T12:26:59.511Z Reads: 69

```
Pictures of the PCB would be useful
```

---
## \#69 Posted by: ducktaperules Posted at: 2018-03-25T19:06:40.017Z Reads: 58

```
so i swapped the DRV and its not giving me errors any more :slight_smile:  but i have not had a chance to spin it up with a motor on yet.
```

---
## \#70 Posted by: davidbonde Posted at: 2018-05-08T09:26:00.716Z Reads: 45

```
[quote="Deckoz, post:54, topic:48874"]
it covers blitz’s want to change on the fly. Use it how you see fit.
[/quote]


Do we need to do motor detection every time if we change between bldc and foc? Are the detection bonded to the mode or is it interchangeable?
```

---
