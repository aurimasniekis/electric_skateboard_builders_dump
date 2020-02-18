# RevWatch - Feedback

### Replies: 34 Views: 968

## \#1 Posted by: binitshah Posted at: 2018-07-03T07:32:05.482Z Reads: 184

```
Hi guys. I'm Binit and I'm new to the forums and EV longboards; however, I'm not new to electronics and longboarding in general. I found this forum a month ago and reading it has become an obsession. Seeing your boards and the cool innovations ([Fliess is insane!](https://www.electric-skateboard.builders/t/fliess-bulletproof-directdrive/47379)) convinced me to get started on my own. I just finished making a deck (using the sandwiched plywood technique) and I'm about to paint it. I can post pictures if anyone is interested. Some background: I'm a computer science student who's currently interning and has way too much time on his hands and also has an affinity for electronics and design. Okay, enough intro.

I'm here to get some feedback on an idea I had for a wrist watch based remote. I'm called the project 'RevWatch' because the motion to accelerate is like revving a motorcycle (except the wrong way... you'll see what I mean). The basic concept is a spring rewinding clip, [example](https://www.amazon.com/Key-Bak-MINI-BAK-Heavy-Retractable-24-Inch/dp/B01N5D8RG2/ref=pd_day0_hl_200_1?_encoding=UTF8&pd_rd_i=B01N5D8RG2&pd_rd_r=1bdfef34-7e89-11e8-afe6-9ba6b10680d3&pd_rd_w=35sef&pd_rd_wg=Kzw0h&pf_rd_i=desktop-dp-sims&pf_rd_m=ATVPDKIKX0DER&pf_rd_p=4014010564823900592&pf_rd_r=NPNVYGVBE4HYXRQPS6YB&pf_rd_s=desktop-dp-sims&pf_rd_t=40701&refRID=NPNVYGVBE4HYXRQPS6YB), acts as a rotary encoder that is tracked by a microcontroller and converted into an acceleration value that is sent over bluetooth to the HM-10 or whatever bluetooth module is connected to your VESC.

That's a bit tough to visualize, so here are some renders I whipped up in Blender.
![render1|690x388](upload://esScwaZFgLh2rV8mJHLHDDMaW4W.jpg)
![render2|690x388](upload://aiCPSXstbFFKRZCmOGVrA59bUjF.png)

Here's where I got the inspiration from. Imagine the mechanism is inside my watch.
![IMG_2430|281x500](upload://vmXGyuRpHaFCFsAxwsEAcsllQVZ.JPG)

I've gone through a couple of revisions of design so far with varying levels of artistic capability.
![IMG_2432|666x500](upload://xGlJuOt81UtZ61FTKvYF19duCWK.JPG)

And I've gotten to the point where I'd like to get some feedback from you guys. But first, some details.

**WHY**
Because I don't want to be seen riding around with one of these
![remote|200x200](upload://wm3RkuhdLTdeyf42jWStVCVXlSY.jpg)
(not trying to throw shade or anything) and while those [DIY remotes](https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543) I've seen are definitely slick, I'd like to try something new.

**GOALS**
The goal is to create a watch that can serve as a daily driver watch (meaning it has to have basic features: time/date/alarms/timer/stopwatch and some nice to have features thanks to bluetooth: notifications/calendar events). Daily driver means the watch needs to be reasonable in size (goal is 14mm height by 40mm diameter). However, this watch must also be capable of controlling a EV board through the mechanism I've described above and it must do it well. 

**FEATURES**
* Acceleration and braking controlled by watch's crown on a retractable reel. 
* Self-rewinding reel acts as a Dead man's switch that stops the board when crown slips out of fingers
* OLED screen for riding information (speed, battery voltage of board and watch, distance traveled, board's current draw and mah remaining)
* Time/date/alarms/timer/stopwatch/notifications/calendar events
* 190 mah lipo should give 3 hrs life (pessimistic estimate) of riding use (tx continuously active)
* 3 programmable switches that are also used for watch's menu navigation
* Companion mobile app for settings/tuning (probably react native).
* Right/Left hand symmetry (must flip UI in firmware)
* Battery protection (over-discharge/current limiter/etc) and Charging via USB Micro B or Mini (status LEDs)

Alright, so what are your thoughts? Would you use something like this? What glaringly obvious thing have I missed? Is the battery life too short and you'd settle for a larger watch? Or would you carry an battery pack and want an even thinner slicker watch? What features need to be included? Would you buy something like this? Would you want an radio version instead of bluetooth?

Thanks for reading and I hope you think it's an interesting concept.
```

