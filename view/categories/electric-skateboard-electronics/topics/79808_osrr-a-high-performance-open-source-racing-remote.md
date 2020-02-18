# OSRR - A High Performance Open Source Racing Remote

### Replies: 209 Views: 4846

## \#1 Posted by: DerelictRobot Posted at: 2019-01-03T21:55:11.281Z Reads: 672

```
Alright, let's get this show on the road. I am currently working on a high-performance, top-tier racing spec remote control design that uses modular internal components that can easily be reconfigured into different shapes/styles/sizes. I feel the remote and control over your throttle is one of the most important aspects of riding, and while there are some great low cost open source options out there I'd like to do something a bit different. 

...I'm going to need a better name. 

I'll rip this band-aid off now to properly set expectations- These are going to be expensive as they will be hand-built and I'm not cutting corners on component choices. I'm certainly open to selling parts kits and looking at ways of reducing cost, but I designed this with quality & performance taking priority over any cost-savings. We're likely looking at a $200-250 retail price for a 'pre-assembled, ready-to-run' Remote & Receiver. Don't quote me on that. I promise nothing at this point. 

I will be releasing the entire project open source under a Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) license. The only caveat being is that I don't yet have permission from the OEM to release the source of the thumbwheel sensor I am using, however the design can accommodate different analog sensor inputs for the throttle. 

Generally speaking I tend to wait until I'm finished with a project before posting about it, but my intention here is to release this project to the community so I'd like to loop you guys in for feedback earlier in my design process. This is *very* early in my development cycle, I only started digging into this seriously over the last 2 weeks, though I am just about ready to send off for my first round of prototype PCBs once I finalize where the LCD placement will be. 

So with that said, here are the specs and proposed development road map. 

**Phase 1 - Remote Reference Design & Basic Receiver**

* **Throttle Sensor** - military-spec (literally from a DOD contracted flight controls manufacturer) high-precision hall-effect thumbwheel sensor, impact resistant, IP-67. Amazing hand-feel, customization options for different trigger/thumbsticks & spring resistance. I'll ping @SeanHacker & @Spiritrunner47  to chime in with feedback as they've held my prototype in hand. The biggest catch here is these things are pretty expensive @ $70-80 depending on configuration.
![IMG_20181202_183042|666x500](upload://x1XVgTGMG5VB4DfWhpxgrGRRkOu.jpeg) 


* **Modular Internal Electronics** - Currently my PCB design is roughly the shape/layout of an 18650 cell, with two analog inputs for the option of a 2nd throttle/thumbwheel if you're feeling saucy. Analog inputs from the hall effect throttle sensors are interfaced via a 12-bit ADC. I am actually using an 18650 cell for power currently, with an integrated li-ion charger/boost circuit, but I'd like to leave this somewhat flexible in the design. Buttons will probably be kept to a minimum by I would like basic mode switching and an optional, programmable Deadman/cruise control trigger button at well.
![PNG|504x500](upload://uyLLLi3VWexu1tzWTgfD5talz5C.jpeg) 


* **Radio Comms Link** - 802.15.4 Xbee3 Radio Modules. I've used the Xbee S2C & 3 in a variety of environments professionally, they're essentially built for high-interference industrial environments. All the bells & whistles you'd expect from a modern, higher end radio comms module. Currently for testing, I've simply created a 115k-250k baudrate transparent UART link from the VESC to the remote using a pair of modules. I must emphasize that this is still very early in testing, I am not set on using these if they don't hold up in real-world performance. The biggest concern with transporting any more complex data structure like this is latency, though based on early testing I'm seeing around 30-35ms round trip time @ 115200 baud, without optimizations. Again, as critical as the comms link is this will still need a lot more testing, I just have a lot of experience using these modules so they're an easy go-to to get up and running quickly. So far they are working really well, but it needs to be thoroughly tested before I'll give it a bulletproof stamp. 
(PS: If your feedback is that you heard 'Xbees suck' I ask that your experience with them extend beyond using older series modules with Zigbee firmware, default settings, on your highschool's FIRST team. They require application/environmental specific configuration to get functioning well, but they do function well when setup correctly).

* **0.9" Color LCD Display/Integrated ESP8266EX SoC/WiFi/SD Card** - Currently prototyping with a 4D Systems IOD-09 module. I intend on keeping the display clean, simple, graphical. Currently I have it displaying speed, board battery, remote battery, odo. Obviously additional info can be added on other screens, etc. Just not a huge priority right now until other bring-up is done. I'll expand on the WiFi/SD in Phase 2. 

https://www.youtube.com/watch?v=6n0_gTyiNMM


*
* **Receiver** - Currently the plan is for a very basic receiver module that just interfaces directly to UART, but keeps costs down to about $25 per receiver for multi-board support. I have the ability to add PPM/PWM, but it's lower on my list of priorities and may end up getting included in the Advanced Receiver project.

* **Remote Grip/Enclosure Design Styles** - 'Nano Style', 'Puck Style' & 'Trigger Style' are the three I chose to start with. The intent here is to allow for people to modify and/or design their own enclosures, but I wanted to make a few basic reference designs available to get people started or to offer to those that don't have modeling/printing abilities. These are intended to be solid-piece prints with access panels for the battery/LCD on the rear and a robust charging port (how many of you have broken a microUSB port off?). Here are a few first-pass sketches as reference. Please note- I am aware I will need to shift the LCD around, these are nowhere near final and will require a good number of print iterations to get the sizing & handfeel correct. Purely for example, but I am printing up a shelled dummy of the red 'Nano Style' in Nylon 910 currently to get started. 

PS: I promise I actually made a consious effort to make them look less like Dongs. Late nights tho

![IMG_20190103_120627%20(1)|500x500](upload://t3JfPUfbIAGiW20AlrDiMjkSwd4.jpeg)  





**Phase 2 - Onboard telemetry logging to SD card/WiFi API for App sync**

This will be the second stage of development after basic functionally is rock solid on the remote. Concept here is that the board/remote should always be logging internally and shouldn't depend upon a Bluetooth tether to your phone. I already have the ESP2866 setup to host a webpage on demand for configuration/tuning, this will be extended as a web API that can be turned on as needed to _**'Sync' your remote to a logging app not dissimilar from how a FitBit style fitness tracker logs/syncs up.**_ I would like for the board & remote to be self contained and not require a phone to be on-hand and connected in order to log ride metrics. SD card onboard the esp board gives us plenty of space for logs. 

**Phase 3 - Advanced Receiver**
This will not replace the basic receiver, rather be an advanced option further down the line. Features will include dual PPM/PWM outputs to give additional throttle output options to the ESC or for compatibility with non-VESC based ESC. UART will still be required for full telemetry obviously. Also want to add a bank of 12v mosfets to control lights, horn, etc. **Open to suggestions on additional features you guys would like to see here.** 

WIP - I'll update with more in a bit, gonna go skate!
```

---
## \#2 Posted by: brenternet Posted at: 2019-01-03T21:55:27.601Z Reads: 583

```
First, I'll take 3 of each
```

---
## \#3 Posted by: J0ker3366 Posted at: 2019-01-03T21:56:54.226Z Reads: 580

```
&lrm; Winning
```

---
## \#4 Posted by: brenternet Posted at: 2019-01-03T21:56:59.418Z Reads: 567

```
[quote="DerelictRobot, post:1, topic:79808"]
PS: I promise I actually made a conscience effort to make them look less like Dongs. Late nights tho
[/quote]

On this note.... I have some names for you.

Top one, "Pocket vibrator"
Middle, "Beam me up Scotty"
Bottom, "Fucking Scarab"

These look amazing, love the shape of the trigger one specifically.
```

---
## \#5 Posted by: DerelictRobot Posted at: 2019-01-03T22:04:57.449Z Reads: 532

```
[quote="brenternet, post:4, topic:79808"]
Top one, “Pocket vibrator”
[/quote]

"Her Majesty's Pleasure"
```

---
## \#6 Posted by: Skunk Posted at: 2019-01-03T22:05:08.523Z Reads: 506

```
Yaaaas
About time :wink:
```

---
## \#7 Posted by: SeanHacker Posted at: 2019-01-03T22:05:58.028Z Reads: 498

```
Fuck yes!!!

Just the throttle alone is awesome! There isn't anything on the market that feels as responsive, smooth, and totally controllable. It's amazing!
```

---
## \#8 Posted by: evoheyax Posted at: 2019-01-03T22:38:41.360Z Reads: 485

```
Good stuff! I'd love to try one. Don't cheap out! I love high quality!
```

---
## \#9 Posted by: okp Posted at: 2019-01-03T23:00:44.185Z Reads: 466

```
well, that's gonna be perfect with my ongoing HAYA build. Congrats man.
```

---
## \#10 Posted by: SeanHacker Posted at: 2019-01-03T23:01:56.368Z Reads: 461

```
[quote="DerelictRobot, post:1, topic:79808"]
PS: I promise I actually made a conscience effort to make them look less like Dongs. Late nights tho
[/quote]

Might be a selling point though dude... ;)
```

---
## \#11 Posted by: Skunk Posted at: 2019-01-03T23:02:57.589Z Reads: 430

```
Guarantees no matter what you're wearing, you'll always have a natural pocket to fit them in
```

---
## \#12 Posted by: Mich21050 Posted at: 2019-01-03T23:03:53.330Z Reads: 427

```
Does the remote have a vibrating function? :joy:
@DerelictRobot
```

---
## \#13 Posted by: evoheyax Posted at: 2019-01-03T23:04:46.724Z Reads: 423

```
How do I get my hands on one before the Barret Junction Race in 2 and a half weeks?

Than you can say race tested!
```

---
## \#14 Posted by: SeanHacker Posted at: 2019-01-03T23:04:48.629Z Reads: 403

