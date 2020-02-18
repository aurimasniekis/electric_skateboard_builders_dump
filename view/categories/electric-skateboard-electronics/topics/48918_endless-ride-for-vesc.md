# Endless Ride for VESC?

### Replies: 89 Views: 3812

## \#1 Posted by: PredatorBoards Posted at: 2018-03-13T00:40:39.214Z Reads: 484

```
Not sure if there was any progress made in this department, but surely we must have someone working on this feature, right? With the advent of the customizable bluetooth remotes like the Firefly and Photon, a feature like this should be pretty simple to implement. I remember the Nunchuck has a cruise-control setting that would maintain the current RPM even when you kick push the board. Obviously you couldn't pay me to use a nunchuck remote.
```

---
## \#2 Posted by: Genghis_Kuan Posted at: 2018-03-13T01:10:25.720Z Reads: 459

```
Doesn't Ackmaniac's ESC tool have a Cruise Control via Secondary Channel?
```

---
## \#3 Posted by: mmaner Posted at: 2018-03-13T01:11:13.898Z Reads: 457

```
The photon has a cruise control feature. It's also in the @Ackmaniac firmware.
```

---
## \#4 Posted by: Rinzler Posted at: 2018-03-13T01:15:13.722Z Reads: 451

```
Endless mode is different than cruise control. The Mellow team explained it like a push board range amplifier. You kick your board foward and it helps to propel you foward but with a lower power than it is needed for endless continuous speed riding, if you stop pushing your board will eventually stop.
```

---
## \#5 Posted by: Pedrodemio Posted at: 2018-03-13T01:18:58.670Z Reads: 422

```
Using an Arduino over UART, it should be easy to implement, or even in the firmware

Something like if speed greater than X start control loop, this loop would be a speed control with dropping speed, you can set various parameters like time constant and etc, maybe an inverse exponential function would mimic well the unpowered board feeling
```

---
## \#6 Posted by: PredatorBoards Posted at: 2018-03-13T01:34:23.036Z Reads: 404

```
Has someone specifically implemented this for the firefly? I'm going to be building one shortly.
```

---
## \#7 Posted by: mmaner Posted at: 2018-03-13T01:52:49.535Z Reads: 395

```
The @Ackmaniac firmware has a push for speed control function as well, sounds similar.
```

---
## \#8 Posted by: pennyboard Posted at: 2018-03-13T02:06:11.751Z Reads: 382

```
This seems like a cool feature, but I don’t really get why you’d want it, except to extend your range. If you have a powered board, why not just use the remote to cruise at the speed you want, slow down, speed up, etc?
```

---
## \#9 Posted by: PredatorBoards Posted at: 2018-03-13T02:42:04.548Z Reads: 371

```
Because endlessride/push assist makes riding more akin to regular longboarding rather than esk8ing. Every push you make is amplified with a surge of power to the wheels. The entire ordeal makes you feel like superman stomping the ground. The ride and sensation feels truly 'endless'.
```

---
## \#10 Posted by: Deckoz Posted at: 2018-03-13T02:46:00.137Z Reads: 356

```
How does going down hills.work? When does it know to not accelerate if gravity is causing acceleration?
```

---
## \#11 Posted by: PredatorBoards Posted at: 2018-03-13T02:47:17.807Z Reads: 338

```
You still have your remote to brake. You truly haven't lived till you pumped your way to full speed. Now do it up a hill. It's pretty cool.

I guess the best way I can explain this to other longboards... is imagine those times you get that **really** satisfying stride when you push. Endless ride basically lets you experience that euphoria every time you push.
```

---
## \#12 Posted by: Deckoz Posted at: 2018-03-13T02:50:18.963Z Reads: 322

```
Ah I thought it was remoteless. 

Interesting.
```

---
## \#13 Posted by: Apolo Posted at: 2018-03-13T04:32:07.043Z Reads: 304

