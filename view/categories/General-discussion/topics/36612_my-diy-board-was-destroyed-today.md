# My diy board was destroyed today!

### Replies: 104 Views: 5780

## \#1 Posted by: quietbun Posted at: 2017-10-27T03:08:35.388Z Reads: 635

```
Hello All,

I got into an accident today. Luckily, no one was hurt, I got myself some road rash in elbow. Here is what happened. I was on my way to the bart train station in San Francisco to go home, from work. At the last stop, for some reason, I could not slowdown or brake, although I saw that the remote is still connected. I decided to bail and jump off, trying to run a few steps before I landed on the street. Unfortunately, my board decided to continue its journey by itself at the same constant speed. It ended up under the electric bus/train wheel and caught on fire.

There are 2 things I'd like to discuss:
1.  Firstly, please make sure that we all have protective gear, and ride that the speed that we can jump and run off. I'm glad that I don't max my speed in the city often.
2.  Second is a question. What could have happened with the vesc to disable my brake? It has been very reliable board. The only difference between today and other is the hot temperature at around 86F degree.

My board configuration is:
+  10s4P battery with BMS (group buy)
+  Maytech vesc
+  6454 motor
+  Maytech new mini remote contorller

I setup my vesc to freewheel if controller is disconnected. But I don't think it is the case, because the controller connection light was always on.

Although I will be boardless for a long while, I'd like to learn if I did anything wrong with my build. Thanks!

My vesc setup:
<img src="/uploads/db1493/original/3X/d/9/d94a3a40999b4820633dd84326a9ef0193661476.png" width="690" height="288">

My board turned into 3 pieces:
<img src="/uploads/db1493/original/3X/9/c/9cd9eabfb7db6f010cadf578a2151d6af14a4cfb.jpg" width="666" height="499"><img src="/uploads/db1493/original/3X/b/e/be76d9cbd41e4483a34e0e2209ae9fc7273e461a.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/0/d/0dba6dfa7637cd4848251866501c93a35946b654.jpg" width="666" height="500">
```

---
## \#2 Posted by: Boardnamics Posted at: 2017-10-27T03:14:00.484Z Reads: 589

```
Woah, every time I see one of these posts I get real nervous. Next think I know my board will cause a California wild fire...
```

---
## \#3 Posted by: DilatedPupils Posted at: 2017-10-27T03:15:13.905Z Reads: 581

```
Then they're gonna get banned.
```

---
## \#4 Posted by: cryo Posted at: 2017-10-27T03:16:43.828Z Reads: 572

```
I'll take those flywheels off your hands if they're not too damaged :slight_smile:
```

---
## \#5 Posted by: Mikenopolis Posted at: 2017-10-27T03:16:54.363Z Reads: 568

```
That's crazy!  Did you do the fail safe where you board slows down when your remote disconnects? Thats one thing I always do or else the board goes full throttle when connection is lost
```

---
## \#6 Posted by: Mikenopolis Posted at: 2017-10-27T03:17:28.597Z Reads: 552

```
Too soon ...Too soon (I was thinking the same thing)
```

---
## \#7 Posted by: thisguyhere Posted at: 2017-10-27T03:18:00.357Z Reads: 549

```
@psychotiller I remember you telling me about this where the board can take off, I don't recall the procedure to avoid this.
```

---
## \#8 Posted by: ARetardedPillow Posted at: 2017-10-27T03:18:29.981Z Reads: 535

```
you use the binding plug to set the failsafe @thisguyhere
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-10-27T03:18:39.099Z Reads: 527

```
u opportunistic dick, let the smoke settle at least goddammm....
```

---
## \#10 Posted by: Mikenopolis Posted at: 2017-10-27T03:19:26.107Z Reads: 516

```
After everything is said and done. Do the remote binding again. Pretty sure that's what @Michaelinvegas said when I learned about fail safe check
```

---
## \#11 Posted by: quietbun Posted at: 2017-10-27T03:19:30.236Z Reads: 504

```
I did the fail safe to have it slow to nutural position. However, as I said, the connection light was always on but I lost control completely.
```

---
## \#12 Posted by: ARetardedPillow Posted at: 2017-10-27T03:19:31.902Z Reads: 497

```
sorry for your loss.. must be hard, Id cry if my board just disappeared one day
```

---
## \#13 Posted by: Ackmaniac Posted at: 2017-10-27T03:19:55.602Z Reads: 496

```
Did you adjust the failsafe correctly for the remote?
Did the board still give some power or did it idle after you jumped off. Because you said that it continued at the same speed.
How long did the board not respond until you jumped off?
```

---
## \#14 Posted by: thisguyhere Posted at: 2017-10-27T03:19:56.986Z Reads: 485

```
make a second board for insurance
```

---
## \#15 Posted by: quietbun Posted at: 2017-10-27T03:20:29.568Z Reads: 491

```
Hahah the flywheel looks fine from the outside but the cores are destroyed.
```

---
## \#16 Posted by: BigBoyToys Posted at: 2017-10-27T03:21:19.724Z Reads: 489

```
Did the police come and take report?
```

---
## \#17 Posted by: cryo Posted at: 2017-10-27T03:21:22.952Z Reads: 491

```
Haha it was a joke (semi-srs).

