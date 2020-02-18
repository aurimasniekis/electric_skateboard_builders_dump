# Ground Up E-Freeboard &#124; Custom Control Algorithm: Dual VESC &#124; Dual, HUB 2200W 150KV Motors &#124; Work In Progress &#124;

### Replies: 67 Views: 8667

## \#1 Posted by: VillainousJackal Posted at: 2017-06-01T18:32:39.691Z Reads: 574

```
Hey Kids,

Intent: This marks the beginning of a multi-month ground up build. I will be attempting to create a electric freeboard almost entirely from scratch. I will periodically post my progress here, as well as links to relevant articles, my CAD files, and my motor control Code.

Background: I am a Senior in Electrical Engineering at Purdue with a heavy background in parts fabrication and controls. This summer, I am interning in Detroit, and my company (omitted), also encourages personal projects that double as learning experiences. Thus, inspired by the LEIF board, an idea was born. What if I could completely design, fabricate, and program an electric freeboard from scratch for under $1000? 

Thus far, I have CADed a proof of concept, begun my second design iteration, have started performing calculations for desired Motor Spec, and have created a (pseudo)-working control algorithm for a 3-phase brushless outrunner I had lying around. 

Lets start with my proof of concept.

<img src="/uploads/db1493/original/3X/5/4/54502df49b09364fdd20d336452c81f29b29f3b9.png" width="690" height="206">

Before you say anything, I know that it looks pretty jank, expensive, and overly complicated. The intent was to demonstrate a working design to get funding before moving on to the next couple iterations. 

Here are a few more pics:

<img src="/uploads/db1493/original/3X/a/7/a7659285216112e86732f3e068837643d9f58fee.png" width="690" height="388">
<img src="/uploads/db1493/original/3X/a/5/a54ebb4f449ea970997c86baf11c87f93eabf98a.png" width="690" height="388">

This design featured off the shelf parts to enable the wheel pods to rotate, mostly a 200lb lazy susan, and a 3 lead, 30 amp slip ring which would allow the passage of current to the pod, without having to worry about leads getting twisted. Additionally, it made use of two, 18" Carbon fiber rods and a series of belly pans to create a superstructure allowing battery mounting and mounting of the control electronics. 

This design has several problems. 
FIRST: It's expensive, It's heavy, and overly complicated. The carbon fiber alone would cost about $170, which is too much for (at best) a medium amount of flash. The Aluminum wouldn't be too expensive itself, but as i no longer own a waterjet, I would need to pay someone to waterjet it for me, which would not only cost more money, but would also dent my pride ;)

Furthermore, 30 amps is not nearly enough to drive these motors, which usually are happy around 60-70 amps each. I looked around online, and couldn't find a slip ring that would fit my design for less than $750 each. So again, no go. 

So, scrap that. She was pretty, but not feasible. 

This brings us to my second design iteration. 
<img src="/uploads/db1493/original/3X/b/7/b7412309c94f131000930b32ed33f025d2cb9b5d.png" width="690" height="388">
<img src="/uploads/db1493/original/3X/e/a/eaee7e0cab87c7bdbc77a9b07b67b05d7ef30135.png" width="690" height="388">

This design features a custom-made, combination slip-ring lazy susan and a wheel mounted directly to the exterior of an outrunner. As seen in the first picture, the lazy susan comprises three stages, each electrically isolated from the others, which doubles as a slip ring, allowing individual currents to pass through each of the three "phases" to the corresponding phase of the motor. 

This design has not been flushed out yet, but that's kind of the point of an ongoing blog right?

On to controls.

I plan to utilize an arduino uno to pass PWM signals to the gates of a standart MOSFET array, allowing current to flow into each phase of the motor in time. A great synopsis of this, as well as the control theory behind brushless motors, can be found here: http://electronoobs.com/eng_circuitos_tut4.php 

I actually plan to follow his process quite closely, finally diverging in the speed control stage. Rather than use a delay between phases (which will result in somewhat choppy feel) i will use PWM control to modify the duty cycle of the motor, allowing speed to vary that way.

Thus far, 
I have built my array, and flashed my arduino.
<img src="/uploads/db1493/original/3X/9/8/9862becc4db4d030fb00b6e3ea89d3515f84bfa1.png" width="666" height="500">
<img src="/uploads/db1493/original/3X/4/d/4d943461a5d63a18a04aa4a3f35e8bc7115a5228.png" width="666" height="500">
<img src="/uploads/db1493/original/3X/c/5/c5e795f0ea5826a43e5d18217f4db452362822dc.png" width="666" height="500">

However, When i execute my code, i have no way to determine the position of the rotor, resulting in a high level of shoot-through and reverse driving. I'm overworking the FETs i have, and am not able to produce the smooth drive action i want. 

Thus, as any electrical engineer does, I need more sensors. 

I plan to buy two motors with hall effect sensors that will allow me to monitor the precise position of the rotor relative to the stator, and create a much smoother motor drive. 

However, before i can do that, I need to buy motors, and before i can buy motors, i need to pick them. 

I am thinking about running a 4 cell set up. The batteries i have are 61 amp hours, so they're massive, and can push any amperage i could ever want. But they're big. Thus, i will use a higher Kv motor, at a lower voltage to achieve similar results to those i would get with a lower Kv motor, and higher cell count.

I have run the math, and it looks like i should be able to hit about 25 mph with 4 cells and two 2000 watt 270kv motors. It's also noteworthy that I will be using 78mm casters. 

I can't obtain any torque curves for these motors, but i think that they should work. Any feedback from people with hands-on experience would be great. 

That's all for now!
```

---
## \#2 Posted by: Davey Posted at: 2017-06-01T20:22:39.653Z Reads: 465

```
subbed! I guess you already know leiftech's electric freeboard?
```

---
## \#3 Posted by: VillainousJackal Posted at: 2017-06-01T20:26:19.846Z Reads: 455

```
Yeah, But the leif board is $1600, I'm shooting for a faster one for under $1000
```

---
## \#4 Posted by: SilentException Posted at: 2017-06-01T20:28:01.562Z Reads: 442

```
This is great, definitely watching this one!

Yes there is LEIFTech eSnowboard and they have patents over this kind of stuff so be aware of that. But I doubt they will do anything to stop your build unless you start selling the boards :)
```

---
## \#5 Posted by: VillainousJackal Posted at: 2017-06-01T20:30:30.972Z Reads: 427

```
Thanks for the info! 

I was thinking about picking up trucks from Freebord, anyone have any experience?
```

