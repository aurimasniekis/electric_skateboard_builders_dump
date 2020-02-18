# Trampa truck steering dampening

### Replies: 76 Views: 3604

## \#1 Posted by: Kug3lis Posted at: 2017-11-22T02:27:58.350Z Reads: 319

```
Hi guys, I was browsing youtube and found this guy in Korea using bike radial steering damper on trucks to manage wobble and etc. Later on, by doing small research I found there are mechanical ones with a dial and electrical ones which use a 12V solenoid valve to manage the damping. Went on eBay found some second-hand electric steering dampeners cheaper than new mechanical. Was thinking it would be cool to connect the dampeners to VESC to get speed information and adjust the stiffness accordingly.

What do you think about this idea? I am thinking of something similar for my build


Here is the video I found:

https://youtu.be/aACAE_WaZEs

Here is damper on eBay (There are many different style and model available)

https://www.ebay.co.uk/itm/HONDA-CBR-1000-RR-2009-STEERING-DAMPER-BREAKING-PARTS-OE/232565721093?hash=item3625ff4805:g:Cw8AAOSw~epZiXGQ
```

---
## \#2 Posted by: Cobber Posted at: 2017-11-22T02:30:26.667Z Reads: 292

```
Yeah Nowind has a steering damper on his trampa and Moestooge also has one on his race board... search em out. There is a pic of Nowinds in the pic thread.
```

---
## \#3 Posted by: Kug3lis Posted at: 2017-11-22T02:31:15.375Z Reads: 286

```
Yeah I already found them I am just thinking about electrical version of this stuff :D Because to align two of them would be pain in the ass I guess
```

---
## \#4 Posted by: Cobber Posted at: 2017-11-22T04:21:17.108Z Reads: 269

```
Sounds cool bro :sunglasses: 
if you can make it work...
Will you be able to adjust front rear bias? that would be the shiznit
Fast turn in on the front, more stable rear...

Having a 4WD eSk8 with active yaw control would be awesome too! 
Do you think you could program that?
```

---
## \#5 Posted by: benjammin Posted at: 2017-11-22T05:10:20.542Z Reads: 249

```
Wait, so you mean the steering would automatically adjust depending on speed? That would be so sick! Is that doable, or did I misunderstand?

Like Cobber said, having the front looser than the rear would be the way to go if possible.
```

---
## \#6 Posted by: Kug3lis Posted at: 2017-11-22T10:33:31.310Z Reads: 237

```
[quote="Cobber, post:4, topic:38970"]
Will you be able to adjust front-rear bias? that would be the shiznit
Fast turn in on the front, more stable rear...
[/quote]

Yes, it should not be a big problem.

[quote="Cobber, post:4, topic:38970"]
Do you think you could program that?
[/quote]

I guess yeah

[quote="benjammin, post:5, topic:38970"]
Wait, so you mean the steering would automatically adjust depending on speed? That would be so sick! Is that doable, or did I misunderstand?
[/quote]

Yes, taking CAN/UART information from VESC RPM I guess because I don't think VESC outputs speeds, and map a graph of dampness for each range of value or have separate SERVO input to be able to control from remote.
```

---
## \#7 Posted by: Okami Posted at: 2017-11-22T10:58:53.403Z Reads: 215

```
The idea sounds really nice on 'paper'.

If this would be possible in real life that would be really great and would solve the wobble / loose truck problem entirely.. 

At least it sort of sounds like the missing piece on how to make board steer well at slower speeds but be stable when going faster

So yeh, im totally supporting pursuing this and trying it out.
```

---
## \#8 Posted by: Kug3lis Posted at: 2017-11-22T11:20:38.909Z Reads: 212

```
I will be trying to get one of those dampers in hand and play around :)
```

---
## \#9 Posted by: Cobber Posted at: 2017-11-22T11:31:10.220Z Reads: 220