@quietbun what are your timeout settings in the app configuration/general tab?
```

---
## \#18 Posted by: Mikenopolis Posted at: 2017-10-27T03:21:33.440Z Reads: 482

```
Scary. Would really like to know what went wrong then. Glad no one was hurt....Except your baby
```

---
## \#19 Posted by: BigBoyToys Posted at: 2017-10-27T03:21:48.435Z Reads: 475

```
Glad you are ok though, looks like a beautiful build. Im.sorry for your loss.
```

---
## \#20 Posted by: quietbun Posted at: 2017-10-27T03:21:57.430Z Reads: 470

```
It did fail safe setting and tested it throughly for week. It lost control for 5 seconds before I jumped off. And it continues with same speed.
```

---
## \#21 Posted by: Ackmaniac Posted at: 2017-10-27T03:23:08.487Z Reads: 446

```
So the board still had some power output but you could not control it anymore?
```

---
## \#22 Posted by: quietbun Posted at: 2017-10-27T03:23:12.398Z Reads: 444

```
Yes, polices, fire truck, and everyone on street, it was like a party... I felt so sorry about it though.
```

---
## \#23 Posted by: Mikenopolis Posted at: 2017-10-27T03:25:10.691Z Reads: 444

```
Tempted to just put loop keys on a long paracord pull strap on my boards just in case.
```

---
## \#24 Posted by: quietbun Posted at: 2017-10-27T03:25:39.449Z Reads: 443

```
I think it was around 0.4 second.
```

---
## \#25 Posted by: thisguyhere Posted at: 2017-10-27T03:26:20.636Z Reads: 445

```
people on the train must have been pissssssed..

is the city going to find you culpable for damages?
```

---
## \#26 Posted by: quietbun Posted at: 2017-10-27T03:26:34.006Z Reads: 443

```
Yes, the motor keeps on going with or without me on the board
```

---
## \#27 Posted by: Ackmaniac Posted at: 2017-10-27T03:27:11.461Z Reads: 442

```
Is this the remote?

https://de.aliexpress.com/item/Maytech-mini-size-remote-controller-for-electrical-remote-control-longboard/32724943691.html?spm=a2g0x.search0302.3.100.jNtTyl&ws_ab_test=searchweb0_0,searchweb201602_0_10536_10538_10537_10539_10055_10177_10056_10059_10534_10533_10060_10180_100031_10184_10107_10547_10304_10307_10548_10341_10186_10065_10142_10340_10068_10343_10541_10342_10103_10345_10102_10344_10302_10194_10073_10193_10152_10151_10319_10154_10155_10312_10314_10313_10084_10083_10321_10320_10322,searchweb201603_0,ppcSwitch_0&algo_pvid=df8b2f26-dd06-494d-a004-96a79a038b1f&algo_expid=df8b2f26-dd06-494d-a004-96a79a038b1f-13
```

---
## \#28 Posted by: quietbun Posted at: 2017-10-27T03:28:27.933Z Reads: 428

```
Yes that's the remote controller.
```

---
## \#29 Posted by: quietbun Posted at: 2017-10-27T03:30:33.454Z Reads: 426

```
Yes, I cried from the inside for a short while. But I'm glad no one was hurt, and the train bus was not damaged.
```

---
## \#30 Posted by: Ackmaniac Posted at: 2017-10-27T03:33:04.552Z Reads: 435

```
Sounds to me that the issue is coming clearly from the remote. I don't know how to adjust the failsafe on that remote but when it still gave throttle and you set the timeout to 0.4 seconds then the receiver gave a signal to the vesc which the VESC understood as a throttle command.