---
## \#6 Posted by: Davey Posted at: 2017-06-01T20:33:21.680Z Reads: 409

```
and you should look at this thread: https://www.electric-skateboard.builders/t/nowinds-first-commercial-board-leiftech-e-snowboard/23571
```

---
## \#7 Posted by: keegancdr Posted at: 2017-06-01T20:44:58.763Z Reads: 396

```
I ride a freebord (not powered) and those bindings are great! they lock your feet in when you need it, but you can easily bail out if needed
```

---
## \#8 Posted by: Mobutusan Posted at: 2017-06-01T20:48:57.463Z Reads: 383

```
Great project! It's about time someone did this. I still want to see an all terrain version; if that would even work. :wink: Just throwing that out there.
```

---
## \#9 Posted by: Davey Posted at: 2017-06-01T21:00:34.728Z Reads: 390

```
I guess you can do At but the question is how it would ride. Maybe I'm wring but I guess the pneumatic wheels will like stop the drift or act weird. But a very interesting idea indeed! :slight_smile:
```

---
## \#10 Posted by: SilentException Posted at: 2017-06-01T21:30:33.396Z Reads: 407

```
[quote="VillainousJackal, post:1, topic:24354"]
Thus, as any electrical engineer does, I need more sensors. 

I plan to buy two motors with hall effect sensors that will allow me to monitor the precise position of the rotor relative to the stator, and create a much smoother motor drive.
[/quote]

Few weeks back I was watching a nice video from Mellow Boards explaining how they drive their motors using FOC and TI Piccolo micro controller with patented algorithm to detect position of the rotor without using any sensors which are in their words just another point of failure :) Maybe of interest to you and your build.

https://www.youtube.com/watch?v=hCq77SYM3bU

I know I learned few things from that video :)
```

---
## \#11 Posted by: VillainousJackal Posted at: 2017-06-01T22:44:26.002Z Reads: 385

```
Hey! Thanks for the link. The way they do that is via the back EMF on the unused coil. When a coil of wire moves through a magnetic field, it generates electromotive Force (EMF) in accordance with faradays law. So like he said, as you power two leads, the magnet turns, moving the field and changing the flux in the third coil. You can actually read the voltage on that coil to determine the relative positions of the rotor. However, because I am using an arduino, I'm limited to 4 milliamps of current into my analog pins. That's 0.004 amps, whereas that back EMF generates about 1,000 times that. This means that i would need to use a current division circuit to divert most of the current to ground. However, even then I run the risk of picking the wrong resistor values and burning out my board, or a resistor coming loose, and burning out my board. 

On the other hand, I could spend the extra $6 for a sensored motor, and get a more precise, more reliable reading of where the rotor is. Also, I'm hoping to go into controls as a career, so the more learning I can force, the better. 

Just my thoughts :slight_smile:
```

---
## \#12 Posted by: VillainousJackal Posted at: 2017-06-01T22:46:19.967Z Reads: 357

```
@Mobutusan, I think the best way to do AT would be to replace the casters with pneumatic, which would increase your ride height significantly. Not sure if that tradeoff is worth it. But hey, follow your dreams!
```

---
## \#13 Posted by: Smorto Posted at: 2017-06-01T23:05:24.974Z Reads: 341

```
This is awesome! I have dreams of doing this myself as I currently ride a non-motorized freebord myself (on that walk back up the hill, the mind starts to dream...). One tip, learn how to ride a non-motorized freebord if you haven't already to get the feel for it before you use your electric one. I am tracking this thread and it should be awesome! Good luck!
```

---
## \#14 Posted by: VillainousJackal Posted at: 2017-06-02T16:07:48.501Z Reads: 374

```
Update 2

Today I created a google drive where i will post all my math, code, and CAD.

https://drive.google.com/open?id=0B0zQsjKfE5R7YVlOYko2S1ZCNmc

Knock yourself out. 

(I found Code from Electronoobs (Link found in original post), and found the Caliber 50 trucks on Grabcad.com.

I ran some more motor calculations, my target being the ability to drive a 300lb person 30 mph up a 5% grade (yay production criteria!), and it looks like I'll need to run two 2200 watt motors to get the torque. I haven't settled on a cell count, so I haven't picked a Kv either. As of now, It's looking like I'll probably make my own 6S4p pack and a motor around 120 Kv. 

I posted my Math in that folder, so you all can run your own calculations from the excel file. Just Change the green criteria, and everything else will adapt. Weight is in Kg, Diameter is in mm, Grade is in degrees, Volts are in Volts (go figure), and Kv is in whatever the heck Kv is in. 

Does anybody have any experience with Alien Power Systems? I was looking at one of their 5065 motors, and was wondering how long they take to arrive in the U.S. Can't really afford to wait 10 weeks with my schedule. 

I will probably use the VTC6 in my packs, build my own protection circuit, and charging inverter, pending approval from my boss.

Going forward, I will be creating a target production schedule along with design criteria, part spec, and deliverable milestones on certain dates. 

After this summer, i will likely build a second iteration on my own, and it's gonna be shiny af (firefly references ftw).

Also looking into building my own deck, likely with clear grip and racing stripes. I have a lazer cutter, so i can etch a dope design into the bottom, likely something Pink Floyd related. More than open to suggestions! 

Later Today, I will continue to flush out design specs, and will (paycheck pending) order some test parts. I'll also try to make another dent in the second Iteration of CAD. 

Here's a Mock-up of everything i have so far.
<img src="/uploads/db1493/original/3X/7/c/7cebe05ee10d260d7b1cd8cd3a8b85d8be29e5e9.png" width="690" height="388">
<img src="/uploads/db1493/original/3X/6/8/687be51f28681b7183d99e1d3031ce338024c451.png" width="690" height="388">

Truly Yours,

VillainousJ

Afterthoughts: Since I'm targeting 30mph, I should invest in some cool helmets and body armor ;)
```

---
## \#15 Posted by: SilentException Posted at: 2017-06-02T19:35:14.610Z Reads: 312

```
Wow, awesome. Looks like you really thought it through. I especially like the slip ring design, ingenious! And looking at the calculations, low kV and low cell count, it seems like you trust it will push quite a current. Did you do any testing yet?

No experience with Alien here but DIY Electric Skateboards has some, higher kV though. Or maybe search HobbyKing for some SK3 motors.
```

---
## \#16 Posted by: VillainousJackal Posted at: 2017-06-02T20:16:23.934Z Reads: 312