```
Planning on building a firefly soon too. Where are you sourcing parts? I don't want to wait 39 days for aliexpress.

Also, are there any instructions or guides to follow?
```

---
## \#14 Posted by: PredatorBoards Posted at: 2018-03-13T08:17:46.466Z Reads: 289

```
eBay. Payment processes faster, and there's generally an American based supplier for what you need. Costs are roughly the same. There's a github wiki and spreadsheet BOM you can follow. https://docs.google.com/spreadsheets/d/1G6cbB9tymxwAx_ul-3dK_ecZLHnj8iVudTKXk6aNmv8

I'm honestly going to hold off until i know for a fact we can implement this endless ride feature. Otherwise the firefly and photon are just glorified PPM controllers with LCD screens. Everyone complaining about the short throw of the Nano remote has likely not bothered adjusting the throttle curves, which makes a huge difference.
```

---
## \#15 Posted by: Ackmaniac Posted at: 2018-03-13T09:52:35.355Z Reads: 274

```
Just get on the baord and try to push while you accelerate with the remote. And if you think that might work then try the same uphill.
```

---
## \#16 Posted by: banjaxxed Posted at: 2018-03-13T09:53:05.994Z Reads: 275

```
And can also help with the legal aspect in some juristictions iirc. A tiny remote with just a brake/light control would be nice to have
```

---
## \#17 Posted by: Lumaci Posted at: 2018-03-13T09:54:56.167Z Reads: 271

```
It could be pretty damn easy to make, if you turn the sensor signal from the motor into a ppm signal it could work.

So the amount of rpm output from the sensor cable will be turned into the amount of throttle on the vesc.

That could also allow you to use a remote, since you could also do this via uart.

Anything thats able to read the rpm could turn the signal back and into the needed ppm signal.
```

---
## \#18 Posted by: lowGuido Posted at: 2018-03-13T10:04:16.266Z Reads: 264

```
I made a board some time ago that had a small button in the tail that would hold the speed so long as you were standing on it, is that what you are talking about here?
its a standard feature in VESC.

I called it kick assist rather than endless, pretty sure I was the first to ever do it.
```

---
## \#19 Posted by: banjaxxed Posted at: 2018-03-13T11:21:29.699Z Reads: 258

```
I saw that vid I think you got a first there dude let nobody take it away from you!

Was it not @Ackmaniac's f/w which allowed this?
```

---
## \#20 Posted by: lowGuido Posted at: 2018-03-13T11:24:25.784Z Reads: 259

```
I have never used @Ackmaniac firmware on any VESC. not because I don't think its great, but because I just never got around to upgrading firmware.
```

---
## \#21 Posted by: banjaxxed Posted at: 2018-03-13T11:43:47.204Z Reads: 245

```
Found it! This needs more uptake

http://www.electric-skateboard.builders/t/low-guidos-hack-board-for-science-now-with-hub-motors/870/41
```

---
## \#22 Posted by: lowGuido Posted at: 2018-03-13T11:57:14.106Z Reads: 242

```
yeah it's a really simple thing to build.
I'm somewhat surprised that no one (except maybe mellow) has really gone anywhere with it.
this whole conversation has inspired me to resurrect that board and build a proper one.
```

---
## \#23 Posted by: webst Posted at: 2018-03-13T12:10:38.904Z Reads: 233

```
Mellow has it much better though
```

---
## \#24 Posted by: banjaxxed Posted at: 2018-03-13T12:29:20.911Z Reads: 227

```
I think it's a great idea especially with the descrete boards coming out of here, twinned with hubs
```

---
## \#25 Posted by: Wajdi Posted at: 2018-03-13T16:48:12.669Z Reads: 225