```
Million bucks says he can add one. :slight_smile:
```

---
## \#15 Posted by: Balth81 Posted at: 2019-01-03T23:04:52.338Z Reads: 415

```
Definitely keen, I would love it if you were able to make it customisable in the sense of top speed in modes so if I wanted low to be 30km/h then I could set and fast be like max of board etc ..
```

---
## \#16 Posted by: Skunk Posted at: 2019-01-03T23:06:00.773Z Reads: 413

```
No but really guys. @DerelictRobot came down to visit a few weeks back and I got to feel what the throttle feels like on these remotes.
Its steps above any thing ive used.
```

---
## \#17 Posted by: SeanHacker Posted at: 2019-01-03T23:06:40.420Z Reads: 425

```
From my understanding is that it can do just about anything VESC settings related. It's run through UART and not PPM. @DerelictRobot can explain better though.
```

---
## \#18 Posted by: Skunk Posted at: 2019-01-03T23:06:46.605Z Reads: 429

```
Lol. Just meet him there
```

---
## \#19 Posted by: evoheyax Posted at: 2019-01-03T23:09:50.843Z Reads: 432

```
Oh, I'll be there!
```

---
## \#20 Posted by: Grozniy Posted at: 2019-01-03T23:15:01.007Z Reads: 430

```
Make it also a sliding puck ;)
```

---
## \#21 Posted by: mmaner Posted at: 2019-01-03T23:19:40.637Z Reads: 390

```
The puck is my favourite, elegant. Excellent work, I'm looking forward to testing these.
```

---
## \#22 Posted by: DerelictRobot Posted at: 2019-01-04T00:10:52.955Z Reads: 408

```
[quote="Mich21050, post:12, topic:79808"]
Does the remote have a vibrating function? :joy:
[/quote]

I plead the fifth. 

[quote="SeanHacker, post:17, topic:79808"]
From my understanding is that it can do just about anything VESC settings related. It’s run through UART and not PPM.
[/quote]

That's correct. There's just work that has to be done to ensure comms are optimized and that latency is not an  issue. 

The design intent is to keep the rider interface minimal and natural. 2 buttons- one for ride-time functions like deadman or cruise control, and another for simple mode switching between motor profiles. 

Ideally the remote should provide enough interface that you should never have to pull out your phone mid-ride. The way I see this working is- your phone should only be an interface for advanced options/settings & log viewing, I'd like the remote to always be logging and to be functionally self-contained during the ride, and then be able to sync up to a phone app via WiFi at set intervals, not dissimilar from how a FitBit syncs data with your phone. This is all future roadmap stuff so I try not to talk too much about features that I've not yet broken ground on, but that is the end goal.
```

---
## \#23 Posted by: DerelictRobot Posted at: 2019-01-04T04:06:59.169Z Reads: 393

```
[quote="evoheyax, post:13, topic:79808, full:true"]
How do I get my hands on one before the Barret Junction Race in 2 and a half weeks?

Than you can say race tested!
[/quote]

I really doubt I can get more than a single prototype done before Barrett, but I intended on bringing that one with me for demo. There is lead time on the PCBs and the thumbwheels are actually handmade to order- I have all the other components to build out a small batch of these remotes for beta testing, but I'm waiting to hear back on the leadtime for more thumbwheels. I'm shooting to have that first batch of prototypes done in Feb though. 

As of today I've got all the dev tools & parts to finish out my first useable prototype though. :slight_smile: 
![IMG_20190103_185828|666x500](upload://1H1aIwsqwVQTgkkn8fsHrHE9M9T.jpeg)
```

---
## \#24 Posted by: Spiritrunner47 Posted at: 2019-01-04T04:11:43.038Z Reads: 376

```
@DerelictRobot see you at the shop tomorrow. Always a pleasure watching you manifest ideas to reality.
```

---
## \#25 Posted by: evoheyax Posted at: 2019-01-04T05:25:03.167Z Reads: 355

```
Well can’t wait to see it at the race! Very exciting!
```

---
## \#26 Posted by: Sender Posted at: 2019-01-04T05:27:57.742Z Reads: 366

```
[quote="DerelictRobot, post:23, topic:79808"]
a small batch of these remotes for beta testing,
[/quote]

😍😍😍😍

&nbsp;
```

---
## \#27 Posted by: Goonman Posted at: 2019-01-04T05:49:06.960Z Reads: 354

```
Priority number 1 for me would be reliability. I dont want to have to update shit just so I can go for a ride. I just want some basic data. Volts amp speed etc. Puckerrup is the best looking.
```

---
## \#28 Posted by: venom121212 Posted at: 2019-01-04T12:51:33.431Z Reads: 341

```
The puck one reminds me of the digivice from that one show that definitely wasn't pokemon...
```

---
## \#29 Posted by: Linny Posted at: 2019-01-04T12:56:42.892Z Reads: 334

```
Digimon.....? 

It looks like a grenade in the render
```

---
## \#30 Posted by: Gerrycorrado Posted at: 2019-01-04T13:11:02.822Z Reads: 333

```
Please put me on the inquiry list! Thx
```

---
## \#31 Posted by: b264 Posted at: 2019-01-04T13:33:05.915Z Reads: 348

```
[quote="DerelictRobot, post:1, topic:79808"]
I promise I actually made a consious effort to make them look less like Dongs
[/quote]

LoLz :rofl:

Just as long as they don't resemble a gun at all so we don't get shot by cops.  The main thing here is not to be firearm-colored.

Have you thought about multiple channels -- example a "wheel" like the mini remote has?  Or another control to allow horn honking, quietly and loudly

What about pairing multiple receivers to one transmitter?  Have you considered that?

As far as breaking micro USB I agree it's a huge problem, but one way I've discovered is that if a remote that draw almost no power has a big 3500mAh cell in it then you might have to charge it twice a year which means it takes a lot longer for the shitty microUSB to break ;-)  But if it's not microUSB I hope it's USB-C :blush:
```

---
## \#32 Posted by: venom121212 Posted at: 2019-01-04T13:42:34.461Z Reads: 321

```
[quote="b264, post:31, topic:79808"]
The main thing here is not to be black.
[/quote]

Hey now...
```

---
## \#33 Posted by: Sn4pz Posted at: 2019-01-04T17:39:04.823Z Reads: 314

```
I told myself I wouldnt spend more on remotes.... but Im game for the 3rd option as soon as theyre ready :tired_face::roll_eyes::joy:
```

---
## \#34 Posted by: DerelictRobot Posted at: 2019-01-04T22:31:13.714Z Reads: 333

```
[quote="b264, post:31, topic:79808"]
Have you thought about multiple channels – example a “wheel” like the mini remote has? Or another control to allow horn honking, quietly and loudly
[/quote]

I've got a 4-channel 12-bit ADC spec'd in. My thought now was 2 for analog thumbwheels/triggers and 2 for buttons. Future plans to make them easily reconfigured through the web API/app. 

[quote="b264, post:31, topic:79808"]
What about pairing multiple receivers to one transmitter? Have you considered that?
[/quote]

Totally. It's one of the reasons why I went with a basic receiver option initially with the intent to have multi board support and offer the receivers for $25ish, with individual riding profiles & telemetry logging. The Xbee radios can pretty easily be reconfigured for a number of different network configurations, they even support mesh networking on different firmware. Multi board support is super simple in this regard, it'll just be some work to make it painless. 

[quote="b264, post:31, topic:79808"]
But if it’s not microUSB I hope it’s USB-C :blush:
[/quote]

So this is something I'm still chewing through, because if I do add usb externally it would need to handle charging in addition to firmware updates. Right now it's easier/faster for me to keep the FTDI off device and use a more robust charging port. I would just prefer to take the time to do USB right if I'm going through the trouble of sourcing a USB C connector and host IC.
```

---
## \#35 Posted by: Zaphod Posted at: 2019-01-04T22:31:20.057Z Reads: 299

```
Coming from a downhill background I really like the bailing ability I get from slide gloves. My current issue is that I can only wear a puck on my non-remote hand when riding electric. Do you have any plans to make your hardware impact resistant enough that a puck could be attached and the unit could take the force of a slide? Is this even a common concern? Cheers and excellent work!
```

---
## \#36 Posted by: brenternet Posted at: 2019-01-04T22:39:10.348Z Reads: 306

```
[quote="Zaphod, post:35, topic:79808"]
Is this even a common concern?
[/quote]

People have definitely brought it up before, so you're not alone.
```

---
## \#37 Posted by: Skunk Posted at: 2019-01-04T22:41:16.066Z Reads: 317

```
I think a remote that strapped around the palm of your hand kind of like a watch but between your pointer finger and thumb.
You can have this display, battery & the majority of the iternals on the back of your hand.
Then have it have a fish hook type of shape for the thumbwheel to still be easily accessed by the thumb.
Then you could just use your normal slide pucks rather than making the remote strong enough to slide on
```

---
## \#38 Posted by: banjaxxed Posted at: 2019-01-04T23:32:55.291Z Reads: 305

```
This is nice I want them all you have my cheddar when they are go
```

---
## \#39 Posted by: DerelictRobot Posted at: 2019-01-04T23:37:06.715Z Reads: 349