---
## \#2 Posted by: ElskerShadow Posted at: 2018-07-03T07:42:06.510Z Reads: 160

```
[quote="binitshah, post:1, topic:60777"]
I can post pictures if anyone is interested.
[/quote]

Glad to have you here, but be aware that on this forum the more photos there is the happier people's are!

Very nice project I will look forward to this
```

---
## \#3 Posted by: ElskerShadow Posted at: 2018-07-03T07:45:00.840Z Reads: 159

```
In the general experience never use Bluetooth to control an Eboard. It's not reliable enough. Use 2,4 ghz.
```

---
## \#4 Posted by: binitshah Posted at: 2018-07-03T07:56:39.340Z Reads: 155

```
Thanks! I appreciate the tip, I'll post them in a new topic soon.
```

---
## \#5 Posted by: b264 Posted at: 2018-07-03T07:59:11.855Z Reads: 151

```
Reliability is #1, #2, and #3.  How awesome it is is #4 and how expensive it is is #5.  Keep that in mind ;-)

Streetface is not a nice thing.  At least if I street my face, I want it to be because I made an error riding... and not because of a mechanical or electrical failure that was beyond my control or because I tried to be cheap...
```

---
## \#6 Posted by: binitshah Posted at: 2018-07-03T08:02:07.722Z Reads: 146

```
I've seen this said on other threads too and I was wondering why Bluetooth is unreliable. How do other boards like Boosted get away with Bluetooth? Anyways, 2.4 ghz makes sense as the alternative. Is there a protocol (PPM/IBUS/DSM) that is preferred by riders here?
```

---
## \#7 Posted by: b264 Posted at: 2018-07-03T08:03:37.127Z Reads: 136

```
[quote="binitshah, post:6, topic:60777"]
Is there a protocol (PPM/IBUS/DSM) that is preferred by riders here?
[/quote]

PPM&nbsp;&nbsp;
```

---
## \#8 Posted by: binitshah Posted at: 2018-07-03T08:05:33.790Z Reads: 133

```
That's fair. Thanks for the priority check. I will definitely have to iterate on my design until reliability has proven itself.
```

---
## \#9 Posted by: b264 Posted at: 2018-07-03T08:05:42.844Z Reads: 135

```
[quote="binitshah, post:6, topic:60777"]
How do other boards like Boosted get away with Bluetooth?
[/quote]

Evolve uses Bluetooth for META remote communication, like what mode it's in, how much charge is left in the battery, et cetera.  The actual throttle/brake is 2.4GHz
```

---
## \#10 Posted by: binitshah Posted at: 2018-07-03T08:09:41.010Z Reads: 130

```
Ah okay, that makes a lot more sense. Since my bluetooth module is also my microcontroller, I'll look into getting a 2.4 GHz radio chip into the schematic. It'll definitely be necessary, although it will complicate things on the battery front a bit probably.
```

---
## \#11 Posted by: bevilacqua Posted at: 2018-07-03T08:09:57.624Z Reads: 124

```
Mellow uses Bluetooth, but they had issues on their first boards, specially on carbon decks. 

If you figure out how to use BT 5.0 it might be doable.
```

---
## \#12 Posted by: b264 Posted at: 2018-07-03T08:10:28.095Z Reads: 123

```
Never forget that nothing is wrong with a wired connection ;-)

Not suggesting to make it wired -- just saying don't overlook the option.

Cord/connector fray could be a bigger liability than the wireless system though in the long-run
```