```
I like the idea of Endless ride, never thought about it before, and I think I have a grasp of how it works from your previous descriptions, its basically mimicking the act of pushing your board but with an amplified force that will be eventually damped out. Its like jumping in real life, but with this feature enabled you jump much higher, and land smoothly.

This can be totally done on the Photon remote, we can even add an option to control power variable through the remote, the lower the value, the closer you will get to regular pushing, the higher the value, the more power and range you will get from a single push. 

[quote="PredatorBoards, post:14, topic:48918"]
firefly and photon are just glorified PPM controllers with LCD screens
[/quote]

PS: the Photon is really much more than just a glorified PPM controller with an LCD :wink:

Added to my TODO list :slight_smile:
```

---
## \#26 Posted by: mikenyc Posted at: 2018-03-13T17:44:48.548Z Reads: 204

```
I've got a Mellow. Endless Mode is cool, I rarely use it because it lacks the speed that I desire. It takes a little bit of getting used to as there is no free roll.
```

---
## \#27 Posted by: Jc06505n Posted at: 2018-03-13T17:48:27.163Z Reads: 197

```
So gear drive + endless ride = profit ?
```

---
## \#28 Posted by: mikenyc Posted at: 2018-03-13T17:56:58.643Z Reads: 195

```
no. I'm moving away from gears
```

---
## \#29 Posted by: PredatorBoards Posted at: 2018-03-13T17:57:05.765Z Reads: 197

```
I would LOVE endless mode for board walking/dancing. You would still need to kick push from time to time, so your routine can still incorporate stepping off the board, but now you can basically maintain longer lines.

Best I can put it is if you tried dancing on smooth marble. You just go on forever.
```

---
## \#30 Posted by: Jc06505n Posted at: 2018-03-13T17:58:24.983Z Reads: 193

```
Really ? Why so? Wouldn’t the Gear Drives’s drew rolling capabilities be best for a feature like this?
```

---
## \#31 Posted by: mikenyc Posted at: 2018-03-13T17:59:59.389Z Reads: 189

```
I think I mistook gears for belts, lol.
```

---
## \#32 Posted by: PredatorBoards Posted at: 2018-03-13T18:01:14.621Z Reads: 184

```
I mean technically if 'endless mode' was to be properly implemented, you wouldn't detect the difference between belt drive and hub drive. Both would 'artificially coast' the same amount.
```

---
## \#33 Posted by: mikenyc Posted at: 2018-03-13T18:01:25.085Z Reads: 181

```
however, I think hubs are probably the best application.
```

---
## \#34 Posted by: Jc06505n Posted at: 2018-03-13T18:08:04.625Z Reads: 175

```
Lol Nha , I meant gears like Arc and Jed.
```

---
## \#35 Posted by: Jc06505n Posted at: 2018-03-13T18:12:51.779Z Reads: 179

```
I see, so the rolling resistance wouldn't interfere at all or need to be accounted in implementation? 

I was hypothesis that the free rolling capabilities of gear drives would make endless riding easier or affect it in some way, whether it be in implementation, calculation, or end result.
```

---
## \#36 Posted by: PredatorBoards Posted at: 2018-03-13T18:17:26.590Z Reads: 180

```
No the rolling resistance will bear zero effect for endless ride. This is effectively an equalizer. The slow decay in speed is artificial and (ideally) programmable.
```

---
## \#37 Posted by: Luuke Posted at: 2018-03-13T18:44:59.798Z Reads: 191

```
Endless mode would be really cool!
with focus on law it sounds even better then the option to push to accelerate and hold the speed.
e.q. limit it to 25km/h and 250watts .

for that control mode two parameters are necessary:
maximum power of support
damping of that power

So by adjusting these two parameters you have full control.
If you set the decrease rate of the power to zero, it is like your implemented push-and-hold-speed mode.

So the remote is just needed to brake, not to accelerate.
```

---
## \#38 Posted by: webst Posted at: 2018-03-13T20:47:37.410Z Reads: 184

```
https://youtu.be/AWWLP7TwsDU?t=2m5s
```