```
@SilentException I've looked at the SK3 motors, and they don't really have the KV I'm looking for. Because the motors will be direct drive, there will be no gearing, so the Kv will directly affect the top speed. 

As for the current, The cells are rated to push that continuously, and even a bit more burst, so everything should be fine there. My biggest concern is the testing of my PWM algorithm, and other high level motor controls. I'll probably run the algorithm on a low amperage motor first, then fine tune it on that scale, before upgrading my MOSFETs and jumping to a bigger motor. Alien is shut down for a few weeks, so i have some dev-time.
```

---
## \#17 Posted by: NickTheDude Posted at: 2017-06-02T22:07:46.279Z Reads: 286

```
You might want to look into rewinding the motor to change the kV. Check this out: https://endless-sphere.com/forums/viewtopic.php?t=36767&f=30
```

---
## \#18 Posted by: SilentException Posted at: 2017-06-02T22:13:34.670Z Reads: 295

```
Yeah, the batteries are solid. I was actually asking about the slip rings and their current transfer capabilities. I really love the design and looking at it, it should work but real world testing is many times a different story :) For example will it handle the rough and the bumps and still provide nice and clean signal for motor. But man, this will be a sweet build, fun times ahead :)
```

---
## \#19 Posted by: Pantologist Posted at: 2017-06-02T23:00:30.762Z Reads: 286

```
Awesome build. I thought arduinos were not well suited to be used as Brushless motor controllers. Can they handle 60k erpm like the VESC?
```

---
## \#20 Posted by: VillainousJackal Posted at: 2017-06-02T23:56:22.683Z Reads: 320

```
@pantologist 
The arduino clocks around 12M Hz, should be more than enough to do the PWM to the FETs. That being said, I haven't done this before! I picked an arduino cause i had one lying around. I checked online and noticed that other people have done it before. Plus i only need to run my motors around 6k.

@Silent Exception, 
Yeah! I'm excited. I'm from a family of 5 engineers, so i have a couple people to bounce ideas off of. I also get a ton of great input from the guys at work. It's a good time to be alive. As for your comment about the slip rings, If you'll refer to the picture of my CAD, those little black pieces are T profile delrin runners with a bolt running through them to the bottom plate, I'm thinking you can tighten them down to keep the top and bottom of the Lazy Susan together.

@NickTheDude
Doesn't Soldering wires together to cut the Kv create a ton of leakage? The fact that one lead will hog most of it also creates a ton of imballance. Beyond that, Don't maxwell's equations play in to create a bunch of eddy currents? I think eddy currents would be one of the last things you'd want in a PM motor. I only skimmed the article, so maybe I'm missing something
```

---
## \#21 Posted by: NickTheDude Posted at: 2017-06-03T00:10:04.303Z Reads: 253

```
No idea. I've just heard that its a common way people reduce the kV of their motors for DIY hub motors.

I believe @The_Dude did it for his motors so he might know what's up.
```

---
## \#22 Posted by: VillainousJackal Posted at: 2017-06-03T00:16:57.800Z Reads: 268

```
Thanks!

So, @The_Dude
It would seem that between finding rugs that pull the room together and watching steve buscemi die on the sidewalk, you solder motors to change their Kv? I'm curious as to whether the Kv drops due to a change in motor characteristics, resulting in an increase in torque, or whether the motor is just less efficient? I would love some input :smile:
```

---
## \#23 Posted by: The_Dude Posted at: 2017-06-03T11:04:54.519Z Reads: 271

```
You got it :sunglasses:
When you convert the motor winding from Delta to Wye the motor kV is reduced by a factor of 1.7.  Additionally the torque increases/is shifted to the lower rpm range.
The is a very thorough description from @Duffman in the german forum available [http://www.elektro-skateboard.de/forum/eigenbauten-95/mbs-pro-90-4x-vesc-ntm5060-12s-4349-2.php](http://www.elektro-skateboard.de/forum/eigenbauten-95/mbs-pro-90-4x-vesc-ntm5060-12s-4349-2.php).
Currently I'm working on a dyno to record the characteristic curves of bldc motors. Doing so, you will know exactly at which rpm the maximum efficiency of you motor is and design your gearing according to that.
```

---
## \#24 Posted by: VillainousJackal Posted at: 2017-06-05T20:56:55.112Z Reads: 314

```
Update 3:

Unfortunately, I spent most of my weekend digging holes and patching sprinkler systems (-_-) so i didn't make quite as much progress recently as i would have liked. However, that doesn't mean i made no progress!

I spent most of my weekend looking at decks. Due to the nature of the conductive slip rings, I need a deck that insulates current, eliminating aluminum and Carbon Fiber. This does leave the classic wood look wide open. I was thinking of doing a 4-5 ply out of either hardened maple or african Mahogany. In any case, I definitely want to do something with racing stripes :sunglasses:
<img src="/uploads/db1493/original/3X/5/5/550efd7efc5ebdb30dee3834fd7875b4e9baabc9.png" width="690" height="436">

I'll probably change my mind back and forth several times before i even begin cutting the deck, but I'm thinking either a red heart or purple heart inlay to make the stripes.

<img src="/uploads/db1493/original/3X/3/8/38411f08dbb8ce5c8cea86a74bfda45423fe205c.png" width="400" height="500">
<img src="/uploads/db1493/original/3X/c/1/c1f486296292a13ae098afb49a9cb1502dbfca15.png" width="406" height="500">

Found both of these pics on pinterest btw. They're not mine. The first is called purple haze, and the second has no notable annotations. Sorry OPs.

Anyway, I'm going to be using the Freebord "Da Blues" wheels, so I'm looking for something that pairs well with their colors. I figure, If it's worth doing, It's worth making it pretty too.
<img src="/uploads/db1493/original/3X/a/f/af187513eb261b15ce00259e30958bc307cab0c8.png" width="500" height="500">

I also did some battery work, Looks like i should be able to package a 8s4p if i use VTC6s. So I cadded for that. In actuality, I'll probably make two different 8s2p packs and just wire them in parallel. Rather than shrinkwrap the pack together, I'll probably just 3D print an enclosure :smile:
<img src="/uploads/db1493/original/3X/9/1/912b7b0a35666e177eb9dd547dba1c4ab65dd928.png" width="690" height="388"> 

Here's what they will look like without their master enclosure mounted on the board. I lined them up opposite eachother so that i can use two ESCs on top of them and run the wires down the according edges, keeping flush to the case. 
<img src="/uploads/db1493/original/3X/7/8/7893d0b5684ee55c9ea315012a2fd8c813ecdbf1.png" width="690" height="388">
<img src="/uploads/db1493/original/3X/f/5/f5a9af0a8657cd2cbe8c7abe6e8451cbcf07777b.png" width="690" height="388">

I also began the process of wire routing, in theory. Due to the fact that the slip rings are actually sunk into the board for stability, I will need to wire leads to them from the top, channeling through the board at an angle, finally connecting to the power electronics at the bottom. This should keep the top pristine and pretty. It may also add some BA circuit board looks :smile: 
<img src="/uploads/db1493/original/3X/f/d/fd0bd1b777a44935de1839f768fef354030766aa.png" width="690" height="388"> 
Grey Lines indicate Wire Routing.


I've been looking at off the shelf parts to drive the motors, And I'm leaning toward writing my own PWM just to prove that i can, then using a pair of VESCs that are Canned together in the final iteration, but that is months off. 

Tomorrow, I will be flushing out the rest of the production cycle in terms of dates and deliverables. Yknow, Setting goals and whatnot. I find that having deadlines pushes me to do better work.

Yours,

A very tired, sunburnt VillainousJ
```