```
I'm not sure if it means anything but on my motorbike I had better luck with the seals on the piston type
<img src="/uploads/db1493/original/3X/7/0/7078e6081a8942a176e53dd0b86f18f3a06a2a79.png" width="500" height="500">
than this sort of style (rotary type)
<img src="/uploads/db1493/original/3X/3/4/3465311a69f7acb63a2a24e72536911eeb8b0a47.png" width="500" height="500">
now I'm not sure if you will have the same experience but keep a open mind if you encounter any problems with seals.
```

---
## \#10 Posted by: Kug3lis Posted at: 2017-11-22T11:33:31.995Z Reads: 207

```
I will be using honda original part so I don't think it should fail, plus the load difference between real bike and longboard is day and night difference I think
```

---
## \#11 Posted by: Cobber Posted at: 2017-11-22T11:36:43.457Z Reads: 205

```
agreed load will be less, but possibly more vibration...
```

---
## \#12 Posted by: Kug3lis Posted at: 2017-11-22T11:49:20.303Z Reads: 206

```
Yeah, but you never know until you try :)
```

---
## \#13 Posted by: Cobber Posted at: 2017-11-22T11:55:35.098Z Reads: 213

```
don't give up, try, try, try again...
https://www.developgoodhabits.com/wp-content/uploads/2016/07/thomas-edison-success-quotes.jpg
could be next level stuff, the purists will hate it because it works!
```

---
## \#14 Posted by: Kug3lis Posted at: 2017-11-22T11:58:21.663Z Reads: 191

```
The only hard part I think is mounting it because it will need 90º mounting bracket
```

---
## \#15 Posted by: Cobber Posted at: 2017-11-22T12:13:40.214Z Reads: 194

```
what does your damper look like?
```

---
## \#16 Posted by: Kug3lis Posted at: 2017-11-22T12:15:04.914Z Reads: 200

```
I am thinking of buying this honda cbr https://www.ebay.co.uk/itm/HONDA-CBR-1000-RR-2009-STEERING-DAMPER-BREAKING-PARTS-OE/232565721093?hash=item3625ff4805:g:Cw8AAOSw~epZiXGQ
```

---
## \#17 Posted by: Kug3lis Posted at: 2017-11-22T12:17:12.224Z Reads: 199

```
I am scared that it will be way bigger than trampa truck itself :D
```

---
## \#18 Posted by: Cobber Posted at: 2017-11-22T12:17:27.907Z Reads: 204

```
what is your object? make a cool one for you or make a product?
```

---
## \#19 Posted by: Kug3lis Posted at: 2017-11-22T12:18:13.966Z Reads: 200

```
Now just make it work, but if it works maybe machine top part from nice single peace aluminium and already with mounting bracket for the truck.
```

---
## \#20 Posted by: Cobber Posted at: 2017-11-22T12:28:23.625Z Reads: 204

```
might be better off using a stock 2017 cost effective part, could be hard for numbers of other people to use what you learn.
can't wait to see what weight oils and valving you use to make it work.
```

---
## \#21 Posted by: Kug3lis Posted at: 2017-11-22T12:30:22.721Z Reads: 191

```
Ahm, you don't need anything much that stuff is everything inside. It has solenoid valve (2 pin connector) you control solenoid and it control how stiff it is
```

---
## \#22 Posted by: Cobber Posted at: 2017-11-22T12:45:24.782Z Reads: 192

```
the speed the valve works controls oil flow, but also oil weight controls how fast it moves chamber to chamber... I don't know digital but analog shocks  and dampers I have used and tuned.
```

---
## \#23 Posted by: Kug3lis Posted at: 2017-11-22T12:51:49.275Z Reads: 192

```
I don't really know much about this stuff, but as far as much I have done research I found similar stuff idea

https://youtu.be/cXyFDnqauik
```

---
## \#24 Posted by: ugothakd Posted at: 2017-11-22T14:14:35.965Z Reads: 188