Possible reasons are a wrong adjusted failsafe signal,
or the receiver needs too long to switch to the failsafe signal,
processor on the remote or receiver freezed,
potentiometer on the remote came loose and gave a wrong signal

With a PPM remote the timeout on the VESC only get's triggered when the receiver is disconnected.  Because when the connection is lost then the receiver sends a failsafe signal so the VESC doesn't know that there is a connection loss.
A solution to still let the VESC detect a connection loss is available in my new firmware mod bat that's another story.
```

---
## \#31 Posted by: quietbun Posted at: 2017-10-27T03:36:21.391Z Reads: 420

```
Oh oh, that's right. I dont think I did the fail safe configuration on that remote. I dont know if there is way to do it. I did for the other one which takes 2 AA batteries.

But I'm I did test the fail safe many times before taking it on the road.
```

---
## \#32 Posted by: gbutcher Posted at: 2017-10-27T03:37:44.159Z Reads: 416

```
Damn sorry to hear this and see the carnage.  Glad you are OK.
```

---
## \#33 Posted by: quietbun Posted at: 2017-10-27T03:38:55.658Z Reads: 414

```
Yes, they were pissed including the train driver. I think everything was fine except my board, there was no damage to the train.
```

---
## \#34 Posted by: Jinra Posted at: 2017-10-27T03:41:37.228Z Reads: 404

```
I remember this board! Yuen right?
```

---
## \#35 Posted by: quietbun Posted at: 2017-10-27T03:43:17.793Z Reads: 393

```
Yeah, we met at a group ride. You tested ride that exact board.
```

---
## \#36 Posted by: Sapphirinia Posted at: 2017-10-27T03:46:29.870Z Reads: 389

```
Aww, that sucks. Sorry for your loss. I died inside the other day when I left my board at the playground parking lot. My heart dropped when I drove back and saw it sitting there. That drive back was stressful enough. I can't imagine how you feel.
```

---
## \#37 Posted by: Mikenopolis Posted at: 2017-10-27T03:46:42.996Z Reads: 380

```
Wondering if you cause any couples' fight tonight

"Some a$$hole ran his skateboard under the bus, stopped it and started a fire"

"A skateboard? Stop a bus? And bursted into flames? Bull$hit! Who were you really with!?" Huh? Huh? Huhhhhh?
```

---
## \#38 Posted by: Jinra Posted at: 2017-10-27T03:48:08.582Z Reads: 378

```
I'm sorry to hear :( I'm glad you're okay though, that's pretty crazy.