---
## \#39 Posted by: Ackmaniac Posted at: 2018-03-13T22:53:45.112Z Reads: 183

```
Did that already. It's available in my firmware mod. Difference is that you need to pull the trigger so that cruise is active. And it doesn't slowly reduce the speed. And by the way. It doesn't make the board legal.
```

---
## \#40 Posted by: banjaxxed Posted at: 2018-03-13T22:58:12.177Z Reads: 183

```
Endless ride should turn Rusty bearings into ceramic Swiss in the feels
```

---
## \#41 Posted by: mikenyc Posted at: 2018-03-13T23:02:51.857Z Reads: 182

```
can it be modified so that you only use the trigger to stop?
```

---
## \#42 Posted by: Ackmaniac Posted at: 2018-03-13T23:07:52.681Z Reads: 180

```
Sure it can but this way it is safer. I think it's a bad idea that the board gives power the moment you push. Hard to keep balance. In my mode you simple release the trigger, push and hold the trigger again.
```

---
## \#43 Posted by: mikenyc Posted at: 2018-03-13T23:09:56.775Z Reads: 181

```
the way mellow works is that it matches the maximum speed that you push the board. it's not so much that there is a jolt of power, it's more like, I push, and then it's a really long coast that gradually slows, kind of how a friction motor works in a toy car

https://www.youtube.com/watch?v=LZNU1uKmj60

edit: adding video
```

---
## \#44 Posted by: Wajdi Posted at: 2018-03-14T00:14:48.377Z Reads: 172

```
@mikenyc @webst
Thanks for the video, and yes mikenyc is correct, the way I see Mellow implementing it is by pushing the board a couple times, get up to a certain speed threshold, controller holds that speed for a period of time using some sort of cruise control, then gradually release power. They use the simplest approach, yet still safe and effective.
```

---
## \#45 Posted by: Ackmaniac Posted at: 2018-03-14T07:36:27.882Z Reads: 166

```
Did anybody ever test a mellow and can tell us if it feels good or bad?
```

---
## \#46 Posted by: lrdesigns Posted at: 2018-03-14T07:45:13.551Z Reads: 168

```
I thought endless ride meant attaching a HUGE solar panel to your helmet, then running wires down your pants to the board. :face_with_raised_eyebrow:
```

---
## \#47 Posted by: b264 Posted at: 2018-03-14T07:53:59.409Z Reads: 163

```
[quote="mikenyc, post:26, topic:48918, full:true"]
I’ve got a Mellow. Endless Mode is cool, I rarely use it because it lacks the speed that I desire. It takes a little bit of getting used to as there is no free roll.
[/quote]

What happens when you start going down a hill?
```

---
## \#48 Posted by: webst Posted at: 2018-03-14T10:02:26.485Z Reads: 158

```
Can't you just watch the mellow video I pasted above?
```

---
## \#49 Posted by: mikenyc Posted at: 2018-03-14T10:18:52.433Z Reads: 156

```
It maintains your speed, so you’d want to apply the brake and either carve down, or use the brake to slow yourself.
```

---
## \#50 Posted by: b264 Posted at: 2018-03-14T10:32:47.533Z Reads: 157

```
So it actually can't differentiate between a downhill and a push then.  Okay
```

---
## \#51 Posted by: mikenyc Posted at: 2018-03-14T11:52:09.500Z Reads: 154

```
Yea but it’s no big deal, just free roll down the hill
```

---
## \#52 Posted by: b264 Posted at: 2018-03-14T12:47:41.236Z Reads: 152

```
What happens if you footbrake, do the motors attempt to overpower your brake?
```

---
## \#53 Posted by: webst Posted at: 2018-03-14T12:52:03.877Z Reads: 154

```
Motors are just slowing down in preprogrammed manner (some fraction of speed per 30 revolutions). There is no distinguishing if you go upwards or downwards so your foot on the ground has no effect on ride unless you're going up really steep hill.
```