```
[quote="Zaphod, post:35, topic:79808"]
Do you have any plans to make your hardware impact resistant enough that a puck could be attached and the unit could take the force of a slide? Is this even a common concern?
[/quote]

You're probably the 10th person to bring this exact point up. I think it's worth looking into if there's enough demand for such a thing. Initially my thoughts are that I'm not sure where the LCD would be effectively placed, obviously it couldn't be in the palm. There's also vibration/impact consideration (would probably need the pot the internals and use a solid billet aluminum metal enclosure) along with the need for a serviceable/replaceable slide disc. Esp8266s are cheap and easy, perhaps a super ruggedized version without an LCD could happen. I need to get past phase 1 before I commit to any further scope creep. But with that said...

[quote="Skunk, post:37, topic:79808"]
I think a remote that strapped around the palm of your hand kind of like a watch but between your pointer finger and thumb.
You can have this display, battery &amp; the majority of the iternals on the back of your hand.
Then have it have a fish hook type of shape for the thumbwheel to still be easily accessed by the thumb.
Then you could just use your normal slide pucks rather than making the remote strong enough to slide on
[/quote]

I love this kind of thinking when it comes to HCI. This was one of the primary design philosophies behind trying to keep the internal PCB, thumbwheel, and buttons modular. I'd like us to be able to break the mold on how we interact with these devices. I worked on a research project a few years back where I built out a wearable telemetry harness that you wore like a backpack and strapped your arms into. Wirelessly linked to a humanoid robot and you could teleoperate the upper torso and arms just by moving your own; the robot would mirror your motion (meaningful interaction with the environment is another story and well, grant funding ran out). I often find myself wishing I had more of my fingers free on my throttle hand, so definitely like the idea of being able to 'let go' of the remote.

Great input guys, appreciate the discussion.
```

---
## \#40 Posted by: Grozniy Posted at: 2019-01-04T23:38:24.021Z Reads: 323

```
[quote="DerelictRobot, post:39, topic:79808"]
perhaps a super ruggedized version without an LCD could happen.
[/quote]

Yes for this
```

---
## \#41 Posted by: b264 Posted at: 2019-01-04T23:40:54.165Z Reads: 303

```
[quote="DerelictRobot, post:34, topic:79808"]
So this is something I’m still chewing through, because if I do add usb externally it would need to handle charging in addition to firmware updates. Right now it’s easier/faster for me to keep the FTDI off device and use a more robust charging port. I would just prefer to take the time to do USB right if I’m going through the trouble of sourcing a USB C connector and host IC.
[/quote]

It's my personal opinion that folks would prefer a USB-C even if it only charged and didn't do firmware updates.  People have cell phones everywhere and USB-C charge cables are everywhere.  A proprietary or unusual charge port would suck.
```

---
## \#42 Posted by: Sn4pz Posted at: 2019-01-05T00:01:54.124Z Reads: 299

```
[quote="b264, post:41, topic:79808"]
USB-C charge cables are everywhere.
[/quote]

speak for yourself... lol

No matter where I go, if my note 8 is low on juice I can guarantee no one will carry a cable that can help me :rofl:
```

---
## \#43 Posted by: DerelictRobot Posted at: 2019-01-05T01:03:54.697Z Reads: 318

```
[quote="b264, post:41, topic:79808"]
It’s my personal opinion that folks would prefer a USB-C even if it only charged and didn’t do firmware updates. People have cell phones everywhere and USB-C charge cables are everywhere. A proprietary or unusual charge port would suck.
[/quote]

This is a super valid point. The charging port is something I've been thinking through and don't have a perfect solution for currently. At the moment I'm using a 5v1amp wallwart with a 2.1/5.5mm plug/jack. Powered from a 3000mAh 18650 battery, we should expect pretty long run time making the need to bring the charger with you less of an issue. But I think I'm leaning more towards USB-C. 

Itd probably be about $10 added to the BOM cost for a separate custom USB-C board that handles the lipo charging as well as uart connection for firmware. Won't happen on the first round prototypes but I could fit that in before the gen1 batch easily. Not much to it as it'll basically be two TI reference designs on PCB to mount the USB-C port.
```

---
## \#44 Posted by: Jacobee Posted at: 2019-01-05T01:43:58.539Z Reads: 305

```
If you guys want to be able to use a slide puck with your remote hand and have a thumb throttle you could use the thumb throttle model and do what @fliess did here
https://www.electric-skateboard.builders/t/fliess-3-einmal-directdrive-immer-directdrive/32279/145
```

---
## \#45 Posted by: JTAG Posted at: 2019-01-05T02:19:15.367Z Reads: 295

```
Your friends are just not mainstream enough😎...

Lookin good with the throttle sensor! I used a similar one for a different application and from experience with then ( not sure whether it is the same brand): make sure thay use a stainless spring and cover the magnet completely in epoxy ( or else they rust), also they have an option to digitally output the knob position and also allow a supply voltage of 3 or 3.3 V not exactly sure on what their minimum was.
```

---
## \#46 Posted by: Arch Posted at: 2019-01-08T03:20:00.510Z Reads: 272

```
great idea
```

---
## \#47 Posted by: Skunk Posted at: 2019-01-08T03:22:19.967Z Reads: 270

```
Thanks.  Im hoping it works out in real life as well as it does in my head.
```

---
## \#48 Posted by: Arch Posted at: 2019-01-08T03:25:32.321Z Reads: 275

```
get someone to draw what's in your head. I think I have a version of it in mine, but yours is surely more complete. being able to hit the ground and not have your remote impacted because the grunt of it is on the top of your hand and not in the palm of your hand is the type of idea that will have everyone saying "what the hell were they using before?" in 10 years. It will take m some iterations, like anything, but once nailed, i can see this really being the future. in the meantime, the 3 proposed designs effing rock. great work man
```

---
## \#49 Posted by: Skunk Posted at: 2019-01-08T03:25:44.595Z Reads: 266

```
 I'm sure if anybody can figure it out it's @DerelictRobot guys a nerd
```

---
## \#50 Posted by: DerelictRobot Posted at: 2019-01-08T03:26:39.428Z Reads: 271

```
:slight_smile: we will have to have some design sessions next time I'm down there
```

---
## \#51 Posted by: Skunk Posted at: 2019-01-08T03:28:35.151Z Reads: 264

```
Hell yeah. Im down
```

---
## \#52 Posted by: Arch Posted at: 2019-01-08T03:29:03.905Z Reads: 267

```
I'm sure you don't have to reinvent the wheel. What other industries have top of hand devices? deep sea diving (no idea, I hate diving, just spitballing here)? perhaps some design exists and only needs to be adapted
```

---
## \#53 Posted by: Skunk Posted at: 2019-01-08T03:32:26.092Z Reads: 267

```
Some inventory guns have a Top Hand straps for watching your numbers as you count product
```

---
## \#54 Posted by: DerelictRobot Posted at: 2019-01-08T03:34:23.656Z Reads: 290

```
I think the biggest challenge here will be getting the throttle mounted just right, and also keep it sturdy enough to not defeat the purpose of moving the rest of the internals out of harm's way. 

I've done some previous work in HCI, but I'm all for leveraging what's out there. I've got a long train ride back to Portland, looks like I'll have to do some reading and drawing. :slight_smile:

I think once the modular internals get dialed in we can really open up creativity with different designs and throttle styles. But it's way too important to be so fragile as it stands.
```

---
## \#55 Posted by: Skunk Posted at: 2019-01-08T03:51:43.050Z Reads: 314

```
This isn't sleek but it's a start and sums up the idea.  Its just attacking the Throttle that's gonna be work.
![ishoxs-hand-strap-remote-highly-flexible-adjustable-hand-arm-strap-for-gopro-wifi-remote-remote-control-with-anti-slip-inlet-also-suitable-for-wetsuit-a54|500x500](upload://ithMeL6frdTbWNgRA1I6ULUBi6b.jpeg) ![ishoxs-hand-strap-remote-highly-flexible-adjustable-hand-arm-strap-for-gopro-wifi-remote-remote-control-with-anti-slip-inlet-also-suitable-for-wetsuit-079|500x500](upload://mTAlw7fExrpIXcNvjz2DPQc7hz0.jpeg)

If it was detachable from the hand strap you could probably manage leaving it attached to your slide gloves.
Maybe the throttle doesn't have to be attached to the main part buy a solid piece?
Could just be a coiled wire that somehow clips to the straps on the palm.

Best example i could find
![jpg_640x640|500x500](upload://cM1pJGB8hwyx4yrstwutNwiieu9.jpeg)
```

---
## \#56 Posted by: DerelictRobot Posted at: 2019-01-08T04:26:09.463Z Reads: 300

```
[quote="Skunk, post:55, topic:79808"]
Best example i could find

[![jpg_640x640|392x392](https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/9/5987c939ad5eaf83e3c03e2490adb2e266901bd5.jpeg)](https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/9/5987c939ad5eaf83e3c03e2490adb2e266901bd5.jpeg)
[/quote]

Oh lawdy. :laughing:
```

---
## \#57 Posted by: Skunk Posted at: 2019-01-08T04:38:04.175Z Reads: 287

```
Yeah it's definitely a bad example it's really just the cord part i wanted to show lol
```

---
## \#58 Posted by: Itsmedant Posted at: 2019-01-08T15:15:25.805Z Reads: 287

```
This project is amazing @DerelictRobot

I'm definitely interested in picking one of these up. I'm sure you have loads of people testing already but if you need anymore, I'm down to pay for a kit when you get it worked out!
```

---
## \#59 Posted by: Chupacabra Posted at: 2019-01-08T15:34:43.937Z Reads: 283

```
Same. 10 char.
```

---
## \#60 Posted by: Zaphod Posted at: 2019-01-12T21:46:16.841Z Reads: 285

```
Thanks for linking that post!
```

---
## \#61 Posted by: DerelictRobot Posted at: 2019-01-13T08:26:06.112Z Reads: 267

```
First rev PCBs for remote & receiver ordered. Should hopefully be in by week after next.
```

---
## \#62 Posted by: hyperIon1 Posted at: 2019-02-04T03:32:10.524Z Reads: 258

```
excellent stuff @DerelictRobot, I can't wait to see the finished product.....
```

---
## \#63 Posted by: lrdesigns Posted at: 2019-02-04T06:43:41.970Z Reads: 256