```
I've thought about using small RC ball joints to mount dampener from truck to board (seeing as there will be a lot of motion)
```

---
## \#25 Posted by: Deckoz Posted at: 2017-11-22T14:44:46.107Z Reads: 186

```
Trampa trucks aren't made for speed. And anti wobble tech...should be all y'all practicing on slacklines and training them ankles...

Just saying, if your wobbling your skating out of your skill. Go ride an analog board down a hill, and learn to skate. Oh wait I already said trampa trucks aren't made for speed. So, ya know, don't use trampa trucks lol. Use a truck designed for the application...
```

---
## \#26 Posted by: Kug3lis Posted at: 2017-11-22T15:03:12.166Z Reads: 176

```
Yeah yeah, longboards were never intended to be propelled by electric motors...
```

---
## \#27 Posted by: Deckoz Posted at: 2017-11-22T15:14:18.075Z Reads: 185

```
Doesn't mean you should rely on engineering to self correct the board. Self correcting board but your body doesn't follow. 

These are boards that are ridden by a sense of balance.  Yea its great we have motors. But take away the feeling of the road and the sensation of balance and pressure of your feet and you have a plank of death. Just saying. Go ahead make some anti wobble tech vs taking the time to learn to skate and being able to let your ankles control the board. 

The issue with wobbles is the board controls your ankles because your ankles are weak. Adding some fancy tech will just make that worse if you still have no ankle control skill/strength. Your just asking to street your face.

You want a solution, buy a slackline. Use it.
```

---
## \#28 Posted by: Crossfire Posted at: 2017-11-22T15:49:40.223Z Reads: 184

```
While I really like what @Kug3lis is trying to achieve here as I'm a tech head myself, I do feel @Deckoz has a good point.

Good, quality trucks with appropriate bushings can solve bigger part of the problem. I did skate a little in my early years but only casually. So the transition to esk8 wasn't that odd...the bigger challenge imho are the higher speeds and the stance to control the board. That was new to me; riding 10 km/h on skate wheels VS 25km/h over mixed roads. 
I've found out that @okp's kind of snowboard stance is the best for daily commute; I just need to be ready when shit happens because on the road it usually does from time to time. He rides hard with trampa trucks but doesn't seem to mind the wobbles? :upside_down:
```

---
## \#29 Posted by: Kug3lis Posted at: 2017-11-22T15:51:12.679Z Reads: 185

```
No you did not understand... :D The problem is that sometimes I want for e.g. really flexiable board for low speed carving and etc, then you go higher speeds the really flexible is really pain in the ass and nothing can help you for this not even your hardcore ankles.

This stiffener it just limits how fast it can move that's all it does not help nothing with steering
```

---
## \#30 Posted by: Kug3lis Posted at: 2017-11-22T16:24:12.461Z Reads: 191

```
Plus this kind of stuff is also amazing

https://www.youtube.com/watch?v=jzNsYGzay70
```

---
## \#31 Posted by: Deckoz Posted at: 2017-11-22T16:37:28.248Z Reads: 187

```
I ride a flex 4 vanguard up to 40mph. Its a noodle. But its all ankles dude. 

I understood perfectly. I'll say it again, trampa trucks aren't designed for speed. And there's no replacement for ankles. And as @Crossfire said there's also no replacement for a proper truck setup. Trucks setup wrong just enhance the problem. 

Springs don't and never will behave like urethane bushings on a kingpin. The throw of the springs and dampas are not linear in compression like a urethane bushing at the proper duro. And the return to center is just straight up whack.
```

---
## \#32 Posted by: benjammin Posted at: 2017-11-22T16:48:16.384Z Reads: 182

```
@Deckoz 

Thing about mountainboards though with the straps and all, is you can't get into a tuck like you can on your vanguard. Much nicer feel at speeds with tight trucks, at least on the rear.
```