There's a lot that could've gone wrong, and after it's destroyed and burned like that, it's probably impossible to tell what happened. Maybe a vibration knocked off the PPM cable, or maybe the VESC threw a fault (there's a couple delay where it will not take input after a fault. You can change the delay time though), or maybe some other cable came loose.
```

---
## \#39 Posted by: Mikenopolis Posted at: 2017-10-27T03:52:02.776Z Reads: 371

```
Hmmm maybe we should do that test and pull the PPM cable as we throttle and see what happens?
```

---
## \#40 Posted by: Ackmaniac Posted at: 2017-10-27T03:53:29.621Z Reads: 379

```
PPM receiver cable comes loose  = VESC starts timeout after 0.4s
VESC has a fault = no power at all

So the VESC still got a signal from the receiver which told it to give some power.
So if everything quietbun is telling is correct the problem came clearly from the remote or receiver. So if the failsafe was setup the correct way then something else fucked up. But the problem is clearly coming from that component.
```

---
## \#41 Posted by: Jinra Posted at: 2017-10-27T04:01:15.016Z Reads: 348

```
VESC would time out (default 1 second I believe), but by default there's no braking current set for timeouts.
```

---
## \#42 Posted by: Ackmaniac Posted at: 2017-10-27T04:02:44.490Z Reads: 348

```
He said already he adjusted it to 0.4 seconds. And when the timeout is triggered it gives no power or brakes. But it doesn't give power.
```

---
## \#43 Posted by: Jinra Posted at: 2017-10-27T04:03:40.569Z Reads: 346

```
Man I need to read better.
```

---
## \#44 Posted by: Mikenopolis Posted at: 2017-10-27T04:12:53.641Z Reads: 341

```
So definitely the remote huh?
```

---
## \#45 Posted by: quietbun Posted at: 2017-10-27T04:18:45.581Z Reads: 334

```
I don't know the exact cause. And I run out of equipment to test or reproduce the issue ;(. But yes, I can confirm the constant speed before and after I jumped off. Could it be the vesc was overheat and misbehave?
```

---
## \#46 Posted by: cryo Posted at: 2017-10-27T04:21:02.934Z Reads: 334

```
My votes with the remote. If you still have it maybe you can do some testing with it and find out, exactly how idk maybe ackmaniac can think of something.
```

---
## \#47 Posted by: quietbun Posted at: 2017-10-27T04:21:16.649Z Reads: 333

```
Yes, I agree there are number of potential issue; but the board was working fine a whole 10 minutes before this issue. I accelerated after a stop light, and my remote lost control.
```

---
## \#48 Posted by: quietbun Posted at: 2017-10-27T04:22:35.968Z Reads: 333

```
Unfortunately, I don't have the receiver anymore, it was threw away together with a whole mess of battery, vesc.
```

---
## \#49 Posted by: Michaelinvegas Posted at: 2017-10-27T04:32:46.217Z Reads: 335

```
I have to agree with @Ackmaniac that is some type of remote issue...not sure if it’s related to the actual signal or settings. 

Man this Esk8 crashes are getting more and more epic
```

---
## \#50 Posted by: cryo Posted at: 2017-10-27T04:47:27.975Z Reads: 319

```
Its only a matter of time until someone makes the news.
```

---
## \#51 Posted by: Michaelinvegas Posted at: 2017-10-27T05:20:50.747Z Reads: 321

```
[quote="cryo, post:50, topic:36612, full:true"]
Its only a matter of time until someone makes the news.
[/quote]

Tis true.. .... eh...people get hurt or killed all the time....it’s when it becomes major property damage...now that’s when we are fucked....let’s just say that fire set the whole dang train 🚂  set a blaze 🔥 lol holy cheese and biscuits Batman...that’s when we get under the microscope and people start really paying attention.  

Maybe we start collectively, some how police ourselves, by maybe setting up some standard rules of the road type stuff that’s common sense but not too restrictive. A difficult balance. Maybe some safety tips in various subjects. Maybe we have people re check some of the components that were used in his build, maybe other people have experienced the same issue. Collecting that type of data would be useful in many different ways.

Just ideas to keep the party going under the nose of the man.
```

---
## \#52 Posted by: cryo Posted at: 2017-10-27T05:43:13.495Z Reads: 307

```
I mean technically most of the production boards are actually illegal in CA according to the esk8 law which includes boosted/evolve, not to mention the DIYer. The law def needs to be changed as I've read somewhere that the law was heavily influenced by an esk8 company to have the it specifically cater to their boards specs of having a speed of 20mph or less. Lobbying at its finest.

More attention could be both good or bad depending on the circumstances.
```

---
## \#53 Posted by: Jinra Posted at: 2017-10-27T05:47:07.522Z Reads: 302

```
Huh? Most production boards are not illegal in CA. Some are illegal, but most fall within the legal realm. Even those that have higher than legal wattage ratings are okay simply because it's impossible to enforce.
```

---
## \#54 Posted by: cryo Posted at: 2017-10-27T05:53:23.446Z Reads: 295

```
I'm just going straight off this thread 
http://www.electric-skateboard.builders/t/lets-break-down-the-california-electric-skateboard-law-ab-604/12714
not aware if the laws been changed recently.

Near the middle says maximum speed of 20mph. While its true no cop is gonna pull you over and check out your 18650 cells, it could be bad though if you somehow end up in a courtroom situation which is entirely possible given what happened to quietbun.
```

---
## \#55 Posted by: Jinra Posted at: 2017-10-27T05:55:01.213Z Reads: 272

```
yea that's why nearly all mfg's limit their speed, but really no one's gonna bust you for going 22mph either. Also, the law, IIRC, only applies the wattage limit at the motors, not discharge potential or watt hours of a pack.
```

---
## \#56 Posted by: cryo Posted at: 2017-10-27T06:07:18.232Z Reads: 290

```
Yea I have yet to see anyone get pulled over in SF for riding their board. Most cops don't even give a second glance. How you find yourself in a courtroom is a different matter though. 

What I'm saying is if someone finds themselves in a courtroom talking with a judge, they might refer to the law and see it stating max speed 20mph while boosted and evolve are blatantly advertising 22mph+ top speed. I've never been in a courtroom so I don't know how closely judges follow the law or how lenient they are. 

Makes me wonder what happened to the guy in this thread
http://www.electric-skateboard.builders/t/putting-californias-electric-skateboard-law-to-the-test-can-it-get-me-out-of-a-ticket/35204
```

---
## \#57 Posted by: Jinra Posted at: 2017-10-27T06:08:41.869Z Reads: 267

```
It's not illegal to have a board that goes over 20mph though, it's only illegal to **go** 20mph. Like cars they can go much faster than our speed limits, whether or not you do determines whether or not you're breaking the law.
```

---
## \#58 Posted by: cryo Posted at: 2017-10-27T06:12:52.723Z Reads: 292

```
Gonna quote evoheyax

[quote="evoheyax, post:1, topic:12714"]
So to meet the legal definition of an "electrically motorized board", your board can't run at more than an average of 1000 watts, or be capable of more than 20 mph.

If you don't meet this definition, your board is still classified as a motorized skateboard, which this law re-affirms is illegal...


(a) A motorized skateboard shall not be propelled on any sidewalk, roadway, or any other part of a highway or on any bikeway, bicycle path or trail, equestrian trail, or hiking or 
recreational trail.
(b) For purposes of this section, an electrically motorized board, as defined in Section 313.5, is not a motorized skateboard.


So there is is, in black and white. If your board is capable of more than 20 mph, your board doesn't meet the definition of an "electrically motorized board", which means you board is a "motorized skateboard", which this law reaffirms is illegal to ride basically any wheres in public.
[/quote]

The law mentions the design of the board based on whether or not it is capable of 20mph+, drawing a line between electric skateboard or motorized skateboard (which is illegal apparently).
```

---
## \#59 Posted by: Jinra Posted at: 2017-10-27T06:15:09.866Z Reads: 276

```
ah guess I remembered wrong. There are a lot of boards that fit the bill (literally) though. Riptide, Meepo, Genesis/Koowheel. The cheaper boards should fall within legality.
```

---
## \#61 Posted by: trigger4point7 Posted at: 2017-10-27T08:07:49.844Z Reads: 262

```
Those trains are on market, also embarcadero, I was on market and I saw an ambulance and fire truck behind me. I'm not sure if it was for this accident but just after that one street over I no doubt was being stalked by cops! They pulled over waited for me to pass and then pulled right behind me. I just followed the rules as if I was a car. I've never seen that before, it definitely was odd. Probably a coincidence.
```

---
## \#62 Posted by: Nordle Posted at: 2017-10-27T08:15:16.108Z Reads: 257

```
Best solution for me is not to ride in the city, or any place with a lot of people/traffic.
```

---
## \#63 Posted by: quietbun Posted at: 2017-10-27T08:19:46.618Z Reads: 255

```
Yep, I've been following traffic rule, stop and yield to pedestrians. I always ride below 17mph. Thankfully the speed was slow and no one was hurt. We tried our best to put out the fire before the firetruck came. This is unfortunate, and I spoke to city Train authority, police and the Fire Fighter. There was no issue, or ticket of any traffic violation. My post was to raise concern about losing control during ride, and potential accident.
```

---
## \#64 Posted by: sunerphey Posted at: 2017-10-27T08:21:29.471Z Reads: 255

```
I've had the same issue, but with wired thumb throttle controls, in some cases damaging permanently the adc pins of the microcontroller. It was because of voltage spikes. I suggest not riding a vehicle without the skills/means to control it offline.
```

---
## \#65 Posted by: pixelsilva Posted at: 2017-10-27T09:55:41.431Z Reads: 258

```
The dang Market Street in San Francisco is a burial site for skateboarders. This is the second mishap this week. I just saw a video post of a local e-boarder eating his teeth on Market's uneven 150-year old-pave-street car-rail-crissxcrossed-reef looking surface.

That **cryo** is an insensible dude. (but hey **quietbun**, if you want to get rid of them flies :bee: I wouldn't be mad if you give me a call) :innocent:
```

---
## \#66 Posted by: cryo Posted at: 2017-10-27T12:43:27.767Z Reads: 243

```
Yea you dont realise how shitty the roads really are until you ride an esk8. I actually had a close encounter like this too on third street because of an elevated crack in the middle of the road that caused me to get thrown off. Thankfully my board flew into the middle inbetween the two tracks near the platform and the only damage was to the nose of the board.
```

---
## \#67 Posted by: Battosaii Posted at: 2017-10-27T12:54:33.713Z Reads: 251

```
That sucks man i know how much it can hurt spending so much time effort and money on a project only to see it go just like that its happened to me with Cars. Just be glad you are alive and well to keep going and making new projects that are better than ever!

it did sound like a remote problem in hindsight it may have worked again if you powered down the remote and back on again while still on the board but things happen so fast that if you havnt already thought about what to do in a situation by the time you figure it out its too late. Its scary because no amount of foot braking or sliding would have stopped the board.
```

---
## \#68 Posted by: Mikenopolis Posted at: 2017-10-27T13:22:21.335Z Reads: 243

```
My two main boards uses the Raptor 1 deck where the power button in on top of the deck. Maybe having it is not a bad design after all since that would've prevent this runoff if you reach down and turn the board off.
```

---
## \#69 Posted by: b264 Posted at: 2017-10-27T14:35:20.692Z Reads: 242

```
[quote="evoheyax, post:1, topic:12714"]
has an electric propulsion system averaging less than 1,000 
watts
[/quote]

Also note the magic word "averaging" --- so if you have dual 7000 watt motors but an average of your power on your trip is under 1000W then you are okay.  The average will almost always be under 1000W.  Especially if you get technical and include the times when you apply brakes as negative wattage, which technically, it is.
```

---
## \#70 Posted by: Battosaii Posted at: 2017-10-27T14:53:51.822Z Reads: 233

```
yea i have a raptor too and my foot never turns off the board while riding and my DIY drop deck board has the switch on the right hand side of the encloser so i can reach down and shut it off too.
```

---
## \#71 Posted by: DougM Posted at: 2017-10-27T14:55:38.180Z Reads: 253

```
It might be time to start talking about a deadman sensor on the boards, so when you come off they immediately (or after a short delay) brake.  I had a runaway too, which fortunately just immolated itself on a chain-link fence.  

Because my boards are weird and have an aluminum frame it was easy to put one on by putting a pressure sensor and some foam between the frame and the wood.  Then when you come off the board the wood de-flexes and the sensor knows that I'm not on the board anymore.  Of course this was a pain in the ass for testing so I don't currently have it turned on in the code.  But I should.

On the regular decks that most of you run it's a bit harder but I bet there's something in the interaction between the battery case and the deck that you could take advantage of.

We should seriously consider this for all our builds because as said above, if we get too many fires or somebody gets hit by a runaway board we're likely to get banned.
```

---
## \#72 Posted by: deucesdown Posted at: 2017-10-27T14:59:36.640Z Reads: 236

```
It sounds like how cruise control would behave? Sorry for your loss :frowning:
```

---
## \#73 Posted by: Mikenopolis Posted at: 2017-10-27T15:16:36.684Z Reads: 236

```
Slightly off topic. I was watching the news this morning. There's another fire in California. It was started by a motorcycle that crash and let up dry brush and now it's a huge fire.

Maybe we should all carry a backpack with a small fire extinguisher when riding....or just for those long rides. 🤔 I would hate if my hard work bursted into flames or inconvenient others with said fire
```

---
## \#74 Posted by: quietbun Posted at: 2017-10-27T15:34:27.958Z Reads: 224

```
I never have cruise control setup. And if it's there, using brake should slow it down.
```

---
## \#75 Posted by: Michael319 Posted at: 2017-10-27T16:08:50.112Z Reads: 221

```
This goes against my own common sense, but still...

One of the main reasons I got into the DIY world of Esk8 is that I won't have to follow any rules. (Not really talking about laws) I don't have to obey manufacturer guidelines to still qualify for a warranty. I'm my own warranty. And I guarantee even if there was some rules in place, it wouldn't prevent things like this happening at all. Anytime there is a freak accident, it's hard to put blame on a single entity.
```

---
## \#76 Posted by: Alphamail Posted at: 2017-10-27T17:57:53.985Z Reads: 217

```
Yikes, that could have been much worse than it was.   Has anyone come up with a bail disconnect like jet skis and ATV's have.  Be it a cord, load sensor or proximity sensor, it may be a good idea to have a kill switch to disconnect the battery when the rider is not present on the board
```

---
## \#77 Posted by: zepton Posted at: 2017-10-27T18:42:12.620Z Reads: 217

```
C'mon man. Have some respect.
```

---
## \#78 Posted by: Michael319 Posted at: 2017-10-27T20:41:48.639Z Reads: 217

```
It's not like he died, I don't think there was any disrespect
```

---
## \#79 Posted by: pixelsilva Posted at: 2017-10-27T23:22:58.419Z Reads: 221

```
I will stay away from Market St. Is an esk8 catastrophe in the making.
```

---
## \#80 Posted by: Jinra Posted at: 2017-10-27T23:29:01.300Z Reads: 222

```
Our ride tomorrow is essentially all Market St :joy:
```

---
## \#81 Posted by: pixelsilva Posted at: 2017-10-27T23:31:58.511Z Reads: 221

```
You saw that poor guy eating the rails last week?
```

---
## \#82 Posted by: Jinra Posted at: 2017-10-27T23:32:36.533Z Reads: 206

```
no haven't heard of that
```

---
## \#83 Posted by: pixelsilva Posted at: 2017-10-27T23:34:27.712Z Reads: 216

```
Yeah, one of the guys posted the video on the FB page. It was last week.
```

---
## \#84 Posted by: pixelsilva Posted at: 2017-10-27T23:35:21.770Z Reads: 224

```
Nothing has changed in 111 years....

[https://youtu.be/8Q5Nur642BU](https://youtu.be/8Q5Nur642BU)

City of lunatics...and now I'm one of them!!
```

---
## \#85 Posted by: Fiori Posted at: 2017-10-28T01:49:14.596Z Reads: 231

```
It's funny that you mention that. I searched out this for that exact reason. I keep it in my backpack just in case something happens. It's also easy to clean up(or, so they say). 

I figure if I have this at least I can stop it from spreading(and save my board most importantly :stuck_out_tongue:) 

https://www.amazon.com/gp/product/B001229JCU/
```

---
## \#86 Posted by: willpark16 Posted at: 2017-10-28T02:55:21.401Z Reads: 231

```
I think we should all start carrying this or some baking soda
```

---
## \#87 Posted by: pennyboard Posted at: 2017-10-28T06:53:46.383Z Reads: 228

```
I still haven't had my court date, it's next month.  I'm hoping that since I was following the law as it's written, the ticket will be dismissed.
```

---
## \#88 Posted by: bartroosen12 Posted at: 2017-10-28T12:00:50.639Z Reads: 233

```
Damn son... that's a sick but sad story. Glad to know you're okay!
```

---
## \#89 Posted by: Jedi Posted at: 2018-03-21T17:38:26.219Z Reads: 207

```
Saw this on IG today, gotta be yours right? 

![IMG_4199|281x500](upload://tgHN33OWxLIBulXNkDbNmR20lTb.PNG)
```

---
## \#90 Posted by: quietbun Posted at: 2018-03-21T21:00:32.949Z Reads: 193

```
Yes it was my eboard. I'm surprised how young people feel good when an accident happened; taking picture, posting, commenting and bashing, but no helping. It's fine that they are not sorry for my board; but I am sorry for their emotionless life.
```

---
## \#91 Posted by: Jedi Posted at: 2018-03-21T22:21:48.427Z Reads: 185

```
That account seems to have a hatred for eboards.
```

---
## \#92 Posted by: Mikenopolis Posted at: 2018-03-21T23:00:34.168Z Reads: 188

```
did you read the comment on that post or any other? There was one that said "ride a moped like a normal person!

 I guess, no, we cannot all just get along
```

---
## \#93 Posted by: ron Posted at: 2018-03-21T23:32:49.710Z Reads: 186

```
Two theories that come into my mind:

-Interferience through WiFi/BT or other 2,4GHz Wireless Radio. It says it is doing Channel Hopping between 126 channels, but it can be that it is poorly implemented, regardless of what they are writing about the specs.

-Maybe it could also be due to a brownout after accellerating at the traffic light.

I thought a little bit about it and got an idea:

Why not copy the principle of the Security-Key/Kill Switch which are used on JetSkies, boats, etc.

You could tie it around your ankle, and if you fall from the board than it gets disconnected and the power gets cut physically and the board has no chance to accelerate anymore.

Just need to find a suitable connector. XT-90 is not ! Maybe this could be integrated into the Anti-Spark switches?! Maybe we could even use those kill switches from a Jet-Ski!?
```

---
## \#94 Posted by: webst Posted at: 2018-03-22T03:18:11.416Z Reads: 180

```
Wouldn’t switching off the remote help?
```

---
## \#95 Posted by: hyperIon1 Posted at: 2018-03-22T04:06:53.395Z Reads: 181

```
So glad you bailed. I have the same remote and used it on one of my prototypes. Needless to say it’s sitting in a box. Even when I configured the failsafe it cut out, luckily it’s all been controlled area testing. I have a nano-x on it now. Not much better. I’m waiting on one of these. 
Photon remotes from www.eboardshop.net
```

---
## \#96 Posted by: Mikenopolis Posted at: 2018-03-22T04:22:59.020Z Reads: 177

```
Not if the remote wasn’t setup with the fail safe. Always test when building. If not done correctly, turning off the remote would make the board go full speed
```

---
## \#97 Posted by: Mikenopolis Posted at: 2018-03-22T04:24:27.492Z Reads: 177

```
GT2B with modded housing is my favorite. Then the Mini. I can’t wait to use the Photon as well
```

---
## \#98 Posted by: webst Posted at: 2018-03-22T06:45:07.771Z Reads: 174

```
I always thought those are the basics you set in vesc. No remote - slow braking. I’m preparing to get first board since 2016 though so I’m not talking from hands on experience. Just the thing I remember not to forget while finally setting the whole thing up soon.
```

---
## \#99 Posted by: sk8l8r Posted at: 2018-03-22T10:59:51.147Z Reads: 165

```
[quote="quietbun, post:90, topic:36612"]
they are not sorry for my board
[/quote]

I felt REALLY sorry for that poor board! was there even a bearing that survived?
```

---
## \#100 Posted by: mmaner Posted at: 2018-03-22T15:07:50.315Z Reads: 164

```
[quote="Mikenopolis, post:92, topic:36612, full:true"]
did you read the comment on that post or any other? There was one that said "ride a moped like a normal person!

I guess, no, we cannot all just get along
[/quote]

I had a guy throw a 2x4 in front of me once.  I was able to run it off, which put me right in front of him.  So being a tempermental old asshole, I clocked him in the jaw and he hit the ground.  I turned around to look for my board and cop is standing 5 feet away.  

He looked at me, grinned, said "I didn't see damned thing".  I left...quickly :slight_smile:

The moral of the story.

There are asshats a plenty, but there's also cool people around when you need them.
```

---
## \#101 Posted by: Mobutusan Posted at: 2018-03-23T04:31:07.545Z Reads: 147

```
That's so great! That's when you really need a GoPro for those unscripted moments. I remember seeing a video from a member here where some douchebag did that, and I wished he had beat the guy into the ground for it. Good on ya. :facepunch:
```

---
## \#102 Posted by: pixelsilva Posted at: 2018-03-23T05:22:24.873Z Reads: 146

```
> @Jedi 
> 
> ![image|281x500](upload://gUNdcYxXK0VflYpFNez83tjwtLr.jpg)

@quietbun, this was at Market St.?
```

---
## \#103 Posted by: stimm Posted at: 2018-03-24T11:46:47.484Z Reads: 139

```
Try riding a normal skateboard on those streets.  I grew up skating and it is funny when people complain about 83mm wheels being too small when I rock 53mm wheels with a 100a hardness on those same streets.   You will also have more of a problem when you have a board with no tail.  If you have a tail you can pop your nose over the pebbles and such which lets you avoid the big stuff.  When you skate you learn to pop the nose and float your back foot so you can float over the rocks, it is a skill that takes time to master.
```

---
## \#104 Posted by: stimm Posted at: 2018-03-24T11:49:24.991Z Reads: 141

```
A weight sensor might be a better solution.
```

---
## \#105 Posted by: getyorma Posted at: 2018-03-24T13:29:34.695Z Reads: 141

```
Damn dude. I am starting to concider mechanical brakes that mbs sells with their boards :D :D If anything goes wrong - i can wiggle my foot - disconnecting the loop key and pulling on the mbs brake. :D The best and the most reliable controller (again imo) is GT2B or similar. Never failed on me and i never had signal problems. I even modded one into a custom 3D controller and it works wonders.
```

---