```
Cool project! I would be happy to help with some 3D design work to make some sleeker and more ergonomic cases for these.
```

---
## \#64 Posted by: Skunk Posted at: 2019-02-04T06:45:15.362Z Reads: 254

```
But will they be phallic ?
```

---
## \#65 Posted by: Sender Posted at: 2019-02-04T06:47:58.154Z Reads: 250

```
To be fair, everything is a dildo if you are brave enough Kelly.

Be brave.
```

---
## \#66 Posted by: lrdesigns Posted at: 2019-02-04T09:47:34.949Z Reads: 240

```
Send duck pics I can use as reference.
```

---
## \#67 Posted by: banjaxxed Posted at: 2019-02-04T10:45:15.648Z Reads: 236

```
Very off but strangely on topic

Let Luke loose at the designs
```

---
## \#68 Posted by: Slak Posted at: 2019-02-04T11:16:04.264Z Reads: 228

```
Really nice work, @DerelictRobot !

But I don't really understand a thing, maybe it's obvious but I'm not a racer. What makes this remote better than a GT2B (already reliable, accurate and responsive) ? What potential problem does it fix ?
```

---
## \#69 Posted by: mmaner Posted at: 2019-02-04T14:01:00.118Z Reads: 225

```
telemetry, military spec trigger, much better shape...its all in the thread.  why be confrontational?
```

---
## \#70 Posted by: Slak Posted at: 2019-02-04T14:57:00.847Z Reads: 228

```
[quote="mmaner, post:69, topic:79808, full:true"]why be confrontational?[/quote]
I was not trolling at all, asking a real question and was trying not be confrontational... Nevermind...
```

---
## \#71 Posted by: DerelictRobot Posted at: 2019-02-04T18:06:51.270Z Reads: 231

```
[quote="lrdesigns, post:63, topic:79808, full:true"]
Cool project! I would be happy to help with some 3D design work to make some sleeker and more ergonomic cases for these.
[/quote]

I am hoping for exactly this. My current plan is just to get some basic functional designs published as a reference design, and the hope is that others can contribute, modify, polish. I've got EE design and firmware well handled for the time being, but iterative design on ergo enclosures is going to be a time sink and is just as important. So thank you, as this is an open source project it's my hope that it is useful enough that others want to continue to build upon it and improve.

Quick update; had a little snafu with the prototype PCBs and then ran into Chinese New Year delays, so a few things got shifted around. I'm still shooting for end of this month/early March for the first batch of beta units. 

My work project schedule got pushed back so I've got the next few weeks to really dig in. Hoping to have the first functional prototype to show in the near future.
```

---
## \#72 Posted by: PatRocks Posted at: 2019-02-04T19:07:27.518Z Reads: 217

```
[quote="PatRocks, post:257, topic:26461"]
anything’s a dildo if you’re brave enough (my favorite thing to say).
[/quote]

I said it first lol
```

---
## \#73 Posted by: DerelictRobot Posted at: 2019-02-04T19:14:07.307Z Reads: 208

```
[quote="PatRocks, post:72, topic:79808"]
I said it first lol
[/quote]

Excuse me, I'm pretty sure the honorable Captain Jean-Luc Picard is on record for that morsel of wisdom.
```

---
## \#74 Posted by: venom121212 Posted at: 2019-02-04T19:17:31.284Z Reads: 210

```
Got all caught up on this thread and I'm so in. My degree is in Biomedical and Human Factors Engineering so I'm pretty sure that means prime beta tester.

Excellent work man. This component has long needed an upgrade

Ooh and I've done haptic feedback work for the Air Force MATB system
```

---
## \#75 Posted by: PatRocks Posted at: 2019-02-04T19:36:40.993Z Reads: 203

```
Interesting _if_ true
```

---
## \#76 Posted by: DerelictRobot Posted at: 2019-02-04T20:25:39.135Z Reads: 209

```
[quote="venom121212, post:74, topic:79808"]
I’m so in.
[/quote]

After you posted about your dick measuring science machine I volunteered you to the Dev team
```

---
## \#77 Posted by: banjaxxed Posted at: 2019-02-04T20:37:47.449Z Reads: 207

```
Stl for that?

[quote="venom121212, post:74, topic:79808"]
I’ve done haptic feedback work for the Air Force MATB system
[/quote]
🤪
```

---
## \#78 Posted by: pat.speed Posted at: 2019-02-04T20:43:12.314Z Reads: 215

```
[quote="banjaxxed, post:77, topic:79808"]
Stl for that?
[/quote]

[quote="venom121212, post:77, topic:79808"]
I’ve done dildo design work for the Air Force MATB system
[/quote]

What is wrong with you people and your dildos
```

---
## \#79 Posted by: Skunk Posted at: 2019-02-04T20:46:58.512Z Reads: 227

```
[quote="pat.speed, post:78, topic:79808"]
What is wrong with you people and your dildos
[/quote]

What's so great about your dildo?
```

---
## \#80 Posted by: SeanHacker Posted at: 2019-02-04T20:48:34.033Z Reads: 232

```
![you-did-it-zsyefg|418x500](upload://1xpPhI3pBHTX10MGyYFlxWIJVcJ.jpeg)
```

---
## \#81 Posted by: pat.speed Posted at: 2019-02-04T20:59:55.951Z Reads: 222

```
It’s my companies, it’s called the speed dildo. I think you can guess why 😉
```

---
## \#82 Posted by: DerelictRobot Posted at: 2019-02-20T03:58:19.191Z Reads: 216

```
Wanted to get input on this- talking with the thumbwheel manufacturer on options. 

This came up at Barrett Junction: how many here would be interested in a version with no brakes? Meaning the entire range of motion on the thumbwheel could be dedicated to throttle, return all the way to one side instead of center. 

I've got one sample on-hand like this and wasn't really considering it until @chaka mentioned that there might be desire for an all throttle, no brakes, gigantic gonads version.

Also PCBs are waiting for me when I get back to the US.
```

---
## \#83 Posted by: Winfly Posted at: 2019-02-20T04:06:15.858Z Reads: 200

```
Sounds like a bad idea. Maybe a second brake mechanism like the R2 remote?
```

---
## \#84 Posted by: mmaner Posted at: 2019-02-20T04:08:38.617Z Reads: 196

```
Would be great for e-foil/surf but I would personally rather have brakes as I like stop gradually, not all at once with lot of blood at the end 😃.
```

---
## \#85 Posted by: Sender Posted at: 2019-02-20T04:10:51.975Z Reads: 194

```
Not a bad idea on a truly purpose built uphill raceboard.

I mean, I want brakes, but I can see the place.  Literally double the fine acceleration control on wicked overpowered boards that do one thing.... win uphill races, and that's it.

Good point on the maytech/r2 solution.

Even if you had a predetermined slowramp brake button... or something. I dunno, been drinkin.
```

---
## \#86 Posted by: lrdesigns Posted at: 2019-02-20T04:13:40.787Z Reads: 200

```
Can't you still have brakes? It's just they will come on automatically when you return the trigger past a point you set in vesc tool. Like in a tesla, one foot driving. Also the brakes will always be on when your not moving.

I would still prefer something that centers, its what im used to and I like spring push back on brakes. 

What about a 70/30 or 60/50 throttle to break ratio, some RC car controllers do that?
```

---
## \#87 Posted by: totalgeek9224 Posted at: 2019-02-20T08:36:21.919Z Reads: 194

```
How about keeping it an option? Should be pretty easy to implement in the software, and then the decision can be made by whoever wants given their preference of the inclusion of the alternate throttle type.
```

---
## \#88 Posted by: Andy87 Posted at: 2019-02-20T09:11:21.476Z Reads: 190

```
how?
I understood that those are two different trigger modules.
one with end / 0 throttle position in center of the trigger travel.
the other with end position in min trigger position.
```

---
## \#89 Posted by: Andy87 Posted at: 2019-02-20T09:14:47.022Z Reads: 183

```
As I don´t plan to use it as race remote i would prefer the option with center position.
I also don´t like the idea, that when I slip off the trigger the board will hit a full break.
```

---
## \#90 Posted by: DerelictRobot Posted at: 2019-02-20T09:25:35.921Z Reads: 190

```
[quote="totalgeek9224, post:87, topic:79808"]
How about keeping it an option?
[/quote]

I should clarify, the all-throttle no brake option is a different model thumbwheel entirely. The thumbwheels ate modular, but they're expensive as hell.

This would be intended as a race track specific variant, zero bearing on the standard offering. 

Thinking back, I wasn't using brakes on the uphill or downhill runs. I can see why people might want this for racing, certainly on uphill where you don't need brakes.

This clearly wouldn't be something everyone would want, but just wanted to put it out there that it's an option. I'll probably grab 1-2 more full throttle thumbwheels
```

---
## \#91 Posted by: DerelictRobot Posted at: 2019-02-20T09:29:01.609Z Reads: 176

```
[quote="Andy87, post:89, topic:79808"]
I also don´t like the idea, that when I slip off the trigger the board will hit a full break.
[/quote]

This can be fixed with proper rate limiting and tuning on the remote firmware. The throttle input can have parametric filtering.
```

---
## \#92 Posted by: totalgeek9224 Posted at: 2019-02-20T10:21:26.081Z Reads: 188

```
Sorry, i should clarify. 
There's two different thumbwheel assemblies in question here:
1) the Full throttle thumbwheel (no brake)
2) Partial throttle thumbwheel (brakes/reverse)

I was suggesting why keep it modular (true to its name :p ) and allow it to be swapped (semi-) easily for those who want it. Like be able to open up the remote, remove the one assembly, and swap in the other. This was those who want it with the Full-throttle thumbwheel can swap it in, whilst also maintaining the usability of the remote with the normal thumbwheel. For those who dont care, it wont matter to them, but for those who do want it, they can install it at their own accord (and cost)

Hope that clarifies a little :p
```