---
## \#33 Posted by: Deckoz Posted at: 2017-11-22T16:55:59.930Z Reads: 179

```
Dude look at the design of the kingpin on trampas. The axle sits ahead of the kingpin like tkp, not trailing behind the pivot point like RKP. They aren't speed trucks.

And tucking? Who mentioned anything about tucking. Sure you can tuck for speed but what good is it if you can't stand up to air check, or speed check. Being forced to ride in a tuck at x speed is just wrong. Your trucks need to be setup so all riding positions feel stable at all speeds, trampa and tkp are not speed trucks. Its that simple...
```

---
## \#34 Posted by: benjammin Posted at: 2017-11-22T17:02:22.105Z Reads: 175

```
@Deckoz 

See your point. I've never been much of a skater. Can't say I've ever had any wobbles on the mountainboard, just like the feel of tighter trucks when going over 30mph. Not so much when going slow though. Having them automatically adjust would be dope!
```

---
## \#35 Posted by: Deckoz Posted at: 2017-11-22T17:13:13.144Z Reads: 177

```
You want them tighter at speed because they slap less. The kingpin design with speed makes them want to rake back and forth. So having them tighter of course fights/minimizes that. 

But with traditional bushing trucks you want them as loose as possible(tight enough so you can barely spin the bushing with your fingers) at the proper duro for your weight. The rest is all ankles. 

Basically to make trampa trucks work at speed your doing the opposite of what you should be doing. To tight of a truck, once the oscillation starts the board will be controlling your ankles,vs your ankles setting and holding the desired angle.

You should be controlling your trucks at all speeds, and not your trucks controlling you, tight trucks will over power you. Its a real shame silverfish is gone, And that you guys don't practice on analog boards to really understand what's happening beneath your feet. And how different truck setups change your ride.
```

---
## \#36 Posted by: benjammin Posted at: 2017-11-22T17:52:21.315Z Reads: 166

```
I like the idea of using a slackline. Even with super ankles though, I still don't think I'd wanna ride these things over 30 with loose trucks.
```

---
## \#37 Posted by: Kug3lis Posted at: 2017-11-24T20:58:17.516Z Reads: 169

```
Today I ordered two pieces for 15£ each will see how they look :)
```

---
## \#38 Posted by: Cobber Posted at: 2017-11-28T02:23:27.643Z Reads: 173

```
[quote="Deckoz, post:35, topic:38970"]
Its a real shame silverfish is gone,
[/quote]
yeah, it was my go to for everything skate...
```

---
## \#39 Posted by: psychotiller Posted at: 2017-11-28T02:37:11.853Z Reads: 169

```
First of all, a Dampener doesn't soften or stiffen up anything. All it does is restrict quick movements and allow slower movements to happen. That's it. 

Employed on a truck isn't a bad idea. It really could shut down a speed wobble. But it isn't going to make you safer at higher speeds if you don't know how to shut down or foot brake.

It's going to give you a major false sense of security and get you into serious trouble quick. There's too many people on this forum reliant on electric brakes. Just what we need is people who have no business going 30mph doing it because they think it's safe.
```

---
## \#40 Posted by: benjammin Posted at: 2017-11-28T03:58:15.714Z Reads: 171

```
I'm failing to see the difference between 'stiffen' and 'restricting quick movement.'

I am ok at foot braking, and pretty comfortable doing a shutdown slide if need be, but certainly not when strapped into a mountainboard on pavement, so yeah I am definitely relying on the brakes, and/or my helmet 😕

Like I said before, I've never been much of a skater, so my understanding is limited. My background is mainly in snowboarding and wakeboarding. I was under the impression that holding a tuck was not only for  aerodynamics, but to position one's weight over the front truck as to prevent speed wobbles. 

Yeah, bummer about silverfish. I'd like to read up to get a better understanding of all this.
```

---
## \#41 Posted by: psychotiller Posted at: 2017-11-28T04:19:38.518Z Reads: 163