---
## \#25 Posted by: Smorto Posted at: 2017-06-05T21:04:13.032Z Reads: 272

```
Awesome! Just out of curiosity, where do you plan on buying your slip rings from? I might be making an electric freebord my self on of these days so it would be nice to know :slight_smile:.
```

---
## \#26 Posted by: VillainousJackal Posted at: 2017-06-05T23:42:29.377Z Reads: 266

```
I was going to combine them with the lazy Susan's. Current travels through the top ring, into the balls, then onto the bottom pod part, hence the 3 phases. So I'll just lathe them myself. I'll post my final CAD, and then you can cut yours too. Or you can bring the files to a machine shop and they can do it too.
```

---
## \#27 Posted by: Smorto Posted at: 2017-06-06T00:03:35.398Z Reads: 255

```
Awesome, looking forward to seeing it completed!
```

---
## \#28 Posted by: Nowind Posted at: 2017-06-14T10:58:37.423Z Reads: 258

```
Awesome work.
Really nice to see your work on this Buddy.

Running a Leiftech for about 4Weeks now, had to replace most of the parts to get it working good : 
Outer Wheels
Center Wheels
Driveshafts
Pulleys
Batteries
Controller

Actually i was able to fix all bugs by myself.
What i'm affraid for is that the Sliprings fails.... so i really really looking forward to your ideas about that.

Continiue the great work

Hang Loose
Jenso
```

---
## \#29 Posted by: gagahlin Posted at: 2017-07-01T17:26:17.573Z Reads: 244

```
Really Nice. I want to get another e-Freeboard choice. The one that I have only from Leiftech. Really want to try something else.
```

---
## \#30 Posted by: VillainousJackal Posted at: 2017-07-03T20:42:18.167Z Reads: 279

```
Update 4:

How do you do, fellow kids?

I've put a lot of work into the electric freeboard over the last few weeks, so let's jump right in.

<img src="/uploads/db1493/original/3X/3/6/3602ee5aafac2c95099f5ba7fe21754467c0589e.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/6/f/6fc7c16ee331ccf9cd641a3833b4d107c105dc4d.jpg" width="690" height="388">

First, I designed a battery box, which includes mounting for the battery pods, as well as mounting for two VESCs, and routing for the battery bus and wires. Furthermore, it comes in a version that uses heat syncs, and an active cooled version with mounting for 2x 40mm fans. 
<img src="/uploads/db1493/original/3X/5/9/5977e3aa8782b6ece60090ac3da4ddea08bf7216.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/3/c/3c99d4e9bbb54dd9f66c8da35d8e25c894b82731.png" width="690" height="388">
and Vented Version
<img src="/uploads/db1493/original/3X/e/7/e786ace5ddc2398d569019482c481f87a535bc74.png" width="690" height="388">

This brings us to my next development. The choosing of a battery and thermodynamics of heat dissipation. 

I think I'll be going with a 6s5p pack of VTC5As for their middle of the road capacity and relatively low run temp at 20 Amps/cell. 

I also ran some basic differential EQs to calculate the amount of heat i would need to keep the cells at 50* C on an extremely hot summer day (40*C).

I used the data collected by the gentleperson-scholar Mooch over at the E-cigarette forums on various 18650s.
https://www.e-cigarette-forum.com/forum/blog-entry/list-of-battery-tests.7436/

After compiling the data for several different cells, I compared their performance versus heat and weighed several different metrics including safety, capacity, and maximum amperage. 

https://drive.google.com/open?id=0B0zQsjKfE5R7THFzSHlkOVpuZ2s 

The VTC5A runs relatively cool at 20A, (73* C) and has a capacity of a little over 2 Ah. 
6s5p should give us a pack that can push 100 amps continuously, at about 12 Ah. Which is massive. Still working on procuring a spot-welder. 

BUT, 73* C is still a bit too toasty for lithium. We certainly don't want another hoverboard situation on our hands. So, I set out to determine how to dissipate some of that heat. 

Despite my ridiculous spec, i do have several things going for me. The first being that when the batteries are outputting max amperage, the board is moving at max speed, leading to a higher coefficient of ambient convection. Beyond that, I have ample space to fit heatsincs and can always switch to an active cooling system.

I won't bore you with the maths (DM me if you're interested), but all in all, I determined that i could keep the batteries at 50* C with a heatsink surface area of 0.07 m^2.

https://drive.google.com/open?id=0B0zQsjKfE5R7UXE5bkwtUk82cnc

This may sound insane, but it won't actually look too bad. 
<img src="/uploads/db1493/original/3X/3/3/3381663a3faaef898144fffff5b428aa8fd0882e.png" width="690" height="388">
<img src="/uploads/db1493/original/3X/8/9/89685cca03977de6b61736887e825fc0680642f3.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/2/a/2acc85848454bfe93cb8328a58b5f29453aef259.jpg" width="690" height="388">
I should be able to cut it out of aluminum with a plasma cutter and a diamond edged saw on a table saw. It'll heat up like nobodies business during the process, but should turn out fine. 

I also cut the majority of the sliprings, but broke a millbit, so have not been able to finish their features. Preliminary tests look good, as i've been able to run an LED phase to phase, spin the slipring and maintain consistent current through the LED. I plan to validate the design by getting a current sensor on the leads and testing the ripple. 
<img src="/uploads/db1493/original/3X/0/1/01aa32fbe672d2c3c91dbebcb3d9c44fa37ce2e1.jpg" width="666" height="500">
I love it when a plan comes together.

Next up is the board itself. 
<img src="/uploads/db1493/original/3X/5/8/589a05ca1859bea95d3c016146971ca6f501c398.jpg" width="690" height="388">

I've procured some 1/8" Purpleheart, and baltic birtch plywood, and am planning to cut the blanks this week. I have .STEP files of the board blanks themselves, as well as .DXFs of the individual wire routing. 
<img src="/uploads/db1493/original/3X/3/7/37d0802281ff016a3bd0b52c85272f8f2daf367e.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/2/e/2efc933336c6adee8411ab927c38f55079efe039.jpg" width="690" height="388">


In other news, my G3R hanger arrived, and i managed to prototype a mounting system out of wood, soon to be cut out of metal (The Freebord guys actually suggested this on the phone. Thanks Freebord guys). I also ordered the rest of the hardware for the board. 
<img src="/uploads/db1493/original/3X/6/1/615fc0dfdc6013d157cb4bc89fe19f2b395a1aae.jpg" width="666" height="500">

Motors arrived too, and VESCs are on the way. The only thing left to buy is a radio-receiver, batteries, and some 3D printing filament. 

On the coding side of things, I managed to get a motor spinning using basic delays and hall effect sensors, but have not been able to implement PWM, as i burned 2 of my FETs, and am waiting on more. 
<img src="/uploads/db1493/original/3X/7/1/712cf156c9e238917c38746506fc6fa0cfc2da7f.jpg" width="666" height="500">

Turns out the Hall effect sensors are actually super easy to work with.

The Orange, White, and Green wires are all 3-phase signal outputs that switch to high as the magnet passes over the sensor. Furthermore, the red wire is power, and the black is ground (standard convention).

Here's my Code:
https://drive.google.com/open?id=0B0zQsjKfE5R7R1hBdENoNXVhM2c

All in all, this design should be able to push a 300lb rider 25mph up a 10 degree grade in 115* F weather.  Which is absolutely insane.

I think that's it for now. 

This week, i hope to have most of the parts cut, with the exception of the power electronics, and a chassis assembled.

Cordially yours,

VillainousJ
```