---
## \#93 Posted by: DerelictRobot Posted at: 2019-02-20T10:24:07.220Z Reads: 192

```
This is 100% on point. The thumbwheel and the enclosures are interchangeable, modular.
```

---
## \#94 Posted by: DerelictRobot Posted at: 2019-02-20T13:09:36.692Z Reads: 212

```
 I fleshed out phase 2 & 3 plans a bit more. Looking for additional feedback. 

Just as a general update on my progress on this project:

I have 2 prototypes built up, one ESP & one arduino based- both roughly the size of a RPI and looking uglier than @b264's ass after a weekend in Vegas. I ran into some delays with a shipping mishap + CNY which pushed things back a bit as I'm currently out of country launching pilot projects for the day job. I return March 4th and plan on diving directly into building out the first batch of prototypes to send out for Beta testing. Just wanted to let you guys know this is still moving forward and I've made progress on the codebase, but waiting on PCBs to arrive before I unveil more.

![IMG_20181230_211732|375x500](upload://bmOb9Jk0IhswuaimL2d7bvGOK82.jpeg) 

I was not kidding on the ugly. Prototypes weeee

![Screenshot_20190220-141444|281x500](upload://6nZ9btexolvCrp1jZRcAGNZOEIj.jpeg)
```

---
## \#95 Posted by: Andy87 Posted at: 2019-02-20T13:15:57.583Z Reads: 197

```
some duck tape can fix it!
will look pretty after :ok_hand:
26 of march is my birthday...so perfect timing for getting a prototype ready :joy:
```

---
## \#96 Posted by: venom121212 Posted at: 2019-02-20T13:19:37.887Z Reads: 198

```
Great to hear man. I really like the idea of double the thumb wheel control but can't sacrifice brakes. I think split trigger is the easiest and best solution.

What do you think about one acceleration thumbwheel (only rotates clockwise we'll say) with a second thumbwheel to the right of it that only rotates CCW to handle brakes? 

Pros
-Double the control for brakes and accel, would allow you to set more aggressive settings 
-familiar mechanism with familiar finger 
-you can't accidentally turn one the wrong way, foolproof
-never been done 
-I said so 

Cons
- costs a bit more for 2 wheels
```

---
## \#97 Posted by: DerelictRobot Posted at: 2019-02-20T13:25:31.885Z Reads: 184

```
Maybe I'm not envisioning what you're describing, but I would think two thumbwheels next to each other might not be very intuitive.

Keep in mind the standard offering will just be a center return throttle with acceleration/brake. I already added 4 analog inputs, 2 of which are dedicated to throttle/brake/Deadman inputs. So technologically adding more analog inputs is no big deal, I just want to ensure they make sense and are immediately intuitive to the rider.
```

---
## \#98 Posted by: venom121212 Posted at: 2019-02-20T13:28:00.406Z Reads: 184

```
I see how easy it would be to f up and push the wrong one if you were unfamiliar. But if they are unilateral and can only be pressed in opposite directions from resting position, it won't matter. You can't accidentally press the brakes forward when accelerating or the accel backwards when braking. Just highdeas. If it is only a center return, this wouldn't work. It would have to be rotary phone style rotation that resets to true 0%, not 50%
```

---
## \#99 Posted by: DerelictRobot Posted at: 2019-02-20T13:35:10.659Z Reads: 193

```
[quote="venom121212, post:98, topic:79808"]
It would have to be rotary phone style rotation that resets to true 0%, not 50%
[/quote]

If you check the first post you'll see the two variants I have on hand for testing. One center return, the other is as you describe. Utilizing either isn't an issue, it's making sure it isn't going to be confusing to the rider, ever, that I'm invested in. I don't like overly complicated HCI, nobody does. 

While two thumbwheel inputs are supported, you'll notice I don't have any variants making use of that yet. I'm not opposed, but I'm also not convinced something like the new Maytech remote isn't awkward as hell to use. I want this simple as possible, even the Deadman switch will be entirely optional and user configured.
```

---
## \#100 Posted by: venom121212 Posted at: 2019-02-20T13:38:48.644Z Reads: 198

```
Can't argue with that. We'll talk more after I get that maytech split ha
Here's my awesome drawing I was mocking up. Patent pending. 

![sketch-1550669734772|281x500](upload://4obcSUjhOYkE17Sgn1m1KkVj8Ib.png)
```

---
## \#101 Posted by: DerelictRobot Posted at: 2019-02-20T13:42:40.359Z Reads: 185

```
Yeah that's kinda what I had imagined you were describing. That would make a pretty fat remote and I'm not convinced the two inputs side by side wouldn't be awkward and prone to fatfingering
```

---
## \#102 Posted by: ducktaperules Posted at: 2019-02-20T13:45:36.435Z Reads: 182

```
[quote="Andy87, post:95, topic:79808"]
some duck tape can fix it!
[/quote]

like most things
```

---
## \#103 Posted by: venom121212 Posted at: 2019-02-20T13:51:37.193Z Reads: 189

```
Last point I'll make for clarification purposes, human factors engineering is my focus as well. 

I agree, with the throttle width used, it would be wide. 

Even if you fat fingered it when accelerating (pushing thumb forward), the brake would already be at stopped, 0 position. You couldn't accidentally brake when accelerating or vice versa. The Japanese call it Poka-Yoke. 

I'm done pitching ideas on your thread :yum:
```

---
## \#104 Posted by: DerelictRobot Posted at: 2019-02-20T14:08:36.967Z Reads: 189

```
[quote="venom121212, post:103, topic:79808"]
I’m done pitching ideas on your thread :yum:
[/quote]

Please don't be! I appreciate the input. I guess my concern is not so much that you could hit brakes while accelerating- rather that you'd have to physically move your thumb between the two controls in order to switch over to brake from accelerating. 

In this scenario, each time you want to suddenly brake from an acceleration, would require allowing the throttle to snap back to 0 (which can be filtered to not cause a sudden deceleration) and then moving your thumb over to your brake and start pulling that back. When we're talking milliseconds of reaction time I think that might add unneeded complexity to the input during a critical time. 

I think if we wanted a full throttle thumbwheel w/ brake it might be more intuitive to have a multi-use trigger button on the grip that could toggle the throttle wheel to brake, or simply act as a "longer you hold it down, the stronger the brake applied is". 

These are the exact type of discussions and feedback I'm looking for. Keep it up!
```

---
## \#105 Posted by: venom121212 Posted at: 2019-02-20T14:37:50.195Z Reads: 184

```
Ok glad to not step on any toes. Ideally, the brake wheel would automatically override accel command. Ergonomically, I'd like to have the resting "nub" on the brake wheel slightly more forward than the slow acceleration throttle position for this exact reason. It would make a smooth transition from accel to brake. I imagine my thumb resting on the brake (pressing it forward, the way it can't move and throw you on your face) while accelerating and just rolling my thumb over to the brake quickly. My main issue I see is left handed users. It is certainly not ambidextrous unless modular. 

Regardless of my personal design ideas, I think throttle and brake control separation is a highly sought after aspect and gives you much more room to play. It's certainly not mainstream yet.
```

---
## \#106 Posted by: Gerrycorrado Posted at: 2019-02-20T14:48:32.968Z Reads: 205

```
Whatever you do and whatever you incorporate: safety is the number 1.
As long as it does not loose connection, that is the most important thing I guess (hey, even running a wire to the board, if that is what it takes, I'll run with a wire...)

Anything else is nice to have
Display, board batt level, left over range, POLICE MODE (man, police mode alone is worth gazillions of dollars overhere in europe, we really need police mode), ...

Personally I only run thumb remotes, brake integrated in the same lever. I simply do not understand the evolve remote hahaha (pushing a dead man switch, throttle and then to swap to the brake lever is something I cannot get use to :smiley: ) 
I prefer to pay more for a decent remote than to skim on 5 bucks..

Ah, something else anoying: if it can do firmware upgrades.. correction: if I have to do firmware upgrades: make sure I can. I do not have a fancy chip programmer at home, plugging in a usb is something i CAN do.
I need to do 4 remotes (5 as I need a replacement), so yes it can be a pain in the ass haha

And: test test test.. I prefer to wait a week longer and have a working version than to have to upgrade the firmware already after 2 weeks of shipping, because inthe meantime bugs were found
```

---
## \#107 Posted by: venom121212 Posted at: 2019-02-20T14:51:48.478Z Reads: 208

```
My old but incredibly reliable remote :rofl:
![image|666x499](upload://sRVK93D7Kya4ctvhUUxnsC0YYSi.jpeg) 
Ugh I've come a long way. 

I keep trying to picture a cylindrical remote with trigger brake and thrumb throttle that is reversible for people who like thumb brake, trigger throttle. @DerelictRobot, design all the things!
```

---
## \#108 Posted by: MoeStooge Posted at: 2019-02-20T15:05:39.044Z Reads: 199

```
These are looking pretty dam cool. 
For my setup brakes are a staple. For Track racing and DH a must have for hard charging turn entry. UP-Hill not as much but still used for flatter grade turn entry set-up.  @DerelictRobot nice work being done here 👍
```

---
## \#109 Posted by: rene Posted at: 2019-02-20T15:36:09.554Z Reads: 190

```
What is the product name of your "triggers" 
Would like to inspect the details of those two.
```

---
## \#110 Posted by: Chupacabra Posted at: 2019-02-20T16:36:25.150Z Reads: 190

```
Put me on a list. Would love to test it out. Need brakes though
```

---
## \#111 Posted by: directC Posted at: 2019-02-20T17:31:57.777Z Reads: 189

```
List me up, looks promising
what's you eta?
```