```
A steering damper in it's simplest form is a tube that has a hole in either end. It has a shaft that runs through it. The shaft has a baffle attached to it. The baffle has small holes in it to allow fluid to pass through it as it slides along the inside of the outer tube. 

Moving slow, the fluid passes thru fairly easy (allowing you to turn with no resistance)
But with fast movement the fluid can't get thru the holes fast enough to allow the baffle to move at that speed (dampening the movement) 

So, If you have a moment of quick movement that could turn into a series of worse movements, the dampening properties of fluid will prevail.
```

---
## \#42 Posted by: benjammin Posted at: 2017-11-28T05:48:46.289Z Reads: 162

```
Thanks for the info, so if I understand correctly, the main difference between a steering damper, and the dampening of normal mountainboard trucks is the resistance is constant throughout as opposed to being proportioned to steering angle. 

Wouldn't we still refer to the level of resistance as being tight or loose though?
```

---
## \#43 Posted by: psychotiller Posted at: 2017-11-28T06:06:34.260Z Reads: 160

```
No. Because dampening is being confused in this thread (a few times) with turn radius. Your turn radius is affected only by your choice of trucks and the degree of their baseplate. You will turn whatever radius the trucks will turn whether you have a steering dampener or not. The dampener only affects how fast your your lean angle can change. Not how sharp you can turn.

The level of resistance is dictated by the type of bushings you are using and how tight you set the nut on your kingpin.

Channel trucks, with springs and eggs, are just different altogether..They either turn super sharp and loose or hardly turn at all if you have eggs in the springs. They aren't made for street. Never were. 
For a dampening system to actuallybe able to work well on channel trucks you would need to ride without eggs.
```

---
## \#44 Posted by: benjammin Posted at: 2017-11-28T07:03:15.660Z Reads: 149

```
Aargh, confusing lol. I'll have to read up more on this when I have the headspace for it. When saying tight or loose though, I was referring to the trucks resistance to turn, not necessarily the turning angle.
```

---
## \#45 Posted by: psychotiller Posted at: 2017-11-28T07:08:00.603Z Reads: 152

```
We could be saying different things but meaning the same...haha
```

---
## \#46 Posted by: thisguyhere Posted at: 2017-11-28T07:12:12.905Z Reads: 163

```
https://thumbs.gfycat.com/MajorMemorableHerring-small.gif
```

---
## \#47 Posted by: Flexboardz Posted at: 2017-11-28T12:57:34.674Z Reads: 164

```
Steering dampeners have been used on some e-boards like Gnarboard (see pics below) or Bajaboard 
http://outbackprague.com/wp-content/uploads/2015/06/ESKate-Promo.jpg

However, it might be time to improve trucks technology to have maniability, stability, improved grip,...
http://flexscoot.com/modules//smartblog/images/43-single-default.jpg
```

---
## \#48 Posted by: rene Posted at: 2017-11-28T13:11:38.522Z Reads: 161

```
Great YT Video - we should combine our Trampa Trucks with motor bike steering dampers controlled by arduinos.
If our speed is getting higher, the arduino hardens the dampers. If we ride low speed, the arduino weill loosen the dampers.

How about taking the steering dampers for a Honda Monkey for front and back Trampa Trucks and trying to design a servo motor to adjust these - while driving.

Of cause we would then remove the original trampa rubber dampers .
```

---
## \#49 Posted by: Kug3lis Posted at: 2017-11-28T13:19:51.885Z Reads: 163

```
You cant remove rubber dumpers, this whole thing is just for slowing down the turning speed of truck. Rubber dampers and springs are for suspension not turning. You can't use servos for turn manual dampers because its 4-5x 360º turns
```

---
## \#50 Posted by: MoeStooge Posted at: 2017-11-28T15:39:03.470Z Reads: 163