---
## \#31 Posted by: Nowind Posted at: 2017-07-04T04:04:30.885Z Reads: 238

```
Super nice Mate.
Straight forward, thanks for the update.
Got the G3 Hangers here by myself, really interrested in your Baseplate solution !

Cheers from Germany
Jenso
```

---
## \#32 Posted by: VillainousJackal Posted at: 2017-07-05T12:51:16.232Z Reads: 246

```
Hi @Nowind, 

I was thinking of doing something like this:
<img src="/uploads/db1493/original/3X/a/9/a94633736272e9aeeb9e8dc6b393fd28ae484197.jpg" width="690" height="388">

The thought is that you cut three pieces out of aluminum, and use the same two side pieces for the different middle pieces. This will allow the adjustment of rock, and easy modifications as to mounting geometry.

For example, if you wanted X inches of rock (i don't know specific numbers as i haven't nailed down other critical dimensions), then you would use a 1/2" lift center. Or if you wanted X+1 inches, you would use a 1+1/2". Pictures attached for reference. 

<img src="/uploads/db1493/original/3X/0/3/03adf03a540b4af07a312d999db2a38bc431017f.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/7/f/7f6a70ab63dde18c1d07cc08c26b04835630f6a6.jpg" width="690" height="388">

The side plates use a common mounting pattern to most longboard trucks, so you should be able to use them on most premade longboard decks. They mount to the center piece via bolts in the XY plane. 

You can prototype too if you like. the only dimension you really need is the angle between face that holds the kingpin bolt, and the pivot cup, which is 150 Degrees. <img src="/uploads/db1493/original/3X/3/2/32f8ff126c87ebb1f0f87dc90cc3fe2a3083f003.png" width="690" height="388">



P.S. I have more parts in the mail from freebord, so i should be able to assemble this mounting concept soon.
```

---
## \#33 Posted by: Maxid Posted at: 2017-07-05T13:08:25.455Z Reads: 221

```
73°C for the batteries would be at constant 20A discharge.
You already said that would equate to 100A continous.
You will never reach those levels - there is no reason for that complicated heatsink design.

[quote="VillainousJackal, post:30, topic:24354, full:true"]
The first being that when the batteries are outputting max amperage, the board is moving at max speed
[/quote]
is also wrong - the top speed is only set by your voltage. You can go full speed with almost zero current if losses are low enough. You will draw current mainly during acceleration - and you won't be just doing stop and go all the time.
```

---
## \#34 Posted by: 1Q-Ford Posted at: 2017-07-05T13:36:28.507Z Reads: 203

```
So very Cool !!! I can't wait to see the end results.
```

---
## \#35 Posted by: VillainousJackal Posted at: 2017-07-05T13:38:13.263Z Reads: 222

```
My thinking is that each of my motors will take 50A a piece (Max spec is 60, but I'll limit that in code), resulting in 100A total. You are correct, that you can go full speed, at almost zero current if you have no load. But the amperage does directly affect torque, and since we live in a real-loaded world, we'll be needing more torque as speed increases, due to the fact that road load increases as well.

After preliminary calculations, and benchmarking commercial products, It looks like my spec will require about a little over 2000 watts per motor. 

My math can be found here: https://drive.google.com/open?id=0B0zQsjKfE5R7dG9ldjhaSnBHSmc

I get that it's counter intuitive to need this much amperage, and if i were designing the board to a lower spec, then i wouldn't need anywhere near that. But, I'm accounting for a high-level of road load including potential grade, wind resistance, and rolling resistance. The spec i was given was insane, basically the purpose of the exercise is to design for a worst case scenario of a 300lb rider, up a 5* Grade, at 25 mph, in 115 degree heat, while maintaining the longevity of the batteries in an optimal temperature range. This means limiting the battery temp to 50 C, which is the the upper end of the happy range of lithium. While they can be run hotter, this decreased battery life fairly significantly.  

I do hope that i made a mistake somewhere as the heatsink will be heavy, and a pain to fabricate, but I've had several other people check my math, and perform the calculations independently, and they all came to the same conclusion.

I realize that my duty cycle is unrealistic, as are my test cases, but these are the specs i was given.
```

---
## \#36 Posted by: VillainousJackal Posted at: 2017-07-05T13:53:46.935Z Reads: 198

```
Oops,

Old Math. 

This is the updated document:
https://drive.google.com/open?id=0B0zQsjKfE5R7dG9ldjhaSnBHSmc
```