---
## \#54 Posted by: mikenyc Posted at: 2018-03-14T13:03:48.375Z Reads: 156

```
It’ll think it’s going uphill. You have to use the remote to stop
```

---
## \#55 Posted by: Dmaxx Posted at: 2018-03-14T13:21:26.836Z Reads: 156

```
I got to try a mellow board yesterday on their west coast tour. They do feel really smooth, and the endless mode feels quite nice. Two kicks would keep me rolling like 40ft on flats. It was raining so i didnt get to REALLY try it out..
```

---
## \#56 Posted by: bevilacqua Posted at: 2018-03-14T14:01:43.562Z Reads: 162

```
I tried your duty cycle push assist mode. It worked fine 90% off the time, but sometimes the motor (Hubmotor-single) would slam the brakes or get stuck after slipping over some gravel on the ground (tested it in winter). 

Have you experienced something like that? 

Current control works fine. 
Tested on: 10S Focbox single Hubmotor (Sensored).
```

---
## \#57 Posted by: Ackmaniac Posted at: 2018-03-14T16:06:11.316Z Reads: 160

```
You should disable braking in the PID settings so that braking is disabled during cruise control.
```

---
## \#58 Posted by: bevilacqua Posted at: 2018-03-14T16:17:41.183Z Reads: 163

```
perfect, will try that. 

Danke :)
```

---
## \#59 Posted by: PredatorBoards Posted at: 2018-03-15T01:23:22.616Z Reads: 163

```
So let me build upon this concept with you guys. Say we get this endless ride thing implemented. We can run a remoteless setup. Basically we can have pressure sensor on the board for just brakes. It's more or less a novelty, however it sounds pretty great for say an electric assisted LDP. I'd like one for the fact that no remote = hardwired control.
```

---
## \#60 Posted by: banjaxxed Posted at: 2018-03-22T11:14:34.981Z Reads: 162

```
Don't forget to support all flavours with 'stomp pedal' positions

![image|526x500](upload://iegnQaigsUcmZ13nZ174cZz21Yy.jpeg)
...oh and I just IP'd esk8 stomp pedals...sorry 😂
```

---
## \#61 Posted by: Luuke Posted at: 2018-04-13T07:55:06.644Z Reads: 153

```
Any update on that topic?
```

---
## \#62 Posted by: Jc06505n Posted at: 2018-04-13T15:05:06.020Z Reads: 155

```
Also interested, Though I wonder how it would be implemented in terms of activation and deactivation. Along with loading it onto the VESC. Hopefully @Ackmaniac or even @rpasichnyk is interested enough to play with or accept collaboration to add it on (time to dust off the old C)
```

---
## \#63 Posted by: killaton Posted at: 2018-04-16T02:24:33.969Z Reads: 151

```
Any updates?
Has anyone implemented a push kick, "endless ride" mode into an of the open source ESC?
Has anyone on esk8 made any remoteless builds yet?
```

---
## \#64 Posted by: webst Posted at: 2018-04-16T17:55:14.827Z Reads: 147

```
How would you like remotless setup to even work?
```

---
## \#65 Posted by: Jc06505n Posted at: 2018-04-16T21:04:53.695Z Reads: 145

```
From what I'm guessing a skate board that only assist in maintaining push speed with programmatic limits of how fast it can go. Though I don't know how you would stop such a set up, I am interested in the concept though. No motion sensors, no remote. Just a push-assist electric board.
```

---
## \#66 Posted by: killaton Posted at: 2018-04-16T23:43:10.411Z Reads: 148

```
[quote="webst, post:64, topic:48918, full:true"]
How would you like remotless setup to even work?
[/quote]

I started a new thread trying to answer that question here
http://www.electric-skateboard.builders/t/remoteless-build/52383/42
```

---
## \#68 Posted by: chuttney1 Posted at: 2018-04-29T01:15:56.666Z Reads: 136