---
## \#13 Posted by: binitshah Posted at: 2018-07-03T08:11:08.092Z Reads: 120

```
Haha you must be joking
```

---
## \#14 Posted by: b264 Posted at: 2018-07-03T08:12:01.132Z Reads: 117

```
Not joking
```

---
## \#15 Posted by: binitshah Posted at: 2018-07-03T08:14:31.106Z Reads: 116

```
Interesting. I'll look into this and see if it can act as a replacement for radio. It'd be nice to use the same chip to communicate with phones and the board.
```

---
## \#16 Posted by: High-roller Posted at: 2018-07-03T08:18:21.253Z Reads: 117

```
Well, this is certainly a new take on remotes....
So I think I get how the acceleration will work- pull/clench fist to go faster- but what about braking? All the remotes I know of use a bi-directional spring-loaded switch of some kind to work both the throttle and the brake. How do you plan to deal with this?
My other big concern is what happens to the remote in the event of a fall? Current remotes might get dropped or "thrown clear" even if they're on a lanyard, thus possibly preventing irripairable damage. Yours might be in danger of getting dragged along, thus getting pretty scratched up pretty quickly. 
How robust is the case going to be?
```

---
## \#17 Posted by: fliess Posted at: 2018-07-03T08:30:44.522Z Reads: 117

```
@binitshah, definitely interesting idea!

I was thinking about middle throttle position issue, but it seems not an issue at all - once watch and crown are installed, you just press a button to initialize middle position, which would be a current position of your hand. So you can initialize it differently depending on how you're going to ride, e.g. for sliding session braking is not needed and middle position is when the palm is straight :heart_eyes:
```

---
## \#18 Posted by: binitshah Posted at: 2018-07-03T08:33:01.535Z Reads: 114

```
Thanks @High-roller. You're right about how the acceleration would work. The way I envisioned this working (and it's still early on, so I'm open to ideas) is that the amount of reel pulled out of the watch falls in zones (accelerating, cruising, and braking) that the user sets when they first get the watch.

If you pull the crown out between your fingers and hold your wrist in the resting position (as shown in the blender renders), you'd be cruising. If you pull/clench the fist closed, then you'd accelerate. If you flex the opposite way, such that amount of reel out gets shorter, then you begin braking. These zones would be user adjustable.

I tend to wear watches quite a bit (as you've might've guessed already) and I haven't ran into the issue of scratching a watch up when I've fallen off my longboard. Typically, my palms end up more scratched. However, it is a good idea to machine the casing out of a sturdy material. I haven't decided yet, so I'm more than open to ideas. I have access to a small mill, so I was partial to a wood casing... but I'd probably prototype with 3D printed parts.
```

---
## \#19 Posted by: binitshah Posted at: 2018-07-03T08:35:56.648Z Reads: 115

```
Thanks @fliess! I have to admit, I'm a bit star struck! Your guide to making direct drives is brilliant and I'm hoping to make my own soon!

Your point is a good one. I initially envisioned that the user would preset zones using their phone when they first setup the watch, however, the center cruise position could change from ride to ride. Setting the new center with a button press is great idea and one that I'll probably adopt.
```

---
## \#20 Posted by: High-roller Posted at: 2018-07-03T08:47:10.582Z Reads: 118

```
I just tried out the motion you're talking about, I think it would be more comfortable to rely only on motion of the fingers, rather than the wrists. 
Imagine holding a traditional remote and having to constantly swing your wrist back and forth, not unlike acceleration on a motorcycle (and in an urban area constant braking and acceleration should be a given). Personally, I'd think I'd get wrist fatigue very fast. sidenote to this- mightn't there be a greater risk of carpral tunnel over time?
```

---
## \#21 Posted by: binitshah Posted at: 2018-07-03T08:57:09.164Z Reads: 101