---
## \#37 Posted by: Maxid Posted at: 2017-07-05T14:10:50.322Z Reads: 206

```
the shared experiences on this forum show that you need around 10-20Wh per km on average.
Please calculate how much current you'll be drawing on average from this.

Your motor CAN do 60A - but you will rarely do that (or 50A for that matter).
At speed the limiting factor is voltage - not current.

It is good practice to overspec the battery so that it can handle the abuse - but to manufacture cooling solutions on the assumption that you will ride at a constant 2000W is unnecessary.
```

---
## \#38 Posted by: VillainousJackal Posted at: 2017-07-28T13:33:29.605Z Reads: 256

```
Update 5:

Things are happening!

I've frozen design, and started production. Since my last post, some minor design changes occurred. 
<img src="/uploads/db1493/original/3X/9/7/9731d557b198d465c3b2efbdba6b39f4b4c20b7b.png" width="690" height="388">

The most significant is probably the electronics move. In previous design iterations, the electronics were on bottom of the battery box. However, this pretty significantly reduced ground clearance, and left the VESCs vulnerable to impact. So, I moved them to the top of the board, and actually sank them into the deck a bit. They are also covered by a 3D printed enclosure, for safety. <img src="/uploads/db1493/original/3X/c/6/c61ec6f29a6350c128bdbdad7e26e9ddbb3560cb.png" width="690" height="388">

This poses several problems, The primary being 3D printing the Top Shell. Since the 3D printer I'm using doesn't have support structure, there's a high probability that the shell will sag. So, I elected to add support Gussets, for construction.
<img src="/uploads/db1493/original/3X/5/f/5f04f8e20ac65ede27b0e84e40a3ec76dc56f5b3.png" width="690" height="388">
Then, we will 3D print the shell upside down, and cut the gussets off with a razor later.
<img src="/uploads/db1493/original/3X/6/a/6a04cc29bf1ceeeea413bc05ba32d3a26056a4d2.png" width="690" height="388">
Also notice the mounting shelves on the northern and southernmost faces. This is where i will glue magnets, resulting in a fastener free method of holding the shell to the board. 

The next design change is to the battery box.
<img src="/uploads/db1493/original/3X/f/0/f052a7925f1599864ecaa8c583562cbb81b3d4d0.png" width="690" height="388">
The box now features removable doors, allowing access to the batteries for diagnostic and repair. Furthermore, it includes mounting points for the VESCs that will protrude through the top of the board. <img src="/uploads/db1493/original/3X/4/e/4e67a37f69aeac6c92dd3dde5f7182d189598f27.png" width="690" height="388">
Other than that, It's essentially the same.

The other major change is to the wheel pods. 
<img src="/uploads/db1493/original/3X/1/0/10a64b3d3d6fee171a1d30e6bb2264268236e3da.png" width="690" height="388">
I moved away from hub mounted wheels to a more standard, chain drive. I have extensive experience using chain, and prefer it due to it's lower space profile over that of belts. 
<img src="/uploads/db1493/original/3X/e/3/e38cbe40e5b415644690c5b980fb784c49f5a079.png" width="690" height="388">

The axle will be 1/2" steel hex shaft, utilizing hex hubs to mount the motor and a 16t hex gear to drive the motor. The other gear will mount to the shell of the motor, and spin with the outrunner. 

Now, Let's move on to some physical developments!

First, I cut and validated the Lazy Susan Slip Ring. Everything worked surprisingly well!. There is some skipping between the phases, but i hope to remedy this with a diaphragm and polished race tracks. 
<img src="/uploads/db1493/original/3X/6/d/6d907a25ba757e620aa5d187c3386ddc53ee3a54.jpg" width="666" height="500">

Next, I cut the board!
<img src="/uploads/db1493/original/3X/3/1/318dc2381a231fab5622ac404af7aa304765bcf7.png" width="375" height="500">
I'm actually manufacturing two decks, one without inlay, and one with. The board without inlay is cut in it's entirety, and the board with inlay still needs the purpleheart additions, and the holes cut. 
I used a ShopBot to fabricate, Essentially a CNC router. 
<img src="/uploads/db1493/original/3X/9/7/97372d8c50c4c9e4cb0b657dc3104af7307b7978.jpg" width="666" height="500">
I started by setting zero, and cutting the top features. Then, flipping the board with the same zero, and cutting the bottom features.
<img src="/uploads/db1493/original/3X/9/c/9c5607108e4e910fab8c94d9d598019ec4da385f.png" width="375" height="500">
<img src="/uploads/db1493/original/3X/8/1/817694d127e4696a537ef20ac432b861d1797b53.png" width="375" height="500">
<img src="/uploads/db1493/original/3X/4/1/415da784ba0ce635836b7492f82d7ba393926d99.png" width="375" height="500">
<img src="/uploads/db1493/original/3X/b/7/b7c4483108cbb224fd52059d569e4df74c4a380e.png" width="375" height="500">

Cutting Decks has never been so easy!

I also started powder-coating parts. The black looks nice.
<img src="/uploads/db1493/original/3X/d/8/d848e83825f97f0c244bb57b190e2f68c1a94568.png" width="638" height="499">

Up next are the battery packs. My pack will be a 6s5p pack comprising VTC5a 18650s supported by 3D printed runners. 
<img src="/uploads/db1493/original/3X/0/7/07bc8742c20ee8a126d6f3123375e58fe88c65f5.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/9/a/9a97ff781019f150d8cd6a3ed1b18faf7fddebfa.png" width="375" height="500">
I will be custom cutting bus bars out of 1/8" copper, and fastening it using silver-conductive epoxy. 

All in all, things are coming together!

Yours,

VillainousJ
```

---
## \#39 Posted by: Mobutusan Posted at: 2017-07-28T17:54:36.450Z Reads: 240

```
So sick! How much ground clearance will you have under the motors? That seemed to be kind of an issue that @Nowind pointed out in his Leiftech abuse thread. Build looks great so far. 👍
```

---
## \#40 Posted by: VillainousJackal Posted at: 2017-07-28T18:09:49.666Z Reads: 240

```
Should have about 0.75" of ground clearance on the motors... I hadn't heard about that abuse. Something to look into!
```

---
## \#41 Posted by: Mobutusan Posted at: 2017-07-28T18:20:01.672Z Reads: 235

```
Probably the most informative and interesting thread on the interwebs about the Leiftech and it's true performance and issues. Makes me want to find a cheap, broken one, just to upgrade it the way @nowind did.

https://www.electric-skateboard.builders/t/nowinds-first-commercial-board-leiftech-e-snowboard/23571
```