---
## \#112 Posted by: rene Posted at: 2019-02-20T19:54:38.714Z Reads: 184

```
ETA: future
```

---
## \#113 Posted by: directC Posted at: 2019-02-20T20:15:13.372Z Reads: 187

```
just wondering if i might to have a chance to get one before i leave for my world trip in august
```

---
## \#114 Posted by: SeanHacker Posted at: 2019-02-20T20:24:31.773Z Reads: 192

```
I can't answer for him. But I do know he's going to be in and out of the county travelling  for work until next month sometime. So it's highly doubtful.
```

---
## \#115 Posted by: DerelictRobot Posted at: 2019-02-21T02:24:37.572Z Reads: 203

```
[quote="Gerrycorrado, post:106, topic:79808"]
Whatever you do and whatever you incorporate: safety is the number 1.
[/quote]

Please read through my posts on here, you'll see that is my top priority. It's the entire reason behind my choice in radios and the extensive testing I've done and will continue to do. 

For anyone worried about brakes... Please read what I wrote above. It's a modular, reconfigurable design. Some people I've talked to do not want brakes, many do. The choice is entirely yours as there will be a few variants made available by the time I'm done. The standard offering is still a center return with throttle/brake.

But one of my primary design considerations is I want this remote to be a serviceable, modular, piece of gear that can be custom tailored exactly to rider preference. That's why I'm going through the effort of designing multiple configurations. 

A limited run of beta units will be available in March, I believe those dozen or so are already spoken for. Depending on how the beta goes and if I need to make major changes to the design, I'm looking to have the first small production batch of 50 units done by late April/early May. Subject to change, but I don't move on to new projects until I've completed my current, so this will keep marching forward.
```

---
## \#116 Posted by: Itsmedant Posted at: 2019-02-21T02:54:54.439Z Reads: 198

```
I’m excited to see this coming together man! I remember when @Skunk brought it to my attention and I’ve been watching ever since. Any idea I’ve had was already posted and asked but I’ll keep thinking!!

Seeing your quality of work or everything else you do, I know these things are gonna be the tits!
```

---
## \#117 Posted by: venom121212 Posted at: 2019-02-21T02:57:29.714Z Reads: 196

```
Yeah is there any way to make it more dong shaped? Asking for a friend...
```

---
## \#118 Posted by: DerelictRobot Posted at: 2019-02-21T03:01:26.650Z Reads: 205

```
Don't let your dreams be dreams man. Go nuts.

But wait until you see the limited edition Jason-X. :smile:
```

---
## \#119 Posted by: Bobby Posted at: 2019-03-28T08:26:55.965Z Reads: 200

```
Any updates on this guy?
```

---
## \#120 Posted by: DerelictRobot Posted at: 2019-03-28T13:51:23.398Z Reads: 213

```
Sorry I'd posted the updates elsewhere. ;)

PCBs are in, right now I'm just waiting on the first order of Thumbwheels from the manufacturer. 

Beta sign up is here:

https://docs.google.com/forms/d/e/1FAIpQLSfur8A2tMX3j8wFzUg5vYyUHeQkvXo-jed9LlgMONP552B5Ag/viewform?usp=send_form

Beta units will be reduced price from the final retail, but as I've already got more signups than expected I might have to decline some people as my stock allows for. I ordered enough parts to build out 25 units for the beta. These won't be the final PCB version and it is a "print your own case/community printed version (Nylon 910 alloy filament, super tough)", however all the expensive components are socketed so beta users will be given the final PCBs to bring their stuff up to production version when it's done. 

No money is being taken right now- I don't really love pre-orders and am trying to avoid that, so once I have units ready to ship I'll invoice. Approximate cost on beta units is $200 USD but subject to change. 

https://forum./t/osrr-a-high-performance-open-source-racing-remote-for-esk8/322
```

---
## \#121 Posted by: youseekcota Posted at: 2019-03-31T17:21:37.899Z Reads: 195

```
Stoked on this remote. Had a chance to use one of the early prototypes and the Hall control is so smooth, and has adequate throw unlike any other remote I've tried.
```

---
## \#122 Posted by: directC Posted at: 2019-03-31T17:54:57.717Z Reads: 198

```
why didn't i see this earlier?!  
signed up, hope i'm still in
```

---
## \#123 Posted by: DerelictRobot Posted at: 2019-03-31T18:03:38.448Z Reads: 202

```
Was great to meet you at Bakersfield! I've been riding with that prototype daily, the amount of throw on the throttle takes a little getting used to but it allows for so much fine control.
```

---
## \#124 Posted by: DerelictRobot Posted at: 2019-04-26T20:58:22.522Z Reads: 200

```
First 10 beta units are getting built up, shooting to ship in approx 1 month. Still have a few slots left on the first batch. PM me for details, those signed up on the beta will be receiving an email and will have first dibs. 

Nano style grip WIP:

https://a360.co/2L7e3EU
```

---
## \#125 Posted by: DerelictRobot Posted at: 2019-05-06T20:46:47.009Z Reads: 204

```
First round of beta is all filled up! I'll have details on round 2 after we get round 1 going.

I've been riding daily using my Nano style prototype to ensure there are plenty of road miles logged before I officially ship the beta units for testing. So far have about 300 miles ride time on my remote, it's performing great.

Zero disconnects of any kind. Line of site in urban environments I have seen about 25m of range before I start seeing substantial packet loss.

On average I'm logging 99.3-99.7% overall signal strength quality. Rock solid. 

![IMG_20190506_100457|375x500](upload://yOT4c1OMBudxqxdUM7dDEexF5gP.jpeg) 
Excuse the rough low-res print, I've been churning out design iterations and focused on internals more than looks for now. 

Printing up latest version of the Nano XL style enclosure as we speak. This is by no means a final version, but I've made the Nano XL available for download for anyone who wants to check it out:

https://a360.co/2L7e3EU

Also started design work on the Grenade/Puck style enclosure last night:

https://a360.co/2J2lDih
```

---
## \#126 Posted by: banjaxxed Posted at: 2019-05-06T20:54:40.084Z Reads: 195

```
Love that Holy Hand Grenade dude, so glad to have jumped on this ride
```

---
## \#127 Posted by: DerelictRobot Posted at: 2019-05-06T20:59:43.225Z Reads: 196

```
And.... You just named that model.
```

---
## \#128 Posted by: torqueboards Posted at: 2019-05-06T21:11:35.262Z Reads: 195

```
Looking good! Remote looks awesome!
```

---
## \#129 Posted by: SeanHacker Posted at: 2019-05-06T21:36:39.974Z Reads: 199

```
Turn that remote around and hold it right dude. ;)
```

---
## \#130 Posted by: DerelictRobot Posted at: 2019-05-08T01:54:42.244Z Reads: 197

```
Printed an updated set of Nano XL shells before I jumped into the 20 hour print of the HHG Puck. Gave them the HD rubberized treatment. 

![IMG_20190507_093128|666x500](upload://fBFXaD1OcQVFetwAMmy867pjVxF.jpeg) ![IMG_20190507_161453|666x500](upload://xafId98QHeRBrxklHDtgtHErmQU.jpeg) 
![IMG_20190507_184822|375x500](upload://JtVgBd54lRFND9x2xsYvLTNm4G.jpeg)

Charging is via magnetic reversible port on USB.

HHG Puck top shell in progress:
![IMG_20190507_185847|666x500](upload://wOI3RC76DZ7OUT1nSg42lmVPR7r.jpeg)
```

---
## \#131 Posted by: DEEIF Posted at: 2019-05-08T02:10:57.407Z Reads: 189

```
Dang derelict I might have to build a board faster just to grab one of these 😍
```

---
## \#132 Posted by: Bobby Posted at: 2019-05-08T02:44:41.707Z Reads: 187

```
For sure in on the second round. Looks effin awesome. Only issue is the display... i hold my remote in my left hand....any chance a left handed remote can be requested
```

---
## \#133 Posted by: Linny Posted at: 2019-05-08T02:52:00.043Z Reads: 184

```
Left hand indeed! 

This awesome progress @DerelictRobot!
```

---
## \#134 Posted by: DerelictRobot Posted at: 2019-05-08T03:15:25.733Z Reads: 184

```
I see no reason why a left handed version couldn't be made. Had it in mind for sure, mirroring each design isn't too hard.
```

---
## \#135 Posted by: Andy87 Posted at: 2019-05-08T03:17:07.710Z Reads: 179

```
@DerelictRobot the magnetic charge port will be standard? If yes, you will also supply the usb part with it or as min share a link where we can get the right cable?
```

---
## \#136 Posted by: DerelictRobot Posted at: 2019-05-08T03:19:53.390Z Reads: 182

```
Sure thing! Not sure if this will be final or if I'll eventually move to USB-C. This is an easy solution to seal the port though. 

NetDot Gen10 Micro USB Nylon Braided Magnetic Fast Charging Cable with Side LED Compatible with Android Device(3.3ft/3 Pack Black) https://www.amazon.com/dp/B07JYZCPLG/ref=cm_sw_r_cp_apa_i_xPK0Cb5X0TST6

Plan is to include one of these cables + magnetic port installed on the beta units.
```

---
## \#137 Posted by: Andy87 Posted at: 2019-05-08T03:27:23.935Z Reads: 182

```
Any thoughts on installing something like this instead of a charge port?

https://s.click.aliexpress.com/e/b7kyX2CS
```

---
## \#138 Posted by: DEEIF Posted at: 2019-05-08T03:29:31.118Z Reads: 178

```
I think you said this but what is the price for a beta?
```

---
## \#139 Posted by: pookybear Posted at: 2019-05-08T03:41:50.576Z Reads: 178

```
Damn. If I only have a third uart port, I would have been all over this.
```