```
Anyone can implement the feature if you know how to code either in C, C++ or something allowing detection of you pushing your board.
```

---
## \#69 Posted by: webst Posted at: 2018-04-29T12:39:01.033Z Reads: 135

```
[quote="chuttney1, post:68, topic:48918, full:true"]
Anyone can implement the feature if you know how to code either in C, C++ or something allowing detection of you pushing your board.
[/quote]

Great example of Dunning-Kruger effect
```

---
## \#70 Posted by: chuttney1 Posted at: 2018-04-29T17:16:07.693Z Reads: 132

```
https://i.redditmedia.com/dDe-jZA1HevSDmcraAsUTn1a4YyTE86FfvytbvfaHPU.png?w=1019&s=242308b94c488bd1d053ba99ea5dfa07
```

---
## \#71 Posted by: sunnyD Posted at: 2018-06-25T18:52:50.411Z Reads: 115

```
HEYO! I see someone else enjoys psychological principles.
```

---
## \#72 Posted by: brenternet Posted at: 2018-08-12T08:10:03.470Z Reads: 106

```
This thread is struggling with people who haven't watched the video or grasped the concept. I'd still really like to see this feature. 

Did any of you super smart gents look into this?

@okp  have you used a mellow board? I feel like if anyone could explain this it would be you.

I think it would be great to build a 30" cruiser with a tail, 10s2p and some spongy wheels to kick around in town.
```

---
## \#73 Posted by: bevilacqua Posted at: 2018-08-12T10:00:27.384Z Reads: 104

```
I built a 10s1p battery onto my normaly „analog“ Quinboards mini me (30“). Combined with a single 70mm hub it was mor than capable to assist. 

The only missing part was the seemles integration that the endless ride provides.
```

---
## \#74 Posted by: okp Posted at: 2018-08-12T13:29:25.268Z Reads: 99

```
Hey mate, yeah I did use one for 1 month. I only rode it in endless mode because to me it's the only interest I see for my riding style. 

The behavior is pretty easy to get, if my memories are correct
- You can push the trigger but if you don't roll, nothings happen (no acceleration)
- When you push, the boards keeps rolling and the speed decrease progressively over time
- Side effect is that if you are at speed, you have to adapt the way you push to get the good sync (because the mellow keeps the speed on the momentum), you have to get used to that when you go up hills.

I decided to try it at the maximum the endless can over which is doing a manual on the hubs all the way on the Inception bridge in Paris. Doing so, you have a complete feeling on how the drive reacts and it's sometimes weird (you need to get used to that), when you have littles micro edges on the ground, the wheels slow down (because of the force cause by the defects on the ground) and then accelerate back; that was the most challenging side to get this manual all the way.

I definitely agree on the fact that a 30" cruiser with a tail, 10S2P on endless ride would be dope. I don't think having the removable battery adds value in this anyway cause you can get serious range on endless ride (++30km  distance if you like to push and carve);

check my insta @ridewithokp I posted the wheeling on one of my videos stream

Cheers!
```

---
## \#75 Posted by: brenternet Posted at: 2018-08-12T14:16:35.952Z Reads: 103

```
Perfect, thank you for that.
```

---
## \#76 Posted by: okp Posted at: 2018-08-12T15:38:40.350Z Reads: 102

```
I got a feeling that the genius that work on the Unity is going to make this reality soon. I found the video - forget about the show off - but look/listen at how the wheels and hubs react to the ground structure.

https://www.youtube.com/watch?v=rmcBiXc-QtU
```

---
## \#77 Posted by: legend27 Posted at: 2018-10-27T18:36:43.347Z Reads: 78

```
I understand none of coding or how it works but I think it's the answer to this thread.

http://bitluni.net/diy-electric-scooter/

www.youtube.com/watch?v=QhxD5owuN8g&t
```

---
## \#78 Posted by: brenternet Posted at: 2018-10-27T18:50:13.940Z Reads: 74