```
That's fair. Fingers could be easier to flex. Ultimately, between fingers or wrist motions (or both), the end goal is to pull more or less reel out of the watch because the watch measures the amount of reel pulled out or returned. I hope to keep the system versatile enough to accommodate user's preferences. However, this will be easier to test once I've made prototypes.
```

---
## \#22 Posted by: fliess Posted at: 2018-07-03T21:44:11.658Z Reads: 86

```
@binitshah, I could have just ignored your excitement about DD, if I changed my opinion with a time. But NO :smile: DD is just the best. The more I ride, the more I realise it again and again. It's a pity, that not everybody can build it as easy as scheiss-belt drive. But if you manage and do it properly, then you will definitely share my opinion.
```

---
## \#23 Posted by: banjaxxed Posted at: 2018-07-03T22:19:05.423Z Reads: 85

```
Very cool but I’d have a concern that the cord would be rock solid and not get stuck in the pulled out mode 

Rock solid

There are full android 6 watches for very little $60 which are borderline working with the metr app

If you took the backplate off a chosen model and had an extension including the radio and cord mechanism, rooted and hacked to edk8 specifics. it could be an incredible combo
```

---
## \#24 Posted by: binitshah Posted at: 2018-07-04T06:22:19.342Z Reads: 78

```
If they ride even half as nice as they look, I'll be very happy. I look forward to sharing my approach to making direct drives.
```

---
## \#25 Posted by: Maxid Posted at: 2018-07-04T06:46:49.586Z Reads: 77

```
Bluetooth is also 2,4Ghz! :thinking:
```

---
## \#26 Posted by: ElskerShadow Posted at: 2018-07-04T07:19:57.800Z Reads: 79

```
Yeah and wifi as well, and many many other communication protocols.
Bluetooth uses low energy and short range RF, up to 4.0 it was never stable enough for these application. 
We shall see and test Bluetooth 5.0 that looks very promising.
```

---
## \#27 Posted by: binitshah Posted at: 2018-07-04T20:22:53.959Z Reads: 70

```
Agreed, this is one example of the kind of issues that could plague the mechanical part of the design. I believe that this one specifically wouldn't be an issue with extensive testing and iteration. 

The idea of ripping a cheap android watch for parts is not a bad idea. Those off-brands are probably very modular. My issue is that space inside one of these watches would likely be limited and fitting the rewinding mechanism inside it would be tough ask. Plus those watches have parts and circuits that this application wouldn't need. Also the price for making one of these RevWatches would have a lump sum $60 included. Finally, I think it'd be cooler (and cheaper) to just design the watch myself from the ground up.
```

---
## \#28 Posted by: janpom Posted at: 2018-07-04T20:40:15.330Z Reads: 70

```
Making something similar that would integrate with protective gloves would be cool. Not everyone wears a watch, but everyone wears gloves. Right? :face_with_raised_eyebrow:
```

---
## \#29 Posted by: banjaxxed Posted at: 2018-07-04T23:12:43.337Z Reads: 72

```
Impressive if you have those skills! I was just refering to taking the backplate off and adding a module which would increase the height probably by almost another 10mm, making it very chunky & yeah the cost

Cool if you go forward on this. The $60 is off-putting From scratch allows you much more options, with Android you have a great platform to provide all the xtra value over the control itself -


* navigation(turn-by-turn) 
* telemetry
* calls
* social
* music


And all the rest
```

---
## \#30 Posted by: High-roller Posted at: 2018-07-05T09:26:29.000Z Reads: 71

```
I just came across these Android smart glasses:

https://pixkol.com/products/m100-smart-glasses?variant=13956318625850
I thought it might be a good to add telemetry to your remote and still keep everything compact, if you're willing to overlook the geekiness. Same goes for everyone else working on this stuff @ackmaniac @Wajdi @solidgeek ... I forget who else.
Maybe there's a way to adapt them to display on a full-face helmet visor?
```

---
## \#31 Posted by: Wajdi Posted at: 2018-07-05T09:37:07.435Z Reads: 69