---
## \#42 Posted by: zeno Posted at: 2017-08-19T10:02:50.470Z Reads: 227

```
Any updates? @VillainousJackal
```

---
## \#43 Posted by: johno Posted at: 2017-11-06T18:43:07.270Z Reads: 215

```
Snap @VillainousJackal would be great to hear how this is progressing.
```

---
## \#44 Posted by: VillainousJackal Posted at: 2017-11-06T19:30:37.169Z Reads: 236

```
Hello friends!

My deepest apologies for the delayed update. New semester started and i didn't have much time to work on the board.


Anyway, let's get down to brass tacks. As it stands, the board is about 90% complete. 
<img src="/uploads/db1493/original/3X/b/6/b6b871b2d339f972d40366b6c1ce08592280a90b.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/6/16fced338051e581ca279f9daa98ba1c1f4eb337.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/b/c/bc05736f2fb3253f0960e8e07bc66e1667c79608.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/f/1fba67249c7bc6c1361a06fdf31db19a424c75c3.jpg" width="666" height="500">

Currently, both VESCs are powered and drive, but i'm having trouble getting them to run at the same time. I haven't had the chance to get an oscilliscope on the CAN signal to determine the cause of the problem. However, the pods can be driven, and rotate as they were designed to! This bodes well for the end product. 

On to the build updates.

I ran into several problems during fabrication. The first being with the batteries. I ended up building a VTC5a 6s5p pack capable of pushing 100 amps continuously. In order to carry this current, i custom cut bus bars out of 1/8th copper. However, due to the thickness of the copper, we were unable to spot weld effectively. So, we found an alternative: silver filled epoxy. 
<img src="/uploads/db1493/original/3X/7/1/717a976e26546842e1791c2ec9dea1bab5a4b340.png" 
width="293" height="220">


<img src="/uploads/db1493/original/3X/3/6/360ff1f9b8b4547c308feb287f24dfcca890c4a4.png" width="312" height="234">
<img src="/uploads/db1493/original/3X/4/a/4aa803ed7584699b367e3954a2eb3c95dcad299e.png" width="312" height="234">

This same epoxy was used to mount the balance wires (seen above). After 10 discharge cycles, no issues have been seen thus far. 

I also plasma cut the remainder of the pieces, drilled, tapped, and added other features. Furthermore, every piece was powedercoated, to provide electrical insulation, and for aesthetic appeal. 
<img src="/uploads/db1493/original/3X/b/b/bbb5f1d8ce0db7e2782bd73debdc00d172805dec.png" width="252" height="197">
<img src="/uploads/db1493/original/3X/b/b/bbb5f1d8ce0db7e2782bd73debdc00d172805dec.png" width="252" height="197">
<img src="/uploads/db1493/original/3X/d/2/d2da5cd84471cd308f12cefd4e59953d718eba1e.png" width="293" height="220">
<img src="/uploads/db1493/original/3X/3/7/37f487f6f96c4f0f99fad2808151e7140073a19b.png" width="182" height="242">
<img src="/uploads/db1493/original/3X/2/a/2a41d6133dd1d80e4319af2dc346afee92aab8af.png" width="323" height="242">
<img src="/uploads/db1493/original/3X/1/c/1ca8483c24431ce3f4783adc41ba7617ad390826.png" width="268" height="201">
<img src="/uploads/db1493/original/3X/c/1/c1f7f2d59afc3a145b5931a38dd639924960b12f.png" width="293" height="220">

Wheels were mounted to hex collars using a lathe, and then placed on hex shafts along with corresponding sprockets. 

Really the only thing that remains to be done is to cut the top cover of the deck, mount the foot holds, wire the hall effect sensors to the slip ring from above and below, and cut and mount the chain.

I hope to keep you updated, but likely won't have time to work on it until Christmas break!

Best,

VillainousJ
```

---
## \#45 Posted by: Deckoz Posted at: 2017-11-06T21:57:25.874Z Reads: 213

```
Make sure you have the master vesc with "multiple esc over can" checked on the ppm page, and the slave needs "send status over can" checked on the app page

Master should have an ID of 0, slave an ID of 1 set on the app page next to the "send status over can" checkbox

Build looks amazing.
```

---
## \#46 Posted by: pat.speed Posted at: 2017-11-06T22:09:24.237Z Reads: 209

```
WOW now that we know silver epoxy sticks well beginners that don't have a spot welder could use that to make there 18650 packs
```

---
## \#47 Posted by: notger Posted at: 2017-11-07T10:06:17.505Z Reads: 203

```
[quote="pat.speed, post:46, topic:24354, full:true"]
WOW now that we know silver epoxy sticks well beginners that don't have a spot welder could use that to make there 18650 packs
[/quote]

I'm a bit sceptic if it will stand rough vibrations or even Jumps with the Board ?
```

---
## \#48 Posted by: notger Posted at: 2017-11-07T10:33:17.612Z Reads: 216

```
It looks amazing !!

If you have Time, id have a few Questions.

- Do you plan to "opensource" it or produce it ?

- what Motordiameter are you using 50 or 63mm ?

- It looks like there could be alot of Torque on the Motor-axle having the Sprocket on the unsupported end. I think it would be good to support the Motor Axle on both Ends, this might also be a good way to protect the Motor from possible Rock and cobblestone impacts. Possibly evene with some "fenders"

I have seen really bashed-up Leif-Board Motors, so that would be an amazing "tough-up-date"

<img src="/uploads/db1493/original/3X/9/b/9b7812486f6b03b714fc3fb0ade924e4aa4fb6a0.png" width="666" height="500">

Greets

Notger
```

---
## \#49 Posted by: VillainousJackal Posted at: 2017-11-07T13:32:08.678Z Reads: 210

```
Hello! 

I have no plans to do any sort of production, as all the components cost me upward of $800, and the machining was on the order of 30-40 hours. The price point would be too expensive for people to buy, I think. I can take a crack at updating my CADs and posting them over the next couple months. They won't reflect a bunch of little, on the fly changes i made however, so they won't be anywhere close to "plug and play".

As to your comment about the integrity of the motor mount, I ran the stress equations on the motor shaft and casing, it doesn't look like there will be any problems. If anything, the teeth on the sprocket will shear. 

The motors are 50mm 150kv 2200 watt motors from that one alien website  (the actual name is escaping me at the moment). I agree! Fenders would be cool in later iterations. For now, I'm just trying to get the board moving. 

I'll keep you updated!

-VillainousJ
```