---
## \#140 Posted by: DerelictRobot Posted at: 2019-05-08T03:56:48.578Z Reads: 176

```
Neat idea but the size of that pad is pretty substantial from the looks of it. 

Beta price on round 1 was $225 for the Dev kit.
```

---
## \#141 Posted by: Andy87 Posted at: 2019-05-08T04:04:41.938Z Reads: 180

```
It was just an example I found on the go. I‘m sure there are other pads which could fit or you could cut in right size. In fact it’s just spiral pad. I‘m happy with any port for sure, just an idea for inspiration 😉
```

---
## \#142 Posted by: DerelictRobot Posted at: 2019-05-08T04:32:11.866Z Reads: 183

```
I dig it, will definitely keep an eye on these. 

Currently The Nano XL design is about the same size range as the GT2B, but personally I find it easier to handle gloved. Not sure how much I can shrink the size of this one without a PCB revision (which will come inevitably). I like the current size of the XL quite a bit though. @SeanHacker has a GT2B remote and has used my Nano XL Prototype, so he can probably comment on the difference & feel.  

The HHG Puck is shaping up to be a more compact design overall, probably better suited for those who don't like larger size remotes. I should have a prototype built up tomorrow.
```

---
## \#143 Posted by: Bobby Posted at: 2019-05-08T04:45:10.058Z Reads: 182

```
Like i said... dibbs on round 2
```

---
## \#144 Posted by: SeanHacker Posted at: 2019-05-08T05:17:21.343Z Reads: 191

```
Yeah. I have a GT2B with a @FLATLINEcustoms MadMunkey case. The comparison is about right. The Nano-XL is thinner than it though. Girth might be a little bigger. I do really like the thumb control which is weird because I'm a trigger guy. 

I'll take comparison pics tomorrow when they're both in the same room. ;)

![IMG_20190507_215130_01|375x499](upload://tOt0AzmUPkNEGWwlADlomGeZGJU.jpeg)
```

---
## \#145 Posted by: Andy87 Posted at: 2019-05-08T05:29:41.768Z Reads: 185

```
Please don’t forget the banana for scale than!
```

---
## \#146 Posted by: SeanHacker Posted at: 2019-05-08T05:59:10.545Z Reads: 183

```
Fuck! I'm out of bananas!!! Calling Mom ASAP!
```

---
## \#147 Posted by: banjaxxed Posted at: 2019-05-08T16:46:23.930Z Reads: 184

```
I'm questioning your choice of control samples Andy

![image|377x500](upload://9TbfGlDwhsjf1h7eBOwodRRK49O.jpeg)
```

---
## \#148 Posted by: Linny Posted at: 2019-05-08T16:47:46.036Z Reads: 183

```
That'll make a mean banana split
```

---
## \#149 Posted by: Bobby Posted at: 2019-05-08T16:50:09.198Z Reads: 193

```
To be fair to Andy, Ive always known bananas to be pretty big myself
![image|375x500](upload://rn6B8wS0ZpMZLqHKGg7h77xefhW.jpeg)
```

---
## \#150 Posted by: DerelictRobot Posted at: 2019-05-08T18:12:35.103Z Reads: 194

```
Road testing, such a hard part of the job. 

![IMG_20190507_190752|666x500](upload://z9HTciLU5wgqPqrMJVlqqF90zFn.jpeg) 

First pass at the HHG Puck enclosure, will build it out tonight.
![IMG_20190508_092752|666x500](upload://eAiEylP6e8F95LAjRVqMdmCGIn3.jpeg) ![IMG_20190508_092830|666x500](upload://aCEieNxFON6sbQWeNNqyjFlw962.jpeg) ![received_337695340263938|301x500](upload://hyfdHlRMM3fiq9HAEVfnAFDnc4Y.jpeg)

Power button is recessed about 4mm from the top of the enclosure. A bit larger than the Hoyt Puck.
```

---
## \#151 Posted by: skelstar Posted at: 2019-05-08T18:49:21.693Z Reads: 185

```
Like the Puck enclosure idea. Pity I wouldn't be able to hold it properly with wrist guards (so annoying).

I haven't read every word: what the throw like on that "joystick"? I one of the main issues I have with triggers/joysticks on remotes.
```

---
## \#152 Posted by: directC Posted at: 2019-05-08T19:09:32.479Z Reads: 182

```
I'm questioning your arm...
```

---
## \#153 Posted by: DerelictRobot Posted at: 2019-05-08T19:35:30.213Z Reads: 190

```
[quote="skelstar, post:151, topic:79808"]
what the throw like on that “joystick”? I one of the main issues I have with triggers/joysticks on remotes.
[/quote]

100 degrees of travel. I can say from 'feel', it feels about double the amount of throw from what we're used to seeing given the added height of the thumbwheel. Takes some getting used to even, it's that noticeable.
```

---
## \#154 Posted by: skelstar Posted at: 2019-05-08T19:57:02.687Z Reads: 184

```
_Ooooooooooo_ _(considers finding and placing an order for joystick)_
```

---
## \#155 Posted by: Sender Posted at: 2019-05-08T20:07:30.068Z Reads: 192

```
[quote="skelstar, post:154, topic:79808, full:true"]
*Ooooooooooo* *(considers finding and placing an order for joystick)*
[/quote]

Gotta know what to do with it 😉🍆🍑.
```

---
## \#156 Posted by: brenternet Posted at: 2019-05-08T23:51:31.819Z Reads: 189

```
[quote="banjaxxed, post:126, topic:79808"]
Love that Holy Hand Grenade
[/quote]

Trust an Irishman to turn this into a religious war
```

---
## \#157 Posted by: banjaxxed Posted at: 2019-05-09T07:03:55.197Z Reads: 184

```
😁 On a Crusade again Sir Brent?
```

---
## \#158 Posted by: Komamtb Posted at: 2019-05-11T08:52:10.931Z Reads: 188

```
I guees I will be selling my photon..
```

---
## \#159 Posted by: DerelictRobot Posted at: 2019-05-19T19:49:41.126Z Reads: 181

```
![IMG_20190519_102915|666x500](upload://usART5s3BM4nqdOO4RYiJdfYE1g.jpeg) ![IMG_20190519_075846|375x500](upload://8SyyLuFUY1Zoy3pgmlgoqxFL1Ft.jpeg) ![received_630534564130978|301x500](upload://rYKK7pQzZopfoa3m7plqabE4O9h.jpeg) ![image-20190518_174654|375x500](upload://wIGMNOPrHJOXi50zgSvGnDXrDG4.jpeg) ![IMG_20190518_163725|666x500](upload://qcfRpeDHy2XeRWbcixZaL3GtiPl.jpeg) ![IMG_20190518_163745|666x500](upload://yo2a72K7C7jgLzUcelyRmpxzLtL.jpeg) ![IMG_20190518_163751|666x500](upload://cObhMAlRSS4RNF7ZJdSWUHMrMPL.jpeg)
```

---
## \#160 Posted by: Sender Posted at: 2019-05-19T19:50:39.162Z Reads: 174

```
Too damn good.
```

---
## \#161 Posted by: DerelictRobot Posted at: 2019-05-19T19:55:36.736Z Reads: 174

```
Flattery will get you everywhere. <3
```

---
## \#162 Posted by: Sender Posted at: 2019-05-19T20:01:58.762Z Reads: 174

```
Not as far as a good blow job...
```

---
## \#163 Posted by: totalgeek9224 Posted at: 2019-05-20T16:16:36.431Z Reads: 174

```
https://memegenerator.net/img/instances/79996546.jpg
```

---
## \#164 Posted by: Sender Posted at: 2019-05-20T16:18:20.982Z Reads: 171

```
For sure. This is the coolest thing going on in the forum RN.

Well, along with this silver surfer Killshot that is 😂😂

![20190519_214338|634x500](upload://sTe2LvqCAFA7qvTqwQSuuhhXFNc.jpeg)
```

---
## \#165 Posted by: totalgeek9224 Posted at: 2019-05-20T16:20:22.056Z Reads: 173

```
Im glad im not the only one who thinks so. I keep refering back to thing like this and that in the hope sof updates or details that i had previously missed. I think im just living vicariously though others ahah

Edit: God damn i want to be able to skin like that. Gonna be another masterpiece when its done. If im ever in AL, know that youve got an intern ;)
```

---
## \#166 Posted by: SeanHacker Posted at: 2019-05-20T16:22:01.683Z Reads: 175

```
[quote="Sender, post:162, topic:79808, full:true"]
Not as far as a good blow job…
[/quote]

Tell me about it... 

![IMG_20190519_102344|375x500](upload://i7sIuaCya3UaKtZwfh3EvERp7JD.jpeg)
```

---
## \#167 Posted by: totalgeek9224 Posted at: 2019-05-20T16:30:08.571Z Reads: 175

```
Why not both? ![38|690x385](upload://dJus8kVZyw0l133M7zNpKYO5nKk.jpeg)
```

---
## \#168 Posted by: Andy87 Posted at: 2019-05-20T17:29:55.732Z Reads: 171

```
@DerelictRobot i‘m about to design a new case for my escs. Could you tell me the dimensions of the receiver box? I would like to make the case directly fit the receiver.
```

---
## \#169 Posted by: brenternet Posted at: 2019-05-20T18:08:18.541Z Reads: 173

```
Ben has a file for that, just ask him to send it over.
```

---
## \#170 Posted by: DerelictRobot Posted at: 2019-05-20T18:58:25.703Z Reads: 167

```
Do you just want to design a spot for the receiver PCB to be integrated into the case? The little enclosure I printed up is optional really. I have 3D models of everything~

BTW- I can't recall if I mentioned it earlier, but download is enabled on both current 3D models for the grip enclosures. They are WIP- but still workable. Names are "official". 

Holy Hand Grenade (HHG): https://a360.co/2J2lDih

Her Majesty's Pleasure (HMP): https://a360.co/2L7e3EU
```