```
I'm very interested in smart glasses, I'm working on some other projects involving Augmented Reality and I can say for sure AR glasses will be the future.
```

---
## \#32 Posted by: E1Allen Posted at: 2018-07-05T12:54:26.446Z Reads: 65

```
So, not to be negative on innovation but your design has some hurdles to overcome.  
Unlike a throttle, unless you don't want brakes you're going to need a neutral point on your string. And since it's a string it will have to be under tension.  So your hand will have to hold neutral at times you would like to coast or not power the board.  You will also limit your hand to a few specific movements while riding.  PPM is a very precise input, I think a wrist is just as capable as finger or thumb control but it would take some getting used to.

Quite a few of us also switch remote hands while riding you will lose this ability, at least a quick switch on the fly.
What happens in a crash?

I like the watch idea, it's small and compact.  The large RC car remotes work because their cheap and have good signal.

What if instead of a string it cord it was a wire attached to a small throttle potentiometer about the size of a small battery flashlight.
![image|220x153](upload://gMHY2uMNL2ScFjDx23shHxQnRAW.jpeg)

This could either attach to the band or under the watch face. This would slide forward or back instead of trigger style. Just a thought.

I like your idea, it just has some design hurdles to overcome.
```

---
## \#33 Posted by: binitshah Posted at: 2018-07-08T07:53:42.394Z Reads: 59

```
@banjaxxed Great point about Android wear. It'd allow for much more functionality, however, it's also a much more complicated project and I don't think I'm that experienced yet. For now, I think I will build my own simple OS that implements the core features outlined above.

@janpom Interesting idea. I know that flex resistor sensors have been used in gloves before (I think Nintendo made a glove called the power glove or something). Having gone down the route of glove projects before, I don't think I'm willing to touch this project for now. Furthermore, the allure of fitting this remote into a wrist watch is that it is hidden as an everyday object. Let me know if you start making this glove design. 

@E1Allen Thanks for the feedback. The ease of holding the reel at a resting position and the discomfort from limited wrist movement could be real problem. @High-roller had a similar point. The control mechanism needs to feel natural. Whether or not it will can only be told when I try it out. The PPM (output) of the watch can be adapted to account for jitters and dead zones in software. As for crash scenarios, I plan to address this buy having the reel act as a deadman's switch. How well this works out in practically, will once again, need to be tested. Potentiometer is a good idea and I was considering it as well, however, I don't see an easy way for the potentiometer+wire to retract easy.

**General Update:** I've spent some researching alternatives to bluetooth module I was going to use. Reliability is key and the bluetooth 4.2 module I was considering might not be good enough. 2.4Ghzs RF is proven while bluetooth 5.0 is unproven but has potential. Therefore, I've decided to make designs for both. I'd like to compare the BT 5.0 against radio and see if it can perform as well or better. For the radio's design, I am fortunate people on this forum using radio remotes have open sourced their designs and GreatScott! has made a video on the topic. I've decided on parts for both and am designing new schematics: one for BT 5.0 and one for radio. Soon after that, I'll start on designing PCBs. I'll continue to post updates on this thread until I've reach some major checkpoint.
```

---
## \#35 Posted by: Slak Posted at: 2018-07-16T12:21:54.346Z Reads: 44

```
There's a lot of work here, nice job !

But I just can't imagine not having full freedom to use my hands as I want when I'm riding. It will maybe work at the end and some people maybe gonna use it everyday but I have doubts about this being massively adopted by the community. When I ride, I (and I'm pretty sure a lot of people, if not most of the people) want to be able, at any moment, to :
 - Say hello or give the finger to anybody
 - Grab my phone in my pocket
 - Swap the hand holding the controller
 - Sit on my board
 - Grab something along the way
 - Etc.
Or just give the controller to a friend wanting to ride the board when I stop

All those moves seems really complicated to achieve in a simple way without overthinking about the way to do it safely and quickly with your system.

Hope I'm wrong ! And keep the good job going, time will tell :)
```

---