---
## \#50 Posted by: VillainousJackal Posted at: 2017-11-07T13:34:12.600Z Reads: 204

```
Yeah I've tried that. 

For whatever reasons, the VESCs won't hold the flash once I load them. So I can't tell if the settings "stick". 

The alternative is just to build a Y cable from the receiver and just deal with any sync issues from there. 

Thanks for your input!

-VillainousJ
```

---
## \#51 Posted by: notger Posted at: 2017-11-07T18:00:48.423Z Reads: 211

```
[quote="VillainousJackal, post:49, topic:24354"]
I can take a crack at updating my CADs and posting them over the next couple months. They won't reflect a bunch of little, on the fly changes i made however, so they won't be anywhere close to "plug and play".
[/quote]


I'm definitely interested in the CAD files, and i know what you mean, i made the same experiences (not beeing plug and play) with my CAD Projects.

Iwould be interested to see some photos of the Motor-Phase-Copper-tracks, -> how did you design the contactor and the Tracks

greets

Notger
```

---
## \#52 Posted by: VillainousJackal Posted at: 2017-11-14T01:56:51.746Z Reads: 195

```
Notes on Silver Epoxy:

The spec sheet seems to indicate that it has very similar strength characteristics as normal epoxy. So, it should be able to hold up relatively well with a large enough contact patch. Considering it's only holding thin copper bus bars, and the contact patch is the entirety of the 18650 ends, I don't see any issues.
```

---
## \#53 Posted by: pat.speed Posted at: 2017-11-14T11:02:48.419Z Reads: 189

```
What about the specs on current flow? I meant like how much current can it safely carry before getting to hot and possibly melting
```

---
## \#54 Posted by: VillainousJackal Posted at: 2017-12-12T19:22:24.700Z Reads: 190

```
I haven't been able to run the motors under load yet. However, having reviewed the spec sheet, it seems like it has a relatively low impedance. So it should run fairly cool. I think the trick is to have a thin layer over a large contact patch, to minimize resistance. I achieved this by laying down a bead and pressing the cells on one at a time. I'll absolutely keep you posted!
```

---
## \#55 Posted by: VillainousJackal Posted at: 2017-12-12T19:29:03.282Z Reads: 211

```
I'll do my best to get the cad files up sometime soon. As per your track question, I actually didn't use brush style slip rings. Instead i cut tracks in 3 phases of aluminum and am running the current through aluminum ball bearings. Pics seen below. The real trick is to keep all three rings in contact at all times. To accomplish this, i used a compressible medium and a diaphragm, allowing the inner rings to "float" and maintain constant contact. 
<img src="/uploads/db1493/original/3X/7/7/77dd113bac24dd3d14936759854e0370bcea216d.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/a/4/a4b51740358fdb3499e510f44ea09691d7086373.png" width="375" height="500">

The inner slipring is simply to pass the Hall Effect sensor signals to the VESC. Most of the current passes through the lazy susan itself.
```

---
## \#56 Posted by: notger Posted at: 2017-12-12T20:00:29.781Z Reads: 200

```
man, thats genious !!!
```

---
## \#57 Posted by: banjaxxed Posted at: 2017-12-13T12:20:39.116Z Reads: 200

```
This is epic on lots of fronts, the simplest point being the silver expoxy part, if it holds and handles the current it has legs

Care to share the brand and what tests for vibration/ current?
```

---
## \#58 Posted by: VillainousJackal Posted at: 2017-12-13T20:00:15.684Z Reads: 203

```
@notger, @banjaxxed
 
I noticed you have some questions about the silver epoxy!

The product is MG Chemical 8331 Silver Filled Epoxy. I haven't had the opportunity to run any physical tests yet, but the math indicates that i will have no problems with vibration or shock! 

The full data sheet is available here: https://www.mgchemicals.com/downloads/tds/tds-8331-2parts.pdf

Some highlights: 
Impedance: 0.0007 Ohm/Cm
Tensile Strength: 15 N/mm^2
Shear Strength: 1.8 N/mm^2. 
Working Temperature, -67 to 306 F 

Considering the large surface patch on the batteries and the small mass of the bus-bars, I am not worried about losing contact. 

Best,

Villainous J
```

---
## \#59 Posted by: banjaxxed Posted at: 2017-12-13T20:43:59.308Z Reads: 189

```
Wow pricey tube of expoxy! May give it a whirl in the future sometimes thanks for sharing
```

---
## \#60 Posted by: notger Posted at: 2018-02-27T14:52:48.307Z Reads: 172

```
Any Progress ? would love to see some Photos.
```

---
## \#61 Posted by: Elgringo Posted at: 2018-04-11T12:14:43.754Z Reads: 161

```
That is such a fucking asume project!!! I am just figuring out my first project. But sadly what you are Foing is so over my level. Hope you get the time to get your board up and running, and having a blast and feedback to the comunity in how to tune such a fun monster :smile:

 And i really need to start undeatranding the concep of freeboarding. This is so going to be my next project.

Wounder how breaking will work...
```

---
## \#62 Posted by: Nordle Posted at: 2018-04-11T12:34:57.729Z Reads: 157

```
If you want to brake on a freebord, you usually just do slides. That‘s what they are made for, snowboard-like feeling.
```

---
## \#63 Posted by: Elgringo Posted at: 2018-04-13T19:49:11.628Z Reads: 144

```
Makes sence! Probably a to stupide thing to comute, do the you would probably do not want to break with a slide or Carve in tight lanes...
```

---
## \#64 Posted by: ybozorg Posted at: 2018-11-10T20:29:34.641Z Reads: 109

```
Mannnnn this is tiiiiiiiight. That looks like way less maintanance then the pulley motor from leiftech. 30mph will be tiiiiiiiight. I've been sitting here trying to figure out how to convert a freeboard to electric. Looks wayyyyy more complicated then I have the smarts for. I'm a stay posted.
```

---
## \#65 Posted by: Balta_6 Posted at: 2018-12-14T15:21:29.350Z Reads: 91

```
Hello everyone, sorry to dig up that project, but is it going !?
Any feedback ? pictures ?
I want to see everything ;-) !
Cheers all
```

---
## \#66 Posted by: TheRider Posted at: 2019-03-15T03:09:54.208Z Reads: 54

```
Is leifboard patent and can you even make something like this? I would like to see a new improvement... I have a leifboard by the way.
```

---
## \#67 Posted by: TheRider Posted at: 2019-03-15T04:13:03.326Z Reads: 51

```
Is the baseplate for the G3-r hanger done i need a pair.
```

---