```
I love this guys attitude :smiley:
```

---
## \#79 Posted by: brenternet Posted at: 2018-10-27T18:57:58.436Z Reads: 73

```
@Martinsp - 10 points if you make this work like he did.
```

---
## \#80 Posted by: Jc06505n Posted at: 2018-10-27T19:17:38.224Z Reads: 73

```
It has less to do with any antispark. It’s a software and possible hardware thing.
```

---
## \#81 Posted by: brenternet Posted at: 2018-10-27T19:24:16.473Z Reads: 74

```
Well yes, it's exactly what he said. Arduino, gyro and calibration. But @Martinsp is the type of person who pursue advancement like this.
```

---
## \#82 Posted by: mixedcreation Posted at: 2018-10-27T19:34:28.612Z Reads: 76

```
Seriously having this feature will be amazing. I wanted this feature for a long time now. As @okp said, endless ride with a 10s2/3p battery would make this a great city/university cruiser. 

My kid would love this shit when she has off time during her softball tournaments.  As well bringing a true stealth look that folks in certain cities need. This feature with a Hummie board...stealth mode to the max.
```

---
## \#83 Posted by: Jc06505n Posted at: 2018-10-27T20:04:06.866Z Reads: 75

```
Not that I’m doubting his skills , but as far as I’ve seen he’s only made Antisparks which he stills working to get the kinks out of. 

You would want @Wajdi who’s already implemented such a thing on his proton apperantly,

Or @Deodand who’s designing the Unity and has shown to have a good handle of Vedders work.
```

---
## \#84 Posted by: brenternet Posted at: 2018-10-27T20:09:21.185Z Reads: 72

```
or @janpom @Kug3lis 

Tag them all brother!
```

---
## \#85 Posted by: janpom Posted at: 2018-10-27T20:25:29.363Z Reads: 71

```
@brenternet There's no way I'm doing this. First, it's way beyond my skills. Second, I'm sure you would change its name! :smile:

Looks cool though.
```

---
## \#86 Posted by: brenternet Posted at: 2018-10-27T20:30:34.645Z Reads: 70

```
You're right, endless ride? I would try to relate the name to someones mom here and end up offending a bunch of people. Lets just let this one hang :call_me_hand:
```

---
## \#87 Posted by: Martinsp Posted at: 2018-11-19T18:34:00.413Z Reads: 59

```
I have tried making this but without an accelerometer. I used a sensor that senses the bend of the deck, when you push on your board you take some weight off your board and that triggered the throttle. It worked in theory but the board was so inconvenient to ride. I think that the major difference is that on a scooter you can hold on to the handlebars but on the skateboard I had trouble keeping the board under control. You can try this if you are curious by lightly pushing the throttle and kicking off. the board accelerates way too fast even with small amount of power because there is only a small amount of weight on it when you are pushing. I therefore ditched the idea, way too inconvenient and even more dangerous unfortuately
```

---
## \#88 Posted by: Vanarian Posted at: 2018-11-19T18:40:46.312Z Reads: 59

```
It would have been simpler to use an encoder instead. Just use wheel speed rotation to act as throttle! And find a way to program a smooth "let go of throttle"
```

---
## \#89 Posted by: Martinsp Posted at: 2018-11-19T18:44:00.748Z Reads: 58

```
Yeah actually, there are sensors in a lot of motors already I did not think of this. Maybe that could be the solution to this problem but then, lighter and heavier riders would need different percentage of power applied so I still think it would get too complex. Maybe there is a simple yet effective solution that I am missing now...
```

---
## \#90 Posted by: Vanarian Posted at: 2018-11-19T18:58:10.302Z Reads: 55

```
What about a duty cycle mode controlled via encoder? It will pull as many amps as needed to reach wheel speed no matter the load. 

Then there's still the soft let go throttle to account for, this and if too much resistance applied (ex : foot braking) soft cut and go freewheel?
```

---