```
My personal experience with running a damper on the rear truck is it soaks up and softens my mistakes and road anomalies for recovery and control. RAF recovery after Fuckup...<img src="/uploads/db1493/original/3X/2/4/243d26be60f2d25f3026f07c56cd703e9f9edfd2.jpg" width="690" height="388">
```

---
## \#51 Posted by: chaka Posted at: 2017-11-28T16:58:43.274Z Reads: 160

```
R.I.P. if you ever need to avoid something. Listen to @Deckoz and dampen your steering with stronger ankles.
```

---
## \#52 Posted by: Okami Posted at: 2017-11-28T17:57:56.677Z Reads: 159

```
[quote="MoeStooge, post:50, topic:38970"]
road anomalies for recovery and control.
[/quote]

I would be with @MoeStooge in this point.. im not sure what cat reflexes are needed but someone should try hitting obstacles at speed.. be it branches, bumps, cracks whatever.. and see how it feels, especially if trucks are a bit loose.

So yeh, I guess im also on the 'Technical' side, supporting the dampener to avoid such drastic shifts in movement after bumps or other irregularities on road. 

---
I had a video with longborder hitting a bump/crack and afterwards wobbling and crashing, too bad I lost it.

---

@Flexboardz Thanks for bringing up the pictures, on a side note I think GnarBoards had somewhat good design / technology, too bad they couldnt handle it or the price was too steep or what not that they disappeared.
```

---
## \#53 Posted by: Kug3lis Posted at: 2017-11-28T18:00:13.187Z Reads: 150

```
Oh you already running with electronics?
```

---
## \#54 Posted by: MoeStooge Posted at: 2017-11-28T18:12:48.557Z Reads: 147

```
Solenoid switched.  CBR1000.
```

---
## \#55 Posted by: Kug3lis Posted at: 2017-11-28T18:13:58.555Z Reads: 147

```
I ordered the same ones I think
```

---
## \#56 Posted by: Flexboardz Posted at: 2017-11-28T18:26:05.047Z Reads: 150

```
adding 21th century technology (electronic control) to correct the defaults of a 19th century technology (skate trucks) seems a bit overengineered to me...
```

---
## \#57 Posted by: Deckoz Posted at: 2017-11-28T19:00:29.188Z Reads: 150

```
I hit rocks, branches, road turds, squirrels, snakes. I'm still saying its all ankles and a proper bushing setup

You see you need strong enough ankles to hold pressure on the rail so that the truck and wheel move around the object and the board stays at the same deflection. The board staying at the same angle will return the trucks to the previous tracking after hitting an object
```

---
## \#58 Posted by: MoeStooge Posted at: 2017-11-28T19:09:49.554Z Reads: 151

```
Over 35 mph is where the damper makes a noticable difference. I cant give you any objectional comparison as my setup is unique. Sorry about your road rash @Deckoz chicks do dig scars👍.
```

---
## \#59 Posted by: Deckoz Posted at: 2017-11-28T19:20:05.572Z Reads: 153

```
Tis but a fleshwound, all healed. I just know RKP are made for me...and Trampa and TKP are not my cup o tea. There's a good reason all the guys going 50+ downhill are mostly RKP...just feels right.
```

---
## \#60 Posted by: Kug3lis Posted at: 2017-11-30T19:05:49.652Z Reads: 157

```
Received today dampers, removed all unnecessary parts in the end left with pretty decent looking stuff. Then applied full 12V I was not able to turn with a small wrench.

<img src="https://i.imgur.com/U5eKN0K.jpg"/>

<img src="https://i.imgur.com/qoFODeH.jpg"/>
```

---
## \#61 Posted by: MoeStooge Posted at: 2017-11-30T20:53:07.602Z Reads: 149

```
Yuup same. Run mine off the BEC, think it pulls just over 1a @ 6v.
```

---
## \#62 Posted by: Kug3lis Posted at: 2017-11-30T21:14:22.039Z Reads: 147