---
## \#171 Posted by: Andy87 Posted at: 2019-05-20T19:41:56.201Z Reads: 164

```
I just want to know how much space I need to reserve for the receiver. With it without box doesn’t matter.
```

---
## \#172 Posted by: DerelictRobot Posted at: 2019-05-20T20:11:00.590Z Reads: 164

```
35x30x16mm with enclosure.
```

---
## \#173 Posted by: SeanHacker Posted at: 2019-05-20T20:16:27.532Z Reads: 173

```
@DerelictRobot does house calls if you're local. Just saying...

![IMG_20190520_100407|666x499](upload://j6fcG93ZREHK41xcm8tskb4QT2J.jpeg)
```

---
## \#174 Posted by: Lionpuncher Posted at: 2019-05-21T23:00:52.364Z Reads: 170

```
Dropped in to check progress, just about shot a load in my pants after seeing that hhg puck. I MUST HAVE!! @DerelictRobot please tell me I’m still on the list for round 2 beta. So excited for this project. Looking hella sexy my friend!!!
```

---
## \#175 Posted by: DerelictRobot Posted at: 2019-05-21T23:30:30.325Z Reads: 174

```
You are indeed!

I think I forgot to post the latest HHG prototype here.

![IMG_20190510_190209_779|500x500](upload://g3A1slZXJR84ne9DXTtEuP15WQV.jpeg) 
![IMG_20190514_102040_717|666x500](upload://8JQWGM2D70yxEtPuLTuyrRIeVF6.jpeg) ![IMG_20190510_170013|666x500](upload://d8IBcCQ9I2dhNx1QJ69XJ2CW0Ev.jpeg) ![IMG_20190511_152341|666x500](upload://dLVqZQohC8yGnL3x8FQJJntAMRM.jpeg)
```

---
## \#176 Posted by: McErono Posted at: 2019-05-21T23:33:17.952Z Reads: 170

```
I want in! Need this thing, maybe both.
```

---
## \#177 Posted by: XplorerBE Posted at: 2019-05-21T23:56:12.755Z Reads: 168

```
Very very nice work.
Following.

Still places available în beta round 2 ?-) 
I would like a spot if still possible.
```

---
## \#178 Posted by: Kellag Posted at: 2019-05-22T00:31:51.948Z Reads: 165

```
Yes same question
```

---
## \#179 Posted by: Kresher Posted at: 2019-05-22T00:44:55.964Z Reads: 168

```
Not to sound redundant, But I would also be happy to be a second round beta tester. And Also, I was wondering about the trigger remote, is that what's next on the list?
```

---
## \#180 Posted by: jimmymagix Posted at: 2019-05-22T02:19:50.210Z Reads: 166

```
I'd like to be on that beta 2 also!
```

---
## \#181 Posted by: McErono Posted at: 2019-05-23T10:08:40.496Z Reads: 161

```
@DerelictRobot  just to make sure: as long as there is no PPM/PWM receiver, the OSRR is not usable with a Unity right?
```

---
## \#182 Posted by: brenternet Posted at: 2019-05-23T10:26:20.167Z Reads: 161

```
I hate it when product developers don't respond. Get the pitchforks out boys
```

---
## \#183 Posted by: Itsmedant Posted at: 2019-05-23T11:39:07.729Z Reads: 165

```
[quote="brenternet, post:182, topic:79808, full:true"]
I hate it when product developers don’t respond. Get the pitchforks out boys
[/quote]
Should we start vendor bashing yet?
```

---
## \#184 Posted by: mikenyc Posted at: 2019-05-23T12:30:47.581Z Reads: 161

```
He's not a vendor though is he? Bash away!
```

---
## \#185 Posted by: venom121212 Posted at: 2019-05-23T13:35:56.597Z Reads: 164

```
Hi, will this remote have the automatically brake if remote dropped anti safety feature?

I call it the BrakeBreak©
```

---
## \#186 Posted by: Sn4pz Posted at: 2019-05-23T13:50:35.030Z Reads: 169

```
Pretty sure that's the estop from @StefanMe s feather remote 🤔 

Regardless, it should be available in all highend remotes. Maybe my feather will go to my Spud and I'll get one of these o3o
```

---
## \#187 Posted by: Itsmedant Posted at: 2019-05-23T13:57:34.744Z Reads: 169

```
I won't bash @DerelictRobot, but I would smash 10/10. Have you seen him? boomshakalaka.
```

---
## \#188 Posted by: brenternet Posted at: 2019-05-23T15:48:15.181Z Reads: 167

```
He reminds me of an older Ed Helms
```

---
## \#189 Posted by: DerelictRobot Posted at: 2019-05-23T16:24:35.998Z Reads: 170

```
Actually I already have standard VESC + Unity support on the remote fully tested. My current daily rider has a Unity + OSRR. 

I still plan on adding PWM/PPM output to the advanced receiver, for now UART has been working great.
```

---
## \#190 Posted by: DerelictRobot Posted at: 2019-05-23T16:33:25.026Z Reads: 176

```
I intentionally kept beta round 1 small to keep it focused, but I haven't capped round 2 in size. Please sign up, when I'm ready to open beta #2 I'll send out an email to everyone on the list with how many slots I've got open and it's filled first come first serve.

Sign up found here:

https://www.electric-skateboard.builders/t/osrr-a-high-performance-open-source-racing-remote/79808/120?u=derelictrobot
```

---
## \#191 Posted by: DerelictRobot Posted at: 2019-05-23T20:22:25.571Z Reads: 156

```
Ed Helms is like... A decade older than I am. 

Are you calling me fat Brent?
```

---
## \#192 Posted by: Bobby Posted at: 2019-05-23T20:27:07.061Z Reads: 158

```
I believe he is just saying you look old af
```

---
## \#193 Posted by: DerelictRobot Posted at: 2019-05-23T20:29:49.716Z Reads: 156

```
You don't want to get in between this lover's quarrel Bobby.
```

---
## \#194 Posted by: Bobby Posted at: 2019-05-23T20:33:15.296Z Reads: 159

```
![image|220x167](upload://5r9eVukvH5KZKUfEKTrm4svHmd4.gif)
```

---
## \#195 Posted by: brenternet Posted at: 2019-05-23T23:08:07.147Z Reads: 156

```
[quote="DerelictRobot, post:191, topic:79808"]
Are you calling me fat Brent?
[/quote]

Yes. Eat shit
```

---
## \#196 Posted by: venom121212 Posted at: 2019-05-23T23:47:38.595Z Reads: 156

```
Or maybe eat less shit? Not sure on calorie count of the average turd.
```

---
## \#197 Posted by: SeanHacker Posted at: 2019-05-23T23:47:55.580Z Reads: 156

```
This is the solution.
```

---
## \#198 Posted by: lrdesigns Posted at: 2019-05-24T00:24:11.359Z Reads: 157

```
Well now I'm googling eating poop. Thanks guys. 

https://gawker.com/5985723/can-you-eat-your-own-poop

https://www.reddit.com/r/askscience/comments/1hjgwq/how_many_calories_are_in_poop_vs_how_many/

I think it would be a decent weight loss strategy.
```

---
## \#199 Posted by: SeanHacker Posted at: 2019-05-24T00:39:54.530Z Reads: 152

```
"Thank you for this interesting inquiry. Drinking your own urine and eating your own poop is perfectly safe."

This is all I read. It's also dinner time at my house. I've been looking for ways to save a buck or two.
```

---
## \#200 Posted by: DerelictRobot Posted at: 2019-05-24T00:43:40.428Z Reads: 156

```
![ryUYlev|480x337](upload://pSnaJx4FOFtM77Y0o1vfwPjoH4C.jpeg)
```

---
## \#201 Posted by: lrdesigns Posted at: 2019-05-24T00:49:32.644Z Reads: 159

```
![image|635x445](upload://x1yj2Ulh7TiSAQn4GoswEqxv5bV.jpeg)
```

---
## \#202 Posted by: DerelictRobot Posted at: 2019-05-24T01:26:23.428Z Reads: 157

```
This is why I'll never be a _real_ vendor. 

Thanks guys.
```

---
## \#203 Posted by: taz Posted at: 2019-05-24T05:25:34.010Z Reads: 158

```
I walked in this thread because I was promised a good show and vendor bashing.

I am deeply disappointed.

(@brenternet , @SeanHacker I expected more from you guys, you let me down).
```

---
## \#204 Posted by: brenternet Posted at: 2019-05-24T07:45:14.481Z Reads: 155

```
It's too easy, Andrew has that whole humble brag thing going on that he ruins himself with. It's like taking candy from a poorer Jason Sudeikis.
```

---
## \#205 Posted by: tomiboi Posted at: 2019-05-26T20:24:28.912Z Reads: 155

```
Sa da tay wadatah... yous a bad lamma tammy! My dilly... sepatown in da tines!
```

---
## \#206 Posted by: Bobby Posted at: 2019-05-26T21:22:44.727Z Reads: 155

```
Well cole me down on the patty sty! Whats the dabble dee?
```

---
## \#207 Posted by: Sender Posted at: 2019-05-27T10:46:08.370Z Reads: 142

```
Due to all the bans, you can find updates on this on the Esk8 News forum.
```

---
## \#208 Posted by: banjaxxed Posted at: 2019-05-27T11:49:59.826Z Reads: 140

```
#freethefour
```

---
## \#209 Posted by: Multi Posted at: 2019-07-23T18:42:10.677Z Reads: 85

```
https://www.coolgear.eu/product/shinecon-ar-game-gun-shooting-games-gamepad-toy-for-smart-phone-supports-all-smartphones-with-for-android-or-ios/

this is a suicidal design
```

---