```
You running it just from plain DC? No pwm?
```

---
## \#63 Posted by: Kug3lis Posted at: 2017-11-30T21:15:03.348Z Reads: 148

```
With my crappy setup I measured 60º turn angle from side to side
```

---
## \#64 Posted by: MoeStooge Posted at: 2017-11-30T21:27:13.030Z Reads: 145

```
That's a big negative on the Pulse Width Modulation. 6v cc dc
```

---
## \#65 Posted by: Kug3lis Posted at: 2017-11-30T21:29:37.790Z Reads: 141

```
If you control mosfet using PWM you practically have CC
```

---
## \#66 Posted by: Kug3lis Posted at: 2017-11-30T21:30:31.681Z Reads: 137

```
That's how bikes control it using info from speed sensor
```

---
## \#67 Posted by: MoeStooge Posted at: 2017-11-30T21:32:19.363Z Reads: 137

```
Yuup. 6v cc happened to be the sweet spot and was convenient and simple. Cool thing is if ya wanna go crazy with telemetry, the option is there. Me I'm happy with the dial a damper and the kiss approach.
```

---
## \#68 Posted by: Kug3lis Posted at: 2017-11-30T21:39:53.234Z Reads: 137

```
I mean I understand you, but you could just went with a manual would be easier... :D I picked this so I could control it but oh well ;)
```

---
## \#69 Posted by: MoeStooge Posted at: 2017-11-30T21:50:59.802Z Reads: 138

```
Form and function. Picked it up from a cycle recycler for under 10bucks. The layout was an easy install and am able to turn it on/off. It gives my board a nice feel under 35mph but not necessary. Over 35 it lowers the oh shit factor considerably. I think you will like these.
```

---
## \#70 Posted by: Kug3lis Posted at: 2017-11-30T21:52:49.824Z Reads: 143

```
How is the turning angle? Is it alright?
```

---
## \#71 Posted by: MoeStooge Posted at: 2017-11-30T21:55:34.575Z Reads: 145

```
It has plenty of throw. Won't be an issue.
```

---
## \#72 Posted by: Yecrtz Posted at: 2017-11-30T21:55:38.192Z Reads: 152

```
And I'm riding my Trampa here every day up to 45ish km/h without dampa's or anything. Just pure springs. :sweat_smile:
```

---
## \#73 Posted by: trampa Posted at: 2017-12-01T22:08:14.420Z Reads: 152

```
KIS - keep it simple!  Tom hit 57.6 Kph with yellow Dampas installed. All those extra parts just make your board heavy and complicated. Riding off-road is a lot of fun and usually you don't set a speed record on loose terrain. 

Have a look at the night time session video to see what performance you can get from a standard setup. 
Yellow dampas installed...

https://www.instagram.com/trampaboards/

Frank
```

---
## \#74 Posted by: Kug3lis Posted at: 2017-12-19T21:36:07.894Z Reads: 139

```
We just took apart that damper, to figure out if possible to make custom top plate, it looks like it's doable so will try to work on it too as I am finishing my work on gearbox.
```

---
## \#75 Posted by: tonycamaro427 Posted at: 2018-09-15T17:15:18.154Z Reads: 92

```
![7d032b5f5b62c99f94802d8ecf257550--electric-skateboard-skate-longboard|667x500](upload://p2YY61Tu2AYathBwBddrz4BzQKQ.jpg)![thPYL4S1XQ|474x282](upload://hkIGDPYZ3e7qzyFC40rnQqpCO6q.jpg)![th1KX2CW7V|474x355](upload://seI25wQFMNQlmpCj1x1vR32yIt2.jpg)I forgot about these guys Gila Boards independent suspention
```

---
## \#76 Posted by: tonycamaro427 Posted at: 2018-09-15T17:26:40.057Z Reads: 89

```
Perfect Video    electronic adjustable damping  some have a knob you can turn, to do it manually.
```

---
